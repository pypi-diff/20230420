# Comparing `tmp/postpruner-1.1.1.tar.gz` & `tmp/postpruner-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postpruner-1.1.1.tar", last modified: Wed Apr 19 23:41:43 2023, max compression
+gzip compressed data, was "postpruner-1.1.2.tar", last modified: Wed Apr 19 23:44:23 2023, max compression
```

## Comparing `postpruner-1.1.1.tar` & `postpruner-1.1.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:41:43.464822 postpruner-1.1.1/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       54 2023-04-19 23:41:43.460822 postpruner-1.1.1/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3648 2023-04-19 22:11:32.000000 postpruner-1.1.1/README.md
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:41:43.456822 postpruner-1.1.1/postpruner/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:14:28.000000 postpruner-1.1.1/postpruner/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1779 2023-04-19 23:40:52.000000 postpruner-1.1.1/postpruner/__main__.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:41:43.460822 postpruner-1.1.1/postpruner/dataset/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.1.1/postpruner/dataset/__init__.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:41:43.460822 postpruner-1.1.1/postpruner/dataset/evaluate/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.1.1/postpruner/dataset/evaluate/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1023 2023-04-19 23:29:53.000000 postpruner-1.1.1/postpruner/dataset/evaluate/glue.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1232 2023-04-19 23:31:54.000000 postpruner-1.1.1/postpruner/dataset/evaluate/nlp.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2094 2023-04-19 23:29:53.000000 postpruner-1.1.1/postpruner/dataset/evaluate/squad.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3804 2023-04-19 22:11:32.000000 postpruner-1.1.1/postpruner/dataset/glue.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    22749 2023-04-19 22:11:32.000000 postpruner-1.1.1/postpruner/dataset/squad.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:41:43.460822 postpruner-1.1.1/postpruner/efficiency/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.1.1/postpruner/efficiency/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1565 2023-04-19 22:11:32.000000 postpruner-1.1.1/postpruner/efficiency/latency.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1633 2023-04-19 22:11:32.000000 postpruner-1.1.1/postpruner/efficiency/mac.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5007 2023-04-19 23:29:53.000000 postpruner-1.1.1/postpruner/generate_lut.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6931 2023-04-19 23:41:34.000000 postpruner-1.1.1/postpruner/postpruner.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:41:43.460822 postpruner-1.1.1/postpruner/prune/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.1.1/postpruner/prune/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1095 2023-04-19 23:29:53.000000 postpruner-1.1.1/postpruner/prune/fisher.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1303 2023-04-19 22:11:32.000000 postpruner-1.1.1/postpruner/prune/rearrange.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7610 2023-04-19 23:29:53.000000 postpruner-1.1.1/postpruner/prune/rescale.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7421 2023-04-19 23:29:53.000000 postpruner-1.1.1/postpruner/prune/search.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:41:43.460822 postpruner-1.1.1/postpruner/utils/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.1.1/postpruner/utils/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3307 2023-04-19 22:11:32.000000 postpruner-1.1.1/postpruner/utils/arch.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      689 2023-04-19 22:11:32.000000 postpruner-1.1.1/postpruner/utils/linalg.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      439 2023-04-19 22:11:32.000000 postpruner-1.1.1/postpruner/utils/meter.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      180 2023-04-19 22:11:32.000000 postpruner-1.1.1/postpruner/utils/schedule.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      807 2023-04-19 22:11:32.000000 postpruner-1.1.1/postpruner/utils/timer.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:41:43.456822 postpruner-1.1.1/postpruner.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       54 2023-04-19 23:41:43.000000 postpruner-1.1.1/postpruner.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      955 2023-04-19 23:41:43.000000 postpruner-1.1.1/postpruner.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-04-19 23:41:43.000000 postpruner-1.1.1/postpruner.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       56 2023-04-19 23:41:43.000000 postpruner-1.1.1/postpruner.egg-info/entry_points.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       58 2023-04-19 23:41:43.000000 postpruner-1.1.1/postpruner.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       11 2023-04-19 23:41:43.000000 postpruner-1.1.1/postpruner.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-04-19 23:41:43.464822 postpruner-1.1.1/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      409 2023-04-19 23:41:40.000000 postpruner-1.1.1/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:44:23.764683 postpruner-1.1.2/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       54 2023-04-19 23:44:23.764683 postpruner-1.1.2/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3648 2023-04-19 22:11:32.000000 postpruner-1.1.2/README.md
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:44:23.756683 postpruner-1.1.2/postpruner/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:14:28.000000 postpruner-1.1.2/postpruner/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1684 2023-04-19 23:43:36.000000 postpruner-1.1.2/postpruner/__main__.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:44:23.760683 postpruner-1.1.2/postpruner/dataset/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.1.2/postpruner/dataset/__init__.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:44:23.760683 postpruner-1.1.2/postpruner/dataset/evaluate/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.1.2/postpruner/dataset/evaluate/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1023 2023-04-19 23:29:53.000000 postpruner-1.1.2/postpruner/dataset/evaluate/glue.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1232 2023-04-19 23:31:54.000000 postpruner-1.1.2/postpruner/dataset/evaluate/nlp.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2094 2023-04-19 23:29:53.000000 postpruner-1.1.2/postpruner/dataset/evaluate/squad.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3804 2023-04-19 22:11:32.000000 postpruner-1.1.2/postpruner/dataset/glue.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    22749 2023-04-19 22:11:32.000000 postpruner-1.1.2/postpruner/dataset/squad.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:44:23.760683 postpruner-1.1.2/postpruner/efficiency/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.1.2/postpruner/efficiency/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1565 2023-04-19 22:11:32.000000 postpruner-1.1.2/postpruner/efficiency/latency.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1633 2023-04-19 22:11:32.000000 postpruner-1.1.2/postpruner/efficiency/mac.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5007 2023-04-19 23:29:53.000000 postpruner-1.1.2/postpruner/generate_lut.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6889 2023-04-19 23:44:10.000000 postpruner-1.1.2/postpruner/postpruner.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:44:23.760683 postpruner-1.1.2/postpruner/prune/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.1.2/postpruner/prune/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1095 2023-04-19 23:29:53.000000 postpruner-1.1.2/postpruner/prune/fisher.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1303 2023-04-19 22:11:32.000000 postpruner-1.1.2/postpruner/prune/rearrange.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7610 2023-04-19 23:29:53.000000 postpruner-1.1.2/postpruner/prune/rescale.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7421 2023-04-19 23:29:53.000000 postpruner-1.1.2/postpruner/prune/search.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:44:23.760683 postpruner-1.1.2/postpruner/utils/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.1.2/postpruner/utils/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3307 2023-04-19 22:11:32.000000 postpruner-1.1.2/postpruner/utils/arch.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      689 2023-04-19 22:11:32.000000 postpruner-1.1.2/postpruner/utils/linalg.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      439 2023-04-19 22:11:32.000000 postpruner-1.1.2/postpruner/utils/meter.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      180 2023-04-19 22:11:32.000000 postpruner-1.1.2/postpruner/utils/schedule.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      807 2023-04-19 22:11:32.000000 postpruner-1.1.2/postpruner/utils/timer.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:44:23.756683 postpruner-1.1.2/postpruner.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       54 2023-04-19 23:44:23.000000 postpruner-1.1.2/postpruner.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      955 2023-04-19 23:44:23.000000 postpruner-1.1.2/postpruner.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-04-19 23:44:23.000000 postpruner-1.1.2/postpruner.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       56 2023-04-19 23:44:23.000000 postpruner-1.1.2/postpruner.egg-info/entry_points.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       58 2023-04-19 23:44:23.000000 postpruner-1.1.2/postpruner.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       11 2023-04-19 23:44:23.000000 postpruner-1.1.2/postpruner.egg-info/top_level.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-04-19 23:44:23.764683 postpruner-1.1.2/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      409 2023-04-19 23:44:22.000000 postpruner-1.1.2/setup.py
```

### Comparing `postpruner-1.1.1/README.md` & `postpruner-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.1/postpruner/__main__.py` & `postpruner-1.1.2/postpruner/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -29,29 +29,27 @@
     parser.add_argument("--constraint", type=float, required=True,
         help="MAC/latency constraint relative to the original model",
     )
     parser.add_argument("--mha_lut", type=str, default=None)
     parser.add_argument("--ffn_lut", type=str, default=None)
     parser.add_argument("--num_samples", type=int, default=2048)
     parser.add_argument("--seed", type=int, default=0)
