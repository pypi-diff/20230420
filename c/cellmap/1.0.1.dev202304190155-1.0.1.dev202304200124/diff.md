# Comparing `tmp/cellmap-1.0.1.dev202304190155-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304200124-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1390321 bytes, number of entries: 6
+Zip file size: 1390356 bytes, number of entries: 6
 -rw-r--r--  2.0 unx  4446947 b- defN 80-Jan-01 00:00 cellmap/CellMap_view_3D.html
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx    62699 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1785 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304190155.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304190155.dist-info/WHEEL
-?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304190155.dist-info/RECORD
-6 files, 4512063 bytes uncompressed, 1389435 bytes compressed:  69.2%
+-rw-r--r--  2.0 unx    63297 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1785 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304200124.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304200124.dist-info/WHEEL
+?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304200124.dist-info/RECORD
+6 files, 4512661 bytes uncompressed, 1389470 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304190155.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304200124.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304190155.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304200124.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304190155.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304200124.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -1,27 +1,29 @@
 from adjustText import adjust_text
 import anndata
 import numpy as np
 import matplotlib
 import matplotlib.pyplot as plt
-from matplotlib import patheffects as PathEffects
 import matplotlib.cm
+import matplotlib.colors
+from matplotlib import patheffects as PathEffects
+
 import networkx as nx
 import scipy
 import sklearn.preprocessing
 import sklearn.neighbors
 from sklearn.linear_model import LinearRegression
 from sklearn.preprocessing import PolynomialFeatures
-import matplotlib.colors
 import pandas as pd
+import plotly.graph_objects as go
+from plotly.offline import plot
 import logging
 import scanpy
 import scvelo as scv
-import plotly.graph_objects as go
-from plotly.offline import plot
+
 
 
 def create_graph(
     X,
     Y,
     cutedge_vol = None,
     cutedge_length = None,
@@ -1273,16 +1275,22 @@
     path_key = 'path',
     n_neighbors = 10,
     contribution_rate_pca = 0.95,
     cutedge_vol  = None,
     cutedge_length = None,
 ):
 
-    # kwargs_arg = check_arguments(adata, verbose = True, exp_key=exp_key, vkey = vkey, basis=basis, graph_method=graph_method)
-    # exp_key,vkey,basis = kwargs_arg['exp_key'],kwargs_arg['vkey'],kwargs_arg['basis']
+    kwargs_arg = check_arguments(adata, verbose = True, basis=basis)
+    basis = kwargs_arg['basis']
+
+    if sum(adata.obs[cluster_key].values == source_cluster) == 0:
+        raise KeyError('Cluster %s was not found' % source_cluster)
+    for trg_ in target_clusters:
+        if sum(adata.obs[cluster_key].values == source_cluster) == 0:
+            raise KeyError('Cluster %s was not found' % trg_)
 
     basis_key = 'X_%s' % basis
     data_pos = adata.obsm[basis_key]
 
     ## Compute graph and edge velocities
     if graph_method == 'Delauney':
         tri_,idx_tri = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_mask = True)
@@ -1361,14 +1369,24 @@
     genes,
     path_key = 'path',
     exp_key = None,
     fontsize_title = 16,
     fontsize_label = 14,
     fontsize_legend = 12,
 ):
+    
+    kwargs_arg = check_arguments(adata, verbose = True, basis=basis)
+    basis = kwargs_arg['basis']
+
+    if sum(adata.obs[cluster_key].values == source_cluster) == 0:
+        raise KeyError('Cluster %s was not found' % source_cluster)
+    for trg_ in target_clusters:
+        if sum(adata.obs[cluster_key].values == source_cluster) == 0:
+            raise KeyError('Cluster %s was not found' % trg_)
+    
     if exp_key == None:
         if scipy.sparse.issparse(adata.X): data_exp = adata.X.toarray()
         else: data_exp = adata.X
     else:
         data_exp = adata.layers[exp_key]
     path = adata.uns[path_key]
     cmap_ = plt.get_cmap("tab10")
```

## Comparing `cellmap-1.0.1.dev202304190155.dist-info/METADATA` & `cellmap-1.0.1.dev202304200124.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304190155
+Version: 1.0.1.dev202304200124
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

