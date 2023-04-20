# Comparing `tmp/openchord-0.1.0.tar.gz` & `tmp/openchord-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openchord-0.1.0.tar", last modified: Thu Apr 20 15:39:15 2023, max compression
+gzip compressed data, was "openchord-0.1.1.tar", last modified: Thu Apr 20 16:29:50 2023, max compression
```

## Comparing `openchord-0.1.0.tar` & `openchord-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxr-x   0 kenny     (1000) kenny     (1000)        0 2023-04-20 15:39:15.138502 openchord-0.1.0/
--rw-rw-r--   0 kenny     (1000) kenny     (1000)    35149 2023-04-20 13:29:24.000000 openchord-0.1.0/LICENSE
--rw-rw-r--   0 kenny     (1000) kenny     (1000)     2252 2023-04-20 15:39:15.138502 openchord-0.1.0/PKG-INFO
--rw-rw-r--   0 kenny     (1000) kenny     (1000)     1735 2023-04-20 13:29:24.000000 openchord-0.1.0/README.md
--rw-rw-r--   0 kenny     (1000) kenny     (1000)      675 2023-04-20 15:39:08.000000 openchord-0.1.0/pyproject.toml
--rw-rw-r--   0 kenny     (1000) kenny     (1000)       38 2023-04-20 15:39:15.142502 openchord-0.1.0/setup.cfg
-drwxrwxr-x   0 kenny     (1000) kenny     (1000)        0 2023-04-20 15:39:15.134502 openchord-0.1.0/src/
-drwxrwxr-x   0 kenny     (1000) kenny     (1000)        0 2023-04-20 15:39:15.138502 openchord-0.1.0/src/openchord/
--rw-rw-r--   0 kenny     (1000) kenny     (1000)        0 2023-04-20 13:36:13.000000 openchord-0.1.0/src/openchord/__init__.py
--rw-rw-r--   0 kenny     (1000) kenny     (1000)     6261 2023-04-20 13:29:24.000000 openchord-0.1.0/src/openchord/openchord.py
-drwxrwxr-x   0 kenny     (1000) kenny     (1000)        0 2023-04-20 15:39:15.138502 openchord-0.1.0/src/openchord.egg-info/
--rw-rw-r--   0 kenny     (1000) kenny     (1000)     2252 2023-04-20 15:39:15.000000 openchord-0.1.0/src/openchord.egg-info/PKG-INFO
--rw-rw-r--   0 kenny     (1000) kenny     (1000)      269 2023-04-20 15:39:15.000000 openchord-0.1.0/src/openchord.egg-info/SOURCES.txt
--rw-rw-r--   0 kenny     (1000) kenny     (1000)        1 2023-04-20 15:39:15.000000 openchord-0.1.0/src/openchord.egg-info/dependency_links.txt
--rw-rw-r--   0 kenny     (1000) kenny     (1000)       20 2023-04-20 15:39:15.000000 openchord-0.1.0/src/openchord.egg-info/requires.txt
--rw-rw-r--   0 kenny     (1000) kenny     (1000)       10 2023-04-20 15:39:15.000000 openchord-0.1.0/src/openchord.egg-info/top_level.txt
+drwxrwxr-x   0 kenny     (1000) kenny     (1000)        0 2023-04-20 16:29:50.523512 openchord-0.1.1/
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)    35149 2023-04-20 13:29:24.000000 openchord-0.1.1/LICENSE
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)     2253 2023-04-20 16:29:50.523512 openchord-0.1.1/PKG-INFO
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)     1736 2023-04-20 16:03:05.000000 openchord-0.1.1/README.md
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)      675 2023-04-20 16:29:42.000000 openchord-0.1.1/pyproject.toml
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)       38 2023-04-20 16:29:50.523512 openchord-0.1.1/setup.cfg
+drwxrwxr-x   0 kenny     (1000) kenny     (1000)        0 2023-04-20 16:29:50.519512 openchord-0.1.1/src/
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)        0 2023-04-20 13:36:13.000000 openchord-0.1.1/src/__init__.py
+drwxrwxr-x   0 kenny     (1000) kenny     (1000)        0 2023-04-20 16:29:50.523512 openchord-0.1.1/src/openchord.egg-info/
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)     2253 2023-04-20 16:29:50.000000 openchord-0.1.1/src/openchord.egg-info/PKG-INFO
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)      249 2023-04-20 16:29:50.000000 openchord-0.1.1/src/openchord.egg-info/SOURCES.txt
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)        1 2023-04-20 16:29:50.000000 openchord-0.1.1/src/openchord.egg-info/dependency_links.txt
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)       20 2023-04-20 16:29:50.000000 openchord-0.1.1/src/openchord.egg-info/requires.txt
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)       19 2023-04-20 16:29:50.000000 openchord-0.1.1/src/openchord.egg-info/top_level.txt
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)     6261 2023-04-20 13:29:24.000000 openchord-0.1.1/src/openchord.py
```

### Comparing `openchord-0.1.0/LICENSE` & `openchord-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openchord-0.1.0/PKG-INFO` & `openchord-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openchord
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library for ploting chord diagrams
 Author-email: Kenny Pang <pangkhangee@gmail.com>
 Project-URL: Homepage, https://github.com/pke1029/open-chord
 Keywords: plot,data science,Jupyter,network,graph
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -30,15 +30,15 @@
 import openchord as ocd
 
 adjacency_matrix = [[ 3, 18,  9,  0, 23],
                     [18,  0, 12,  5, 29],
                     [ 9, 12,  0, 27, 10],
                     [ 0,  5, 27,  0,  0],
                     [23, 29, 10,  0,  0]]
