# Comparing `tmp/block-recurrent-transformer-pytorch-0.4.0.tar.gz` & `tmp/block-recurrent-transformer-pytorch-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "block-recurrent-transformer-pytorch-0.4.0.tar", last modified: Thu Apr 20 20:38:08 2023, max compression
+gzip compressed data, was "block-recurrent-transformer-pytorch-0.4.1.tar", last modified: Thu Apr 20 21:12:01 2023, max compression
```

## Comparing `block-recurrent-transformer-pytorch-0.4.0.tar` & `block-recurrent-transformer-pytorch-0.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:38:08.295941 block-recurrent-transformer-pytorch-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-20 20:37:56.000000 block-recurrent-transformer-pytorch-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-20 20:38:08.295941 block-recurrent-transformer-pytorch-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-04-20 20:37:56.000000 block-recurrent-transformer-pytorch-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:38:08.291942 block-recurrent-transformer-pytorch-0.4.0/block_recurrent_transformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-20 20:37:56.000000 block-recurrent-transformer-pytorch-0.4.0/block_recurrent_transformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37124 2023-04-20 20:37:56.000000 block-recurrent-transformer-pytorch-0.4.0/block_recurrent_transformer_pytorch/block_recurrent_transformer_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:38:08.291942 block-recurrent-transformer-pytorch-0.4.0/block_recurrent_transformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-20 20:38:08.000000 block-recurrent-transformer-pytorch-0.4.0/block_recurrent_transformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-20 20:38:08.000000 block-recurrent-transformer-pytorch-0.4.0/block_recurrent_transformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 20:38:08.000000 block-recurrent-transformer-pytorch-0.4.0/block_recurrent_transformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-20 20:38:08.000000 block-recurrent-transformer-pytorch-0.4.0/block_recurrent_transformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-20 20:38:08.000000 block-recurrent-transformer-pytorch-0.4.0/block_recurrent_transformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 20:38:08.295941 block-recurrent-transformer-pytorch-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-20 20:37:56.000000 block-recurrent-transformer-pytorch-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:12:01.645211 block-recurrent-transformer-pytorch-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-20 21:11:47.000000 block-recurrent-transformer-pytorch-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-20 21:12:01.645211 block-recurrent-transformer-pytorch-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-04-20 21:11:47.000000 block-recurrent-transformer-pytorch-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:12:01.645211 block-recurrent-transformer-pytorch-0.4.1/block_recurrent_transformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-20 21:11:47.000000 block-recurrent-transformer-pytorch-0.4.1/block_recurrent_transformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37124 2023-04-20 21:11:47.000000 block-recurrent-transformer-pytorch-0.4.1/block_recurrent_transformer_pytorch/block_recurrent_transformer_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:12:01.645211 block-recurrent-transformer-pytorch-0.4.1/block_recurrent_transformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-20 21:12:01.000000 block-recurrent-transformer-pytorch-0.4.1/block_recurrent_transformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-20 21:12:01.000000 block-recurrent-transformer-pytorch-0.4.1/block_recurrent_transformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 21:12:01.000000 block-recurrent-transformer-pytorch-0.4.1/block_recurrent_transformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 21:12:01.000000 block-recurrent-transformer-pytorch-0.4.1/block_recurrent_transformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-20 21:12:01.000000 block-recurrent-transformer-pytorch-0.4.1/block_recurrent_transformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 21:12:01.645211 block-recurrent-transformer-pytorch-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-20 21:11:47.000000 block-recurrent-transformer-pytorch-0.4.1/setup.py
```

### Comparing `block-recurrent-transformer-pytorch-0.4.0/LICENSE` & `block-recurrent-transformer-pytorch-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `block-recurrent-transformer-pytorch-0.4.0/PKG-INFO` & `block-recurrent-transformer-pytorch-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: block-recurrent-transformer-pytorch
-Version: 0.4.0
+Version: 0.4.1
 Summary: Block Recurrent Transformer - Pytorch
 Home-page: https://github.com/lucidrains/block-recurrent-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence
 Classifier: Development Status :: 4 - Beta
```

### Comparing `block-recurrent-transformer-pytorch-0.4.0/README.md` & `block-recurrent-transformer-pytorch-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `block-recurrent-transformer-pytorch-0.4.0/block_recurrent_transformer_pytorch/block_recurrent_transformer_pytorch.py` & `block-recurrent-transformer-pytorch-0.4.1/block_recurrent_transformer_pytorch/block_recurrent_transformer_pytorch.py`

 * *Files identical despite different names*

### Comparing `block-recurrent-transformer-pytorch-0.4.0/block_recurrent_transformer_pytorch.egg-info/PKG-INFO` & `block-recurrent-transformer-pytorch-0.4.1/block_recurrent_transformer_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: block-recurrent-transformer-pytorch
-Version: 0.4.0
+Version: 0.4.1
 Summary: Block Recurrent Transformer - Pytorch
 Home-page: https://github.com/lucidrains/block-recurrent-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence
 Classifier: Development Status :: 4 - Beta
```

### Comparing `block-recurrent-transformer-pytorch-0.4.0/setup.py` & `block-recurrent-transformer-pytorch-0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'block-recurrent-transformer-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.4.0',
+  version = '0.4.1',
   license='MIT',
   description = 'Block Recurrent Transformer - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/block-recurrent-transformer-pytorch',
   keywords = [
@@ -15,15 +15,15 @@
     'deep learning',
     'transformers',
     'attention mechanism',
     'recurrence'
   ],
   install_requires=[
     'beartype',
-    'einops>=0.4',
+    'einops>=0.6.1',
     'memorizing-transformers-pytorch>=0.4.0',
     'torch>=1.6',
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
```

