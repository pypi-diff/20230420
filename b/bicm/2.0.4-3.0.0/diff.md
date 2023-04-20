# Comparing `tmp/bicm-2.0.4.tar.gz` & `tmp/bicm-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bicm-2.0.4.tar", last modified: Mon Jun 21 08:33:07 2021, max compression
+gzip compressed data, was "bicm-3.0.0.tar", last modified: Thu Apr 20 14:02:46 2023, max compression
```

## Comparing `bicm-2.0.4.tar` & `bicm-3.0.0.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxrwxrwx   0        0        0        0 2021-06-21 08:33:07.577939 bicm-2.0.4/
--rw-rw-rw-   0        0        0     4752 2021-06-21 08:33:07.576925 bicm-2.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3175 2021-02-08 10:12:31.000000 bicm-2.0.4/README.txt
-drwxrwxrwx   0        0        0        0 2021-06-21 08:33:07.510105 bicm-2.0.4/bicm/
--rw-rw-rw-   0        0        0      471 2021-06-21 08:29:07.000000 bicm-2.0.4/bicm/__init__.py
--rw-rw-rw-   0        0        0    54861 2021-04-14 20:24:41.000000 bicm-2.0.4/bicm/graph_classes.py
--rw-rw-rw-   0        0        0    16084 2021-02-15 14:02:50.000000 bicm-2.0.4/bicm/models_functions.py
--rw-rw-rw-   0        0        0    10775 2021-06-21 08:29:07.000000 bicm-2.0.4/bicm/network_functions.py
--rw-rw-rw-   0        0        0     6409 2020-09-24 10:44:02.000000 bicm-2.0.4/bicm/poibin.py
--rw-rw-rw-   0        0        0     9434 2021-02-15 11:48:48.000000 bicm-2.0.4/bicm/solver_functions.py
-drwxrwxrwx   0        0        0        0 2021-06-21 08:33:07.558982 bicm-2.0.4/bicm.egg-info/
--rw-rw-rw-   0        0        0     4752 2021-06-21 08:33:07.000000 bicm-2.0.4/bicm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2021-06-21 08:33:07.000000 bicm-2.0.4/bicm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-06-21 08:33:07.000000 bicm-2.0.4/bicm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2021-06-21 08:33:07.000000 bicm-2.0.4/bicm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2021-06-21 08:33:07.000000 bicm-2.0.4/bicm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-06-21 08:33:07.577939 bicm-2.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1003 2021-06-21 08:29:07.000000 bicm-2.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2021-06-21 08:33:07.573933 bicm-2.0.4/tests/
--rw-rw-rw-   0        0        0     9480 2021-04-14 20:32:50.000000 bicm-2.0.4/tests/BiCM_test.py
--rw-rw-rw-   0        0        0        0 2020-07-26 09:43:21.000000 bicm-2.0.4/tests/__init__.py
+drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-04-20 14:02:46.872950 bicm-3.0.0/
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     1068 2023-01-04 08:23:41.000000 bicm-3.0.0/LICENSE.txt
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     4602 2023-04-20 14:02:46.872950 bicm-3.0.0/PKG-INFO
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     3928 2023-04-20 13:13:38.000000 bicm-3.0.0/README.md
+drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-04-20 14:02:46.872950 bicm-3.0.0/bicm/
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)      471 2023-04-06 09:27:43.000000 bicm-3.0.0/bicm/__init__.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)    72178 2023-04-20 12:32:35.000000 bicm-3.0.0/bicm/graph_classes.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)    40970 2023-04-20 08:23:16.000000 bicm-3.0.0/bicm/models_functions.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)    11883 2023-04-20 08:31:25.000000 bicm-3.0.0/bicm/network_functions.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     6409 2023-01-04 08:23:41.000000 bicm-3.0.0/bicm/poibin.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     9439 2023-04-06 09:27:43.000000 bicm-3.0.0/bicm/solver_functions.py
+drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-04-20 14:02:46.872950 bicm-3.0.0/bicm.egg-info/
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     4602 2023-04-20 14:02:46.000000 bicm-3.0.0/bicm.egg-info/PKG-INFO
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)      415 2023-04-20 14:02:46.000000 bicm-3.0.0/bicm.egg-info/SOURCES.txt
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)        1 2023-04-20 14:02:46.000000 bicm-3.0.0/bicm.egg-info/dependency_links.txt
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)       50 2023-04-20 14:02:46.000000 bicm-3.0.0/bicm.egg-info/requires.txt
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)       11 2023-04-20 14:02:46.000000 bicm-3.0.0/bicm.egg-info/top_level.txt
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)       38 2023-04-20 14:02:46.872950 bicm-3.0.0/setup.cfg
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     1042 2023-04-06 09:27:43.000000 bicm-3.0.0/setup.py
+drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-04-20 14:02:46.872950 bicm-3.0.0/tests/
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     9480 2023-01-04 08:23:41.000000 bicm-3.0.0/tests/BiCM_test.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)        0 2023-01-04 08:23:41.000000 bicm-3.0.0/tests/__init__.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     1804 2023-01-08 16:20:56.000000 bicm-3.0.0/tests/biwcm_c.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     2378 2023-01-08 16:20:56.000000 bicm-3.0.0/tests/biwcm_d.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     7224 2023-01-08 16:20:57.000000 bicm-3.0.0/tests/biwcm_main.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)      462 2023-01-04 18:33:41.000000 bicm-3.0.0/tests/delta_converter.py
```

### Comparing `bicm-2.0.4/README.txt` & `bicm-3.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,108 @@
-BiCM package.
+Metadata-Version: 2.1
+Name: bicm
+Version: 3.0.0
+Summary: Package for bipartite configuration model
+Home-page: https://github.com/mat701/BiCM
+Author: Matteo Bruno
+Author-email: matteobruno180@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+﻿## BiCM package
 
 This is a Python package for the computation of the maximum entropy bipartite configuration model (BiCM) and the projection of bipartite networks on one layer. It was developed with Python 3.5.
 
-You can install this package via pip:
+You can install this package via pip: 
 
     pip install bicm
 
-Documentation is available at https://bipartite-configuration-model.readthedocs.io/en/latest/.
+Documentation is available at https://bipartite-configuration-model.readthedocs.io/en/latest/ .
+
+This package is also a module of NEMtropy that you can find at https://github.com/nicoloval/NEMtropy .
+
+For more solvers of maximum entropy configuration models visit https://meh.imtlucca.it/ .
 
-For more solvers of maximum entropy configuration models visit https://meh.imtlucca.it/
 
 ## Basic functionalities
 
 To install:
-
+    
     pip install bicm
 
 To import the module:
-
+    
     import bicm
 
 To generate a Graph object and initialize it (with a biadjacency matrix, edgelist or degree sequences):
-
+    
     from bicm import BipartiteGraph
     myGraph = BipartiteGraph()
     myGraph.set_biadjacency_matrix(my_biadjacency_matrix)
     myGraph.set_adjacency_list(my_adjacency_list)
     myGraph.set_edgelist(my_edgelist)
     myGraph.set_degree_sequences((first_degree_sequence, second_degree_sequence))
 
 Or alternatively, with the respective data structure as input:
-
+    
     from bicm import BipartiteGraph
     myGraph = BipartiteGraph(biadjacency=my_biadjacency_matrix, adjacency_list=my_adjacency_list, edgelist=my_edgelist, degree_sequences=((first_degree_sequence, second_degree_sequence)))
 
 To compute the BiCM probability matrix of the graph or the relative fitnesses coefficients as dictionaries containing the nodes names as keys:
 
     my_probability_matrix = myGraph.get_bicm_matrix()
     my_x, my_y = myGraph.get_bicm_fitnesses()
 
-This will solve the bicm using recommended settings for the solver.
+This will solve the bicm using recommended settings for the solver. 
 To customize the solver you can alternatively use (in advance) the following method:
-
+    
     myGraph.solve_tool(light_mode=False, method='newton', initial_guess=None, tolerance=1e-8, max_steps=None, verbose=False, linsearch=True, regularise=False, print_error=True, exp=False)
 
 To get the rows or columns projection of the graph:
 
     myGraph.get_rows_projection()
     myGraph.get_cols_projection()
 
 Alternatively, to customize the projection:
 
     myGraph.compute_projection(rows=True, alpha=0.05, method='poisson', threads_num=4, progress_bar=True)
+    
+Now version 3.0.0 is online, and you can use the package with weighted networks as well using the BiWCM models!
 
