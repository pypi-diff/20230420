# Comparing `tmp/mlpath-1.0.2.tar.gz` & `tmp/mlpath-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpath-1.0.2.tar", last modified: Sun Apr  9 10:41:37 2023, max compression
+gzip compressed data, was "mlpath-1.0.3.tar", last modified: Thu Apr 20 16:01:45 2023, max compression
```

## Comparing `mlpath-1.0.2.tar` & `mlpath-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-04-09 10:41:37.997042 mlpath-1.0.2/
--rw-r--r--   0 essam      (501) staff       (20)    18092 2023-03-22 10:05:32.000000 mlpath-1.0.2/LICENSE
--rw-r--r--   0 essam      (501) staff       (20)      192 2023-03-22 10:05:32.000000 mlpath-1.0.2/MANIFEST.in
--rw-r--r--   0 essam      (501) staff       (20)    17518 2023-04-09 10:41:37.996828 mlpath-1.0.2/PKG-INFO
--rw-r--r--   0 essam      (501) staff       (20)    16718 2023-03-22 10:57:02.000000 mlpath-1.0.2/README.md
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-04-09 10:41:37.994139 mlpath-1.0.2/mlpath/
--rw-r--r--   0 essam      (501) staff       (20)      122 2023-03-22 10:05:32.000000 mlpath-1.0.2/mlpath/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-04-09 10:41:37.995509 mlpath-1.0.2/mlpath/mldir_cli/
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-03-22 10:05:32.000000 mlpath-1.0.2/mlpath/mldir_cli/__init__.py
--rw-r--r--   0 essam      (501) staff       (20)     2049 2023-03-22 10:05:32.000000 mlpath-1.0.2/mlpath/mldir_cli/cli.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-04-09 10:41:37.996361 mlpath-1.0.2/mlpath/mlquest/
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-03-22 10:05:32.000000 mlpath-1.0.2/mlpath/mlquest/__init__.py
--rw-r--r--   0 essam      (501) staff       (20)    16563 2023-04-09 10:39:50.000000 mlpath-1.0.2/mlpath/mlquest/mlquest.py
--rw-r--r--   0 essam      (501) staff       (20)     7509 2023-03-22 10:05:32.000000 mlpath-1.0.2/mlpath/mlquest/utils.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-04-09 10:41:37.995231 mlpath-1.0.2/mlpath.egg-info/
--rw-r--r--   0 essam      (501) staff       (20)    17518 2023-04-09 10:41:37.000000 mlpath-1.0.2/mlpath.egg-info/PKG-INFO
--rw-r--r--   0 essam      (501) staff       (20)      369 2023-04-09 10:41:37.000000 mlpath-1.0.2/mlpath.egg-info/SOURCES.txt
--rw-r--r--   0 essam      (501) staff       (20)        1 2023-04-09 10:41:37.000000 mlpath-1.0.2/mlpath.egg-info/dependency_links.txt
--rw-r--r--   0 essam      (501) staff       (20)       85 2023-04-09 10:41:37.000000 mlpath-1.0.2/mlpath.egg-info/entry_points.txt
--rw-r--r--   0 essam      (501) staff       (20)       20 2023-04-09 10:41:37.000000 mlpath-1.0.2/mlpath.egg-info/requires.txt
--rw-r--r--   0 essam      (501) staff       (20)        7 2023-04-09 10:41:37.000000 mlpath-1.0.2/mlpath.egg-info/top_level.txt
--rw-r--r--   0 essam      (501) staff       (20)       38 2023-04-09 10:41:37.997120 mlpath-1.0.2/setup.cfg
--rw-r--r--   0 essam      (501) staff       (20)     2065 2023-04-09 10:41:34.000000 mlpath-1.0.2/setup.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-04-20 16:01:45.394504 mlpath-1.0.3/
+-rw-r--r--   0 essam      (501) staff       (20)    18092 2023-03-22 10:05:32.000000 mlpath-1.0.3/LICENSE
+-rw-r--r--   0 essam      (501) staff       (20)      192 2023-03-22 10:05:32.000000 mlpath-1.0.3/MANIFEST.in
+-rw-r--r--   0 essam      (501) staff       (20)    17606 2023-04-20 16:01:45.394237 mlpath-1.0.3/PKG-INFO
+-rw-r--r--   0 essam      (501) staff       (20)    16806 2023-04-20 16:01:05.000000 mlpath-1.0.3/README.md
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-04-20 16:01:45.390871 mlpath-1.0.3/mlpath/
+-rw-r--r--   0 essam      (501) staff       (20)      122 2023-03-22 10:05:32.000000 mlpath-1.0.3/mlpath/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-04-20 16:01:45.392537 mlpath-1.0.3/mlpath/mldir_cli/
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-03-22 10:05:32.000000 mlpath-1.0.3/mlpath/mldir_cli/__init__.py
+-rw-r--r--   0 essam      (501) staff       (20)     2049 2023-03-22 10:05:32.000000 mlpath-1.0.3/mlpath/mldir_cli/cli.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-04-20 16:01:45.393732 mlpath-1.0.3/mlpath/mlquest/
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-03-22 10:05:32.000000 mlpath-1.0.3/mlpath/mlquest/__init__.py
+-rw-r--r--   0 essam      (501) staff       (20)    19811 2023-04-20 14:39:55.000000 mlpath-1.0.3/mlpath/mlquest/mlquest.py
+-rw-r--r--   0 essam      (501) staff       (20)    10190 2023-04-20 15:47:31.000000 mlpath-1.0.3/mlpath/mlquest/utils.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-04-20 16:01:45.392195 mlpath-1.0.3/mlpath.egg-info/
+-rw-r--r--   0 essam      (501) staff       (20)    17606 2023-04-20 16:01:44.000000 mlpath-1.0.3/mlpath.egg-info/PKG-INFO
+-rw-r--r--   0 essam      (501) staff       (20)      369 2023-04-20 16:01:45.000000 mlpath-1.0.3/mlpath.egg-info/SOURCES.txt
+-rw-r--r--   0 essam      (501) staff       (20)        1 2023-04-20 16:01:44.000000 mlpath-1.0.3/mlpath.egg-info/dependency_links.txt
+-rw-r--r--   0 essam      (501) staff       (20)       85 2023-04-20 16:01:45.000000 mlpath-1.0.3/mlpath.egg-info/entry_points.txt
+-rw-r--r--   0 essam      (501) staff       (20)       20 2023-04-20 16:01:45.000000 mlpath-1.0.3/mlpath.egg-info/requires.txt
+-rw-r--r--   0 essam      (501) staff       (20)        7 2023-04-20 16:01:45.000000 mlpath-1.0.3/mlpath.egg-info/top_level.txt
+-rw-r--r--   0 essam      (501) staff       (20)       38 2023-04-20 16:01:45.394592 mlpath-1.0.3/setup.cfg
+-rw-r--r--   0 essam      (501) staff       (20)     2065 2023-04-20 16:01:31.000000 mlpath-1.0.3/setup.py
```

### Comparing `mlpath-1.0.2/LICENSE` & `mlpath-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mlpath-1.0.2/PKG-INFO` & `mlpath-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpath
-Version: 1.0.2
+Version: 1.0.3
 Summary: A lightweight api for machine and deep learning experiment logging in the form of a python library. 
 Home-page: https://mlpath.readthedocs.io/
 Author: Essam W., Abdullah A.
 Author-email: essamwisam@outlook.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -70,18 +70,21 @@
 # Model Initialization
 model = l(RadialBasisNet)(x_data_f, 99, 19, 31)
 
 # Model Training
 accuracy = train_model(model)
 
 # log the accuracy
