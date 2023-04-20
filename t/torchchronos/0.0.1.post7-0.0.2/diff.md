# Comparing `tmp/torchchronos-0.0.1.post7.tar.gz` & `tmp/torchchronos-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchchronos-0.0.1.post7.tar", max compression
+gzip compressed data, was "torchchronos-0.0.2.tar", max compression
```

## Comparing `torchchronos-0.0.1.post7.tar` & `torchchronos-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,19 @@
--rw-r--r--   0        0        0     1071 2023-03-27 07:35:04.201640 torchchronos-0.0.1.post7/LICENSE
--rw-r--r--   0        0        0     2551 2023-03-27 07:35:04.201640 torchchronos-0.0.1.post7/README.md
--rw-r--r--   0        0        0      612 2023-03-27 07:35:21.745778 torchchronos-0.0.1.post7/pyproject.toml
--rw-r--r--   0        0        0       19 2023-03-27 07:35:04.201640 torchchronos-0.0.1.post7/torchchronos/__init__.py
--rw-r--r--   0        0        0       72 2023-03-27 07:35:04.201640 torchchronos-0.0.1.post7/torchchronos/datasets/__init__.py
--rw-r--r--   0        0        0     1860 2023-03-27 07:35:21.745778 torchchronos-0.0.1.post7/torchchronos/datasets/ucr_uea_dataset.py
--rw-r--r--   0        0        0     1365 2023-03-27 07:35:04.201640 torchchronos-0.0.1.post7/torchchronos/download.py
--rw-r--r--   0        0        0       40 2023-03-27 07:35:04.201640 torchchronos-0.0.1.post7/torchchronos/lightning/__init__.py
--rw-r--r--   0        0        0     3397 2023-03-27 07:35:04.201640 torchchronos-0.0.1.post7/torchchronos/lightning/ucr_uea_module.py
--rw-r--r--   0        0        0      135 2023-03-27 07:35:04.201640 torchchronos-0.0.1.post7/torchchronos/transforms/__init__.py
--rw-r--r--   0        0        0      868 2023-03-27 07:35:04.201640 torchchronos-0.0.1.post7/torchchronos/transforms/base.py
--rw-r--r--   0        0        0      635 2023-03-27 07:35:04.201640 torchchronos-0.0.1.post7/torchchronos/transforms/padding.py
--rw-r--r--   0        0        0     1338 2023-03-27 07:35:21.745778 torchchronos-0.0.1.post7/torchchronos/utils.py
--rw-r--r--   0        0        0     3273 1970-01-01 00:00:00.000000 torchchronos-0.0.1.post7/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-04-20 08:07:10.115949 torchchronos-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3767 2023-04-20 08:07:10.115949 torchchronos-0.0.2/README.md
+-rw-r--r--   0        0        0      605 2023-04-20 08:07:10.115949 torchchronos-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       19 2023-04-20 08:07:09.667947 torchchronos-0.0.2/torchchronos/__init__.py
+-rw-r--r--   0        0        0      131 2023-04-20 08:07:10.115949 torchchronos-0.0.2/torchchronos/datasets/__init__.py
+-rw-r--r--   0        0        0     3557 2023-04-20 08:07:10.115949 torchchronos-0.0.2/torchchronos/datasets/tfc_pretrain.py
+-rw-r--r--   0        0        0     1841 2023-04-20 08:07:10.115949 torchchronos-0.0.2/torchchronos/datasets/ucr_uea.py
+-rw-r--r--   0        0        0     1860 2023-04-20 08:07:09.667947 torchchronos-0.0.2/torchchronos/datasets/ucr_uea_dataset.py
+-rw-r--r--   0        0        0     1765 2023-04-20 08:07:10.115949 torchchronos-0.0.2/torchchronos/download.py
+-rw-r--r--   0        0        0      143 2023-04-20 08:07:10.115949 torchchronos-0.0.2/torchchronos/lightning/__init__.py
+-rw-r--r--   0        0        0     2320 2023-04-20 08:07:10.115949 torchchronos-0.0.2/torchchronos/lightning/tfc_pretrain.py
+-rw-r--r--   0        0        0     3348 2023-04-20 08:07:10.115949 torchchronos-0.0.2/torchchronos/lightning/ucr_uea.py
+-rw-r--r--   0        0        0     3397 2023-04-20 08:07:09.667947 torchchronos-0.0.2/torchchronos/lightning/ucr_uea_module.py
+-rw-r--r--   0        0        0      135 2023-04-20 08:06:54.531840 torchchronos-0.0.2/torchchronos/transforms/__init__.py
+-rw-r--r--   0        0        0      868 2023-04-20 08:06:54.531840 torchchronos-0.0.2/torchchronos/transforms/base.py
+-rw-r--r--   0        0        0      635 2023-04-20 08:06:54.531840 torchchronos-0.0.2/torchchronos/transforms/padding.py
+-rw-r--r--   0        0        0      202 2023-04-20 08:07:10.115949 torchchronos-0.0.2/torchchronos/typing.py
+-rw-r--r--   0        0        0     1338 2023-04-20 08:06:54.531840 torchchronos-0.0.2/torchchronos/utils.py
+-rw-r--r--   0        0        0     4483 1970-01-01 00:00:00.000000 torchchronos-0.0.2/PKG-INFO
```

### Comparing `torchchronos-0.0.1.post7/LICENSE` & `torchchronos-0.0.2/LICENSE`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023, Maurice Kraus 
+Copyright (c) 2023, Maurice Kraus and Contributors
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `torchchronos-0.0.1.post7/pyproject.toml` & `torchchronos-0.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [tool.poetry]
 name = "torchchronos"
