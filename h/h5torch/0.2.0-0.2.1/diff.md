# Comparing `tmp/h5torch-0.2.0.tar.gz` & `tmp/h5torch-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h5torch-0.2.0.tar", last modified: Thu Apr  6 09:32:10 2023, max compression
+gzip compressed data, was "h5torch-0.2.1.tar", last modified: Thu Apr 20 14:31:11 2023, max compression
```

## Comparing `h5torch-0.2.0.tar` & `h5torch-0.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:32:10.044968 h5torch-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:32:10.036968 h5torch-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:32:10.036968 h5torch-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-06 09:31:53.000000 h5torch-0.2.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-06 09:31:53.000000 h5torch-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-06 09:31:53.000000 h5torch-0.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-06 09:31:53.000000 h5torch-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-04-06 09:32:10.044968 h5torch-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-06 09:31:53.000000 h5torch-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:32:10.040968 h5torch-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-06 09:31:53.000000 h5torch-0.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-06 09:31:53.000000 h5torch-0.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-06 09:31:53.000000 h5torch-0.2.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:32:10.040968 h5torch-0.2.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-06 09:31:53.000000 h5torch-0.2.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-06 09:31:53.000000 h5torch-0.2.0/docs/source/h5torch.rst
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-06 09:31:53.000000 h5torch-0.2.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    28656 2023-04-06 09:31:53.000000 h5torch-0.2.0/docs/source/tutorial.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:32:10.040968 h5torch-0.2.0/h5torch/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-06 09:31:53.000000 h5torch-0.2.0/h5torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10788 2023-04-06 09:31:53.000000 h5torch-0.2.0/h5torch/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12323 2023-04-06 09:31:53.000000 h5torch-0.2.0/h5torch/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:32:10.040968 h5torch-0.2.0/h5torch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-04-06 09:32:10.000000 h5torch-0.2.0/h5torch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-06 09:32:10.000000 h5torch-0.2.0/h5torch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 09:32:10.000000 h5torch-0.2.0/h5torch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-06 09:32:10.000000 h5torch-0.2.0/h5torch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-06 09:32:10.000000 h5torch-0.2.0/h5torch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:32:10.040968 h5torch-0.2.0/img/
--rw-r--r--   0 runner    (1001) docker     (123)   100333 2023-04-06 09:31:53.000000 h5torch-0.2.0/img/centralvsaligned.svg
--rw-r--r--   0 runner    (1001) docker     (123)   166130 2023-04-06 09:31:53.000000 h5torch-0.2.0/img/multidim.svg
--rw-r--r--   0 runner    (1001) docker     (123)   450263 2023-04-06 09:31:53.000000 h5torch-0.2.0/img/sampling.svg
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-06 09:31:53.000000 h5torch-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-06 09:32:10.044968 h5torch-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:11.117284 h5torch-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:11.105284 h5torch-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:11.109284 h5torch-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-20 14:31:00.000000 h5torch-0.2.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-20 14:31:00.000000 h5torch-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-20 14:31:00.000000 h5torch-0.2.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-20 14:31:00.000000 h5torch-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-04-20 14:31:11.117284 h5torch-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-04-20 14:31:00.000000 h5torch-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:11.109284 h5torch-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-20 14:31:00.000000 h5torch-0.2.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-20 14:31:00.000000 h5torch-0.2.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-20 14:31:00.000000 h5torch-0.2.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:11.113284 h5torch-0.2.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-20 14:31:00.000000 h5torch-0.2.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-20 14:31:00.000000 h5torch-0.2.1/docs/source/h5torch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-20 14:31:00.000000 h5torch-0.2.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    28656 2023-04-20 14:31:00.000000 h5torch-0.2.1/docs/source/tutorial.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:11.113284 h5torch-0.2.1/h5torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-20 14:31:00.000000 h5torch-0.2.1/h5torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10788 2023-04-20 14:31:00.000000 h5torch-0.2.1/h5torch/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12171 2023-04-20 14:31:00.000000 h5torch-0.2.1/h5torch/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:11.113284 h5torch-0.2.1/h5torch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-04-20 14:31:11.000000 h5torch-0.2.1/h5torch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-20 14:31:11.000000 h5torch-0.2.1/h5torch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:31:11.000000 h5torch-0.2.1/h5torch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 14:31:11.000000 h5torch-0.2.1/h5torch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 14:31:11.000000 h5torch-0.2.1/h5torch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:11.117284 h5torch-0.2.1/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   100333 2023-04-20 14:31:00.000000 h5torch-0.2.1/img/centralvsaligned.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   166130 2023-04-20 14:31:00.000000 h5torch-0.2.1/img/multidim.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   450263 2023-04-20 14:31:00.000000 h5torch-0.2.1/img/sampling.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-20 14:31:00.000000 h5torch-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-20 14:31:11.117284 h5torch-0.2.1/setup.cfg
```

### Comparing `h5torch-0.2.0/.github/workflows/publish.yml` & `h5torch-0.2.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `h5torch-0.2.0/.gitignore` & `h5torch-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `h5torch-0.2.0/LICENSE` & `h5torch-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `h5torch-0.2.0/PKG-INFO` & `h5torch-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5torch
-Version: 0.2.0
+Version: 0.2.1
 Summary: HDF5 data utilities for PyTorch
 Home-page: https://github.com/gdewael/h5torch
 Author: Gaetan De Waele
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -16,22 +16,22 @@
 
 [![PyPi Version](https://img.shields.io/pypi/v/h5torch.svg)](https://pypi.python.org/pypi/h5torch/)
 [![GitHub license](https://img.shields.io/github/license/gdewael/h5torch)](https://github.com/gdewael/h5torch/blob/main/LICENSE)
 [![Documentation](https://readthedocs.org/projects/h5torch/badge/?version=latest&style=flat-default)](https://h5torch.readthedocs.io/en/latest/index.html)
 
 </div>
 
-`h5torch` consists of two main parts: (1) `h5torch.File`: a wrapper around `h5py.File` as an interface to create HDF5 files compatible with (2) `h5torch.Dataset`, a wrapper around `torch.utils.data.Dataset`. As a library, `h5torch` establishes a "code" for linking [h5py] and [torch]. To do this, this package has to formulate a vocabulary for how datasets generally look, unifying as many ML settings to the best of its abilities. In turn, this vocabulary allows dataloading of various machine learning data settings from a single dataset class definition, reducing boilerplate in your projects.
+`h5torch` consists of two main parts: (1) `h5torch.File`: a wrapper around `h5py.File` as an interface to create HDF5 files compatible with (2) `h5torch.Dataset`, a wrapper around `torch.utils.data.Dataset`. As a library, `h5torch` establishes a "code" for linking [h5py](https://docs.h5py.org/en/stable/) and [torch](https://pytorch.org/docs/stable/index.html). To do this, this package has to formulate a vocabulary for how datasets generally look, unifying as many ML settings to the best of its abilities. In turn, this vocabulary allows dataloading of various machine learning data settings from a single dataset class definition, reducing boilerplate in your projects.
 
 ### Who is this package for?
 Loading data from HDF5 files allows for efficient data-loading from an **on-disk** format, drastically reducing memory overhead. Additionally, you will find your datasets to be more **organized** using the HDF5 format, as everything is neatly arrayed in a single file.
 
 If you want to use this package but are not sure your use-case is covered by the current formulation of the package, feel free to open an issue.
 
-## Install
+### Install
 Since PyTorch is a dependency of `h5torch`, we recommend [installing PyTorch](https://pytorch.org/get-started/locally/) independently first, as your system may require a specific version (e.g. CUDA drivers).
 
 After PyTorch installation, `h5torch` can be installed using `pip`
 ```bash
 pip install h5torch
 ```
 
@@ -76,20 +76,20 @@
 Once a dataset is created using `h5torch.File`, it can be used as a PyTorch Dataset using `h5torch.Dataset`. Sampling can occur along any of the axes in the central object, upon which the corresponding indices in the objects aligned to that axis are also sampled. Alternatively, `coo` sampling (available for `N-D` and `coo`-type central objects) samples one specific element of the central dataset, along with the corresponding indices of all axis-aligned objects.
 
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/gdewael/h5torch/main/img/sampling.svg" width="750">
 </p>
 
-## Usage
+### Usage
 
 Refer to the [tutorial on the documentation page](https://h5torch.readthedocs.io/en/latest/tutorial.html).
 
 
-# Package roadmap
+### Package roadmap
 - [x] Implement typing
 - [x] Provide data type conversion capabilities for registering datasets
 - [x] Add support for custom samplers
 - [x] Add support for making data splits
 - [ ] Implement a collater for variable length objects
 - [x] Add a slice sampler
 - [x] Implement a way to pre-specify dataset size and append to it
```