-mlq.log_metrics(accuracy)        # can also do mlq.log_metric(acc=accuracy) so its logged as acc
+mlq.log_metrics(accuracy)                             # pass acc=accuracy to log as acc
 
 mlq.end_quest()
 
+mlq.show_table('Radial Basis Pipeline', last_k=10)    # show the table for the last 10 runs
+```
+
 ```
 After three runs, the markdown file under the ```Quests``` folder has
 <table>
 <tr>
 <th colspan=4 style="text-align: center; vertical-align: middle;">info</th>
 <th colspan=3 style="text-align: center; vertical-align: middle;">Preprocessing</th>
 <th colspan=3 style="text-align: center; vertical-align: middle;">FeatureExtraction</th>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mlpath Version: 1.0.2 Summary: A lightweight api
+Metadata-Version: 2.1 Name: mlpath Version: 1.0.3 Summary: A lightweight api
 for machine and deep learning experiment logging in the form of a python
 library. Home-page: https://mlpath.readthedocs.io/ Author: Essam W., Abdullah
 A. Author-email: essamwisam@outlook.com License: GPLv3 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
@@ -25,17 +25,18 @@
 mlquest as mlq l = mlq.l # Start a new quest, this corresponds to a table where
 every run of the Python file will be logged. mlq.start_quest('Radial Basis
 Pipeline', log_defs=False) # Preprocessing x_data_p = l(Preprocessing)(x_data=
 [1, 2, 3], alpha=1114, beta_param=2, c=925) # Feature Extraction x_data_f = l
 (FeatureExtraction)(x_data_p, 32, 50, 4) # x_data_p is an array so it won't be
 logged. # Model Initialization model = l(RadialBasisNet)(x_data_f, 99, 19, 31)
 # Model Training accuracy = train_model(model) # log the accuracy