-version = "0.0.1-post7"
+version = "0.0.2"
 authors = ["Maurice Kraus <dev@mkraus.io>"]
 readme = "README.md"
 description = "PyTorch and Lightning compatible library that provides easy and flexible access to various time-series datasets for classification and regression tasks"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 sktime = "^0.16.1"
 torch = "^2.0.0"
 lightning = "^2.0.0"
 fastapi = { version = "^0.88.0" }
 
-
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 pytest = "^7.2.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `torchchronos-0.0.1.post7/torchchronos/datasets/ucr_uea_dataset.py` & `torchchronos-0.0.2/torchchronos/datasets/ucr_uea_dataset.py`

 * *Files identical despite different names*

### Comparing `torchchronos-0.0.1.post7/torchchronos/download.py` & `torchchronos-0.0.2/torchchronos/download.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+import shutil
+import tempfile
+import urllib.request
+import zipfile
 from pathlib import Path
 from typing import Optional
-import zipfile
 
 from sktime.datasets._data_io import _download_and_extract, _list_available_datasets
+from .typing import AnyPath
 
 
-def download_uea_ucr(extract_path: Optional[Path], dataset_name: str):
+def download_uea_ucr(extract_path: Optional[Path], dataset_name: str) -> None:
     """This downloads the uea ucr dataset from sktime to the path extract_path."""
     # Download UCR/UEA archive from sktime
     if extract_path is not None:
         local_dirname = extract_path
     else:
         local_dirname = Path(".cache/data")
     local_dirname.mkdir(parents=True, exist_ok=True)
@@ -27,7 +31,16 @@
             )
         except zipfile.BadZipFile as e:
             raise ValueError(
                 f"Invalid dataset name ={dataset_name} is not available on extract path ="
                 f"{extract_path}. Nor is it available on "
                 f"https://timeseriesclassification.com/.",
             ) from e
