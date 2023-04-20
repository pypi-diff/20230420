# Comparing `tmp/noise2read-0.0.71.tar.gz` & `tmp/noise2read-0.0.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noise2read-0.0.71.tar", last modified: Fri Feb 17 13:19:48 2023, max compression
+gzip compressed data, was "noise2read-0.0.73.tar", last modified: Thu Apr 20 02:54:47 2023, max compression
```

## Comparing `noise2read-0.0.71.tar` & `noise2read-0.0.73.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-02-17 13:19:48.270414 noise2read-0.0.71/
--rw-r--r--   0 pping    (55472) Research  (5010)     1068 2022-08-24 03:12:13.000000 noise2read-0.0.71/LICENSE
--rw-r--r--   0 pping    (55472) Research  (5010)     1052 2023-02-17 13:19:48.272080 noise2read-0.0.71/PKG-INFO
--rw-r--r--   0 pping    (55472) Research  (5010)      633 2023-02-16 01:47:12.000000 noise2read-0.0.71/README.rst
--rw-r--r--   0 pping    (55472) Research  (5010)       90 2022-12-28 02:32:35.000000 noise2read-0.0.71/pyproject.toml
--rw-r--r--   0 pping    (55472) Research  (5010)      950 2023-02-17 13:19:48.276421 noise2read-0.0.71/setup.cfg
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-02-17 13:19:48.108822 noise2read-0.0.71/src/
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-02-17 13:19:48.212022 noise2read-0.0.71/src/noise2read/
--rw-r--r--   0 pping    (55472) Research  (5010)      182 2023-02-17 13:19:13.000000 noise2read-0.0.71/src/noise2read/__init__.py
--rw-r--r--   0 pping    (55472) Research  (5010)    12460 2023-02-16 00:10:03.000000 noise2read-0.0.71/src/noise2read/classifier.py
--rw-r--r--   0 pping    (55472) Research  (5010)    16050 2023-02-16 00:10:21.000000 noise2read-0.0.71/src/noise2read/config.py
--rw-r--r--   0 pping    (55472) Research  (5010)     2701 2023-02-16 00:10:34.000000 noise2read-0.0.71/src/noise2read/coverage.py
--rw-r--r--   0 pping    (55472) Research  (5010)    65198 2023-02-17 13:15:44.000000 noise2read-0.0.71/src/noise2read/data_analysis.py
--rw-r--r--   0 pping    (55472) Research  (5010)    44432 2023-02-16 00:10:55.000000 noise2read-0.0.71/src/noise2read/data_generation.py
--rw-r--r--   0 pping    (55472) Research  (5010)    11181 2023-02-16 00:11:05.000000 noise2read-0.0.71/src/noise2read/data_preprocessing.py
--rw-r--r--   0 pping    (55472) Research  (5010)    29580 2023-02-16 00:11:17.000000 noise2read-0.0.71/src/noise2read/encoding.py
--rw-r--r--   0 pping    (55472) Research  (5010)    30567 2023-02-16 00:11:24.000000 noise2read-0.0.71/src/noise2read/error_orrection.py
--rw-r--r--   0 pping    (55472) Research  (5010)    16773 2023-02-16 00:11:32.000000 noise2read-0.0.71/src/noise2read/isolates_correction.py
--rw-r--r--   0 pping    (55472) Research  (5010)    25668 2023-02-16 00:12:04.000000 noise2read-0.0.71/src/noise2read/noise2read.py
--rw-r--r--   0 pping    (55472) Research  (5010)    34365 2023-02-16 00:11:43.000000 noise2read-0.0.71/src/noise2read/reads2vectors.py
--rw-r--r--   0 pping    (55472) Research  (5010)    12273 2023-02-16 00:11:52.000000 noise2read-0.0.71/src/noise2read/simulation.py
--rw-r--r--   0 pping    (55472) Research  (5010)     3475 2023-02-16 00:12:17.000000 noise2read-0.0.71/src/noise2read/umitest.py
--rw-r--r--   0 pping    (55472) Research  (5010)    15927 2023-02-16 00:12:28.000000 noise2read-0.0.71/src/noise2read/utils.py
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-02-17 13:19:48.245374 noise2read-0.0.71/src/noise2read.egg-info/
--rw-r--r--   0 pping    (55472) Research  (5010)     1052 2023-02-17 13:19:48.000000 noise2read-0.0.71/src/noise2read.egg-info/PKG-INFO
--rw-r--r--   0 pping    (55472) Research  (5010)      851 2023-02-17 13:19:48.000000 noise2read-0.0.71/src/noise2read.egg-info/SOURCES.txt
--rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-02-17 13:19:48.000000 noise2read-0.0.71/src/noise2read.egg-info/dependency_links.txt
--rw-r--r--   0 pping    (55472) Research  (5010)       58 2023-02-17 13:19:48.000000 noise2read-0.0.71/src/noise2read.egg-info/entry_points.txt
--rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-02-16 00:19:13.000000 noise2read-0.0.71/src/noise2read.egg-info/not-zip-safe
--rw-r--r--   0 pping    (55472) Research  (5010)      202 2023-02-17 13:19:48.000000 noise2read-0.0.71/src/noise2read.egg-info/requires.txt
--rw-r--r--   0 pping    (55472) Research  (5010)       11 2023-02-17 13:19:48.000000 noise2read-0.0.71/src/noise2read.egg-info/top_level.txt
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-02-17 13:19:48.265440 noise2read-0.0.71/tests/
--rw-r--r--   0 pping    (55472) Research  (5010)        0 2022-08-24 03:12:14.000000 noise2read-0.0.71/tests/test.py
--rw-r--r--   0 pping    (55472) Research  (5010)     3641 2023-02-16 00:04:36.000000 noise2read-0.0.71/tests/test_data_generation.py
--rw-r--r--   0 pping    (55472) Research  (5010)      985 2023-02-16 00:05:10.000000 noise2read-0.0.71/tests/test_reads2vector.py
--rw-r--r--   0 pping    (55472) Research  (5010)     4216 2023-02-16 00:05:25.000000 noise2read-0.0.71/tests/test_utils.py
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-04-20 02:54:47.503448 noise2read-0.0.73/
+-rw-r--r--   0 pping    (55472) Research  (5010)     1068 2022-08-24 03:12:13.000000 noise2read-0.0.73/LICENSE
+-rw-r--r--   0 pping    (55472) Research  (5010)     1192 2023-04-20 02:54:47.504825 noise2read-0.0.73/PKG-INFO
+-rw-r--r--   0 pping    (55472) Research  (5010)      773 2023-04-20 02:54:36.000000 noise2read-0.0.73/README.rst
+-rw-r--r--   0 pping    (55472) Research  (5010)       90 2022-12-28 02:32:35.000000 noise2read-0.0.73/pyproject.toml
+-rw-r--r--   0 pping    (55472) Research  (5010)      950 2023-04-20 02:54:47.507504 noise2read-0.0.73/setup.cfg
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-04-20 02:54:47.369931 noise2read-0.0.73/src/
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-04-20 02:54:47.452598 noise2read-0.0.73/src/noise2read/
+-rw-r--r--   0 pping    (55472) Research  (5010)      182 2023-04-06 02:41:39.000000 noise2read-0.0.73/src/noise2read/__init__.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    12784 2023-04-07 12:32:06.000000 noise2read-0.0.73/src/noise2read/classifier.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    16050 2023-02-16 00:10:21.000000 noise2read-0.0.73/src/noise2read/config.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     2701 2023-02-16 00:10:34.000000 noise2read-0.0.73/src/noise2read/coverage.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    70175 2023-04-11 07:09:30.000000 noise2read-0.0.73/src/noise2read/data_analysis.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    45177 2023-04-07 11:41:15.000000 noise2read-0.0.73/src/noise2read/data_generation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    11181 2023-02-16 00:11:05.000000 noise2read-0.0.73/src/noise2read/data_preprocessing.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    29580 2023-02-16 00:11:17.000000 noise2read-0.0.73/src/noise2read/encoding.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    30699 2023-04-07 06:44:23.000000 noise2read-0.0.73/src/noise2read/error_orrection.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    16773 2023-02-16 00:11:32.000000 noise2read-0.0.73/src/noise2read/isolates_correction.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    26130 2023-04-05 07:34:22.000000 noise2read-0.0.73/src/noise2read/noise2read.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    34369 2023-04-07 06:47:06.000000 noise2read-0.0.73/src/noise2read/reads2vectors.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    12273 2023-02-16 00:11:52.000000 noise2read-0.0.73/src/noise2read/simulation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     3475 2023-02-16 00:12:17.000000 noise2read-0.0.73/src/noise2read/umitest.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    15905 2023-04-07 07:22:18.000000 noise2read-0.0.73/src/noise2read/utils.py
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-04-20 02:54:47.483018 noise2read-0.0.73/src/noise2read.egg-info/
+-rw-r--r--   0 pping    (55472) Research  (5010)     1192 2023-04-20 02:54:47.000000 noise2read-0.0.73/src/noise2read.egg-info/PKG-INFO
+-rw-r--r--   0 pping    (55472) Research  (5010)      851 2023-04-20 02:54:47.000000 noise2read-0.0.73/src/noise2read.egg-info/SOURCES.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-04-20 02:54:47.000000 noise2read-0.0.73/src/noise2read.egg-info/dependency_links.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)       58 2023-04-20 02:54:47.000000 noise2read-0.0.73/src/noise2read.egg-info/entry_points.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-02-16 00:19:13.000000 noise2read-0.0.73/src/noise2read.egg-info/not-zip-safe
+-rw-r--r--   0 pping    (55472) Research  (5010)      202 2023-04-20 02:54:47.000000 noise2read-0.0.73/src/noise2read.egg-info/requires.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)       11 2023-04-20 02:54:47.000000 noise2read-0.0.73/src/noise2read.egg-info/top_level.txt
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-04-20 02:54:47.499028 noise2read-0.0.73/tests/
+-rw-r--r--   0 pping    (55472) Research  (5010)        0 2022-08-24 03:12:14.000000 noise2read-0.0.73/tests/test.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     3641 2023-02-16 00:04:36.000000 noise2read-0.0.73/tests/test_data_generation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)      985 2023-02-16 00:05:10.000000 noise2read-0.0.73/tests/test_reads2vector.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     4216 2023-02-16 00:05:25.000000 noise2read-0.0.73/tests/test_utils.py
```

### Comparing `noise2read-0.0.71/LICENSE` & `noise2read-0.0.73/LICENSE`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.71/README.rst` & `noise2read-0.0.73/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .. image:: ./logo/logo.svg
    :align: center
 
-noise2read: turn noise to signal in short reads
-===============================================
+Turn 'noise' to signal: accurately rectify millions of erroneous short reads through graph learning on edit distances
+=====================================================================================================================
 
 A novel machine-learning-based error correction algorithm noise2read follows the diversity of the PCR and sequencing process to clear errors in short reads, including DNA and RNA sequencing (DNA/RNA-seq), small RNA, unique molecular identifiers (UMI) and amplicon sequencing data.
 
 Click `noise2read <https://noise2read.readthedocs.io/en/latest/>`__ to jump to noise2read documentation
 =======================================================================================================