-mlq.log_metrics(accuracy) # can also do mlq.log_metric(acc=accuracy) so its
-logged as acc mlq.end_quest() ``` After three runs, the markdown file under the
-```Quests``` folder has
+mlq.log_metrics(accuracy) # pass acc=accuracy to log as acc mlq.end_quest()
+mlq.show_table('Radial Basis Pipeline', last_k=10) # show the table for the
+last 10 runs ``` ``` After three runs, the markdown file under the ```Quests```
+folder has
 info                     Preprocessing FeatureExtraction RadialBasisNet metrics
 16:31: 02/11/ 1.01 min 1 74   12 95    13  530 4         99 99 3        50
 16     23
 16:32: 02/11/ 4.91 ms  2 14   2  95    132 530 4         99 19 3        70
 40     23
 16:32: 02/11/ 4.93 ms  3 1114 2  925   32  50  4         99 19 31       70
 57     23
```

### Comparing `mlpath-1.0.2/README.md` & `mlpath-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,18 +49,21 @@
 # Model Initialization
 model = l(RadialBasisNet)(x_data_f, 99, 19, 31)
 
 # Model Training
 accuracy = train_model(model)
 
 # log the accuracy
-mlq.log_metrics(accuracy)        # can also do mlq.log_metric(acc=accuracy) so its logged as acc
+mlq.log_metrics(accuracy)                             # pass acc=accuracy to log as acc
 
 mlq.end_quest()
 
+mlq.show_table('Radial Basis Pipeline', last_k=10)    # show the table for the last 10 runs
+```
+
 ```
 After three runs, the markdown file under the ```Quests``` folder has
 <table>
 <tr>
 <th colspan=4 style="text-align: center; vertical-align: middle;">info</th>
 <th colspan=3 style="text-align: center; vertical-align: middle;">Preprocessing</th>
 <th colspan=3 style="text-align: center; vertical-align: middle;">FeatureExtraction</th>
```

#### html2text {}

```diff
@@ -15,17 +15,18 @@
 mlquest as mlq l = mlq.l # Start a new quest, this corresponds to a table where
 every run of the Python file will be logged. mlq.start_quest('Radial Basis
 Pipeline', log_defs=False) # Preprocessing x_data_p = l(Preprocessing)(x_data=
 [1, 2, 3], alpha=1114, beta_param=2, c=925) # Feature Extraction x_data_f = l
 (FeatureExtraction)(x_data_p, 32, 50, 4) # x_data_p is an array so it won't be
 logged. # Model Initialization model = l(RadialBasisNet)(x_data_f, 99, 19, 31)
 # Model Training accuracy = train_model(model) # log the accuracy
-mlq.log_metrics(accuracy) # can also do mlq.log_metric(acc=accuracy) so its
-logged as acc mlq.end_quest() ``` After three runs, the markdown file under the
-```Quests``` folder has
+mlq.log_metrics(accuracy) # pass acc=accuracy to log as acc mlq.end_quest()
+mlq.show_table('Radial Basis Pipeline', last_k=10) # show the table for the
+last 10 runs ``` ``` After three runs, the markdown file under the ```Quests```
+folder has
 info                     Preprocessing FeatureExtraction RadialBasisNet metrics
 16:31: 02/11/ 1.01 min 1 74   12 95    13  530 4         99 99 3        50
 16     23
 16:32: 02/11/ 4.91 ms  2 14   2  95    132 530 4         99 19 3        70
 40     23
 16:32: 02/11/ 4.93 ms  3 1114 2  925   32  50  4         99 19 31       70
 57     23
```