-labels = [Emma', 'Isabella', 'Ava', 'Olivia', 'Sophia']
+labels = ['Emma', 'Isabella', 'Ava', 'Olivia', 'Sophia']
 
 fig = ocd.Chord(adjacency_matrix, labels)
 fig.show()
 ```
 Color can be changed like so
 ```python
 fig.color_map = ['#636EFA', '#EF553B', '#00CC96', '#AB63FA', '#FFA15A', '#19D3F3', '#FF6692', '#B6E880', '#FF97FF', '#FECB52']
```

### Comparing `openchord-0.1.0/README.md` & `openchord-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import openchord as ocd
 
 adjacency_matrix = [[ 3, 18,  9,  0, 23],
                     [18,  0, 12,  5, 29],
                     [ 9, 12,  0, 27, 10],
                     [ 0,  5, 27,  0,  0],
                     [23, 29, 10,  0,  0]]
-labels = [Emma', 'Isabella', 'Ava', 'Olivia', 'Sophia']
+labels = ['Emma', 'Isabella', 'Ava', 'Olivia', 'Sophia']
 
 fig = ocd.Chord(adjacency_matrix, labels)
 fig.show()
 ```
 Color can be changed like so
 ```python
 fig.color_map = ['#636EFA', '#EF553B', '#00CC96', '#AB63FA', '#FFA15A', '#19D3F3', '#FF6692', '#B6E880', '#FF97FF', '#FECB52']
```

### Comparing `openchord-0.1.0/pyproject.toml` & `openchord-0.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openchord"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     {name = "Kenny Pang", email = "pangkhangee@gmail.com"},
 ]
 description = "A library for ploting chord diagrams"
 readme = "README.md"
 requires-python = ">=3.6"
 keywords = ["plot", "data science", "Jupyter", "network", "graph"]
```

### Comparing `openchord-0.1.0/src/openchord/openchord.py` & `openchord-0.1.1/src/openchord.py`

 * *Files identical despite different names*

### Comparing `openchord-0.1.0/src/openchord.egg-info/PKG-INFO` & `openchord-0.1.1/src/openchord.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openchord
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library for ploting chord diagrams
 Author-email: Kenny Pang <pangkhangee@gmail.com>
 Project-URL: Homepage, https://github.com/pke1029/open-chord
 Keywords: plot,data science,Jupyter,network,graph
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -30,15 +30,15 @@
 import openchord as ocd
 
 adjacency_matrix = [[ 3, 18,  9,  0, 23],
                     [18,  0, 12,  5, 29],
                     [ 9, 12,  0, 27, 10],
                     [ 0,  5, 27,  0,  0],
                     [23, 29, 10,  0,  0]]
-labels = [Emma', 'Isabella', 'Ava', 'Olivia', 'Sophia']
+labels = ['Emma', 'Isabella', 'Ava', 'Olivia', 'Sophia']
 
 fig = ocd.Chord(adjacency_matrix, labels)
 fig.show()
 ```
 Color can be changed like so
 ```python
 fig.color_map = ['#636EFA', '#EF553B', '#00CC96', '#AB63FA', '#FFA15A', '#19D3F3', '#FF6692', '#B6E880', '#FF97FF', '#FECB52']
```

