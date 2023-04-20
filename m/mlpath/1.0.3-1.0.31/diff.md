# Comparing `tmp/mlpath-1.0.3.tar.gz` & `tmp/mlpath-1.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpath-1.0.3.tar", last modified: Thu Apr 20 16:01:45 2023, max compression
+gzip compressed data, was "mlpath-1.0.31.tar", last modified: Thu Apr 20 16:27:24 2023, max compression
```

## Comparing `mlpath-1.0.3.tar` & `mlpath-1.0.31.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-04-20 16:01:45.394504 mlpath-1.0.3/
--rw-r--r--   0 essam      (501) staff       (20)    18092 2023-03-22 10:05:32.000000 mlpath-1.0.3/LICENSE
--rw-r--r--   0 essam      (501) staff       (20)      192 2023-03-22 10:05:32.000000 mlpath-1.0.3/MANIFEST.in
--rw-r--r--   0 essam      (501) staff       (20)    17606 2023-04-20 16:01:45.394237 mlpath-1.0.3/PKG-INFO
--rw-r--r--   0 essam      (501) staff       (20)    16806 2023-04-20 16:01:05.000000 mlpath-1.0.3/README.md
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-04-20 16:01:45.390871 mlpath-1.0.3/mlpath/
--rw-r--r--   0 essam      (501) staff       (20)      122 2023-03-22 10:05:32.000000 mlpath-1.0.3/mlpath/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-04-20 16:01:45.392537 mlpath-1.0.3/mlpath/mldir_cli/
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-03-22 10:05:32.000000 mlpath-1.0.3/mlpath/mldir_cli/__init__.py
--rw-r--r--   0 essam      (501) staff       (20)     2049 2023-03-22 10:05:32.000000 mlpath-1.0.3/mlpath/mldir_cli/cli.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-04-20 16:01:45.393732 mlpath-1.0.3/mlpath/mlquest/
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-03-22 10:05:32.000000 mlpath-1.0.3/mlpath/mlquest/__init__.py
--rw-r--r--   0 essam      (501) staff       (20)    19811 2023-04-20 14:39:55.000000 mlpath-1.0.3/mlpath/mlquest/mlquest.py
--rw-r--r--   0 essam      (501) staff       (20)    10190 2023-04-20 15:47:31.000000 mlpath-1.0.3/mlpath/mlquest/utils.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-04-20 16:01:45.392195 mlpath-1.0.3/mlpath.egg-info/
--rw-r--r--   0 essam      (501) staff       (20)    17606 2023-04-20 16:01:44.000000 mlpath-1.0.3/mlpath.egg-info/PKG-INFO
--rw-r--r--   0 essam      (501) staff       (20)      369 2023-04-20 16:01:45.000000 mlpath-1.0.3/mlpath.egg-info/SOURCES.txt
--rw-r--r--   0 essam      (501) staff       (20)        1 2023-04-20 16:01:44.000000 mlpath-1.0.3/mlpath.egg-info/dependency_links.txt
--rw-r--r--   0 essam      (501) staff       (20)       85 2023-04-20 16:01:45.000000 mlpath-1.0.3/mlpath.egg-info/entry_points.txt
--rw-r--r--   0 essam      (501) staff       (20)       20 2023-04-20 16:01:45.000000 mlpath-1.0.3/mlpath.egg-info/requires.txt
--rw-r--r--   0 essam      (501) staff       (20)        7 2023-04-20 16:01:45.000000 mlpath-1.0.3/mlpath.egg-info/top_level.txt
--rw-r--r--   0 essam      (501) staff       (20)       38 2023-04-20 16:01:45.394592 mlpath-1.0.3/setup.cfg
--rw-r--r--   0 essam      (501) staff       (20)     2065 2023-04-20 16:01:31.000000 mlpath-1.0.3/setup.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-04-20 16:27:24.235901 mlpath-1.0.31/
+-rw-r--r--   0 essam      (501) staff       (20)    18092 2023-04-20 16:25:39.000000 mlpath-1.0.31/LICENSE
+-rw-r--r--   0 essam      (501) staff       (20)      192 2023-04-20 16:25:39.000000 mlpath-1.0.31/MANIFEST.in
+-rw-r--r--   0 essam      (501) staff       (20)    17710 2023-04-20 16:27:24.235595 mlpath-1.0.31/PKG-INFO
+-rw-r--r--   0 essam      (501) staff       (20)    16909 2023-04-20 16:25:39.000000 mlpath-1.0.31/README.md
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-04-20 16:27:24.232029 mlpath-1.0.31/mlpath/
+-rw-r--r--   0 essam      (501) staff       (20)      122 2023-04-20 16:25:39.000000 mlpath-1.0.31/mlpath/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-04-20 16:27:24.233850 mlpath-1.0.31/mlpath/mldir_cli/
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-04-20 16:25:39.000000 mlpath-1.0.31/mlpath/mldir_cli/__init__.py
+-rw-r--r--   0 essam      (501) staff       (20)     2049 2023-04-20 16:25:39.000000 mlpath-1.0.31/mlpath/mldir_cli/cli.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-04-20 16:27:24.235077 mlpath-1.0.31/mlpath/mlquest/
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-04-20 16:25:39.000000 mlpath-1.0.31/mlpath/mlquest/__init__.py
+-rw-r--r--   0 essam      (501) staff       (20)    19811 2023-04-20 16:25:39.000000 mlpath-1.0.31/mlpath/mlquest/mlquest.py
+-rw-r--r--   0 essam      (501) staff       (20)    10190 2023-04-20 16:25:39.000000 mlpath-1.0.31/mlpath/mlquest/utils.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-04-20 16:27:24.233492 mlpath-1.0.31/mlpath.egg-info/
+-rw-r--r--   0 essam      (501) staff       (20)    17710 2023-04-20 16:27:23.000000 mlpath-1.0.31/mlpath.egg-info/PKG-INFO
+-rw-r--r--   0 essam      (501) staff       (20)      369 2023-04-20 16:27:24.000000 mlpath-1.0.31/mlpath.egg-info/SOURCES.txt
+-rw-r--r--   0 essam      (501) staff       (20)        1 2023-04-20 16:27:23.000000 mlpath-1.0.31/mlpath.egg-info/dependency_links.txt
+-rw-r--r--   0 essam      (501) staff       (20)       85 2023-04-20 16:27:23.000000 mlpath-1.0.31/mlpath.egg-info/entry_points.txt
+-rw-r--r--   0 essam      (501) staff       (20)       20 2023-04-20 16:27:24.000000 mlpath-1.0.31/mlpath.egg-info/requires.txt
+-rw-r--r--   0 essam      (501) staff       (20)        7 2023-04-20 16:27:24.000000 mlpath-1.0.31/mlpath.egg-info/top_level.txt
+-rw-r--r--   0 essam      (501) staff       (20)       38 2023-04-20 16:27:24.235991 mlpath-1.0.31/setup.cfg
+-rw-r--r--   0 essam      (501) staff       (20)     2066 2023-04-20 16:27:01.000000 mlpath-1.0.31/setup.py
```

### Comparing `mlpath-1.0.3/LICENSE` & `mlpath-1.0.31/LICENSE`

 * *Files identical despite different names*

### Comparing `mlpath-1.0.3/PKG-INFO` & `mlpath-1.0.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpath
-Version: 1.0.3
+Version: 1.0.31
 Summary: A lightweight api for machine and deep learning experiment logging in the form of a python library. 
 Home-page: https://mlpath.readthedocs.io/
 Author: Essam W., Abdullah A.
 Author-email: essamwisam@outlook.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -70,23 +70,22 @@
 # Model Initialization
 model = l(RadialBasisNet)(x_data_f, 99, 19, 31)
 
 # Model Training
 accuracy = train_model(model)
 
 # log the accuracy
