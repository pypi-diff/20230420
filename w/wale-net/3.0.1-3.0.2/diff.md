# Comparing `tmp/wale-net-3.0.1.tar.gz` & `tmp/wale-net-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wale-net-3.0.1.tar", last modified: Mon Dec 19 12:26:52 2022, max compression
+gzip compressed data, was "wale-net-3.0.2.tar", last modified: Thu Apr 20 07:25:45 2023, max compression
```

## Comparing `wale-net-3.0.1.tar` & `wale-net-3.0.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2022-12-19 12:26:52.157999 wale-net-3.0.1/
--rw-rw-r--   0 max       (1000) max       (1000)     1071 2022-05-31 13:43:26.000000 wale-net-3.0.1/LICENSE
--rw-rw-r--   0 max       (1000) max       (1000)      175 2022-05-31 13:43:26.000000 wale-net-3.0.1/MANIFEST.in
--rw-rw-r--   0 max       (1000) max       (1000)      928 2022-12-19 12:26:52.157999 wale-net-3.0.1/PKG-INFO
--rw-rw-r--   0 max       (1000) max       (1000)     4151 2022-05-31 13:43:26.000000 wale-net-3.0.1/README.md
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2022-12-19 12:26:52.153999 wale-net-3.0.1/prediction/
--rw-rw-r--   0 max       (1000) max       (1000)       62 2022-05-31 13:43:26.000000 wale-net-3.0.1/prediction/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     4623 2022-05-31 13:43:26.000000 wale-net-3.0.1/prediction/bayesian_optimization.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2022-12-19 12:26:52.153999 wale-net-3.0.1/prediction/configs/
--rw-rw-r--   0 max       (1000) max       (1000)     1694 2022-05-31 13:43:26.000000 wale-net-3.0.1/prediction/configs/README.md
--rw-rw-r--   0 max       (1000) max       (1000)      898 2022-05-31 13:43:26.000000 wale-net-3.0.1/prediction/configs/best_config.json
--rw-rw-r--   0 max       (1000) max       (1000)      824 2022-05-31 13:44:15.000000 wale-net-3.0.1/prediction/configs/default.json
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2022-12-19 12:26:52.153999 wale-net-3.0.1/prediction/configs/online/
--rw-rw-r--   0 max       (1000) max       (1000)     1309 2022-05-31 13:43:26.000000 wale-net-3.0.1/prediction/configs/online/README.md
--rw-rw-r--   0 max       (1000) max       (1000)      394 2022-05-31 13:46:41.000000 wale-net-3.0.1/prediction/configs/online/default.json
--rw-rw-r--   0 max       (1000) max       (1000)      747 2022-05-31 13:43:26.000000 wale-net-3.0.1/prediction/configs/online_learning.json
--rw-rw-r--   0 max       (1000) max       (1000)     8629 2022-05-31 13:43:26.000000 wale-net-3.0.1/prediction/evaluate.py
--rw-rw-r--   0 max       (1000) max       (1000)     8336 2022-05-31 13:43:26.000000 wale-net-3.0.1/prediction/evaluate_online_learning.py
--rw-rw-r--   0 max       (1000) max       (1000)    34912 2022-12-19 12:22:49.000000 wale-net-3.0.1/prediction/main.py
--rw-rw-r--   0 max       (1000) max       (1000)     1479 2022-05-31 13:43:26.000000 wale-net-3.0.1/prediction/nvrgrad.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2022-12-19 12:26:52.157999 wale-net-3.0.1/prediction/tools/
--rw-rw-r--   0 max       (1000) max       (1000)        0 2022-05-31 13:43:26.000000 wale-net-3.0.1/prediction/tools/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)    10634 2022-05-31 13:43:26.000000 wale-net-3.0.1/prediction/tools/commonroad_dataset.py
--rw-rw-r--   0 max       (1000) max       (1000)     9387 2022-05-31 13:43:26.000000 wale-net-3.0.1/prediction/tools/eval_analysis.py
--rw-rw-r--   0 max       (1000) max       (1000)     5946 2022-05-31 13:43:26.000000 wale-net-3.0.1/prediction/tools/grad_variance.py
--rw-rw-r--   0 max       (1000) max       (1000)      296 2022-05-31 13:43:26.000000 wale-net-3.0.1/prediction/tools/rename.py
--rw-rw-r--   0 max       (1000) max       (1000)    13978 2022-05-31 14:55:25.000000 wale-net-3.0.1/prediction/train.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2022-12-19 12:26:52.157999 wale-net-3.0.1/prediction/trained_models/
--rw-rw-r--   0 max       (1000) max       (1000)   446790 2022-05-31 13:43:26.000000 wale-net-3.0.1/prediction/trained_models/best_model.tar
--rw-rw-r--   0 max       (1000) max       (1000)  1468458 2022-05-31 13:43:26.000000 wale-net-3.0.1/prediction/trained_models/online_learning.tar
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2022-12-19 12:26:52.157999 wale-net-3.0.1/prediction/utils/
--rw-rw-r--   0 max       (1000) max       (1000)        0 2022-05-31 13:43:26.000000 wale-net-3.0.1/prediction/utils/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)      373 2022-05-31 13:43:26.000000 wale-net-3.0.1/prediction/utils/cuda.py
--rw-rw-r--   0 max       (1000) max       (1000)     3890 2022-05-31 13:43:26.000000 wale-net-3.0.1/prediction/utils/dataset.py
--rw-rw-r--   0 max       (1000) max       (1000)     5345 2022-05-31 13:43:26.000000 wale-net-3.0.1/prediction/utils/geometry.py
--rw-rw-r--   0 max       (1000) max       (1000)    11490 2022-05-31 13:43:26.000000 wale-net-3.0.1/prediction/utils/model.py
--rw-rw-r--   0 max       (1000) max       (1000)     6076 2022-05-31 13:43:26.000000 wale-net-3.0.1/prediction/utils/neural_network.py
--rw-rw-r--   0 max       (1000) max       (1000)     7576 2022-06-22 08:15:54.000000 wale-net-3.0.1/prediction/utils/preprocessing.py
--rw-rw-r--   0 max       (1000) max       (1000)    14173 2022-05-31 13:43:26.000000 wale-net-3.0.1/prediction/utils/visualization.py
--rw-rw-r--   0 max       (1000) max       (1000)      193 2022-06-22 08:28:25.000000 wale-net-3.0.1/requirements.txt
--rw-rw-r--   0 max       (1000) max       (1000)       38 2022-12-19 12:26:52.157999 wale-net-3.0.1/setup.cfg
--rw-rw-r--   0 max       (1000) max       (1000)     1516 2022-12-19 12:26:22.000000 wale-net-3.0.1/setup.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2022-12-19 12:26:52.157999 wale-net-3.0.1/wale_net.egg-info/
--rw-rw-r--   0 max       (1000) max       (1000)      928 2022-12-19 12:26:52.000000 wale-net-3.0.1/wale_net.egg-info/PKG-INFO
--rw-rw-r--   0 max       (1000) max       (1000)     1098 2022-12-19 12:26:52.000000 wale-net-3.0.1/wale_net.egg-info/SOURCES.txt
--rw-rw-r--   0 max       (1000) max       (1000)        1 2022-12-19 12:26:52.000000 wale-net-3.0.1/wale_net.egg-info/dependency_links.txt
--rw-rw-r--   0 max       (1000) max       (1000)      192 2022-12-19 12:26:52.000000 wale-net-3.0.1/wale_net.egg-info/requires.txt
--rw-rw-r--   0 max       (1000) max       (1000)       11 2022-12-19 12:26:52.000000 wale-net-3.0.1/wale_net.egg-info/top_level.txt
+drwxrwxr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-20 07:25:45.108377 wale-net-3.0.2/
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     1071 2022-12-19 14:40:59.000000 wale-net-3.0.2/LICENSE
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)      175 2022-12-19 14:40:59.000000 wale-net-3.0.2/MANIFEST.in
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)      891 2023-04-20 07:25:45.108377 wale-net-3.0.2/PKG-INFO
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     4151 2022-12-19 14:40:59.000000 wale-net-3.0.2/README.md
+drwxrwxr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-20 07:25:45.104377 wale-net-3.0.2/prediction/
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)       62 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/__init__.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     4623 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/bayesian_optimization.py
+drwxrwxr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-20 07:25:45.108377 wale-net-3.0.2/prediction/configs/
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     1694 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/configs/README.md
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)      898 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/configs/best_config.json
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)      824 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/configs/default.json
+drwxrwxr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-20 07:25:45.108377 wale-net-3.0.2/prediction/configs/online/
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     1309 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/configs/online/README.md
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)      394 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/configs/online/default.json
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)      747 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/configs/online_learning.json
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     8629 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/evaluate.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     8336 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/evaluate_online_learning.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)    35277 2023-03-23 12:22:12.000000 wale-net-3.0.2/prediction/main.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     1479 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/nvrgrad.py
+drwxrwxr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-20 07:25:45.108377 wale-net-3.0.2/prediction/tools/
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)        0 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/tools/__init__.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)    10634 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/tools/commonroad_dataset.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     9387 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/tools/eval_analysis.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     5946 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/tools/grad_variance.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)      296 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/tools/rename.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)    13978 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/train.py
+drwxrwxr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-20 07:25:45.108377 wale-net-3.0.2/prediction/trained_models/
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)   446790 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/trained_models/best_model.tar
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)  1468458 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/trained_models/online_learning.tar
+drwxrwxr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-20 07:25:45.108377 wale-net-3.0.2/prediction/utils/
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)        0 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/utils/__init__.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)      373 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/utils/cuda.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     3890 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/utils/dataset.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     5345 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/utils/geometry.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)    11490 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/utils/model.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     6076 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/utils/neural_network.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     9618 2023-01-17 18:38:18.000000 wale-net-3.0.2/prediction/utils/preprocessing.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)    14173 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/utils/visualization.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)      185 2023-03-23 12:22:46.000000 wale-net-3.0.2/requirements.txt
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)       38 2023-04-20 07:25:45.108377 wale-net-3.0.2/setup.cfg
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     1512 2023-04-20 07:19:07.000000 wale-net-3.0.2/setup.py
+drwxrwxr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-20 07:25:45.108377 wale-net-3.0.2/wale_net.egg-info/
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)      891 2023-04-20 07:25:45.000000 wale-net-3.0.2/wale_net.egg-info/PKG-INFO
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     1098 2023-04-20 07:25:45.000000 wale-net-3.0.2/wale_net.egg-info/SOURCES.txt
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)        1 2023-04-20 07:25:45.000000 wale-net-3.0.2/wale_net.egg-info/dependency_links.txt
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)      184 2023-04-20 07:25:45.000000 wale-net-3.0.2/wale_net.egg-info/requires.txt
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)       11 2023-04-20 07:25:45.000000 wale-net-3.0.2/wale_net.egg-info/top_level.txt
```

### Comparing `wale-net-3.0.1/LICENSE` & `wale-net-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.1/PKG-INFO` & `wale-net-3.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 Metadata-Version: 2.1
 Name: wale-net