-    parser.add_argument("--head_mask_output", type=str, default="head_mask.pt")
-    parser.add_argument("--neuron_mask_output", type=str, default="neuron_mask.pt")
+    # parser.add_argument("--head_mask_output", type=str, default="head_mask.pt")
+    # parser.add_argument("--neuron_mask_output", type=str, default="neuron_mask.pt")
     args = parser.parse_args()
 
     run(
         model_name=args.model_name,
         task_name=args.task_name,
         ckpt_dir=args.ckpt_dir,
         constraint=args.constraint,
         output_dir=args.output_dir,
         gpu=args.gpu,
         metric=args.metric,
         mha_lut=args.mha_lut,
         ffn_lut=args.ffn_lut,
         num_samples=args.num_samples,
         seed=args.seed,
-        head_mask_output=args.head_mask_output,
-        neuron_mask_output=args.neuron_mask_output
     )
 
 if __name__ == "__main__":
     main()
```

### Comparing `postpruner-1.1.1/postpruner/dataset/evaluate/glue.py` & `postpruner-1.1.2/postpruner/dataset/evaluate/glue.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.1/postpruner/dataset/evaluate/nlp.py` & `postpruner-1.1.2/postpruner/dataset/evaluate/nlp.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.1/postpruner/dataset/evaluate/squad.py` & `postpruner-1.1.2/postpruner/dataset/evaluate/squad.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.1/postpruner/dataset/glue.py` & `postpruner-1.1.2/postpruner/dataset/glue.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.1/postpruner/dataset/squad.py` & `postpruner-1.1.2/postpruner/dataset/squad.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.1/postpruner/efficiency/latency.py` & `postpruner-1.1.2/postpruner/efficiency/latency.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.1/postpruner/efficiency/mac.py` & `postpruner-1.1.2/postpruner/efficiency/mac.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.1/postpruner/generate_lut.py` & `postpruner-1.1.2/postpruner/generate_lut.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.1/postpruner/postpruner.py` & `postpruner-1.1.2/postpruner/postpruner.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from postpruner.prune.rearrange import rearrange_mask
 from postpruner.prune.rescale import rescale_mask
 from postpruner.dataset.evaluate.nlp import test_accuracy
 from postpruner.utils.schedule import get_pruning_schedule
 
 logger = logging.getLogger(__name__)
 
