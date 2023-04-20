# Comparing `tmp/phast-0.1.0.tar.gz` & `tmp/phast-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phast-0.1.0.tar", max compression
+gzip compressed data, was "phast-0.1.1.tar", max compression
```

## Comparing `phast-0.1.0.tar` & `phast-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-03-03 17:36:07.565556 phast-0.1.0/LICENSE
--rw-r--r--   0        0        0     4916 2023-04-01 17:58:12.826567 phast-0.1.0/README.md
--rw-r--r--   0        0        0      430 2023-04-01 17:56:35.949582 phast-0.1.0/phast/__init__.py
--rw-r--r--   0        0        0    18523 2023-04-01 17:44:59.078037 phast-0.1.0/phast/embedding.py
--rw-r--r--   0        0        0    20280 2023-04-01 17:19:54.691659 phast-0.1.0/phast/graph_rewiring.py
--rw-r--r--   0        0        0      686 2023-03-31 19:53:39.169536 phast-0.1.0/phast/utils.py
--rw-r--r--   0        0        0      649 2023-04-01 17:59:32.491844 phast-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5692 1970-01-01 00:00:00.000000 phast-0.1.0/setup.py
--rw-r--r--   0        0        0     5478 1970-01-01 00:00:00.000000 phast-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-03-03 17:36:07.565556 phast-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5556 2023-04-01 18:34:54.482182 phast-0.1.1/README.md
+-rw-r--r--   0        0        0      430 2023-04-01 17:56:35.949582 phast-0.1.1/phast/__init__.py
+-rw-r--r--   0        0        0    18705 2023-04-01 18:34:54.482599 phast-0.1.1/phast/embedding.py
+-rw-r--r--   0        0        0    20280 2023-04-01 17:19:54.691659 phast-0.1.1/phast/graph_rewiring.py
+-rw-r--r--   0        0        0      686 2023-03-31 19:53:39.169536 phast-0.1.1/phast/utils.py
+-rw-r--r--   0        0        0      648 2023-04-20 15:14:59.060240 phast-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6338 1970-01-01 00:00:00.000000 phast-0.1.1/setup.py
+-rw-r--r--   0        0        0     6109 1970-01-01 00:00:00.000000 phast-0.1.1/PKG-INFO
```

### Comparing `phast-0.1.0/LICENSE` & `phast-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `phast-0.1.0/README.md` & `phast-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,58 @@
 <p align="center">
-<br/>
-<strong><a href="https://github.com/vict0rsch/phast" target="_blank">💻 Code</a></strong>
+<strong><a href="https://github.com/vict0rsch/phast" target="_blank">💻&nbsp;&nbsp;Code</a></strong>
 <strong>&nbsp;&nbsp;•&nbsp;&nbsp;</strong>
-<strong><a href="https://phast.readthedocs.io/" target="_blank">Docs 📑</a></strong>
-<br/>
+<strong><a href="https://phast.readthedocs.io/" target="_blank">Docs&nbsp;&nbsp;📑</a></strong>
 </p>
 
-# PhAST: Physics-Aware, Scalable, and Task-specific GNNs for Accelerated Catalyst Design
-
 <p align="center">
     <a>
-	    <img src='https://img.shields.io/badge/python-3.9%2B-blue' alt='Python' />
+	    <img src='https://img.shields.io/badge/python-3.8%2B-blue' alt='Python' />
 	</a>
 	<a href='https://phast.readthedocs.io/en/latest/?badge=latest'>
     	<img src='https://readthedocs.org/projects/phast/badge/?version=latest' alt='Documentation Status' />
 	</a>
     <a href="https://github.com/psf/black">
 	    <img src='https://img.shields.io/badge/code%20style-black-black' />
 	</a>
+<a href="https://pytorch.org">
+<img src="https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?logo=PyTorch&logoColor=white"/>
+</a>
 </p>
+<br/>
+
+# PhAST: Physics-Aware, Scalable, and Task-specific GNNs for Accelerated Catalyst Design
 
-## About
 
 This repository contains implementations for 2 of the PhAST components presented in the [paper](https://arxiv.org/abs/2211.12020):
 
 * `PhysEmbedding` that allows one to create an embedding vector from atomic numbers that is the concatenation of:
   * A learned embedding for the atom's group
   * A learned embedding for the atom's period
   * A fixed or learned embedding from a set of known physical properties, as reported by [`mendeleev`](https://mendeleev.readthedocs.io/en/stable/data.html#elements)
   * In the case of the OC20 dataset, a learned embedding for the atom's tag (adsorbate, catalyst surface or catalyst sub-surface)
 * Tag-based **graph rewiring** strategies for the OC20 dataset:
   * `remove_tag0_nodes` deletes all nodes in the graph associated with a tag 0 and recomputes edges
   * `one_supernode_per_graph` replaces all tag 0 atoms with a single new atom
-  * `one_supernode_per_atom_typs` replaces all tag 0 atoms *of a given element* with its own super node
+  * `one_supernode_per_atom_type` replaces all tag 0 atoms *of a given element* with its own super node
 
     <img src="https://raw.githubusercontent.com/vict0rsch/phast/main/examples/data/rewiring.png" width="600px" />
 
 Also: https://github.com/vict0rsch/faenet
 
+## Installation
+
+```
+pip install phast
+```
+
+⚠️ The above installation does not include `torch_geometric` which is a complex and very variable dependency you have to install yourself if you want to use the graph re-wiring functions of `phast`.
+
+☮️ Ignore `torch_geometric` if you only care about the `PhysEmbeddings`.
+
 ## Getting started
 
 ### Physical embeddings
 
 ![Embedding illustration](https://raw.githubusercontent.com/vict0rsch/phast/main/examples/data/embedding.png)
 
 ```python
@@ -61,14 +72,18 @@
 tags = torch.randint(0, 3, (3, 12))
 phys_embedding = PhysEmbedding(
     tag_emb_size=32, # default is 0, this is OC20-specific
     final_proj_size=64, # default is 0, no projection, just the concat. of embeds.
 )
 
 h = phys_embedding(z, tags) # h.shape = (3, 12, 64)
+
+# Assuming torch_geometric is installed:
+data = torch.load("examples/data/is2re_bs3.pt")
+h = phys_embedding(data.atomic_numbers.long(), data.tags) # h.shape = (261, 64)
 ```
 
 ### Graph rewiring
 
 ![Rewiring illustration](https://raw.githubusercontent.com/vict0rsch/phast/main/examples/data/rewiring.png)
 
 ```python
@@ -76,15 +91,15 @@
 import torch
 from phast.graph_rewiring import (
     remove_tag0_nodes,
     one_supernode_per_graph,
     one_supernode_per_atom_type,
 )
 
