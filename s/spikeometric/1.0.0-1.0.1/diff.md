# Comparing `tmp/spikeometric-1.0.0.tar.gz` & `tmp/spikeometric-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spikeometric-1.0.0.tar", max compression
+gzip compressed data, was "spikeometric-1.0.1.tar", max compression
```

## Comparing `spikeometric-1.0.0.tar` & `spikeometric-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35149 2023-02-23 21:23:20.295275 spikeometric-1.0.0/LICENSE
--rw-r--r--   0        0        0     1359 2023-02-23 21:23:20.295275 spikeometric-1.0.0/README.md
--rw-r--r--   0        0        0      917 2023-02-23 21:32:14.998009 spikeometric-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      325 2023-02-23 21:23:20.355275 spikeometric-1.0.0/spikeometric/datasets/__init__.py
--rw-r--r--   0        0        0     4251 2023-02-23 21:23:20.355275 spikeometric-1.0.0/spikeometric/datasets/connectivity_dataset.py
--rw-r--r--   0        0        0     1558 2023-02-23 21:23:20.355275 spikeometric-1.0.0/spikeometric/datasets/connectivity_generator.py
--rw-r--r--   0        0        0     1428 2023-02-23 21:23:20.355275 spikeometric-1.0.0/spikeometric/datasets/mexican_hat_connectivity_generator.py
--rw-r--r--   0        0        0     3426 2023-02-23 21:23:20.355275 spikeometric-1.0.0/spikeometric/datasets/normal_connectivity_generator.py
--rw-r--r--   0        0        0     2069 2023-02-23 21:23:20.355275 spikeometric-1.0.0/spikeometric/datasets/uniform_connectivity_generator.py
--rw-r--r--   0        0        0      534 2023-02-23 21:23:20.355275 spikeometric-1.0.0/spikeometric/models/__init__.py
--rw-r--r--   0        0        0    15433 2023-02-23 21:23:20.355275 spikeometric-1.0.0/spikeometric/models/base_model.py
--rw-r--r--   0        0        0    12428 2023-02-23 21:23:20.355275 spikeometric-1.0.0/spikeometric/models/bernoulli_glm_model.py
--rw-r--r--   0        0        0     6830 2023-02-23 21:23:20.355275 spikeometric-1.0.0/spikeometric/models/poisson_glm_model.py
--rw-r--r--   0        0        0     6928 2023-02-23 21:23:20.355275 spikeometric-1.0.0/spikeometric/models/rectified_lnp_model.py
--rw-r--r--   0        0        0     6522 2023-02-23 21:23:20.355275 spikeometric-1.0.0/spikeometric/models/rectified_sa_model.py
--rw-r--r--   0        0        0     7782 2023-02-23 21:23:20.355275 spikeometric-1.0.0/spikeometric/models/sa_model.py
--rw-r--r--   0        0        0     6353 2023-02-23 21:23:20.355275 spikeometric-1.0.0/spikeometric/models/threshold_sa_model.py
--rw-r--r--   0        0        0      192 2023-02-23 21:23:20.355275 spikeometric-1.0.0/spikeometric/stimulus/__init__.py
--rw-r--r--   0        0        0     3052 2023-02-23 21:23:20.355275 spikeometric-1.0.0/spikeometric/stimulus/poisson_stimulus.py
--rw-r--r--   0        0        0     2205 2023-02-23 21:23:20.355275 spikeometric-1.0.0/spikeometric/stimulus/regular_stimulus.py
--rw-r--r--   0        0        0     2420 2023-02-23 21:23:20.355275 spikeometric-1.0.0/spikeometric/stimulus/sin_stimulus.py
--rw-r--r--   0        0        0     2349 1970-01-01 00:00:00.000000 spikeometric-1.0.0/setup.py
--rw-r--r--   0        0        0     2407 1970-01-01 00:00:00.000000 spikeometric-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-02-23 21:23:20.295275 spikeometric-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1359 2023-02-23 21:23:20.295275 spikeometric-1.0.1/README.md
+-rw-r--r--   0        0        0      917 2023-04-20 10:08:25.569925 spikeometric-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      325 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/datasets/__init__.py
+-rw-r--r--   0        0        0     4251 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/datasets/connectivity_dataset.py
+-rw-r--r--   0        0        0     1558 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/datasets/connectivity_generator.py
+-rw-r--r--   0        0        0     1428 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/datasets/mexican_hat_connectivity_generator.py
+-rw-r--r--   0        0        0     3426 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/datasets/normal_connectivity_generator.py
+-rw-r--r--   0        0        0     2069 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/datasets/uniform_connectivity_generator.py
+-rw-r--r--   0        0        0      534 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/models/__init__.py
+-rw-r--r--   0        0        0    15433 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/models/base_model.py
+-rw-r--r--   0        0        0    12420 2023-04-20 09:56:38.368186 spikeometric-1.0.1/spikeometric/models/bernoulli_glm_model.py
+-rw-r--r--   0        0        0     6830 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/models/poisson_glm_model.py
+-rw-r--r--   0        0        0     6928 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/models/rectified_lnp_model.py
+-rw-r--r--   0        0        0     6522 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/models/rectified_sa_model.py
+-rw-r--r--   0        0        0     7782 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/models/sa_model.py
+-rw-r--r--   0        0        0     6353 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/models/threshold_sa_model.py
+-rw-r--r--   0        0        0      192 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/stimulus/__init__.py
+-rw-r--r--   0        0        0     3052 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/stimulus/poisson_stimulus.py
+-rw-r--r--   0        0        0     2205 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/stimulus/regular_stimulus.py
+-rw-r--r--   0        0        0     2420 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/stimulus/sin_stimulus.py
+-rw-r--r--   0        0        0     2349 1970-01-01 00:00:00.000000 spikeometric-1.0.1/setup.py
+-rw-r--r--   0        0        0     2407 1970-01-01 00:00:00.000000 spikeometric-1.0.1/PKG-INFO
```

### Comparing `spikeometric-1.0.0/LICENSE` & `spikeometric-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spikeometric-1.0.0/README.md` & `spikeometric-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `spikeometric-1.0.0/pyproject.toml` & `spikeometric-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spikeometric"
-version = "1.0.0"
+version = "1.0.1"
 description = "Spikeometric is a Pytorch Geometric based framework for simulating Spiking Neural Networks using Linear Non-linear Cascade models"
 authors = ["Jakob Sønstebø <jakobls16@gmail.com>"]
 readme = "README.md"
 license = "GNU General Public License v3.0"
 documentation = "https://spikeometric.readthedocs.io/en/latest/"
 repository = "https://github.com/bioAI-Oslo/Spikeometric"
 packages = [{include = "spikeometric"}]
```