```

### Comparing `noise2read-0.0.71/setup.cfg` & `noise2read-0.0.73/setup.cfg`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.71/src/noise2read/classifier.py` & `noise2read-0.0.73/src/noise2read/classifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-02-16 11:01:06
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-02-16 11:10:03
+# @Last Modified time: 2023-04-07 22:31:52
 
 import optuna
 from sklearn.model_selection import train_test_split
 import os
 import xgboost as xgb
 import numpy as np
 # from imblearn.combine import SMOTEENN
@@ -49,15 +49,15 @@
         # self.x_test_weight, self.x_val_weight = train_test_split(test_val_weight, test_size=0.50, random_state=self.config.random_state, shuffle=False)
         # self.logger.debug(type(self.x_val_weight))
         # self.logger.debug(f'{self.x_val}, {self.y_val.shape}, {len(self.x_val_weight)}')
         self.logger.info(f'The number of negative and positive samples: {sorted(collections.Counter(self.y_train).items())}')
 
         sm = SMOTE(random_state=0)
         self.X_resampled, self.y_resampled = sm.fit_resample(self.x_train, self.y_train)
-        self.logger.info(f'After over-sampling {sorted(collections.Counter(self.y_resampled).items())}')
+        self.logger.info(f'After over-sampling: {sorted(collections.Counter(self.y_resampled).items())}')
 
         # rus = RandomUnderSampler(random_state=42)
         # self.X_resampled, self.y_resampled = rus.fit_resample(self.x_train, self.y_train)
         # self.logger.info(f'After under-sampling {sorted(collections.Counter(self.y_resampled).items())}')
 
         # smote_enn = SMOTEENN(random_state=0)
         # self.X_resampled, self.y_resampled = smote_enn.fit_resample(self.x_train, self.y_train)
@@ -144,17 +144,18 @@
         # train_f1 = f1_score(self.y_resampled, xgbc.predict(self.X_resampled))
         train_f1 = f1_score(self.y_train, xgbc.predict(self.x_train))
         test_f1 = f1_score(self.y_test, xgbc.predict(self.x_test))
         
         trial.report(test_accuracy, trial.number)
         if trial.should_prune():
             raise optuna.TrialPruned()
-
-        self.logger.info("Train Accuracy: {}, Test Accuracy: {}".format(train_accuracy, test_accuracy))
-        self.logger.info("Train F1: {}, Test F1: {}".format(train_f1, test_f1))
+        
+        self.logger.info( " Trial " + str(trial.number))
+        self.logger.info("      Train Accuracy: {}, Test Accuracy: {}".format(train_accuracy, test_accuracy))
+        self.logger.info("      Train F1: {}, Test F1: {}".format(train_f1, test_f1))
         trial.set_user_attr(key="best_model", value=xgbc) # save model
 
         # results = xgbc.evals_result()
         # test_logloss = results['validation_1']['logloss']
         # test_auc = results['validation_1']['auc']
         # return test_logloss
         return test_accuracy
@@ -170,17 +171,19 @@
         Returns:
             array: numpy ndarray of shape (n_samples, n_classes)
             Estimated probabilities.
         """
         # study = optuna.create_study(study_name = self.study_name,
         #     pruner=optuna.pruners.MedianPruner(n_warmup_steps=5), direction="maximize" 
         # ) #, interval_steps=10 n_startup_trials=5, 
+        self.logger.info("-------------------------------------------------------------")
         study = optuna.create_study(study_name = self.study_name, direction="maximize")
         study.optimize(self.objective, n_trials, show_progress_bar=False, gc_after_trial=True)
         # print(study.best_trial)
+        
         self.logger.info(f'Study Name: {self.study_name}')
         self.logger.info('Number of finished trials: {}'.format(len(study.trials)))
         self.logger.info('Best trial:')
         best_trial = study.best_trial
         self.logger.info('  Test Accuracy: {}'.format(best_trial.value))
         self.logger.info('  Params: ')
         for key, value in best_trial.params.items():
@@ -188,16 +191,16 @@
 
         # best_trial_copy = copy.deepcopy(best_trial)
 
         # re-evaluate
         # self.objective(best_trial)
         # # # the user attribute is overwritten by re-evaluation
         # assert best_trial.user_attrs != best_trial_copy.user_attrs
-        if best_trial.value < self.config.best_accuracy:
-            self.logger.warning(f"The stduy {self.study_name} output bad best trial accuracy of {best_trial.value}, which may result in bad error correction performance.")
+        # if best_trial.value < self.config.best_accuracy:
+        #     self.logger.warning(f"The stduy {self.study_name} output lower best trial accuracy of {best_trial.value} than the pre-set self.config.best_accuracy, which may result in bad error correction performance.")
         # fig1 = optuna.visualization.plot_optimization_history(study)
         # fig1.write_image(os.path.join(self.config.result_dir, "optimization_history.png"))
 
         # fig2 = optuna.visualization.plot_intermediate_values(study)
         # fig2.write_image(os.path.join(self.config.result_dir, "intermediate_values.png"))
 
         # fig3 = optuna.visualization.plot_parallel_coordinate(study)
@@ -217,10 +220,11 @@
         ax.plot(results['validation_0']['logloss'], label='train')
         ax.plot(results['validation_1']['logloss'], label='test')
         # show the legend
         ax.legend()
         # show the plot
         fig.savefig(os.path.join(self.config.result_dir, self.study_name + '_train-test-logloss.png'))
         predictions = best_model.predict_proba(self.ambi_data)[:, 1]
-
+        
+        self.logger.info("-------------------------------------------------------------")
         del study
         return predictions
```