### Comparing `mlpath-1.0.2/mlpath/mldir_cli/cli.py` & `mlpath-1.0.3/mlpath/mldir_cli/cli.py`

 * *Files identical despite different names*

### Comparing `mlpath-1.0.2/mlpath/mlquest/mlquest.py` & `mlpath-1.0.3/mlpath/mlquest/mlquest.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import warnings
 import inspect
 from varname import  argname
 from copy import copy
 import pickle
 import os
 import json
+from IPython.display import display, Markdown, HTML
 
 class mlquest():
     '''
     The mlquest class provides methods and attributes to log machine learning experiments.
     '''
     quests = {}             # dictionary of quests (e.g, one for each model) that contains a list of logs (runs)
     log = {}                     # dictionary of the current log (run)
@@ -67,14 +68,15 @@
          mlquest.active = True
          mlquest.log['info'] = {}
          mlquest.log['info']['name'] = quest_name
          mlquest.start_time = time.time()
          mlquest.log['info']['time'] =  time.strftime('%X') 
          mlquest.log['info']['date'] = time.strftime('%x')
    
+   
     @staticmethod
     def clear():
        '''
         Clear the log record of the current run. You may use it while handling exceptions or debugging.
        '''
        if mlquest.active == False: warnings.warn("Attempting to clear the current run when no run is active will do nothing")
        mlquest.log = {}
@@ -298,20 +300,56 @@
          else:
             id = 1
             mlquest.log['info']['id'] = id
             quest_name = mlquest.log['info']['name']
             mlquest.quests[quest_name] = [mlquest.log]
          utils.runs_to_json(mlquest.relative_path, mlquest.curr_dir, mlquest.quests[quest_name], quest_name, mlquest.log_defs, mlquest.non_default_log)
          utils.json_to_html_table(mlquest.relative_path, mlquest.curr_dir, f'Quests/{mlquest.curr_dir}/{quest_name}/json/{quest_name}.json',
-                                  f'Quests/{mlquest.curr_dir}/{quest_name}/json/{quest_name}-config.json',  quest_name)
+                                  f'Quests/{mlquest.curr_dir}/{quest_name}/json/{quest_name}-config.json',  quest_name, last_k=None, save=True)
          mlquest.active = False
          mlquest.log = {}
          mlquest.save_quest(quest_name)
          
+   
+    @staticmethod
+    def show_logs(quest_name,  table_dest='', last_k=None):
+      '''
+      Shows the logs of a quest in a table.
+      
+      :param quest_name: The name of the quest to show the logs of
+      :type quest_name: string
+      :param log_defs: Whether to show the log defaults or not
+      :type log_defs: bool
+      :param table_dest: The destination of the Quests folder
+      :type table_dest: string
+      
+      :Example:
+      
+      >>> mlq.show_logs('NaiveBayesExp')
+      
+      This would show the logs of the NaiveBayesExp quest as saved in :samp:`../Quests/<ParentFolder>/NaiveBayesExp/`
          
+      '''
+      # get the name of the folder containing the current file
+      mlquest.relative_path = table_dest
+      mlquest.curr_dir = os.path.basename(os.getcwd())
+      assert os.path.exists(f'{mlquest.relative_path}Quests/{mlquest.curr_dir}/{quest_name}'), f'Quest {quest_name} does not exist yet. Please start a quest with that name first.'
+         
+      if 'quests.mlq' in os.listdir(f'{mlquest.relative_path}Quests/{mlquest.curr_dir}/{quest_name}'):
+         with open(mlquest.relative_path + f'Quests/{mlquest.curr_dir}/{quest_name}/quests.mlq', 'rb') as f:
+            mlquest.quests = pickle.load(f)
+            
+      # convert the file to html table
+      table = utils.json_to_html_table(mlquest.relative_path, mlquest.curr_dir, f'Quests/{mlquest.curr_dir}/{quest_name}/json/{quest_name}.json',
+                                 f'Quests/{mlquest.curr_dir}/{quest_name}/json/{quest_name}-config.json',  quest_name, last_k)
+            
+            
+      # display the table
+      display(HTML(table))
+      
     @staticmethod
     def delete_runs(table_dest, quest_name, run_ids):
       '''
       permanently deletes runs that have ids in run_ids from the log.
       
       :param table_dest: The destination of the Quests folder
       :type table_dest: string
@@ -335,15 +373,14 @@
       '''
       curr_dir = os.path.basename(os.getcwd())
       
       # read the mlq file from table_dest and quest_name
       with open(f'{table_dest}Quests/{curr_dir}/{quest_name}/quests.mlq', 'rb') as f:
          data = dict(pickle.load(f))
          