+
+
+def download_and_unzip_dataset(url: str, path: AnyPath) -> None:
+    with tempfile.NamedTemporaryFile() as zipped_file:
+        with urllib.request.urlopen(url) as response:
+            shutil.copyfileobj(response, zipped_file)
+
+        with zipfile.ZipFile(zipped_file) as zf:
+            zf.extractall(path)
```

### Comparing `torchchronos-0.0.1.post7/torchchronos/lightning/ucr_uea_module.py` & `torchchronos-0.0.2/torchchronos/lightning/ucr_uea_module.py`

 * *Files identical despite different names*

### Comparing `torchchronos-0.0.1.post7/torchchronos/transforms/base.py` & `torchchronos-0.0.2/torchchronos/transforms/base.py`

 * *Files identical despite different names*

### Comparing `torchchronos-0.0.1.post7/torchchronos/transforms/padding.py` & `torchchronos-0.0.2/torchchronos/transforms/padding.py`

 * *Files identical despite different names*

### Comparing `torchchronos-0.0.1.post7/torchchronos/utils.py` & `torchchronos-0.0.2/torchchronos/utils.py`

 * *Files identical despite different names*

### Comparing `torchchronos-0.0.1.post7/PKG-INFO` & `torchchronos-0.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchchronos
-Version: 0.0.1.post7
+Version: 0.0.2
 Summary: PyTorch and Lightning compatible library that provides easy and flexible access to various time-series datasets for classification and regression tasks
 License: MIT
 Author: Maurice Kraus
 Author-email: dev@mkraus.io
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,53 +13,65 @@
 Requires-Dist: fastapi (>=0.88.0,<0.89.0)
 Requires-Dist: lightning (>=2.0.0,<3.0.0)
 Requires-Dist: sktime (>=0.16.1,<0.17.0)
 Requires-Dist: torch (>=2.0.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # torchchronos
+
+[![PyPI version](https://img.shields.io/pypi/v/torchchronos.svg?color=blue)](https://pypi.org/project/torchchronos)
+[![license](https://img.shields.io/pypi/l/torchchronos.svg?color=blue)](https://github.com/felixdivo/torchchronos/blob/main/LICENSE)
+[![python version](https://img.shields.io/badge/python-3.10+-blue)](https://devguide.python.org/versions/)
+
 [![test](https://github.com/mauricekraus/torchchronos/actions/workflows/main.yml/badge.svg)](https://github.com/mauricekraus/torchchronos/actions/workflows/main.yml)
+[![code style](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
 
-*torchchronos* is an experimental PyTorch and Lightning compatible library that provides easy and flexible access to various time-series datasets for classification and regression tasks. It also provides a simple and extensible transform API to preprocess data.
-It is inspired by the much more complex [torchtime](https://github.com/philipdarke/torchtime).
+*torchchronos* is an experimental [PyTorch](https://pytorch.org/) and [Lightning](https://lightning.ai/pytorch-lightning/) compatible library that provides easy and flexible access to various time-series datasets for classification and regression tasks. It also provides a simple and extensible transform API to preprocess data.
+It is inspired by the much more complicated [torchtime](https://github.com/philipdarke/torchtime).
 
 ## Installation
 You can install torchchronos via pip:
 
 `pip install torchchronos`
 
 ## Usage
 ### Datasets
 torchchronos currently provides access to several popular time-series datasets, including:
 
-- UCR/UEA Time Series Classification Repository
+- [UCR/UEA Time Series Classification Repository](https://www.timeseriesclassification.com/): `torchchronos.datasets.UCRUEADataset`
+- Time series as preprocessed in the [TFC paper](https://github.com/mims-harvard/TFC-pretraining): `torchchronos.datasets.TFCPretrainDataset` (datasets `Gesture` and `EMG`)
 
 To use a dataset, you can simply import the corresponding dataset class and create an instance:
 
 ```python
 from torchchronos.datasets import UCRUEADataset
 from torchchronos.transforms import PadFront
 from torchchronos.download import download_uea_ucr
 
 download_uea_ucr(Path(".cache/data"), "ECG5000")
-dataset = UCRUEADataset('ECG5000',path=Path(".cache/data"), transforms=PadFront(10))
+dataset = UCRUEADataset('ECG5000', path=Path(".cache") / "data", transforms=PadFront(10))
 ```
 
 ### Data Modules
-torchchronos also provides a multi gpu Lightning compatible DataModules to make it easy to load and preprocess data. For example:
+torchchronos also provides [Lightning compatible `DataModules`](https://lightning.ai/docs/pytorch/stable/data/datamodule.html) to make it easy to load and preprocess data. They support common use cases like (multi-)GPU training and train/test/val-splitting out of the box. For example:
 
 ```python
-from torchchronos.lightning import UCRUEAModule
+from torchchronos.lightning import UCRUEADataModule
 from torchchronos.transforms import PadFront, PadBack
 
-module = UCRUEAModule('ECG5000', split_ratio= (0.75, 0.15), batch_size= 32) transforms=Compose([PadFront(10), PadBack(10)]))
+module = UCRUEAModule('ECG5000', split_ratio= (0.75, 0.15), batch_size= 32,
+                      transforms=Compose([PadFront(10), PadBack(10)]))
 ```
 
+Analogous the the datasets above, these dataloaders are supported as of now, wrapping the respective datasets:
+- `torchchronos.lightning.UCRUEADataModule`
+- `torchchronos.lightning.TFCPretrainDataModule`
+
 ### Transforms
-torchchronos provides a flexible transform API to preprocess time-series data. For example, to normalize a dataset, you can define a transform like this:
+torchchronos provides a flexible transform API to preprocess time-series data. For example, to normalize a dataset, you can define a custom `Transform` like this:
 
 ```python
 from torchchronos.transforms import Transform
 
 class Normalize(Transform):
     def __init__(self, mean=None, std=None):
         self.mean = mean
@@ -72,18 +84,18 @@
     def __call__(self, data):
         return (data - self.mean) / self.std
 ```
 
 ## Roadmap
 The following features are planned for future releases of torchchronos:
 
-Support for additional time-series datasets, including:
-- Energy consumption dataset
-- Traffic dataset
-- PhysioNet Challenge 2012 (in-hospital mortality)
-- PhysioNet Challenge 2019 (sepsis prediction) datasets
-Additional transform classes, including:
-- Resampling
-- Missing value imputation
+- Support for additional time-series datasets, including:
+    - Energy consumption dataset
+    - Traffic dataset
+    - PhysioNet Challenge 2012 (in-hospital mortality)
+    - PhysioNet Challenge 2019 (sepsis prediction) datasets
+- Additional transform classes, including:
+    - Resampling
+    - Missing value imputation
 
 If you have any feature requests or suggestions, please open an issue on our GitHub page.
```

