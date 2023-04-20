# Comparing `tmp/eulerpi-0.1.5.tar.gz` & `tmp/eulerpi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eulerpi-0.1.5.tar", max compression
+gzip compressed data, was "eulerpi-0.2.0.tar", max compression
```

## Comparing `eulerpi-0.1.5.tar` & `eulerpi-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,39 @@
--rw-r--r--   0        0        0     1117 2023-03-14 21:09:11.591241 eulerpi-0.1.5/LICENSE.md
--rw-r--r--   0        0        0     4622 2023-04-06 17:27:03.192999 eulerpi-0.1.5/README.md
--rw-r--r--   0        0        0      564 2023-03-14 21:09:11.599241 eulerpi-0.1.5/eulerpi/__init__.py
--rw-r--r--   0        0        0      191 2023-03-14 21:09:11.599241 eulerpi-0.1.5/eulerpi/core/__init__.py
--rw-r--r--   0        0        0    10041 2023-04-06 17:27:03.196999 eulerpi-0.1.5/eulerpi/core/dense_grid.py
--rw-r--r--   0        0        0     4844 2023-04-06 17:27:03.196999 eulerpi-0.1.5/eulerpi/core/inference.py
--rw-r--r--   0        0        0     3684 2023-03-14 21:09:11.599241 eulerpi-0.1.5/eulerpi/core/kde.py
--rw-r--r--   0        0        0    12491 2023-04-06 17:27:03.196999 eulerpi-0.1.5/eulerpi/core/model.py
--rw-r--r--   0        0        0    10709 2023-04-06 17:27:03.196999 eulerpi-0.1.5/eulerpi/core/result_manager.py
--rw-r--r--   0        0        0    14930 2023-04-06 17:27:03.196999 eulerpi-0.1.5/eulerpi/core/sampling.py
--rw-r--r--   0        0        0    19548 2023-04-06 17:27:03.196999 eulerpi-0.1.5/eulerpi/core/sparsegrid.py
--rw-r--r--   0        0        0     6213 2023-04-06 17:27:03.196999 eulerpi-0.1.5/eulerpi/core/transformations.py
--rw-r--r--   0        0        0    14800 2023-03-14 21:09:11.599241 eulerpi-0.1.5/eulerpi/examples/corona/CoronaData.csv
--rw-r--r--   0        0        0       94 2023-03-14 21:09:11.599241 eulerpi-0.1.5/eulerpi/examples/corona/__init__.py
--rw-r--r--   0        0        0     2483 2023-04-06 17:27:03.196999 eulerpi-0.1.5/eulerpi/examples/corona/corona.py
--rw-r--r--   0        0        0     1295 2023-03-14 21:09:11.599241 eulerpi-0.1.5/eulerpi/examples/cpp/CMakeLists.txt
--rw-r--r--   0        0        0        0 2023-03-14 21:09:11.599241 eulerpi-0.1.5/eulerpi/examples/cpp/__init__.py
--rw-r--r--   0        0        0     2214 2023-03-14 21:09:11.599241 eulerpi-0.1.5/eulerpi/examples/cpp/cpp_model.hpp
--rw-r--r--   0        0        0     1191 2023-04-06 17:27:03.196999 eulerpi-0.1.5/eulerpi/examples/cpp/cpp_plant.py
--rw-r--r--   0        0        0     2559 2023-04-06 17:27:03.196999 eulerpi-0.1.5/eulerpi/examples/cpp/python_reference_plants.py
--rw-r--r--   0        0        0      357 2023-03-14 21:09:11.599241 eulerpi-0.1.5/eulerpi/examples/cpp/wrapper.cpp
--rw-r--r--   0        0        0     1811 2023-03-14 21:09:11.599241 eulerpi-0.1.5/eulerpi/examples/sbml/Caffeine_2Wks_Exponential_decay.xml
--rw-r--r--   0        0        0     1251 2023-04-06 17:27:03.196999 eulerpi-0.1.5/eulerpi/examples/sbml/sbml_caffeine_model.py
--rw-r--r--   0        0        0     1682 2023-04-06 17:27:03.196999 eulerpi-0.1.5/eulerpi/examples/sbml/sbml_menten_model.py
--rw-r--r--   0        0        0     5493 2023-03-14 21:09:11.599241 eulerpi-0.1.5/eulerpi/examples/sbml/sbml_menten_model.xml
--rw-r--r--   0        0        0     2241 2023-04-06 17:27:03.196999 eulerpi-0.1.5/eulerpi/examples/simple_models.py
--rw-r--r--   0        0        0   189602 2023-03-14 21:09:11.599241 eulerpi-0.1.5/eulerpi/examples/stock/ETF.csv
--rw-r--r--   0        0        0      268 2023-03-14 21:09:11.599241 eulerpi-0.1.5/eulerpi/examples/stock/ETF50.csv
--rw-r--r--   0        0        0       88 2023-03-14 21:09:11.611241 eulerpi-0.1.5/eulerpi/examples/stock/__init__.py
--rw-r--r--   0        0        0     5556 2023-04-06 17:27:03.196999 eulerpi-0.1.5/eulerpi/examples/stock/stock.py
--rw-r--r--   0        0        0     5877 2023-03-14 21:09:11.611241 eulerpi-0.1.5/eulerpi/examples/temperature/TemperatureArtificialParams.csv
--rw-r--r--   0        0        0     5046 2023-03-14 21:09:11.611241 eulerpi-0.1.5/eulerpi/examples/temperature/TemperatureData.csv
--rw-r--r--   0        0        0      215 2023-03-14 21:09:11.611241 eulerpi-0.1.5/eulerpi/examples/temperature/__init__.py
--rw-r--r--   0        0        0     2136 2023-04-06 17:27:03.196999 eulerpi-0.1.5/eulerpi/examples/temperature/temperature.py
--rw-r--r--   0        0        0     2169 2023-03-14 21:09:11.611241 eulerpi-0.1.5/eulerpi/jax_extension.py
--rw-r--r--   0        0        0     2331 2023-04-06 17:29:24.392456 eulerpi-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     6054 1970-01-01 00:00:00.000000 eulerpi-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1117 2023-04-20 21:54:42.257745 eulerpi-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     4634 2023-04-20 21:54:42.257745 eulerpi-0.2.0/README.md
+-rw-r--r--   0        0        0      564 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/__init__.py
+-rw-r--r--   0        0        0      191 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/core/__init__.py
+-rw-r--r--   0        0        0    10754 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/core/dense_grid.py
+-rw-r--r--   0        0        0      355 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/core/dense_grid_types.py
+-rw-r--r--   0        0        0     4609 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/core/inference.py
+-rw-r--r--   0        0        0      514 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/core/inference_types.py
+-rw-r--r--   0        0        0     3684 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/core/kde.py
+-rw-r--r--   0        0        0    15213 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/core/model.py
+-rw-r--r--   0        0        0    17486 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/core/result_manager.py
+-rw-r--r--   0        0        0    17240 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/core/sampling.py
+-rw-r--r--   0        0        0    20662 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/core/sparsegrid.py
+-rw-r--r--   0        0        0     6393 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/core/transformations.py
+-rw-r--r--   0        0        0    14800 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/examples/corona/CoronaData.csv
+-rw-r--r--   0        0        0       94 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/examples/corona/__init__.py
+-rw-r--r--   0        0        0     2767 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/examples/corona/corona.py
+-rw-r--r--   0        0        0     1295 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/examples/cpp/CMakeLists.txt
+-rw-r--r--   0        0        0        0 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/cpp/__init__.py
+-rw-r--r--   0        0        0     2214 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/cpp/cpp_model.hpp
+-rw-r--r--   0        0        0     1191 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/cpp/cpp_plant.py
+-rw-r--r--   0        0        0     2559 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/cpp/python_reference_plants.py
+-rw-r--r--   0        0        0      357 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/cpp/wrapper.cpp
+-rw-r--r--   0        0        0     1811 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/sbml/Caffeine_2Wks_Exponential_decay.xml
+-rw-r--r--   0        0        0     1133 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/sbml/sbml_caffeine_model.py
+-rw-r--r--   0        0        0     1564 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/sbml/sbml_menten_model.py
+-rw-r--r--   0        0        0     5493 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/sbml/sbml_menten_model.xml
+-rw-r--r--   0        0        0     2241 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/simple_models.py
+-rw-r--r--   0        0        0   189602 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/stock/ETF.csv
+-rw-r--r--   0        0        0      268 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/stock/ETF50.csv
+-rw-r--r--   0        0        0       88 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/stock/__init__.py
+-rw-r--r--   0        0        0     5556 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/stock/stock.py
+-rw-r--r--   0        0        0     5877 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/temperature/TemperatureArtificialParams.csv
+-rw-r--r--   0        0        0     5046 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/temperature/TemperatureData.csv
+-rw-r--r--   0        0        0      215 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/temperature/__init__.py
+-rw-r--r--   0        0        0     2136 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/temperature/temperature.py
+-rw-r--r--   0        0        0     2169 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/jax_extension.py
+-rw-r--r--   0        0        0     2344 2023-04-20 21:54:42.269745 eulerpi-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6058 1970-01-01 00:00:00.000000 eulerpi-0.2.0/PKG-INFO
```

### Comparing `eulerpi-0.1.5/LICENSE.md` & `eulerpi-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eulerpi-0.1.5/README.md` & `eulerpi-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 ```bash
 pip install eulerpi
 ```
 
 Make sure that you have the following C++ libraries installed
 
 ```bash
-sudo apt install -y swig libblas-dev libatlas-base-dev
+sudo apt install -y swig libblas-dev libatlas-base-dev libhdf5-dev
 ```
 
 You can also build the library from the latest source code by following the [Development Quickstart Guide](./DEVELOPMENT.md#quickstart).
 
 ## Using the library
 
 To use EPI, derive your model from the `Model` class and implement the abstract functions. Here's an example code snippet:
```

### Comparing `eulerpi-0.1.5/eulerpi/__init__.py` & `eulerpi-0.2.0/eulerpi/__init__.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.1.5/eulerpi/core/dense_grid.py` & `eulerpi-0.2.0/eulerpi/core/dense_grid.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,23 @@
-from enum import Enum
-from multiprocessing import Pool
+import typing
+from itertools import repeat
+from multiprocessing import get_context
 from typing import Dict, Tuple, Union
 
 import numpy as np
 from numpy.polynomial.chebyshev import chebpts1
 
+from eulerpi.core.dense_grid_types import DenseGridType
+from eulerpi.core.inference_types import InferenceType
 from eulerpi.core.model import Model
 from eulerpi.core.result_manager import ResultManager
 from eulerpi.core.sampling import calc_kernel_width
 from eulerpi.core.transformations import evaluate_density
 
 
-class DenseGridType(Enum):
-    """The type of grid to be used."""
-
-    EQUIDISTANT = 0  #: The equidistant grid has the same distance between two grid points in each dimension.
-    CHEBYSHEV = 1  #: The Chebyshev grid is a tensor product of Chebyshev polynomial roots. They are optimal for polynomial interpolation and quadrature.
-
-
 def generate_chebyshev_grid(
     num_grid_points: np.ndarray, limits: np.ndarray, flatten=False
 ) -> Union[np.ndarray, list[np.ndarray]]:
     """Generate a grid with the given number of grid points for each dimension.
 
     Args:
         num_grid_points(np.ndarray): The number of grid points for each dimension.
@@ -67,14 +63,44 @@
     mesh = np.meshgrid(*axes, indexing="ij")
     if flatten:
         return np.array(mesh).reshape(ndim, -1).T
     else:
         return mesh
 
 
+def evaluate_on_grid_chunk(
+    args: typing.Tuple[np.ndarray, Model, np.ndarray, np.ndarray, np.ndarray]
+) -> np.ndarray:
+    """Define a function which evaluates the density for a given grid chunk. The input args contains the grid chunk, the model, the data, the data_stdevs and the slice.
+
+    Args:
+        grid_chunk(np.ndarray): The grid chunk contains the grid points (parameter vectors) for which the density should be evaluated.
+        model(Model): The model used for the inference.
+        data(np.ndarray): The data points used for the inference.
+        data_stdevs(np.ndarray): The standard deviations of the data points. (Currently the kernel width, #TODO!)
+        slice(np.ndarray): The slice defines for which dimensions of the grid points / paramater vectors the marginal density should be evaluated.
+
+    Returns:
+        np.ndarray: The evaluation results for the given grid chunk. It is a vector, containing the parameters in the first columns, the simulation results in the second columns and the density evaluations in the last columns.
+    """
+    grid_chunk, model, data, data_stdevs, slice = args
+
+    # Init the result array
+    evaluation_results = np.zeros(
+        (grid_chunk.shape[0], data.shape[1] + slice.shape[0] + 1)
+    )
+    # Evaluate the grid points
+    for i, gridPoint in enumerate(grid_chunk):
+        density, param_sim_res_density = evaluate_density(
+            gridPoint, model, data, data_stdevs, slice
+        )
+        evaluation_results[i] = param_sim_res_density
+    return evaluation_results
+
+
 def run_dense_grid_evaluation(
     model: Model,
     data: np.ndarray,
     slice: np.ndarray,
     result_manager: ResultManager,
     num_grid_points: np.ndarray,
     dense_grid_type: DenseGridType,
@@ -119,50 +145,27 @@
     else:
         raise ValueError(f"Unknown grid type: {dense_grid_type}")
 
     # Split the grid into chunks that can be evaluated by each process
     grid_chunks = np.array_split(
         grid, num_processes * load_balancing_safety_faktor
     )
-    # Calc cumsum for indexing
-    grid_chunks_cumsum = np.cumsum(
-        [0] + [grid_chunk.shape[0] for grid_chunk in grid_chunks]
-    )
-    # Define a function which evaluates the density for a given grid chunk
-    global evaluate_on_grid_chunk  # Needed to make this function pickleable
-
-    def evaluate_on_grid_chunk(args):
-        grid_chunk, model, data, data_stdevs, slice = args
-        # Init the result array
-        evaluation_results = np.zeros(
-            (grid_chunk.shape[0], data.shape[1] + slice.shape[0] + 1)
-        )
-        # Evaluate the grid points
-        for i, gridPoint in enumerate(grid_chunk):
-            density, param_sim_res_density = evaluate_density(
-                gridPoint, model, data, data_stdevs, slice
-            )
-            evaluation_results[i] = param_sim_res_density
-        return evaluation_results
-
-    pool = Pool(processes=num_processes)
-    results = np.zeros((grid.shape[0], data.shape[1] + slice.shape[0] + 1))
-    for i, result in enumerate(
-        pool.imap(
-            evaluate_on_grid_chunk,
-            [
-                (grid_chunks[i], model, data, data_stdevs, slice)
-                for i in range(len(grid_chunks))
-            ],
-        )
-    ):
-        results[grid_chunks_cumsum[i] : grid_chunks_cumsum[i + 1]] = result
 
+    pool = get_context("spawn").Pool(processes=num_processes)
+    tasks = zip(
+        grid_chunks,
+        repeat(model),
+        repeat(data),
+        repeat(data_stdevs),
+        repeat(slice),
+    )
+    results = pool.map(evaluate_on_grid_chunk, tasks)
     pool.close()
     pool.join()
+    results = np.concatenate(results)
 
     result_manager.save_overall(
         slice,
         results[:, 0 : slice.shape[0]],
         results[:, slice.shape[0] : slice.shape[0] + data.shape[1]],
         results[:, slice.shape[0] + data.shape[1] :],
     )
@@ -233,13 +236,22 @@
             slice=slice,
             result_manager=result_manager,
             num_grid_points=n_points,
             dense_grid_type=dense_grid_type,
             num_processes=num_processes,
             load_balancing_safety_faktor=load_balancing_safety_faktor,
         )
+        result_manager.save_inference_information(
+            slice=slice,
+            model=model,
+            inference_type=InferenceType.DENSE_GRID,
+            num_processes=num_processes,
+            load_balancing_safety_faktor=load_balancing_safety_faktor,
+            num_grid_points=n_points,
+            dense_grid_type=dense_grid_type,
+        )
     return (
         overall_params,
         overall_sim_results,
         overall_density_evals,
         result_manager,
     )
```

### Comparing `eulerpi-0.1.5/eulerpi/core/inference.py` & `eulerpi-0.2.0/eulerpi/core/inference.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,22 @@
 import os
 import pathlib
-from enum import Enum
 from typing import Dict, Optional, Tuple, Union
 
 import jax.numpy as jnp
 import numpy as np
 
 from eulerpi.core.dense_grid import inference_dense_grid
+from eulerpi.core.inference_types import InferenceType
 from eulerpi.core.model import Model
 from eulerpi.core.result_manager import ResultManager
 from eulerpi.core.sampling import inference_mcmc
 from eulerpi.core.sparsegrid import inference_sparse_grid
 
 
-# Define an enum for the inference types: DenseGrid, MCMC
-class InferenceType(Enum):
-    """The type of inference to be used."""
-
-    DENSE_GRID = 0  #: The dense grid inference uses a dense grid to evaluate the joint distribution.
-    MCMC = 1  #: The MCMC inference uses a Markov Chain Monte Carlo sampler to sample from the joint distribution.
-    SPARSE_GRID = 2  #: The sparse grid inference uses a sparse grid to evaluate the joint distribution. It is not tested and not recommended.
-
-
 def inference(
     model: Model,
     data: Union[str, os.PathLike, np.ndarray],
     inference_type: InferenceType = InferenceType.MCMC,
     slices: Optional[list[np.ndarray]] = None,
     num_processes: int = 4,
     run_name: str = "default_run",
@@ -61,25 +52,29 @@
     if isinstance(data, (str, os.PathLike, pathlib.Path)):
         data = np.loadtxt(data, delimiter=",", ndmin=2)
     elif not isinstance(data, (np.ndarray, jnp.ndarray)):
         raise TypeError(
             f"The data argument must be a path to a file or a numpy array. The argument passed was of type {type(data)}."
         )
 
+    # TODO Calculate Transformation to normalize data and normalize data, create transformation object
+    # TODO rename std_dev to kernel_width, adapt calculation of kernel width
+
     slices = slices or [
         np.arange(model.param_dim)
     ]  # If no slice is given, compute full joint distribution, i.e. a slice with all parameters
     result_manager = result_manager or ResultManager(
-        model.name, run_name
+        model.name, run_name, slices
     )  # If no result_manager is given, create one with default paths
 
     if not continue_sampling:
-        result_manager.delete_application_folder_structure(model, slices)
-    result_manager.create_application_folder_structure(model, slices)
+        result_manager.delete_application_folder_structure()
+    result_manager.create_application_folder_structure()
 
+    # TODO give transformation object to inference functions
     if inference_type == InferenceType.DENSE_GRID:
         return inference_dense_grid(
             model=model,
             data=data,
             result_manager=result_manager,
             slices=slices,
             num_processes=num_processes,
```

### Comparing `eulerpi-0.1.5/eulerpi/core/kde.py` & `eulerpi-0.2.0/eulerpi/core/kde.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.1.5/eulerpi/core/model.py` & `eulerpi-0.2.0/eulerpi/core/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import inspect
 import os
+import tempfile
 from abc import ABC, abstractmethod
 from functools import partial
 from typing import Optional, Tuple, Union
 
 import jax.numpy as jnp
 import numpy as np
 from jax import jacrev, jit, vmap
@@ -270,69 +271,143 @@
         central_param(np.ndarray): The central parameter for the model
         param_limits(np.ndarray): The parameter limits for the model
     """
 
     @property
     def param_dim(self):
         """The number of parameters of the model."""
-        return len(self.model.getParameterIds())
+        return len(self.amici_model.getParameterIds())
 
     @property
     def data_dim(self):
         """The number of observables of the model."""
-        return len(self.model.getObservableIds())
+        return len(self.amici_model.getObservableIds())
 
     def __init__(
         self,
         sbml_file: str,
         central_param: np.ndarray,
         param_limits: np.ndarray,
         param_names=None,
         tEnd=1.0,
         skip_creation: bool = False,
         name: Optional[str] = None,
         **kwargs,
     ) -> None:
         super().__init__(central_param, param_limits, name, **kwargs)
 
-        model_name = self.name
-        model_dir = "./amici"
+        self.tEnd = tEnd
+
+        self.amici_model_name = self.name
+        self.amici_model_dir = "./amici/" + self.amici_model_name
 
         # Generate python code
         if not skip_creation:
             sbml_importer = amici.SbmlImporter(sbml_file)
-            sbml_importer.sbml2amici(model_name, model_dir)
+            sbml_importer.sbml2amici(
+                self.amici_model_name, self.amici_model_dir
+            )
 
         # Load the generated model
-        model_module = amici.import_model_module(model_name, model_dir)
-        model = model_module.getModel()
-        solver = model.getSolver()
-
-        model.setTimepoints([tEnd])
-        model.requireSensitivitiesForAllParameters()
-        solver.setSensitivityMethod(amici.SensitivityMethod.forward)
-        solver.setSensitivityOrder(amici.SensitivityOrder.first)
+        self.load_amici_model_and_solver()
 
-        self.param_names = param_names or model.getParameterNames()
+        self.param_names = param_names or self.amici_model.getParameterNames()
 
-        self.model = model
-        self.solver = solver
+    def load_amici_model_and_solver(self):
+        """Loads the AMICI model from the previously generated model."""
+        amici_model_module = amici.import_model_module(
+            self.amici_model_name, self.amici_model_dir
+        )
+        self.amici_model = amici_model_module.getModel()
+        self.amici_solver = self.amici_model.getSolver()
+
+        # TODO: Maybe this is redundant when using settings to hdf5
+        self.amici_model.setTimepoints([self.tEnd])
+        self.amici_model.requireSensitivitiesForAllParameters()
+        self.amici_solver.setSensitivityMethod(amici.SensitivityMethod.forward)
+        self.amici_solver.setSensitivityOrder(amici.SensitivityOrder.first)
 
     def forward(self, params):
         for i, param in enumerate(params):
-            self.model.setParameterByName(self.param_names[i], param)
-        rdata = amici.runAmiciSimulation(self.model, self.solver)
+            self.amici_model.setParameterByName(self.param_names[i], param)
+        rdata = amici.runAmiciSimulation(self.amici_model, self.amici_solver)
         return rdata.x[-1]
 
     def jacobian(self, params):
         for i, param in enumerate(params):
-            self.model.setParameterByName(self.param_names[i], param)
-        rdata = amici.runAmiciSimulation(self.model, self.solver)
+            self.amici_model.setParameterByName(self.param_names[i], param)
+        rdata = amici.runAmiciSimulation(self.amici_model, self.amici_solver)
         return rdata.sx[-1].T
 
     def forward_and_jacobian(
         self, params: np.ndarray
     ) -> Tuple[np.ndarray, np.ndarray]:
         for i, param in enumerate(params):
-            self.model.setParameterByName(self.param_names[i], param)
-        rdata = amici.runAmiciSimulation(self.model, self.solver)
+            self.amici_model.setParameterByName(self.param_names[i], param)
+        rdata = amici.runAmiciSimulation(self.amici_model, self.amici_solver)
         return rdata.x[-1], rdata.sx[-1].T
+
+    # Allow the model to be pickled
+    def __getstate__(self):
+        # Create a copy of the object's state
+        state = self.__dict__.copy()
+
+        # Save the amici solver settings to
+        _fd, _file = tempfile.mkstemp()
+        try:
+            # write amici solver settings to file
+            try:
+                amici.writeSolverSettingsToHDF5(self.amici_solver, _file)
+            except AttributeError as e:
+                e.args += (
+                    "Pickling the SBMLModel requires an AMICI "
+                    "installation with HDF5 support.",
+                )
+                raise
+            # read in byte stream
+            with open(_fd, "rb", closefd=False) as f:
+                state["amici_solver_settings"] = f.read()
+        finally:
+            # close file descriptor and remove temporary file
+            os.close(_fd)
+            os.remove(_file)
+
+        state["amici_model_settings"] = amici.get_model_settings(
+            self.amici_model
+        )
+
+        # Remove the unpicklable entries.
+        del state["amici_model"]
+        del state["amici_solver"]
+        return state
+
+    def __setstate__(self, state):
+        self.__dict__.update(state)
+
+        # Restore amici model and solver
+        self.load_amici_model_and_solver()
+
+        _fd, _file = tempfile.mkstemp()
+        try:
+            # write solver settings to temporary file
+            with open(_fd, "wb", closefd=False) as f:
+                f.write(state["amici_solver_settings"])
+            # read in solver settings
+            try:
+                amici.readSolverSettingsFromHDF5(_file, self.amici_solver)
+            except AttributeError as err:
+                if not err.args:
+                    err.args = ("",)
+                err.args += (
+                    "Unpickling an AmiciObjective requires an AMICI "
+                    "installation with HDF5 support.",
+                )
+                raise
+        finally:
+            # close file descriptor and remove temporary file
+            os.close(_fd)
+            os.remove(_file)
+
+        amici.set_model_settings(
+            self.amici_model,
+            state["amici_model_settings"],
+        )
```

### Comparing `eulerpi-0.1.5/eulerpi/core/sampling.py` & `eulerpi-0.2.0/eulerpi/core/sampling.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,35 +9,63 @@
     NUM_WALKERS (int): Default number of walkers in the emcee sampler.
     NUM_STEPS (int): Default number of steps each walker performs before storing the sub run.
     NUM_PROCESSES (int): Default number of parallel threads.
 
 """
 
 import typing
+from multiprocessing import get_context
 from os import path
 
 import emcee
 import numpy as np
-from schwimmbad import MultiPool
 
 from eulerpi import logger
+from eulerpi.core.inference_types import InferenceType
 from eulerpi.core.kde import calc_kernel_width
 from eulerpi.core.model import Model
 from eulerpi.core.result_manager import ResultManager
 from eulerpi.core.transformations import eval_log_transformed_density
 
 # TODO: This works on the blob
 # Return the samples.
 # return sampler.get_chain(discard=0, thin=1, flat=True)
 # TODO: This stores the sample as 2d array in the format walker1_step1, walker2_step1, walker3_step1, walker1_step2, walker2_step2, walker3_step2, ...
 # sampler_results = samplerBlob.reshape(
 #     num_walkers * num_steps, sampling_dim + data_dim + 1
 # )
 
 
+# TODO Give transformation object to eval function
+def evaluate_sample(
+    param: np.ndarray,
+    model: Model,
+    data: np.ndarray,
+    data_stdevs: np.ndarray,
+    slice: np.ndarray,
+) -> typing.Tuple[float, np.ndarray]:
+    """Evaluate the log transformed density at the given parameter values.
+
+    Args:
+        param (np.ndarray): parameter values
+        model (Model): The model which will be sampled
+        data (np.ndarray): data
+        data_stdevs (np.ndarray): kernel width for the data
+        slice (np.ndarray): slice of the parameter space which will be sampled
+
+    Returns:
+        typing.Tuple[float, np.ndarray]: log transformed density and the sampler result
+    """
+
+    log_samplerresult = eval_log_transformed_density(
+        param, model, data, data_stdevs, slice
+    )
+    return log_samplerresult
+
+
 def run_emcee_once(
     model: Model,
     data: np.ndarray,
     data_stdevs: np.ndarray,
     slice: np.ndarray,
     initial_walker_positions: np.ndarray,
     num_walkers: int,
@@ -57,46 +85,26 @@
         num_processes (int): number of parallel threads
 
     Returns:
         np.ndarray: samples from the transformed parameter density
 
     """
 
-    global work
-
-    def work(params):
-        s = eval_log_transformed_density(
-            params, model, data, data_stdevs, slice
-        )
-        return s
-
-    pool = MultiPool(processes=num_processes)
-
-    # define a custom move policy
-    movePolicy = [
-        (emcee.moves.WalkMove(), 0.1),
-        (emcee.moves.StretchMove(), 0.1),
-        (
-            emcee.moves.GaussianMove(0.00001, mode="sequential", factor=None),
-            0.8,
-        ),
-    ]
-    # movePolicy = [(emcee.moves.GaussianMove(0.00001, mode='sequential', factor=None), 1.0)]
+    # Create a pool of worker processes
+    pool = get_context("spawn").Pool(processes=num_processes)
     sampling_dim = slice.shape[0]
 
     # Call the sampler for all parallel workers (possibly use arg moves = movePolicy)
     try:
         sampler = emcee.EnsembleSampler(
             num_walkers,
             sampling_dim,
-            # eval_log_transformed_density,
-            work,
+            evaluate_sample,
             pool=pool,
-            moves=movePolicy,
-            # args=[model, data, data_stdevs, slice],
+            args=[model, data, data_stdevs, slice],
         )
         # Extract the final walker position and close the pool of worker processes.
         final_walker_positions, _, _, _ = sampler.run_mcmc(
             initial_walker_positions, num_steps, tune=True, progress=True
         )
     except ValueError as e:
         # If the message equals "Probability function returned NaN."
@@ -143,34 +151,38 @@
     data: np.ndarray,
     slice: np.ndarray,
     result_manager: ResultManager,
     num_processes: int,
     num_runs: int,
     num_walkers: int,
     num_steps: int,
+    num_burn_in_samples: int,
+    thinning_factor: int,
 ) -> typing.Tuple[np.ndarray, np.ndarray, np.ndarray]:
     """Create a representative sample from the transformed parameter density using the emcee particle swarm sampler.
        Inital values are not stored in the chain and each file contains <num_steps> blocks of size num_walkers.
 
     Args:
         model (Model): The model which will be sampled
         data (np.ndarray): data
         slice (np.ndarray): slice of the parameter space which will be sampled
         result_manager (ResultManager): ResultManager which will store the results
         num_processes (int): number of parallel threads.
         num_runs (int): number of stored sub runs.
         num_walkers (int): number of particles in the particle swarm sampler.
         num_steps (int): number of samples each particle performs before storing the sub run.
+        num_burn_in_samples (int): number of samples to be discarded as burn-in.
+        thinning_factor (int): thinning factor for the samples.
 
     Returns:
         typing.Tuple[np.ndarray, np.ndarray, np.ndarray]: Array with all params, array with all data, array with all log probabilities
         TODO check: are those really log probabilities?
 
     """
-
+    # Calculate the standard deviation of the data for each dimension
     data_stdevs = calc_kernel_width(data)
     sampling_dim = slice.shape[0]
     central_param = model.central_param
 
     # Initialize each walker at a Gaussian-drawn random, slightly different parameter close to the central parameter.
     # TODO Make random variation of initial walker positions dependent on sampling limits?
     initial_walker_positions = central_param[slice] + 0.002 * (
@@ -217,17 +229,24 @@
 
     (
         overall_params,
         overall_sim_results,
         overall_density_evals,
     ) = concatenate_emcee_sampling_results(model, result_manager, slice)
     result_manager.save_overall(
-        slice, overall_params, overall_sim_results, overall_density_evals
+        slice,
+        overall_params[num_burn_in_samples::thinning_factor, :],
+        overall_sim_results[num_burn_in_samples::thinning_factor, :],
+        overall_density_evals[num_burn_in_samples::thinning_factor],
+    )
+    return (
+        overall_params[num_burn_in_samples::thinning_factor, :],
+        overall_sim_results[num_burn_in_samples::thinning_factor, :],
+        overall_density_evals[num_burn_in_samples::thinning_factor],
     )
-    return overall_params, overall_sim_results, overall_density_evals
 
 
 # TODO: Make this a method of the ResultManager? It uses the ResultManager to load the results and many hard coded paths.
 def concatenate_emcee_sampling_results(
     model: Model, result_manager: ResultManager, slice: np.ndarray
 ) -> typing.Tuple[np.ndarray, np.ndarray, np.ndarray]:
     """Concatenate many sub runs of the emcee sampler to create 3 large files for sampled parameters, corresponding simulation results and density evaluations.
@@ -278,38 +297,38 @@
     return overall_params, overall_sim_results, overall_density_evals
 
 
 def calc_walker_acceptance(
     model: Model,
     slice: np.ndarray,
     num_walkers: int,
-    num_burn_samples: int,
+    num_burn_in_samples: int,
     result_manager: ResultManager,
 ):
     """Calculate the acceptance ratio for each individual walker of the emcee chain.
     This is especially important to find "zombie" walkers, that are never moving.
 
     Args:
         model (Model): The model for which the acceptance ratio should be calculated
         slice (np.ndarray): slice for which the acceptance ratio should be calculated
         num_walkers (int): number of walkers in the emcee chain
-        num_burn_samples (int): number of samples that were ignored at the beginning of each chain
+        num_burn_in_samples (int): number of samples that were ignored at the beginning of each chain
         result_manager (ResultManager): ResultManager to load the results from
 
     Returns:
         np.ndarray: Array with the acceptance ratio for each walker
 
     """
 
     # load the emcee parameter chain
     params = np.loadtxt(
         result_manager.get_slice_path(slice) + "/overall_params.csv",
         delimiter=",",
         ndmin=2,
-    )[num_burn_samples:, :]
+    )[num_burn_in_samples:, :]
 
     # calculate the number of steps each walker walked
     # subtract 1 because we count the steps between the parameters
     num_steps = int(params.shape[0] / num_walkers) - 1
 
     # Unflatten the parameter chain and count the number of accepted steps for each walker
     params = params.reshape(num_steps + 1, num_walkers, model.param_dim)
@@ -330,17 +349,19 @@
 
 def inference_mcmc(
     model: Model,
     data: np.ndarray,
     result_manager: ResultManager,
     slices: list[np.ndarray],
     num_processes: int,
-    num_runs: int = 2,
+    num_runs: int = 1,
     num_walkers: int = 10,
     num_steps: int = 2500,
+    num_burn_in_samples: typing.Optional[int] = None,
+    thinning_factor: typing.Optional[int] = None,
     calc_walker_acceptance_bool: bool = False,
 ) -> typing.Tuple[
     typing.Dict[str, np.ndarray],
     typing.Dict[str, np.ndarray],
     typing.Dict[str, np.ndarray],
     ResultManager,
 ]:
@@ -348,24 +369,32 @@
 
     Args:
         model (Model): The model describing the mapping from parameters to data.
         data (np.ndarray): The data to be used for the inference.
         result_manager (ResultManager): The result manager to be used for the inference.
         slices (np.ndarray): A list of slices to be used for the inference.
         num_processes (int): The number of processes to be used for the inference.
-        num_runs (int, optional): The number of runs to be used for the inference. Defaults to 2.
-        num_walkers (int, optional): The number of walkers to be used for the inference. Defaults to 10.
+        num_runs (int, optional): The number of runs to be used for the inference. For each run except the first, all walkers continue with the end position of the previous run - this parameter does not affect the number of Markov chains, but how often results for each chain are saved. Defaults to 1.
+        num_walkers (int, optional): The number of walkers to be used for the inference. Corresponds to the number of Markov chains. Defaults to 10.
         num_steps (int, optional): The number of steps to be used for the inference. Defaults to 2500.
+        num_burn_in_samples (int, optional): number of samples to be discarded as burn-in. Defaults to None means a burn in of 10% of the total number of samples.
+        thinning_factor (int, optional): thinning factor for the samples. Defaults to None means no thinning.
         calc_walker_acceptance_bool (bool, optional): If True, the acceptance rate of the walkers is calculated and printed. Defaults to False.
 
     Returns:
         Tuple[typing.Dict[str, np.ndarray], typing.Dict[str, np.ndarray], typing.Dict[str, np.ndarray], ResultManager]: The parameter samples, the corresponding simulation results, the corresponding density
         evaluations for each slice and the result manager used for the inference.
 
     """
+    # Set default values for burn in and thinning factor
+    if num_burn_in_samples is None:
+        num_burn_in_samples = int(num_runs * num_walkers * num_steps * 0.1)
+    if thinning_factor is None:
+        thinning_factor = 1
+
     # create the return dictionaries
     overall_params, overall_sim_results, overall_density_evals = {}, {}, {}
 
     for slice in slices:
         slice_name = result_manager.get_slice_name(slice)
         (
             overall_params[slice_name],
@@ -375,19 +404,32 @@
             model=model,
             data=data,
             slice=slice,
             result_manager=result_manager,
             num_runs=num_runs,
             num_walkers=num_walkers,
             num_steps=num_steps,
+            num_burn_in_samples=num_burn_in_samples,
+            thinning_factor=thinning_factor,
+            num_processes=num_processes,
+        )
+        result_manager.save_inference_information(
+            slice=slice,
+            model=model,
+            inference_type=InferenceType.MCMC,
             num_processes=num_processes,
+            num_runs=num_runs,
+            num_walkers=num_walkers,
+            num_steps=num_steps,
+            num_burn_in_samples=num_burn_in_samples,
+            thinning_factor=thinning_factor,
         )
 
         if calc_walker_acceptance_bool:
-            num_burn_in_steps = int(num_steps * 0.01)
+            num_burn_in_steps = int(num_steps * num_runs * 0.01)
             acceptance = calc_walker_acceptance(
                 model, slice, num_walkers, num_burn_in_steps, result_manager
             )
             logger.info(f"Acceptance rate for slice {slice}: {acceptance}")
 
     return (
         overall_params,
```

### Comparing `eulerpi-0.1.5/eulerpi/core/sparsegrid.py` & `eulerpi-0.2.0/eulerpi/core/sparsegrid.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 
         The inference with this class is not tested and not recommended for use!
 
 .. _SGs: https://en.wikipedia.org/wiki/Sparse_grid
 """
 
 import typing
-from functools import partial
-from multiprocessing import Pool
+from itertools import repeat
+from multiprocessing import get_context
 
 import numpy as np
 
 from eulerpi import logger
+from eulerpi.core.inference_types import InferenceType
 from eulerpi.core.kde import calc_kernel_width
 from eulerpi.core.model import Model
 from eulerpi.core.result_manager import ResultManager
-from eulerpi.core.transformations import eval_log_transformed_density
+from eulerpi.core.transformations import evaluate_density
 
 
 def basis_1d(
     points1D: np.ndarray, centre1D: np.double, level: int
 ) -> np.ndarray:
     """Evaluate a 1D hat function in an array of doubles. The hat is centered around centre1D
     and the hat's level defines its support. The support shrinks exponentially with growing level and a level of 0 is equivalent with full support on [0,1].
@@ -363,34 +364,54 @@
                             self.points[p, :],
                             self.levels,
                         )
                         * self.coeffs[p]
                     )
 
 
+def evaluate_on_sparse_grid(
+    args: typing.Tuple[np.ndarray, Model, np.ndarray, np.ndarray, np.ndarray]
+) -> np.ndarray:
+    """This function is used to evaluate a function on a sparse grid in parallel. The input args is a tuple containing the function, the sparse grid and the number of processes to be used.
+
+    Args:
+        params (np.ndarray): The parameters to be evaluated.
+        model(Model): The model used for the inference.
+        data(np.ndarray): The data points used for the inference.
+        data_stdevs(np.ndarray): The standard deviations of the data points. (Currently the kernel width, #TODO!)
+        slice(np.ndarray): The slice defines for which dimensions of the grid points / paramater vectors the marginal density should be evaluated.
+
+    Returns:
+        np.ndarray: The density values for the given params.
+    """
+
+    params, model, data, data_stdevs, slice = args
+    return evaluate_density(params, model, data, data_stdevs, slice)[1]
+
+
 def inference_sparse_grid(
     model: Model,
     data: np.ndarray,
     result_manager: ResultManager,
     slices: typing.List[np.ndarray],
     num_processes: int,
-    numLevels: int = 5,
+    num_levels: int = 5,
 ) -> typing.Tuple[
     typing.Dict[str, np.ndarray],
     typing.Dict[str, np.ndarray],
     typing.Dict[str, np.ndarray],
     ResultManager,
 ]:
     """Evaluates the transformed parameter density over a set of points resembling a sparse grid, thereby attempting parameter inference. If a data path is given, it is used to load the data for the model. Else, the default data path of the model is used.
 
     Args:
       model(Model): The model describing the mapping from parameters to data.
       data(np.ndarray): The data to be used for inference.
       num_processes(int): number of processes to use for parallel evaluation of the model.
-      numLevels(int, optional): Maximum sparse grid level depth that mainly defines the number of points. Defaults to 5.
+      num_levels(int, optional): Maximum sparse grid level depth that mainly defines the number of points. Defaults to 5.
 
     Returns:
         Tuple[typing.Dict[str, np.ndarray], typing.Dict[str, np.ndarray], typing.Dict[str, np.ndarray], ResultManager]: The parameter samples, the corresponding simulation results, the corresponding density
         evaluations for each slice and the result manager used for the inference.
 
     """
 
@@ -400,51 +421,49 @@
     data_stdevs = calc_kernel_width(data)
 
     # create the return dictionaries
     overall_params, overall_sim_results, overall_density_evals = {}, {}, {}
 
     for slice in slices:
         # build the sparse grid over [0,1]^param_dim
-        grid = SparseGrid(slice.shape[0], numLevels)
+        grid = SparseGrid(slice.shape[0], num_levels)
 
         # get the model's parameter limits
         param_limits = model.param_limits
 
         # scale the sparse grid points from [0,1]^param_dim to the scaled parameter space
         scaledSparseGridPoints = param_limits[slice, 0] + grid.points * (
             param_limits[slice, 1] - param_limits[slice, 0]
         )
 
-        # allocate Memory for the parameters, their simulation evaluation and their probability density
-        results = np.zeros(
-            (grid.n_points, slice.shape[0] + model.data_dim + 1)
-        )
-
         # Create a pool of worker processes
-        pool = Pool(processes=num_processes)
+        pool = get_context("spawn").Pool(processes=num_processes)
+        tasks = zip(
+            scaledSparseGridPoints,
+            repeat(model),
+            repeat(data),
+            repeat(data_stdevs),
+            repeat(slice),
+        )
 
         # evaluate the probability density transformation for all sparse grid points in parallel
-        parResults = pool.map(
-            partial(
-                eval_log_transformed_density,
-                model=model,
-                data=data,
-                data_stdevs=data_stdevs,
-                slice=slice,
-            ),
-            scaledSparseGridPoints,
+        results = pool.map(
+            evaluate_on_sparse_grid,
+            tasks,
         )
 
         # close the worker pool
         pool.close()
         pool.join()
 
-        # extract the parameter, simulation result and transformed density evaluation
-        for i in range(grid.n_points):
-            results[i, :] = parResults[i][1]
+        # convert the results to a numpy array
+        # Take care! The results here are for single points, therefore we cant use np.concatenate
+        results = np.vstack(results)
+
+        print(results.shape)
 
         # save the results
         result_manager.save_overall(
             slice,
             results[:, 0 : data.shape[1]],
             results[:, data.shape[1] : data.shape[1] + slice.shape[0]],
             results[:, data.shape[1] + slice.shape[0] :],
@@ -453,13 +472,21 @@
         overall_params[slice_name] = results[:, 0 : data.shape[1]]
         overall_sim_results[slice_name] = results[
             :, data.shape[1] : data.shape[1] + slice.shape[0]
         ]
         overall_density_evals[slice_name] = results[
             :, data.shape[1] + slice.shape[0] :
         ]
+        result_manager.save_inference_information(
+            slice=slice,
+            model=model,
+            inference_type=InferenceType.DENSE_GRID,
+            num_processes=num_processes,
+            num_levels=num_levels,
+        )
+
     return (
         overall_params,
         overall_sim_results,
         overall_density_evals,
         result_manager,
     )
```

### Comparing `eulerpi-0.1.5/eulerpi/core/transformations.py` & `eulerpi-0.2.0/eulerpi/core/transformations.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,17 @@
         return 0, np.zeros(slice.shape[0] + model.data_dim + 1)
 
     # If the parameter is within the valid ranges...
     else:
         # Evaluating the model and the jacobian for the specified parameter simultaneously provide a little speedup over calculating it separately in some cases.
         sim_res, jac = model.forward_and_jacobian(fullParam)
 
-        # Evaluate the data density in the simulation result.
+        # TODO transform sim res and use transformed simres below
+
+        # Evaluate the data density in the simulation result. # TODO scale with determinant transformation matrix
         densityEvaluation = eval_kde_gauss(data, sim_res, data_stdevs)
 
         # Calculate the simulation model's pseudo-determinant in the parameter point (also called the correction factor).
         correction = calc_gram_determinant(jac)
 
         # Multiply data density and correction factor.
         trafo_density_evaluation = densityEvaluation * correction
@@ -85,14 +87,15 @@
 
     Returns:
         Tuple[np.double, np.ndarray]:
             : natural log of the parameter density at the point param
             : sampler_results (array concatenation of parameters, simulation results and evaluated density, stored as "blob" by the emcee sampler)
 
     """
+    # TODO give transformation object to evaluation function
     trafo_density_evaluation, evaluation_results = evaluate_density(
         param, model, data, data_stdevs, slice
     )
     if trafo_density_evaluation == 0:
         return -np.inf, evaluation_results
     return np.log(trafo_density_evaluation), evaluation_results
```

### Comparing `eulerpi-0.1.5/eulerpi/examples/corona/CoronaData.csv` & `eulerpi-0.2.0/eulerpi/examples/corona/CoronaData.csv`

 * *Files identical despite different names*

### Comparing `eulerpi-0.1.5/eulerpi/examples/corona/corona.py` & `eulerpi-0.2.0/eulerpi/examples/corona/corona.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,15 +68,24 @@
 
         except Exception as e:
             logger.warning("ODE solution not possible!", exc_info=e)
             return np.array([-np.inf, -np.inf, -np.inf, -np.inf])
 
 
 class CoronaArtificial(Corona, ArtificialModelInterface):
-    param_limits = np.array([[-2.5, -1.0], [-0.75, 0.75], [0.0, 1.5]])
+    PARAM_LIMITS = np.array([[-2.5, -1.0], [-0.75, 0.75], [0.0, 1.5]])
+
+    def __init__(
+        self,
+        central_param: np.ndarray = Corona.CENTRAL_PARAM,
+        param_limits: np.ndarray = PARAM_LIMITS,
+        name: Optional[str] = None,
+        **kwargs,
+    ) -> None:
+        super().__init__(central_param, param_limits, name=name, **kwargs)
 
     def generate_artificial_params(self, num_samples):
         lower_bound = np.array([-1.9, -0.1, 0.6])
         upper_bound = np.array([-1.7, 0.1, 0.8])
 
         true_param_sample = lower_bound + (
             upper_bound - lower_bound
```

### Comparing `eulerpi-0.1.5/eulerpi/examples/cpp/CMakeLists.txt` & `eulerpi-0.2.0/eulerpi/examples/cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `eulerpi-0.1.5/eulerpi/examples/cpp/cpp_model.hpp` & `eulerpi-0.2.0/eulerpi/examples/cpp/cpp_model.hpp`

 * *Files identical despite different names*

### Comparing `eulerpi-0.1.5/eulerpi/examples/cpp/cpp_plant.py` & `eulerpi-0.2.0/eulerpi/examples/cpp/cpp_plant.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.1.5/eulerpi/examples/cpp/python_reference_plants.py` & `eulerpi-0.2.0/eulerpi/examples/cpp/python_reference_plants.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.1.5/eulerpi/examples/sbml/Caffeine_2Wks_Exponential_decay.xml` & `eulerpi-0.2.0/eulerpi/examples/sbml/Caffeine_2Wks_Exponential_decay.xml`

 * *Files identical despite different names*

### Comparing `eulerpi-0.1.5/eulerpi/examples/sbml/sbml_caffeine_model.py` & `eulerpi-0.2.0/eulerpi/examples/sbml/sbml_caffeine_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import importlib
-from typing import Optional
 
 import numpy as np
 
 from eulerpi.core.model import ArtificialModelInterface, SBMLModel
 
 
 class CaffeineSBMLModel(SBMLModel, ArtificialModelInterface):
@@ -14,29 +13,25 @@
     CENTRAL_PARAM = np.array([1.0, 1.0])
     PARAM_LIMITS = np.array([[0.0, 2.0], [0.0, 2.0]])
 
     def __init__(
         self,
         central_param: np.ndarray = CENTRAL_PARAM,
         param_limits: np.ndarray = PARAM_LIMITS,
-        name: Optional[str] = None,
         **kwargs,
     ) -> None:
         sbml_file = importlib.resources.path(
             "eulerpi.examples.sbml", "Caffeine_2Wks_Exponential_decay.xml"
         )
         param_names = ["A", "B"]
         super().__init__(
             sbml_file,
             central_param,
             param_limits,
             param_names,
-            1.0,
-            False,
-            name,
             **kwargs,
         )
 
     def generate_artificial_params(self, num_samples: int) -> np.ndarray:
         diff0 = 0.2
         diff1 = 0.2
         params = np.random.rand(num_samples, self.param_dim)
```

### Comparing `eulerpi-0.1.5/eulerpi/examples/sbml/sbml_menten_model.py` & `eulerpi-0.2.0/eulerpi/examples/sbml/sbml_menten_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import importlib
-from typing import Optional
 
 import numpy as np
 
 from eulerpi.core.model import ArtificialModelInterface, SBMLModel
 
 
 class MentenSBMLModel(SBMLModel, ArtificialModelInterface):
@@ -11,29 +10,25 @@
     CENTRAL_PARAM = np.array([50.0, 1.0])
     PARAM_LIMITS = np.array([[0.0, 100.0], [0.0, 2.0]])
 
     def __init__(
         self,
         central_param: np.ndarray = CENTRAL_PARAM,
         param_limits: np.ndarray = PARAM_LIMITS,
-        name: Optional[str] = None,
         **kwargs,
     ) -> None:
         sbml_file = importlib.resources.path(
             "eulerpi.examples.sbml", "sbml_menten_model.xml"
         )
         param_names = ["Km", "kcat"]
         super().__init__(
             sbml_file,
             central_param,
             param_limits,
             param_names,
-            1.0,
-            False,
-            name,
             **kwargs,
         )
 
     # Overwrite the forward, jacobian, and forward_and_jacobian methods to remove the first variable which is not dependent on the parameters
     def forward(self, params) -> np.ndarray:
         return super().forward(params)[1:]
```

### Comparing `eulerpi-0.1.5/eulerpi/examples/sbml/sbml_menten_model.xml` & `eulerpi-0.2.0/eulerpi/examples/sbml/sbml_menten_model.xml`

 * *Files identical despite different names*

### Comparing `eulerpi-0.1.5/eulerpi/examples/simple_models.py` & `eulerpi-0.2.0/eulerpi/examples/simple_models.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.1.5/eulerpi/examples/stock/ETF.csv` & `eulerpi-0.2.0/eulerpi/examples/stock/ETF.csv`

 * *Files identical despite different names*

### Comparing `eulerpi-0.1.5/eulerpi/examples/stock/stock.py` & `eulerpi-0.2.0/eulerpi/examples/stock/stock.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.1.5/eulerpi/examples/temperature/TemperatureArtificialParams.csv` & `eulerpi-0.2.0/eulerpi/examples/temperature/TemperatureArtificialParams.csv`

 * *Files identical despite different names*

### Comparing `eulerpi-0.1.5/eulerpi/examples/temperature/TemperatureData.csv` & `eulerpi-0.2.0/eulerpi/examples/temperature/TemperatureData.csv`

 * *Files identical despite different names*

### Comparing `eulerpi-0.1.5/eulerpi/examples/temperature/temperature.py` & `eulerpi-0.2.0/eulerpi/examples/temperature/temperature.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.1.5/eulerpi/jax_extension.py` & `eulerpi-0.2.0/eulerpi/jax_extension.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.1.5/pyproject.toml` & `eulerpi-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "eulerpi"
-version = "0.1.5"
-description = "The EPI returns a parameter distribution, which is consistent with the observed data by solving the inverse problem directly. In the case of a one-to-one mapping, this is the true underlying distribution."
+version = "0.2.0"
+description = "The eulerian parameter inference (eulerpi) returns a parameter distribution, which is consistent with the observed data by solving the inverse problem directly. In the case of a one-to-one mapping, this is the true underlying distribution."
 authors = ["Lars Kaiser <lars.g.kaiser@gmx.de>", "Sebastian Hoepfl <sebastian.hoepfl@ist.uni-stuttgart.de>", "Vincent Wagner <vincent.wagner@ist.uni-stuttgart.de>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
@@ -25,15 +25,14 @@
 diffrax = "^0.3.1"
 emcee = "^3.1.4"
 jaxlib = "^0.4.7"
 tqdm = "^4.65.0"
 seedir = "^0.4.2"
 yfinance = "^0.2.14"
 amici = "^0.16.1"
-schwimmbad = "^0.3.2"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.2.2"
 black = "^23.3.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 pytest = "^7.2.2"
```

### Comparing `eulerpi-0.1.5/PKG-INFO` & `eulerpi-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: eulerpi
-Version: 0.1.5
-Summary: The EPI returns a parameter distribution, which is consistent with the observed data by solving the inverse problem directly. In the case of a one-to-one mapping, this is the true underlying distribution.
+Version: 0.2.0
+Summary: The eulerian parameter inference (eulerpi) returns a parameter distribution, which is consistent with the observed data by solving the inverse problem directly. In the case of a one-to-one mapping, this is the true underlying distribution.
 Author: Lars Kaiser
 Author-email: lars.g.kaiser@gmx.de
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -15,15 +15,14 @@
 Requires-Dist: amici (>=0.16.1,<0.17.0)
 Requires-Dist: diffrax (>=0.3.1,<0.4.0)
 Requires-Dist: emcee (>=3.1.4,<4.0.0)
 Requires-Dist: jax (>=0.4.8,<0.5.0)
 Requires-Dist: jaxlib (>=0.4.7,<0.5.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
-Requires-Dist: schwimmbad (>=0.3.2,<0.4.0)
 Requires-Dist: seedir (>=0.4.2,<0.5.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: yfinance (>=0.2.14,<0.3.0)
 Project-URL: Bug Tracker, https://github.com/Systems-Theory-in-Systems-Biology/EPI/issues
 Project-URL: Documentation, https://Systems-Theory-in-Systems-Biology.github.io/EPI/
 Project-URL: Homepage, https://github.com/Systems-Theory-in-Systems-Biology/EPI
 Description-Content-Type: text/markdown
@@ -65,15 +64,15 @@
 ```bash
 pip install eulerpi
 ```
 
 Make sure that you have the following C++ libraries installed
 
 ```bash
-sudo apt install -y swig libblas-dev libatlas-base-dev
+sudo apt install -y swig libblas-dev libatlas-base-dev libhdf5-dev
 ```
 
 You can also build the library from the latest source code by following the [Development Quickstart Guide](./DEVELOPMENT.md#quickstart).
 
 ## Using the library
 
 To use EPI, derive your model from the `Model` class and implement the abstract functions. Here's an example code snippet:
```