### Comparing `spikeometric-1.0.0/spikeometric/datasets/connectivity_dataset.py` & `spikeometric-1.0.1/spikeometric/datasets/connectivity_dataset.py`

 * *Files identical despite different names*

### Comparing `spikeometric-1.0.0/spikeometric/datasets/connectivity_generator.py` & `spikeometric-1.0.1/spikeometric/datasets/connectivity_generator.py`

 * *Files identical despite different names*

### Comparing `spikeometric-1.0.0/spikeometric/datasets/mexican_hat_connectivity_generator.py` & `spikeometric-1.0.1/spikeometric/datasets/mexican_hat_connectivity_generator.py`

 * *Files identical despite different names*

### Comparing `spikeometric-1.0.0/spikeometric/datasets/normal_connectivity_generator.py` & `spikeometric-1.0.1/spikeometric/datasets/normal_connectivity_generator.py`

 * *Files identical despite different names*

### Comparing `spikeometric-1.0.0/spikeometric/datasets/uniform_connectivity_generator.py` & `spikeometric-1.0.1/spikeometric/datasets/uniform_connectivity_generator.py`

 * *Files identical despite different names*

### Comparing `spikeometric-1.0.0/spikeometric/models/__init__.py` & `spikeometric-1.0.1/spikeometric/models/__init__.py`

 * *Files identical despite different names*

### Comparing `spikeometric-1.0.0/spikeometric/models/base_model.py` & `spikeometric-1.0.1/spikeometric/models/base_model.py`

 * *Files identical despite different names*

