# Comparing `tmp/Fau_tools-1.4.2-2.tar.gz` & `tmp/fau_tools-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fau_tools-1.4.2-2.tar", last modified: Sat Mar 25 05:29:11 2023, max compression
+gzip compressed data, was "fau_tools-1.4.3.tar", max compression
```

## Comparing `Fau_tools-1.4.2-2.tar` & `fau_tools-1.4.3.tar`

### file list

```diff
@@ -1,25 +1,21 @@
-drwxr-xr-x   0 fau        (501) admin       (80)        0 2023-03-25 05:29:11.135601 Fau_tools-1.4.2-2/
-drwxr-xr-x   0 fau        (501) admin       (80)        0 2023-03-25 05:29:11.127729 Fau_tools-1.4.2-2/Fau_tools/
--rw-r--r--   0 fau        (501) admin       (80)      179 2022-09-17 06:01:57.000000 Fau_tools-1.4.2-2/Fau_tools/__init__.py
-drwxr-xr-x   0 fau        (501) admin       (80)        0 2023-03-25 05:29:11.130499 Fau_tools-1.4.2-2/Fau_tools/data_structure/
--rw-r--r--   0 fau        (501) admin       (80)       30 2022-11-07 07:34:00.000000 Fau_tools-1.4.2-2/Fau_tools/data_structure/__init__.py
--rw-r--r--   0 fau        (501) admin       (80)     3776 2023-03-24 08:19:16.000000 Fau_tools-1.4.2-2/Fau_tools/data_structure/data_structure.py
--rw-r--r--   0 fau        (501) admin       (80)     1038 2023-03-24 08:16:48.000000 Fau_tools-1.4.2-2/Fau_tools/data_structure/data_structure.pyi
--rw-r--r--   0 fau        (501) admin       (80)      678 2023-03-24 03:23:27.000000 Fau_tools-1.4.2-2/Fau_tools/pyproject.toml
-drwxr-xr-x   0 fau        (501) admin       (80)        0 2023-03-25 05:29:11.132983 Fau_tools-1.4.2-2/Fau_tools/torch_tools/
--rw-r--r--   0 fau        (501) admin       (80)       27 2022-09-17 05:48:40.000000 Fau_tools-1.4.2-2/Fau_tools/torch_tools/__init__.py
--rw-r--r--   0 fau        (501) admin       (80)    12027 2023-03-25 05:28:52.000000 Fau_tools-1.4.2-2/Fau_tools/torch_tools/torch_tools.py
--rw-r--r--   0 fau        (501) admin       (80)     1553 2023-03-24 08:00:32.000000 Fau_tools-1.4.2-2/Fau_tools/torch_tools/torch_tools.pyi
-drwxr-xr-x   0 fau        (501) admin       (80)        0 2023-03-25 05:29:11.134719 Fau_tools-1.4.2-2/Fau_tools/utility/
--rw-r--r--   0 fau        (501) admin       (80)       23 2022-09-17 05:58:01.000000 Fau_tools-1.4.2-2/Fau_tools/utility/__init__.py
--rw-r--r--   0 fau        (501) admin       (80)     8727 2023-03-24 06:33:55.000000 Fau_tools-1.4.2-2/Fau_tools/utility/utility.py
--rw-r--r--   0 fau        (501) admin       (80)      797 2023-03-24 02:36:31.000000 Fau_tools-1.4.2-2/Fau_tools/utility/utility.pyi
-drwxr-xr-x   0 fau        (501) admin       (80)        0 2023-03-25 05:29:11.129232 Fau_tools-1.4.2-2/Fau_tools.egg-info/
--rw-r--r--   0 fau        (501) admin       (80)      251 2023-03-25 05:29:11.000000 Fau_tools-1.4.2-2/Fau_tools.egg-info/PKG-INFO
--rw-r--r--   0 fau        (501) admin       (80)      519 2023-03-25 05:29:11.000000 Fau_tools-1.4.2-2/Fau_tools.egg-info/SOURCES.txt
--rw-r--r--   0 fau        (501) admin       (80)        1 2023-03-25 05:29:11.000000 Fau_tools-1.4.2-2/Fau_tools.egg-info/dependency_links.txt
--rw-r--r--   0 fau        (501) admin       (80)       10 2023-03-25 05:29:11.000000 Fau_tools-1.4.2-2/Fau_tools.egg-info/top_level.txt
--rw-r--r--   0 fau        (501) admin       (80)      251 2023-03-25 05:29:11.135236 Fau_tools-1.4.2-2/PKG-INFO
--rw-r--r--   0 fau        (501) admin       (80)     2680 2023-03-24 07:19:19.000000 Fau_tools-1.4.2-2/README.md
--rw-r--r--   0 fau        (501) admin       (80)       38 2023-03-25 05:29:11.135750 Fau_tools-1.4.2-2/setup.cfg
--rw-r--r--   0 fau        (501) admin       (80)      398 2023-03-25 05:29:06.000000 Fau_tools-1.4.2-2/setup.py
+-rw-r--r--   0        0        0     2680 2023-04-20 02:37:45.625671 fau_tools-1.4.3/README.md
+-rw-r--r--   0        0        0     6148 2023-01-07 12:47:38.094251 fau_tools-1.4.3/fau_tools/.DS_Store
+-rw-r--r--   0        0        0      179 2022-09-17 06:01:57.485247 fau_tools-1.4.3/fau_tools/__init__.py
+-rw-r--r--   0        0        0       30 2022-11-07 07:34:00.261010 fau_tools-1.4.3/fau_tools/data_structure/__init__.py
+-rw-r--r--   0        0        0      221 2022-11-07 08:03:32.272377 fau_tools-1.4.3/fau_tools/data_structure/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4683 2023-04-20 02:49:37.919630 fau_tools-1.4.3/fau_tools/data_structure/__pycache__/data_structure.cpython-310.pyc
+-rw-r--r--   0        0        0     3420 2023-04-20 02:46:11.824418 fau_tools-1.4.3/fau_tools/data_structure/data_structure.py
+-rw-r--r--   0        0        0      914 2023-04-20 02:46:11.824752 fau_tools-1.4.3/fau_tools/data_structure/data_structure.pyi
+-rw-r--r--   0        0        0      678 2023-03-24 03:23:27.260855 fau_tools-1.4.3/fau_tools/pyproject.toml
+-rw-r--r--   0        0        0       27 2022-09-17 05:48:40.673809 fau_tools-1.4.3/fau_tools/torch_tools/__init__.py
+-rw-r--r--   0        0        0      215 2022-09-18 01:31:17.722972 fau_tools-1.4.3/fau_tools/torch_tools/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     8154 2023-04-20 02:49:35.921881 fau_tools-1.4.3/fau_tools/torch_tools/__pycache__/torch_tools.cpython-310.pyc
+-rw-r--r--   0        0        0    10050 2023-04-20 02:47:54.439467 fau_tools-1.4.3/fau_tools/torch_tools/torch_tools.py
+-rw-r--r--   0        0        0     1440 2023-04-20 02:46:11.825456 fau_tools-1.4.3/fau_tools/torch_tools/torch_tools.pyi
+-rw-r--r--   0        0        0       23 2022-09-17 05:58:01.298778 fau_tools-1.4.3/fau_tools/utility/__init__.py
+-rw-r--r--   0        0        0      207 2022-09-18 01:31:17.726340 fau_tools-1.4.3/fau_tools/utility/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4470 2023-03-24 06:35:44.247630 fau_tools-1.4.3/fau_tools/utility/__pycache__/utility.cpython-310.pyc
+-rw-r--r--   0        0        0     8727 2023-03-24 06:33:55.632551 fau_tools-1.4.3/fau_tools/utility/utility.py
+-rw-r--r--   0        0        0      797 2023-03-24 02:36:31.555258 fau_tools-1.4.3/fau_tools/utility/utility.pyi
+-rw-r--r--   0        0        0      468 2023-04-20 02:56:20.565005 fau_tools-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0     3429 1970-01-01 00:00:00.000000 fau_tools-1.4.3/PKG-INFO
```

### Comparing `Fau_tools-1.4.2-2/Fau_tools/data_structure/data_structure.py` & `fau_tools-1.4.3/fau_tools/data_structure/data_structure.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,31 +74,27 @@
 
 
 class TrainRecorder:
   """Record the process of training."""
 
   def __init__(self):
     self.loss_list, self.accuracy_list = list(), list()
