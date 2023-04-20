# Comparing `tmp/pytreeclass-0.2.8.tar.gz` & `tmp/pytreeclass-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytreeclass-0.2.8.tar", last modified: Sun Apr 16 20:46:40 2023, max compression
+gzip compressed data, was "pytreeclass-0.3.0.tar", last modified: Wed Apr 19 23:59:42 2023, max compression
```

## Comparing `pytreeclass-0.2.8.tar` & `pytreeclass-0.3.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:46:40.528353 pytreeclass-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29188 2023-04-16 20:46:40.524353 pytreeclass-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28312 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:46:40.524353 pytreeclass-0.2.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:46:40.524353 pytreeclass-0.2.8/pytreeclass/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/pytreeclass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:46:40.524353 pytreeclass-0.2.8/pytreeclass/_src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/pytreeclass/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18680 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/pytreeclass/_src/tree_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/pytreeclass/_src/tree_freeze.py
--rw-r--r--   0 runner    (1001) docker     (123)    19421 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/pytreeclass/_src/tree_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    31487 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/pytreeclass/_src/tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/pytreeclass/_src/tree_trace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:46:40.524353 pytreeclass-0.2.8/pytreeclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29188 2023-04-16 20:46:40.000000 pytreeclass-0.2.8/pytreeclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-16 20:46:40.000000 pytreeclass-0.2.8/pytreeclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 20:46:40.000000 pytreeclass-0.2.8/pytreeclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 20:46:40.000000 pytreeclass-0.2.8/pytreeclass.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-16 20:46:40.000000 pytreeclass-0.2.8/pytreeclass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-16 20:46:40.000000 pytreeclass-0.2.8/pytreeclass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 20:46:40.528353 pytreeclass-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:46:40.524353 pytreeclass-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18439 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/tests/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/tests/test_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10220 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/tests/test_tree_freeze.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/tests/test_tree_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/tests/test_tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/tests/test_tree_viz_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    17379 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/tests/test_treeclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/tests/test_under_jit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:59:42.322212 pytreeclass-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29135 2023-04-19 23:59:42.322212 pytreeclass-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28259 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:59:42.318212 pytreeclass-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:59:42.318212 pytreeclass-0.3.0/pytreeclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/pytreeclass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:59:42.322212 pytreeclass-0.3.0/pytreeclass/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/pytreeclass/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16425 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/pytreeclass/_src/tree_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/pytreeclass/_src/tree_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19019 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/pytreeclass/_src/tree_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31417 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/pytreeclass/_src/tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11678 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/pytreeclass/_src/tree_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:59:42.318212 pytreeclass-0.3.0/pytreeclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29135 2023-04-19 23:59:42.000000 pytreeclass-0.3.0/pytreeclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-19 23:59:42.000000 pytreeclass-0.3.0/pytreeclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:59:42.000000 pytreeclass-0.3.0/pytreeclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:59:42.000000 pytreeclass-0.3.0/pytreeclass.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-19 23:59:42.000000 pytreeclass-0.3.0/pytreeclass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-19 23:59:42.000000 pytreeclass-0.3.0/pytreeclass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 23:59:42.322212 pytreeclass-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:59:42.322212 pytreeclass-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17268 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/tests/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/tests/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/tests/test_tree_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/tests/test_tree_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17626 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/tests/test_tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/tests/test_tree_viz_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14936 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/tests/test_treeclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/tests/test_under_jit.py
```

### Comparing `pytreeclass-0.2.8/LICENSE` & `pytreeclass-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.2.8/PKG-INFO` & `pytreeclass-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytreeclass
-Version: 0.2.8
+Version: 0.3.0
 Summary: JAX compatible dataclass.
 Home-page: https://github.com/ASEM000/pytreeclass
 Author: Mahmoud Asem
 Author-email: asem00@kaist.ac.kr
 License: Apache-2.0
 Keywords: python machine-learning pytorch jax
 Classifier: Development Status :: 5 - Production/Stable
@@ -60,15 +60,15 @@
 
 ```python
 pip install git+https://github.com/ASEM000/PyTreeClass
 ```
 
 ## 📖 Description<a id="description"></a>
 
-`PyTreeClass` is a JAX-compatible `dataclass`-like decorator to create and operate on stateful JAX PyTrees.
+`PyTreeClass` is a JAX-compatible class builder to create and operate on stateful JAX PyTrees.
 
 The package aims to achieve _two goals_:
 
 1. 🔒 To maintain safe and correct behaviour by using _immutable_ modules with _functional_ API.
 2. To achieve the **most intuitive** user experience in the `JAX` ecosystem by :
    - 🏗️ Defining layers similar to `PyTorch` or `TensorFlow` subclassing style.
    - ☝️ Filtering\Indexing layer values similar to `jax.numpy.at[].{get,set,apply,...}`
@@ -85,16 +85,15 @@
 <td>
 
 ```python
 import jax
 import jax.numpy as jnp
 import pytreeclass as pytc
 
-@pytc.treeclass
-class Tree:
+class Tree(pytc.TreeClass):
     a:int = 1
     b:tuple[float] = (2.,3.)
     c:jax.Array = jnp.array([4.,5.,6.])
 
     def __call__(self, x):
         return self.a + self.b[0] + self.c + x
 
@@ -299,16 +298,15 @@
 ```python
 
 import pytreeclass as pytc
 import jax
 import jax.numpy as jnp
 
 
-@pytc.treeclass
-class Tree:
+class Tree(pytc.TreeClass)
     a: int = 1
     b: tuple[float] = (2., 3.)
     c: jax.Array = jnp.array([4., 5., 6.])
 
     def __call__(self, x):
         return self.a + self.b[0] + self.c + x
 
@@ -424,24 +422,23 @@
 
 <details>
 
 <summary>
 
 ## 📜 Stateful computations<a id="stateful_computation"></a> </summary>
 
