# Comparing `tmp/datamodelsFrontier-1.2.3.tar.gz` & `tmp/datamodelsFrontier-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamodelsFrontier-1.2.3.tar", last modified: Tue Apr 18 15:51:17 2023, max compression
+gzip compressed data, was "datamodelsFrontier-1.2.4.tar", last modified: Thu Apr 20 13:38:39 2023, max compression
```

## Comparing `datamodelsFrontier-1.2.3.tar` & `datamodelsFrontier-1.2.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:51:17.776777 datamodelsFrontier-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-18 15:51:07.000000 datamodelsFrontier-1.2.3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-18 15:51:07.000000 datamodelsFrontier-1.2.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-18 15:51:07.000000 datamodelsFrontier-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-18 15:51:17.776777 datamodelsFrontier-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-18 15:51:07.000000 datamodelsFrontier-1.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 15:51:17.776777 datamodelsFrontier-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-18 15:51:07.000000 datamodelsFrontier-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:51:17.776777 datamodelsFrontier-1.2.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:51:07.000000 datamodelsFrontier-1.2.3/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:51:17.776777 datamodelsFrontier-1.2.3/src/datamodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:51:07.000000 datamodelsFrontier-1.2.3/src/datamodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-18 15:51:07.000000 datamodelsFrontier-1.2.3/src/datamodels/downstream.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-18 15:51:07.000000 datamodelsFrontier-1.2.3/src/datamodels/external.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:51:17.776777 datamodelsFrontier-1.2.3/src/datamodelsFrontier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-18 15:51:17.000000 datamodelsFrontier-1.2.3/src/datamodelsFrontier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-18 15:51:17.000000 datamodelsFrontier-1.2.3/src/datamodelsFrontier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:51:17.000000 datamodelsFrontier-1.2.3/src/datamodelsFrontier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-18 15:51:17.000000 datamodelsFrontier-1.2.3/src/datamodelsFrontier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-18 15:51:17.000000 datamodelsFrontier-1.2.3/src/datamodelsFrontier.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:51:17.776777 datamodelsFrontier-1.2.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:51:07.000000 datamodelsFrontier-1.2.3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-18 15:51:07.000000 datamodelsFrontier-1.2.3/test/test_downstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-18 15:51:07.000000 datamodelsFrontier-1.2.3/test/test_external.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:38:39.047784 datamodelsFrontier-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-20 13:38:26.000000 datamodelsFrontier-1.2.4/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-20 13:38:26.000000 datamodelsFrontier-1.2.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-20 13:38:26.000000 datamodelsFrontier-1.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-20 13:38:39.047784 datamodelsFrontier-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-20 13:38:26.000000 datamodelsFrontier-1.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 13:38:39.047784 datamodelsFrontier-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-20 13:38:26.000000 datamodelsFrontier-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:38:39.043784 datamodelsFrontier-1.2.4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:38:26.000000 datamodelsFrontier-1.2.4/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:38:39.043784 datamodelsFrontier-1.2.4/src/datamodelsFrontier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:38:26.000000 datamodelsFrontier-1.2.4/src/datamodelsFrontier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-20 13:38:26.000000 datamodelsFrontier-1.2.4/src/datamodelsFrontier/downstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-20 13:38:26.000000 datamodelsFrontier-1.2.4/src/datamodelsFrontier/external.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:38:39.047784 datamodelsFrontier-1.2.4/src/datamodelsFrontier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-20 13:38:38.000000 datamodelsFrontier-1.2.4/src/datamodelsFrontier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-20 13:38:39.000000 datamodelsFrontier-1.2.4/src/datamodelsFrontier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 13:38:38.000000 datamodelsFrontier-1.2.4/src/datamodelsFrontier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-20 13:38:38.000000 datamodelsFrontier-1.2.4/src/datamodelsFrontier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-20 13:38:38.000000 datamodelsFrontier-1.2.4/src/datamodelsFrontier.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:38:39.047784 datamodelsFrontier-1.2.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:38:26.000000 datamodelsFrontier-1.2.4/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-20 13:38:26.000000 datamodelsFrontier-1.2.4/test/test_downstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-20 13:38:26.000000 datamodelsFrontier-1.2.4/test/test_external.py
```

### Comparing `datamodelsFrontier-1.2.3/LICENSE.txt` & `datamodelsFrontier-1.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datamodelsFrontier-1.2.3/PKG-INFO` & `datamodelsFrontier-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamodelsFrontier
-Version: 1.2.3
+Version: 1.2.4
 Summary: Datamodels needed for Frontier API
 Home-page: UNKNOWN
 Author: THG-Frontier
 Author-email: DL-TechAPIGateway@thehutgroup.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -28,17 +28,17 @@
 
 *Command Line*
 ```bash
 $ pip install datamodelsFrontier
 ```
 *Python*
 ```python
-from datamodels.external import Barcode
+from datamodelsFrontier.external import Barcode
 
-from datamodels.downstream import ChildProduct
+from datamodelsFrotnier.downstream import ChildProduct
 ```
 
 
 ### Code Information
 #### Example Code:
 ```python
 InventoryItemDimension(height_mm=3, width_mm=4, depth_mm=5, mass_kg=5)
```