-      
       for run_id in run_ids:
          # loop on the runs and delete the run with the given id
          for i, run in enumerate(data[quest_name]):
             if run['info']['id'] == run_id:
                del data[quest_name][i]
                break
             if i == len(data[quest_name])-1:
@@ -351,9 +388,44 @@
       
       # save the data to the mlq file
       with open(f'{table_dest}Quests/{curr_dir}/{quest_name}/quests.mlq', 'wb') as f:
          pickle.dump(data, f)
          
       # update the json and html files
       utils.runs_to_json(table_dest, curr_dir, data[quest_name], quest_name, None, None)
-      utils.json_to_html_table(table_dest, curr_dir, f'Quests/{curr_dir}/{quest_name}/json/{quest_name}.json', f'Quests/{curr_dir}/{quest_name}/json/{quest_name}-config.json',  quest_name)
-         
+      utils.json_to_html_table(table_dest, curr_dir, f'Quests/{curr_dir}/{quest_name}/json/{quest_name}.json', f'Quests/{curr_dir}/{quest_name}/json/{quest_name}-config.json',  quest_name, last_k=None, save=True)
+         
+         
+    @staticmethod
+    def get_col_logs(quest_name, col_name, sub_col_name, table_dest=''):
+      '''
+      Returns a list of values of a column in the log of a quest.
+      
+      :param quest_name: The name of the quest to get the column from
+      :type quest_name: string
+      :param col_name: The name of the column to get the values from
+      :type col_name: string
+      :param sub_col_name: The name of the sub-column to get the values from
+      :type sub_col_name: string
+      :param table_dest: The destination of the Quests folder
+      :type table_dest: string
+      
+      :Example:
+      
+      >>> mlq.get_logs('NaiveBayesExp', 'metrics', 'accuracy')
+      
+      This would return a list of the accuracy values of the runs in the NaiveBayesExp quest found in :samp:`../Quests/<ParentFolder>/NaiveBayesExp/`
+      
+      '''
+      # get the name of the folder containing the current file
+      mlquest.relative_path = table_dest
+      mlquest.curr_dir = os.path.basename(os.getcwd())
+      assert os.path.exists(f'{mlquest.relative_path}Quests/{mlquest.curr_dir}/{quest_name}'), f'Quest {quest_name} does not exist yet. Please start a quest with that name first.'
+         
+      # get the data from the json file
+      with open(mlquest.relative_path + f'Quests/{mlquest.curr_dir}/{quest_name}/json/{quest_name}.json', 'r') as f:
+         table = json.load(f)
+      
+      # get the values of the column
+      column = table[col_name][sub_col_name]
+      
+      return column
```

### Comparing `mlpath-1.0.2/mlpath/mlquest/utils.py` & `mlpath-1.0.3/mlpath/mlquest/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -35,17 +35,82 @@
       subkeys = [item for sublist in subkeys for item in sublist]
       subkeys = unique(subkeys)
       for subkey in subkeys:
             values = [d.get(key, {}).get(subkey) for d in dict_list]    # None if not found
             big_dict[key][subkey] = values
    return big_dict
 