-mlq.log_metrics(accuracy)                             # pass acc=accuracy to log as acc
+mlq.log_metrics(accuracy)        # can also do mlq.log_metric(acc=accuracy) so its logged as acc
 
 mlq.end_quest()
 
 mlq.show_table('Radial Basis Pipeline', last_k=10)    # show the table for the last 10 runs
-```
 
 ```
-After three runs, the markdown file under the ```Quests``` folder has
+After the third run, this shows up under the Quests folder (and the notebook itself):
 <table>
 <tr>
 <th colspan=4 style="text-align: center; vertical-align: middle;">info</th>
 <th colspan=3 style="text-align: center; vertical-align: middle;">Preprocessing</th>
 <th colspan=3 style="text-align: center; vertical-align: middle;">FeatureExtraction</th>
 <th colspan=3 style="text-align: center; vertical-align: middle;">RadialBasisNet</th>
 <th colspan=1 style="text-align: center; vertical-align: middle;">metrics</th>
@@ -201,14 +200,16 @@
 
 # report the accuracy
 accuracy = model.score(x_val_f, y_val_i).item()     # .item() so its a scalar that can be logged
 
 mlq.log_metrics(acc=accuracy)
 
 mlq.end_quest()
+
+mlq.show_table('Fractal-GB', last_k=10)    # show the table for the last 10 runs
 ```
 <table>
 <tr>
 <th colspan=4 style="text-align: center; vertical-align: middle;">info</th>
 <th colspan=1 style="text-align: center; vertical-align: middle;">apply_SFTA</th>
 <th colspan=3 style="text-align: center; vertical-align: middle;">GradientBoostingClassifier</th>
 <th colspan=1 style="text-align: center; vertical-align: middle;">metrics</th>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mlpath Version: 1.0.3 Summary: A lightweight api
+Metadata-Version: 2.1 Name: mlpath Version: 1.0.31 Summary: A lightweight api
 for machine and deep learning experiment logging in the form of a python
 library. Home-page: https://mlpath.readthedocs.io/ Author: Essam W., Abdullah
 A. Author-email: essamwisam@outlook.com License: GPLv3 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
@@ -25,18 +25,18 @@
 mlquest as mlq l = mlq.l # Start a new quest, this corresponds to a table where
 every run of the Python file will be logged. mlq.start_quest('Radial Basis
 Pipeline', log_defs=False) # Preprocessing x_data_p = l(Preprocessing)(x_data=
 [1, 2, 3], alpha=1114, beta_param=2, c=925) # Feature Extraction x_data_f = l
 (FeatureExtraction)(x_data_p, 32, 50, 4) # x_data_p is an array so it won't be
 logged. # Model Initialization model = l(RadialBasisNet)(x_data_f, 99, 19, 31)
 # Model Training accuracy = train_model(model) # log the accuracy
-mlq.log_metrics(accuracy) # pass acc=accuracy to log as acc mlq.end_quest()
-mlq.show_table('Radial Basis Pipeline', last_k=10) # show the table for the
-last 10 runs ``` ``` After three runs, the markdown file under the ```Quests```
-folder has
+mlq.log_metrics(accuracy) # can also do mlq.log_metric(acc=accuracy) so its
+logged as acc mlq.end_quest() mlq.show_table('Radial Basis Pipeline',
+last_k=10) # show the table for the last 10 runs ``` After the third run, this
+shows up under the Quests folder (and the notebook itself):
 info                     Preprocessing FeatureExtraction RadialBasisNet metrics
 16:31: 02/11/ 1.01 min 1 74   12 95    13  530 4         99 99 3        50
 16     23
 16:32: 02/11/ 4.91 ms  2 14   2  95    132 530 4         99 19 3        70
 40     23
 16:32: 02/11/ 4.93 ms  3 1114 2  925   32  50  4         99 19 31       70
 57     23