### Comparing `datamodelsFrontier-1.2.3/setup.py` & `datamodelsFrontier-1.2.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 import os
 
 # Open readme when package starts
-with open("README.md", "r") as fh:
+with open("pypi-description.md", "r") as fh:
     long_description = fh.read()
 
 # Read the version number from the environment variable
 version = os.getenv('PACKAGE_VERSION', '0.0.0')
 
 # Dependencies
 extra_test = [
```

### Comparing `datamodelsFrontier-1.2.3/src/datamodels/external.py` & `datamodelsFrontier-1.2.4/src/datamodelsFrontier/external.py`

 * *Files identical despite different names*

### Comparing `datamodelsFrontier-1.2.3/src/datamodelsFrontier.egg-info/PKG-INFO` & `datamodelsFrontier-1.2.4/src/datamodelsFrontier.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamodelsFrontier
-Version: 1.2.3
+Version: 1.2.4
 Summary: Datamodels needed for Frontier API
 Home-page: UNKNOWN
 Author: THG-Frontier
 Author-email: DL-TechAPIGateway@thehutgroup.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -28,17 +28,17 @@
 
 *Command Line*
 ```bash
 $ pip install datamodelsFrontier
 ```
 *Python*
 ```python
-from datamodels.external import Barcode
+from datamodelsFrontier.external import Barcode
 
-from datamodels.downstream import ChildProduct
+from datamodelsFrotnier.downstream import ChildProduct
 ```
 
 
 ### Code Information
 #### Example Code:
 ```python
 InventoryItemDimension(height_mm=3, width_mm=4, depth_mm=5, mass_kg=5)
```

### Comparing `datamodelsFrontier-1.2.3/test/test_downstream.py` & `datamodelsFrontier-1.2.4/test/test_downstream.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from src.datamodels.downstream import ChildProduct
+from src.datamodelsFrontier.downstream import ChildProduct
 
 
 def test_child_product():
     cp = ChildProduct(
         id="id",
         title="title",
         barcode="barcode",
```

### Comparing `datamodelsFrontier-1.2.3/test/test_external.py` & `datamodelsFrontier-1.2.4/test/test_external.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from src.datamodels.external import InventoryItemDimension
-from src.datamodels.external import Barcode
-from src.datamodels.external import InventoryItem
+from src.datamodelsFrontier.external import InventoryItemDimension
+from src.datamodelsFrontier.external import Barcode
+from src.datamodelsFrontier.external import InventoryItem
 
 
 def test_inventory_item_dimension():
     iid = InventoryItemDimension(height_mm=3, width_mm=4, depth_mm=5, mass_kg=5)
     assert iid.height_mm == 3
     assert iid.width_mm == 4
     assert iid.depth_mm == 5
```