-    self.precision_list, self.recall_list, self.f1_list = list(), list(), list()
 
-  def update(self, loss_value, accuracy, precision, recall, f1):
+  def update(self, loss_value, accuracy):
     """
     Update the training recorder.
 
     Parameters
     ----------
     loss_value : the current loss value
     accuracy : the current accuracy rate
 
     """
     self.loss_list.append(loss_value)
     self.accuracy_list.append(accuracy)
-    self.precision_list.append(precision)
-    self.recall_list.append(recall)
-    self.f1_list.append(f1)
 
   def save(self, file_name):
     """
     Save the training process.
 
     Parameters
     ----------
@@ -107,18 +103,18 @@
     Returns
     -------
     will generate a csv_file; there are some columns recorded the values variation during training.
 
     """
     file_name = rf"{file_name}.csv"
     with open(rf"{file_name}", "w") as file:
-      col_list = ", ".join(("loss", "accuracy", "precision", "recall", "f1")) + "\n"
+      col_list = ", ".join(("loss", "accuracy")) + "\n"
       file.write(col_list)
-      for loss, accuracy, precision, recall, f1 in zip(self.loss_list, self.accuracy_list, self.precision_list, self.recall_list, self.f1_list):
-        line = f"{loss:.6f}, {accuracy:.6f}, {precision:.6f}, {recall:.6f}, {f1:.6f}\n"
+      for loss, accuracy in zip(self.loss_list, self.accuracy_list):
+        line = f"{loss:.6f}, {accuracy:.6f}\n"
         file.write(line)
 
     cprint(rf"{__class__.__name__}: save a record file named {file_name} successfully!", "green")