### Comparing `h5torch-0.2.0/README.md` & `h5torch-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 
 [![PyPi Version](https://img.shields.io/pypi/v/h5torch.svg)](https://pypi.python.org/pypi/h5torch/)
 [![GitHub license](https://img.shields.io/github/license/gdewael/h5torch)](https://github.com/gdewael/h5torch/blob/main/LICENSE)
 [![Documentation](https://readthedocs.org/projects/h5torch/badge/?version=latest&style=flat-default)](https://h5torch.readthedocs.io/en/latest/index.html)
 
 </div>
 
-`h5torch` consists of two main parts: (1) `h5torch.File`: a wrapper around `h5py.File` as an interface to create HDF5 files compatible with (2) `h5torch.Dataset`, a wrapper around `torch.utils.data.Dataset`. As a library, `h5torch` establishes a "code" for linking [h5py] and [torch]. To do this, this package has to formulate a vocabulary for how datasets generally look, unifying as many ML settings to the best of its abilities. In turn, this vocabulary allows dataloading of various machine learning data settings from a single dataset class definition, reducing boilerplate in your projects.
+`h5torch` consists of two main parts: (1) `h5torch.File`: a wrapper around `h5py.File` as an interface to create HDF5 files compatible with (2) `h5torch.Dataset`, a wrapper around `torch.utils.data.Dataset`. As a library, `h5torch` establishes a "code" for linking [h5py](https://docs.h5py.org/en/stable/) and [torch](https://pytorch.org/docs/stable/index.html). To do this, this package has to formulate a vocabulary for how datasets generally look, unifying as many ML settings to the best of its abilities. In turn, this vocabulary allows dataloading of various machine learning data settings from a single dataset class definition, reducing boilerplate in your projects.
 
 ### Who is this package for?
 Loading data from HDF5 files allows for efficient data-loading from an **on-disk** format, drastically reducing memory overhead. Additionally, you will find your datasets to be more **organized** using the HDF5 format, as everything is neatly arrayed in a single file.
 
 If you want to use this package but are not sure your use-case is covered by the current formulation of the package, feel free to open an issue.
 
-## Install
+### Install
 Since PyTorch is a dependency of `h5torch`, we recommend [installing PyTorch](https://pytorch.org/get-started/locally/) independently first, as your system may require a specific version (e.g. CUDA drivers).
 
 After PyTorch installation, `h5torch` can be installed using `pip`
 ```bash
 pip install h5torch
 ```
 
@@ -66,20 +66,20 @@
 Once a dataset is created using `h5torch.File`, it can be used as a PyTorch Dataset using `h5torch.Dataset`. Sampling can occur along any of the axes in the central object, upon which the corresponding indices in the objects aligned to that axis are also sampled. Alternatively, `coo` sampling (available for `N-D` and `coo`-type central objects) samples one specific element of the central dataset, along with the corresponding indices of all axis-aligned objects.
 
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/gdewael/h5torch/main/img/sampling.svg" width="750">
 </p>
 
-## Usage
+### Usage
 
 Refer to the [tutorial on the documentation page](https://h5torch.readthedocs.io/en/latest/tutorial.html).
 
 
-# Package roadmap
+### Package roadmap
 - [x] Implement typing
 - [x] Provide data type conversion capabilities for registering datasets
 - [x] Add support for custom samplers
 - [x] Add support for making data splits
 - [ ] Implement a collater for variable length objects
 - [x] Add a slice sampler
 - [x] Implement a way to pre-specify dataset size and append to it
```

### Comparing `h5torch-0.2.0/docs/Makefile` & `h5torch-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `h5torch-0.2.0/docs/make.bat` & `h5torch-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `h5torch-0.2.0/docs/source/conf.py` & `h5torch-0.2.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `h5torch-0.2.0/docs/source/tutorial.ipynb` & `h5torch-0.2.1/docs/source/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `h5torch-0.2.0/h5torch/dataset.py` & `h5torch-0.2.1/h5torch/dataset.py`

 * *Files identical despite different names*

### Comparing `h5torch-0.2.0/h5torch/file.py` & `h5torch-0.2.1/h5torch/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,20 +201,16 @@
             )
         dtype_save_np = default_dtype(data[0], dtype_save)
         dtype_load_np = default_dtype(data[0], dtype_load)
 
         shape = [len(data)]
         if length is not None:
             shape[0] = length
-            self.create_dataset(name, dtype=h5py.vlen_dtype(dtype_save_np), shape=shape)
-            self[name][: len(data)] = [d.astype(dtype_save_np) for d in data]
-        else:
-            self.create_dataset(
-                name, data=data, dtype=h5py.vlen_dtype(dtype_save_np), shape=shape
-            )
+        self.create_dataset(name, dtype=h5py.vlen_dtype(dtype_save_np), shape=shape)
+        self[name][: len(data)] = [d.astype(dtype_save_np) for d in data]
 
         self[name].attrs["shape"] = shape
         self[name].attrs["mode"] = "vlen"
         self[name].attrs["dtypes"] = [str(dtype_save_np), str(dtype_load_np)]
         self[name].attrs["filled_to"] = len(data)
 
     def _separate_register(self, data, name, dtype_save, dtype_load, length):
```

### Comparing `h5torch-0.2.0/h5torch.egg-info/PKG-INFO` & `h5torch-0.2.1/h5torch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5torch
-Version: 0.2.0
+Version: 0.2.1
 Summary: HDF5 data utilities for PyTorch
 Home-page: https://github.com/gdewael/h5torch
 Author: Gaetan De Waele
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -16,22 +16,22 @@
 
 [![PyPi Version](https://img.shields.io/pypi/v/h5torch.svg)](https://pypi.python.org/pypi/h5torch/)
 [![GitHub license](https://img.shields.io/github/license/gdewael/h5torch)](https://github.com/gdewael/h5torch/blob/main/LICENSE)
 [![Documentation](https://readthedocs.org/projects/h5torch/badge/?version=latest&style=flat-default)](https://h5torch.readthedocs.io/en/latest/index.html)
 
 </div>
 
-`h5torch` consists of two main parts: (1) `h5torch.File`: a wrapper around `h5py.File` as an interface to create HDF5 files compatible with (2) `h5torch.Dataset`, a wrapper around `torch.utils.data.Dataset`. As a library, `h5torch` establishes a "code" for linking [h5py] and [torch]. To do this, this package has to formulate a vocabulary for how datasets generally look, unifying as many ML settings to the best of its abilities. In turn, this vocabulary allows dataloading of various machine learning data settings from a single dataset class definition, reducing boilerplate in your projects.
+`h5torch` consists of two main parts: (1) `h5torch.File`: a wrapper around `h5py.File` as an interface to create HDF5 files compatible with (2) `h5torch.Dataset`, a wrapper around `torch.utils.data.Dataset`. As a library, `h5torch` establishes a "code" for linking [h5py](https://docs.h5py.org/en/stable/) and [torch](https://pytorch.org/docs/stable/index.html). To do this, this package has to formulate a vocabulary for how datasets generally look, unifying as many ML settings to the best of its abilities. In turn, this vocabulary allows dataloading of various machine learning data settings from a single dataset class definition, reducing boilerplate in your projects.
 
 ### Who is this package for?
 Loading data from HDF5 files allows for efficient data-loading from an **on-disk** format, drastically reducing memory overhead. Additionally, you will find your datasets to be more **organized** using the HDF5 format, as everything is neatly arrayed in a single file.
 
 If you want to use this package but are not sure your use-case is covered by the current formulation of the package, feel free to open an issue.
 
-## Install
+### Install
 Since PyTorch is a dependency of `h5torch`, we recommend [installing PyTorch](https://pytorch.org/get-started/locally/) independently first, as your system may require a specific version (e.g. CUDA drivers).
 
 After PyTorch installation, `h5torch` can be installed using `pip`
 ```bash
 pip install h5torch
 ```
 
@@ -76,20 +76,20 @@
 Once a dataset is created using `h5torch.File`, it can be used as a PyTorch Dataset using `h5torch.Dataset`. Sampling can occur along any of the axes in the central object, upon which the corresponding indices in the objects aligned to that axis are also sampled. Alternatively, `coo` sampling (available for `N-D` and `coo`-type central objects) samples one specific element of the central dataset, along with the corresponding indices of all axis-aligned objects.
 
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/gdewael/h5torch/main/img/sampling.svg" width="750">
 </p>
 
-## Usage
+### Usage
 
 Refer to the [tutorial on the documentation page](https://h5torch.readthedocs.io/en/latest/tutorial.html).
 
 
-# Package roadmap
+### Package roadmap
 - [x] Implement typing
 - [x] Provide data type conversion capabilities for registering datasets
 - [x] Add support for custom samplers
 - [x] Add support for making data splits
 - [ ] Implement a collater for variable length objects
 - [x] Add a slice sampler
 - [x] Implement a way to pre-specify dataset size and append to it
```

### Comparing `h5torch-0.2.0/h5torch.egg-info/SOURCES.txt` & `h5torch-0.2.1/h5torch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `h5torch-0.2.0/img/centralvsaligned.svg` & `h5torch-0.2.1/img/centralvsaligned.svg`

 * *Files identical despite different names*

### Comparing `h5torch-0.2.0/img/multidim.svg` & `h5torch-0.2.1/img/multidim.svg`

 * *Files identical despite different names*

### Comparing `h5torch-0.2.0/img/sampling.svg` & `h5torch-0.2.1/img/sampling.svg`

 * *Files identical despite different names*