-Version: 3.0.1
+Version: 3.0.2
 Summary: Prediction module for CommonRoad
 Home-page: https://github.com/TUMFTM/Wale-Net
 Author: Maximilian Geisslinger, Phillip Karle
 Author-email: maximilian.geisslinger@tum.de, karle@ftm.mw.tum.de
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 This package provides a Recurrent Neural Network (RNN) for vehicle trajectory prediction with uncertainties.
 It builds up on the work of [Convolutional Social Pooling](https://github.com/nachiket92/conv-social-pooling).
 It has been adapted to CommonRoad and extended by the ability of scene understanding and online learning.
 
 For further information see the Readme here:
 https://github.com/TUMFTM/Wale-Net
-
-
```

### Comparing `wale-net-3.0.1/README.md` & `wale-net-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.1/prediction/bayesian_optimization.py` & `wale-net-3.0.2/prediction/bayesian_optimization.py`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.1/prediction/configs/README.md` & `wale-net-3.0.2/prediction/configs/README.md`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.1/prediction/configs/best_config.json` & `wale-net-3.0.2/prediction/configs/best_config.json`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.1/prediction/configs/default.json` & `wale-net-3.0.2/prediction/configs/default.json`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.1/prediction/configs/online/README.md` & `wale-net-3.0.2/prediction/configs/online/README.md`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.1/prediction/configs/online_learning.json` & `wale-net-3.0.2/prediction/configs/online_learning.json`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.1/prediction/evaluate.py` & `wale-net-3.0.2/prediction/evaluate.py`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.1/prediction/evaluate_online_learning.py` & `wale-net-3.0.2/prediction/evaluate_online_learning.py`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.1/prediction/main.py` & `wale-net-3.0.2/prediction/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     import prediction  # noqa: F401
 
     __package__ = "prediction"
 
 # Custom imports
 from prediction.utils.geometry import transform_trajectories, transform_back
 from prediction.utils.preprocessing import (
+    generate_scimg,
     generate_self_rendered_sc_img,
     generate_nbr_array,
 )
 from prediction.utils.model import predictionNet
 from prediction.utils.neural_network import NLL, MSE
 from prediction.utils.visualization import draw_uncertain_predictions
 from prediction.utils.cuda import cudanize
@@ -64,18 +65,17 @@
             multiprocessing (bool, optional): [True if multiprocessing should be used]. Defaults to False.
         """
         self.scenario = scenario
         self.__common_args = common_args
         self.__multiprocessing = multiprocessing
 
         self.time_list = []
-        self.num_obstacles_list = []
         self.online_args = None
 
-    def step(self, time_step, obstacle_id_list, scenario=None):
+    def step(self, time_step, obstacle_id_list=None, scenario=None):
         """Step function that executes the main function of the prediction.
 
         Arguments:
             scenario ([commonroad.Scenario]) -- [CommonRoad scenario object]
             time_step {[int]} -- [time_step of CommonRoad scenario]
             obstacle_id_list {[list]} -- [list of obstacle ids that should be predicted]
 
@@ -84,16 +84,23 @@
 
         Returns:
             prediction_result [dict] -- [dictionary with obstacle ids as keys and x,y position and covariance matrix as values]
         """
         # Update scenario
         if scenario:
             self.scenario = scenario
+
+        # Take all obstacle ids if non are given
+        if obstacle_id_list is None:
+            obstacle_id_list = list(self.scenario._dynamic_obstacles.keys())
+
         self.prediction_result = {}
         self.time_step = time_step
+        self.time_list = []
+        self.num_obstacles_list = []
 
         # Check if all obstacles are still in the scenario
         obstacle_id_list = self._obstacles_in_scenario(time_step, obstacle_id_list)
 
         obstacle_id_list.sort(
             key=lambda x: len(
                 self.scenario._dynamic_obstacles[x].prediction.trajectory.state_list
@@ -548,15 +555,15 @@
                 hist.append(traj_state_list[time_step - (i + initial_time_step)].position)
             else:
                 hist.append([np.nan, np.nan])
 
         translation = hist[-1]
         rotation = (
             self.scenario._dynamic_obstacles[obstacle_id]
-            .prediction.trajectory.state_list[time_step]
+            .prediction.trajectory.state_list[time_step-initial_time_step]
             .orientation
         )
 
         # Adapt rotation
         rotation -= math.pi / 2
 
         self.translation_dict[obstacle_id] = translation
@@ -577,17 +584,18 @@
                             i
                         ].prediction.trajectory.state_list
                     ),
                 )
             ]
             for i in range(0, len(self.scenario.dynamic_obstacles))
         ]
+        initial_time_step_list = [self.scenario.dynamic_obstacles[i].initial_state.time_step for i in range(0, len(self.scenario.dynamic_obstacles))]
         trans_traj_list = transform_trajectories(traj_list, translation, rotation)
         nbrs, _, _, _ = generate_nbr_array(
-            trans_traj_list, time_step, pp=self.pred_common_args["in_length"]
+            trans_traj_list, time_step, pp=self.pred_common_args["in_length"], initial_time_step_list=initial_time_step_list
         )
         nbrs = nbrs.reshape(nbrs.shape[0] * nbrs.shape[1], nbrs.shape[2], nbrs.shape[3])
         nbrs = np.swapaxes(nbrs, 0, 1)
 
         if "self" in self.pred_common_args["scene_image_method"]:
             sc_img = generate_self_rendered_sc_img(
                 self.pred_common_args["watch_radius"],
@@ -931,21 +939,21 @@
     time_step = 0
 
     fig, ax = plt.subplots()
 
     while time_step < 150:
 
         # Call step function for predictions
-        obstacle_list = list(scenario._dynamic_obstacles.keys())
-        predictions = predictor.step(time_step, obstacle_list)
+        predictions = predictor.step(time_step)
 
         if matplotlib.get_backend() != "agg":
 
             rnd = MPRenderer(plot_limits=[-50, 80, -30, 60])
-            scenario.draw(rnd, draw_params={'time_begin': time_step})
+            rnd.draw_params.time_begin = time_step
+            scenario.draw(rnd)
             rnd.render()
 
             draw_uncertain_predictions(predictions, ax)
             plt.gca().set_aspect("equal")
 
             # # draw ground truth
             # for obst_id in list(scenario._dynamic_obstacles.keys()):
```

### Comparing `wale-net-3.0.1/prediction/nvrgrad.py` & `wale-net-3.0.2/prediction/nvrgrad.py`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.1/prediction/tools/commonroad_dataset.py` & `wale-net-3.0.2/prediction/tools/commonroad_dataset.py`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.1/prediction/tools/eval_analysis.py` & `wale-net-3.0.2/prediction/tools/eval_analysis.py`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.1/prediction/tools/grad_variance.py` & `wale-net-3.0.2/prediction/tools/grad_variance.py`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.1/prediction/train.py` & `wale-net-3.0.2/prediction/train.py`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.1/prediction/trained_models/best_model.tar` & `wale-net-3.0.2/prediction/trained_models/best_model.tar`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.1/prediction/trained_models/online_learning.tar` & `wale-net-3.0.2/prediction/trained_models/online_learning.tar`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.1/prediction/utils/dataset.py` & `wale-net-3.0.2/prediction/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.1/prediction/utils/geometry.py` & `wale-net-3.0.2/prediction/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.1/prediction/utils/model.py` & `wale-net-3.0.2/prediction/utils/model.py`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.1/prediction/utils/neural_network.py` & `wale-net-3.0.2/prediction/utils/neural_network.py`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.1/prediction/utils/preprocessing.py` & `wale-net-3.0.2/prediction/utils/preprocessing.py`

 * *Files 15% similar despite different names*

```diff
@@ -178,47 +178,109 @@
     # there must be any kind of optimisation for saving pickling large tensors
     # in the background
     # pylint: disable=not-callable
     return img
     # pylint: enable=not-callable
     # endregion
 
-def generate_nbr_array(trans_traj_list, time_step, pp=30, window_size=[18, 78]):
+
+def generate_scimg(
+    lanelet_network, now_point, theta, time_step, watch_radius=64, draw_shape=True
+):
+    """Generate image input for neural network
+
+    Arguments:
+        scenario {[Commonroad scenario]} -- [Scenario object from CommonRoad]
+        now_point {[list]} -- [[x,y] coordinates of vehicle right now that will be predicted]
+        theta {[float]} -- [orientation of the vehicle that will be predicted]
+        time_step {[float]} -- [Global time step of scenario]
+
+    Keyword Arguments:
+        draw_shape {bool} -- [Draw shapes of dynamic obstacles in image] (default: {True})
+
+    Returns:
+        img_gray [np.array] -- [Black and white image with 256 x 256 pixels of the scene]
+    """
+    my_dpi = 300
+    draw_fig = plt.figure(
+        figsize=(256 / my_dpi, 256 / my_dpi), dpi=my_dpi
+    )  # 40 ms --> TODO shift outside the loop
+
+    if theta > 2 * np.pi:
+        theta -= 2 * np.pi
+    elif theta < -(2 * np.pi):
+        theta += 2 * np.pi
+
+    lanelet_network.translate_rotate(np.array(-now_point), -theta)
+
+    draw_params = {
+        "time_begin": time_step,
+        "lanelet_network": {"traffic_light": {"draw_traffic_lights": False}},
+    }
+
+    draw_object(
+        lanelet_network,
+        draw_params=draw_params,
+    )
+
+    plt.gca().set_axis_off()
+    plt.subplots_adjust(top=1, bottom=0, right=1, left=0, hspace=0, wspace=0)
+    plt.gca().set_aspect("equal")
+    plt.xlim(-watch_radius, watch_radius)
+    plt.ylim(-watch_radius, watch_radius)
+
+    draw_fig.canvas.draw()
+    plt.close(draw_fig)
+
+    # convert canvas to image
+    img = np.fromstring(draw_fig.canvas.tostring_rgb(), dtype=np.uint8, sep="")
+    img = img.reshape(draw_fig.canvas.get_width_height()[::-1] + (3,))
+
+    img_gray = ~cv2.cvtColor(img, cv2.COLOR_RGB2GRAY)
+
+    return img_gray
+
+
+def generate_nbr_array(trans_traj_list, time_step, pp=30, window_size=[18, 78], initial_time_step_list=None):
     """Generates the array of trajectories around the vehicle being predicted
 
     Arguments:
         trans_traj_list {[type]} -- [description]
         time_step {[type]} -- [description]
 
     Keyword Arguments:
         pp {int} -- [description] (default: {31})
         window_size {list} -- [description] (default: {[18, 78]})
 
     Returns:
         [type] -- [description]
     """
 
+    # Define initial_time_step list with zeros if None
+    if initial_time_step_list is None:
+        initial_time_step_list = [0] * len(trans_traj_list)
+
     # Define window to identify neihbors
     r1 = [int(-i / 2) for i in window_size]  # [-9, -39]
     r2 = [int(i / 2) for i in window_size]
 
     nbrs = np.zeros((3, 13, pp, 2))
     pir_list = []
-    for nbr in trans_traj_list:
+    for nbr, init_ts in zip(trans_traj_list, initial_time_step_list):
         try:
             now_point_nbr = nbr[time_step]
         except IndexError:
             continue
 
         pir = point_in_rectangle(r1, r2, now_point_nbr)
         if pir:
             nbr_tmp = []
             for i in reversed(range(pp)):
-                if time_step - i >= 0:
-                    nbr_tmp.append(nbr[time_step - i])
+                if time_step - (i + init_ts) >= 0:
+                    nbr_tmp.append(nbr[time_step - (i + init_ts)])
                 else:
                     nbr_tmp.append([np.nan, np.nan])
 
             nbrs[pir] = nbr_tmp
             pir_list.append(pir)
 
     return nbrs, pir_list, r1, r2
```

### Comparing `wale-net-3.0.1/prediction/utils/visualization.py` & `wale-net-3.0.2/prediction/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.1/setup.py` & `wale-net-3.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 
 
 def git(*args):
     return subprocess.check_output(["git"] + list(args))
 
 
 # get latest tag
-# latest = git("describe", "--tags").decode().strip()
-# latest = latest.split("-")[0]
+latest = git("describe", "--tags").decode().strip()
+latest = latest.split("-")[0]
 # for pypi package the tag must be set manually
-latest = "3.0.1"
+latest = "3.0.2"
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 
 long_description = """
 This package provides a Recurrent Neural Network (RNN) for vehicle trajectory prediction with uncertainties.
```

### Comparing `wale-net-3.0.1/wale_net.egg-info/PKG-INFO` & `wale-net-3.0.2/wale_net.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 Metadata-Version: 2.1
 Name: wale-net
-Version: 3.0.1
+Version: 3.0.2
 Summary: Prediction module for CommonRoad
 Home-page: https://github.com/TUMFTM/Wale-Net
 Author: Maximilian Geisslinger, Phillip Karle
 Author-email: maximilian.geisslinger@tum.de, karle@ftm.mw.tum.de
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 This package provides a Recurrent Neural Network (RNN) for vehicle trajectory prediction with uncertainties.
 It builds up on the work of [Convolutional Social Pooling](https://github.com/nachiket92/conv-social-pooling).
 It has been adapted to CommonRoad and extended by the ability of scene understanding and online learning.
 
 For further information see the Readme here:
 https://github.com/TUMFTM/Wale-Net
-
-
```

### Comparing `wale-net-3.0.1/wale_net.egg-info/SOURCES.txt` & `wale-net-3.0.2/wale_net.egg-info/SOURCES.txt`

 * *Files identical despite different names*