+
+def remove_duplicate_rows(json_obj):
+   '''
+      Removes duplicate rows from the given nested json_obj which is expected to be a
+      two-level nested dictionary where the values are lists representing column values.      
+   '''
+   # read json file from path as dict
+   num_rows = len(json_obj['info']['id'])
+   rows_to_remove = []
+   old_row_values, new_row_values = [], []
+   for i in range(num_rows):
+      for key in json_obj.keys():
+         for subkey in json_obj[key].keys():
+            value = json_obj[key][subkey][i]
+            # if the key is not info then append the value to the list
+            if key != 'info':     new_row_values.append(value)
+      
+      if new_row_values == old_row_values:
+         rows_to_remove.append(i)
+         
+      old_row_values = new_row_values
+      new_row_values = []
+   
+   # remove the duplicate rows
+   for i in range(len(rows_to_remove)-1, -1, -1):
+      k = rows_to_remove[i]
+      for key in json_obj.keys():
+         for subkey in json_obj[key].keys():
+            json_obj[key][subkey].pop(k)
+            
+   return json_obj
+      
+
+def get_path_mask(json_obj):
+   '''
+   Given a json_obj return a mask_obj of the same structure (two level dictionary of keys and subkeys
+   and where values are lists) this returns a mask of the same shape as the json_obj but where if a value
+   is different from the previous row then it is a 1, otherwise it is a 0.
+   '''
+   # make mask obj of the same structure as json_obj
+   mask_obj = {}
+   for key in json_obj.keys():
+      mask_obj[key] = {}
+      for subkey in json_obj[key].keys():
+         mask_obj[key][subkey] = []
+         
+   num_rows = len(json_obj['info']['id'])
+   for i in range(num_rows):
+      for key in json_obj.keys():
+         for subkey in json_obj[key].keys():
+            value = json_obj[key][subkey][i]
+            if key != 'info':
+               if i != 0:
+                  if value != json_obj[key][subkey][i-1]:
+                     mask_obj[key][subkey].append(1)
+                  else :
+                     mask_obj[key][subkey].append(0)
+               else:
+                  mask_obj[key][subkey].append(0)
+            else:
+               mask_obj[key][subkey].append(0)
+   return mask_obj
+            
+
+         
+
        
-       
-def json_to_html_table(relative_path, curr_dir, json_path, config_path, quest_name):
+def json_to_html_table(relative_path, curr_dir, json_path, config_path, quest_name, last_k, colored=True, save=False):
    '''
       Makes an html table from a nested json file. 
       
       :param json_path: The path to the json file
       :type json_path: string
       
       :param quest_name: The name of the quest to be converted
@@ -53,48 +118,61 @@
    '''
    # read json file from path as dict
    with open(relative_path + json_path, 'rb') as JSON:
       json_obj = json.load(JSON)
    with open(relative_path + config_path, 'rb') as JSON:
       config_obj = json.load(JSON)
    
+   json_obj = remove_duplicate_rows(json_obj)
+   mask_obj = get_path_mask(json_obj)
    # convert to html table
    table = '<table>\n'
    # make a header row
    table += '<tr>\n'
    # for each key in the top-level dict make a column with colspan being the number of subkeys
    for key in json_obj.keys():
       # the length of the colspan is the number of subkeys with value 'true' in the config file
       length = [config_obj[key][subkey] for subkey in config_obj[key].keys()].count('true')
       if length > 0 : 
          table += f'<th colspan={length} style="text-align: center; vertical-align: middle;">{key}</th>\n'
    table += '</tr>\n'
+   
    # for each subkey of the top-level dict, make a subheader row
    for key in json_obj.keys():
       for subkey in json_obj[key].keys():
          if config_obj[key][subkey] == 'true':
             table += f'<th style="text-align: center; vertical-align: middle;">{subkey}</th>\n'
    table += '</tr>\n'
+   
+   
    # get the number of ids to infer the number of rows
    num_rows = len(json_obj['info']['id'])
-   for i in range(num_rows):
+   if last_k is None:      last_k = num_rows
+   if last_k > num_rows:     last_k = num_rows
+   
+   
+   for i in range(num_rows - last_k, num_rows):
       table += '<tr>\n'
       for key in json_obj.keys():
          for subkey in json_obj[key].keys():
             if config_obj[key][subkey] == 'true':
+               color = 'yellow' if mask_obj[key][subkey][i] and colored else 'white'
                value = json_obj[key][subkey][i] if json_obj[key][subkey][i] is not None else ''
-               table += f'<td style="text-align: center; vertical-align: middle;">{value}</td>\n'
+               table += f'<td style="text-align: center; vertical-align: middle;"> <font color={color}>{value}</font></td>\n'
       table += '</tr>\n'
 
-
    # save the html file