@@ -58,15 +58,16 @@
 y_train_i, y_val_i = read_data() # preprocess the data x_train_p, x_val_p =
 preprocess_data(x_train_i, x_val_i) # extract fractal features x_train_f,
 x_val_f = mlq.l(apply_SFTA)(x_train_p, x_val_p, deviation=10) # initialize a GB
 model model = mlq.l(GradientBoostingClassifier)(n_estimators=10,
 learning_rate=220, max_depth=110) # train the model model.fit(x_train_f,
 y_train_i) # report the accuracy accuracy = model.score(x_val_f, y_val_i).item
 () # .item() so its a scalar that can be logged mlq.log_metrics(acc=accuracy)
-mlq.end_quest() ```
+mlq.end_quest() mlq.show_table('Fractal-GB', last_k=10) # show the table for
+the last 10 runs ```
 info                          apply_SFTA GradientBoostingClassifier metrics
 17:26:34 02/11/23 2.33 min  1 30         10 50  12                  0.5
 17:29:08 02/11/23 344.98 ms 2 10         50 20  10                  0.5
 17:29:14 02/11/23 251.52 ms 3 10         50 20  10                  0.5
 17:29:22 02/11/23 266.31 ms 4 10         10 220 110                 0.5
 ### An example with PyTorch A real example on a dummy dataset that demonstrates
 using the library on real models is provided in the MLDir examples mentioned