```

### Comparing `Fau_tools-1.4.2-2/Fau_tools/data_structure/data_structure.pyi` & `fau_tools-1.4.3/fau_tools/data_structure/data_structure.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -20,19 +20,16 @@
 
 
 
 class TrainRecorder:
   def __init__(self):
     self.loss_list: list
     self.accuracy_list: list
-    self.precision_list: list
-    self.recall_list: list
-    self.f1_list: list
 
-  def update(self, loss_value: float, accuracy: float, precision: float, recall: float, f1: float) -> None: ...
+  def update(self, loss_value: float, accuracy: float) -> None: ...
 
   def save(self, file_name: str) -> None: ...
 
 
 
 class TimeManager:
   def __init__(self):
```

### Comparing `Fau_tools-1.4.2-2/Fau_tools/pyproject.toml` & `fau_tools-1.4.3/fau_tools/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Fau_tools-1.4.2-2/Fau_tools/torch_tools/torch_tools.py` & `fau_tools-1.4.3/fau_tools/torch_tools/torch_tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import pandas as pd
 import torch
 import matplotlib.pyplot as plt
 from matplotlib import ticker
-from sklearn.metrics import accuracy_score, precision_score, recall_score, f1_score, roc_curve
 
 from Fau_tools import utility
 from Fau_tools.data_structure import ModelManager, TimeManager, TrainRecorder
 from Fau_tools.utility import cprint
 
 
 
@@ -103,66 +102,14 @@
     accuracy: float = sum(test_result) / len(test_result)  # get average accuracy
 
   model.train()  # recover
   return round(accuracy, 6)
 
 
 