-See a more detailed walkthrough in **tests/bicm_tests** notebook or python script, or check out the API in the documentation.
+See a more detailed walkthrough in **tests/bicm_test** or **tests/biwcm_test** notebooks, or check out the API in the documentation.
 
 ## How to cite
 
 If you use the `bicm` module, please cite its location on Github
 [https://github.com/mat701/BiCM](https://github.com/mat701/BiCM) and the
-original articles \[Saracco2015\] and \[Saracco2017\].
+original articles [Vallarano2021], [Saracco2015] and [Saracco2017].
+
+If you use the weighted models BiWCM_c or BiMCM you might consider citing also the following paper introducing the solvers of this package:
+
+* Bruno, M., Mazzilli, D., Patelli, A., Squartini, T., and Saracco, F. \
+    *Inferring comparative advantage via entropy maximization.* \
+    In preparation
 
 ### References
 
-\[Saracco2015\] [F. Saracco, R. Di Clemente, A. Gabrielli, T. Squartini, Randomizing bipartite networks: the case of the World Trade Web, Scientific Reports 5, 10595 (2015)](http://www.nature.com/articles/srep10595).
+[Vallarano2021] [N. Vallarano, M. Bruno, E. Marchese, G. Trapani, F. Saracco, T. Squartini, G. Cimini, M. Zanon, Fast and scalable likelihood maximization for Exponential Random Graph Models with local constraints, Nature Scientific Reports](https://doi.org/10.1038/s41598-021-93830-4)
+
+[Saracco2015] [F. Saracco, R. Di Clemente, A. Gabrielli, T. Squartini, Randomizing bipartite networks: the case of the World Trade Web, Scientific Reports 5, 10595 (2015)](http://www.nature.com/articles/srep10595).
+
+[Saracco2017] [F. Saracco, M. J. Straka, R. Di Clemente, A. Gabrielli, G. Caldarelli, and T. Squartini, Inferring monopartite projections of bipartite networks: an entropy-based approach, New J. Phys. 19, 053022 (2017)](http://stacks.iop.org/1367-2630/19/i=5/a=053022)
+
+
+_Author_:
+
+[Matteo Bruno](https://csl.sony.it/member/matteo-bruno/) (BiCM) (a.k.a. [mat701](https://github.com/mat701))
 
-\[Saracco2017\] [F. Saracco, M. J. Straka, R. Di Clemente, A. Gabrielli, G. Caldarelli, and T. Squartini, Inferring monopartite projections of bipartite networks: an entropy-based approach, New J. Phys. 19, 053022 (2017)](http://stacks.iop.org/1367-2630/19/i=5/a=053022)
 
-\[Squartini2011\] [T. Squartini, D. Garlaschelli, Analytical maximum-likelihood method to detect patterns in real networks, New Journal of Physics 13, (2011)](http://iopscience.iop.org/article/10.1088/1367-2630/13/8/083001)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bicm-2.0.4/bicm/graph_classes.py` & `bicm-3.0.0/bicm/graph_classes.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 The solver functions are located here for compatibility with the numba package.
 """
 
 import numpy as np
 import scipy.sparse
 import scipy
 from scipy.stats import norm, poisson
-from . import models_functions as mof
-from . import solver_functions as sof
-from . import network_functions as nef
+import bicm.models_functions as mof
+import bicm.solver_functions as sof
+import bicm.network_functions as nef
 from tqdm import tqdm
-from . import poibin as pb
+import bicm.poibin as pb
 from functools import partial
 from platform import system
 
 if system() != 'Windows':
     from multiprocessing import Pool
 
 
+
+
 class BipartiteGraph:
     """Bipartite Graph class for undirected binary bipartite networks.
 
     This class handles the bipartite graph object to compute the
     Bipartite Configuration Model (BiCM), which can be used as a null model
     for the analysis of undirected and binary bipartite networks.
     The class provides methods for calculating the probabilities and matrices
@@ -68,16 +70,14 @@
         self.r_cols_deg = None
         self.rows_dict = None
         self.cols_dict = None
         self.is_initialized = False
         self.is_randomized = False
         self.is_reduced = False
         self.rows_projection = None
-        self._initialize_graph(biadjacency=biadjacency, adjacency_list=adjacency_list, edgelist=edgelist,
-                               degree_sequences=degree_sequences)
         self.avg_mat = None
         self.x = None
         self.y = None
         self.r_x = None
         self.r_y = None
         self.solution_array = None
         self.dict_x = None
@@ -90,14 +90,16 @@
         self.projected_rows_adj_list = None
         self.projected_cols_adj_list = None
         self.v_adj_list = None
         self.projection_method = 'poisson'
         self.threads_num = 1
         self.rows_pvals = None
         self.cols_pvals = None
+        self.rows_pvals_mat = None
+        self.cols_pvals_mat = None
         self.is_rows_projected = False
         self.is_cols_projected = False
         self.initial_guess = None
         self.method = None
         self.rows_multiplicity = None
         self.cols_multiplicity = None
         self.r_invert_rows_deg = None
@@ -113,19 +115,28 @@
         self.fixed_rows = None
         self.full_rows_num = None
         self.nonfixed_cols = None
         self.fixed_cols = None
         self.full_cols_num = None
         self.J_T = None
         self.residuals = None
-        self.full_rows_num = None
-        self.full_rows_num = None
         self.solution_converged = None
         self.loglikelihood = None
         self.progress_bar = None
+        self.weighted = False
+        self.continuous_weights = False
+        self.rows_seq = None
+        self.cols_seq = None
+        self.r_rows_seq = None
+        self.r_cols_seq = None
+        self.pvals_mat = None
+        self.exp = False
+        self.error = None
+        self._initialize_graph(biadjacency=biadjacency, adjacency_list=adjacency_list, edgelist=edgelist,
+                               degree_sequences=degree_sequences)
 
     def _initialize_graph(self, biadjacency=None, adjacency_list=None, edgelist=None, degree_sequences=None):
         """
         Internal method for the initialization of the graph.
         Use the setter methods instead.
 
         :param biadjacency: binary input matrix describing the biadjacency matrix
@@ -151,28 +162,43 @@
             else:
                 if isinstance(biadjacency, list):
                     self.biadjacency = np.array(biadjacency)
                 else:
                     self.biadjacency = biadjacency
                 if self.biadjacency.shape[0] == self.biadjacency.shape[1]:
                     print(
-                        'Your matrix is square. Please remember that it is treated as a biadjacency matrix, not an adjacency matrix.')
-                self.adj_list, self.inv_adj_list, self.rows_deg, self.cols_deg = \
-                    nef.adjacency_list_from_biadjacency(self.biadjacency)
+                        'Your matrix is square. Please remember that it \
+                        is treated as a biadjacency matrix, not an adjacency matrix.')
+                self.continuous_weights = not np.all(np.equal(np.mod(self.biadjacency, 1), 0))
+                if self.continuous_weights or np.max(self.biadjacency) > 1:
+                    self.weighted = True
+                    self.rows_seq = self.biadjacency.sum(1)
+                    self.cols_seq = self.biadjacency.sum(0)
+                    self.rows_deg = (self.biadjacency != 0).sum(1)
+                    self.cols_deg = (self.biadjacency != 0).sum(0)
+                    if self.continuous_weights:
+                        print('Continuous weighted model: BiWCM_c')
+                    else:
+                        print('Discrete weighted model: BiWCM_d')
+                else:
+                    self.adj_list, self.inv_adj_list, self.rows_deg, self.cols_deg = \
+                        nef.adjacency_list_from_biadjacency(self.biadjacency)
+
                 self.n_rows = len(self.rows_deg)
                 self.n_cols = len(self.cols_deg)
                 self._initialize_node_dictionaries()
                 self.is_initialized = True
 
         elif edgelist is not None:
             if not isinstance(edgelist, (list, np.ndarray)):
                 raise TypeError('The edgelist must be passed as a list or numpy array')
             elif len(edgelist[0]) != 2:
                 raise ValueError(
-                    'This is not an edgelist. An edgelist must be a vector of couples of nodes. Try passing a biadjacency matrix')
+                    'This is not an edgelist. An edgelist must be a vector of couples of nodes. Try passing a '
+                    'biadjacency matrix')
             else:
                 self.adj_list, self.inv_adj_list, self.rows_deg, self.cols_deg, self.rows_dict, self.cols_dict = \
                     nef.adjacency_list_from_edgelist_bipartite(edgelist)
                 self.inv_rows_dict = {v: k for k, v in self.rows_dict.items()}
                 self.inv_cols_dict = {v: k for k, v in self.cols_dict.items()}
                 self.is_initialized = True
 
@@ -231,14 +257,17 @@
             cols_deg = self.cols_deg
         else:
             rows_deg -= self.full_cols_num
         self.r_rows_deg, self.r_invert_rows_deg, self.rows_multiplicity \
             = np.unique(rows_deg, return_index=False, return_inverse=True, return_counts=True)
         self.r_cols_deg, self.r_invert_cols_deg, self.cols_multiplicity \
             = np.unique(cols_deg, return_index=False, return_inverse=True, return_counts=True)
+        if self.weighted:
+            self.r_rows_seq = np.copy(self.r_rows_deg)
+            self.r_cols_seq = np.copy(self.r_cols_deg)
         self.r_n_rows = self.r_rows_deg.size
         self.r_n_cols = self.r_cols_deg.size
         self.r_dim = self.r_n_rows + self.r_n_cols
         self.r_n_edges = np.sum(rows_deg)
         self.is_reduced = True
 
     def _set_initial_guess(self):
@@ -256,17 +285,24 @@
             self.r_y = np.ones(self.r_n_cols, dtype=np.float64)
         elif self.initial_guess == 'degrees':
             self.r_x = self.r_rows_deg.astype(np.float64)
             self.r_y = self.r_cols_deg.astype(np.float64)
         else:
             raise ValueError('initial_guess must be None, "chung_lu", "random", "uniform" or "degrees"')
         if not self.exp:
+            if self.weighted:  # Avoid negative thetas
+                normalization = max(np.max(self.r_x), np.max(self.r_y))
+                if normalization >= 1:
+                    self.r_x /= 2 * normalization
+                    self.r_y /= 2 * normalization
             self.r_theta_x = - np.log(self.r_x)
             self.r_theta_y = - np.log(self.r_y)
             self.x0 = np.concatenate((self.r_theta_x, self.r_theta_y))
+            # if self.weighted: # Avoid thetas' products = 1
+            #     self.x0 /= 2 * np.max(np.abs(self.x0))
         else:
             self.x0 = np.concatenate((self.r_x, self.r_y))
 
     def initialize_avg_mat(self):
         """
         Reduces the matrix eliminating empty or full rows or columns.
         It repeats the process on the so reduced matrix until no more reductions are possible.
@@ -277,33 +313,38 @@
         rows_num, cols_num = self.biadjacency.shape
         rows_degs = self.biadjacency.sum(1)
         cols_degs = self.biadjacency.sum(0)
         good_rows = np.arange(rows_num)
         good_cols = np.arange(cols_num)
         zero_rows = np.where(rows_degs == 0)[0]
         zero_cols = np.where(cols_degs == 0)[0]
-        full_rows = np.where(rows_degs == cols_num)[0]
-        full_cols = np.where(cols_degs == rows_num)[0]
+        if not self.weighted:
+            full_rows = np.where(rows_degs == cols_num)[0]
+            full_cols = np.where(cols_degs == rows_num)[0]
+        else:
+            full_rows = np.array([])
+            full_cols = np.array([])
         self.full_rows_num = 0
         self.full_cols_num = 0
         while zero_rows.size + zero_cols.size + full_rows.size + full_cols.size > 0:
             r_biad_mat = r_biad_mat[np.delete(np.arange(r_biad_mat.shape[0]), zero_rows), :]
             r_biad_mat = r_biad_mat[:, np.delete(np.arange(r_biad_mat.shape[1]), zero_cols)]
             good_rows = np.delete(good_rows, zero_rows)
             good_cols = np.delete(good_cols, zero_cols)
-            full_rows = np.where(r_biad_mat.sum(1) == r_biad_mat.shape[1])[0]
-            full_cols = np.where(r_biad_mat.sum(0) == r_biad_mat.shape[0])[0]
-            self.full_rows_num += len(full_rows)
-            self.full_cols_num += len(full_cols)
-            self.avg_mat[good_rows[full_rows][:, None], good_cols] = 1
-            self.avg_mat[good_rows[:, None], good_cols[full_cols]] = 1
-            good_rows = np.delete(good_rows, full_rows)
-            good_cols = np.delete(good_cols, full_cols)
-            r_biad_mat = r_biad_mat[np.delete(np.arange(r_biad_mat.shape[0]), full_rows), :]
-            r_biad_mat = r_biad_mat[:, np.delete(np.arange(r_biad_mat.shape[1]), full_cols)]
+            if not self.weighted:
+                full_rows = np.where(r_biad_mat.sum(1) == r_biad_mat.shape[1])[0]
+                full_cols = np.where(r_biad_mat.sum(0) == r_biad_mat.shape[0])[0]
+                self.full_rows_num += len(full_rows)
+                self.full_cols_num += len(full_cols)
+                self.avg_mat[good_rows[full_rows][:, None], good_cols] = 1
+                self.avg_mat[good_rows[:, None], good_cols[full_cols]] = 1
+                good_rows = np.delete(good_rows, full_rows)
+                good_cols = np.delete(good_cols, full_cols)
+                r_biad_mat = r_biad_mat[np.delete(np.arange(r_biad_mat.shape[0]), full_rows), :]
+                r_biad_mat = r_biad_mat[:, np.delete(np.arange(r_biad_mat.shape[1]), full_cols)]
             zero_rows = np.where(r_biad_mat.sum(1) == 0)[0]
             zero_cols = np.where(r_biad_mat.sum(0) == 0)[0]
 
         self.nonfixed_rows = good_rows
         self.fixed_rows = np.delete(np.arange(rows_num), good_rows)
         self.nonfixed_cols = good_cols
         self.fixed_cols = np.delete(np.arange(cols_num), good_cols)
@@ -324,29 +365,35 @@
         good_cols = np.arange(self.n_cols)
         bad_rows = np.array([])
         bad_cols = np.array([])
         self.full_rows_num = 0
         self.full_cols_num = 0
         if np.any(np.isin(self.rows_deg, (0, self.n_cols))) or np.any(np.isin(self.cols_deg, (0, self.n_rows))):
             print('''
-                      WARNING: this system has at least a node that is disconnected or connected to all nodes of the opposite layer. 
-                      This may cause some convergence issues.
-                      Please use the full mode providing a biadjacency matrix or an edgelist, or clean your data from these nodes. 
+                      WARNING: this system has at least a node that is disconnected or connected to all nodes
+                       of the opposite layer. This may cause some convergence issues.
+                      Please use the full mode providing a biadjacency matrix or an edgelist,
+                       or clean your data from these nodes. 
                       ''')
             zero_rows = np.where(self.rows_deg == 0)[0]
             zero_cols = np.where(self.cols_deg == 0)[0]
-            full_rows = np.where(self.rows_deg == self.n_cols)[0]
-            full_cols = np.where(self.cols_deg == self.n_rows)[0]
-            self.x[full_rows] = np.inf
-            self.y[full_cols] = np.inf
             if not self.exp:
-                self.theta_x[full_rows] = - np.inf
-                self.theta_y[full_rows] = - np.inf
                 self.theta_x[zero_rows] = np.inf
                 self.theta_y[zero_cols] = np.inf
+            if not self.weighted:
+                full_rows = np.where(self.rows_deg == self.n_cols)[0]
+                full_cols = np.where(self.cols_deg == self.n_rows)[0]
+                self.x[full_rows] = np.inf
+                self.y[full_cols] = np.inf
+                if not self.exp:
+                    self.theta_x[full_rows] = - np.inf
+                    self.theta_y[full_rows] = - np.inf
+            else:
+                full_rows = np.array([])
+                full_cols = np.array([])
             bad_rows = np.concatenate((zero_rows, full_rows))
             bad_cols = np.concatenate((zero_cols, full_cols))
             good_rows = np.delete(np.arange(self.n_rows), bad_rows)
             good_cols = np.delete(np.arange(self.n_cols), bad_cols)
             self.full_rows_num += len(full_rows)
             self.full_cols_num += len(full_cols)
 
@@ -358,67 +405,138 @@
     def _initialize_problem(self, rows_deg=None, cols_deg=None):
         """
         Initializes the solver reducing the degree sequences,
         setting the initial guess and setting the functions for the solver.
         The two parameters rows_deg and cols_deg are passed if there were some full or empty rows or columns.
         """
         if ~self.is_reduced:
-            self.degree_reduction(rows_deg=rows_deg, cols_deg=cols_deg)
+            self.degree_reduction(rows_deg=rows_deg, cols_deg=cols_deg)  # if weighted rows_deg=rows_seq
         self._set_initial_guess()
         if self.method == 'root':
             self.J_T = np.zeros((self.r_dim, self.r_dim), dtype=np.float64)
             self.residuals = np.zeros(self.r_dim, dtype=np.float64)
         else:
             self.args = (self.r_rows_deg, self.r_cols_deg, self.rows_multiplicity, self.cols_multiplicity)
-            d_fun = {
-                'newton': lambda x: - mof.loglikelihood_prime_bicm(x, self.args),
-                'quasinewton': lambda x: - mof.loglikelihood_prime_bicm(x, self.args),
-                'fixed-point': lambda x: mof.iterative_bicm(x, self.args),
-                'newton_exp': lambda x: - mof.loglikelihood_prime_bicm_exp(x, self.args),
-                'quasinewton_exp': lambda x: - mof.loglikelihood_prime_bicm_exp(x, self.args),
-                'fixed-point_exp': lambda x: mof.iterative_bicm_exp(x, self.args),
-            }
-            d_fun_jac = {
-                'newton': lambda x: - mof.loglikelihood_hessian_bicm(x, self.args),
-                'quasinewton': lambda x: - mof.loglikelihood_hessian_diag_bicm(x, self.args),
-                'fixed-point': None,
-                'newton_exp': lambda x: - mof.loglikelihood_hessian_bicm_exp(x, self.args),
-                'quasinewton_exp': lambda x: - mof.loglikelihood_hessian_diag_bicm_exp(x, self.args),
-                'fixed-point_exp': None,
-            }
-            d_fun_step = {
-                'newton': lambda x: - mof.loglikelihood_bicm(x, self.args),
-                'quasinewton': lambda x: - mof.loglikelihood_bicm(x, self.args),
-                'fixed-point': lambda x: - mof.loglikelihood_bicm(x, self.args),
-                'newton_exp': lambda x: - mof.loglikelihood_bicm_exp(x, self.args),
-                'quasinewton_exp': lambda x: - mof.loglikelihood_bicm_exp(x, self.args),
-                'fixed-point_exp': lambda x: - mof.loglikelihood_bicm_exp(x, self.args),
-            }
+            if self.continuous_weights:
+                d_fun = {
+                    'newton': lambda x: - mof.loglikelihood_prime_biwcm_c(x, self.args),
+                    'quasinewton': lambda x: - mof.loglikelihood_prime_biwcm_c(x, self.args),
+                    'fixed-point': lambda x: mof.iterative_biwcm_c(x, self.args),
+                    'newton_exp': lambda x: - mof.loglikelihood_prime_biwcm_c_exp(x, self.args),
+                    'quasinewton_exp': lambda x: - mof.loglikelihood_prime_biwcm_c_exp(x, self.args),
+                    'fixed-point_exp': lambda x: mof.iterative_biwcm_c_exp(x, self.args),
+                }
+                d_fun_jac = {
+                    'newton': lambda x: - mof.loglikelihood_hessian_biwcm_c(x, self.args),
+                    'quasinewton': lambda x: - mof.loglikelihood_hessian_diag_biwcm_c(x, self.args),
+                    'fixed-point': None,
+                    'newton_exp': lambda x: - mof.loglikelihood_hessian_biwcm_c_exp(x, self.args),
+                    'quasinewton_exp': lambda x: - mof.loglikelihood_hessian_diag_biwcm_c_exp(x, self.args),
+                    'fixed-point_exp': None,
+                }
+                d_fun_step = {
+                    # 'newton': lambda x: - mof.loglikelihood_biwcm_c(x, self.args),
+                    # 'quasinewton': lambda x: - mof.loglikelihood_biwcm_c(x, self.args),
+                    # 'fixed-point': lambda x: - mof.loglikelihood_biwcm_c(x, self.args),
+                    'newton': lambda x: mof.mrse_biwcm_c(x, self.args),
+                    'quasinewton': lambda x: mof.mrse_biwcm_c(x, self.args),
+                    'fixed-point': lambda x: mof.mrse_biwcm_c(x, self.args),
+                    'newton_exp': lambda x: - mof.loglikelihood_biwcm_c_exp(x, self.args),
+                    'quasinewton_exp': lambda x: - mof.loglikelihood_biwcm_c_exp(x, self.args),
+                    'fixed-point_exp': lambda x: - mof.loglikelihood_biwcm_c_exp(x, self.args),
+                }
+            elif self.weighted:
+                d_fun = {
+                    'newton': lambda x: - mof.loglikelihood_prime_biwcm_d(x, self.args),
+                    'quasinewton': lambda x: - mof.loglikelihood_prime_biwcm_d(x, self.args),
+                    'fixed-point': lambda x: mof.iterative_biwcm_d(x, self.args),
+                    'newton_exp': lambda x: - mof.loglikelihood_prime_biwcm_d_exp(x, self.args),
+                    'quasinewton_exp': lambda x: - mof.loglikelihood_prime_biwcm_d_exp(x, self.args),
+                    'fixed-point_exp': lambda x: mof.iterative_biwcm_d_exp(x, self.args),
+                }
+                d_fun_jac = {
+                    'newton': lambda x: - mof.loglikelihood_hessian_biwcm_d(x, self.args),
+                    'quasinewton': lambda x: - mof.loglikelihood_hessian_diag_biwcm_d(x, self.args),
+                    'fixed-point': None,
+                    'newton_exp': lambda x: - mof.loglikelihood_hessian_biwcm_d_exp(x, self.args),
+                    'quasinewton_exp': lambda x: - mof.loglikelihood_hessian_diag_biwcm_d_exp(x, self.args),
+                    'fixed-point_exp': None,
+                }
+                d_fun_step = {
+                    # 'newton': lambda x: - mof.loglikelihood_biwcm_d(x, self.args),
+                    # 'quasinewton': lambda x: - mof.loglikelihood_biwcm_d(x, self.args),
+                    # 'fixed-point': lambda x: - mof.loglikelihood_biwcm_d(x, self.args),
+                    'newton': lambda x: mof.mrse_biwcm_d(x, self.args),
+                    'quasinewton': lambda x: mof.mrse_biwcm_d(x, self.args),
+                    'fixed-point': lambda x: mof.mrse_biwcm_d(x, self.args),
+                    'newton_exp': lambda x: - mof.loglikelihood_biwcm_d_exp(x, self.args),
+                    'quasinewton_exp': lambda x: - mof.loglikelihood_biwcm_d_exp(x, self.args),
+                    'fixed-point_exp': lambda x: - mof.loglikelihood_biwcm_d_exp(x, self.args),
+                }
+            else:
+                d_fun = {
+                    'newton': lambda x: - mof.loglikelihood_prime_bicm(x, self.args),
+                    'quasinewton': lambda x: - mof.loglikelihood_prime_bicm(x, self.args),
+                    'fixed-point': lambda x: mof.iterative_bicm(x, self.args),
+                    'newton_exp': lambda x: - mof.loglikelihood_prime_bicm_exp(x, self.args),
+                    'quasinewton_exp': lambda x: - mof.loglikelihood_prime_bicm_exp(x, self.args),
+                    'fixed-point_exp': lambda x: mof.iterative_bicm_exp(x, self.args),
+                }
+                d_fun_jac = {
+                    'newton': lambda x: - mof.loglikelihood_hessian_bicm(x, self.args),
+                    'quasinewton': lambda x: - mof.loglikelihood_hessian_diag_bicm(x, self.args),
+                    'fixed-point': None,
+                    'newton_exp': lambda x: - mof.loglikelihood_hessian_bicm_exp(x, self.args),
+                    'quasinewton_exp': lambda x: - mof.loglikelihood_hessian_diag_bicm_exp(x, self.args),
+                    'fixed-point_exp': None,
+                }
+                d_fun_step = {
+                    'newton': lambda x: - mof.loglikelihood_bicm(x, self.args),
+                    'quasinewton': lambda x: - mof.loglikelihood_bicm(x, self.args),
+                    'fixed-point': lambda x: - mof.loglikelihood_bicm(x, self.args),
+                    'newton_exp': lambda x: - mof.loglikelihood_bicm_exp(x, self.args),
+                    'quasinewton_exp': lambda x: - mof.loglikelihood_bicm_exp(x, self.args),
+                    'fixed-point_exp': lambda x: - mof.loglikelihood_bicm_exp(x, self.args),
+                }
 
             if self.exp:
                 self.hessian_regulariser = sof.matrix_regulariser_function_eigen_based
             else:
                 self.hessian_regulariser = sof.matrix_regulariser_function
-
+            
             if self.exp:
-                lins_args = (mof.loglikelihood_bicm_exp, self.args)
+                method = self.method + '_exp'
             else:
-                lins_args = (mof.loglikelihood_bicm, self.args)
+                method = self.method
+            
+            # lins_args = (d_fun_step[method], self.args)
+            if self.continuous_weights:
+                if self.exp:
+                    lins_args = (mof.loglikelihood_biwcm_c_exp, self.args)
+                else:
+                    lins_args = (mof.loglikelihood_biwcm_c, self.args)
+            elif self.weighted:
+                if self.exp:
+                    lins_args = (mof.loglikelihood_biwcm_d_exp, self.args)
+                else:
+                    lins_args = (mof.loglikelihood_biwcm_d, self.args)
+            else:
+                if self.exp:
+                    lins_args = (mof.loglikelihood_bicm_exp, self.args)
+                else:
+                    lins_args = (mof.loglikelihood_bicm, self.args)
             lins_fun = {
                 'newton': lambda x: mof.linsearch_fun_BiCM(x, lins_args),
                 'quasinewton': lambda x: mof.linsearch_fun_BiCM(x, lins_args),
                 'fixed-point': lambda x: mof.linsearch_fun_BiCM_fixed(x),
                 'newton_exp': lambda x: mof.linsearch_fun_BiCM_exp(x, lins_args),
                 'quasinewton_exp': lambda x: mof.linsearch_fun_BiCM_exp(x, lins_args),
                 'fixed-point_exp': lambda x: mof.linsearch_fun_BiCM_exp_fixed(x),
             }
-            if self.exp:
-                method = self.method + '_exp'
-            else:
-                method = self.method
+            
             try:
                 self.fun = d_fun[method]
                 self.fun_jac = d_fun_jac[method]
                 self.step_fun = d_fun_step[method]
                 self.fun_linsearch = lins_fun[method]
             except (TypeError, KeyError):
                 raise ValueError('Method must be "newton","quasinewton", "fixed-point" or "root".')
@@ -461,96 +579,142 @@
         opz = {'col_deriv': True, 'diag': None}
         res = scipy.optimize.root(self._residuals_jacobian, x0,
                                   method='hybr', jac=True, options=opz)
         self._clean_root()
         return res.x
 
     @staticmethod
-    def check_sol(biad_mat, avg_bicm, return_error=False, in_place=False):
+    def check_sol(biad_mat, avg_bicm, return_error=False, in_place=False, mrse=None):
         """
         Static method.
-        This function prints the rows sums differences between two matrices, that originally are the biadjacency matrix and its bicm average matrix.
-        The intended use of this is to check if an average matrix is actually a solution for a bipartite configuration model.
+        This function prints the rows sums differences between two matrices,
+        that originally are the biadjacency matrix and its bicm average matrix.
+        The intended use of this is to check if an average matrix is actually a solution
+         for a bipartite configuration model.
 
         If return_error is set to True, it returns 1 if the sum of the differences is bigger than 1.
 
         If in_place is set to True, it checks and sums also the total error entry by entry.
         The intended use of this is to check if two solutions are the same solution.
         """
         error = 0
+        weighted = np.max(biad_mat) > 1
         if np.any(avg_bicm < 0):
-            print('Negative probabilities in the average matrix! This means negative node fitnesses.')
+            print('Negative probabilities in the average matrix!')
             error = 1
-        if np.any(avg_bicm > 1):
-            print('Probabilities greater than 1 in the average matrix! This means negative node fitnesses.')
-            error = 1
-        rows_error_vec = np.abs(np.sum(biad_mat, axis=1) - np.sum(avg_bicm, axis=1))
+        if not weighted:
+            if np.any(avg_bicm > 1):
+                print('Probabilities greater than 1 in the average matrix!')
+                error = 1
+        if mrse is None:
+            if weighted:
+                mrse = True
+            else:
+                mrse = False
+        rows_sums = np.sum(biad_mat, axis=1)
+        cols_sums = np.sum(biad_mat, axis=0)
+        if mrse:
+            rows_error_vec = np.zeros(len(rows_sums))
+            cols_error_vec = np.zeros(len(cols_sums))
+            nonzero_rows = np.where(rows_sums != 0)[0]
+            nonzero_cols = np.where(cols_sums != 0)[0]
+            rows_error_vec[nonzero_rows] = \
+                np.abs(rows_sums - np.sum(avg_bicm, axis=1))[nonzero_rows] / rows_sums[nonzero_rows]
+            cols_error_vec[nonzero_cols] = \
+                np.abs(cols_sums - np.sum(avg_bicm, axis=0))[nonzero_cols] / cols_sums[nonzero_cols]
+        else:
+            rows_error_vec = np.abs(rows_sums - np.sum(avg_bicm, axis=1))
+            cols_error_vec = np.abs(cols_sums - np.sum(avg_bicm, axis=0))    
         err_rows = np.max(rows_error_vec)
-        print('max rows error =', err_rows)
-        cols_error_vec = np.abs(np.sum(biad_mat, axis=0) - np.sum(avg_bicm, axis=0))
         err_cols = np.max(cols_error_vec)
+        print('max rows error =', err_rows)
         print('max columns error =', err_cols)
         tot_err = np.sum(rows_error_vec) + np.sum(cols_error_vec)
         print('total error =', tot_err)
-        if tot_err > 1:
-            error = 1
-            print('WARNING total error > 1')
-            if tot_err > 10:
-                print('total error > 10')
-        if err_rows + err_cols > 1:
-            print('max error > 1')
-            error = 1
-            if err_rows + err_cols > 10:
-                print('max error > 10')
+        max_err = np.max([err_rows, err_cols])
+        if max_err > 1e-3:
+            # error = 1
+            print('WARNING max error > 0.001')
+            # if tot_err > 10:
+            #     print('total error > 10')
+        # if err_rows + err_cols > 1:
+        #     print('max error > 1')
+        #     error = 1
+        #     if err_rows + err_cols > 10:
+        #         print('max error > 10')
         if in_place:
             diff_mat = np.abs(biad_mat - avg_bicm)
             print('In-place total error:', np.sum(diff_mat))
             print('In-place max error:', np.max(diff_mat))
         if return_error:
-            return error
+            if error == 1:
+                return error
+            else:
+                return max_err
         else:
             return
 
     def check_sol_light(self, return_error=False):
         """
         Light version of the check_sol function, working only on the fitnesses and the degree sequences.
         """
         error = 0
-        rows_error_vec = []
+        exp_rows_sum = np.zeros(self.r_n_rows)
+        exp_cols_sum = np.zeros(self.r_n_cols)
+    
         for i in range(self.r_n_rows):
-            row_avgs = self.r_x[i] * self.r_y / (1 + self.r_x[i] * self.r_y)
-            if error == 0:
-                if np.any(row_avgs < 0):
-                    print('Warning: negative link probabilities')
-                    error = 1
-                if np.any(row_avgs > 1):
-                    print('Warning: link probabilities > 1')
-                    error = 1
-            rows_error_vec.append(np.sum(self.cols_multiplicity * row_avgs) - self.r_rows_deg[i])
-        rows_error_vec = np.abs(rows_error_vec)
+            for j in range(self.r_n_cols):
+                if self.continuous_weights:
+                    multiplier = 1 / (self.r_theta_x[i] + self.r_theta_y[j])
+                elif self.weighted:
+                    xy = self.r_x[i] * self.r_y[j]
+                    multiplier = xy / (1 - xy)
+                else:
+                    xy = self.r_x[i] * self.r_y[j]
+                    multiplier = xy / (1 + xy)
+                exp_rows_sum[i] += self.cols_multiplicity[j] * multiplier
+                exp_cols_sum[j] += self.rows_multiplicity[i] * multiplier
+                if error == 0:
+                    if multiplier < 0:
+                        print('Warning: negative link probabilities')
+                        error = 1
+                    if not self.weighted:
+                        if multiplier > 1:
+                            print('Warning: link probabilities > 1')
+                            error = 1
+        if self.weighted:
+            # use mrse
+            rows_error_vec = np.abs((exp_rows_sum - self.r_rows_seq) / self.r_rows_seq)
+            cols_error_vec = np.abs((exp_cols_sum - self.r_cols_seq) / self.r_cols_seq)
+        else:
+            # use made
+            rows_error_vec = np.abs((exp_rows_sum - self.r_rows_deg))
+            cols_error_vec = np.abs((exp_cols_sum - self.r_cols_deg))
         err_rows = np.max(rows_error_vec)
         print('max rows error =', err_rows)
-        cols_error_vec = np.abs([(self.rows_multiplicity * self.r_x * self.r_y[j] / (1 + self.r_x * self.r_y[j])).sum()
-                                 - self.r_cols_deg[j] for j in range(self.r_n_cols)])
         err_cols = np.max(cols_error_vec)
         print('max columns error =', err_cols)
         tot_err = np.sum(rows_error_vec) + np.sum(cols_error_vec)
         print('total error =', tot_err)
-        if tot_err > 1:
-            error = 1
-            print('WARNING total error > 1')
-            if tot_err > 10:
-                print('total error > 10')
-        if err_rows + err_cols > 1:
-            print('max error > 1')
-            error = 1
-            if err_rows + err_cols > 10:
-                print('max error > 10')
+        max_err = np.max([err_rows, err_cols])
+        if max_err > 1e-3:
+            # error = 1
+            print('WARNING max error > 0.001')
+            # if tot_err > 10:
+            #     print('total error > 10')
+        # if err_rows + err_cols > 1:
+        #     print('max error > 1')
+        #     error = 1
+        #     if err_rows + err_cols > 10:
+        #         print('max error > 10')
         if return_error:
-            return error
+            if error == 1:
+                return error
+            else:
+                return max_err
         else:
             return
 
     def _check_solution(self, return_error=False, in_place=False):
         """
         Check if the solution of the BiCM is compatible with the degree sequences of the graph.
 
@@ -568,16 +732,18 @@
         Sets the solution of the problem.
 
         :param numpy.ndarray solution: A numpy array containing that reduced fitnesses of the two layers, consecutively.
         """
         if not self.exp:
             if self.theta_x is None:
                 self.theta_x = np.zeros(self.n_rows)
+                self.theta_x[:] = np.inf
             if self.theta_y is None:
                 self.theta_y = np.zeros(self.n_cols)
+                self.theta_y[:] = np.inf
             self.r_theta_xy = solution
             self.r_theta_x = self.r_theta_xy[:self.r_n_rows]
             self.r_theta_y = self.r_theta_xy[self.r_n_rows:]
             self.solution_array = np.exp(- self.r_theta_xy)
             self.r_x = np.exp(- self.r_theta_x)
             self.r_y = np.exp(- self.r_theta_y)
             self.theta_x[self.nonfixed_rows] = self.r_theta_x[self.r_invert_rows_deg]
@@ -597,31 +763,47 @@
         if self.full_return:
             self.comput_time = solution[1]
             self.n_steps = solution[2]
             self.norm_seq = solution[3]
             self.diff_seq = solution[4]
             self.alfa_seq = solution[5]
         if self.method != 'root':
-            self.loglikelihood = self.step_fun(self.solution_array)
+            if self.continuous_weights:
+                if self.exp:
+                    self.loglikelihood = mof.loglikelihood_biwcm_c_exp(self.solution_array, self.args)
+                else:
+                    self.loglikelihood = mof.loglikelihood_biwcm_c(self.solution_array, self.args)
+            elif self.weighted:
+                if self.exp:
+                    self.loglikelihood = mof.loglikelihood_biwcm_d_exp(self.solution_array, self.args)
+                else:
+                    self.loglikelihood = mof.loglikelihood_biwcm_d(self.solution_array, self.args)
+            else:
+                self.loglikelihood = self.step_fun(self.solution_array)
         # Reset solver lambda functions for multiprocessing compatibility
         self.hessian_regulariser = None
         self.fun = None
         self.fun_jac = None
         self.step_fun = None
         self.fun_linsearch = None
 
     def _solve_bicm_full(self):
         """
         Internal method for computing the solution of the BiCM via matrices.
         """
         r_biadjacency = self.initialize_avg_mat()
         if len(r_biadjacency) > 0:  # Every time the matrix is not perfectly nested
-            rows_deg = self.rows_deg[self.nonfixed_rows]
-            cols_deg = self.cols_deg[self.nonfixed_cols]
-            self._initialize_problem(rows_deg=rows_deg, cols_deg=cols_deg)
+            if self.weighted:
+                rows_seq = self.rows_seq[self.nonfixed_rows]
+                cols_seq = self.cols_seq[self.nonfixed_cols]
+                self._initialize_problem(rows_deg=rows_seq, cols_deg=cols_seq)
+            else:
+                rows_deg = self.rows_deg[self.nonfixed_rows]
+                cols_deg = self.cols_deg[self.nonfixed_cols]
+                self._initialize_problem(rows_deg=rows_deg, cols_deg=cols_deg)
             if self.method == 'root':
                 sol = self._solve_root()
             else:
                 x0 = self.x0
                 sol = sof.solver(
                     x0,
                     fun=self.fun,
@@ -635,15 +817,20 @@
                     method=self.method,
                     verbose=self.verbose,
                     regularise=self.regularise,
                     full_return=self.full_return,
                     linsearch=self.linsearch,
                 )
             self._set_solved_problem(sol)
-            r_avg_mat = nef.bicm_from_fitnesses(self.x[self.nonfixed_rows], self.y[self.nonfixed_cols])
+            if self.continuous_weights:
+                r_avg_mat = nef.biwcm_c_from_fitnesses(self.x[self.nonfixed_rows], self.y[self.nonfixed_cols])
+            elif self.weighted:
+                r_avg_mat = nef.biwcm_d_from_fitnesses(self.x[self.nonfixed_rows], self.y[self.nonfixed_cols])
+            else:
+                r_avg_mat = nef.bicm_from_fitnesses(self.x[self.nonfixed_rows], self.y[self.nonfixed_cols])
             self.avg_mat[self.nonfixed_rows[:, None], self.nonfixed_cols] = np.copy(r_avg_mat)
 
     def _solve_bicm_light(self):
         """
         Internal method for computing the solution of the BiCM via degree sequences.
         """
         self._initialize_fitnesses()
@@ -675,64 +862,99 @@
     def _set_parameters(self, method, initial_guess, tol, eps, regularise, max_steps, verbose, linsearch, exp,
                         full_return):
         """
         Internal method for setting the parameters of the solver.
         """
         self.method = method
         self.initial_guess = initial_guess
-        self.tol = tol
-        self.eps = eps
+        if tol is None:
+            self.tol = 1e-8
+            if self.weighted:
+                self.tol *= 1e-10
+        else:
+            self.tol = tol
+        if eps is None:
+            self.eps = 1e-8
+            if self.weighted:
+                self.eps *= 1e-10
+        else:
+            self.eps = tol
         self.verbose = verbose
         self.linsearch = linsearch
         self.regularise = regularise
         self.exp = exp
         self.full_return = full_return
         if max_steps is None:
             if method == 'fixed-point':
                 self.max_steps = 200
             else:
                 self.max_steps = 100
+            if self.weighted:
+                self.max_steps *= 1000
         else:
             self.max_steps = max_steps
 
     def solve_tool(
             self,
-            method='newton',
+            method=None,
             initial_guess=None,
             light_mode=None,
-            tol=1e-8,
-            eps=1e-8,
+            tol=None,
+            eps=None,
             max_steps=None,
             verbose=False,
             linsearch=True,
             regularise=None,
             print_error=True,
             full_return=False,
-            exp=False):
+            exp=False,
+            model=None):
         """Solve the BiCM of the graph.
         It does not return the solution, use the getter methods instead.
 
         :param bool light_mode: Doesn't use matrices in the computation if this is set to True.
             If the graph has been initialized without the matrix, the light mode is used regardless.
-        :param str method: Method of choice among *newton*, *quasinewton* or *iterative*, default is newton
-        :param str initial_guess: Initial guess of choice among *None*, *random*, *uniform* or *degrees*, default is None
+        :param str method: Method of choice among *newton*, *quasinewton* or *iterative*, default is set by the model
+        solved
+        :param str initial_guess: Initial guess of choice among *None*, *random*, *uniform* or *degrees*,
+        default is None
         :param float tol: Tolerance of the solution, optional
+        :param float eps: Tolerance of the difference between consecutive solutions, optional
         :param int max_steps: Maximum number of steps, optional
         :param bool, optional verbose: Print elapsed time, errors and iteration steps, optional
         :param bool linsearch: Implement the linesearch when searching for roots, default is True
         :param bool regularise: Regularise the matrices in the computations, optional
         :param bool print_error: Print the final error of the solution
+        :param bool full_return: If True, the solver returns some more insights on the convergence. Default False.
         :param bool exp: if this is set to true the solver works with the reparameterization $x_i = e^{-\theta_i}$,
             $y_\alpha = e^{-\theta_\alpha}$. It might be slightly faster but also might not converge.
+        :param str model: Model to be used, to be passed only if the user wants to use a different model
+        than the recognized one.
         """
+        if model == 'biwcm_c':
+            self.continuous_weights = True
+            self.weighted = True
+        elif model == 'biwcm_d':
+            self.continuous_weights = False
+            self.weighted = True
+        elif model == 'bicm':
+            self.weighted = False
+            self.continuous_weights = False
+        if method is None:
+            if self.continuous_weights:
+                method = 'fixed-point'
+            # elif self.weighted:
+            #     method = 'quasinewton'
+            else:
+                method = 'newton'
         if not self.is_initialized:
             print('Graph is not initialized. I can\'t compute the BiCM.')
             return
         if regularise is None:
-            if exp:
+            if self.weighted or exp:
                 regularise = False
             else:
                 regularise = True
         if regularise and exp:
             print('Warning: regularise is only recommended in non-exp mode.')
         if method == 'root':
             exp = True
@@ -746,19 +968,27 @@
                 print('''
                 I cannot work with the full mode without the biadjacency matrix.
                 This will not account for disconnected or fully connected nodes.
                 Solving in light mode...
                 ''')
             self._solve_bicm_light()
         if print_error:
-            self.solution_converged = not bool(self._check_solution(return_error=True))
+            max_err = self._check_solution(return_error=True)
+            if max_err >= 0.001:
+                self.solution_converged = False
+            else:
+                self.solution_converged = True
             if self.solution_converged:
                 print('Solver converged.')
             else:
-                print('Solver did not converge.')
+                if max_err >= 1:
+                    print('Solver did not converge: error', max_err)
+                else:
+                    print('Solver finished with an error of {:.2f}%'.format(max_err * 100))
+            self.error = max_err
         self.is_randomized = True
 
     def solve_bicm(
             self,
             method='newton',
             initial_guess=None,
             light_mode=None,
@@ -824,20 +1054,21 @@
 
     def get_fitnesses(self):
         """See get_bicm_fitnesses."""
         self.get_bicm_fitnesses()
 
     def pval_calculator(self, v_list_key, x, y):
         """
-        Calculate the p-values of the v-motifs numbers of one vertices and all its neighbours.
+        Calculate the p-values of the v-motifs numbers of one vertex and all its neighbours.
 
         :param int v_list_key: the key of the node to consider for the adjacency list of the v-motifs.
         :param numpy.ndarray x: the fitnesses of the layer of the desired projection.
         :param numpy.ndarray y: the fitnesses of the opposite layer.
-        :returns: a dictionary containing as keys the nodes that form v-motifs with the considered node, and as values the corresponding p-values.
+        :returns: a dictionary containing as keys the nodes that form v-motifs with the
+        considered node, and as values the corresponding p-values.
         """
         node_xy = x[v_list_key] * y
         temp_pvals_dict = {}
         for neighbor in self.v_adj_list[v_list_key]:
             neighbor_xy = x[neighbor] * y
             probs = node_xy * neighbor_xy / ((1 + node_xy) * (1 + neighbor_xy))
             avg_v = np.sum(probs)
@@ -853,21 +1084,20 @@
                 sigma_v = np.sqrt(np.sum(var_v_arr))
                 gamma_v = (sigma_v ** (-3)) * np.sum(var_v_arr * (1 - 2 * probs))
                 eval_x = (self.v_adj_list[v_list_key][neighbor] + 0.5 - avg_v) / sigma_v
                 pval = norm.cdf(eval_x) + gamma_v * (1 - eval_x ** 2) * norm.pdf(eval_x) / 6
                 temp_pvals_dict[neighbor] = max(min(pval, 1), 0)
         return temp_pvals_dict
 
-    def pval_calculator_poibin(self, deg_couple, deg_dict, degs, x, y):
+    def pval_calculator_poibin(self, deg_couple, deg_dict, x, y):
         """
         Calculate the p-values of the v-motifs numbers of all nodes with a given couple degrees.
 
         :param tuple deg_couple: the couple of degrees considered.
-        :param tuple deg_couple: the couple of degrees considered.
-        :param tuple deg_couple: the couple of degrees considered.
+        :param dict deg_dict: node-degrees dictionary.
         :param numpy.ndarray x: the fitnesses of the layer of the desired projection.
         :param numpy.ndarray y: the fitnesses of the opposite layer.
         :returns: a list containing 3-tuples with the two nodes considered and their p-value.
         """
         node_xy = x[deg_dict[deg_couple[0]][0]] * y
         neighbor_xy = x[deg_dict[deg_couple[1]][0]] * y
         probs = node_xy * neighbor_xy / ((1 + node_xy) * (1 + neighbor_xy))
@@ -937,140 +1167,211 @@
             deg_couples = [(unique_degs[deg_i], unique_degs[deg_j])
                            for deg_i in range(len(unique_degs))
                            for deg_j in range(deg_i, len(unique_degs))]
             if self.progress_bar:
                 print('Calculating p-values...')
             if self.threads_num > 1:
                 with Pool(processes=self.threads_num) as pool:
-                    partial_function = partial(self.pval_calculator_poibin, deg_dict=deg_dict, degs=degs, x=x, y=y)
+                    partial_function = partial(self.pval_calculator_poibin, deg_dict=deg_dict, x=x, y=y)
                     if self.progress_bar:
                         pvals_dicts = pool.map(partial_function, tqdm(deg_couples))
                     else:
                         pvals_dicts = pool.map(partial_function, deg_couples)
             else:
                 pvals_dicts = []
                 if self.progress_bar:
                     for deg_couple in tqdm(deg_couples):
                         pvals_dicts.append(
-                            self.pval_calculator_poibin(deg_couple, deg_dict=deg_dict, degs=degs, x=x, y=y))
+                            self.pval_calculator_poibin(deg_couple, deg_dict=deg_dict, x=x, y=y))
                 else:
                     for deg_couple in v_list_coupled:
                         pvals_dicts.append(
-                            self.pval_calculator_poibin(deg_couple, deg_dict=deg_dict, degs=degs, x=x, y=y))
+                            self.pval_calculator_poibin(deg_couple, deg_dict=deg_dict, x=x, y=y))
             pval_adj_list = {k: dict() for k in self.v_adj_list}
             for pvals_dict in pvals_dicts:
                 for node in pvals_dict:
                     pval_adj_list[node].update(pvals_dict[node])
         return pval_adj_list
 
-    def compute_projection(self, rows=True, alpha=0.05, method='poisson', threads_num=None, progress_bar=True):
+    def compute_projection(self, rows=True, alpha=0.05, approx_method=None, method=None,
+                           threads_num=None, progress_bar=True, validation_method='fdr'):
         """Compute the projection of the network on the rows or columns layer.
         If the BiCM has not been computed, it also computes it with standard settings.
         This is the most customizable method for the pvalues computation.
 
-        :param bool rows: True if requesting the rows projection.
-        :param float alpha: Threshold for the FDR validation.
-        :param str method: Method for the approximation of the pvalues computation.
+        :param bool rows: True if requesting the rows' projection.
+        :param float alpha: Threshold for the p-values validation.
+        :param str approx_method: Method for the approximation of the pvalues computation.
             Implemented methods are *poisson*, *poibin*, *normal*, *rna*.
+        :param str method: Deprecated, same as approx_method.
         :param threads_num: Number of threads to use for the parallelization. If it is set to 1,
             the computation is not parallelized.
         :param bool progress_bar: Show progress bar of the pvalues computation.
+        :param str validation_method:  The type of validation to apply: 'global' for a global threshold,
+         'fdr' for False Discovery Rate or 'bonferroni' for Bonferroni correction.
         """
+        if approx_method is None:
+            if method is not None:
+                print('"method" is deprecated, use approx_method instead')
+                approx_method = method
+            else:
+                approx_method = 'poisson'
         self.rows_projection = rows
-        self.projection_method = method
+        self.projection_method = approx_method
         self.progress_bar = progress_bar
+        if self.weighted:
+            print('Weighted projection not yet implemented.')
+            return
         if threads_num is None:
             if system() == 'Windows':
                 threads_num = 1
             else:
                 threads_num = 4
         else:
             if system() == 'Windows' and threads_num != 1:
                 threads_num = 1
                 print('Parallel processes not yet implemented on Windows, computing anyway...')
         self.threads_num = threads_num
-        if self.adj_list is None:
+        if self.adj_list is None and self.biadjacency is None:
             print('''
             Without the edges I can't compute the projection. 
             Use set_biadjacency_matrix, set_adjacency_list or set_edgelist to add edges.
             ''')
             return
         else:
             if not self.is_randomized:
                 print('First I have to compute the BiCM. Computing...')
                 self.solve_tool()
             if rows:
                 self.rows_pvals = self._projection_calculator()
-                self.projected_rows_adj_list = self._projection_from_pvals(alpha=alpha)
+                self.projected_rows_adj_list = self._projection_from_pvals(alpha=alpha,
+                                                                           validation_method=validation_method)
                 self.is_rows_projected = True
             else:
                 self.cols_pvals = self._projection_calculator()
-                self.projected_cols_adj_list = self._projection_from_pvals(alpha=alpha)
+                self.projected_cols_adj_list = self._projection_from_pvals(alpha=alpha,
+                                                                           validation_method=validation_method)
                 self.is_cols_projected = True
+                
+    def compute_weighted_pvals_mat(self):
+        """
+        Compute the pvalues matrix representing the significance of the original matrix.
+        """
+        if self.biadjacency is None:
+            assert self.edgelist is not None or self.adj_list is not None, 'Graph links must be given in some format!'
+            print('Computing biadjacency matrix...')
+            if self.edgelist is not None:
+                self.biadjacency = nef.biadjacency_from_edgelist(self.edgelist)[0]
+            elif self.adj_list is not None:
+                self.biadjacency = nef.biadjacency_from_adjacency_list(self.adj_list)
+        if not self.is_randomized:
+            print('First I have to compute the BiCM. Computing...')
+            self.solve_tool()
+        if not self.weighted:
+            self.pvals_mat = self.avg_mat ** self.biadjacency
+        self.pvals_mat = (np.tile(self.x, (len(self.y), 1)).T * np.tile(self.y, (len(self.x), 1))) ** self.biadjacency
+
+    def get_weighted_pvals_mat(self):
+        """
+        Return the pvalues matrix representing the significance of the original matrix.
+        """
+        if self.pvals_mat is None:
+            self.compute_weighted_pvals_mat()
+        return self.pvals_mat
+
+    def get_validated_matrix(self, significance=0.01, validation_method=None):
+        """
+        Extract a backbone of the original network keeping only the most significant links.
+        At the moment this method only applies a global significance level for any link.
+
+        :param float significance:  Threshold for the pvalues significance.
+        :param str validation_method:  The type of validation to apply: 'global' for a global threshold,
+         'fdr' for False Discovery Rate or 'bonferroni' for Bonferroni correction.
+        """
+        if self.pvals_mat is None:
+            self.compute_weighted_pvals_mat()
+        if validation_method is None:
+            print('FDR validated matrix will be returned by default. '
+                  'Set validation_method to "global" or "bonferroni" for alternatives or use .get_weighted_pvals_mat.')
+            validation_method = 'fdr'
+        assert validation_method in ['bonferroni', 'fdr', 'global'], 'validation_method must be a valid string'
+        pvals_array = self.pvals_mat.flatten()
+        val_threshold = self._pvals_validator(pvals_array, alpha=significance, validation_method=validation_method)
+        return (self.pvals_mat < val_threshold).astype(np.ubyte)
 
-    def _pvals_validator(self, pval_list, alpha=0.05):
+    def _pvals_validator(self, pval_list, alpha=0.05, validation_method='fdr'):
         sorted_pvals = np.sort(pval_list)
         if self.rows_projection:
             multiplier = 2 * alpha / (self.n_rows * (self.n_rows - 1))
         else:
             multiplier = 2 * alpha / (self.n_cols * (self.n_cols - 1))
-        try:
-            eff_fdr_pos = np.where(sorted_pvals <= (np.arange(1, len(sorted_pvals) + 1) * alpha * multiplier))[0][-1]
-        except IndexError:
-            print('No V-motifs will be validated. Try increasing alpha')
-            eff_fdr_pos = 0
-        eff_fdr_th = (eff_fdr_pos + 1) * multiplier  # +1 because of Python numbering: our pvals are ordered 1,...,n
+        eff_fdr_th = alpha
+        if validation_method == 'bonferroni':
+            eff_fdr_th = multiplier
+            if sorted_pvals[0] > eff_fdr_th:
+                print('No V-motifs will be validated. Try increasing alpha')
+        elif validation_method == 'fdr':
+            try:
+                eff_fdr_pos = np.where(sorted_pvals <= (np.arange(1, len(sorted_pvals) + 1) * alpha * multiplier))[0][-1]
+            except IndexError:
+                print('No V-motifs will be validated. Try increasing alpha')
+                eff_fdr_pos = 0
+            eff_fdr_th = (eff_fdr_pos + 1) * multiplier  # +1 because of Python numbering: our pvals are ordered 1,...,n
         return eff_fdr_th
 
-    def _projection_from_pvals(self, alpha=0.05):
+    def _projection_from_pvals(self, alpha=0.05, validation_method='fdr'):
         """Internal method to build the projected network from pvalues.
 
-        :param float alpha:  Threshold for the FDR validation.
+        :param float alpha:  Threshold for the validation.
+        :param str validation_method:  The type of validation to apply.
         """
         pval_list = []
         if self.rows_projection:
             pvals_adj_list = self.rows_pvals
         else:
             pvals_adj_list = self.cols_pvals
         for node in pvals_adj_list:
             for neighbor in pvals_adj_list[node]:
                 pval_list.append(pvals_adj_list[node][neighbor])
-        eff_fdr_th = self._pvals_validator(pval_list, alpha=alpha)
+        eff_fdr_th = self._pvals_validator(pval_list, alpha=alpha, validation_method=validation_method)
         projected_adj_list = dict([])
         for node in self.v_adj_list:
             for neighbor in self.v_adj_list[node]:
                 if pvals_adj_list[node][neighbor] <= eff_fdr_th:
                     if node not in projected_adj_list.keys():
                         projected_adj_list[node] = []
                     projected_adj_list[node].append(neighbor)
         return projected_adj_list
 
     def get_rows_projection(self,
                             alpha=0.05,
                             method='poisson',
                             threads_num=None,
                             progress_bar=True,
-                            fmt='adjacency_list'):
+                            fmt='adjacency_list',
+                            validation_method='fdr'):
         """Get the projected network on the rows layer of the graph.
 
         :param alpha: threshold for the validation of the projected edges.
         :type alpha: float, optional
-        :param method: approximation method for the calculation of the p-values.a
+        :param method: approximation method for the calculation of the p-values.
             Implemented choices are: poisson, poibin, normal, rna
         :type method: str, optional
         :param threads_num: number of threads to use for the parallelization. If it is set to 1,
             the computation is not parallelized.
         :type threads_num: int, optional
         :param bool progress_bar: Show the progress bar
         :param str fmt: the desired format for the output: adjacency_list (default) or edgelist
         :returns: the projected network on the rows layer, in the format specified by fmt
+        :param str validation_method:  The type of validation to apply: 'global' for a global threshold,
+         'fdr' for False Discovery Rate or 'bonferroni' for Bonferroni correction.
         """
         if not self.is_rows_projected:
-            self.compute_projection(rows=True, alpha=alpha, method=method, threads_num=threads_num,
-                                    progress_bar=progress_bar)
+            self.compute_projection(rows=True, alpha=alpha, approx_method=method, threads_num=threads_num,
+                                    progress_bar=progress_bar, validation_method=validation_method)
 
         if self.rows_dict is None:
             adj_list_to_return = self.projected_rows_adj_list
         else:
             adj_list_to_return = {}
             for node in self.projected_rows_adj_list:
                 adj_list_to_return[self.rows_dict[node]] = []
@@ -1099,27 +1400,76 @@
         :type threads_num: int, optional
         :param bool progress_bar: Show the progress bar
         :param str fmt: the desired format for the output: adjacency_list (default) or edgelist
         :returns: the projected network on the columns layer, in the format specified by fmt
         """
         if not self.is_cols_projected:
             self.compute_projection(rows=False,
-                                    alpha=alpha, method=method, threads_num=threads_num, progress_bar=progress_bar)
+                                    alpha=alpha, approx_method=method, threads_num=threads_num, progress_bar=progress_bar)
         if self.cols_dict is None:
             return self.projected_cols_adj_list
         else:
             adj_list_to_return = {}
             for node in self.projected_cols_adj_list:
                 adj_list_to_return[self.cols_dict[node]] = []
                 for neighbor in self.projected_cols_adj_list[node]:
                     adj_list_to_return[self.cols_dict[node]].append(self.cols_dict[neighbor])
         if fmt == 'adjacency_list':
             return adj_list_to_return
         elif fmt == 'edgelist':
             return nef.edgelist_from_adjacency_list_bipartite(adj_list_to_return)
+        
+    def _compute_projected_pvals_mat(self, layer='rows'):
+        """
+        Compute the pvalues matrix representing the significance of the original matrix.
+        """
+        if layer == 'rows':
+            n_dim = self.n_rows
+            pval_adjlist = self.rows_pvals
+        elif layer == 'columns':
+            n_dim = self.n_cols
+            pval_adjlist = self.cols_pvals
+        pval_mat = np.ones((n_dim, n_dim))
+        for v in pval_adjlist:
+            for w in pval_adjlist[v]:
+                pval_mat[v,w] = pval_adjlist[v][w]
+                pval_mat[w,v] = pval_mat[v,w]
+        if layer == 'rows':
+            self.rows_pvals_mat = pval_mat
+        elif layer == 'columns':
+            self.cols_pvals_mat = pval_mat
+
+    def get_projected_pvals_mat(self, layer=None):
+        """
+        Return the pvalues matrix of the projection if it has been computed.
+        
+        :param layer: the layer to return.
+        :type layer: string, optional
+        """
+        if layer is None:
+            if not self.is_rows_projected and not self.is_cols_projected:
+                print('First compute a projection.')
+                return None
+            elif self.is_rows_projected and self.is_cols_projected:
+                print("Please specify the layer with layer='rows' or layer='columns'.")
+                return None
+            elif self.is_rows_projected:
+                layer = 'rows'
+            elif self.is_cols_projected:
+                layer = 'columns'
+        if layer == 'rows':
+            if self.rows_pvals_mat is None:
+                self._compute_projected_pvals_mat(layer=layer)
+            return self.rows_pvals_mat
+        elif layer == 'columns':
+            if self.cols_pvals_mat is None:
+                self._compute_projected_pvals_mat(layer=layer)
+            return self.cols_pvals_mat
+        else:
+            raise ValueError("layer must be either 'rows' or 'columns' or None")
 
     def set_biadjacency_matrix(self, biadjacency):
         """Set the biadjacency matrix of the graph.
 
         :param biadjacency: binary input matrix describing the biadjacency matrix
                 of a bipartite graph with the nodes of one layer along the rows
                 and the nodes of the other layer along the columns.
```

### Comparing `bicm-2.0.4/bicm/network_functions.py` & `bicm-3.0.0/bicm/network_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,51 @@
     for i in range(len(x)):
         for j in range(len(y)):
             xy = x[i] * y[j]
             avg_mat[i, j] = xy / (1 + xy)
     return avg_mat
 
 
+@jit(nopython=True)
+def biwcm_d_from_fitnesses(x, y):
+    """
+    Rebuilds the average probability matrix of the BiWCM_d from the fitnesses
+
+    :param x: the fitness vector of the rows layer
+    :type x: numpy.ndarray
+    :param y: the fitness vector of the columns layer
+    :type y: numpy.ndarray
+    """
+    avg_mat = np.zeros((len(x), len(y)))
+    for i in range(len(x)):
+        for j in range(len(y)):
+            xy = x[i] * y[j]
+            avg_mat[i, j] = xy / (1 - xy)
+    return avg_mat
+
+
+@jit(nopython=True)
+def biwcm_c_from_fitnesses(x, y):
+    """
+    Rebuilds the average probability matrix of the BiWCM_c from the fitnesses
+
+    :param x: the fitness vector of the rows layer
+    :type x: numpy.ndarray
+    :param y: the fitness vector of the columns layer
+    :type y: numpy.ndarray
+    """
+    avg_mat = np.zeros((len(x), len(y)))
+    theta_x = - np.log(x)
+    theta_y = - np.log(y)
+    for i in range(len(x)):
+        for j in range(len(y)):
+            avg_mat[i, j] = 1 / (theta_x[i] + theta_y[j])
+    return avg_mat
+
+
 def sample_bicm(avg_mat):
     """
     Build a biadjacency matrix sampling from the probability matrix of a BiCM.
     """
     if not isinstance(avg_mat, np.ndarray):
         avg_mat = np.array(avg_mat)
     dim1, dim2 = avg_mat.shape
@@ -79,22 +116,22 @@
     Build the edgelist of a bipartite network from its biadjacency matrix.
     Accounts for sparse matrices and returns a structured array.
     """
     if scipy.sparse.isspmatrix(biadjacency):
         coords = biadjacency.nonzero()
         if np.sum(biadjacency.data != 1) > 0:
             raise ValueError('Only binary matrices')
-        return np.array(list(zip(coords[0], coords[1])), dtype=np.dtype([('rows', int), ('columns', int)])),\
-               np.array(biadjacency.sum(1)).flatten(), np.array(biadjacency.sum(0)).flatten()
+        return np.array(list(zip(coords[0], coords[1])), dtype=np.dtype([('rows', int), ('columns', int)])), \
+            np.array(biadjacency.sum(1)).flatten(), np.array(biadjacency.sum(0)).flatten()
     else:
         if np.sum(biadjacency[biadjacency != 0] != 1) > 0:
             raise ValueError('Only binary matrices')
         return np.array(edgelist_from_biadjacency_fast(biadjacency),
-                        dtype=np.dtype([('rows', int), ('columns', int)])),\
-               np.sum(biadjacency, axis=1), np.sum(biadjacency, axis=0)
+                        dtype=np.dtype([('rows', int), ('columns', int)])), \
+            np.sum(biadjacency, axis=1), np.sum(biadjacency, axis=0)
 
 
 def biadjacency_from_edgelist(edgelist, fmt='array'):
     """
     Build the biadjacency matrix of a bipartite network from its edgelist.
     Returns a matrix of the type specified by ``fmt``, by default a numpy array.
     """
@@ -134,18 +171,22 @@
     return edgelist_new, rows_degs, cols_degs, rows_dict, cols_dict
 
 
 def adjacency_list_from_edgelist_bipartite(edgelist, convert_type=True):
     """
     Creates the adjacency list from the edgelist.
     Method for bipartite networks.
-    Returns two dictionaries, each containing an adjacency list with the rows as keys and the columns as keys, respectively.
+    Returns two dictionaries containing an adjacency list with the rows as keys and the columns as keys, respectively.
     If convert_type is True (default), then the nodes are enumerated and the adjacency list is returned as integers.
     Returns also two dictionaries that keep track of the nodes and the two degree sequences.
     """
+    rows_degs = None
+    cols_degs = None
+    rows_dict = None
+    cols_dict = None
     if convert_type:
         edgelist, rows_degs, cols_degs, rows_dict, cols_dict = edgelist_from_edgelist_bipartite(edgelist)
     adj_list = {}
     inv_adj_list = {}
     for edge in edgelist:
         adj_list.setdefault(edge[0], set()).add(edge[1])
         inv_adj_list.setdefault(edge[1], set()).add(edge[0])
@@ -163,15 +204,15 @@
     Method for bipartite networks.
     Returns two dictionaries, each representing an adjacency list with the rows or columns as keys, respectively.
     Original keys are treated as rows, values as columns.
     The nodes are enumerated and the adjacency list contains the related integers.
     Returns also two dictionaries that keep track of the nodes and the two degree sequences.
     """
     rows_dict = dict(enumerate(np.unique(list(old_adj_list.keys()))))
-    cols_dict = dict(enumerate(np.unique([el for l in old_adj_list.values() for el in l])))
+    cols_dict = dict(enumerate(np.unique([el for lst in old_adj_list.values() for el in lst])))
     inv_rows_dict = {v: k for k, v in rows_dict.items()}
     inv_cols_dict = {v: k for k, v in cols_dict.items()}
     adj_list = {}
     inv_adj_list = {}
     for k in old_adj_list:
         adj_list.setdefault(inv_rows_dict[k], set()).update({inv_cols_dict[val] for val in old_adj_list[k]})
         for val in old_adj_list[k]:
@@ -235,15 +276,15 @@
     Creates the biadjacency matrix from an adjacency list given as a dictionary.
     Returns the biadjacency as a numpy array by default, or sparse scipy matrix if fmt='sparse'.
     The biadjacency comes with the keys as rows of the matrix and the values as columns.
     :param dict adj_list: the adjacency list to be converted. Must contain integers that will be used as indexes.
     :param str fmt: the desired format of the output biadjacency matrix, either 'array' or 'sparse', optional
     """
     assert np.isin(fmt, ['array', 'sparse']), 'fmt must be either array or sparse'
-    assert isinstance(list(adj_list.keys())[0], (int, float, complex)), 'Adjacency list must be numeric'
+    assert isinstance(list(adj_list.keys())[0], (np.number)), 'Adjacency list must be numeric'
     rows_index = [k for k, v in adj_list.items() for _ in range(len(v))]
     cols_index = [i for ids in adj_list.values() for i in ids]
-    biad_mat = scipy.sparse.csr_matrix(([1] * len(rows_index), (rows_index, cols_index)))
+    biad_mat = scipy.sparse.csr_array(([1] * len(rows_index), (rows_index, cols_index)))
     if fmt == 'sparse':
         return biad_mat
     else:
         return biad_mat.toarray()
```

### Comparing `bicm-2.0.4/bicm/poibin.py` & `bicm-3.0.0/bicm/poibin.py`

 * *Files identical despite different names*

### Comparing `bicm-2.0.4/bicm/solver_functions.py` & `bicm-3.0.0/bicm/solver_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from numba import jit
 import time
 
 
 def matrix_regulariser_function(b, eps):
     """Trasforms input matrix in a positive defined matrix
     by adding positive quantites to the main diagonal.
+
     :param b: Matrix.
     :type b: numpy.ndarray
     :param eps: Positive quantity to add.
     :type eps: float
     :return: Regularised matrix.
     :rtype: numpy.ndarray
     """
@@ -20,14 +21,15 @@
 
     return bf
 
 
 def matrix_regulariser_function_eigen_based(b, eps):
     """Trasform input matrix in a positive defined matrix
     by regularising eigenvalues.
+
     :param b: Matrix.
     :type b: numpy.ndarray
     :param eps: Positive quantity to add.
     :type eps: float
     :return: Regularised matrix.
     :rtype: numpy.ndarray
     """
@@ -40,14 +42,15 @@
 
 
 @jit(nopython=True)
 def sufficient_decrease_condition(
     f_old, f_new, alpha, grad_f, p, c1=1e-04, c2=0.9
 ):
     """Returns True if upper wolfe condition is respected.
+
     :param f_old: Function value at previous iteration.
     :type f_old: float
     :param f_new: Function value at current iteration.
     :type f_new: float
     :param alpha: Alpha parameter of linsearch.
     :type alpha: float
     :param grad_f: Function gradient.
@@ -80,14 +83,15 @@
     regularise=True,
     regularise_eps=1e-3,
     full_return=False,
     linsearch=True,
 ):
     """Find roots of eq. fun = 0, using newton, quasinewton or
     fixed-point algorithm.
+
     :param x0: Initial point
     :type x0: numpy.ndarray
     :param fun: Function handle of the function to find the roots of.
     :type fun: function
     :param step_fun: Function to compute the algorithm step
     :type step_fun: function
     :param linsearch_fun: Function to compute the linsearch
@@ -291,8 +295,8 @@
         print("toc_loop = {}".format(toc_loop))
         print("toc_all = {}".format(toc_all))
 
     if full_return:
         return (x, toc_all, n_steps, np.array(norm_seq),
                 np.array(diff_seq), np.array(alfa_seq))
     else:
-        return x
+        return x
```

### Comparing `bicm-2.0.4/setup.py` & `bicm-3.0.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="bicm",
-    version="2.0.4",
+    version="3.0.0",
     author="Matteo Bruno",
-    author_email="matteo.bruno@imtlucca.it",
+    author_email="matteobruno180@gmail.com",
     description="Package for bipartite configuration model",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mat701/BiCM",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
@@ -22,10 +22,11 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.5',
     install_requires=[
                       "numpy>=1.14",
                       "scipy>=1.4",
-                      "tqdm>=4.52.0"
+                      "tqdm>=4.52.0",
+                      "numba>=0.52.0"
                       ],
 )
```

### Comparing `bicm-2.0.4/tests/BiCM_test.py` & `bicm-3.0.0/tests/BiCM_test.py`

 * *Files identical despite different names*