### Comparing `noise2read-0.0.71/src/noise2read/config.py` & `noise2read-0.0.73/src/noise2read/config.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.71/src/noise2read/coverage.py` & `noise2read-0.0.73/src/noise2read/coverage.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.71/src/noise2read/data_analysis.py` & `noise2read-0.0.73/src/noise2read/data_analysis.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-01-30 09:35:18
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-02-18 00:15:44
+# @Last Modified time: 2023-04-11 17:09:30
 
 from collections import Counter
 import collections
 import math
 from Bio import SeqIO
 import os
 import editdistance
@@ -21,14 +21,16 @@
 import numpy as np
 import math
 import matplotlib.pyplot as plt
 import seaborn as sns
 import matplotlib as mpl
 from matplotlib.colors import ListedColormap, LinearSegmentedColormap
 from random import shuffle
+from tqdm import tqdm
+from mpire import WorkerPool
 
 class DataAnalysis():
     """
     A class to evaluate an error correction method.
     """
     def __init__(self, logger, config):
         """
@@ -36,14 +38,15 @@
 
         Args:
             logger (class): customized logging
             config (class): parameters setting using configparser
         """
         self.logger = logger
         self.config = config
+        self.logger.info("-------------------------------------------------------------")
         self.logger.info(f'Raw dataset: {config.input_file}')
         self.logger.info(f'Correct dataset: {config.correct_data}')
         self.logger.info(f'Ground truth dataset: {config.ground_truth_data}')
         if os.path.exists(self.config.result_dir):
             self.logger.info("Directory '% s' already exists" % self.config.result_dir)
             # for f in os.listdir(self.config.result_dir):
             #     os.remove(os.path.join(self.config.result_dir, f))
@@ -96,24 +99,46 @@
         correct_record_iterator, correct_file_tye = parse_data(self.config.correct_data)
         raw_seqs = []
         correct_seqs = []
 
         self.raw_len2seqs_dict = {}
         self.raw_len_lst = []
         total_reads_num = 0
+        
+        raw_record_dict = {}
+        correct_record_dict = {}
+        id_lst = []
         for raw_item, correct_item in zip(raw_record_iterator, correct_record_iterator):
+            raw_id = str(raw_item.id)
             raw_seq = str(raw_item.seq)
+
+            cor_id = str(correct_item.id)
+            cor_seq = str(correct_item.seq)
+            
             raw_seqs.append(raw_seq)
-            correct_seqs.append(str(correct_item.seq))
+            correct_seqs.append(cor_seq)
             
             ll = len(raw_seq)
             self.raw_len_lst.append(ll)
             self.raw_len2seqs_dict.setdefault(ll, []).append(raw_seq)
             total_reads_num += 1
+            
+            raw_record_dict[raw_id] = raw_seq
+            correct_record_dict[cor_id] = cor_seq
+            
+            id_lst.append(raw_id)
+
+        corrected_reads_num = 0
 
+        for item in tqdm(id_lst):
+            ori_read = raw_record_dict[item]
+            cor_read = correct_record_dict[item]
+            if str(cor_read) != str(ori_read):
+                corrected_reads_num += 1
+                
         raw_read2count = Counter(raw_seqs)
         correct_read2count = Counter(correct_seqs)
 
         raw_read2count_val_lst = list(raw_read2count.values())
         raw_read2count_val_lst.sort(reverse=True)
 
         correct_read2count_val_lst = list(correct_read2count.values())
@@ -149,14 +174,18 @@
             raw_rank = self.ranking(raw_read_count, raw_read2count_val_lst)
             worksheet.write(row, col + 5, raw_rank)
             row += 1
 
         self.logger.debug(f'Ground truth: {self.config.ground_truth_data}')
         if self.config.ground_truth_data:
             self.evaluation_with_groundtruth()