```

### Comparing `mlpath-1.0.3/README.md` & `mlpath-1.0.31/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,23 +49,22 @@
 # Model Initialization
 model = l(RadialBasisNet)(x_data_f, 99, 19, 31)
 
 # Model Training
 accuracy = train_model(model)
 
 # log the accuracy
-mlq.log_metrics(accuracy)                             # pass acc=accuracy to log as acc
+mlq.log_metrics(accuracy)        # can also do mlq.log_metric(acc=accuracy) so its logged as acc
 
 mlq.end_quest()
 
 mlq.show_table('Radial Basis Pipeline', last_k=10)    # show the table for the last 10 runs
-```
 
 ```
-After three runs, the markdown file under the ```Quests``` folder has
+After the third run, this shows up under the Quests folder (and the notebook itself):
 <table>
 <tr>
 <th colspan=4 style="text-align: center; vertical-align: middle;">info</th>
 <th colspan=3 style="text-align: center; vertical-align: middle;">Preprocessing</th>
 <th colspan=3 style="text-align: center; vertical-align: middle;">FeatureExtraction</th>
 <th colspan=3 style="text-align: center; vertical-align: middle;">RadialBasisNet</th>
 <th colspan=1 style="text-align: center; vertical-align: middle;">metrics</th>
@@ -180,14 +179,16 @@
 
 # report the accuracy
 accuracy = model.score(x_val_f, y_val_i).item()     # .item() so its a scalar that can be logged
 
 mlq.log_metrics(acc=accuracy)
 
 mlq.end_quest()
+
+mlq.show_table('Fractal-GB', last_k=10)    # show the table for the last 10 runs
 ```
 <table>
 <tr>
 <th colspan=4 style="text-align: center; vertical-align: middle;">info</th>
 <th colspan=1 style="text-align: center; vertical-align: middle;">apply_SFTA</th>
 <th colspan=3 style="text-align: center; vertical-align: middle;">GradientBoostingClassifier</th>
 <th colspan=1 style="text-align: center; vertical-align: middle;">metrics</th>
```

#### html2text {}

```diff
@@ -15,18 +15,18 @@
 mlquest as mlq l = mlq.l # Start a new quest, this corresponds to a table where
 every run of the Python file will be logged. mlq.start_quest('Radial Basis
 Pipeline', log_defs=False) # Preprocessing x_data_p = l(Preprocessing)(x_data=
 [1, 2, 3], alpha=1114, beta_param=2, c=925) # Feature Extraction x_data_f = l
 (FeatureExtraction)(x_data_p, 32, 50, 4) # x_data_p is an array so it won't be
 logged. # Model Initialization model = l(RadialBasisNet)(x_data_f, 99, 19, 31)
 # Model Training accuracy = train_model(model) # log the accuracy
-mlq.log_metrics(accuracy) # pass acc=accuracy to log as acc mlq.end_quest()
-mlq.show_table('Radial Basis Pipeline', last_k=10) # show the table for the
-last 10 runs ``` ``` After three runs, the markdown file under the ```Quests```
-folder has
+mlq.log_metrics(accuracy) # can also do mlq.log_metric(acc=accuracy) so its
+logged as acc mlq.end_quest() mlq.show_table('Radial Basis Pipeline',
+last_k=10) # show the table for the last 10 runs ``` After the third run, this
+shows up under the Quests folder (and the notebook itself):
 info                     Preprocessing FeatureExtraction RadialBasisNet metrics
 16:31: 02/11/ 1.01 min 1 74   12 95    13  530 4         99 99 3        50
 16     23
 16:32: 02/11/ 4.91 ms  2 14   2  95    132 530 4         99 19 3        70
 40     23
 16:32: 02/11/ 4.93 ms  3 1114 2  925   32  50  4         99 19 31       70
 57     23
