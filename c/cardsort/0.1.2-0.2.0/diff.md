# Comparing `tmp/cardsort-0.1.2.tar.gz` & `tmp/cardsort-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardsort-0.1.2.tar", max compression
+gzip compressed data, was "cardsort-0.2.0.tar", max compression
```

## Comparing `cardsort-0.1.2.tar` & `cardsort-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rwxr-xr-x   0        0        0     1077 2023-03-22 16:10:05.525809 cardsort-0.1.2/LICENSE
--rw-r--r--   0        0        0     2251 2023-03-28 12:33:31.490638 cardsort-0.1.2/README.md
--rw-r--r--   0        0        0      615 2023-03-28 11:53:56.177826 cardsort-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      110 2023-03-16 12:18:44.253758 cardsort-0.1.2/src/cardsort/__init__.py
--rw-r--r--   0        0        0     9780 2023-03-21 14:56:00.370940 cardsort-0.1.2/src/cardsort/analysis.py
--rw-r--r--   0        0        0     3089 1970-01-01 00:00:00.000000 cardsort-0.1.2/setup.py
--rw-r--r--   0        0        0     2912 1970-01-01 00:00:00.000000 cardsort-0.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1077 2023-04-20 10:05:19.419947 cardsort-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2320 2023-04-20 10:05:19.419947 cardsort-0.2.0/README.md
+-rw-r--r--   0        0        0     1330 2023-04-20 10:06:11.984773 cardsort-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-04-20 10:05:19.423947 cardsort-0.2.0/src/cardsort/__init__.py
+-rw-r--r--   0        0        0     9780 2023-04-20 10:05:19.423947 cardsort-0.2.0/src/cardsort/analysis.py
+-rw-r--r--   0        0        0     3034 1970-01-01 00:00:00.000000 cardsort-0.2.0/PKG-INFO
```

### Comparing `cardsort-0.1.2/LICENSE` & `cardsort-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cardsort-0.1.2/README.md` & `cardsort-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 ## Table of Contents
 
 - [Documentation](#documentation)
 - [Quick start](#quick-start)
   - [Installation](#installation)
   - [Usage](#usage)
   - [Accepted data](#accepted-data)
+  - [Advanced usage](#advanced-usage)
 - [Contributing](#contributing)
 - [License](#license)
 - [Credits](#credits)
 
 ## Documentation
 [cardsort.readthedocs.io](https://cardsort.readthedocs.io)
 
@@ -34,38 +35,40 @@
 
 ```python
 from cardsort import analysis
 import pandas as pd
 
 path = "example-data.csv" # data with columns: card_id, card_label, category_id, category_label, user_id
 df = pd.read_csv(path) 
-
-# create a dendrogram that summarized user-generated clusters
+```
+__Create a dendrogram that summarizes user-generated clusters__
+```python
 analysis.create_dendrogram(df)
 ```
 
 __Output__
 
 ![Dendrogram plot generated from example data](https://github.com/katoss/cardsort/blob/main/docs/dendrogram.png?raw=true)
 
+__Learn which category labels users gave to clusters__
 ```python
-# learn which category labels users gave to clusters
 cards = ['Banana', 'Apple']
 analysis.get_cluster_labels(df, cards)
 ```
 __Output__
-
+```python
 ['Healthy snacks', 'Snacks', 'Fruits', 'Food']
-
+```
 
 ### Accepted data
 * This package works with data exports from [kardsort.com](https://kardsort.com/) (Export format 'Casolysis Data (.csv) - Recommended')
 * This data equals the following structure: ```card_id, card_label, category_id, category_label, user_id```
 
-See the [documentation](https://cardsort.readthedocs.io) for details.
+### Advanced usage
+See [documentation](https://cardsort.readthedocs.io)
 
 ## Contributing
 
 Interested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.
 
 ## License
```

### Comparing `cardsort-0.1.2/src/cardsort/analysis.py` & `cardsort-0.2.0/src/cardsort/analysis.py`

 * *Files identical despite different names*

### Comparing `cardsort-0.1.2/PKG-INFO` & `cardsort-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: cardsort
-Version: 0.1.2
-Summary: Analyse cardsorting data
+Version: 0.2.0
+Summary: Analyse data from open card sorting
 License: MIT
 Author: Katharina Kloppenborg
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
+Requires-Dist: myst-nb (>=0.17.1,<0.18.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Cardsort analysis
 
@@ -29,14 +30,15 @@
 ## Table of Contents
 
 - [Documentation](#documentation)
 - [Quick start](#quick-start)
   - [Installation](#installation)
   - [Usage](#usage)
   - [Accepted data](#accepted-data)
+  - [Advanced usage](#advanced-usage)
 - [Contributing](#contributing)
 - [License](#license)
 - [Credits](#credits)
 
 ## Documentation
 [cardsort.readthedocs.io](https://cardsort.readthedocs.io)
 
@@ -53,38 +55,40 @@
 
 ```python
 from cardsort import analysis
 import pandas as pd
 
 path = "example-data.csv" # data with columns: card_id, card_label, category_id, category_label, user_id
 df = pd.read_csv(path) 
-
-# create a dendrogram that summarized user-generated clusters
+```
+__Create a dendrogram that summarizes user-generated clusters__
+```python
 analysis.create_dendrogram(df)
 ```
 
 __Output__
 
 ![Dendrogram plot generated from example data](https://github.com/katoss/cardsort/blob/main/docs/dendrogram.png?raw=true)
 
+__Learn which category labels users gave to clusters__
 ```python
-# learn which category labels users gave to clusters
 cards = ['Banana', 'Apple']
 analysis.get_cluster_labels(df, cards)
 ```
 __Output__
-
+```python
 ['Healthy snacks', 'Snacks', 'Fruits', 'Food']
-
+```
 
 ### Accepted data
 * This package works with data exports from [kardsort.com](https://kardsort.com/) (Export format 'Casolysis Data (.csv) - Recommended')
 * This data equals the following structure: ```card_id, card_label, category_id, category_label, user_id```
 
-See the [documentation](https://cardsort.readthedocs.io) for details.
+### Advanced usage
+See [documentation](https://cardsort.readthedocs.io)
 
 ## Contributing
 
 Interested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.
 
 ## License
```