-   if not os.path.exists(f'{relative_path}Quests/{curr_dir}/{quest_name}'):
-      os.makedirs(f'{relative_path}Quests/{curr_dir}/{quest_name}')
-   with open(relative_path + f'Quests/{curr_dir}/{quest_name}/{quest_name}.md', 'w') as f:
-      f.write(table)
+   if save:
+      if not os.path.exists(f'{relative_path}Quests/{curr_dir}/{quest_name}'):
+         os.makedirs(f'{relative_path}Quests/{curr_dir}/{quest_name}')
+      with open(relative_path + f'Quests/{curr_dir}/{quest_name}/{quest_name}.md', 'w') as f:
+         f.write(table)
+   
+   # return the html table
+   return table
    
       
     
 def runs_to_json(relative_path, curr_dir, runs, quest_name, log_defs, non_default_log):
    '''
    converts the runs of a quest to a json file
    :param quest_name: The name of the quest to be converted
```

### Comparing `mlpath-1.0.2/mlpath.egg-info/PKG-INFO` & `mlpath-1.0.3/mlpath.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpath
-Version: 1.0.2
+Version: 1.0.3
 Summary: A lightweight api for machine and deep learning experiment logging in the form of a python library. 
 Home-page: https://mlpath.readthedocs.io/
 Author: Essam W., Abdullah A.
 Author-email: essamwisam@outlook.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -70,18 +70,21 @@
 # Model Initialization
 model = l(RadialBasisNet)(x_data_f, 99, 19, 31)
 
 # Model Training
 accuracy = train_model(model)
 
 # log the accuracy
-mlq.log_metrics(accuracy)        # can also do mlq.log_metric(acc=accuracy) so its logged as acc
+mlq.log_metrics(accuracy)                             # pass acc=accuracy to log as acc
 
 mlq.end_quest()
 
+mlq.show_table('Radial Basis Pipeline', last_k=10)    # show the table for the last 10 runs
+```
+
 ```
 After three runs, the markdown file under the ```Quests``` folder has
 <table>
 <tr>
 <th colspan=4 style="text-align: center; vertical-align: middle;">info</th>
 <th colspan=3 style="text-align: center; vertical-align: middle;">Preprocessing</th>
 <th colspan=3 style="text-align: center; vertical-align: middle;">FeatureExtraction</th>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mlpath Version: 1.0.2 Summary: A lightweight api
+Metadata-Version: 2.1 Name: mlpath Version: 1.0.3 Summary: A lightweight api
 for machine and deep learning experiment logging in the form of a python
 library. Home-page: https://mlpath.readthedocs.io/ Author: Essam W., Abdullah
 A. Author-email: essamwisam@outlook.com License: GPLv3 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
@@ -25,17 +25,18 @@
 mlquest as mlq l = mlq.l # Start a new quest, this corresponds to a table where
 every run of the Python file will be logged. mlq.start_quest('Radial Basis
 Pipeline', log_defs=False) # Preprocessing x_data_p = l(Preprocessing)(x_data=
 [1, 2, 3], alpha=1114, beta_param=2, c=925) # Feature Extraction x_data_f = l
 (FeatureExtraction)(x_data_p, 32, 50, 4) # x_data_p is an array so it won't be
 logged. # Model Initialization model = l(RadialBasisNet)(x_data_f, 99, 19, 31)
 # Model Training accuracy = train_model(model) # log the accuracy
-mlq.log_metrics(accuracy) # can also do mlq.log_metric(acc=accuracy) so its
-logged as acc mlq.end_quest() ``` After three runs, the markdown file under the
-```Quests``` folder has
+mlq.log_metrics(accuracy) # pass acc=accuracy to log as acc mlq.end_quest()
+mlq.show_table('Radial Basis Pipeline', last_k=10) # show the table for the
+last 10 runs ``` ``` After three runs, the markdown file under the ```Quests```
+folder has
 info                     Preprocessing FeatureExtraction RadialBasisNet metrics
 16:31: 02/11/ 1.01 min 1 74   12 95    13  530 4         99 99 3        50
 16     23
 16:32: 02/11/ 4.91 ms  2 14   2  95    132 530 4         99 19 3        70
 40     23
 16:32: 02/11/ 4.93 ms  3 1114 2  925   32  50  4         99 19 31       70
 57     23
```

### Comparing `mlpath-1.0.2/setup.py` & `mlpath-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         requirements = f.read().splitlines()
     return requirements
 
 
 # This call to setup() does all the work
 setup(
     name="mlpath",
-    version="1.0.2",
+    version="1.0.3",
     description="A lightweight api for machine and deep learning experiment logging in the form of a python library. ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://mlpath.readthedocs.io/",
     author="Essam W., Abdullah A.",
     author_email="essamwisam@outlook.com",
     license="GPLv3",
```