@@ -48,15 +48,16 @@
 y_train_i, y_val_i = read_data() # preprocess the data x_train_p, x_val_p =
 preprocess_data(x_train_i, x_val_i) # extract fractal features x_train_f,
 x_val_f = mlq.l(apply_SFTA)(x_train_p, x_val_p, deviation=10) # initialize a GB
 model model = mlq.l(GradientBoostingClassifier)(n_estimators=10,
 learning_rate=220, max_depth=110) # train the model model.fit(x_train_f,
 y_train_i) # report the accuracy accuracy = model.score(x_val_f, y_val_i).item
 () # .item() so its a scalar that can be logged mlq.log_metrics(acc=accuracy)
-mlq.end_quest() ```
+mlq.end_quest() mlq.show_table('Fractal-GB', last_k=10) # show the table for
+the last 10 runs ```
 info                          apply_SFTA GradientBoostingClassifier metrics
 17:26:34 02/11/23 2.33 min  1 30         10 50  12                  0.5
 17:29:08 02/11/23 344.98 ms 2 10         50 20  10                  0.5
 17:29:14 02/11/23 251.52 ms 3 10         50 20  10                  0.5
 17:29:22 02/11/23 266.31 ms 4 10         10 220 110                 0.5
 ### An example with PyTorch A real example on a dummy dataset that demonstrates
 using the library on real models is provided in the MLDir examples mentioned
```

### Comparing `mlpath-1.0.3/mlpath/mldir_cli/cli.py` & `mlpath-1.0.31/mlpath/mldir_cli/cli.py`

 * *Files identical despite different names*

### Comparing `mlpath-1.0.3/mlpath/mlquest/mlquest.py` & `mlpath-1.0.31/mlpath/mlquest/mlquest.py`

 * *Files identical despite different names*

### Comparing `mlpath-1.0.3/mlpath/mlquest/utils.py` & `mlpath-1.0.31/mlpath/mlquest/utils.py`

 * *Files identical despite different names*

### Comparing `mlpath-1.0.3/mlpath.egg-info/PKG-INFO` & `mlpath-1.0.31/mlpath.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpath
-Version: 1.0.3
+Version: 1.0.31
 Summary: A lightweight api for machine and deep learning experiment logging in the form of a python library. 
 Home-page: https://mlpath.readthedocs.io/
 Author: Essam W., Abdullah A.
 Author-email: essamwisam@outlook.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -70,23 +70,22 @@
 # Model Initialization
 model = l(RadialBasisNet)(x_data_f, 99, 19, 31)
 
 # Model Training
 accuracy = train_model(model)
 
 # log the accuracy
-mlq.log_metrics(accuracy)                             # pass acc=accuracy to log as acc
+mlq.log_metrics(accuracy)        # can also do mlq.log_metric(acc=accuracy) so its logged as acc
 
 mlq.end_quest()
 
 mlq.show_table('Radial Basis Pipeline', last_k=10)    # show the table for the last 10 runs
-```
 
 ```
-After three runs, the markdown file under the ```Quests``` folder has
+After the third run, this shows up under the Quests folder (and the notebook itself):
 <table>
 <tr>
 <th colspan=4 style="text-align: center; vertical-align: middle;">info</th>
 <th colspan=3 style="text-align: center; vertical-align: middle;">Preprocessing</th>
 <th colspan=3 style="text-align: center; vertical-align: middle;">FeatureExtraction</th>
 <th colspan=3 style="text-align: center; vertical-align: middle;">RadialBasisNet</th>
 <th colspan=1 style="text-align: center; vertical-align: middle;">metrics</th>
@@ -201,14 +200,16 @@
 
 # report the accuracy
 accuracy = model.score(x_val_f, y_val_i).item()     # .item() so its a scalar that can be logged
 
 mlq.log_metrics(acc=accuracy)
 
 mlq.end_quest()