-def calc_evaluation_indicators(model, test_loader, DEVICE=None):
-  """
-  Calculate the evaluation indicators in the test dataset.
-
-  Added in version 1.4.2
-
-  Parameters
-  ----------
-  model : the training model
-  test_loader : the test data loader
-  DEVICE : cpu or cuda; if None, will be judged automatically
-
-  Returns
-  -------
-  The (accuracy, precision, recall, f1) evaluation indicators
-  in the test dataset. (Round to 6 decimal places)
-
-  """
-  if DEVICE is None: DEVICE = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
-
-  model.eval()  # evaluation mode
-
-  with torch.no_grad():
-    accuracy_list, precision_list = list(), list()
-    recall_list, f1_list = list(), list()
-    for (test_features, test_labels) in test_loader:
-      test_features, test_labels = test_features.to(DEVICE), test_labels.to(DEVICE)
-      test_output: torch.Tensor = model(test_features)
-      test_prediction: torch.Tensor = test_output.argmax(1)  # get classification result set
-      test_labels, test_prediction = test_labels.cpu(), test_prediction.cpu()
-
-      cur_accuracy  = accuracy_score(test_labels, test_prediction)
-      cur_precision = precision_score(test_labels, test_prediction, average="macro", zero_division=0)
-      cur_recall    = recall_score(test_labels, test_prediction, average="macro", zero_division=0)
-      cur_f1        = f1_score(test_labels, test_prediction, average="macro", zero_division=0)
-
-      accuracy_list.append(cur_accuracy)
-      precision_list.append(cur_precision)
-      recall_list.append(cur_recall)
-      f1_list.append(cur_f1)
-
-    accuracy: float  = sum(accuracy_list) / len(accuracy_list)
-    precision: float = sum(precision_list) / len(precision_list)
-    recall: float    = sum(recall_list) / len(recall_list)
-    f1: float        = sum(f1_list) / len(f1_list)
-
-  model.train()  # recover
-  return round(accuracy, 6), round(precision, 6), round(recall, 6), round(f1, 6)
-
-
-
-
 @utility.calc_time
 def torch_train(model, train_loader, test_loader, optimizer, loss_function, EPOCH=100, early_stop=None, name=None, save_model=True, DEVICE=None):
   """
   Train the model.
 
   Parameters
   ----------
@@ -210,31 +157,33 @@
   # begin training
   model = model.to(DEVICE); model.train()  # initialization
 
   # for showing training process
   time_manager = TimeManager()
 
   for epoch in range(EPOCH):
+    loss_list = list()
     for _, (train_x, train_y) in enumerate(train_loader):
       train_x, train_y = train_x.to(DEVICE), train_y.to(DEVICE)
       output: torch.Tensor = model(train_x)
       loss: torch.Tensor = loss_function(output, train_y)
+      loss_list.append(loss.item())
 
       optimizer.zero_grad()
       loss.backward()
       optimizer.step()
 
     # end of epoch
-    loss_value, (accuracy, precision, recall, f1) = loss.item(), calc_evaluation_indicators(model, test_loader)
+    loss_value, accuracy = sum(loss_list) / len(loss_list), calc_accuracy(model, test_loader, DEVICE)  # get loss and acc
     time_manager.time_tick()  # tick current time
     __show_progress(epoch, EPOCH, loss_value, accuracy, time_manager)
 
     # update and record
     model_manager.update(model, loss_value, accuracy, epoch)
-    train_recorder.update(loss_value, accuracy, precision, recall, f1)
+    train_recorder.update(loss_value, accuracy)
 
     # Judge early stop
     if early_stop is not None and __stop_training(epoch, model_manager, early_stop):
       cprint(f"Early stop: The model has gone through {early_stop} epochs without being optimized.", "yellow")
       break
```

### Comparing `Fau_tools-1.4.2-2/Fau_tools/torch_tools/torch_tools.pyi` & `fau_tools-1.4.3/fau_tools/torch_tools/torch_tools.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 # --------------- Function --- training
 # ------------------------------------------------------------
 
 def __show_progress(now: int, total: int, loss: float=None, accuracy: float=None, time_manager: TimeManager=None) -> None: ...
 
 def calc_accuracy(model: nn.Module, test_loader: tdata.DataLoader, DEVICE: torch.device=None) -> float: ...
 
-def calc_evaluation_indicators(model: nn.Module, test_loader: tdata.DataLoader, DEVICE: torch.device=None): ...
-
 def torch_train(model: nn.Module, train_loader: tdata.DataLoader, test_loader: tdata.DataLoader,
                 optimizer: torch.optim.Optimizer, loss_function: nn.Module, EPOCH: int=100, early_stop: int=None,
                 name: str=None, save_model: bool=True, DEVICE: torch.device=None) -> None: ...
 
 
 
 # ------------------------------------------------------------
```

### Comparing `Fau_tools-1.4.2-2/Fau_tools/utility/utility.py` & `fau_tools-1.4.3/fau_tools/utility/utility.py`

 * *Files identical despite different names*

### Comparing `Fau_tools-1.4.2-2/Fau_tools/utility/utility.pyi` & `fau_tools-1.4.3/fau_tools/utility/utility.pyi`

 * *Files identical despite different names*

### Comparing `Fau_tools-1.4.2-2/README.md` & `fau_tools-1.4.3/README.md`

 * *Files identical despite different names*

