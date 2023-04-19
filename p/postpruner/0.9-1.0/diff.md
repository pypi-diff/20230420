# Comparing `tmp/postpruner-0.9.tar.gz` & `tmp/postpruner-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postpruner-0.9.tar", last modified: Wed Apr 19 23:23:22 2023, max compression
+gzip compressed data, was "postpruner-1.0.tar", last modified: Wed Apr 19 23:32:10 2023, max compression
```

## Comparing `postpruner-0.9.tar` & `postpruner-1.0.tar`

### file list

```diff
@@ -1,17 +1,43 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:23:22.893780 postpruner-0.9/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       52 2023-04-19 23:23:22.893780 postpruner-0.9/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3648 2023-04-19 22:11:32.000000 postpruner-0.9/README.md
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:23:22.893780 postpruner-0.9/postpruner/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:14:28.000000 postpruner-0.9/postpruner/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1680 2023-04-19 23:23:13.000000 postpruner-0.9/postpruner/__main__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4996 2023-04-19 22:11:32.000000 postpruner-0.9/postpruner/generate_lut.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7983 2023-04-19 23:19:06.000000 postpruner-0.9/postpruner/postpruner.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:23:22.893780 postpruner-0.9/postpruner.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       52 2023-04-19 23:23:22.000000 postpruner-0.9/postpruner.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      322 2023-04-19 23:23:22.000000 postpruner-0.9/postpruner.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-04-19 23:23:22.000000 postpruner-0.9/postpruner.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       56 2023-04-19 23:23:22.000000 postpruner-0.9/postpruner.egg-info/entry_points.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       58 2023-04-19 23:23:22.000000 postpruner-0.9/postpruner.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       11 2023-04-19 23:23:22.000000 postpruner-0.9/postpruner.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-04-19 23:23:22.893780 postpruner-0.9/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      407 2023-04-19 23:23:21.000000 postpruner-0.9/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:32:10.321321 postpruner-1.0/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       52 2023-04-19 23:32:10.321321 postpruner-1.0/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3648 2023-04-19 22:11:32.000000 postpruner-1.0/README.md
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:32:10.317321 postpruner-1.0/postpruner/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:14:28.000000 postpruner-1.0/postpruner/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1690 2023-04-19 23:29:53.000000 postpruner-1.0/postpruner/__main__.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:32:10.317321 postpruner-1.0/postpruner/dataset/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.0/postpruner/dataset/__init__.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:32:10.321321 postpruner-1.0/postpruner/dataset/evaluate/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.0/postpruner/dataset/evaluate/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1023 2023-04-19 23:29:53.000000 postpruner-1.0/postpruner/dataset/evaluate/glue.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1232 2023-04-19 23:31:54.000000 postpruner-1.0/postpruner/dataset/evaluate/nlp.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2094 2023-04-19 23:29:53.000000 postpruner-1.0/postpruner/dataset/evaluate/squad.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3804 2023-04-19 22:11:32.000000 postpruner-1.0/postpruner/dataset/glue.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    22749 2023-04-19 22:11:32.000000 postpruner-1.0/postpruner/dataset/squad.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:32:10.321321 postpruner-1.0/postpruner/efficiency/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.0/postpruner/efficiency/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1565 2023-04-19 22:11:32.000000 postpruner-1.0/postpruner/efficiency/latency.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1633 2023-04-19 22:11:32.000000 postpruner-1.0/postpruner/efficiency/mac.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5007 2023-04-19 23:29:53.000000 postpruner-1.0/postpruner/generate_lut.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     8092 2023-04-19 23:30:56.000000 postpruner-1.0/postpruner/postpruner.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:32:10.321321 postpruner-1.0/postpruner/prune/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.0/postpruner/prune/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1095 2023-04-19 23:29:53.000000 postpruner-1.0/postpruner/prune/fisher.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1303 2023-04-19 22:11:32.000000 postpruner-1.0/postpruner/prune/rearrange.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7610 2023-04-19 23:29:53.000000 postpruner-1.0/postpruner/prune/rescale.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7421 2023-04-19 23:29:53.000000 postpruner-1.0/postpruner/prune/search.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:32:10.321321 postpruner-1.0/postpruner/utils/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.0/postpruner/utils/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3307 2023-04-19 22:11:32.000000 postpruner-1.0/postpruner/utils/arch.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      689 2023-04-19 22:11:32.000000 postpruner-1.0/postpruner/utils/linalg.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      439 2023-04-19 22:11:32.000000 postpruner-1.0/postpruner/utils/meter.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      180 2023-04-19 22:11:32.000000 postpruner-1.0/postpruner/utils/schedule.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      807 2023-04-19 22:11:32.000000 postpruner-1.0/postpruner/utils/timer.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:32:10.317321 postpruner-1.0/postpruner.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       52 2023-04-19 23:32:10.000000 postpruner-1.0/postpruner.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      955 2023-04-19 23:32:10.000000 postpruner-1.0/postpruner.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-04-19 23:32:10.000000 postpruner-1.0/postpruner.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       56 2023-04-19 23:32:10.000000 postpruner-1.0/postpruner.egg-info/entry_points.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       58 2023-04-19 23:32:10.000000 postpruner-1.0/postpruner.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       11 2023-04-19 23:32:10.000000 postpruner-1.0/postpruner.egg-info/top_level.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-04-19 23:32:10.321321 postpruner-1.0/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      407 2023-04-19 23:32:07.000000 postpruner-1.0/setup.py
```

### Comparing `postpruner-0.9/README.md` & `postpruner-1.0/README.md`

 * *Files identical despite different names*

### Comparing `postpruner-0.9/postpruner/__main__.py` & `postpruner-1.0/postpruner/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # __main__.py
 
 import sys