+        self.logger.info("corrected {} reads out of {} ({:.6f}) reads".format(corrected_reads_num, total_reads_num, corrected_reads_num/total_reads_num))
+        raw_unique_num = len(raw_read2count)
+        correct_unique_num = len(correct_read2count)
+        self.logger.info("Unique reads decreased by {} from {} to {} ({:.6f}) reads".format(raw_unique_num - correct_unique_num, raw_unique_num, correct_unique_num, (raw_unique_num - correct_unique_num)/raw_unique_num))
         # no ground truth entropy
         self.evaluation_without_groundtruth(raw_read2count, correct_read2count, total_reads_num)
         return
 
     # rely on read frequency instead of sequecing id
     def evaluation_with_groundtruth(self):
         """
@@ -337,15 +366,15 @@
                 read_level['fn'] += cor_positive_reads  
             if total_negative_reads >= cor_negative_reads:
                 read_level['tn'] += cor_negative_reads
                 read_level['fp'] += total_negative_reads - cor_negative_reads  
             if total_positive_reads < cor_positive_reads:
                 read_level['tp'] += 0
                 read_level['fn'] += total_positive_reads
-                self.logger.warning(f'Read-level Evaluation: introduced additional {cor_positive_reads - total_positive_reads} positive reads after correction for UMI {str(umi)}') 
+                # self.logger.warning(f'Read-level Evaluation: introduced additional {cor_positive_reads - total_positive_reads} positive reads after correction for UMI {str(umi)}') 
             if total_negative_reads < cor_negative_reads:
                 read_level['tn'] += total_negative_reads
                 read_level['fp'] += 0
                 # self.logger.warning(f'Read-level Evaluation: introduced additional {cor_negative_reads - total_negative_reads} negative reads after correction for UMI {str(umi)}') 
 
             ## fn
             raw_positive_seqs = set(raw_seqs) - set(true_seqs)
@@ -438,14 +467,16 @@
         # correctset_entropy_noTruth = self.read_counts_entropy(correct_read2count, total_reads_num)
         # self.save_entropy('ReadCountEntropy', rawset_entropy_noTruth, correctset_entropy_noTruth) 
 
         # entropy = self.noise2signal_entropy(raw_read2count, correct_read2count, total_reads_num)
         entropy = self.noise2read_entropy(raw_read2count, correct_read2count, total_reads_num)
         # self.save_entropy('Entropy H', entropy[0], entropy[1]) 
         self.logger.info("{}: raw dataset entropy: {}, correct dataset entropy: {}".format('Entropy H', entropy[0], entropy[1]))
+        self.logger.info("Information Gain: {}".format(entropy[0] - entropy[1]))
+        
         worksheet3 = self.workbook_flie.add_worksheet('Non-frequent Entropy')
         worksheet3.write('A1', 'H')
         worksheet3.write('A2', entropy[0])
         worksheet3.write('B1', "H'")
         worksheet3.write('B2', entropy[1]) 
         worksheet3.write('C1', '\u0394 H')
         worksheet3.write('C2', entropy[0] - entropy[1]) 
@@ -587,19 +618,18 @@
         cbar.cmap.set_under('red')
         # cbar.cmap.set_over('red')
         fig.tight_layout()
         fig.savefig(os.path.join(self.config.result_dir, self.prefix + '_information_gain.png'), transparent=True)
 
         return
 
-    def entropy_item(self, shared_vars, freq):
-        total_freq, n = shared_vars
+    def entropy_item(self, total_freq, freq):
         if freq > 0:
             p = freq / total_freq
-            result = - p * math.log2(p)/ math.log2(n)
+            result = - p * math.log2(p)
         return result
 
     def noise2read_entropy(self, raw_read2count, correct_read2count, total_num):
 
         raw_unique_reads = set(raw_read2count.keys())
         correct_unique_reads = set(correct_read2count.keys())
 
@@ -609,33 +639,28 @@
         non_frequent_raw_reads = raw_unique_reads - frequent_reads
         raw_entropy_items = []
         for read in non_frequent_raw_reads:
             raw_entropy_items.append(raw_read2count[read])
 
         raw_nonFre_reads_total_num = sum(raw_entropy_items)
         # raw entropy
-        raw_unique_num = len(non_frequent_raw_reads)
-        shared_vars1 = raw_nonFre_reads_total_num, raw_unique_num
-        with WorkerPool(self.config.num_workers, shared_objects=shared_vars1, start_method='fork') as pool:
+        with WorkerPool(self.config.num_workers, shared_objects=raw_nonFre_reads_total_num, start_method='fork') as pool:
             raw_entropy_lst = pool.map(self.entropy_item, raw_entropy_items)
         raw_entropy = sum(raw_entropy_lst) 
 
         # correct dateset
         non_frequent_correct_reads = correct_unique_reads - frequent_reads
         correct_entropy_items = []
         for read in non_frequent_correct_reads:
             correct_entropy_items.append(correct_read2count[read])
 
         # correct entropy
         correct_nonFre_reads_total_num = sum(correct_entropy_items)
 
-        correct_unique_num = len(non_frequent_correct_reads)
-        shared_vars2 = correct_nonFre_reads_total_num, correct_unique_num
-
-        with WorkerPool(self.config.num_workers, shared_objects=shared_vars2, start_method='fork') as pool:
+        with WorkerPool(self.config.num_workers, shared_objects=correct_nonFre_reads_total_num, start_method='fork') as pool:
             correct_entropy_lst = pool.map(self.entropy_item, correct_entropy_items) 
         correct_entropy = sum(correct_entropy_lst)
         ##################################################################################
         #information gain (\delta I) heatmap
         new_reads = correct_unique_reads - raw_unique_reads
         new_reads_num = len(new_reads)
         self.logger.info("Wrongly introduced {} new reads".format(new_reads_num))
@@ -643,34 +668,26 @@
         raw_kept_counts = []
         correct_kept_counts = []
         kept_reads = correct_unique_reads & raw_unique_reads
         for read in kept_reads:
             correct_kept_counts.append(correct_read2count[read])
             raw_kept_counts.append(raw_read2count[read])
 
-        raw_kept_total_num = sum(raw_kept_counts)
-
-        unique_kept_reads_num = len(kept_reads)
-        shared_vars3 = raw_kept_total_num, unique_kept_reads_num
-        with WorkerPool(self.config.num_workers, shared_objects=shared_vars3, start_method='fork') as pool:
+        with WorkerPool(self.config.num_workers, shared_objects=total_num, start_method='fork') as pool:
             raw_kept_entropy_lst = pool.map(self.entropy_item, raw_kept_counts)
 
-        correct_kept_total_num = sum(correct_kept_counts)
-        shared_vars4 = correct_kept_total_num, unique_kept_reads_num
-        with WorkerPool(self.config.num_workers, shared_objects=shared_vars4, start_method='fork') as pool:
+        with WorkerPool(self.config.num_workers, shared_objects=total_num, start_method='fork') as pool:
             correct_kept_entropy_lst = pool.map(self.entropy_item, correct_kept_counts) 
 
         raw_removed_reads = raw_unique_reads - correct_unique_reads
         raw_removed_items = []
         for read in raw_removed_reads:
             raw_removed_items.append(raw_read2count[read])
-        removed_total_num = sum(raw_removed_items)
-        unique_removed_num = len(raw_removed_reads)
-        shared_vars5 = removed_total_num, unique_removed_num
-        with WorkerPool(self.config.num_workers, shared_objects=shared_vars5, start_method='fork') as pool:
+
+        with WorkerPool(self.config.num_workers, shared_objects=total_num, start_method='fork') as pool:
             raw_removed_entropy_items_lst = pool.map(self.entropy_item, raw_removed_items)
         for i in raw_removed_entropy_items_lst:
             if i <=0:
                 print('Warning')
         entropy_item_lst = []
         for i, j in zip(raw_kept_entropy_lst, correct_kept_entropy_lst):
             entropy_item_lst.append(i - j)
@@ -1450,8 +1467,102 @@
 
     def entropy_item(self, shared_vars, freq):
         total_freq, n, delta = shared_vars
         if freq > 0:
             p = freq / total_freq
             result = - delta * (p * math.log2(p)/ math.log2(n))
         return result
+
+
+    def entropy_item(self, shared_vars, freq):
+        total_freq, n = shared_vars
+        if freq > 0:
+            p = freq / total_freq
+            # result = - p * math.log2(p) / math.log2(n)
+            result = - p * math.log2(p)
+        return result
+
+    def noise2read_entropy(self, raw_read2count, correct_read2count, total_num):
+
+        raw_unique_reads = set(raw_read2count.keys())
+        correct_unique_reads = set(correct_read2count.keys())
+
+        frequent_reads = set([k for k, v in raw_read2count.items() if v > self.config.high_freq_thre])
+
+        # raw dataset
+        non_frequent_raw_reads = raw_unique_reads - frequent_reads
+        raw_entropy_items = []
+        for read in non_frequent_raw_reads:
+            raw_entropy_items.append(raw_read2count[read])
+
+        raw_nonFre_reads_total_num = sum(raw_entropy_items)
+        # raw entropy
+        non_frequent_raw_unique_num = len(non_frequent_raw_reads)
+
+        shared_vars1 = raw_nonFre_reads_total_num, non_frequent_raw_unique_num
+        with WorkerPool(self.config.num_workers, shared_objects=shared_vars1, start_method='fork') as pool:
+            raw_entropy_lst = pool.map(self.entropy_item, raw_entropy_items)
+        raw_entropy = sum(raw_entropy_lst) 
+
+        # correct dateset
+        non_frequent_correct_reads = correct_unique_reads - frequent_reads
+        correct_entropy_items = []
+        for read in non_frequent_correct_reads:
+            correct_entropy_items.append(correct_read2count[read])
+
+        # correct entropy
+        correct_nonFre_reads_total_num = sum(correct_entropy_items)
+
+        # correct_unique_num = len(non_frequent_correct_reads)
+        shared_vars2 = correct_nonFre_reads_total_num, non_frequent_raw_unique_num
+
+        with WorkerPool(self.config.num_workers, shared_objects=shared_vars2, start_method='fork') as pool:
+            correct_entropy_lst = pool.map(self.entropy_item, correct_entropy_items) 
+        correct_entropy = sum(correct_entropy_lst)
+        ##################################################################################
+        #information gain (\delta I) heatmap
+        new_reads = correct_unique_reads - raw_unique_reads
+        new_reads_num = len(new_reads)
+        self.logger.info("Wrongly introduced {} new reads".format(new_reads_num))
+
+        raw_kept_counts = []
+        correct_kept_counts = []
+        kept_reads = correct_unique_reads & raw_unique_reads
+        for read in kept_reads:
+            correct_kept_counts.append(correct_read2count[read])
+            raw_kept_counts.append(raw_read2count[read])
+
+        # unique_kept_reads_num = len(kept_reads)
+        raw_unique_num = len(raw_unique_reads)
+        shared_vars3 = total_num, raw_unique_num
+        with WorkerPool(self.config.num_workers, shared_objects=shared_vars3, start_method='fork') as pool:
+            raw_kept_entropy_lst = pool.map(self.entropy_item, raw_kept_counts)
+
+        correct_kept_total_num = sum(correct_kept_counts)
+        # shared_vars4 = correct_kept_total_num, unique_kept_reads_num
+        shared_vars4 = total_num, raw_unique_num
+        with WorkerPool(self.config.num_workers, shared_objects=shared_vars4, start_method='fork') as pool:
+            correct_kept_entropy_lst = pool.map(self.entropy_item, correct_kept_counts) 
+
+        raw_removed_reads = raw_unique_reads - correct_unique_reads
+        raw_removed_items = []
+        for read in raw_removed_reads:
+            raw_removed_items.append(raw_read2count[read])
+        # removed_total_num = sum(raw_removed_items)
+        # unique_removed_num = len(raw_removed_reads)
+        shared_vars5 = total_num, raw_unique_num
+        with WorkerPool(self.config.num_workers, shared_objects=shared_vars5, start_method='fork') as pool:
+            raw_removed_entropy_items_lst = pool.map(self.entropy_item, raw_removed_items)
+        for i in raw_removed_entropy_items_lst:
+            if i <=0:
+                print('Warning')
+        entropy_item_lst = []
+        for i, j in zip(raw_kept_entropy_lst, correct_kept_entropy_lst):
+            entropy_item_lst.append(i - j)
+        entropy_item_lst.extend(raw_removed_entropy_items_lst)
+        if new_reads_num > 0:
+            entropy_item_lst.extend([np.nan] * new_reads_num)
+        shuffle(entropy_item_lst)
+        self.gain2heatmap(entropy_item_lst)
+        return [raw_entropy, correct_entropy]
+
     '''
```

### Comparing `noise2read-0.0.71/src/noise2read/data_generation.py` & `noise2read-0.0.73/src/noise2read/data_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-01-16 15:52:44
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-02-16 11:10:55
+# @Last Modified time: 2023-04-07 21:41:15
 
 import editdistance
 import networkx as nx
 import os
 import csv
 from tqdm import tqdm
 from noise2read.utils import *
@@ -266,20 +266,21 @@
             ambiguous_csv = self.config.result_dir + "ambiguous2.csv"  
 
         genuine_lst = []
         ambiguous_lst = []
         subgraph_num = len(subgraphs)
         shared_obs = subgraphs, edit_dis
         idx = 0
+        self.logger.info("Extracting genuine and ambiguous errors...")
         with WorkerPool(self.config.num_workers, shared_objects=shared_obs, start_method='fork') as pool:
             for genu_ambi_lst in pool.imap(self.extract_genuine_ambi_errs_subgraph, range(subgraph_num), progress_bar=self.config.verbose):
                 if genu_ambi_lst[0]:
                     genuine_lst.extend(genu_ambi_lst[0])
                     ambiguous_lst.extend(genu_ambi_lst[1])
-                    
+        self.logger.info("Extraction done.")                    
         # with WorkerPool(self.config.num_workers, shared_objects=shared_obs, start_method='fork') as pool:
         #     with tqdm(total=subgraph_num, desc=self.logger.info("Extract samples with genuine errors"), miniters=int(subgraph_num/self.config.min_iters)) as pbar:   
         #         for genu_ambi_lst in pool.imap(self.extract_genuine_ambi_errs_subgraph, range(subgraph_num)):
         #             if genu_ambi_lst[0]:
         #                 genuine_lst.extend(genu_ambi_lst[0])
         #                 ambiguous_lst.extend(genu_ambi_lst[1])
         #             pbar.update()
@@ -416,14 +417,16 @@
         Args:
             edit_dis (int): set edit distance 1 or 2 to search edges for constructing graph
 
         Returns:
             MultiVariables: MultiVariables for next step error correction
         """
         # 1nt-edit-distance-based graph