-data = torch.load("./examples/data/is2re_bs3.pt")  # 3 OC20 IS2RE data samples
+data = torch.load("./examples/data/is2re_bs3.pt")  # 3 batched OC20 IS2RE data samples
 print(
     "Data initially contains {} graphs, a total of {} atoms and {} edges".format(
         len(data.natoms), data.ptr[-1], len(data.cell_offsets)
     )
 )
 rewired_data = remove_tag0_nodes(deepcopy(data))
 print(
```

#### html2text {}

```diff
@@ -1,59 +1,67 @@
+                         ð»  Code   â¢   Docs  ð
+  [Python] [Documentation_Status] [https://img.shields.io/badge/code%20style-
+              black-black] [https://img.shields.io/badge/PyTorch-
+                  %23EE4C2C.svg?logo=PyTorch&logoColor=white]
 
-                         ð»_Code   â¢   Docs_ð
 # PhAST: Physics-Aware, Scalable, and Task-specific GNNs for Accelerated
-Catalyst Design
-  [Python] [Documentation_Status] [https://img.shields.io/badge/code%20style-
-                                 black-black]
-## About This repository contains implementations for 2 of the PhAST components
-presented in the [paper](https://arxiv.org/abs/2211.12020): * `PhysEmbedding`
-that allows one to create an embedding vector from atomic numbers that is the
-concatenation of: * A learned embedding for the atom's group * A learned
-embedding for the atom's period * A fixed or learned embedding from a set of
-known physical properties, as reported by [`mendeleev`](https://
-mendeleev.readthedocs.io/en/stable/data.html#elements) * In the case of the
-OC20 dataset, a learned embedding for the atom's tag (adsorbate, catalyst
-surface or catalyst sub-surface) * Tag-based **graph rewiring** strategies for
-the OC20 dataset: * `remove_tag0_nodes` deletes all nodes in the graph
-associated with a tag 0 and recomputes edges * `one_supernode_per_graph`
-replaces all tag 0 atoms with a single new atom * `one_supernode_per_atom_typs`
+Catalyst Design This repository contains implementations for 2 of the PhAST
+components presented in the [paper](https://arxiv.org/abs/2211.12020): *
+`PhysEmbedding` that allows one to create an embedding vector from atomic
+numbers that is the concatenation of: * A learned embedding for the atom's
+group * A learned embedding for the atom's period * A fixed or learned
+embedding from a set of known physical properties, as reported by [`mendeleev`]
+(https://mendeleev.readthedocs.io/en/stable/data.html#elements) * In the case
+of the OC20 dataset, a learned embedding for the atom's tag (adsorbate,
+catalyst surface or catalyst sub-surface) * Tag-based **graph rewiring**
+strategies for the OC20 dataset: * `remove_tag0_nodes` deletes all nodes in the
+graph associated with a tag 0 and recomputes edges * `one_supernode_per_graph`
+replaces all tag 0 atoms with a single new atom * `one_supernode_per_atom_type`
 replaces all tag 0 atoms *of a given element* with its own super node [https://
 raw.githubusercontent.com/vict0rsch/phast/main/examples/data/rewiring.png]
-Also: https://github.com/vict0rsch/faenet ## Getting started ### Physical
-embeddings ![Embedding illustration](https://raw.githubusercontent.com/
-vict0rsch/phast/main/examples/data/embedding.png) ```python import torch from
-phast.embedding import PhysEmbedding z = torch.randint(1, 85, (3, 12)) # batch
-of 3 graphs with 12 atoms each phys_embedding = PhysEmbedding( z_emb_size=32, #
-default period_emb_size=32, # default group_emb_size=32, # default
-properties_proj_size=32, # default is 0 -> no learned projection n_elements=85,
-# default ) h = phys_embedding(z) # h.shape = (3, 12, 128) tags = torch.randint
-(0, 3, (3, 12)) phys_embedding = PhysEmbedding( tag_emb_size=32, # default is
-0, this is OC20-specific final_proj_size=64, # default is 0, no projection,
-just the concat. of embeds. ) h = phys_embedding(z, tags) # h.shape = (3, 12,
-64) ``` ### Graph rewiring ![Rewiring illustration](https://
+Also: https://github.com/vict0rsch/faenet ## Installation ``` pip install phast
+``` â ï¸ The above installation does not include `torch_geometric` which is a
+complex and very variable dependency you have to install yourself if you want
+to use the graph re-wiring functions of `phast`. â®ï¸ Ignore
+`torch_geometric` if you only care about the `PhysEmbeddings`. ## Getting
+started ### Physical embeddings ![Embedding illustration](https://
+raw.githubusercontent.com/vict0rsch/phast/main/examples/data/embedding.png)
+```python import torch from phast.embedding import PhysEmbedding z =
+torch.randint(1, 85, (3, 12)) # batch of 3 graphs with 12 atoms each
+phys_embedding = PhysEmbedding( z_emb_size=32, # default period_emb_size=32, #
+default group_emb_size=32, # default properties_proj_size=32, # default is 0 -
+> no learned projection n_elements=85, # default ) h = phys_embedding(z) #
+h.shape = (3, 12, 128) tags = torch.randint(0, 3, (3, 12)) phys_embedding =
+PhysEmbedding( tag_emb_size=32, # default is 0, this is OC20-specific
+final_proj_size=64, # default is 0, no projection, just the concat. of embeds.
+) h = phys_embedding(z, tags) # h.shape = (3, 12, 64) # Assuming
+torch_geometric is installed: data = torch.load("examples/data/is2re_bs3.pt") h
+= phys_embedding(data.atomic_numbers.long(), data.tags) # h.shape = (261, 64)
+``` ### Graph rewiring ![Rewiring illustration](https://
 raw.githubusercontent.com/vict0rsch/phast/main/examples/data/rewiring.png)
 ```python from copy import deepcopy import torch from phast.graph_rewiring
 import ( remove_tag0_nodes, one_supernode_per_graph,
 one_supernode_per_atom_type, ) data = torch.load("./examples/data/
-is2re_bs3.pt") # 3 OC20 IS2RE data samples print( "Data initially contains {}
-graphs, a total of {} atoms and {} edges".format( len(data.natoms), data.ptr[-
-1], len(data.cell_offsets) ) ) rewired_data = remove_tag0_nodes(deepcopy(data))
-print( "Data without tag-0 nodes contains {} graphs, a total of {} atoms and {}
-edges".format( len(rewired_data.natoms), rewired_data.ptr[-1], len
-(rewired_data.cell_offsets) ) ) rewired_data = one_supernode_per_graph(deepcopy
-(data)) print( "Data with one super node per graph contains a total of {} atoms
-and {} edges".format( rewired_data.ptr[-1], len(rewired_data.cell_offsets) ) )
-rewired_data = one_supernode_per_atom_type(deepcopy(data)) print( "Data with
-one super node per atom type contains a total of {} atoms and {} edges".format
-( rewired_data.ptr[-1], len(rewired_data.cell_offsets) ) ) ``` ``` Data
-initially contains 3 graphs, a total of 261 atoms and 11596 edges Data without
-tag-0 nodes contains 3 graphs, a total of 64 atoms and 1236 edges Data with one
-super node per graph contains a total of 67 atoms and 1311 edges Data with one
-super node per atom type contains a total of 71 atoms and 1421 edges ``` ##
-Tests This requires [`poetry`](https://python-poetry.org/docs/). Make sure to
-have `torch` and `torch_geometric` installed in your environment before you can
-run the tests. Unfortunately because of CUDA/torch compatibilities, neither
-`torch` nor `torch_geometric` are part of the explicit dependencies and must be
-installed independently. ```bash git clone git@github.com:vict0rsch/phast.git
-poetry install --with dev pytest --cov=phast --cov-report term-missing ```
-Testing on Macs you may encounter a [Library Not Loaded Error](https://
-github.com/pyg-team/pytorch_geometric/issues/6530)
+is2re_bs3.pt") # 3 batched OC20 IS2RE data samples print( "Data initially
+contains {} graphs, a total of {} atoms and {} edges".format( len(data.natoms),
+data.ptr[-1], len(data.cell_offsets) ) ) rewired_data = remove_tag0_nodes
+(deepcopy(data)) print( "Data without tag-0 nodes contains {} graphs, a total
+of {} atoms and {} edges".format( len(rewired_data.natoms), rewired_data.ptr[-
+1], len(rewired_data.cell_offsets) ) ) rewired_data = one_supernode_per_graph
+(deepcopy(data)) print( "Data with one super node per graph contains a total of
+{} atoms and {} edges".format( rewired_data.ptr[-1], len
+(rewired_data.cell_offsets) ) ) rewired_data = one_supernode_per_atom_type
+(deepcopy(data)) print( "Data with one super node per atom type contains a
+total of {} atoms and {} edges".format( rewired_data.ptr[-1], len
+(rewired_data.cell_offsets) ) ) ``` ``` Data initially contains 3 graphs, a
+total of 261 atoms and 11596 edges Data without tag-0 nodes contains 3 graphs,
+a total of 64 atoms and 1236 edges Data with one super node per graph contains
+a total of 67 atoms and 1311 edges Data with one super node per atom type
+contains a total of 71 atoms and 1421 edges ``` ## Tests This requires
+[`poetry`](https://python-poetry.org/docs/). Make sure to have `torch` and
+`torch_geometric` installed in your environment before you can run the tests.
+Unfortunately because of CUDA/torch compatibilities, neither `torch` nor
+`torch_geometric` are part of the explicit dependencies and must be installed
+independently. ```bash git clone git@github.com:vict0rsch/phast.git poetry
+install --with dev pytest --cov=phast --cov-report term-missing ``` Testing on
+Macs you may encounter a [Library Not Loaded Error](https://github.com/pyg-
+team/pytorch_geometric/issues/6530)
```

### Comparing `phast-0.1.0/phast/embedding.py` & `phast-0.1.1/phast/embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,18 @@
     phys_embedding = PhysEmbedding(
         tag_emb_size=32, # default is 0, this is OC20-specific
         final_proj_size=64, # default is 0, no projection, just the concat. of embeds.
     )
 
     h = phys_embedding(z, tags) # h.shape = (3, 12, 64)
 
+    # Assuming torch_geometric is installed:
+
+    data = torch.load("examples/data/is2re_bs3.pt")
+    h = phys_embedding(data.atomic_numbers.long(), data.tags) # h.shape = (261, 64)
 
 """
 
 import os
 from typing import Optional
 import pandas as pd
 import torch
```

### Comparing `phast-0.1.0/phast/graph_rewiring.py` & `phast-0.1.1/phast/graph_rewiring.py`

 * *Files identical despite different names*

### Comparing `phast-0.1.0/phast/utils.py` & `phast-0.1.1/phast/utils.py`

 * *Files identical despite different names*

### Comparing `phast-0.1.0/setup.py` & `phast-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 packages = \
 ['phast']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['mendeleev>=0.12.1,<0.13.0', 'pandas>=1.4,<2.0', 'torch>=1.10.0,<2.0.0']
+['mendeleev>=0.12.1,<0.13.0', 'pandas>=1.4,<2.0', 'torch>=1.11']
 
 setup_kwargs = {
     'name': 'phast',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
-    'long_description': '<p align="center">\n<br/>\n<strong><a href="https://github.com/vict0rsch/phast" target="_blank">💻 Code</a></strong>\n<strong>&nbsp;&nbsp;•&nbsp;&nbsp;</strong>\n<strong><a href="https://phast.readthedocs.io/" target="_blank">Docs 📑</a></strong>\n<br/>\n</p>\n\n# PhAST: Physics-Aware, Scalable, and Task-specific GNNs for Accelerated Catalyst Design\n\n<p align="center">\n    <a>\n\t    <img src=\'https://img.shields.io/badge/python-3.9%2B-blue\' alt=\'Python\' />\n\t</a>\n\t<a href=\'https://phast.readthedocs.io/en/latest/?badge=latest\'>\n    \t<img src=\'https://readthedocs.org/projects/phast/badge/?version=latest\' alt=\'Documentation Status\' />\n\t</a>\n    <a href="https://github.com/psf/black">\n\t    <img src=\'https://img.shields.io/badge/code%20style-black-black\' />\n\t</a>\n</p>\n\n## About\n\nThis repository contains implementations for 2 of the PhAST components presented in the [paper](https://arxiv.org/abs/2211.12020):\n\n* `PhysEmbedding` that allows one to create an embedding vector from atomic numbers that is the concatenation of:\n  * A learned embedding for the atom\'s group\n  * A learned embedding for the atom\'s period\n  * A fixed or learned embedding from a set of known physical properties, as reported by [`mendeleev`](https://mendeleev.readthedocs.io/en/stable/data.html#elements)\n  * In the case of the OC20 dataset, a learned embedding for the atom\'s tag (adsorbate, catalyst surface or catalyst sub-surface)\n* Tag-based **graph rewiring** strategies for the OC20 dataset:\n  * `remove_tag0_nodes` deletes all nodes in the graph associated with a tag 0 and recomputes edges\n  * `one_supernode_per_graph` replaces all tag 0 atoms with a single new atom\n  * `one_supernode_per_atom_typs` replaces all tag 0 atoms *of a given element* with its own super node\n\n    <img src="https://raw.githubusercontent.com/vict0rsch/phast/main/examples/data/rewiring.png" width="600px" />\n\nAlso: https://github.com/vict0rsch/faenet\n\n## Getting started\n\n### Physical embeddings\n\n![Embedding illustration](https://raw.githubusercontent.com/vict0rsch/phast/main/examples/data/embedding.png)\n\n```python\nimport torch\nfrom phast.embedding import PhysEmbedding\n\nz = torch.randint(1, 85, (3, 12)) # batch of 3 graphs with 12 atoms each\nphys_embedding = PhysEmbedding(\n    z_emb_size=32, # default\n    period_emb_size=32, # default\n    group_emb_size=32, # default\n    properties_proj_size=32, # default is 0 -> no learned projection\n    n_elements=85, # default\n)\nh = phys_embedding(z) # h.shape = (3, 12, 128)\n\ntags = torch.randint(0, 3, (3, 12))\nphys_embedding = PhysEmbedding(\n    tag_emb_size=32, # default is 0, this is OC20-specific\n    final_proj_size=64, # default is 0, no projection, just the concat. of embeds.\n)\n\nh = phys_embedding(z, tags) # h.shape = (3, 12, 64)\n```\n\n### Graph rewiring\n\n![Rewiring illustration](https://raw.githubusercontent.com/vict0rsch/phast/main/examples/data/rewiring.png)\n\n```python\nfrom copy import deepcopy\nimport torch\nfrom phast.graph_rewiring import (\n    remove_tag0_nodes,\n    one_supernode_per_graph,\n    one_supernode_per_atom_type,\n)\n\ndata = torch.load("./examples/data/is2re_bs3.pt")  # 3 OC20 IS2RE data samples\nprint(\n    "Data initially contains {} graphs, a total of {} atoms and {} edges".format(\n        len(data.natoms), data.ptr[-1], len(data.cell_offsets)\n    )\n)\nrewired_data = remove_tag0_nodes(deepcopy(data))\nprint(\n    "Data without tag-0 nodes contains {} graphs, a total of {} atoms and {} edges".format(\n        len(rewired_data.natoms), rewired_data.ptr[-1], len(rewired_data.cell_offsets)\n    )\n)\nrewired_data = one_supernode_per_graph(deepcopy(data))\nprint(\n    "Data with one super node per graph contains a total of {} atoms and {} edges".format(\n        rewired_data.ptr[-1], len(rewired_data.cell_offsets)\n    )\n)\nrewired_data = one_supernode_per_atom_type(deepcopy(data))\nprint(\n    "Data with one super node per atom type contains a total of {} atoms and {} edges".format(\n        rewired_data.ptr[-1], len(rewired_data.cell_offsets)\n    )\n)\n```\n\n```\nData initially contains 3 graphs, a total of 261 atoms and 11596 edges\nData without tag-0 nodes contains 3 graphs, a total of 64 atoms and 1236 edges\nData with one super node per graph contains a total of 67 atoms and 1311 edges\nData with one super node per atom type contains a total of 71 atoms and 1421 edges\n```\n\n## Tests\n\nThis requires [`poetry`](https://python-poetry.org/docs/). Make sure to have `torch` and `torch_geometric` installed in your environment before you can run the tests. Unfortunately because of CUDA/torch compatibilities, neither `torch` nor `torch_geometric` are part of the explicit dependencies and must be installed independently.\n\n```bash\ngit clone git@github.com:vict0rsch/phast.git\npoetry install --with dev\npytest --cov=phast --cov-report term-missing\n```\n\nTesting on Macs you may encounter a [Library Not Loaded Error](https://github.com/pyg-team/pytorch_geometric/issues/6530)\n',
+    'long_description': '<p align="center">\n<strong><a href="https://github.com/vict0rsch/phast" target="_blank">💻&nbsp;&nbsp;Code</a></strong>\n<strong>&nbsp;&nbsp;•&nbsp;&nbsp;</strong>\n<strong><a href="https://phast.readthedocs.io/" target="_blank">Docs&nbsp;&nbsp;📑</a></strong>\n</p>\n\n<p align="center">\n    <a>\n\t    <img src=\'https://img.shields.io/badge/python-3.8%2B-blue\' alt=\'Python\' />\n\t</a>\n\t<a href=\'https://phast.readthedocs.io/en/latest/?badge=latest\'>\n    \t<img src=\'https://readthedocs.org/projects/phast/badge/?version=latest\' alt=\'Documentation Status\' />\n\t</a>\n    <a href="https://github.com/psf/black">\n\t    <img src=\'https://img.shields.io/badge/code%20style-black-black\' />\n\t</a>\n<a href="https://pytorch.org">\n<img src="https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?logo=PyTorch&logoColor=white"/>\n</a>\n</p>\n<br/>\n\n# PhAST: Physics-Aware, Scalable, and Task-specific GNNs for Accelerated Catalyst Design\n\n\nThis repository contains implementations for 2 of the PhAST components presented in the [paper](https://arxiv.org/abs/2211.12020):\n\n* `PhysEmbedding` that allows one to create an embedding vector from atomic numbers that is the concatenation of:\n  * A learned embedding for the atom\'s group\n  * A learned embedding for the atom\'s period\n  * A fixed or learned embedding from a set of known physical properties, as reported by [`mendeleev`](https://mendeleev.readthedocs.io/en/stable/data.html#elements)\n  * In the case of the OC20 dataset, a learned embedding for the atom\'s tag (adsorbate, catalyst surface or catalyst sub-surface)\n* Tag-based **graph rewiring** strategies for the OC20 dataset:\n  * `remove_tag0_nodes` deletes all nodes in the graph associated with a tag 0 and recomputes edges\n  * `one_supernode_per_graph` replaces all tag 0 atoms with a single new atom\n  * `one_supernode_per_atom_type` replaces all tag 0 atoms *of a given element* with its own super node\n\n    <img src="https://raw.githubusercontent.com/vict0rsch/phast/main/examples/data/rewiring.png" width="600px" />\n\nAlso: https://github.com/vict0rsch/faenet\n\n## Installation\n\n```\npip install phast\n```\n\n⚠️ The above installation does not include `torch_geometric` which is a complex and very variable dependency you have to install yourself if you want to use the graph re-wiring functions of `phast`.\n\n☮️ Ignore `torch_geometric` if you only care about the `PhysEmbeddings`.\n\n## Getting started\n\n### Physical embeddings\n\n![Embedding illustration](https://raw.githubusercontent.com/vict0rsch/phast/main/examples/data/embedding.png)\n\n```python\nimport torch\nfrom phast.embedding import PhysEmbedding\n\nz = torch.randint(1, 85, (3, 12)) # batch of 3 graphs with 12 atoms each\nphys_embedding = PhysEmbedding(\n    z_emb_size=32, # default\n    period_emb_size=32, # default\n    group_emb_size=32, # default\n    properties_proj_size=32, # default is 0 -> no learned projection\n    n_elements=85, # default\n)\nh = phys_embedding(z) # h.shape = (3, 12, 128)\n\ntags = torch.randint(0, 3, (3, 12))\nphys_embedding = PhysEmbedding(\n    tag_emb_size=32, # default is 0, this is OC20-specific\n    final_proj_size=64, # default is 0, no projection, just the concat. of embeds.\n)\n\nh = phys_embedding(z, tags) # h.shape = (3, 12, 64)\n\n# Assuming torch_geometric is installed:\ndata = torch.load("examples/data/is2re_bs3.pt")\nh = phys_embedding(data.atomic_numbers.long(), data.tags) # h.shape = (261, 64)\n```\n\n### Graph rewiring\n\n![Rewiring illustration](https://raw.githubusercontent.com/vict0rsch/phast/main/examples/data/rewiring.png)\n\n```python\nfrom copy import deepcopy\nimport torch\nfrom phast.graph_rewiring import (\n    remove_tag0_nodes,\n    one_supernode_per_graph,\n    one_supernode_per_atom_type,\n)\n\ndata = torch.load("./examples/data/is2re_bs3.pt")  # 3 batched OC20 IS2RE data samples\nprint(\n    "Data initially contains {} graphs, a total of {} atoms and {} edges".format(\n        len(data.natoms), data.ptr[-1], len(data.cell_offsets)\n    )\n)\nrewired_data = remove_tag0_nodes(deepcopy(data))\nprint(\n    "Data without tag-0 nodes contains {} graphs, a total of {} atoms and {} edges".format(\n        len(rewired_data.natoms), rewired_data.ptr[-1], len(rewired_data.cell_offsets)\n    )\n)\nrewired_data = one_supernode_per_graph(deepcopy(data))\nprint(\n    "Data with one super node per graph contains a total of {} atoms and {} edges".format(\n        rewired_data.ptr[-1], len(rewired_data.cell_offsets)\n    )\n)\nrewired_data = one_supernode_per_atom_type(deepcopy(data))\nprint(\n    "Data with one super node per atom type contains a total of {} atoms and {} edges".format(\n        rewired_data.ptr[-1], len(rewired_data.cell_offsets)\n    )\n)\n```\n\n```\nData initially contains 3 graphs, a total of 261 atoms and 11596 edges\nData without tag-0 nodes contains 3 graphs, a total of 64 atoms and 1236 edges\nData with one super node per graph contains a total of 67 atoms and 1311 edges\nData with one super node per atom type contains a total of 71 atoms and 1421 edges\n```\n\n## Tests\n\nThis requires [`poetry`](https://python-poetry.org/docs/). Make sure to have `torch` and `torch_geometric` installed in your environment before you can run the tests. Unfortunately because of CUDA/torch compatibilities, neither `torch` nor `torch_geometric` are part of the explicit dependencies and must be installed independently.\n\n```bash\ngit clone git@github.com:vict0rsch/phast.git\npoetry install --with dev\npytest --cov=phast --cov-report term-missing\n```\n\nTesting on Macs you may encounter a [Library Not Loaded Error](https://github.com/pyg-team/pytorch_geometric/issues/6530)\n',
     'author': 'Victor Schmidt',
     'author_email': 'vsch@pm.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,51 +1,58 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['phast']
 package_data = \ {'': ['*']} install_requires = \ ['mendeleev>=0.12.1,<0.13.0',
-'pandas>=1.4,<2.0', 'torch>=1.10.0,<2.0.0'] setup_kwargs = { 'name': 'phast',
-'version': '0.1.0', 'description': '', 'long_description': '
-                                      \n
-                       \nð»_Code\n  â¢  \nDocs_ð\n
-                                      \n
-\n\n# PhAST: Physics-Aware, Scalable, and Task-specific GNNs for Accelerated
-Catalyst Design\n\n
+'pandas>=1.4,<2.0', 'torch>=1.11'] setup_kwargs = { 'name': 'phast', 'version':
+'0.1.1', 'description': '', 'long_description': '
+                      \nð»  Code\n  â¢  \nDocs  ð\n
+\n\n
   \n \n\t [\'Python\']\n\t\n\t\n_\t'_/>\n\t\n \n\t_[\'https://img.shields.io/
-                    badge/code%20style-black-black\']\n\t\n
-\n\n## About\n\nThis repository contains implementations for 2 of the PhAST
-components presented in the [paper](https://arxiv.org/abs/2211.12020):\n\n*
-`PhysEmbedding` that allows one to create an embedding vector from atomic
+badge/code%20style-black-black\']\n\t\n\n[https://img.shields.io/badge/PyTorch-
+                %23EE4C2C.svg?logo=PyTorch&logoColor=white]\n\n
+\n
+\n\n# PhAST: Physics-Aware, Scalable, and Task-specific GNNs for Accelerated
+Catalyst Design\n\n\nThis repository contains implementations for 2 of the
+PhAST components presented in the [paper](https://arxiv.org/abs/2211.12020):
+\n\n* `PhysEmbedding` that allows one to create an embedding vector from atomic
 numbers that is the concatenation of:\n * A learned embedding for the atom\'s
 group\n * A learned embedding for the atom\'s period\n * A fixed or learned
 embedding from a set of known physical properties, as reported by [`mendeleev`]
 (https://mendeleev.readthedocs.io/en/stable/data.html#elements)\n * In the case
 of the OC20 dataset, a learned embedding for the atom\'s tag (adsorbate,
 catalyst surface or catalyst sub-surface)\n* Tag-based **graph rewiring**
 strategies for the OC20 dataset:\n * `remove_tag0_nodes` deletes all nodes in
 the graph associated with a tag 0 and recomputes edges\n *
 `one_supernode_per_graph` replaces all tag 0 atoms with a single new atom\n *
-`one_supernode_per_atom_typs` replaces all tag 0 atoms *of a given element*
+`one_supernode_per_atom_type` replaces all tag 0 atoms *of a given element*
 with its own super node\n\n [https://raw.githubusercontent.com/vict0rsch/phast/
 main/examples/data/rewiring.png]\n\nAlso: https://github.com/vict0rsch/
-faenet\n\n## Getting started\n\n### Physical embeddings\n\n![Embedding
-illustration](https://raw.githubusercontent.com/vict0rsch/phast/main/examples/
-data/embedding.png)\n\n```python\nimport torch\nfrom phast.embedding import
-PhysEmbedding\n\nz = torch.randint(1, 85, (3, 12)) # batch of 3 graphs with 12
-atoms each\nphys_embedding = PhysEmbedding(\n z_emb_size=32, # default\n
-period_emb_size=32, # default\n group_emb_size=32, # default\n
-properties_proj_size=32, # default is 0 -> no learned projection\n
-n_elements=85, # default\n)\nh = phys_embedding(z) # h.shape = (3, 12,
-128)\n\ntags = torch.randint(0, 3, (3, 12))\nphys_embedding = PhysEmbedding(\n
-tag_emb_size=32, # default is 0, this is OC20-specific\n final_proj_size=64, #
-default is 0, no projection, just the concat. of embeds.\n)\n\nh =
-phys_embedding(z, tags) # h.shape = (3, 12, 64)\n```\n\n### Graph rewiring\n\n!
-[Rewiring illustration](https://raw.githubusercontent.com/vict0rsch/phast/main/
-examples/data/rewiring.png)\n\n```python\nfrom copy import deepcopy\nimport
-torch\nfrom phast.graph_rewiring import (\n remove_tag0_nodes,\n
-one_supernode_per_graph,\n one_supernode_per_atom_type,\n)\n\ndata = torch.load
-("./examples/data/is2re_bs3.pt") # 3 OC20 IS2RE data samples\nprint(\n "Data
-initially contains {} graphs, a total of {} atoms and {} edges".format(\n len
+faenet\n\n## Installation\n\n```\npip install phast\n```\n\nâ ï¸ The above
+installation does not include `torch_geometric` which is a complex and very
+variable dependency you have to install yourself if you want to use the graph
+re-wiring functions of `phast`.\n\nâ®ï¸ Ignore `torch_geometric` if you only
+care about the `PhysEmbeddings`.\n\n## Getting started\n\n### Physical
+embeddings\n\n![Embedding illustration](https://raw.githubusercontent.com/
+vict0rsch/phast/main/examples/data/embedding.png)\n\n```python\nimport
+torch\nfrom phast.embedding import PhysEmbedding\n\nz = torch.randint(1, 85,
+(3, 12)) # batch of 3 graphs with 12 atoms each\nphys_embedding = PhysEmbedding
+(\n z_emb_size=32, # default\n period_emb_size=32, # default\n
+group_emb_size=32, # default\n properties_proj_size=32, # default is 0 -> no
+learned projection\n n_elements=85, # default\n)\nh = phys_embedding(z) #
+h.shape = (3, 12, 128)\n\ntags = torch.randint(0, 3, (3, 12))\nphys_embedding =
+PhysEmbedding(\n tag_emb_size=32, # default is 0, this is OC20-specific\n
+final_proj_size=64, # default is 0, no projection, just the concat. of
+embeds.\n)\n\nh = phys_embedding(z, tags) # h.shape = (3, 12, 64)\n\n# Assuming
+torch_geometric is installed:\ndata = torch.load("examples/data/
+is2re_bs3.pt")\nh = phys_embedding(data.atomic_numbers.long(), data.tags) #
+h.shape = (261, 64)\n```\n\n### Graph rewiring\n\n![Rewiring illustration]
+(https://raw.githubusercontent.com/vict0rsch/phast/main/examples/data/
+rewiring.png)\n\n```python\nfrom copy import deepcopy\nimport torch\nfrom
+phast.graph_rewiring import (\n remove_tag0_nodes,\n one_supernode_per_graph,\n
+one_supernode_per_atom_type,\n)\n\ndata = torch.load("./examples/data/
+is2re_bs3.pt") # 3 batched OC20 IS2RE data samples\nprint(\n "Data initially
+contains {} graphs, a total of {} atoms and {} edges".format(\n len
 (data.natoms), data.ptr[-1], len(data.cell_offsets)\n )\n)\nrewired_data =
 remove_tag0_nodes(deepcopy(data))\nprint(\n "Data without tag-0 nodes contains
 {} graphs, a total of {} atoms and {} edges".format(\n len
 (rewired_data.natoms), rewired_data.ptr[-1], len(rewired_data.cell_offsets)\n
 )\n)\nrewired_data = one_supernode_per_graph(deepcopy(data))\nprint(\n "Data
 with one super node per graph contains a total of {} atoms and {} edges".format
 (\n rewired_data.ptr[-1], len(rewired_data.cell_offsets)\n )\n)\nrewired_data =
```

### Comparing `phast-0.1.0/PKG-INFO` & `phast-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,65 +1,76 @@
 Metadata-Version: 2.1
 Name: phast
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: MIT
 Author: Victor Schmidt
 Author-email: vsch@pm.me
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: mendeleev (>=0.12.1,<0.13.0)
 Requires-Dist: pandas (>=1.4,<2.0)
-Requires-Dist: torch (>=1.10.0,<2.0.0)
+Requires-Dist: torch (>=1.11)
 Description-Content-Type: text/markdown
 
 <p align="center">
-<br/>
-<strong><a href="https://github.com/vict0rsch/phast" target="_blank">💻 Code</a></strong>
+<strong><a href="https://github.com/vict0rsch/phast" target="_blank">💻&nbsp;&nbsp;Code</a></strong>
 <strong>&nbsp;&nbsp;•&nbsp;&nbsp;</strong>
-<strong><a href="https://phast.readthedocs.io/" target="_blank">Docs 📑</a></strong>
-<br/>
+<strong><a href="https://phast.readthedocs.io/" target="_blank">Docs&nbsp;&nbsp;📑</a></strong>
 </p>
 
-# PhAST: Physics-Aware, Scalable, and Task-specific GNNs for Accelerated Catalyst Design
-
 <p align="center">
     <a>
-	    <img src='https://img.shields.io/badge/python-3.9%2B-blue' alt='Python' />
+	    <img src='https://img.shields.io/badge/python-3.8%2B-blue' alt='Python' />
 	</a>
 	<a href='https://phast.readthedocs.io/en/latest/?badge=latest'>
     	<img src='https://readthedocs.org/projects/phast/badge/?version=latest' alt='Documentation Status' />
 	</a>
     <a href="https://github.com/psf/black">
 	    <img src='https://img.shields.io/badge/code%20style-black-black' />
 	</a>
+<a href="https://pytorch.org">
+<img src="https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?logo=PyTorch&logoColor=white"/>
+</a>
 </p>
+<br/>
+
+# PhAST: Physics-Aware, Scalable, and Task-specific GNNs for Accelerated Catalyst Design
 
-## About
 
 This repository contains implementations for 2 of the PhAST components presented in the [paper](https://arxiv.org/abs/2211.12020):
 
 * `PhysEmbedding` that allows one to create an embedding vector from atomic numbers that is the concatenation of:
   * A learned embedding for the atom's group
   * A learned embedding for the atom's period
   * A fixed or learned embedding from a set of known physical properties, as reported by [`mendeleev`](https://mendeleev.readthedocs.io/en/stable/data.html#elements)
   * In the case of the OC20 dataset, a learned embedding for the atom's tag (adsorbate, catalyst surface or catalyst sub-surface)
 * Tag-based **graph rewiring** strategies for the OC20 dataset:
   * `remove_tag0_nodes` deletes all nodes in the graph associated with a tag 0 and recomputes edges
   * `one_supernode_per_graph` replaces all tag 0 atoms with a single new atom
-  * `one_supernode_per_atom_typs` replaces all tag 0 atoms *of a given element* with its own super node
+  * `one_supernode_per_atom_type` replaces all tag 0 atoms *of a given element* with its own super node
 
     <img src="https://raw.githubusercontent.com/vict0rsch/phast/main/examples/data/rewiring.png" width="600px" />
 
 Also: https://github.com/vict0rsch/faenet
 
+## Installation
+
+```
+pip install phast
+```
+
+⚠️ The above installation does not include `torch_geometric` which is a complex and very variable dependency you have to install yourself if you want to use the graph re-wiring functions of `phast`.
+
+☮️ Ignore `torch_geometric` if you only care about the `PhysEmbeddings`.
+
 ## Getting started
 
 ### Physical embeddings
 
 ![Embedding illustration](https://raw.githubusercontent.com/vict0rsch/phast/main/examples/data/embedding.png)
 
 ```python
@@ -79,14 +90,18 @@
 tags = torch.randint(0, 3, (3, 12))
 phys_embedding = PhysEmbedding(
     tag_emb_size=32, # default is 0, this is OC20-specific
     final_proj_size=64, # default is 0, no projection, just the concat. of embeds.
 )
 
 h = phys_embedding(z, tags) # h.shape = (3, 12, 64)
+
+# Assuming torch_geometric is installed:
+data = torch.load("examples/data/is2re_bs3.pt")
+h = phys_embedding(data.atomic_numbers.long(), data.tags) # h.shape = (261, 64)
 ```
 
 ### Graph rewiring
 
 ![Rewiring illustration](https://raw.githubusercontent.com/vict0rsch/phast/main/examples/data/rewiring.png)
 
 ```python
@@ -94,15 +109,15 @@
 import torch
 from phast.graph_rewiring import (
     remove_tag0_nodes,
     one_supernode_per_graph,
     one_supernode_per_atom_type,
 )
 
-data = torch.load("./examples/data/is2re_bs3.pt")  # 3 OC20 IS2RE data samples
+data = torch.load("./examples/data/is2re_bs3.pt")  # 3 batched OC20 IS2RE data samples
 print(
     "Data initially contains {} graphs, a total of {} atoms and {} edges".format(
         len(data.natoms), data.ptr[-1], len(data.cell_offsets)
     )
 )
 rewired_data = remove_tag0_nodes(deepcopy(data))
 print(
```

#### html2text {}

```diff
@@ -1,67 +1,75 @@
-Metadata-Version: 2.1 Name: phast Version: 0.1.0 Summary: License: MIT Author:
+Metadata-Version: 2.1 Name: phast Version: 0.1.1 Summary: License: MIT Author:
 Victor Schmidt Author-email: vsch@pm.me Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: mendeleev (>=0.12.1,<0.13.0)
-Requires-Dist: pandas (>=1.4,<2.0) Requires-Dist: torch (>=1.10.0,<2.0.0)
-Description-Content-Type: text/markdown
+Requires-Dist: pandas (>=1.4,<2.0) Requires-Dist: torch (>=1.11) Description-
+Content-Type: text/markdown
+                         ð»  Code   â¢   Docs  ð
+  [Python] [Documentation_Status] [https://img.shields.io/badge/code%20style-
+              black-black] [https://img.shields.io/badge/PyTorch-
+                  %23EE4C2C.svg?logo=PyTorch&logoColor=white]
 
-                         ð»_Code   â¢   Docs_ð
 # PhAST: Physics-Aware, Scalable, and Task-specific GNNs for Accelerated
-Catalyst Design
-  [Python] [Documentation_Status] [https://img.shields.io/badge/code%20style-
-                                 black-black]
-## About This repository contains implementations for 2 of the PhAST components
-presented in the [paper](https://arxiv.org/abs/2211.12020): * `PhysEmbedding`
-that allows one to create an embedding vector from atomic numbers that is the
-concatenation of: * A learned embedding for the atom's group * A learned
-embedding for the atom's period * A fixed or learned embedding from a set of
-known physical properties, as reported by [`mendeleev`](https://
-mendeleev.readthedocs.io/en/stable/data.html#elements) * In the case of the
-OC20 dataset, a learned embedding for the atom's tag (adsorbate, catalyst
-surface or catalyst sub-surface) * Tag-based **graph rewiring** strategies for
-the OC20 dataset: * `remove_tag0_nodes` deletes all nodes in the graph
-associated with a tag 0 and recomputes edges * `one_supernode_per_graph`
-replaces all tag 0 atoms with a single new atom * `one_supernode_per_atom_typs`
+Catalyst Design This repository contains implementations for 2 of the PhAST
+components presented in the [paper](https://arxiv.org/abs/2211.12020): *
+`PhysEmbedding` that allows one to create an embedding vector from atomic
+numbers that is the concatenation of: * A learned embedding for the atom's
+group * A learned embedding for the atom's period * A fixed or learned
+embedding from a set of known physical properties, as reported by [`mendeleev`]
+(https://mendeleev.readthedocs.io/en/stable/data.html#elements) * In the case
+of the OC20 dataset, a learned embedding for the atom's tag (adsorbate,
+catalyst surface or catalyst sub-surface) * Tag-based **graph rewiring**
+strategies for the OC20 dataset: * `remove_tag0_nodes` deletes all nodes in the
+graph associated with a tag 0 and recomputes edges * `one_supernode_per_graph`
+replaces all tag 0 atoms with a single new atom * `one_supernode_per_atom_type`
 replaces all tag 0 atoms *of a given element* with its own super node [https://
 raw.githubusercontent.com/vict0rsch/phast/main/examples/data/rewiring.png]
-Also: https://github.com/vict0rsch/faenet ## Getting started ### Physical
-embeddings ![Embedding illustration](https://raw.githubusercontent.com/
-vict0rsch/phast/main/examples/data/embedding.png) ```python import torch from
-phast.embedding import PhysEmbedding z = torch.randint(1, 85, (3, 12)) # batch
-of 3 graphs with 12 atoms each phys_embedding = PhysEmbedding( z_emb_size=32, #
-default period_emb_size=32, # default group_emb_size=32, # default
-properties_proj_size=32, # default is 0 -> no learned projection n_elements=85,
-# default ) h = phys_embedding(z) # h.shape = (3, 12, 128) tags = torch.randint
-(0, 3, (3, 12)) phys_embedding = PhysEmbedding( tag_emb_size=32, # default is
-0, this is OC20-specific final_proj_size=64, # default is 0, no projection,
-just the concat. of embeds. ) h = phys_embedding(z, tags) # h.shape = (3, 12,
-64) ``` ### Graph rewiring ![Rewiring illustration](https://
+Also: https://github.com/vict0rsch/faenet ## Installation ``` pip install phast
+``` â ï¸ The above installation does not include `torch_geometric` which is a
+complex and very variable dependency you have to install yourself if you want
+to use the graph re-wiring functions of `phast`. â®ï¸ Ignore
+`torch_geometric` if you only care about the `PhysEmbeddings`. ## Getting
+started ### Physical embeddings ![Embedding illustration](https://
+raw.githubusercontent.com/vict0rsch/phast/main/examples/data/embedding.png)
+```python import torch from phast.embedding import PhysEmbedding z =
+torch.randint(1, 85, (3, 12)) # batch of 3 graphs with 12 atoms each
+phys_embedding = PhysEmbedding( z_emb_size=32, # default period_emb_size=32, #
+default group_emb_size=32, # default properties_proj_size=32, # default is 0 -
+> no learned projection n_elements=85, # default ) h = phys_embedding(z) #
+h.shape = (3, 12, 128) tags = torch.randint(0, 3, (3, 12)) phys_embedding =
+PhysEmbedding( tag_emb_size=32, # default is 0, this is OC20-specific
+final_proj_size=64, # default is 0, no projection, just the concat. of embeds.
+) h = phys_embedding(z, tags) # h.shape = (3, 12, 64) # Assuming
+torch_geometric is installed: data = torch.load("examples/data/is2re_bs3.pt") h
+= phys_embedding(data.atomic_numbers.long(), data.tags) # h.shape = (261, 64)
+``` ### Graph rewiring ![Rewiring illustration](https://
 raw.githubusercontent.com/vict0rsch/phast/main/examples/data/rewiring.png)
 ```python from copy import deepcopy import torch from phast.graph_rewiring
 import ( remove_tag0_nodes, one_supernode_per_graph,
 one_supernode_per_atom_type, ) data = torch.load("./examples/data/
-is2re_bs3.pt") # 3 OC20 IS2RE data samples print( "Data initially contains {}
-graphs, a total of {} atoms and {} edges".format( len(data.natoms), data.ptr[-
-1], len(data.cell_offsets) ) ) rewired_data = remove_tag0_nodes(deepcopy(data))
-print( "Data without tag-0 nodes contains {} graphs, a total of {} atoms and {}
-edges".format( len(rewired_data.natoms), rewired_data.ptr[-1], len
-(rewired_data.cell_offsets) ) ) rewired_data = one_supernode_per_graph(deepcopy
-(data)) print( "Data with one super node per graph contains a total of {} atoms
-and {} edges".format( rewired_data.ptr[-1], len(rewired_data.cell_offsets) ) )
-rewired_data = one_supernode_per_atom_type(deepcopy(data)) print( "Data with
-one super node per atom type contains a total of {} atoms and {} edges".format
-( rewired_data.ptr[-1], len(rewired_data.cell_offsets) ) ) ``` ``` Data
-initially contains 3 graphs, a total of 261 atoms and 11596 edges Data without
-tag-0 nodes contains 3 graphs, a total of 64 atoms and 1236 edges Data with one
-super node per graph contains a total of 67 atoms and 1311 edges Data with one
-super node per atom type contains a total of 71 atoms and 1421 edges ``` ##
-Tests This requires [`poetry`](https://python-poetry.org/docs/). Make sure to
-have `torch` and `torch_geometric` installed in your environment before you can
-run the tests. Unfortunately because of CUDA/torch compatibilities, neither
-`torch` nor `torch_geometric` are part of the explicit dependencies and must be
-installed independently. ```bash git clone git@github.com:vict0rsch/phast.git
-poetry install --with dev pytest --cov=phast --cov-report term-missing ```
-Testing on Macs you may encounter a [Library Not Loaded Error](https://
-github.com/pyg-team/pytorch_geometric/issues/6530)
+is2re_bs3.pt") # 3 batched OC20 IS2RE data samples print( "Data initially
+contains {} graphs, a total of {} atoms and {} edges".format( len(data.natoms),
+data.ptr[-1], len(data.cell_offsets) ) ) rewired_data = remove_tag0_nodes
+(deepcopy(data)) print( "Data without tag-0 nodes contains {} graphs, a total
+of {} atoms and {} edges".format( len(rewired_data.natoms), rewired_data.ptr[-
+1], len(rewired_data.cell_offsets) ) ) rewired_data = one_supernode_per_graph
+(deepcopy(data)) print( "Data with one super node per graph contains a total of
+{} atoms and {} edges".format( rewired_data.ptr[-1], len
+(rewired_data.cell_offsets) ) ) rewired_data = one_supernode_per_atom_type
+(deepcopy(data)) print( "Data with one super node per atom type contains a
+total of {} atoms and {} edges".format( rewired_data.ptr[-1], len
+(rewired_data.cell_offsets) ) ) ``` ``` Data initially contains 3 graphs, a
+total of 261 atoms and 11596 edges Data without tag-0 nodes contains 3 graphs,
+a total of 64 atoms and 1236 edges Data with one super node per graph contains
+a total of 67 atoms and 1311 edges Data with one super node per atom type
+contains a total of 71 atoms and 1421 edges ``` ## Tests This requires
+[`poetry`](https://python-poetry.org/docs/). Make sure to have `torch` and
+`torch_geometric` installed in your environment before you can run the tests.
+Unfortunately because of CUDA/torch compatibilities, neither `torch` nor
+`torch_geometric` are part of the explicit dependencies and must be installed
+independently. ```bash git clone git@github.com:vict0rsch/phast.git poetry
+install --with dev pytest --cov=phast --cov-report term-missing ``` Testing on
+Macs you may encounter a [Library Not Loaded Error](https://github.com/pyg-
+team/pytorch_geometric/issues/6530)
```

