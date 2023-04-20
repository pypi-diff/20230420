# Comparing `tmp/postpruner-1.1.4.tar.gz` & `tmp/postpruner-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postpruner-1.1.4.tar", last modified: Thu Apr 20 07:14:45 2023, max compression
+gzip compressed data, was "postpruner-1.2.tar", last modified: Thu Apr 20 09:33:50 2023, max compression
```

## Comparing `postpruner-1.1.4.tar` & `postpruner-1.2.tar`

### file list

```diff
@@ -1,43 +1,46 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 07:14:45.914296 postpruner-1.1.4/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       54 2023-04-20 07:14:45.914296 postpruner-1.1.4/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3648 2023-04-19 22:11:32.000000 postpruner-1.1.4/README.md
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 07:14:45.906296 postpruner-1.1.4/postpruner/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       28 2023-04-20 07:08:02.000000 postpruner-1.1.4/postpruner/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1684 2023-04-19 23:43:36.000000 postpruner-1.1.4/postpruner/__main__.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 07:14:45.910296 postpruner-1.1.4/postpruner/dataset/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.1.4/postpruner/dataset/__init__.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 07:14:45.910296 postpruner-1.1.4/postpruner/dataset/evaluate/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.1.4/postpruner/dataset/evaluate/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1023 2023-04-19 23:29:53.000000 postpruner-1.1.4/postpruner/dataset/evaluate/glue.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1232 2023-04-19 23:31:54.000000 postpruner-1.1.4/postpruner/dataset/evaluate/nlp.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2094 2023-04-19 23:29:53.000000 postpruner-1.1.4/postpruner/dataset/evaluate/squad.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3804 2023-04-19 22:11:32.000000 postpruner-1.1.4/postpruner/dataset/glue.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    22749 2023-04-19 22:11:32.000000 postpruner-1.1.4/postpruner/dataset/squad.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 07:14:45.910296 postpruner-1.1.4/postpruner/efficiency/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.1.4/postpruner/efficiency/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1565 2023-04-19 22:11:32.000000 postpruner-1.1.4/postpruner/efficiency/latency.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1633 2023-04-19 22:11:32.000000 postpruner-1.1.4/postpruner/efficiency/mac.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5007 2023-04-19 23:29:53.000000 postpruner-1.1.4/postpruner/generate_lut.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6889 2023-04-20 07:04:03.000000 postpruner-1.1.4/postpruner/postpruner.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 07:14:45.914296 postpruner-1.1.4/postpruner/prune/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.1.4/postpruner/prune/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1095 2023-04-19 23:29:53.000000 postpruner-1.1.4/postpruner/prune/fisher.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1303 2023-04-19 22:11:32.000000 postpruner-1.1.4/postpruner/prune/rearrange.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7610 2023-04-19 23:29:53.000000 postpruner-1.1.4/postpruner/prune/rescale.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7421 2023-04-19 23:29:53.000000 postpruner-1.1.4/postpruner/prune/search.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 07:14:45.914296 postpruner-1.1.4/postpruner/utils/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.1.4/postpruner/utils/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3307 2023-04-19 22:11:32.000000 postpruner-1.1.4/postpruner/utils/arch.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      689 2023-04-19 22:11:32.000000 postpruner-1.1.4/postpruner/utils/linalg.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      439 2023-04-19 22:11:32.000000 postpruner-1.1.4/postpruner/utils/meter.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      180 2023-04-19 22:11:32.000000 postpruner-1.1.4/postpruner/utils/schedule.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      807 2023-04-19 22:11:32.000000 postpruner-1.1.4/postpruner/utils/timer.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 07:14:45.906296 postpruner-1.1.4/postpruner.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       54 2023-04-20 07:14:45.000000 postpruner-1.1.4/postpruner.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      955 2023-04-20 07:14:45.000000 postpruner-1.1.4/postpruner.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-04-20 07:14:45.000000 postpruner-1.1.4/postpruner.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       57 2023-04-20 07:14:45.000000 postpruner-1.1.4/postpruner.egg-info/entry_points.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       58 2023-04-20 07:14:45.000000 postpruner-1.1.4/postpruner.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       11 2023-04-20 07:14:45.000000 postpruner-1.1.4/postpruner.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-04-20 07:14:45.914296 postpruner-1.1.4/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      465 2023-04-20 07:14:44.000000 postpruner-1.1.4/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 09:33:50.408047 postpruner-1.2/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       43 2023-04-20 09:33:20.000000 postpruner-1.2/MANIFEST.in
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       52 2023-04-20 09:33:50.408047 postpruner-1.2/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3678 2023-04-20 09:33:41.000000 postpruner-1.2/README.md
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 09:33:50.400047 postpruner-1.2/postpruner/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       28 2023-04-20 07:08:02.000000 postpruner-1.2/postpruner/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1684 2023-04-19 23:43:36.000000 postpruner-1.2/postpruner/__main__.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 09:33:50.404047 postpruner-1.2/postpruner/dataset/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.2/postpruner/dataset/__init__.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 09:33:50.404047 postpruner-1.2/postpruner/dataset/evaluate/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.2/postpruner/dataset/evaluate/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1023 2023-04-19 23:29:53.000000 postpruner-1.2/postpruner/dataset/evaluate/glue.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1232 2023-04-19 23:31:54.000000 postpruner-1.2/postpruner/dataset/evaluate/nlp.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2094 2023-04-19 23:29:53.000000 postpruner-1.2/postpruner/dataset/evaluate/squad.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3804 2023-04-19 22:11:32.000000 postpruner-1.2/postpruner/dataset/glue.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    22749 2023-04-19 22:11:32.000000 postpruner-1.2/postpruner/dataset/squad.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 09:33:50.408047 postpruner-1.2/postpruner/efficiency/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.2/postpruner/efficiency/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1565 2023-04-19 22:11:32.000000 postpruner-1.2/postpruner/efficiency/latency.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1633 2023-04-19 22:11:32.000000 postpruner-1.2/postpruner/efficiency/mac.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 09:33:50.408047 postpruner-1.2/postpruner/figures/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)   105406 2023-04-19 22:11:32.000000 postpruner-1.2/postpruner/figures/overview.png
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5007 2023-04-19 23:29:53.000000 postpruner-1.2/postpruner/generate_lut.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6889 2023-04-20 07:04:03.000000 postpruner-1.2/postpruner/postpruner.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 09:33:50.408047 postpruner-1.2/postpruner/prune/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.2/postpruner/prune/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1095 2023-04-19 23:29:53.000000 postpruner-1.2/postpruner/prune/fisher.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1303 2023-04-19 22:11:32.000000 postpruner-1.2/postpruner/prune/rearrange.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7610 2023-04-19 23:29:53.000000 postpruner-1.2/postpruner/prune/rescale.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7421 2023-04-19 23:29:53.000000 postpruner-1.2/postpruner/prune/search.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 09:33:50.408047 postpruner-1.2/postpruner/utils/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.2/postpruner/utils/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3307 2023-04-19 22:11:32.000000 postpruner-1.2/postpruner/utils/arch.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      689 2023-04-19 22:11:32.000000 postpruner-1.2/postpruner/utils/linalg.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      439 2023-04-19 22:11:32.000000 postpruner-1.2/postpruner/utils/meter.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      180 2023-04-19 22:11:32.000000 postpruner-1.2/postpruner/utils/schedule.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      807 2023-04-19 22:11:32.000000 postpruner-1.2/postpruner/utils/timer.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 09:33:50.404047 postpruner-1.2/postpruner.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       52 2023-04-20 09:33:50.000000 postpruner-1.2/postpruner.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      999 2023-04-20 09:33:50.000000 postpruner-1.2/postpruner.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-04-20 09:33:50.000000 postpruner-1.2/postpruner.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       56 2023-04-20 09:33:50.000000 postpruner-1.2/postpruner.egg-info/entry_points.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       58 2023-04-20 09:33:50.000000 postpruner-1.2/postpruner.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       11 2023-04-20 09:33:50.000000 postpruner-1.2/postpruner.egg-info/top_level.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-04-20 09:33:50.408047 postpruner-1.2/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      438 2023-04-20 09:33:49.000000 postpruner-1.2/setup.py
```

### Comparing `postpruner-1.1.4/README.md` & `postpruner-1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # A Fast Post-Training Pruning Framework for Transformers
+```
+python setup.py sdist
 
+```
 > Implemented BERT Large on the Kaggle P100 with 15GB, takes 11.1 GB memory.
 
 Inspired by post-training quantization (PTQ) toolkits, we propose a post-training pruning framework tailored for Transformers.
 Different from existing pruning methods, our framework does not require re-training to retain high accuracy after pruning.
 This makes our method fully automated and 10x-1000x faster in terms of pruning time.
 [[paper link](https://arxiv.org/abs/2204.09656)]
```

### Comparing `postpruner-1.1.4/postpruner/__main__.py` & `postpruner-1.2/postpruner/__main__.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.4/postpruner/dataset/evaluate/glue.py` & `postpruner-1.2/postpruner/dataset/evaluate/glue.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.4/postpruner/dataset/evaluate/nlp.py` & `postpruner-1.2/postpruner/dataset/evaluate/nlp.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.4/postpruner/dataset/evaluate/squad.py` & `postpruner-1.2/postpruner/dataset/evaluate/squad.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.4/postpruner/dataset/glue.py` & `postpruner-1.2/postpruner/dataset/glue.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.4/postpruner/dataset/squad.py` & `postpruner-1.2/postpruner/dataset/squad.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.4/postpruner/efficiency/latency.py` & `postpruner-1.2/postpruner/efficiency/latency.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.4/postpruner/efficiency/mac.py` & `postpruner-1.2/postpruner/efficiency/mac.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.4/postpruner/generate_lut.py` & `postpruner-1.2/postpruner/generate_lut.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.4/postpruner/postpruner.py` & `postpruner-1.2/postpruner/postpruner.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.4/postpruner/prune/fisher.py` & `postpruner-1.2/postpruner/prune/fisher.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.4/postpruner/prune/rearrange.py` & `postpruner-1.2/postpruner/prune/rearrange.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.4/postpruner/prune/rescale.py` & `postpruner-1.2/postpruner/prune/rescale.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.4/postpruner/prune/search.py` & `postpruner-1.2/postpruner/prune/search.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.4/postpruner/utils/arch.py` & `postpruner-1.2/postpruner/utils/arch.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.4/postpruner/utils/linalg.py` & `postpruner-1.2/postpruner/utils/linalg.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.4/postpruner/utils/timer.py` & `postpruner-1.2/postpruner/utils/timer.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.4/postpruner.egg-info/SOURCES.txt` & `postpruner-1.2/postpruner.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+MANIFEST.in
 README.md
 setup.py
 postpruner/__init__.py
 postpruner/__main__.py
 postpruner/generate_lut.py
 postpruner/postpruner.py
 postpruner.egg-info/PKG-INFO
@@ -16,14 +17,15 @@
 postpruner/dataset/evaluate/__init__.py
 postpruner/dataset/evaluate/glue.py
 postpruner/dataset/evaluate/nlp.py
 postpruner/dataset/evaluate/squad.py
 postpruner/efficiency/__init__.py
 postpruner/efficiency/latency.py
 postpruner/efficiency/mac.py
+postpruner/figures/overview.png
 postpruner/prune/__init__.py
 postpruner/prune/fisher.py
 postpruner/prune/rearrange.py
 postpruner/prune/rescale.py
 postpruner/prune/search.py
 postpruner/utils/__init__.py
 postpruner/utils/arch.py
```