+        self.logger.info("-------------------------------------------------------------")
+        self.logger.info("1nt-edit-distance read graph error correction")
         graph, seqs_lens_lst, seqs2id_dict, unique_seqs = self.generate_graph(self.config.input_file, edit_dis)
         seq_max_len = max(seqs_lens_lst)
         seq_min_len = min(seqs_lens_lst)
         self.logger.debug(seqs_lens_lst)
         self.logger.debug("Reads Max length: {}".format(seq_max_len))
         self.logger.debug("Reads Min length: {}".format(seq_min_len))
         if edit_dis == 1 and self.config.high_ambiguous:
@@ -445,14 +448,15 @@
         Args:
             graph (object): A graph constructed using NetworkX.
             edit_dis (int): set edit distance 1 or 2 to search edges for constructing graph
 
         Returns:
             DataFrame: one pandas dataframe saving isolated high frequency reads
         """
+        self.logger.info("Extracting negative samples...")
         if not nx.is_connected(graph):
             self.logger.debug("G is a connected graph: {}".format(nx.is_connected(graph)))
             isolates = set(list(nx.isolates(graph)))        
         else:
             self.logger.debug("G is a connected graph: {}".format(nx.is_connected(graph)) )
 
         self.logger.debug("Isolated Nodes Number: {}".format(len(isolates)))
@@ -466,28 +470,30 @@
             k_count = graph.nodes[k]['count']
             if k_count >= self.config.high_freq_thre:
                 k_degree = graph.degree[k]
                 line = [k, k_count, k_degree]
                 negative_df.loc[len(negative_df)] = line  
         if self.config.verbose:
             negative_df.to_csv(negative_csv, index=False) 
+        self.logger.info("Extraction done!")
         return negative_df
 
     def extract_isolates(self, graph, unique_seqs, seqs2id_dict):
         """
         split the source file into two files of isolates and non-isolates based on constructed graph
 
         Args:
             graph (object): A graph constructed using NetworkX.
             unique_seqs (list): All the unique reads in the dataset
             seqs2id_dict (dict): key: read, id: sequencing id
 
         Returns:
             files: two files of isolates and non-isolates based on constructed graph
         """
+        self.logger.info("Extracting isolated nodes.")
         if not nx.is_connected(graph):
             self.logger.debug("G is a connected graph: {}".format(nx.is_connected(graph)))
             isolates = set(list(nx.isolates(graph)))
         else:
             self.logger.debug("G is a connected graph: {}".format(nx.is_connected(graph)) )
 
         self.logger.debug("Isolated Nodes Number: {}".format(len(isolates)))
@@ -514,15 +520,15 @@
         elif self.file_type == 'fasta' or self.file_type == 'fa' or self.file_type == 'fasta.gz' or self.file_type == 'fas.gz':
             isolates_file = self.config.result_dir + base[0] + '_isolates.fasta'
             non_isolates_file = self.config.result_dir + base[0] + '_non_isolates.fasta' 
 
         extract_records(self.config.result_dir, name_lst, self.config.input_file, isolates_file)
         extract_records(self.config.result_dir, non_name_lst, self.config.input_file, non_isolates_file)
 
-        self.logger.info("Isolated nodes extraction completed.")
+        self.logger.info("Extraction done.")
         return isolates_file, non_isolates_file
 
     def generate_graph(self, data_set, edit_dis):
         """
         construct 1nt- or 2nt-edit-distance-based read graph
 
         Args:
@@ -532,16 +538,15 @@
         Returns:
             MultiVariables: Multi Variables after constructing edit-distance-based read graph
         """
         # if not os.path.exists(data_set):
         #     self.logger.error("No input file!")
         #     # os._exit(0)
         # else:
-        self.logger.info(data_set)
-
+        self.logger.info("Input dataset '% s'" % data_set)
         record_iterator, file_type = parse_data(data_set)
         seqs2id_dict = {}
         total_seqs = []
         seq_lens_set = set()
         for item in record_iterator:
             seq = str(item.seq)
             ll = len(seq)
@@ -550,32 +555,35 @@
             seqs2id_dict.setdefault(seq, []).append(str(item.id))
         unique_seqs = set(total_seqs)
 
         graph = nx.Graph()
         read_count = Counter(total_seqs)
         high_freq = []
         low_freq = []
-        for read, frequency in tqdm(read_count.items(), desc=self.logger.info("Read Counts"), miniters=int(len(read_count)/self.config.min_iters)):
+
+        for read, frequency in tqdm(read_count.items(), desc=self.logger.info("Adding nodes to " + str(edit_dis) + "-edit-distance read graph..."), miniters=int(len(read_count)/self.config.min_iters)):
             if not graph.has_node(read):
                 graph.add_node(read, count = frequency, flag=False)  
             if frequency >= self.config.high_freq_thre:
                 high_freq.append(read)
             else:
                 low_freq.append(read)
         if len(high_freq) == 0:
             self.logger.error("Error Correction Failed as no high-frequency reads detected.")
             sys.exit(1)
         self.logger.debug(len(read_count))
+
         ######################################################
         edges_lst = []
         if edit_dis == 1:
             shared_unique_seqs = unique_seqs
         elif edit_dis == 2:
             shared_unique_seqs = low_freq
-
+        
+        self.logger.info("Searching edges for constructing " + str(edit_dis) + "-edit-distance read graph...")
         with WorkerPool(self.config.num_workers, shared_objects=shared_unique_seqs, start_method='fork') as pool:
             if edit_dis == 1:
                 for edge_lst in pool.imap(self.real_ed1_seqs, high_freq, progress_bar=self.config.verbose):
                     edges_lst.extend(edge_lst)
             elif edit_dis == 2:
                 for edge_lst in pool.imap(self.real_ed2_seqs, high_freq, progress_bar=self.config.verbose):
                     edges_lst.extend(edge_lst)
@@ -590,15 +598,15 @@
         #             for edge_lst in pool.imap(self.real_ed2_seqs, high_freq):
         #                 edges_lst.extend(edge_lst)
         #                 pbar.update()
         if len(edges_lst) > 0:
             self.logger.debug(len(edges_lst))
             self.logger.debug(edges_lst[0])
             graph.add_edges_from(edges_lst)
-
+        self.logger.info(str(edit_dis) + "-edit-distance read graph construction finished.")
         ########################################################
         # save graphs
         if self.config.graph_visualization or self.config.save_graph:
             if edit_dis == 1:
                 subdir = self.config.result_dir + "graph1/"                
             elif edit_dis == 2:
                 subdir = self.config.result_dir + "graph2/"
@@ -762,15 +770,15 @@
             subgraphs (class): Subgraphs of graph constructed using NetworkX.
 
         Returns:
             DataFrame: One pandas dataframe saving high ambiguous errors
         """
         high_ambiguous_df = pd.DataFrame(columns=["idx", "StartRead", "StartReadCount", "StartDegree", "ErrorTye","ErrorPosition", "StartErrKmer", "EndErrKmer", "EndRead", "EndReadCount", "EndDegree"])
         idx = 0
-        for s in tqdm(subgraphs, desc=self.logger.info("Extract samples of high ambiguous errors from 1nt-edit-distance graph"), miniters=int(len(subgraphs)/self.config.min_iters)):
+        for s in tqdm(subgraphs, desc=self.logger.info("Extracting high ambiguous errors from 1nt-edit-distance graph"), miniters=int(len(subgraphs)/self.config.min_iters)):
             edges_lst = [e for e in s.edges()]
             if len(edges_lst) > 0:
                 for (a, b) in edges_lst:
                     a_count = s.nodes[a]['count']
                     b_count = s.nodes[b]['count']
                     a_degree = s.degree[a]
                     b_degree = s.degree[b]
@@ -784,14 +792,15 @@
                         new_b2a.insert(0, idx)
                         high_ambiguous_df.loc[len(high_ambiguous_df)] = new_b2a
                         idx += 1
             del edges_lst
         if self.config.verbose:
             high_ambiguous_csv = self.config.result_dir + "high_ambiguous_1nt.csv"
             high_ambiguous_df.to_csv(high_ambiguous_csv, index=False)  
