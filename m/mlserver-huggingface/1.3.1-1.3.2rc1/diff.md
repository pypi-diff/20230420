# Comparing `tmp/mlserver-huggingface-1.3.1.tar.gz` & `tmp/mlserver-huggingface-1.3.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlserver-huggingface-1.3.1.tar", last modified: Fri Apr 14 18:06:24 2023, max compression
+gzip compressed data, was "mlserver-huggingface-1.3.2rc1.tar", last modified: Thu Apr 20 16:09:17 2023, max compression
```

## Comparing `mlserver-huggingface-1.3.1.tar` & `mlserver-huggingface-1.3.2rc1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:24.946085 mlserver-huggingface-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-04-14 18:05:53.000000 mlserver-huggingface-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-14 18:06:24.946085 mlserver-huggingface-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-14 18:05:53.000000 mlserver-huggingface-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:24.942084 mlserver-huggingface-1.3.1/mlserver_huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-14 18:05:53.000000 mlserver-huggingface-1.3.1/mlserver_huggingface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:24.946085 mlserver-huggingface-1.3.1/mlserver_huggingface/codecs/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-14 18:05:53.000000 mlserver-huggingface-1.3.1/mlserver_huggingface/codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-14 18:05:53.000000 mlserver-huggingface-1.3.1/mlserver_huggingface/codecs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-14 18:05:53.000000 mlserver-huggingface-1.3.1/mlserver_huggingface/codecs/conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-14 18:05:53.000000 mlserver-huggingface-1.3.1/mlserver_huggingface/codecs/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-14 18:05:53.000000 mlserver-huggingface-1.3.1/mlserver_huggingface/codecs/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-14 18:05:53.000000 mlserver-huggingface-1.3.1/mlserver_huggingface/codecs/jsonlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-14 18:05:53.000000 mlserver-huggingface-1.3.1/mlserver_huggingface/codecs/numpylist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-14 18:05:53.000000 mlserver-huggingface-1.3.1/mlserver_huggingface/codecs/raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-04-14 18:05:53.000000 mlserver-huggingface-1.3.1/mlserver_huggingface/codecs/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-14 18:05:53.000000 mlserver-huggingface-1.3.1/mlserver_huggingface/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-14 18:05:53.000000 mlserver-huggingface-1.3.1/mlserver_huggingface/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-04-14 18:05:53.000000 mlserver-huggingface-1.3.1/mlserver_huggingface/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-14 18:05:53.000000 mlserver-huggingface-1.3.1/mlserver_huggingface/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-04-14 18:05:53.000000 mlserver-huggingface-1.3.1/mlserver_huggingface/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 18:05:53.000000 mlserver-huggingface-1.3.1/mlserver_huggingface/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:24.946085 mlserver-huggingface-1.3.1/mlserver_huggingface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-14 18:06:24.000000 mlserver-huggingface-1.3.1/mlserver_huggingface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-14 18:06:24.000000 mlserver-huggingface-1.3.1/mlserver_huggingface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:06:24.000000 mlserver-huggingface-1.3.1/mlserver_huggingface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-14 18:06:24.000000 mlserver-huggingface-1.3.1/mlserver_huggingface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 18:06:24.000000 mlserver-huggingface-1.3.1/mlserver_huggingface.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 18:06:24.946085 mlserver-huggingface-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-14 18:05:53.000000 mlserver-huggingface-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:09:17.847061 mlserver-huggingface-1.3.2rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-04-20 16:08:27.000000 mlserver-huggingface-1.3.2rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-20 16:09:17.847061 mlserver-huggingface-1.3.2rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-20 16:08:27.000000 mlserver-huggingface-1.3.2rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:09:17.847061 mlserver-huggingface-1.3.2rc1/mlserver_huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-20 16:08:27.000000 mlserver-huggingface-1.3.2rc1/mlserver_huggingface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:09:17.847061 mlserver-huggingface-1.3.2rc1/mlserver_huggingface/codecs/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-20 16:08:27.000000 mlserver-huggingface-1.3.2rc1/mlserver_huggingface/codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-20 16:08:27.000000 mlserver-huggingface-1.3.2rc1/mlserver_huggingface/codecs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-20 16:08:27.000000 mlserver-huggingface-1.3.2rc1/mlserver_huggingface/codecs/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-20 16:08:27.000000 mlserver-huggingface-1.3.2rc1/mlserver_huggingface/codecs/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-20 16:08:27.000000 mlserver-huggingface-1.3.2rc1/mlserver_huggingface/codecs/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-20 16:08:27.000000 mlserver-huggingface-1.3.2rc1/mlserver_huggingface/codecs/jsonlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-20 16:08:27.000000 mlserver-huggingface-1.3.2rc1/mlserver_huggingface/codecs/numpylist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-20 16:08:27.000000 mlserver-huggingface-1.3.2rc1/mlserver_huggingface/codecs/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-04-20 16:08:27.000000 mlserver-huggingface-1.3.2rc1/mlserver_huggingface/codecs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-20 16:08:27.000000 mlserver-huggingface-1.3.2rc1/mlserver_huggingface/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-20 16:08:27.000000 mlserver-huggingface-1.3.2rc1/mlserver_huggingface/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-04-20 16:08:27.000000 mlserver-huggingface-1.3.2rc1/mlserver_huggingface/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-20 16:08:27.000000 mlserver-huggingface-1.3.2rc1/mlserver_huggingface/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-04-20 16:08:27.000000 mlserver-huggingface-1.3.2rc1/mlserver_huggingface/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-20 16:08:27.000000 mlserver-huggingface-1.3.2rc1/mlserver_huggingface/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:09:17.847061 mlserver-huggingface-1.3.2rc1/mlserver_huggingface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-20 16:09:17.000000 mlserver-huggingface-1.3.2rc1/mlserver_huggingface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-20 16:09:17.000000 mlserver-huggingface-1.3.2rc1/mlserver_huggingface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 16:09:17.000000 mlserver-huggingface-1.3.2rc1/mlserver_huggingface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-20 16:09:17.000000 mlserver-huggingface-1.3.2rc1/mlserver_huggingface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-20 16:09:17.000000 mlserver-huggingface-1.3.2rc1/mlserver_huggingface.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 16:09:17.847061 mlserver-huggingface-1.3.2rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-20 16:08:27.000000 mlserver-huggingface-1.3.2rc1/setup.py
```

### Comparing `mlserver-huggingface-1.3.1/LICENSE` & `mlserver-huggingface-1.3.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.3.1/PKG-INFO` & `mlserver-huggingface-1.3.2rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlserver-huggingface
-Version: 1.3.1
+Version: 1.3.2rc1
 Summary: HuggingFace runtime for MLServer
 Home-page: https://github.com/SeldonIO/MLServer.git
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: # HuggingFace runtime for MLServer
```

### Comparing `mlserver-huggingface-1.3.1/README.md` & `mlserver-huggingface-1.3.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.3.1/mlserver_huggingface/codecs/__init__.py` & `mlserver-huggingface-1.3.2rc1/mlserver_huggingface/codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.3.1/mlserver_huggingface/codecs/base.py` & `mlserver-huggingface-1.3.2rc1/mlserver_huggingface/codecs/base.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.3.1/mlserver_huggingface/codecs/conversation.py` & `mlserver-huggingface-1.3.2rc1/mlserver_huggingface/codecs/conversation.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.3.1/mlserver_huggingface/codecs/image.py` & `mlserver-huggingface-1.3.2rc1/mlserver_huggingface/codecs/image.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.3.1/mlserver_huggingface/codecs/json.py` & `mlserver-huggingface-1.3.2rc1/mlserver_huggingface/codecs/json.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.3.1/mlserver_huggingface/codecs/jsonlist.py` & `mlserver-huggingface-1.3.2rc1/mlserver_huggingface/codecs/jsonlist.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.3.1/mlserver_huggingface/codecs/numpylist.py` & `mlserver-huggingface-1.3.2rc1/mlserver_huggingface/codecs/numpylist.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.3.1/mlserver_huggingface/codecs/raw.py` & `mlserver-huggingface-1.3.2rc1/mlserver_huggingface/codecs/raw.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.3.1/mlserver_huggingface/codecs/utils.py` & `mlserver-huggingface-1.3.2rc1/mlserver_huggingface/codecs/utils.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.3.1/mlserver_huggingface/common.py` & `mlserver-huggingface-1.3.2rc1/mlserver_huggingface/common.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import json
 import numpy as np
 
 from typing import Callable
 from functools import partial
 from mlserver.settings import ModelSettings
 