+
+mlq.show_table('Fractal-GB', last_k=10)    # show the table for the last 10 runs
 ```
 <table>
 <tr>
 <th colspan=4 style="text-align: center; vertical-align: middle;">info</th>
 <th colspan=1 style="text-align: center; vertical-align: middle;">apply_SFTA</th>
 <th colspan=3 style="text-align: center; vertical-align: middle;">GradientBoostingClassifier</th>
 <th colspan=1 style="text-align: center; vertical-align: middle;">metrics</th>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mlpath Version: 1.0.3 Summary: A lightweight api
+Metadata-Version: 2.1 Name: mlpath Version: 1.0.31 Summary: A lightweight api
 for machine and deep learning experiment logging in the form of a python
 library. Home-page: https://mlpath.readthedocs.io/ Author: Essam W., Abdullah
 A. Author-email: essamwisam@outlook.com License: GPLv3 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
@@ -25,18 +25,18 @@
 mlquest as mlq l = mlq.l # Start a new quest, this corresponds to a table where
 every run of the Python file will be logged. mlq.start_quest('Radial Basis
 Pipeline', log_defs=False) # Preprocessing x_data_p = l(Preprocessing)(x_data=
 [1, 2, 3], alpha=1114, beta_param=2, c=925) # Feature Extraction x_data_f = l
 (FeatureExtraction)(x_data_p, 32, 50, 4) # x_data_p is an array so it won't be
 logged. # Model Initialization model = l(RadialBasisNet)(x_data_f, 99, 19, 31)
 # Model Training accuracy = train_model(model) # log the accuracy
-mlq.log_metrics(accuracy) # pass acc=accuracy to log as acc mlq.end_quest()
-mlq.show_table('Radial Basis Pipeline', last_k=10) # show the table for the
-last 10 runs ``` ``` After three runs, the markdown file under the ```Quests```
-folder has
+mlq.log_metrics(accuracy) # can also do mlq.log_metric(acc=accuracy) so its
+logged as acc mlq.end_quest() mlq.show_table('Radial Basis Pipeline',
+last_k=10) # show the table for the last 10 runs ``` After the third run, this
+shows up under the Quests folder (and the notebook itself):
 info                     Preprocessing FeatureExtraction RadialBasisNet metrics
 16:31: 02/11/ 1.01 min 1 74   12 95    13  530 4         99 99 3        50
 16     23
 16:32: 02/11/ 4.91 ms  2 14   2  95    132 530 4         99 19 3        70
 40     23
 16:32: 02/11/ 4.93 ms  3 1114 2  925   32  50  4         99 19 31       70
 57     23
@@ -58,15 +58,16 @@
 y_train_i, y_val_i = read_data() # preprocess the data x_train_p, x_val_p =
 preprocess_data(x_train_i, x_val_i) # extract fractal features x_train_f,
 x_val_f = mlq.l(apply_SFTA)(x_train_p, x_val_p, deviation=10) # initialize a GB
 model model = mlq.l(GradientBoostingClassifier)(n_estimators=10,
 learning_rate=220, max_depth=110) # train the model model.fit(x_train_f,
 y_train_i) # report the accuracy accuracy = model.score(x_val_f, y_val_i).item
 () # .item() so its a scalar that can be logged mlq.log_metrics(acc=accuracy)
-mlq.end_quest() ```
+mlq.end_quest() mlq.show_table('Fractal-GB', last_k=10) # show the table for
+the last 10 runs ```
 info                          apply_SFTA GradientBoostingClassifier metrics
 17:26:34 02/11/23 2.33 min  1 30         10 50  12                  0.5
 17:29:08 02/11/23 344.98 ms 2 10         50 20  10                  0.5
 17:29:14 02/11/23 251.52 ms 3 10         50 20  10                  0.5
 17:29:22 02/11/23 266.31 ms 4 10         10 220 110                 0.5
 ### An example with PyTorch A real example on a dummy dataset that demonstrates
 using the library on real models is provided in the MLDir examples mentioned
```

### Comparing `mlpath-1.0.3/setup.py` & `mlpath-1.0.31/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         requirements = f.read().splitlines()
     return requirements
 
 
 # This call to setup() does all the work
 setup(
     name="mlpath",
-    version="1.0.3",
+    version="1.0.31",
     description="A lightweight api for machine and deep learning experiment logging in the form of a python library. ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://mlpath.readthedocs.io/",
     author="Essam W., Abdullah A.",
     author_email="essamwisam@outlook.com",
     license="GPLv3",
```