-First, [Under jax.jit jax requires states to be explicit](https://jax.readthedocs.io/en/latest/jax-101/07-state.html?highlight=state), this means that for any class instance; variables needs to be separated from the class and be passed explictly. However when using @pytc.treeclass no need to separate the instance variables ; instead the whole instance is passed as a state.
+First, [Under jax.jit jax requires states to be explicit](https://jax.readthedocs.io/en/latest/jax-101/07-state.html?highlight=state), this means that for any class instance; variables needs to be separated from the class and be passed explictly. However when using `TreeClass` no need to separate the instance variables ; instead the whole instance is passed as a state.
 
 Using the following pattern,Updating state **functionally** can be achieved under `jax.jit`
 
 ```python
 import jax
 import pytreeclass as pytc
 
-@pytc.treeclass
-class Counter:
+class Counter(pytc.TreeClass):
     calls : int = 0
 
     def increment(self):
         self.calls += 1
 counter = Counter() # Counter(calls=0)
 ```
 
@@ -544,16 +541,15 @@
     if not isinstance(value, int):
         raise TypeError("Value must be an integer")
     if value <= 0:
         raise ValueError("Value must be positive")
     return value
 
 
-@pytc.treeclass
-class Tree:
+class Tree(pytc.TreeClass):
     in_features:int = pytc.field(callbacks=[positive_int_callback])
 
 
 tree = Tree(1)
 # no error
 
 tree = Tree(0)
@@ -573,16 +569,15 @@
 import functools as ft
 import pytreeclass as pytc
 import jax
 import jax.tree_util as jtu
 import jax.numpy as jnp
 
 
-@ft.partial(pytc.treeclass, leafwise=True)
-class Tree:
+class Tree(pytc.TreeClass, leafwise=True):
     a: int = 1
     b: tuple[float] = (2., 3.)
     c: jax.Array = jnp.array([4., 5., 6.])
 
     def __call__(self, x):
         return self.a + self.b[0] + self.c + x
 
@@ -632,16 +627,15 @@
 TDLR
 
 ```python
 import functools as ft
 import pytreeclass as pytc
 import jax.numpy as jnp
 
-@ft.partial(pytc.treeclass, leafwise=True)
-class Tree:
+class Tree(pytc.TreeClass, leafwise=True):
     a:int = 1
     b:tuple[float] = (2.,3.)
     c:jax.Array = jnp.array([4.,5.,6.])
 
 tree = Tree()
 
 print(pytc.bcmap(jnp.where)(tree>2, tree+100, 0))
@@ -718,16 +712,16 @@
 #  Array(1000, dtype=int32, weak_type=True))
 ```
 
 lets then take this a step further to eliminate `mask` from the equation
 by using `pytreeclass` with `leafwise=True `
 
 ```python
-@ft.partial(pytc.treeclass, leafwise=True)
-class Tree:
+
+class Tree(pytc.TreeClass, leafwise=True):
     tree : tuple = ([1], {"a":1, "b":2}, (1,), -1,)
 
 tree = Tree()
 # Tree(tree=([1], {a:1, b:2}, (1), -1))
 ```
 
 case 1: broadcast scalar to tree
@@ -912,16 +906,15 @@
 For demonstration , the following figure contains the 4 variants of the same `Tree` instance define
 
 ```python
 import jax
 import jax.numpy as jnp
 import pytreeclass as pytc
 
-@pytc.treeclass
-class Tree:
+class Tree(pytc.TreeClass):
     a:int = 1
     b:tuple[float] = (2.,3.)
     c:jax.Array = jnp.array([4.,5.,6.])
 ```
 
 ![image](assets/tree_figures.png)
```

### Comparing `pytreeclass-0.2.8/README.md` & `pytreeclass-0.3.0/pytreeclass.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: pytreeclass
+Version: 0.3.0
+Summary: JAX compatible dataclass.
+Home-page: https://github.com/ASEM000/pytreeclass
+Author: Mahmoud Asem
+Author-email: asem00@kaist.ac.kr
+License: Apache-2.0
+Keywords: python machine-learning pytorch jax
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <!-- <h1 align="center" style="font-family:Monospace" >Py🌲Class</h1> -->
 <h5 align="center">
 <img width="250px" src="https://user-images.githubusercontent.com/48389287/227880173-bf78c02c-d28b-4cf4-95e6-fa49b82a43a1.svg"> <br>
 
 <br>
 
 [**Installation**](#installation)
@@ -37,15 +60,15 @@
 
 ```python
 pip install git+https://github.com/ASEM000/PyTreeClass
 ```
 
 ## 📖 Description<a id="description"></a>
 
-`PyTreeClass` is a JAX-compatible `dataclass`-like decorator to create and operate on stateful JAX PyTrees.
+`PyTreeClass` is a JAX-compatible class builder to create and operate on stateful JAX PyTrees.
 
 The package aims to achieve _two goals_:
 
 1. 🔒 To maintain safe and correct behaviour by using _immutable_ modules with _functional_ API.
 2. To achieve the **most intuitive** user experience in the `JAX` ecosystem by :
    - 🏗️ Defining layers similar to `PyTorch` or `TensorFlow` subclassing style.
    - ☝️ Filtering\Indexing layer values similar to `jax.numpy.at[].{get,set,apply,...}`
@@ -62,16 +85,15 @@
 <td>
 
 ```python
 import jax
 import jax.numpy as jnp
 import pytreeclass as pytc
 
-@pytc.treeclass
-class Tree:
+class Tree(pytc.TreeClass):
     a:int = 1
     b:tuple[float] = (2.,3.)
     c:jax.Array = jnp.array([4.,5.,6.])
 
     def __call__(self, x):
         return self.a + self.b[0] + self.c + x
 
@@ -276,16 +298,15 @@
 ```python
 
 import pytreeclass as pytc
 import jax
 import jax.numpy as jnp
 
 
-@pytc.treeclass
-class Tree:
+class Tree(pytc.TreeClass)
     a: int = 1
     b: tuple[float] = (2., 3.)
     c: jax.Array = jnp.array([4., 5., 6.])
 
     def __call__(self, x):
         return self.a + self.b[0] + self.c + x
 
@@ -401,24 +422,23 @@
 
 <details>
 
 <summary>
 
 ## 📜 Stateful computations<a id="stateful_computation"></a> </summary>
 
-First, [Under jax.jit jax requires states to be explicit](https://jax.readthedocs.io/en/latest/jax-101/07-state.html?highlight=state), this means that for any class instance; variables needs to be separated from the class and be passed explictly. However when using @pytc.treeclass no need to separate the instance variables ; instead the whole instance is passed as a state.
+First, [Under jax.jit jax requires states to be explicit](https://jax.readthedocs.io/en/latest/jax-101/07-state.html?highlight=state), this means that for any class instance; variables needs to be separated from the class and be passed explictly. However when using `TreeClass` no need to separate the instance variables ; instead the whole instance is passed as a state.
 
 Using the following pattern,Updating state **functionally** can be achieved under `jax.jit`
 
 ```python
 import jax
 import pytreeclass as pytc
 
-@pytc.treeclass
-class Counter:
+class Counter(pytc.TreeClass):
     calls : int = 0
 
     def increment(self):
         self.calls += 1
 counter = Counter() # Counter(calls=0)
 ```
 
@@ -521,16 +541,15 @@
     if not isinstance(value, int):
         raise TypeError("Value must be an integer")
     if value <= 0:
         raise ValueError("Value must be positive")
     return value
 
 
-@pytc.treeclass
-class Tree:
+class Tree(pytc.TreeClass):
     in_features:int = pytc.field(callbacks=[positive_int_callback])
 
 
 tree = Tree(1)
 # no error
 
 tree = Tree(0)
@@ -550,16 +569,15 @@
 import functools as ft
 import pytreeclass as pytc
 import jax
 import jax.tree_util as jtu
 import jax.numpy as jnp
 
 
-@ft.partial(pytc.treeclass, leafwise=True)
-class Tree:
+class Tree(pytc.TreeClass, leafwise=True):
     a: int = 1
     b: tuple[float] = (2., 3.)
     c: jax.Array = jnp.array([4., 5., 6.])
 
     def __call__(self, x):
         return self.a + self.b[0] + self.c + x
 
@@ -609,16 +627,15 @@
 TDLR
 
 ```python
 import functools as ft
 import pytreeclass as pytc
 import jax.numpy as jnp
 
-@ft.partial(pytc.treeclass, leafwise=True)
-class Tree:
+class Tree(pytc.TreeClass, leafwise=True):
     a:int = 1
     b:tuple[float] = (2.,3.)
     c:jax.Array = jnp.array([4.,5.,6.])
 
 tree = Tree()
 
 print(pytc.bcmap(jnp.where)(tree>2, tree+100, 0))
@@ -695,16 +712,16 @@
 #  Array(1000, dtype=int32, weak_type=True))
 ```
 
 lets then take this a step further to eliminate `mask` from the equation
 by using `pytreeclass` with `leafwise=True `
 
 ```python
-@ft.partial(pytc.treeclass, leafwise=True)
-class Tree:
+
+class Tree(pytc.TreeClass, leafwise=True):
     tree : tuple = ([1], {"a":1, "b":2}, (1,), -1,)
 
 tree = Tree()
 # Tree(tree=([1], {a:1, b:2}, (1), -1))
 ```
 
 case 1: broadcast scalar to tree
@@ -889,16 +906,15 @@
 For demonstration , the following figure contains the 4 variants of the same `Tree` instance define
 
 ```python
 import jax
 import jax.numpy as jnp
 import pytreeclass as pytc
 
-@pytc.treeclass
-class Tree:
+class Tree(pytc.TreeClass):
     a:int = 1
     b:tuple[float] = (2.,3.)
     c:jax.Array = jnp.array([4.,5.,6.])
 ```
 
 ![image](assets/tree_figures.png)
```

### Comparing `pytreeclass-0.2.8/docs/conf.py` & `pytreeclass-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.2.8/pytreeclass/__init__.py` & `pytreeclass-0.3.0/pytreeclass/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pytreeclass._src.tree_decorator import field, fields, is_treeclass, treeclass
+from pytreeclass._src.tree_decorator import TreeClass, field
 from pytreeclass._src.tree_freeze import freeze, is_frozen, is_nondiff, unfreeze
 from pytreeclass._src.tree_indexer import bcmap, is_tree_equal, tree_indexer
 from pytreeclass._src.tree_pprint import (
     tree_diagram,
     tree_indent,
     tree_mermaid,
     tree_repr,
@@ -15,19 +15,17 @@
     tree_flatten_with_trace,
     tree_leaves_with_trace,
     tree_map_with_trace,
 )
 
 __all__ = (
     # general utils
-    "treeclass",
-    "is_treeclass",
+    "TreeClass",
     "is_tree_equal",
     "field",
-    "fields",
     # pprint utils
     "tree_diagram",
     "tree_mermaid",
     "tree_repr",
     "tree_str",
     "tree_indent",
     "tree_summary",
@@ -43,8 +41,8 @@
     "register_pytree_node_trace",
     "tree_map_with_trace",
     "tree_leaves_with_trace",
     "tree_flatten_with_trace",
     "tree_repr_with_trace",
 )
 
-__version__ = "0.2.8"
+__version__ = "0.3.0"
```

### Comparing `pytreeclass-0.2.8/pytreeclass/_src/tree_decorator.py` & `pytreeclass-0.3.0/pytreeclass/_src/tree_decorator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,48 @@
 from __future__ import annotations
 
 import functools as ft
 import sys
+from abc import ABCMeta
 from collections.abc import MutableMapping, MutableSequence
-from contextlib import suppress
 from types import FunctionType, MappingProxyType
 from typing import Any, Callable, NamedTuple, Sequence, TypeVar
 
-import jax.tree_util as jtu
+from jax.tree_util import register_pytree_node
 from typing_extensions import dataclass_transform
 
 from pytreeclass._src.tree_freeze import tree_hash
 from pytreeclass._src.tree_indexer import (
-    _conditional_mutable_method,
     _leafwise_transform,
     _mutable_context,
+    _mutable_instance_registry,
     is_tree_equal,
     tree_copy,
     tree_indexer,
 )
 from pytreeclass._src.tree_pprint import tree_repr, tree_str
 from pytreeclass._src.tree_trace import register_pytree_node_trace
 
 
 class NOT_SET:
     __repr__ = lambda _: "?"
 
 
-PyTree = Any
 T = TypeVar("T")
+PyTree = Any
+
 _NOT_SET = NOT_SET()
-_FIELDS = "__fields__"
+_FIELDS = "_fields"
 _POST_INIT = "__post_init__"
 _MUTABLE_TYPES = (MutableSequence, MutableMapping, set)
 
 
 """Define a class decorator that is compatible with JAX's transformation."""
 
 
-def is_treeclass(node: Any) -> bool:
-    """Check if a node is a `treeclass`."""
-    return (node if isinstance(node, type) else type(node)).__setattr__ is _setattr
-
-
 class Field(NamedTuple):
     name: str | None = None
     type: type | None = None
     default: Any = _NOT_SET
     factory: Any = None
     init: bool = True
     repr: bool = True
@@ -55,28 +51,24 @@
     metadata: MappingProxyType[str, Any] | None = None
     callbacks: Sequence[Any] = ()
     alias: str | None = None
 
     def __eq__(self, other: Any) -> bool:
         return hash(self) == hash(other)
 
-    def __repr__(self) -> str:
-        return tree_repr(self)
-
     def __hash__(self) -> int:
-        parameters = (
+        return tree_hash(
             self.name,
             self.default,
             self.factory,
             self.init,
             self.kw_only,
             self.pos_only,
             self.alias,
         )
-        return tree_hash(parameters)
 
 
 def field(
     *,
     default: Any = _NOT_SET,
     factory: Callable | None = None,
     init: bool = True,
@@ -108,16 +100,15 @@
         ...    return wrapper
 
 
         >>> def positive_check_callback(x):
         ...    assert x > 0
         ...    return x
 
-        >>> @pytc.treeclass
-        ... class Employee:
+        >>> class Employee(pytc.TreeClass):
         ...    # assert employee `name` is str
         ...    name: str = pytc.field(callbacks=[instance_cb_factory(str)])
         ...    # use callback compostion to assert employee `age` is int and positive
         ...    age: int = pytc.field(callbacks=[instance_cb_factory(int), positive_check_callback])
         ...    # use `id` in the constructor for `_id` attribute
         ...    # this is useful for private attributes that are not supposed to be accessed directly
         ...    # and hide it from the repr, also add extra info for this field
@@ -169,47 +160,36 @@
         pos_only=pos_only,
         metadata=metadata,  # type: ignore
         callbacks=callbacks,
         alias=alias,
     )
 
 
-def fields(item: Any) -> Sequence[Field]:
-    """Get the fields of a `treeclass` instance."""
-    if not hasattr(item, _FIELDS):
-        raise TypeError(f"Cannot get fields of {item!r}.")
-
-    return tuple(vars(item)[_FIELDS].values())
-
-
 @ft.lru_cache
 def _generate_field_map(klass: type) -> dict[str, Field]:
     field_map = dict()
 
     if klass is object:
         return field_map
 
     for base in reversed(klass.__mro__[1:]):
-        # get the fields of the base class in the MRO in reverse order to ensure
-        # the correct order of the fields are preserved
         field_map.update(_generate_field_map(base))
 
     # TODO: use inspect to get annotations, once we are on minimum python version >3.9
     if "__annotations__" not in vars(klass):
         return field_map
 
     for name in (annotation_map := vars(klass)["__annotations__"]):
         value = vars(klass).get(name, _NOT_SET)
         type = annotation_map[name]
 
         if name == "self":
             # while `dataclasses` allows `self` as a field name, its confusing
             # and not recommended. so raise an error
-            msg = "Field name cannot be `self`."
-            raise ValueError(msg)
+            raise ValueError("Field name cannot be `self`.")
 
         if isinstance(value, Field):
             # case: `x: Any = field(default=1)`
             if isinstance(value.default, _MUTABLE_TYPES):
                 # example case: `x: Any = field(default=[1, 2, 3])`
                 msg = f"Mutable default value of field `{name}` is not allowed, use "
                 msg += f"`factory=lambda: {value.default}` instead."
@@ -240,192 +220,122 @@
 def _generate_init_code(fields: Sequence[Field]) -> str:
     head = body = ""
 
     for field in fields:
         name = field.name  # name in body
         alias = field.alias or name  # name in constructor
 
-        mark0 = f"field_map['{name}'].default"
-        mark1 = f"field_map['{name}'].factory()"
-        mark2 = f"self.{name}"
-
         if field.kw_only and "*" not in head and field.init:
             head += "*, "
 
         if field.default is not _NOT_SET:
-            # in head: def f(.. x= default_value)
-            head += f"{alias}={mark0}, " if field.init else ""
-            # in body:  self.x = default_value
-            body += f"\t\t{mark2}=" + (f"{alias}\n " if field.init else f"{mark0}\n")
+            vref = f"field_map['{name}'].default"
+            head += f"{alias}={vref}, " if field.init else ""
+            body += f"\t\tself.{name}=" + (f"{alias}\n " if field.init else f"{vref}\n")
         elif field.factory is not None:
-            head += f"{alias}={mark1}, " if field.init else ""
-            body += f"\t\t{mark2}=" + (f"{alias}\n" if field.init else f"{mark1}\n")
+            vref = f"field_map['{name}'].factory()"
+            head += f"{alias}={vref}, " if field.init else ""
+            body += f"\t\tself.{name}=" + (f"{alias}\n" if field.init else f"{vref}\n")
         else:
-            # no defaults are added
             head += f"{alias}, " if field.init else ""
-            body += f"\t\t{mark2}={alias}\n " if field.init else ""
+            body += f"\t\tself.{name}={alias}\n " if field.init else ""
 
         if field.pos_only and field.init:
-            if "/" in head:
-                head = head.replace("/,", "")
+            head = head.replace("/,", "") + "/, "
 
-            head += "/, "
-
-    # add pass to avoid syntax error if all fields are ignored
-    body += "\t\tpass"
+    body += "\t\tpass"  # add pass to avoid syntax error if all fields are ignored
     body = "\tdef __init__(self, " + head[:-2] + "):\n" + body
     body = f"def closure(field_map):\n{body}\n\treturn __init__"
     return body.expandtabs(4)
 
 
-def _generate_init(klass: type) -> FunctionType:
+def _generate_init_method(klass: type) -> FunctionType:
     field_map = _generate_field_map(klass)
-    local_namespace = dict()  # type: ignore
-    global_namespace = vars(sys.modules[klass.__module__])
     init_code = _generate_init_code(tuple(field_map.values()))
-    exec(init_code, global_namespace, local_namespace)
+    exec(init_code, vars(sys.modules[klass.__module__]), local_namespace := dict())
     method = local_namespace["closure"](field_map)
-
-    return FunctionType(
-        code=method.__code__,
-        globals=global_namespace,
-        name=method.__name__,
-        argdefs=method.__defaults__,
-        closure=method.__closure__,
-    )
+    method.__qualname__ = f"{klass.__qualname__}.__init__"
+    return method
 
 
-@_conditional_mutable_method
 def _setattr(tree: PyTree, key: str, value: Any) -> None:
-    if key in (field_map := vars(tree)[_FIELDS]):
+    if id(tree) not in _mutable_instance_registry:
+        msg = f"Cannot set attribute `{key}` = {value!r} on immutable instance of "
+        msg += f"`{type(tree).__name__}`.\nUse `.at[`{key}`].set({value!r})` instead."
+        raise AttributeError(msg)
+
+    if key in (field_map := vars(tree).get(_FIELDS, ())):
         for callback in field_map[key].callbacks:
             try:
                 # callback is a function that takes the value of the field
                 # and returns a modified value
                 value = callback(value)
             except Exception as e:
                 msg = f"Error for field=`{key}`:\n{e}"
                 raise type(e)(msg)
 
-    if is_treeclass(value):
+    elif isinstance(value, TreeClass):
         # auto registers the instance value if it is a registered `treeclass`
         # this behavior is similar to PyTorch behavior in `nn.Module`
         # with instances of `Parameter`/`Module`.
         # the behavior is useful to avoid repetitive code pattern in field definition and
         # and initialization inside init method.
         kv = {key: Field(type=type(value), init=False, name=key)}
-        vars(tree)[_FIELDS] = MappingProxyType({**vars(tree)[_FIELDS], **kv})
+        vars(tree)[_FIELDS] = MappingProxyType({**field_map, **kv})
 
     vars(tree)[key] = value  # type: ignore
 
 
-@_conditional_mutable_method
 def _delattr(tree, key: str) -> None:
     # delete the attribute under `_mutable_context` context
     # otherwise raise an error
-    del vars(tree)[key]
-
-
-def _init_wrapper(init_func: Callable) -> Callable:
-    @ft.wraps(init_func)
-    def wrapper(tree, *a, **k) -> None:
-        with _mutable_context(tree):
-            kvs = dict(_generate_field_map(type(tree)))
-            vars(tree)[_FIELDS] = MappingProxyType(kvs)
-            output = init_func(tree, *a, **k)
-
-            if post_init_func := getattr(type(tree), _POST_INIT, None):
-                # to simplify the logic, we call the post init method
-                # even if the init method is not code-generated.
-                post_init_func(tree)
-
-        # handle non-initialized fields
-        if len(keys := set(kvs) - set(vars(tree))) > 0:
-            msg = f"Uninitialized fields: ({', '.join(keys)}) "
-            msg += f"in class `{type(tree).__name__}`"
-            raise AttributeError(msg)
-        return output
+    if id(tree) not in _mutable_instance_registry:
+        msg = f"Cannot delete attribute `{key}` on immutable instance of "
+        msg += f"`{type(tree).__name__}`.\n"
+        raise AttributeError(msg)
 
-    return wrapper
+    del vars(tree)[key]
 
 
 def _tree_unflatten(klass: type, treedef: Any, leaves: list[Any]):
+    # unflatten rule for `treeclass` to use with `jax.tree_unflatten`
     tree = object.__new__(klass)
-    # update through vars, to avoid calling the `setattr` method
-    # that will check for callbacks.
     vars(tree).update(treedef[1])
     vars(tree).update(zip(treedef[0], leaves))
     return tree
 
 
 def _tree_flatten(tree: PyTree):
-    # Flatten rule for `treeclass` to use with `jax.tree_flatten`
+    # flatten rule for `treeclass` to use with `jax.tree_flatten`
     static, dynamic = dict(vars(tree)), dict()
-    for key in static[_FIELDS]:
+    for key in static.get(_FIELDS, ()):
         dynamic[key] = static.pop(key)
     return list(dynamic.values()), (tuple(dynamic.keys()), static)
 
 
 def _tree_trace(tree: PyTree) -> list[tuple[Any, Any, Any, Any]]:
     # Trace flatten rule to be used with the `tree_trace` module
     leaves, (keys, _) = _tree_flatten(tree)
     names = (f"{key}" for key in keys)
     types = map(type, leaves)
     indices = range(len(leaves))
     return [*zip(names, types, indices)]
 
 
-def _register_treeclass(klass: type[T]) -> type[T]:
-    with suppress(ValueError):
-        # `ValueError` is raised for duplicate registration.
-        # there are two cases where a class is registered more than once:
-        # first, when a class is decorated with `treeclass` more than once (e.g. `treeclass(treeclass(Class))`)
-        # second when a class is decorated with `treeclass` and has a parent class that is decorated with `treeclass`
-        # in that case `__init_subclass__` registers the class before the decorator registers it.
-        # register the trace flatten rule
-        register_pytree_node_trace(klass, _tree_trace)
-        # register the flatten/unflatten rules with jax
-        jtu.register_pytree_node(klass, _tree_flatten, ft.partial(_tree_unflatten, klass))  # type: ignore
-
-    return klass
-
-
-def _init_subclass_wrapper(init_subclass_method: Callable) -> Callable:
-    # Non-decorated subclasses uses the base `treeclass` leaves only
-    @classmethod  # type: ignore
-    @ft.wraps(init_subclass_method)
-    def wrapper(klass: type, *a, **k) -> None:
-        init_subclass_method(*a, **k)
-        _register_treeclass(klass)
-
-    return wrapper
-
-
 def _treeclass_transform(klass: type[T]) -> type[T]:
     for key, method in (("__setattr__", _setattr), ("__delattr__", _delattr)):
-        # basic required methods
         if key in vars(klass):
-            if vars(klass)[key] is method:
-                return klass  # already transformed
-            # the user defined a method that conflicts with the required method
-            msg = f"Unable to transform the class `{klass.__name__}` with {key} method defined."
+            # the user defined a method that conflicts with the reserved method
+            msg = f"Unable to transform the class `{klass.__name__}` "
+            msg += f"with resereved `{key}` method defined on the class."
             raise TypeError(msg)
         setattr(klass, key, method)
 
     if "__init__" not in vars(klass):
-        # generate the init method in case it is not defined by the user
-        setattr(klass, "__init__", _generate_init(klass))
-
-    for key, wrapper in (
-        ("__init__", _init_wrapper),
-        ("__init_subclass__", _init_subclass_wrapper),
-    ):
-        # wrappers to enable the field initialization, and registering
-        # the class with jax
-        setattr(klass, key, wrapper(getattr(klass, key)))
+        setattr(klass, "__init__", _generate_init_method(klass))
 
     # basic optional methods
     for key, method in (
         ("__repr__", tree_repr),
         ("__str__", tree_str),
         ("__copy__", tree_copy),
         ("__hash__", tree_hash),
@@ -436,48 +346,74 @@
             # keep the original method if it is defined by the user
             # this behavior similar is to `dataclasses.dataclass`
             setattr(klass, key, method)
 
     return klass
 
 
+def _register_treeclass(klass: type[T]) -> type[T]:
+    # handle all registration logic for `treeclass`
+    # TODO: register with jax path registry once jax version >= 0.4.7
+    register_pytree_node_trace(klass, _tree_trace)
+    register_pytree_node(klass, _tree_flatten, ft.partial(_tree_unflatten, klass))
+    return klass
+
+
+class TreeClassMeta(ABCMeta):
+    def __call__(klass: type[T], *a, **k) -> T:
+        self = klass.__new__(klass, *a, **k)
+
+        with _mutable_context(self):
+            vars(self)[_FIELDS] = MappingProxyType(_generate_field_map(klass))
+            klass.__init__(self, *a, **k)
+
+            if post_init_func := getattr(klass, _POST_INIT, None):
+                # to simplify the logic, we call the post init method
+                # even if the init method is not code-generated.
+                post_init_func(self)
+
+        # handle non-initialized fields
+        if len(keys := set(getattr(self, _FIELDS)) - set(vars(self))) > 0:
+            msg = f"Uninitialized fields: ({', '.join(keys)}) "
+            msg += f"in class `{type(self).__name__}`"
+            raise AttributeError(msg)
+        return self
+
+
 @dataclass_transform(field_specifiers=(field, Field), frozen_default=True)
-def treeclass(klass: type[T], *, leafwise: bool = False) -> type[T]:
+class TreeClass(metaclass=TreeClassMeta):
     """Convert a class to a JAX compatible tree structure.
 
     Args:
         klass: class to be converted to a `treeclass`
         leafwise: Wether to generate leafwise math operations methods. Defaults to `False`.
 
     Example:
         >>> import functools as ft
         >>> import jax
         >>> import pytreeclass as pytc
 
         >>> # Tree leaves are defined by type hinted fields at the class level
-        >>> @pytc.treeclass
-        ... class Tree:
+        >>> class Tree(pytc.TreeClass):
         ...     a:int = 1
         ...     b:float = 2.0
         >>> tree = Tree()
         >>> jax.tree_util.tree_leaves(tree)
         [1, 2.0]
 
         >>> # Leaf-wise math operations are supported by setting `leafwise=True`
-        >>> @ft.partial(pytc.treeclass, leafwise=True)
-        ... class Tree:
+        >>> class Tree(pytc.TreeClass, leafwise=True):
         ...     a:int = 1
         ...     b:float = 2.0
         >>> tree = Tree()
         >>> tree + 1
         Tree(a=2, b=3.0)
 
         >>> # Advanced indexing is supported using `at` property
-        >>> @pytc.treeclass
-        ... class Tree:
+        ... class Tree(pytc.TreeClass):
         ...     a:int = 1
         ...     b:float = 2.0
         >>> tree = Tree()
         >>> tree.at[0].get()
         Tree(a=1, b=None)
         >>> tree.at["a"].get()
         Tree(a=1, b=None)
@@ -499,17 +435,12 @@
             '__rlshift__', '__rmatmul__', '__rmod__', '__rmul__', '__ror__', '__round__', '__rpow__',
             '__rrshift__', '__rshift__', '__rsub__', '__rtruediv__', '__rxor__', '__sub__',
             '__truediv__', '__trunc__', '__xor__',
 
     Raises:
         TypeError: if the input is not a class.
     """
-    klass = _register_treeclass(klass)
-    # add math operations methods if leafwise
-    # do not override any user defined methods
-    klass = _leafwise_transform(klass) if leafwise else klass
-    # add `repr`,'str', 'at', 'copy', 'hash', 'copy'
-    # add the immutable setters and deleters
-    # generate the `__init__` method if not present using type hints.
-    klass = _treeclass_transform(klass)
 
-    return klass
+    def __init_subclass__(klass: type[T], leafwise: bool = False) -> None:
+        klass = _register_treeclass(klass)
+        klass = _leafwise_transform(klass) if leafwise else klass
+        klass = _treeclass_transform(klass)
```

### Comparing `pytreeclass-0.2.8/pytreeclass/_src/tree_freeze.py` & `pytreeclass-0.3.0/pytreeclass/_src/tree_freeze.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     if isinstance(node, dict):
         return hash(frozenset(node.items()))
     if isinstance(node, list):
         return hash(tuple(node))
     return hash(node)
 
 
-def tree_hash(tree: PyTree) -> int:
-    hashed = jtu.tree_map(_hash_node, jtu.tree_leaves(tree))
-    return hash((*hashed, jtu.tree_structure(tree)))
+def tree_hash(*trees: PyTree) -> int:
+    hashed = jtu.tree_map(_hash_node, jtu.tree_leaves(trees))
+    return hash((*hashed, jtu.tree_structure(trees)))
 
 
 class _ImmutableWrapper:
     def __init__(self, x: Any) -> None:
         # disable composition of Wrappers
         vars(self)[_WRAPPED] = x.unwrap() if isinstance(x, _ImmutableWrapper) else x
 
@@ -53,41 +53,39 @@
             return False
         return _hash_node(self.unwrap()) == _hash_node(rhs.unwrap())
 
     def __hash__(self) -> int:
         return tree_hash(self.unwrap())
 
 
-class FrozenWrapper(_ImmutableWrapper):
+class _FrozenWrapper(_ImmutableWrapper):
     def __repr__(self):
         return f"#{self.unwrap()!r}"
 
     def __eq__(self, rhs: Any) -> bool:
-        if not isinstance(rhs, FrozenWrapper):
+        if not isinstance(rhs, _FrozenWrapper):
             return False
         return self.unwrap() == rhs.unwrap()
 
     def __hash__(self) -> int:
         return tree_hash(self.unwrap())
 
 
-def _frozen_flatten(tree: Any) -> tuple[tuple, Any]:
+def _flatten(tree: Any) -> tuple[tuple, Any]:
     return (None,), _HashableWrapper(tree.unwrap())
 
 
-def _frozen_unflatten(treedef: Any, _: Sequence[Any]) -> PyTree:
-    tree = object.__new__(FrozenWrapper)  # type: ignore
-    vars(tree)[_WRAPPED] = treedef.unwrap()
-    return tree
+def _unflatten(treedef: Any, _: Sequence[Any]) -> PyTree:
+    return _FrozenWrapper(treedef.unwrap())
 
 
-jtu.register_pytree_node(FrozenWrapper, _frozen_flatten, _frozen_unflatten)
+jtu.register_pytree_node(_FrozenWrapper, _flatten, _unflatten)
 
 
-def freeze(wrapped: Any) -> FrozenWrapper:
+def freeze(wrapped: Any) -> _FrozenWrapper:
     r"""Freeze a value to avoid updating it by `jax` transformations.
 
     Example:
         >>> import jax
         >>> import pytreeclass as pytc
         >>> import jax.tree_util as jtu
         >>> # Usage with `jax.tree_util.tree_leaves`
@@ -101,16 +99,15 @@
 
         >>> # Usage with `jax.tree_util.tree_map`
         >>> a= [1,2,3]
         >>> a[1] = pytc.freeze(a[1])
         >>> jtu.tree_map(lambda x:x+100, a)
         [101, #2, 103]
 
-        >>> @pytc.treeclass
-        ... class Test:
+        >>> class Test(pytc.TreeClass):
         ...     a: float
         ...     @jax.value_and_grad
         ...     def __call__(self, x):
         ...         # unfreeze `a` to update it
         ...         self = jax.tree_util.tree_map(pytc.unfreeze, self, is_leaf=pytc.is_frozen)
         ...         return x ** self.a
 
@@ -130,15 +127,15 @@
         >>> tree = Test(a = 2.)
         >>> frozen_tree = jax.tree_map(pytc.freeze, tree)
         >>> value, grad = frozen_tree(2.)
         >>> print(f"value: {value}\ngrad: {grad}")
         value: 4.0
         grad: Test(a=#2.0)
     """
-    return FrozenWrapper(wrapped)
+    return _FrozenWrapper(wrapped)
 
 
 def unfreeze(x: Any) -> Any:
     """Unfreeze `frozen` value, otherwise return the value itself.
 
     - use `is_leaf=pytc.is_frozen` with `jax.tree_util.tree_map` to unfreeze a tree.**
 
@@ -150,20 +147,20 @@
         1
         >>> # usage with `jax.tree_map`
         >>> frozen_tree = jtu.tree_map(pytc.freeze, {"a": 1, "b": 2})
         >>> unfrozen_tree = jtu.tree_map(pytc.unfreeze, frozen_tree, is_leaf=pytc.is_frozen)
         >>> unfrozen_tree
         {'a': 1, 'b': 2}
     """
-    return x.unwrap() if isinstance(x, FrozenWrapper) else x
+    return x.unwrap() if isinstance(x, _FrozenWrapper) else x
 
 
 def is_frozen(wrapped: Any) -> bool:
     """Returns True if the value is a frozen wrapper."""
-    return isinstance(wrapped, FrozenWrapper)
+    return isinstance(wrapped, _FrozenWrapper)
 
 
 def is_nondiff(x: Any) -> bool:
     """Returns False if the node is a float, complex number, or a numpy array of floats or complex numbers.
 
     Example:
         >>> import pytreeclass as pytc
```

### Comparing `pytreeclass-0.2.8/pytreeclass/_src/tree_indexer.py` & `pytreeclass-0.3.0/pytreeclass/_src/tree_indexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,40 +14,29 @@
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import numpy as np
 
 from pytreeclass._src.tree_trace import tree_map_with_trace
 
+T = TypeVar("T")
+PyTree = TypeVar("PyTree")
 EllipsisType = type(Ellipsis)
 TraceType = Any
+
 _no_initializer = object()
 _non_partial = object()
-PyTree = TypeVar("PyTree")
-T = TypeVar("T")
 
-# allow methods in mutable context to be called without raising an error
+# allow methods in mutable context to be called without raising `AttributeError`
+# the instances are registered  during initialization and using `at` property with `__call__
 # this is done by registering the instance id in a set before entering the
 # mutable context and removing it after exiting the context
 _mutable_instance_registry: set[int] = set()
 
 
-def _conditional_mutable_method(method: Callable) -> Callable:
-    # decorator to allow for decorated methods to be called
-    # within the mutable context and raise an error otherwise
-    @ft.wraps(method)
-    def wrapper(self, *a, **k):
-        if id(self) in _mutable_instance_registry:
-            return method(self, *a, **k)
-        msg = f"Cannot call `{method.__name__}` on frozen instance."
-        raise AttributeError(msg)
-
-    return wrapper
-
-
 @contextmanager
 def _mutable_context(tree: PyTree, *, kopy: bool = False):
     tree = copy.copy(tree) if kopy else tree
     _mutable_instance_registry.add(id(tree))
     yield tree
     _mutable_instance_registry.discard(id(tree))
 
@@ -57,15 +46,15 @@
 
 def _get_at_mask(
     tree: PyTree, where: PyTree, is_leaf: Callable[[Any], bool] | None
 ) -> PyTree:
     def leaf_get(leaf: Any, where: Any):
         # check if where is a boolean leaf inside the `tree_map`
         # to avoid extrachecks in `tree_map`
-        if isinstance(leaf, (jax.Array, np.ndarray)):
+        if isinstance(leaf, (jax.Array, np.ndarray)) and jnp.ndim(leaf) > 0:
             # return empty array instead of None if condition is not met
             # not `jittable` as size of array changes
             return leaf[jnp.where(where)]
         return leaf if where else None
 
     return jtu.tree_map(leaf_get, tree, where, is_leaf=is_leaf)
 
@@ -154,25 +143,25 @@
     ):
         names, _, indices = trace
         is_array = isinstance(leaf, (jax.Array, np.ndarray))
 
         if len(where) > len(indices):
             return jnp.zeros_like(leaf, dtype=bool) if is_array else False
         for i, item in enumerate(where):
-            if item is ... or indices[i] == item or names[i] == item:
-                # no mismatch in where and trace
-                continue
-            return jnp.zeros_like(leaf, dtype=bool) if is_array else False
+            if not (item is ... or indices[i] == item or names[i] == item):
+                return jnp.zeros_like(leaf, dtype=bool) if is_array else False
         return jnp.ones_like(leaf, dtype=bool) if is_array else True
 
     def merge_boolean_where(*leaves):
         def is_leaf_bool(leaf: Any) -> bool:
-            if hasattr(leaf, "dtype"):
-                return leaf.dtype == "bool"
-            return isinstance(leaf, bool)
+            return (
+                leaf.dtype == "bool"
+                if hasattr(leaf, "dtype")
+                else isinstance(leaf, bool)
+            )
 
         verdict = True
         for leaf in leaves:
             if not is_leaf_bool(leaf):
                 msg = f"Expected boolean leaf, found {type(leaf).__name__}."
                 raise TypeError(msg)
             verdict &= leaf
@@ -208,16 +197,15 @@
     def __getitem__(self, where: str | int | PyTree | EllipsisType) -> AtIndexer:
         if isinstance(where, (type(self.tree), str, int, EllipsisType)):
             return AtIndexer(self.tree, (*self.where, where))
 
         raise NotImplementedError(
             f"Indexing with {type(where).__name__} is not implemented.\n"
             "Example of supported indexing:\n\n"
-            "@pytc.treeclass\n"
-            f"class {type(self.tree).__name__}:\n"
+            f"class {type(self.tree).__name__}:(pytc.TreeClass)\n"
             "    ...\n\n"
             f">>> tree = {type(self.tree).__name__}(...)\n"
             ">>> # indexing by boolean pytree\n"
             ">>> tree.at[tree > 0].get()\n\n"
             ">>> # indexing by attribute name\n"
             ">>> tree.at[`attribute_name`].get()\n\n"
             ">>> # indexing by attribute index\n"
@@ -332,16 +320,15 @@
         is_leaf: a function that returns True if the argument is a leaf of the pytree
 
     Example:
         >>> import jax
         >>> import pytreeclass as pytc
         >>> import functools as ft
 
-        >>> @ft.partial(pytc.treeclass, leafwise=True)
-        ... class Test:
+        >>> class Test(pytc.TreeClass, leafwise=True):
         ...    a: tuple[int] = (1,2,3)
         ...    b: tuple[int] = (4,5,6)
         ...    c: jax.Array = jnp.array([1,2,3])
 
         >>> tree = Test()
 
         >>> # 0 is broadcasted to all leaves of the pytree
```

### Comparing `pytreeclass-0.2.8/pytreeclass/_src/tree_pprint.py` & `pytreeclass-0.3.0/pytreeclass/_src/tree_pprint.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         return _tuple_pprint(node, indent, kind, width, depth)
     if isinstance(node, set):
         return _set_pprint(node, indent, kind, width, depth)
     if isinstance(node, dict):
         return _dict_pprint(node, indent, kind, width, depth)
     if dc.is_dataclass(node):
         return _dataclass_pprint(node, indent, kind, width, depth)
-    if pytc.is_treeclass(node):
+    if isinstance(node, pytc.TreeClass):
         return _treeclass_pprint(node, indent, kind, width, depth)
     return _general_pprint(node, indent, kind, width, depth)
 
 
 def _general_pprint(
     node: Any,
     indent: int,
@@ -82,15 +82,14 @@
     """Pretty print a node with dtype and shape"""
     del indent, kind, depth
 
     shape = f"{node.shape}".replace(",", "")
     shape = shape.replace("(", "[")
     shape = shape.replace(")", "]")
     shape = shape.replace(" ", ",")
-    shape = shape.replace("[]", "[0]")
     dtype = f"{node.dtype}".replace("int", "i")
     dtype = dtype.replace("float", "f")
     dtype = dtype.replace("complex", "c")
     return _format_width(dtype + shape, width)
 
 
 def _numpy_pprint(
@@ -247,15 +246,15 @@
     depth: int,
 ) -> str:
     name = type(node).__name__
 
     if depth == 0:
         fmt = "..."
     else:
-        kvs = ((F.name, vars(node)[F.name]) for F in dc.fields(node) if F.repr)
+        kvs = ((f.name, vars(node)[f.name]) for f in dc.fields(node) if f.repr)
         fmt = (f"{k}={_node_pprint(v,indent+1,kind,width,depth-1)}" for k, v in kvs)
         fmt = (", \n" + "\t" * (indent + 1)).join(fmt)
 
     fmt = f"{name}(\n" + "\t" * (indent + 1) + (fmt) + "\n" + "\t" * (indent) + ")"
     return _format_width(fmt, width)
 
 
@@ -267,15 +266,15 @@
     depth: int,
 ) -> str:
     name = type(node).__name__
     if depth == 0:
         fmt = "..."
 
     else:
-        kvs = ((F.name, vars(node)[F.name]) for F in pytc.fields(node) if F.repr)
+        kvs = ((k, vars(node)[k]) for k, f in node._fields.items() if f.repr)
         fmt = (f"{k}={_node_pprint(v,indent+1,kind,width,depth-1)}" for k, v in kvs)
         fmt = (", \n" + "\t" * (indent + 1)).join(fmt)
     fmt = f"{name}(\n" + "\t" * (indent + 1) + (fmt) + "\n" + "\t" * (indent) + ")"
     return _format_width(fmt, width)
 
 
 def _node_type_pprint(
@@ -525,22 +524,20 @@
         tree: PyTree
         depth: depth of the tree to print. default is max depth
         width: max width of line. default is 60
         is_leaf: function to determine if a node is a leaf. default is None
 
     Example:
         >>> import pytreeclass as pytc
-        >>> @pytc.treeclass
-        ... class A:
+        >>> class A(pytc.TreeClass):
         ...        x: int = 10
         ...        y: int = (20,30)
         ...        z: int = 40
 
-        >>> @pytc.treeclass
-        ... class B:
+        >>> class B(pytc.TreeClass):
         ...     a: int = 10
         ...     b: tuple = (20,30, A())
 
         >>> print(pytc.tree_diagram(B(), depth=0))
         B
 
         >>> print(pytc.tree_diagram(B(), depth=1))
@@ -901,16 +898,15 @@
     Args:
         tree: pytree to summarize.
         is_leaf: function to determine if a node is a leaf. defaults to None
         transpose: transpose the table. i.e. rows become cols and cols become rows
 
     Example:
         >>> import pytreeclass as pytc
-        >>> @pytc.treeclass
-        ... class Test:
+        >>> class Test(pytc.TreeClass):
         ...    a:int = 1
         ...    b:float = 2.0
 
         >>> tree = Test()
         >>> print(pytc.tree_repr_with_trace(Test()))  # doctest: +SKIP
         Test(
           a=
```

### Comparing `pytreeclass-0.2.8/pytreeclass/_src/tree_trace.py` & `pytreeclass-0.3.0/pytreeclass/_src/tree_trace.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from jax._src.tree_util import _registry
 
 """Extending `jax.tree_util` to support `tree_viz` and `tree_indexer` functionality"""
 
 # the code style is heavilty influenced by `jax.tree_util`
 # https://github.com/google/jax/blob/main/jax/_src/tree_util.py
 
-
 PyTree = Any
 TraceType = Any
 
 
 def _jaxable_trace_func(tree: Any) -> list[TraceType]:
     # fallback trace function in case no trace function is registered for a given
     # class in the `trace` registry
@@ -60,27 +59,27 @@
                 msg += "Expected 3 entries, in the order of"
                 msg += f"(name, type, index), got {trace}"
                 raise ValueError(msg)
 
             if not isinstance(trace[0], (str, type(None))):
                 msg = "Trace name entry is not defined properly for "
                 msg += f"class=`{type(tree).__name__}`."
-                msg += f" Expected a string, got {trace[0]}"
+                msg += f" Expected a string or `None`, got {trace[0]}"
                 raise TypeError(msg)
 
             if not isinstance(trace[1], type):
                 msg = "Trace type entry is not defined properly for "
                 msg += f"class=`{type(tree).__name__}`."
                 msg += f" Expected a type, got {trace[1]}"
                 raise TypeError(msg)
 
             if not isinstance(trace[2], (int, type(None))):
                 msg = "Trace index entry is not defined properly for "
                 msg += f"class=`{type(tree).__name__}`."
-                msg += f" Expected an integer, got {trace[2]}"
+                msg += f" Expected an integer or `None`, got {trace[2]}"
                 raise TypeError(msg)
 
         wrapper.has_run = True
         return traces
 
     wrapper.has_run = False
     return wrapper
@@ -216,16 +215,15 @@
         A list of (trace, leaf) pairs.
 
     Example:
         >>> import pytreeclass as pytc
         >>> tree = [1, [2, [3]]]
         >>> traces, _ = zip(*pytc.tree_leaves_with_trace(tree))
     """
-    trace = ((), (), ())
-    return list(flatten_one_trace_level(trace, tree, is_leaf, is_trace_leaf))
+    return list(flatten_one_trace_level(((), (), ()), tree, is_leaf, is_trace_leaf))
 
 
 def tree_flatten_with_trace(
     tree: PyTree,
     *,
     is_leaf: Callable[[Any], bool] | None = None,
 ) -> tuple[Sequence[tuple[TraceType, Any]], jtu.PyTreeDef]:
```

### Comparing `pytreeclass-0.2.8/pytreeclass.egg-info/PKG-INFO` & `pytreeclass-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: pytreeclass
-Version: 0.2.8
-Summary: JAX compatible dataclass.
-Home-page: https://github.com/ASEM000/pytreeclass
-Author: Mahmoud Asem
-Author-email: asem00@kaist.ac.kr
-License: Apache-2.0
-Keywords: python machine-learning pytorch jax
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <!-- <h1 align="center" style="font-family:Monospace" >Py🌲Class</h1> -->
 <h5 align="center">
 <img width="250px" src="https://user-images.githubusercontent.com/48389287/227880173-bf78c02c-d28b-4cf4-95e6-fa49b82a43a1.svg"> <br>
 
 <br>
 
 [**Installation**](#installation)
@@ -60,15 +37,15 @@
 
 ```python
 pip install git+https://github.com/ASEM000/PyTreeClass
 ```
 
 ## 📖 Description<a id="description"></a>
 
-`PyTreeClass` is a JAX-compatible `dataclass`-like decorator to create and operate on stateful JAX PyTrees.
+`PyTreeClass` is a JAX-compatible class builder to create and operate on stateful JAX PyTrees.
 
 The package aims to achieve _two goals_:
 
 1. 🔒 To maintain safe and correct behaviour by using _immutable_ modules with _functional_ API.
 2. To achieve the **most intuitive** user experience in the `JAX` ecosystem by :
    - 🏗️ Defining layers similar to `PyTorch` or `TensorFlow` subclassing style.
    - ☝️ Filtering\Indexing layer values similar to `jax.numpy.at[].{get,set,apply,...}`
@@ -85,16 +62,15 @@
 <td>
 
 ```python
 import jax
 import jax.numpy as jnp
 import pytreeclass as pytc
 
-@pytc.treeclass
-class Tree:
+class Tree(pytc.TreeClass):
     a:int = 1
     b:tuple[float] = (2.,3.)
     c:jax.Array = jnp.array([4.,5.,6.])
 
     def __call__(self, x):
         return self.a + self.b[0] + self.c + x
 
@@ -299,16 +275,15 @@
 ```python
 
 import pytreeclass as pytc
 import jax
 import jax.numpy as jnp
 
 
-@pytc.treeclass
-class Tree:
+class Tree(pytc.TreeClass)
     a: int = 1
     b: tuple[float] = (2., 3.)
     c: jax.Array = jnp.array([4., 5., 6.])
 
     def __call__(self, x):
         return self.a + self.b[0] + self.c + x
 
@@ -424,24 +399,23 @@
 
 <details>
 
 <summary>
 
 ## 📜 Stateful computations<a id="stateful_computation"></a> </summary>
 
-First, [Under jax.jit jax requires states to be explicit](https://jax.readthedocs.io/en/latest/jax-101/07-state.html?highlight=state), this means that for any class instance; variables needs to be separated from the class and be passed explictly. However when using @pytc.treeclass no need to separate the instance variables ; instead the whole instance is passed as a state.
+First, [Under jax.jit jax requires states to be explicit](https://jax.readthedocs.io/en/latest/jax-101/07-state.html?highlight=state), this means that for any class instance; variables needs to be separated from the class and be passed explictly. However when using `TreeClass` no need to separate the instance variables ; instead the whole instance is passed as a state.
 
 Using the following pattern,Updating state **functionally** can be achieved under `jax.jit`
 
 ```python
 import jax
 import pytreeclass as pytc
 
-@pytc.treeclass
-class Counter:
+class Counter(pytc.TreeClass):
     calls : int = 0
 
     def increment(self):
         self.calls += 1
 counter = Counter() # Counter(calls=0)
 ```
 
@@ -544,16 +518,15 @@
     if not isinstance(value, int):
         raise TypeError("Value must be an integer")
     if value <= 0:
         raise ValueError("Value must be positive")
     return value
 
 
-@pytc.treeclass
-class Tree:
+class Tree(pytc.TreeClass):
     in_features:int = pytc.field(callbacks=[positive_int_callback])
 
 
 tree = Tree(1)
 # no error
 
 tree = Tree(0)
@@ -573,16 +546,15 @@
 import functools as ft
 import pytreeclass as pytc
 import jax
 import jax.tree_util as jtu
 import jax.numpy as jnp
 
 
-@ft.partial(pytc.treeclass, leafwise=True)
-class Tree:
+class Tree(pytc.TreeClass, leafwise=True):
     a: int = 1
     b: tuple[float] = (2., 3.)
     c: jax.Array = jnp.array([4., 5., 6.])
 
     def __call__(self, x):
         return self.a + self.b[0] + self.c + x
 
@@ -632,16 +604,15 @@
 TDLR
 
 ```python
 import functools as ft
 import pytreeclass as pytc
 import jax.numpy as jnp
 
-@ft.partial(pytc.treeclass, leafwise=True)
-class Tree:
+class Tree(pytc.TreeClass, leafwise=True):
     a:int = 1
     b:tuple[float] = (2.,3.)
     c:jax.Array = jnp.array([4.,5.,6.])
 
 tree = Tree()
 
 print(pytc.bcmap(jnp.where)(tree>2, tree+100, 0))
@@ -718,16 +689,16 @@
 #  Array(1000, dtype=int32, weak_type=True))
 ```
 
 lets then take this a step further to eliminate `mask` from the equation
 by using `pytreeclass` with `leafwise=True `
 
 ```python
-@ft.partial(pytc.treeclass, leafwise=True)
-class Tree:
+
+class Tree(pytc.TreeClass, leafwise=True):
     tree : tuple = ([1], {"a":1, "b":2}, (1,), -1,)
 
 tree = Tree()
 # Tree(tree=([1], {a:1, b:2}, (1), -1))
 ```
 
 case 1: broadcast scalar to tree
@@ -912,16 +883,15 @@
 For demonstration , the following figure contains the 4 variants of the same `Tree` instance define
 
 ```python
 import jax
 import jax.numpy as jnp
 import pytreeclass as pytc
 
-@pytc.treeclass
-class Tree:
+class Tree(pytc.TreeClass):
     a:int = 1
     b:tuple[float] = (2.,3.)
     c:jax.Array = jnp.array([4.,5.,6.])
 ```
 
 ![image](assets/tree_figures.png)
```

### Comparing `pytreeclass-0.2.8/pytreeclass.egg-info/SOURCES.txt` & `pytreeclass-0.3.0/pytreeclass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.2.8/setup.py` & `pytreeclass-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.2.8/tests/test_indexing.py` & `pytreeclass-0.3.0/tests/test_indexing.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 from __future__ import annotations
 
-import functools as ft
 from collections import namedtuple
 
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import numpy.testing as npt
 import pytest
 
 import pytreeclass as pytc
+from pytreeclass import TreeClass
 from pytreeclass._src.tree_indexer import _mutable_context
 
 
-@ft.partial(pytc.treeclass, leafwise=True)
-class Tree:
+class Tree(TreeClass, leafwise=True):
     a: float
     b: float
     c: float
     d: jnp.ndarray
     name: str
 
     def __post_init__(self):
         self.name = pytc.freeze(self.name)
 
 
 def test_getter_by_val():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class level1:
+    class level1(TreeClass, leafwise=True):
         a: int
         b: int
         c: int
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class level2:
+    class level2(TreeClass, leafwise=True):
         d: level1
         e: level1
 
     A = level2(
         d=level1(a=1, b=10, c=jnp.array([1, 2, 3, 4, 5])),
         e=level1(a=2, b=20, c=jnp.array([-1, -2, -3, -4, -5])),
     )
@@ -70,29 +67,26 @@
         B = A.at[A].get()
 
     # with pytest.raises(NotImplementedError):
     #     B = A.at[0].get()
 
 
 def test_getter_by_param():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class L0:
+    class L0(TreeClass, leafwise=True):
         a: int = 1
         b: int = 2
         c: int = 3
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class L1:
+    class L1(TreeClass, leafwise=True):
         a: int = 1
         b: int = 2
         c: int = 3
         d: L0 = L0()
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class L2:
+    class L2(TreeClass, leafwise=True):
         a: int = 10
         b: int = 20
         c: int = 30
         d: L1 = L1()
 
     # t = L2()
 
@@ -100,22 +94,20 @@
     #     t.at["s"].get()
 
     # with pytest.raises(AttributeError):
     #     t.at["s"].apply(lambda _: 100)
 
 
 def test_setter_by_val():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class level1:
+    class level1(TreeClass, leafwise=True):
         a: int
         b: int
         c: int
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class level2:
+    class level2(TreeClass, leafwise=True):
         d: level1
         e: level1
 
     A = level2(
         d=level1(a=1, b=10, c=jnp.array([1, 2, 3, 4, 5])),
         e=level1(a=2, b=20, c=jnp.array([-1, -2, -3, -4, -5])),
     )
@@ -132,44 +124,40 @@
 
     with pytest.raises(TypeError):
         B = A.at[A].set(0)
 
     # with pytest.raises(NotImplementedError):
     #     B = A.at[0].set(0)
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class L0:
+    class L0(TreeClass, leafwise=True):
         a: int = 1
         b: int = 2
         c: int = 3
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class L1:
+    class L1(TreeClass, leafwise=True):
         a: int = 1
         b: int = 2
         c: int = 3
         d: L0 = L0()
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class L2:
+    class L2(TreeClass, leafwise=True):
         a: int = 10
         b: int = 20
         c: int = 30
         d: L1 = L1()
 
     t = L2()
 
     tt = L2(100, 200, 300, L1(10, 20, 30, L0(10, 20, 30)))
     lhs = t.at[t == t].set(tt)
     assert pytc.is_tree_equal(lhs, tt)
 
 
 def test_apply_and_its_derivatives():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class A:
+    class A(TreeClass, leafwise=True):
         a: int
         b: int
         c: jnp.ndarray
 
     init = A(1, 2, jnp.array([1, 2, 3, 4, 5]))
 
     # By boolean pytree
@@ -196,29 +184,26 @@
     lhs = A(20, 30, jnp.array([20, 30, 40, 50, 60]))
     rhs = init.at[...].apply(lambda x: (x + 1) * 10)
     assert pytc.is_tree_equal(lhs, rhs)
 
     with pytest.raises(TypeError):
         init.at[init].apply(lambda x: (x + 1) * 10)
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class L0:
+    class L0(TreeClass, leafwise=True):
         a: int = 1
         b: int = 2
         c: int = 3
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class L1:
+    class L1(TreeClass, leafwise=True):
         a: int = 1
         b: int = 2
         c: int = 3
         d: L0 = L0()
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class L2:
+    class L2(TreeClass, leafwise=True):
         a: int = 10
         b: int = 20
         c: int = 30
         d: L1 = L1()
 
     lhs = A(2, 3, jnp.array([2, 3, 4, 5, 6]))
     rhs = init.at[init == init].apply(lambda x: x + 1)
@@ -273,16 +258,15 @@
 
     lhs = A(1, 4, jnp.array([1, 4, 3, 4, 5]))
     rhs = init.at[init == 2].apply(lambda x: x * 2)
     assert pytc.is_tree_equal(lhs, rhs)
 
 
 def test_reduce():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class A:
+    class A(TreeClass, leafwise=True):
         a: int
         b: int
         c: jnp.ndarray
 
     init = A(1, 2, jnp.array([1, 2, 3, 4, 5]))
 
     lhs = 2 + 2 + 3 + 4 + 5
@@ -293,55 +277,51 @@
     rhs = init.at[init > 2].reduce(lambda x, y: x + jnp.sum(y), initializer=0)
     assert lhs == rhs
 
     lhs = 0
     rhs = init.at[init > 100].reduce(lambda x, y: x + jnp.sum(y), initializer=0)
     assert lhs == rhs
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class B:
+    class B(TreeClass, leafwise=True):
         a: int
         b: int
         c: jnp.ndarray
         d: tuple
 
     init = B(1, 2, jnp.array([1, 2, 3, 4, 5]), (10, 20, 30))
 
     lhs = 2 + 2 + 3 + 4 + 5 + 10 + 20 + 30
     rhs = init.at[init > 1].reduce(lambda x, y: x + jnp.sum(y), initializer=0)
     assert lhs == rhs
 
     with pytest.raises(TypeError):
         init.at[init].reduce(lambda x, y: x + jnp.sum(y), initializer=0)
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Tree:
+    class Tree(TreeClass, leafwise=True):
         a: tuple[int]
 
     lhs = Tree((1, 2, 3)).at["a"].reduce(lambda x, y: x + y, initializer=0)
     assert lhs == 6
 
 
 def test_reduce_and_its_derivatives():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Linear:
+    class Linear(TreeClass, leafwise=True):
         weight: jnp.ndarray
         bias: jnp.ndarray
 
         def __init__(self, key, in_dim, out_dim):
             self.weight = jax.random.normal(key, shape=(in_dim, out_dim)) * jnp.sqrt(
                 2 / in_dim
             )
             self.bias = jnp.ones((1, out_dim))
 
         # def __call__(self, x):
         #     return x @ self.weight + self.bias
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class StackedLinear:
+    class StackedLinear(TreeClass, leafwise=True):
         l1: Linear
         l2: Linear
 
         def __init__(self, key, in_dim, out_dim, hidden_dim):
             keys = jax.random.split(key, 3)
 
             self.l1 = Linear(key=keys[0], in_dim=in_dim, out_dim=hidden_dim)
@@ -366,16 +346,15 @@
     npt.assert_allclose(
         tree.at[tree > 0].reduce(lambda x, y: x * jnp.product(y), initializer=1),
         1.8088213,
     )
 
 
 def test_is_leaf():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Tree:
+    class Tree(TreeClass, leafwise=True):
         a: int
 
     t = Tree([1, 2, 3, None])
 
     mask = jtu.tree_map(lambda x: True, t, is_leaf=lambda x: x is None)
 
     assert pytc.is_tree_equal(
@@ -385,71 +364,63 @@
     assert pytc.is_tree_equal(
         t.at[mask].apply(lambda x: 10, is_leaf=lambda x: x is None),
         Tree([10, 10, 10, 10]),
     )
 
 
 def test_attribute_get():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class l0:
+    class l0(TreeClass, leafwise=True):
         a: int = 2
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Tree:
+    class Tree(TreeClass, leafwise=True):
         a: int = 1
         b: l0 = l0()
 
     t = Tree()
     assert pytc.is_tree_equal(t.at["a"].get(), Tree(1, l0(None)))
     assert pytc.is_tree_equal(t.at["b"].at["a"].get(), Tree(None, l0(2)))
 
 
 def test_attribute_set():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class l0:
+    class l0(TreeClass, leafwise=True):
         a: int = 2
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Tree:
+    class Tree(TreeClass, leafwise=True):
         a: int = 1
         b: l0 = l0()
 
     t = Tree()
     t.at["a"].set(10)
 
     assert pytc.is_tree_equal(t, Tree())
     assert pytc.is_tree_equal(t.at["a"].set(10), Tree(10, l0()))
     assert pytc.is_tree_equal(t.at["b"].at["a"].set(100), Tree(1, l0(100)))
 
 
 def test_attributre_apply():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class l0:
+    class l0(TreeClass, leafwise=True):
         a: int = 2
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Tree:
+    class Tree(TreeClass, leafwise=True):
         a: int = 1
         b: l0 = l0()
 
     t = Tree()
     t.at["a"].apply(lambda _: 10)
 
     assert pytc.is_tree_equal(t, Tree())
     assert pytc.is_tree_equal(t.at["a"].apply(lambda _: 10), Tree(10))
     assert pytc.is_tree_equal(t.at["b"].at["a"].apply(lambda _: 100), Tree(1, l0(100)))
 
 
 def test_trace_get():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class l0:
+    class l0(TreeClass, leafwise=True):
         a: int = 2
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Tree:
+    class Tree(TreeClass, leafwise=True):
         a: int = 1
         b: l0 = l0()
 
     t = Tree()
     assert pytc.is_tree_equal(t.at[0].get(), Tree(1, l0(None)))
     assert pytc.is_tree_equal(t.at[1].at[0].get(), Tree(None, l0(2)))
 
@@ -461,90 +432,81 @@
     # with pytest.raises(IndexError):
     #     t.at[0].at[1].apply(lambda _: 10)
     # with pytest.raises(IndexError):
     #     t.at[0].at[1].reduce(lambda _, __: 10)
 
 
 def test_trace_set():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class l0:
+    class l0(TreeClass, leafwise=True):
         a: int = 2
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Tree:
+    class Tree(TreeClass, leafwise=True):
         a: int = 1
         b: l0 = l0()
 
     t = Tree()
     t.at["a"].set(10)
 
     assert pytc.is_tree_equal(t, Tree())
     assert pytc.is_tree_equal(t.at[0].set(10), Tree(10, l0()))
     assert pytc.is_tree_equal(t.at[1].at[0].set(100), Tree(1, l0(100)))
 
 
 def test_trace_apply():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class l0:
+    class l0(TreeClass, leafwise=True):
         a: int = 2
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Tree:
+    class Tree(TreeClass, leafwise=True):
         a: int = 1
         b: l0 = l0()
 
     t = Tree()
     t.at["a"].apply(lambda _: 10)
 
     assert pytc.is_tree_equal(t, Tree())
     assert pytc.is_tree_equal(t.at[0].apply(lambda _: 10), Tree(10))
     assert pytc.is_tree_equal(t.at[1].at[0].apply(lambda _: 100), Tree(1, l0(100)))
 
 
 def test_trace_reduce():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class A:
+    class A(TreeClass, leafwise=True):
         a: int
         b: int
         c: jnp.ndarray
 
     init = A(1, 2, jnp.array([1, 2, 3, 4, 5]))
 
     lhs = 1 + 2 + 3 + 4 + 5
     rhs = init.at[2].reduce(lambda x, y: x + jnp.sum(y), initializer=0)
     assert lhs == rhs
 
 
 def test_mixed_get():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class l0:
+    class l0(TreeClass, leafwise=True):
         a: int = 2
         b: int = 1
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Tree:
+    class Tree(TreeClass, leafwise=True):
         a: int = 1
         b: l0 = l0()
 
     t = Tree()
     assert pytc.is_tree_equal(t.at[1].at[t == 2].get(), Tree(None, l0(2, None)))
     assert pytc.is_tree_equal(t.at[t == 2].at[1].get(), Tree(None, l0(2, None)))
 
     # with pytest.raises(IndexError):
     #     t.at[0].at[2].get()
 
 
 def test_mixed_set():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class l0:
+    class l0(TreeClass, leafwise=True):
         a: int = 2
         b: int = 1
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Tree:
+    class Tree(TreeClass, leafwise=True):
         a: int = 1
         b: l0 = l0()
 
     t = Tree()
 
     assert pytc.is_tree_equal(t.at["b"].at[t == 2].set(100), Tree(1, l0(100)))
     assert pytc.is_tree_equal(t.at[t == 2].at["b"].set(100), Tree(1, l0(100)))
@@ -553,61 +515,56 @@
     assert pytc.is_tree_equal(t.at["b"].at[0].set(100), Tree(1, l0(100)))
 
     # with pytest.raises(IndexError):
     #     assert pytc.is_tree_equal(t.at[0].at["b"].set(100), Tree(1, l0(100, 2)))
 
 
 def test_mixed_apply():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class l0:
+    class l0(TreeClass, leafwise=True):
         a: int = 2
         b: int = 1
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Tree:
+    class Tree(TreeClass, leafwise=True):
         a: int = 1
         b: l0 = l0()
 
     t = Tree()
 
     assert pytc.is_tree_equal(t.at[1].at[t == 2].apply(lambda _: 100), Tree(1, l0(100)))
     assert pytc.is_tree_equal(t.at["b"].at[0].apply(lambda _: 100), Tree(1, l0(100)))
 
     # with pytest.raises(IndexError):
     #     t.at[0].at["a"].apply(lambda _: 100), Tree(1, l0(100))
 
 
 def test_method_call():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Tree:
+    class Tree(TreeClass, leafwise=True):
         a: int = 1
 
         def increment(self):
             self.a += 1
 
         def show(self):
             return 1
 
     t = Tree()
 
-    @pytc.treeclass
-    class Tree2:
+    class Tree2(TreeClass):
         b: Tree = Tree()
 
     assert pytc.is_tree_equal(t.at["increment"]()[1], Tree(2))
     assert pytc.is_tree_equal(Tree2().at["b"].at["show"]()[0], 1)
 
     with pytest.raises(AttributeError):
         t.at["bla"]()
 
     with pytest.raises(TypeError):
         t.at["a"]()
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class A:
+    class A(TreeClass, leafwise=True):
         a: int
 
         def __call__(self, x):
             self.a += x
             return x
 
     a = A(1)
@@ -617,16 +574,15 @@
     assert jtu.tree_leaves(b) == [3]
 
     with pytest.raises(TypeError):
         a.at[0](1)
 
 
 def test_composed_at():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Tree:
+    class Tree(TreeClass, leafwise=True):
         a: jnp.ndarray
 
         def __init__(self, a=jnp.array([1, 2, 3, 4, 5])) -> None:
             self.a = a
 
     t = Tree()
 
@@ -636,58 +592,45 @@
         t.at[t > 0].bet
 
     with pytest.raises(AttributeError):
         t.at["a"].bet
 
 
 def test_repr_str():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Tree:
+    class Tree(TreeClass, leafwise=True):
         a: int = 1
         b: int = 2
 
     t = Tree()
 
     assert repr(t.at["a"]) == "AtIndexer(tree=Tree(a=1, b=2), where=('a',))"
     assert str(t.at["a"]) == "AtIndexer(tree=Tree(a=1, b=2), where=('a',))"
     assert repr(t.at[...]) == "AtIndexer(tree=Tree(a=1, b=2), where=(Ellipsis,))"
 
 
 def test_not_equal():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Tree:
+    class Tree(TreeClass, leafwise=True):
         a: int = 1
         b: float = 1.0
 
     t = Tree()
 
     assert pytc.is_tree_equal(t.at[t != 10].set(10.0), Tree(a=10.0, b=10.0))
 
 
 def test_iterable_node():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Tree:
+    class Tree(TreeClass, leafwise=True):
         a: int
 
     t = Tree([1, 2, 3, 4])
     assert pytc.is_tree_equal(t.at[...].set(True), Tree([True, True, True, True]))
 
 
-# def test_at_set_apply_is_leaf():
-#     @ft.partial(pytc.treeclass, leafwise=True)
-#     class Tree:
-#         a: int = 1
-#         b: int = 2
-
-# t = Tree()
-
-
 def test_call_context():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class L2:
+    class L2(TreeClass, leafwise=True):
         a: int = 1
 
         def delete(self, name):
             del self.a
 
     t = L2()
 
@@ -695,16 +638,15 @@
         tx.delete("a")
 
     with pytest.raises(AttributeError):
         t.delete("a")
 
 
 def test_unsupported_indexing_type():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class L2:
+    class L2(TreeClass, leafwise=True):
         a: int = 1
 
         def delete(self, name):
             del self.a
 
     t = L2()
 
@@ -717,16 +659,15 @@
         pytc.register_pytree_node_trace(None, None)
 
     with pytest.raises(ValueError):
         pytc.register_pytree_node_trace(list, lambda x: x)
 
 
 def test_mixed_not_implemented():
-    @pytc.treeclass
-    class T:
+    class T(TreeClass):
         a: tuple[int, ...] = namedtuple("a", ["x", "y"])(1, 2)
 
     t = T()
 
     with pytest.raises(NotImplementedError):
         t.at["a"].at[[1]].get()
```

### Comparing `pytreeclass-0.2.8/tests/test_nn.py` & `pytreeclass-0.3.0/tests/test_nn.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,32 @@
-import functools as ft
 from typing import Callable, Sequence
 
 import jax
 import jax.numpy as jnp
 import jax.random as jr
 import jax.tree_util as jtu
 import numpy as np
 import pytest
 
 import pytreeclass as pytc
 
 
 def test_nn():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Linear:
+    class Linear(pytc.TreeClass, leafwise=True):
         weight: jax.Array
         bias: jax.Array
 
         def __init__(self, key, in_dim, out_dim):
             self.weight = jr.normal(key, shape=(in_dim, out_dim)) * jnp.sqrt(2 / in_dim)
             self.bias = jnp.ones((1, out_dim))
 
         def __call__(self, x):
             return x @ self.weight + self.bias
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class StackedLinear:
+    class StackedLinear(pytc.TreeClass, leafwise=True):
         layers: Sequence[Linear]
 
         def __init__(self, key, layers):
             keys = jr.split(key, len(layers) - 1)
 
             self.layers = []
 
@@ -59,16 +56,15 @@
     for _ in range(1, 2001):
         value, NN = update(NN, x, y)
 
     np.testing.assert_allclose(value, jnp.array(0.00103019), atol=1e-5)
 
 
 def test_nn_with_func_input():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Linear:
+    class Linear(pytc.TreeClass, leafwise=True):
         weight: jax.Array
         bias: jax.Array
         act_func: Callable
 
         def __init__(self, key, in_dim, out_dim, act_func):
             self.act_func = act_func
             self.weight = jr.normal(key, shape=(in_dim, out_dim)) * jnp.sqrt(2 / in_dim)
@@ -81,28 +77,26 @@
     x = jnp.linspace(0, 1, 100)[:, None]
     # y = x**3 + jr.uniform(jr.PRNGKey(0), (100, 1)) * 0.01
     layer(x)
     return True
 
 
 def test_compact_nn():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Linear:
+    class Linear(pytc.TreeClass, leafwise=True):
         weight: jax.Array
         bias: jax.Array
 
         def __init__(self, key, in_dim, out_dim):
             self.weight = jr.normal(key, shape=(in_dim, out_dim)) * jnp.sqrt(2 / in_dim)
             self.bias = jnp.ones((1, out_dim))
 
         def __call__(self, x):
             return x @ self.weight + self.bias
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class StackedLinear:
+    class StackedLinear(pytc.TreeClass, leafwise=True):
         def __init__(self, key, in_dim, out_dim, hidden_dim):
             keys = jr.split(key, 3)
 
             self.l1 = Linear(key=keys[0], in_dim=in_dim, out_dim=hidden_dim)
             self.l2 = Linear(key=keys[1], in_dim=hidden_dim, out_dim=hidden_dim)
             self.l3 = Linear(key=keys[2], in_dim=hidden_dim, out_dim=out_dim)
 
@@ -134,32 +128,30 @@
     for _ in range(1, 10_001):
         value, NN = update(NN, x, y)
 
     np.testing.assert_allclose(value, jnp.array(0.0031012), atol=1e-5)
 
 
 def test_freeze_nondiff():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Linear:
+    class Linear(pytc.TreeClass, leafwise=True):
         weight: jax.Array
         bias: jax.Array
         count: int
         use_bias: bool
 
         def __init__(self, key, in_dim, out_dim):
             self.weight = jr.normal(key, shape=(in_dim, out_dim)) * jnp.sqrt(2 / in_dim)
             self.bias = jnp.ones((1, out_dim))
             self.use_bias = True
             self.count = 0
 
         def __call__(self, x):
             return x @ self.weight + self.bias
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class StackedLinear:
+    class StackedLinear(pytc.TreeClass, leafwise=True):
         name: str
         exact_array: jax.Array
         bool_array: jax.Array
 
         def __init__(self, key, in_dim, out_dim, hidden_dim):
             self.name = "stack"
             self.exact_array = jnp.array([1, 2, 3])
```

### Comparing `pytreeclass-0.2.8/tests/test_tree_freeze.py` & `pytreeclass-0.3.0/tests/test_tree_freeze.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-import functools as ft
 from typing import Any, Callable
 
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import pytest
 
 import pytreeclass as pytc
 from pytreeclass._src.tree_freeze import _HashableWrapper, tree_hash
 
 
 def test_freeze_unfreeze():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class A:
+    class A(pytc.TreeClass, leafwise=True):
         a: int
         b: int
 
     a = A(1, 2)
     b = a.at[...].apply(pytc.freeze)
     c = (
         a.at["a"]
@@ -27,26 +25,23 @@
 
     assert jtu.tree_leaves(a) == [1, 2]
     assert jtu.tree_leaves(b) == []
     assert jtu.tree_leaves(c) == [1, 2]
 
     assert pytc.unfreeze(pytc.freeze(1.0)) == 1.0
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class A:
+    class A(pytc.TreeClass, leafwise=True):
         a: int
         b: int
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class B:
+    class B(pytc.TreeClass, leafwise=True):
         c: int = 3
         d: A = A(1, 2)
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class A:
+    class A(pytc.TreeClass, leafwise=True):
         a: int
         b: int
 
     a = A(1, 2)
     b = jtu.tree_map(pytc.freeze, a)
     c = (
         a.at["a"]
@@ -55,79 +50,70 @@
         .apply(pytc.unfreeze, is_leaf=pytc.is_frozen)
     )
 
     assert jtu.tree_leaves(a) == [1, 2]
     assert jtu.tree_leaves(b) == []
     assert jtu.tree_leaves(c) == [1, 2]
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class l0:
+    class l0(pytc.TreeClass, leafwise=True):
         a: int = 0
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class l1:
+    class l1(pytc.TreeClass, leafwise=True):
         b: l0 = l0()
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class l2:
+    class l2(pytc.TreeClass, leafwise=True):
         c: l1 = l1()
 
     t = jtu.tree_map(pytc.freeze, l2())
 
     assert jtu.tree_leaves(t) == []
     assert jtu.tree_leaves(t.c) == []
     assert jtu.tree_leaves(t.c.b) == []
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class l1:
+    class l1(pytc.TreeClass, leafwise=True):
         def __init__(self):
             self.b = l0()
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class l2:
+    class l2(pytc.TreeClass, leafwise=True):
         def __init__(self):
             self.c = l1()
 
     t = jtu.tree_map(pytc.freeze, l2())
     assert jtu.tree_leaves(t.c) == []
     assert jtu.tree_leaves(t.c.b) == []
 
 
 def test_freeze_errors():
     class T:
         pass
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Test:
+    class Test(pytc.TreeClass, leafwise=True):
         a: Any
 
     t = Test(T())
 
     # with pytest.raises(Exception):
     t.at[...].set(0)
 
     with pytest.raises(TypeError):
         t.at[...].apply(jnp.sin)
 
     t.at[...].reduce(jnp.sin)
 
 
 def test_freeze_with_ops():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class A:
+    class A(pytc.TreeClass, leafwise=True):
         a: int
         b: int
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class B:
+    class B(pytc.TreeClass, leafwise=True):
         c: int = 3
         d: A = A(1, 2)
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Test:
+    class Test(pytc.TreeClass, leafwise=True):
         a: int = 1
         b: float = pytc.freeze(1.0)
         c: str = pytc.freeze("test")
 
     t = Test()
     assert jtu.tree_leaves(t) == [1]
 
@@ -139,120 +125,108 @@
 
     hash(t)
 
     t = Test()
     jtu.tree_map(pytc.unfreeze, t, is_leaf=pytc.is_frozen)
     jtu.tree_map(pytc.freeze, t)
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Test:
+    class Test(pytc.TreeClass, leafwise=True):
         a: int
 
     t = jtu.tree_map(pytc.freeze, (Test(100)))
 
     assert pytc.is_tree_equal(t.at[...].set(0), t)
     assert pytc.is_tree_equal(t.at[...].apply(lambda x: x + 1), t)
     assert pytc.is_tree_equal(t.at[...].reduce(jnp.sin, initializer=0), 0.0)
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Test:
+    class Test(pytc.TreeClass, leafwise=True):
         x: jnp.ndarray
 
         def __init__(self, x):
             self.x = x
 
     t = Test(jnp.array([1, 2, 3]))
     assert pytc.is_tree_equal(t.at[...].set(None), Test(x=None))
 
-    @ft.partial(pytc.treeclass, leafwise=True)
     class t0:
         a: int = 1
 
-    @ft.partial(pytc.treeclass, leafwise=True)
     class t1:
         a: int = t0()
 
     t = t1()
 
 
 def test_freeze_diagram():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class A:
+    class A(pytc.TreeClass, leafwise=True):
         a: int
         b: int
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class B:
+    class B(pytc.TreeClass, leafwise=True):
         c: int = 3
         d: A = A(1, 2)
 
     a = B()
     a = a.at["d"].set(pytc.freeze(a.d))
     a = B()
 
     a = a.at["d"].set(pytc.freeze(a.d))  # = a.d.freeze()
 
 
 def test_freeze_mask():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Test:
+    class Test(pytc.TreeClass, leafwise=True):
         a: int = 1
         b: int = 2
         c: float = 3.0
 
     t = Test()
 
     assert jtu.tree_leaves(jtu.tree_map(pytc.freeze, t)) == []
 
 
 def test_freeze_nondiff():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Test:
+    class Test(pytc.TreeClass, leafwise=True):
         a: int = pytc.freeze(1)
         b: str = "a"
 
     t = Test()
 
     assert jtu.tree_leaves(t) == ["a"]
     assert jtu.tree_leaves(jtu.tree_map(pytc.freeze, t)) == []
     assert jtu.tree_leaves(
         (jtu.tree_map(pytc.freeze, t))
         .at["b"]
         .apply(pytc.unfreeze, is_leaf=pytc.is_frozen)
     ) == ["a"]
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class T0:
+    class T0(pytc.TreeClass, leafwise=True):
         a: Test = Test()
 
     t = T0()
 
     assert jtu.tree_leaves(t) == ["a"]
     assert jtu.tree_leaves(jtu.tree_map(pytc.freeze, t)) == []
 
     assert jtu.tree_leaves(t) == ["a"]
     assert jtu.tree_leaves(jtu.tree_map(pytc.freeze, t)) == []
 
 
 def test_freeze_nondiff_with_mask():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class L0:
+    class L0(pytc.TreeClass, leafwise=True):
         a: int = 1
         b: int = 2
         c: int = 3
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class L1:
+    class L1(pytc.TreeClass, leafwise=True):
         a: int = 1
         b: int = 2
         c: int = 3
         d: L0 = L0()
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class L2:
+    class L2(pytc.TreeClass, leafwise=True):
         a: int = 10
         b: int = 20
         c: int = 30
         d: L1 = L1()
 
     t = L2()
     t = t.at["d"].at["d"].at["a"].apply(pytc.freeze)
@@ -262,21 +236,19 @@
 
 
 def test_non_dataclass_input_to_freeze():
     assert jtu.tree_leaves(pytc.freeze(1)) == []
 
 
 def test_tree_freeze():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class l0:
+    class l0(pytc.TreeClass, leafwise=True):
         x: int = 2
         y: int = 3
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class l1:
+    class l1(pytc.TreeClass, leafwise=True):
         a: int = 1
         b: l0 = l0()
 
     tree = l1()
 
     assert jtu.tree_leaves(tree) == [1, 2, 3]
     assert jtu.tree_leaves(jtu.tree_map(pytc.freeze, tree)) == []
@@ -289,21 +261,19 @@
     assert jtu.tree_leaves(tree.at["a"].apply(pytc.freeze)) == [2, 3]
     assert jtu.tree_leaves(tree.at["b"].apply(pytc.freeze)) == [1]
     assert jtu.tree_leaves(tree.at["b"].at["x"].apply(pytc.freeze)) == [1, 3]
     assert jtu.tree_leaves(tree.at["b"].at["y"].apply(pytc.freeze)) == [1, 2]
 
 
 def test_tree_unfreeze():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class l0:
+    class l0(pytc.TreeClass, leafwise=True):
         x: int = 2
         y: int = 3
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class l1:
+    class l1(pytc.TreeClass, leafwise=True):
         a: int = 1
         b: l0 = l0()
 
     tree = l1()
 
     frozen_tree = tree.at[...].apply(pytc.freeze)
     assert jtu.tree_leaves(frozen_tree) == []
@@ -320,21 +290,19 @@
     assert jtu.tree_leaves(unfrozen_tree) == [1]
 
     unfrozen_tree = frozen_tree.at["b"].apply(pytc.unfreeze, is_leaf=pytc.is_frozen)  # fmt: skip
     assert jtu.tree_leaves(unfrozen_tree) == [2, 3]
 
 
 def test_tree_freeze_unfreeze():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class l0:
+    class l0(pytc.TreeClass, leafwise=True):
         x: int = 2
         y: int = 3
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class l1:
+    class l1(pytc.TreeClass, leafwise=True):
         a: int = 1
         b: l0 = l0()
 
     tree = l1()
 
     mask = tree == tree
     frozen_tree = tree.at[...].apply(pytc.freeze)
@@ -343,16 +311,15 @@
 
     frozen_tree = tree.at["a"].apply(pytc.freeze)
     unfrozen_tree = frozen_tree.at["a"].apply(pytc.unfreeze, is_leaf=pytc.is_frozen)  # fmt: skip
     assert jtu.tree_leaves(unfrozen_tree) == [1, 2, 3]
 
 
 def test_freeze_nondiff_func():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Test:
+    class Test(pytc.TreeClass, leafwise=True):
         a: int = 1.0
         b: int = 2
         c: int = 3
         act: Callable = jax.nn.tanh
 
         def __call__(self, x):
             return self.act(x + self.a)
```

### Comparing `pytreeclass-0.2.8/tests/test_tree_operator.py` & `pytreeclass-0.3.0/tests/test_tree_operator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from __future__ import annotations
 
-import functools as ft
 import math
 
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import pytest
 
 import pytreeclass as pytc
 from pytreeclass._src.tree_freeze import _hash_node
 from pytreeclass._src.tree_indexer import bcmap
 
 
 def test_bcmap():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Test:
+    class Test(pytc.TreeClass, leafwise=True):
         a: tuple[int]
         b: tuple[int]
         c: jnp.ndarray
         d: int
 
         def __init__(self, a=(1, 2, 3), b=(4, 5, 6), c=jnp.array([1, 2, 3]), d=1):
             self.a = a
@@ -43,16 +41,15 @@
     assert pytc.is_tree_equal(lhs, rhs)
 
     lhs = bcmap(jnp.where)(condition=tree > 1, x=0, y=tree)
     assert pytc.is_tree_equal(lhs, rhs)
 
 
 def test_math_operations():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Test:
+    class Test(pytc.TreeClass, leafwise=True):
         a: float
         b: float
         c: float
         name: str
 
         def __post_init__(self):
             self.name = pytc.freeze(self.name)
@@ -62,16 +59,15 @@
 
     assert (A + A) == Test(20, 40, 60, ("A"))
     assert (A - A) == Test(0, 0, 0, ("A"))
     # assert ((A["a"] + A) | A) == Test(20, 20, 30, ("A"))
     assert A.at[...].reduce(lambda x, y: x + jnp.sum(y)) == jnp.array(60)
     assert abs(A) == A
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Test:
+    class Test(pytc.TreeClass, leafwise=True):
         a: float
         b: float
         name: str
 
         def __post_init__(self):
             self.name = pytc.freeze(self.name)
 
@@ -110,16 +106,15 @@
     assert A**A == Test(-(10**-10), 20**20, ("A"))
     assert round(A) == Test(round(-10), round(20), ("A"))
     assert A - A == Test(-10 + 10, 20 - 20, ("A"))
     assert A ^ A == Test(-10 ^ -10, 20 ^ 20, ("A"))
 
 
 def test_math_operations_errors():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Test:
+    class Test(pytc.TreeClass, leafwise=True):
         a: float
         b: float
         c: float
         name: str
         d: jnp.ndarray = None
 
         def __post_init__(self):
```

### Comparing `pytreeclass-0.2.8/tests/test_tree_pprint.py` & `pytreeclass-0.3.0/tests/test_tree_pprint.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 from __future__ import annotations
 
 import dataclasses as dc
-import functools as ft
 from collections import namedtuple
 
 # import jax
 import jax.tree_util as jtu
 import pytest
 from jax import numpy as jnp
 
 import pytreeclass as pytc
 from pytreeclass import (
+    TreeClass,
     tree_diagram,
     tree_indent,
     tree_mermaid,
     tree_repr,
     tree_repr_with_trace,
     tree_str,
     tree_summary,
 )
 
 
-@ft.partial(pytc.treeclass, leafwise=True)
-class Repr1:
+class Repr1(TreeClass, leafwise=True):
     a: int = 1
     b: str = "string"
     c: float = 1.0
     d: tuple = "a" * 5
     e: list = None
     f: set = None
     g: dict = None
@@ -52,21 +51,21 @@
 r1 = Repr1()
 
 
 def test_repr():
     assert (
         tree_repr(r1)
         # trunk-ignore(flake8/E501)
-        == "Repr1(\n  a=1, \n  b='string', \n  c=1.0, \n  d='aaaaa', \n  e=[10, 10, 10, 10, 10], \n  f={1, 2, 3}, \n  g={\n    a:'aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa', \n    b:'bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb', \n    c:f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])\n  }, \n  h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  l=a(b=1, c=2), \n  m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  n=bool[0], \n  o=c64[2]\n)"
+        == "Repr1(\n  a=1, \n  b='string', \n  c=1.0, \n  d='aaaaa', \n  e=[10, 10, 10, 10, 10], \n  f={1, 2, 3}, \n  g={\n    a:'aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa', \n    b:'bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb', \n    c:f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])\n  }, \n  h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  l=a(b=1, c=2), \n  m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  n=bool[], \n  o=c64[2]\n)"
     )
 
     assert (
         tree_repr(r1, depth=1)
         # trunk-ignore(flake8/E501)
-        == "Repr1(\n  a=1, \n  b='string', \n  c=1.0, \n  d='aaaaa', \n  e=[...], \n  f={...}, \n  g={...}, \n  h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  l=a(...), \n  m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  n=bool[0], \n  o=c64[2]\n)"
+        == "Repr1(\n  a=1, \n  b='string', \n  c=1.0, \n  d='aaaaa', \n  e=[...], \n  f={...}, \n  g={...}, \n  h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  l=a(...), \n  m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  n=bool[], \n  o=c64[2]\n)"
     )
 
     assert tree_repr(r1, depth=0) == "Repr1(...)"
 
 
 def test_str():
     assert (
@@ -87,34 +86,34 @@
         tree_summary(r1, depth=0)
         == "┌────┬─────┬─────┐\n│Name│Type │Count│\n├────┼─────┼─────┤\n│Σ   │Repr1│1    │\n└────┴─────┴─────┘"
     )
 
     assert (
         tree_summary(r1, depth=1)
         # trunk-ignore(flake8/E501)
-        == "┌────┬────────────┬─────┐\n│Name│Type        │Count│\n├────┼────────────┼─────┤\n│a   │int         │1    │\n├────┼────────────┼─────┤\n│b   │str         │1    │\n├────┼────────────┼─────┤\n│c   │float       │1    │\n├────┼────────────┼─────┤\n│d   │str         │1    │\n├────┼────────────┼─────┤\n│e   │list        │1    │\n├────┼────────────┼─────┤\n│f   │set         │1    │\n├────┼────────────┼─────┤\n│g   │dict        │1    │\n├────┼────────────┼─────┤\n│h   │f32[5,1]    │5    │\n├────┼────────────┼─────┤\n│i   │f32[1,6]    │6    │\n├────┼────────────┼─────┤\n│j   │f32[1,1,4,5]│20   │\n├────┼────────────┼─────┤\n│k   │tuple       │1    │\n├────┼────────────┼─────┤\n│l   │a           │1    │\n├────┼────────────┼─────┤\n│m   │f32[5,5]    │25   │\n├────┼────────────┼─────┤\n│n   │bool[0]     │1    │\n├────┼────────────┼─────┤\n│o   │c64[2]      │2    │\n├────┼────────────┼─────┤\n│Σ   │Repr1       │68   │\n└────┴────────────┴─────┘"
+        == "┌────┬────────────┬─────┐\n│Name│Type        │Count│\n├────┼────────────┼─────┤\n│a   │int         │1    │\n├────┼────────────┼─────┤\n│b   │str         │1    │\n├────┼────────────┼─────┤\n│c   │float       │1    │\n├────┼────────────┼─────┤\n│d   │str         │1    │\n├────┼────────────┼─────┤\n│e   │list        │1    │\n├────┼────────────┼─────┤\n│f   │set         │1    │\n├────┼────────────┼─────┤\n│g   │dict        │1    │\n├────┼────────────┼─────┤\n│h   │f32[5,1]    │5    │\n├────┼────────────┼─────┤\n│i   │f32[1,6]    │6    │\n├────┼────────────┼─────┤\n│j   │f32[1,1,4,5]│20   │\n├────┼────────────┼─────┤\n│k   │tuple       │1    │\n├────┼────────────┼─────┤\n│l   │a           │1    │\n├────┼────────────┼─────┤\n│m   │f32[5,5]    │25   │\n├────┼────────────┼─────┤\n│n   │bool[]      │1    │\n├────┼────────────┼─────┤\n│o   │c64[2]      │2    │\n├────┼────────────┼─────┤\n│Σ   │Repr1       │68   │\n└────┴────────────┴─────┘"
     )
 
     assert (
         tree_summary(r1, depth=2)
         == tree_summary(r1)
         # trunk-ignore(flake8/E501)
-        == "┌──────┬────────────┬─────┐\n│Name  │Type        │Count│\n├──────┼────────────┼─────┤\n│a     │int         │1    │\n├──────┼────────────┼─────┤\n│b     │str         │1    │\n├──────┼────────────┼─────┤\n│c     │float       │1    │\n├──────┼────────────┼─────┤\n│d     │str         │1    │\n├──────┼────────────┼─────┤\n│e[0]  │int         │1    │\n├──────┼────────────┼─────┤\n│e[1]  │int         │1    │\n├──────┼────────────┼─────┤\n│e[2]  │int         │1    │\n├──────┼────────────┼─────┤\n│e[3]  │int         │1    │\n├──────┼────────────┼─────┤\n│e[4]  │int         │1    │\n├──────┼────────────┼─────┤\n│f     │set         │1    │\n├──────┼────────────┼─────┤\n│g['a']│str         │1    │\n├──────┼────────────┼─────┤\n│g['b']│str         │1    │\n├──────┼────────────┼─────┤\n│g['c']│f32[5,5]    │25   │\n├──────┼────────────┼─────┤\n│h     │f32[5,1]    │5    │\n├──────┼────────────┼─────┤\n│i     │f32[1,6]    │6    │\n├──────┼────────────┼─────┤\n│j     │f32[1,1,4,5]│20   │\n├──────┼────────────┼─────┤\n│k[0]  │int         │1    │\n├──────┼────────────┼─────┤\n│k[1]  │int         │1    │\n├──────┼────────────┼─────┤\n│k[2]  │int         │1    │\n├──────┼────────────┼─────┤\n│l.b   │int         │1    │\n├──────┼────────────┼─────┤\n│l.c   │int         │1    │\n├──────┼────────────┼─────┤\n│m     │f32[5,5]    │25   │\n├──────┼────────────┼─────┤\n│n     │bool[0]     │1    │\n├──────┼────────────┼─────┤\n│o     │c64[2]      │2    │\n├──────┼────────────┼─────┤\n│Σ     │Repr1       │101  │\n└──────┴────────────┴─────┘"
+        == "┌──────┬────────────┬─────┐\n│Name  │Type        │Count│\n├──────┼────────────┼─────┤\n│a     │int         │1    │\n├──────┼────────────┼─────┤\n│b     │str         │1    │\n├──────┼────────────┼─────┤\n│c     │float       │1    │\n├──────┼────────────┼─────┤\n│d     │str         │1    │\n├──────┼────────────┼─────┤\n│e[0]  │int         │1    │\n├──────┼────────────┼─────┤\n│e[1]  │int         │1    │\n├──────┼────────────┼─────┤\n│e[2]  │int         │1    │\n├──────┼────────────┼─────┤\n│e[3]  │int         │1    │\n├──────┼────────────┼─────┤\n│e[4]  │int         │1    │\n├──────┼────────────┼─────┤\n│f     │set         │1    │\n├──────┼────────────┼─────┤\n│g['a']│str         │1    │\n├──────┼────────────┼─────┤\n│g['b']│str         │1    │\n├──────┼────────────┼─────┤\n│g['c']│f32[5,5]    │25   │\n├──────┼────────────┼─────┤\n│h     │f32[5,1]    │5    │\n├──────┼────────────┼─────┤\n│i     │f32[1,6]    │6    │\n├──────┼────────────┼─────┤\n│j     │f32[1,1,4,5]│20   │\n├──────┼────────────┼─────┤\n│k[0]  │int         │1    │\n├──────┼────────────┼─────┤\n│k[1]  │int         │1    │\n├──────┼────────────┼─────┤\n│k[2]  │int         │1    │\n├──────┼────────────┼─────┤\n│l.b   │int         │1    │\n├──────┼────────────┼─────┤\n│l.c   │int         │1    │\n├──────┼────────────┼─────┤\n│m     │f32[5,5]    │25   │\n├──────┼────────────┼─────┤\n│n     │bool[]      │1    │\n├──────┼────────────┼─────┤\n│o     │c64[2]      │2    │\n├──────┼────────────┼─────┤\n│Σ     │Repr1       │101  │\n└──────┴────────────┴─────┘"
     )
 
 
 def _tree_to_indent(str):
     return str.replace("├── ", "    ").replace("└── ", "    ").replace("│", " ")
 
 
 def test_tree_diagram():
     assert tree_diagram(r1, depth=0) == tree_indent(r1, depth=0) == "Repr1"
 
     # trunk-ignore(flake8/E501)
-    out = "Repr1\n├── a=1\n├── b='string'\n├── c=1.0\n├── d='aaaaa'\n├── e=[...]\n├── f={...}\n├── g={...}\n├── h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── k=(...)\n├── l=a(...)\n├── m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── n=bool[0]\n└── o=c64[2]"
+    out = "Repr1\n├── a=1\n├── b='string'\n├── c=1.0\n├── d='aaaaa'\n├── e=[...]\n├── f={...}\n├── g={...}\n├── h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── k=(...)\n├── l=a(...)\n├── m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── n=bool[]\n└── o=c64[2]"
 
     assert tree_diagram(r1, depth=1) == out
     assert tree_indent(r1, depth=1) == _tree_to_indent(out)
 
 
 def test_custom_jax_class():
     @jtu.register_pytree_node_class
@@ -147,20 +146,20 @@
     assert tree_str(Test) == str(Test)
 
 
 def test_tree_mermaid():
     assert (
         tree_mermaid(r1, depth=1)
         # trunk-ignore(flake8/E501)
-        == 'flowchart LR\n    id0(<b>Repr1</b>)\n    id0 --- id1("</b>a=1</b>")\n    id0 --- id2("</b>b=\'string\'</b>")\n    id0 --- id3("</b>c=1.0</b>")\n    id0 --- id4("</b>d=\'aaaaa\'</b>")\n    id0 --- id5("</b>e=[...]</b>")\n    id0 --- id6("</b>f={...}</b>")\n    id0 --- id7("</b>g={...}</b>")\n    id0 --- id8("</b>h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id9("</b>i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id10("</b>j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id11("</b>k=(...)</b>")\n    id0 --- id12("</b>l=a(...)</b>")\n    id0 --- id13("</b>m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id14("</b>n=bool[0]</b>")\n    id0 --- id15("</b>o=c64[2]</b>")\n'
+        == 'flowchart LR\n    id0(<b>Repr1</b>)\n    id0 --- id1("</b>a=1</b>")\n    id0 --- id2("</b>b=\'string\'</b>")\n    id0 --- id3("</b>c=1.0</b>")\n    id0 --- id4("</b>d=\'aaaaa\'</b>")\n    id0 --- id5("</b>e=[...]</b>")\n    id0 --- id6("</b>f={...}</b>")\n    id0 --- id7("</b>g={...}</b>")\n    id0 --- id8("</b>h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id9("</b>i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id10("</b>j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id11("</b>k=(...)</b>")\n    id0 --- id12("</b>l=a(...)</b>")\n    id0 --- id13("</b>m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id14("</b>n=bool[]</b>")\n    id0 --- id15("</b>o=c64[2]</b>")\n'
     )
     assert (
         tree_mermaid(r1, depth=2)
         # trunk-ignore(flake8/E501)
-        == 'flowchart LR\n    id5 --- id6("</b>[0]=10</b>")\n    id5 --- id7("</b>[1]=10</b>")\n    id5 --- id8("</b>[2]=10</b>")\n    id5 --- id9("</b>[3]=10</b>")\n    id5 --- id10("</b>[4]=10</b>")\n    id12 --- id13("</b>[\'a\']=\'aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa\'</b>")\n    id12 --- id14("</b>[\'b\']=\'bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb\'</b>")\n    id12 --- id15("</b>[\'c\']=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id19 --- id20("</b>[0]=1</b>")\n    id19 --- id21("</b>[1]=2</b>")\n    id19 --- id22("</b>[2]=3</b>")\n    id23 --- id24("</b>b=1</b>")\n    id23 --- id25("</b>c=2</b>")\n    id0(<b>Repr1</b>)\n    id0 --- id1("</b>a=1</b>")\n    id0 --- id2("</b>b=\'string\'</b>")\n    id0 --- id3("</b>c=1.0</b>")\n    id0 --- id4("</b>d=\'aaaaa\'</b>")\n    id0 --- id5("</b>e:list</b>")\n    id0 --- id11("</b>f={1, 2, 3}</b>")\n    id0 --- id12("</b>g:dict</b>")\n    id0 --- id16("</b>h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id17("</b>i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id18("</b>j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id19("</b>k:tuple</b>")\n    id0 --- id23("</b>l:a</b>")\n    id0 --- id26("</b>m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id27("</b>n=bool[0]</b>")\n    id0 --- id28("</b>o=c64[2]</b>")\n'
+        == 'flowchart LR\n    id5 --- id6("</b>[0]=10</b>")\n    id5 --- id7("</b>[1]=10</b>")\n    id5 --- id8("</b>[2]=10</b>")\n    id5 --- id9("</b>[3]=10</b>")\n    id5 --- id10("</b>[4]=10</b>")\n    id12 --- id13("</b>[\'a\']=\'aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa\'</b>")\n    id12 --- id14("</b>[\'b\']=\'bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb\'</b>")\n    id12 --- id15("</b>[\'c\']=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id19 --- id20("</b>[0]=1</b>")\n    id19 --- id21("</b>[1]=2</b>")\n    id19 --- id22("</b>[2]=3</b>")\n    id23 --- id24("</b>b=1</b>")\n    id23 --- id25("</b>c=2</b>")\n    id0(<b>Repr1</b>)\n    id0 --- id1("</b>a=1</b>")\n    id0 --- id2("</b>b=\'string\'</b>")\n    id0 --- id3("</b>c=1.0</b>")\n    id0 --- id4("</b>d=\'aaaaa\'</b>")\n    id0 --- id5("</b>e:list</b>")\n    id0 --- id11("</b>f={1, 2, 3}</b>")\n    id0 --- id12("</b>g:dict</b>")\n    id0 --- id16("</b>h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id17("</b>i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id18("</b>j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id19("</b>k:tuple</b>")\n    id0 --- id23("</b>l:a</b>")\n    id0 --- id26("</b>m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id27("</b>n=bool[]</b>")\n    id0 --- id28("</b>o=c64[2]</b>")\n'
     )
 
 
 def test_misc():
     x = (1, 2, 3)
     assert tree_repr(x) == tree_str(x) == "(1, 2, 3)"
 
@@ -185,45 +184,40 @@
         a: int = 1
 
     assert pytc.tree_repr(Test()) == pytc.tree_str(Test()) == "Test(a=1)"
     assert pytc.tree_repr(Test(), depth=0) == "Test(...)"
 
 
 def test_extra_tree_diagram():
-    @pytc.treeclass
-    class L0:
+    class L0(TreeClass):
         a: int = 1
         b: int = 2
 
-    @pytc.treeclass
-    class L1:
+    class L1(TreeClass):
         c: L0 = L0()
         d: int = 3
 
-    @pytc.treeclass
-    class L2:
+    class L2(TreeClass):
         e: int = 4
         f: L1 = L1()
         g: L0 = L0()
         h: int = 5
 
     tree = L2()
     # trunk-ignore(flake8/E501)
     out = "L2\n├── e=4\n├── f:L1\n│   ├── c:L0\n│   │   ├── a=1\n│   │   └── b=2\n│   └── d=3\n├── g:L0\n│   ├── a=1\n│   └── b=2\n└── h=5"
 
     assert (tree_diagram(tree)) == out
 
     assert tree_indent(tree) == _tree_to_indent(out)
 
-    @pytc.treeclass
-    class L0:
+    class L0(TreeClass):
         a: int = 1
 
-    @pytc.treeclass
-    class L1:
+    class L1(TreeClass):
         b: L0 = L0()
 
     tree = L1()
 
     assert tree_diagram(tree) == "L1\n└── b:L0\n    └── a=1"
 
 
@@ -233,16 +227,15 @@
     with pytest.raises(TypeError):
         tree_summary(1, depth="a")
     with pytest.raises(TypeError):
         tree_mermaid(1, depth="a")
 
 
 def test_tree_repr_with_trace():
-    @pytc.treeclass
-    class Test:
+    class Test(TreeClass, leafwise=True):
         a: int = 1
         b: float = 2.0
 
     tree = Test()
 
     assert (
         str(tree_repr_with_trace(tree))
```

### Comparing `pytreeclass-0.2.8/tests/test_tree_viz_util.py` & `pytreeclass-0.3.0/tests/test_tree_viz_util.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.2.8/tests/test_under_jit.py` & `pytreeclass-0.3.0/tests/test_under_jit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,33 @@
-import functools as ft
-
 import jax
 import jax.tree_util as jtu
 import numpy.testing as npt
 import pytest
 from jax import numpy as jnp
 
 import pytreeclass as pytc
 
 
 def test_jit_freeze():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Linear:
+    class Linear(pytc.TreeClass, leafwise=True):
         weight: jax.Array
         bias: jax.Array
         name: str
 
         def __init__(self, key, in_dim, out_dim):
             self.weight = jax.random.normal(key, shape=(in_dim, out_dim)) * jnp.sqrt(
                 2 / in_dim
             )
             self.bias = jnp.ones((1, out_dim))
             self.name = pytc.freeze("a")
 
         def __call__(self, x):
             return x @ self.weight + self.bias
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class StackedLinear:
+    class StackedLinear(pytc.TreeClass, leafwise=True):
         l1: Linear
         l2: Linear
         l3: Linear
 
         def __init__(self, key, in_dim, out_dim, hidden_dim):
             keys = jax.random.split(key, 3)
             self.l1 = Linear(key=keys[0], in_dim=in_dim, out_dim=hidden_dim)
@@ -103,22 +99,20 @@
         return value, model
 
     for _ in range(2):
         value, model = train_step(x, y, epochs=20_000)
 
 
 def test_ops_with_jit():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class T0:
+    class T0(pytc.TreeClass, leafwise=True):
         a: jax.Array = jnp.array(1)
         b: jax.Array = jnp.array(2)
         c: jax.Array = jnp.array(3)
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class T1:
+    class T1(pytc.TreeClass, leafwise=True):
         a: jax.Array = jnp.array(1)
         b: jax.Array = jnp.array(2)
         c: jax.Array = jnp.array(3)
         d: jax.Array = jnp.array([1, 2, 3])
 
     @jax.jit
     def getter(tree):
```