+import torch
+import tensorflow as tf
+
 from optimum.pipelines import pipeline as opt_pipeline
 from transformers.pipelines import pipeline as trf_pipeline
 from transformers.pipelines.base import Pipeline
 
 from .settings import HuggingFaceSettings
 
 
@@ -27,14 +30,28 @@
     batch_size = 1
     if settings.max_batch_size:
         batch_size = settings.max_batch_size
 
     tokenizer = hf_settings.pretrained_tokenizer
     if not tokenizer:
         tokenizer = hf_settings.pretrained_model
+    if hf_settings.framework == "tf":
+        if hf_settings.inter_op_threads is not None:
+            tf.config.threading.set_inter_op_parallelism_threads(
+                hf_settings.inter_op_threads
+            )
+        if hf_settings.intra_op_threads is not None:
+            tf.config.threading.set_intra_op_parallelism_threads(
+                hf_settings.intra_op_threads
+            )
+    elif hf_settings.framework == "pt":
+        if hf_settings.inter_op_threads is not None:
+            torch.set_num_interop_threads(hf_settings.inter_op_threads)
+        if hf_settings.intra_op_threads is not None:
+            torch.set_num_threads(hf_settings.intra_op_threads)
 
     hf_pipeline = pipeline(
         hf_settings.task_name,
         model=hf_settings.pretrained_model,
         tokenizer=tokenizer,
         device=hf_settings.device,
         batch_size=batch_size,
```

### Comparing `mlserver-huggingface-1.3.1/mlserver_huggingface/errors.py` & `mlserver-huggingface-1.3.2rc1/mlserver_huggingface/errors.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.3.1/mlserver_huggingface/metadata.py` & `mlserver-huggingface-1.3.2rc1/mlserver_huggingface/metadata.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.3.1/mlserver_huggingface/runtime.py` & `mlserver-huggingface-1.3.2rc1/mlserver_huggingface/runtime.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.3.1/mlserver_huggingface/settings.py` & `mlserver-huggingface-1.3.2rc1/mlserver_huggingface/settings.py`

 * *Files 23% similar despite different names*

```diff
@@ -81,14 +81,32 @@
 
     device: int = -1
     """
     Device in which this pipeline will be loaded (e.g., "cpu", "cuda:1", "mps",
     or a GPU ordinal rank like 1).
     """
 
+    inter_op_threads: Optional[int] = None
+    """
+    Threads used for parallelism between independent operations.
+    PyTorch:
+    https://pytorch.org/docs/stable/notes/cpu_threading_torchscript_inference.html
+    Tensorflow:
+    https://www.tensorflow.org/api_docs/python/tf/config/threading/set_inter_op_parallelism_threads
+    """
+
+    intra_op_threads: Optional[int] = None
+    """
+    Threads used within an individual op for parallelism.
+    PyTorch:
+    https://pytorch.org/docs/stable/notes/cpu_threading_torchscript_inference.html
+    Tensorflow:
+    https://www.tensorflow.org/api_docs/python/tf/config/threading/set_intra_op_parallelism_threads
+    """
+
     @property
     def task_name(self):
         if self.task == "translation":
             return f"{self.task}{self.task_suffix}"
         return self.task
```

### Comparing `mlserver-huggingface-1.3.1/mlserver_huggingface.egg-info/PKG-INFO` & `mlserver-huggingface-1.3.2rc1/mlserver_huggingface.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlserver-huggingface
-Version: 1.3.1
+Version: 1.3.2rc1
 Summary: HuggingFace runtime for MLServer
 Home-page: https://github.com/SeldonIO/MLServer.git
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: # HuggingFace runtime for MLServer
```

### Comparing `mlserver-huggingface-1.3.1/mlserver_huggingface.egg-info/SOURCES.txt` & `mlserver-huggingface-1.3.2rc1/mlserver_huggingface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.3.1/setup.py` & `mlserver-huggingface-1.3.2rc1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,13 +32,14 @@
     author="Seldon Technologies Ltd.",
     author_email="hello@seldon.io",
     description="HuggingFace runtime for MLServer",
     packages=find_packages(exclude=["tests", "tests.*"]),
     install_requires=[
         "mlserver",
         "optimum[onnxruntime]>=1.4.0, <1.8.0",
+        "tensorflow",
         "Pillow",
     ],
     long_description=_load_description(),
     long_description_content_type="text/markdown",
     license="Apache 2.0",
 )
```