### Comparing `spikeometric-1.0.0/spikeometric/models/bernoulli_glm_model.py` & `spikeometric-1.0.1/spikeometric/models/bernoulli_glm_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,15 @@
         --------
         W : torch.Tensor [n_edges, T]
             The connectivity filter
         edge_index : torch.Tensor [2, n_edges]
             The edge index (with self edges added)
         """
         # Add self edges to the connectivity matrix
-        n_edges = edge_index.shape[1]
+        n_edges = W0.shape[0]
         n_neurons = edge_index.max().item() + 1
         edge_index, _ = add_remaining_self_loops(edge_index, num_nodes=n_neurons)
         W0 = torch.cat([W0, torch.zeros(edge_index.shape[1] - n_edges, device=W0.device)], dim=0)
 
         # Compute the indices of the self edges
         is_self_edge = edge_index[0] == edge_index[1]
```

### Comparing `spikeometric-1.0.0/spikeometric/models/poisson_glm_model.py` & `spikeometric-1.0.1/spikeometric/models/poisson_glm_model.py`

 * *Files identical despite different names*

### Comparing `spikeometric-1.0.0/spikeometric/models/rectified_lnp_model.py` & `spikeometric-1.0.1/spikeometric/models/rectified_lnp_model.py`

 * *Files identical despite different names*

### Comparing `spikeometric-1.0.0/spikeometric/models/rectified_sa_model.py` & `spikeometric-1.0.1/spikeometric/models/rectified_sa_model.py`

 * *Files identical despite different names*

### Comparing `spikeometric-1.0.0/spikeometric/models/sa_model.py` & `spikeometric-1.0.1/spikeometric/models/sa_model.py`

 * *Files identical despite different names*

### Comparing `spikeometric-1.0.0/spikeometric/models/threshold_sa_model.py` & `spikeometric-1.0.1/spikeometric/models/threshold_sa_model.py`

 * *Files identical despite different names*

### Comparing `spikeometric-1.0.0/spikeometric/stimulus/poisson_stimulus.py` & `spikeometric-1.0.1/spikeometric/stimulus/poisson_stimulus.py`

 * *Files identical despite different names*

### Comparing `spikeometric-1.0.0/spikeometric/stimulus/regular_stimulus.py` & `spikeometric-1.0.1/spikeometric/stimulus/regular_stimulus.py`

 * *Files identical despite different names*

### Comparing `spikeometric-1.0.0/spikeometric/stimulus/sin_stimulus.py` & `spikeometric-1.0.1/spikeometric/stimulus/sin_stimulus.py`

 * *Files identical despite different names*

### Comparing `spikeometric-1.0.0/setup.py` & `spikeometric-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'numpy>=1.21.4,<2.0.0',
  'scipy>=1.7.3,<2.0.0',
  'seaborn>=0.11.2,<0.12.0',
  'tqdm>=4.62.3,<5.0.0']
 
 setup_kwargs = {
     'name': 'spikeometric',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': 'Spikeometric is a Pytorch Geometric based framework for simulating Spiking Neural Networks using Linear Non-linear Cascade models',
     'long_description': '# Spikeometric - Linear Non-Linear Cascade Spiking Neural Networks with PyTorch Geometric\n\nThe spikeometric package is a framework for simulating spiking neural networks (SNNs) using generalized linear models (GLMs) and Linear-Nonlinear-Poisson models (LNPs) in Python. It is built on top of the [PyTorch Geometric](https://pytorch-geometric.readthedocs.io/en/latest/) package and makes use of their powerful graph neural network (GNN) modules and efficient graph representation. It is designed to be fast, flexible and easy to use, and is intended for research purposes.\n\n# Install\nBefore installing `spikeometric` you will need to download versions of PyTorch and PyTorch Geometric that work with your hardware. When you have done that (for example in a conda environment), you are ready to download spikeometric with:\n\n    pip install spikeometric\n\n# Documentation\n\nFor more information about the package and a full API reference check out our [documentation](https://spikeometric.readthedocs.io/en/latest/).\n\n# How to contribute\nWe welcome contributions from users and developers. If you find bugs, please report an issue on github.\nIf you would like to contribute to new features you can either find an issue you would like to work on, or fork this project and develop something great. \nSend pull request for review. We will respond as soon as possible.\n',
     'author': 'Jakob Sønstebø',
     'author_email': 'jakobls16@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bioAI-Oslo/Spikeometric',
```

### Comparing `spikeometric-1.0.0/PKG-INFO` & `spikeometric-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spikeometric
-Version: 1.0.0
+Version: 1.0.1
 Summary: Spikeometric is a Pytorch Geometric based framework for simulating Spiking Neural Networks using Linear Non-linear Cascade models
 Home-page: https://github.com/bioAI-Oslo/Spikeometric
 License: GNU General Public License v3.0
 Author: Jakob Sønstebø
 Author-email: jakobls16@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: Other/Proprietary License
```