-def run(model_name, task_name, ckpt_dir, constraint, output_dir=None, gpu=0, metric='mac', mha_lut=None, ffn_lut=None, num_samples=2048, seed=0, head_mask_output, neuron_mask_output):
+def run(model_name, task_name, ckpt_dir, constraint, output_dir=None, gpu=0, metric='mac', mha_lut=None, ffn_lut=None, num_samples=2048, seed=0):
     IS_SQUAD = "squad" in task_name
     IS_LARGE = "large" in model_name
     seq_len = 170 if IS_SQUAD else avg_seq_length(task_name)
 
     # Create the output directory
     if output_dir is None:
         output_dir = os.path.join(
@@ -109,16 +109,16 @@
     model.eval()
     for param in model.parameters():
         param.requires_grad_(False)
 
     full_head_mask = torch.ones(config.num_hidden_layers, config.num_attention_heads).cuda()
     full_neuron_mask = torch.ones(config.num_hidden_layers, config.intermediate_size).cuda()
     
-    head_mask_path = os.path.join(output_dir, head_mask_output)
-    neuron_mask_path = os.path.join(output_dir, neuron_mask_output)
+    head_mask_path = os.path.join(output_dir, "head_mask.pt")
+    neuron_mask_path = os.path.join(output_dir, "neuron_mask.pt")
 
     if not os.path.exists(head_mask_path) or not os.path.exists(neuron_mask_path):
         print("No head_mask or neuron_mask exists, pruning")
         start = time.time()
         # Search the optimal mask
         head_grads, neuron_grads = collect_mask_grads(
             model,
```

### Comparing `postpruner-1.1.1/postpruner/prune/fisher.py` & `postpruner-1.1.2/postpruner/prune/fisher.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.1/postpruner/prune/rearrange.py` & `postpruner-1.1.2/postpruner/prune/rearrange.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.1/postpruner/prune/rescale.py` & `postpruner-1.1.2/postpruner/prune/rescale.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.1/postpruner/prune/search.py` & `postpruner-1.1.2/postpruner/prune/search.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.1/postpruner/utils/arch.py` & `postpruner-1.1.2/postpruner/utils/arch.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.1/postpruner/utils/linalg.py` & `postpruner-1.1.2/postpruner/utils/linalg.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.1/postpruner/utils/timer.py` & `postpruner-1.1.2/postpruner/utils/timer.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.1/postpruner.egg-info/SOURCES.txt` & `postpruner-1.1.2/postpruner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