+        self.logger.info("Extraction done!")
         return high_ambiguous_df
 
 '''
     def extract_genuine_ambi_errs(self, subgraphs, edit_dis):
         """
         extract genuine and ambiguous errors from read graph
```

### Comparing `noise2read-0.0.71/src/noise2read/data_preprocessing.py` & `noise2read-0.0.73/src/noise2read/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.71/src/noise2read/encoding.py` & `noise2read-0.0.73/src/noise2read/encoding.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.71/src/noise2read/error_orrection.py` & `noise2read-0.0.73/src/noise2read/error_orrection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-02-16 11:01:06
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-02-16 11:11:24
+# @Last Modified time: 2023-04-07 16:44:23
 
 import os
 from Bio import SeqIO
 import pandas as pd
 from Bio.Seq import Seq
 from Bio.SeqRecord import SeqRecord
 from noise2read.isolates_correction import IsolatesErrorCorrection
@@ -58,29 +58,32 @@
                 new_negative_df: pandas dataframe containing negative samples from the prediction result of ambiguous errors
         """
         corrected_file = self.config.result_dir + self.base[0] + '_corrected.' + self.out_file_tye  
         if isinstance(high_ambiguous_df, pd.DataFrame):
             genuine_ambi_errs_df, new_negative_df, high_ambi_df = self.all_in_one_ambiguous_err_prediction(unique_seqs, genuine_df, negative_df, ambiguous_df, high_ambiguous_df, edit_dis=1)
             # correct errors
             genuine_corrected_file = self.correct_errors(non_isolates_file, genuine_ambi_errs_df)
-            self.logger.info("1nt-edit-distance based genuine and ambiguous errors corrected.")
+            self.logger.info("Genuine and ambiguous errors corrected.")
+            
             del genuine_ambi_errs_df, genuine_df, negative_df, ambiguous_df, unique_seqs
             ###############################################################################################
             # IEC = IsolatesErrorCorrection(self.logger, self.config.num_workers, isolates_file, genuine_corrected_file, self.config.result_dir, self.config.iso_change_detail, self.config.min_iters)
             # tmp_corrected_isolates = IEC.bcool_correct_isolates() 
             # tmp_correct = self.config.result_dir + self.base[0] + '_correct_no_high.' + self.out_file_tye  
             # if tmp_corrected_isolates and genuine_corrected_file:
             #     os.system("cat %s %s > %s" % (tmp_corrected_isolates, genuine_corrected_file, tmp_correct))
             # # if os.path.exists(tmp_corrected_isolates):     
             # #     os.system("rm %s" % tmp_corrected_isolates)
             # del IEC
             #####################################################################
             non_isolates_correct = self.all_in_one_high_ambiguous_err_correction(genuine_corrected_file, high_ambi_df)
             del high_ambiguous_df
+            self.logger.info("High ambiguous errors corrected.")
             self.logger.info('1nt-edit-distance based Errors Correction finished.')
+            self.logger.info("#############################################")
         else:
             genuine_ambi_errs_df, new_negative_df = self.all_in_one_ambiguous_err_prediction(unique_seqs, genuine_df, negative_df, ambiguous_df, high_ambiguous_df=None, edit_dis=1)
             # correct errors
             self.logger.info("Correcting 1nt-edit-distance based Errors")
 
             non_isolates_correct = self.correct_errors(non_isolates_file, genuine_ambi_errs_df)
             self.logger.info('1nt-edit-distance based Errors Correction Finished')
```

### Comparing `noise2read-0.0.71/src/noise2read/isolates_correction.py` & `noise2read-0.0.73/src/noise2read/isolates_correction.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.71/src/noise2read/noise2read.py` & `noise2read-0.0.73/src/noise2read/noise2read.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,53 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2022-12-29 23:04:12
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-02-16 11:12:04
+# @Last Modified time: 2023-04-05 17:34:22
 
 from noise2read.config import Config
 import sys, getopt
 from noise2read.data_generation import DataGneration
 from noise2read.error_orrection import ErrorCorrection
 from noise2read.data_analysis import DataAnalysis
 import os
 from noise2read.simulation import Simulation
 from noise2read.utils import custom_logger, usage
 from noise2read.data_preprocessing import DataProcessing
+from contextlib import redirect_stdout
 
 def main():
     argv = sys.argv[1:]
     # create logger
     logger = custom_logger("noise2read", debug_mode=False)
+
     ##############################################################
     try:
         # opts, args = getopt.getopt(argv, "m:c:i:u:t:r:d:p:a:g:o:l:h:", ["module=", "config=", "input=", "umi_file", "true", "rectification", "directory", "parallel", "high_ambiguous", "tree_method", "over_sampling", "libray_layout", "help"]) 
-        opts, args = getopt.getopt(argv, "m:c:i:u:t:r:d:p:a:g:l:h:", ["module=", "config=", "input=", "umi_file", "true", "rectification", "directory", "parallel", "high_ambiguous", "tree_method", "libray_layout", "help"]) 
+        opts, args = getopt.getopt(argv, "m:c:i:u:t:r:d:p:a:g:l:h", ["module=", "config=", "input=", "umi_file", "true", "rectification", "directory", "parallel", "high_ambiguous", "tree_method", "libray_layout", "help"]) 
+        script_name = sys.argv[0]
+        input_commands = [script_name]
+
+        for opt, arg in opts:
+            input_commands.append(opt)
+            if arg:
+                input_commands.append(arg)
+
+        for arg in args:
+            input_commands.append(arg)
+        logger.info("Commands: " + " ".join(input_commands))
+        
         if opts:
             opts_dict = dict(opts)
             opts_keys = list(opts_dict.keys())
             tar_set = set(opts_keys)
-            # print(tar_set)
+
             h_lst = list({'-h', '--help'}.intersection(tar_set))
             if h_lst:
-                usage()                
+                usage()           
                 sys.exit()  
             else: 
                 m_lst = list({"-m", "--module"}.intersection(tar_set))
                 c_lst = list({"-c", "--config"}.intersection(tar_set)) 
                 i_lst = list({"-i", "--input"}.intersection(tar_set)) 
                 u_lst = list({"-u", "--umi_file"}.intersection(tar_set)) 
                 t_lst = list({"-t", "--true"}.intersection(tar_set)) 
@@ -46,20 +60,23 @@
 
                 # l_lst = list({"-l", "--libray_layout"}.intersection(tar_set))
                 # ref_lst = list({"-f", "--reference_in"}.intersection(tar_set))
                 # r0_lst = list({"-0", "--read"}.intersection(tar_set))
                 # r1_lst = list({"-1", "--read1"}.intersection(tar_set))
                 # r2_lst = list({"-2", "--read1"}.intersection(tar_set))
                 # align_lst = list({"-A", "--Alignment"}.intersection(tar_set))
+                    
                 if m_lst:
                     module_arg = opts_dict[m_lst[0]]
+                        
                 else:
                     logger.error("Not select any module, using command noise2read -h/--help for usage.")
                     sys.exit()
                 available_cpu_cores = os.cpu_count()
+
 ############################################################################################################################
                 if module_arg == "correction":
                     # try: 
                     if c_lst:
                         config = Config(opts_dict[c_lst[0]], logger) 
                         if i_lst:
                             config.input_file = opts_dict[i_lst[0]]
@@ -411,15 +428,18 @@
                     if config.num_workers <= 0:
                         config.num_workers = available_cpu_cores - 2
                     if config.num_workers > available_cpu_cores:
                         logger.error(f"Only {available_cpu_cores} available to use.") 
                         config.num_workers = available_cpu_cores - 2
                     Simulation(logger, config).simulation()
 ############################################################################################################################
+                # elif module_arg == "extract_isolates": 
+
                 else:
                     # logger.error("Invalid module name, please check.")
                     logger.error("Input wrong module name, using command noise2read -h/--help for usage.")
                     sys.exit()
+        
         else:
             logger.error("No valid arguments input, using command noise2read -h/--help for usage")
     except getopt.GetoptError as err:
         logger.error(err)
```

### Comparing `noise2read-0.0.71/src/noise2read/reads2vectors.py` & `noise2read-0.0.73/src/noise2read/reads2vectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-02-16 11:01:06
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-02-16 11:11:43
+# @Last Modified time: 2023-04-07 16:47:06
 
 from typing import Counter
 import numpy as np
 # import os
 from sklearn.preprocessing import StandardScaler
 from noise2read.encoding import EncodeScheme
 from mpire import WorkerPool
@@ -60,15 +60,15 @@
         # onehot_fea = ES.descriptors("OneHot", reads_lst1[i])
         # features.extend(onehot_fea)
         features.extend(other_features[i])
         # self.logger.debug(f'FourierTransform: {len(ft_fea)}, ChaosGame: {len(cg_fea)}, Entropy: {len(entropy_fea)}, FickettScore: {len(fs_fea)}')
         return features 
 
     def high_all_in_one_embedding(self, genuine_df, negative_df, new_negative_df, ambiguous_df):
-        self.logger.info("Embedding genuine and high ambiguous data.")
+        self.logger.info("  Embedding genuine and high ambiguous data.")
         genuine_reads_lst1 = []
         negtive_reads_lst1 = []
         ambiguous_reads_lst1 = []
 
         genuine_reads_lst2 = []
         negtive_reads_lst2 = []
         ambiguous_reads_lst2 = []
@@ -214,15 +214,15 @@
         self.logger.debug(ambiguous_data.shape)
         train, ambiguous = self.scaler(train_data, ambiguous_data, high_flag=True)
         self.logger.debug(train[0])
         del train_data, ambiguous_data, genuine_fea, negative_fea, ambiguous_fea, read_features
         return train, labels, ambiguous
 
     def all_in_one_embedding(self, total_reads, genuine_df, negative_df, ambiguous_df, high_flag):
-        self.logger.info("Embedding genuine and ambiguous data.")
+        self.logger.info("  Embedding genuine and ambiguous data.")
         genuine_reads_lst1 = []
         negtive_reads_lst1 = []
         ambiguous_reads_lst1 = []
 
         genuine_reads_lst2 = []
         negtive_reads_lst2 = []
         ambiguous_reads_lst2 = []
```

### Comparing `noise2read-0.0.71/src/noise2read/simulation.py` & `noise2read-0.0.73/src/noise2read/simulation.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.71/src/noise2read/umitest.py` & `noise2read-0.0.73/src/noise2read/umitest.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.71/src/noise2read/utils.py` & `noise2read-0.0.73/src/noise2read/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-02-16 11:01:06
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-02-16 11:12:28
+# @Last Modified time: 2023-04-07 17:22:18
 
 from Bio import SeqIO
 import gzip
 # from Bio.SeqRecord import SeqRecord
 # from Bio.Seq import Seq
-from tqdm import tqdm
-from mpire import WorkerPool
 import logging
 from colorlog import ColoredFormatter
 import copy
 import random
 import editdistance
 import os
+import datetime
 
-def custom_logger(root_name, debug_mode) -> logging.Logger:
-    logger = logging.getLogger(root_name)
+def custom_logger(root_name, debug_mode) -> logging.Logger: 
+    logger = logging.getLogger(root_name)    
+    
     formatter = ColoredFormatter(
         "%(green)s[%(asctime)s] %(blue)s%(name)s %(log_color)s%(levelname)-8s%(reset)s %(message)s",
         datefmt=None,
         reset=True,
         log_colors={
             'DEBUG':    'cyan',
             'INFO':     'green',
@@ -33,25 +33,25 @@
         secondary_log_colors={},
         style='%'
     )
     if debug_mode:
         logger.setLevel(logging.DEBUG)
     else:
         logger.setLevel(logging.INFO)
-
     stream_handler = logging.StreamHandler()
     stream_handler.setFormatter(formatter)
     logger.addHandler(stream_handler)
     
-    # # Output full log
-    # file_handler = logging.FileHandler('noise2read.log')
-    # file_handler.setLevel(logging.INFO)
-    # # formatter = logging.Formatter(log_format)
-    # file_handler.setFormatter(formatter)
-    # logger.addHandler(file_handler)
+    # Output full log
+    file_handler = logging.FileHandler( datetime.datetime.now().strftime("%Y_%m_%d_%H_%M_") + 'noise2read.log')
+
+    file_handler.setLevel(logging.INFO)
+
+    # formatter = logging.Formatter(log_format)
+    logger.addHandler(file_handler)
 
     # # Output warning log
     # file_handler = logging.FileHandler('noise2read.Warning.log')
     # file_handler.setLevel(logging.WARNING)
     # # formatter = logging.Formatter(log_format)
     # file_handler.setFormatter(formatter)
     # logger.addHandler(file_handler)
@@ -338,26 +338,26 @@
         return [errorType, f_kmer, s_kmer]
     else:
         raise ValueError("The editdistance of two reads in the input list must equal to one!")
 
 def usage():
     # print(" ")
     print("noise2read Usage:")
-    print("   Mandatary:")
+    print("   Mandatory:")
     print("     -m|--module                   module selection")
     print("   Modules: [correction, amplicon_correction, umi_correction, mimic_umi, real_umi, evaluation, simulation]")
     # print(" ")
     print("1. Using config file")
     print("     noise2read -m|--module <module_name> -c <path_configuration_file>")
-    print("   Mandatary:")
+    print("   Mandatory:")
     print("     -c|--config                   input configuration file")
     # print(" ")
     print("2. Using command line with the default parameters")
     print("     noise2read -m|--module <module_name> -i <path_raw_data.fastq|fasta|fa|fq>")
-    print("   Mandatary:")
+    print("   Mandatory:")
     print("     -i|--input                    input raw data to be corrected")
     print("   Options:")
     print("     -d|--directory                set output directory")
     print("     -a|--high_ambiguous           predict high ambiguous errors using machine learning when set true, defaut true")
     print("     -t|--true                     input ground truth data if you have")
     print("     -r|--rectification            input corrected data when using module evaluation")
     print("     -p|--parallel                 use multiple cpu cores, default total cpu cores - 2")
```

### Comparing `noise2read-0.0.71/src/noise2read.egg-info/SOURCES.txt` & `noise2read-0.0.73/src/noise2read.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.71/tests/test_data_generation.py` & `noise2read-0.0.73/tests/test_data_generation.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.71/tests/test_reads2vector.py` & `noise2read-0.0.73/tests/test_reads2vector.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.71/tests/test_utils.py` & `noise2read-0.0.73/tests/test_utils.py`

 * *Files identical despite different names*