-from .postpruner import run
+from postpruner.postpruner import run
 
 def main():
     import argparse
 
     parser = argparse.ArgumentParser()
     parser.add_argument("--model_name", type=str, required=True)
     parser.add_argument("--task_name", type=str, required=True, choices=[
```

### Comparing `postpruner-0.9/postpruner/generate_lut.py` & `postpruner-1.0/postpruner/generate_lut.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import math
 import os
 
 import torch
 import torch.nn as nn
 from transformers import AutoConfig
 
-from utils.timer import CPUTimer, GPUTimer
+from postpruner.utils.timer import CPUTimer, GPUTimer
 
 
 class BertMHA(nn.Module):
 
     def __init__(
         self,
         num_attention_heads,
```

### Comparing `postpruner-0.9/postpruner/postpruner.py` & `postpruner-1.0/postpruner/postpruner.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,24 +11,24 @@
     AutoModelForSequenceClassification,
     AutoModelForQuestionAnswering,
     AutoTokenizer,
     DataCollatorWithPadding,
     set_seed,
 )
 
-from .dataset.glue import glue_dataset, max_seq_length, avg_seq_length
-from .dataset.squad import squad_dataset
-from .efficiency.mac import compute_mask_mac
-from .efficiency.latency import estimate_latency
-from .prune.fisher import collect_mask_grads
-from .prune.search import search_mac, search_latency
-from .prune.rearrange import rearrange_mask
-from .prune.rescale import rescale_mask
-from evaluate.nlp import test_accuracy
-from .utils.schedule import get_pruning_schedule
+from postpruner.dataset.glue import glue_dataset, max_seq_length, avg_seq_length
+from postpruner.dataset.squad import squad_dataset
+from postpruner.efficiency.mac import compute_mask_mac
+from postpruner.efficiency.latency import estimate_latency
+from postpruner.prune.fisher import collect_mask_grads
+from postpruner.prune.search import search_mac, search_latency
+from postpruner.prune.rearrange import rearrange_mask
+from postpruner.prune.rescale import rescale_mask
+from postpruner.dataset.evaluate.nlp import test_accuracy
+from postpruner.utils.schedule import get_pruning_schedule
 
 
 logger = logging.getLogger(__name__)
 
 
 parser = argparse.ArgumentParser()
 parser.add_argument("--model_name", type=str, required=True)
```

