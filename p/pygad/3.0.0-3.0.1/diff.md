# Comparing `tmp/pygad-3.0.0.tar.gz` & `tmp/pygad-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygad-3.0.0.tar", last modified: Sat Apr  8 18:31:16 2023, max compression
+gzip compressed data, was "pygad-3.0.1.tar", last modified: Thu Apr 20 13:31:16 2023, max compression
```

## Comparing `pygad-3.0.0.tar` & `pygad-3.0.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-08 18:31:16.373571 pygad-3.0.0/
--rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)    18208 2023-04-08 18:31:16.373571 pygad-3.0.0/PKG-INFO
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    17829 2023-04-08 18:12:48.000000 pygad-3.0.0/README.md
-drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-08 18:31:16.373571 pygad-3.0.0/pygad/
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       63 2023-04-03 22:14:20.000000 pygad-3.0.0/pygad/__init__.py
-drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-08 18:31:16.373571 pygad-3.0.0/pygad/cnn/
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       43 2023-02-23 13:33:40.000000 pygad-3.0.0/pygad/cnn/__init__.py
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    37968 2023-02-23 13:33:40.000000 pygad-3.0.0/pygad/cnn/cnn.py
-drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-08 18:31:16.373571 pygad-3.0.0/pygad/gacnn/
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       45 2023-02-23 13:33:40.000000 pygad-3.0.0/pygad/gacnn/__init__.py
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)     5166 2023-02-23 13:33:40.000000 pygad-3.0.0/pygad/gacnn/gacnn.py
-drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-08 18:31:16.373571 pygad-3.0.0/pygad/gann/
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       44 2023-02-23 13:33:40.000000 pygad-3.0.0/pygad/gann/__init__.py
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    21058 2023-02-23 13:33:40.000000 pygad-3.0.0/pygad/gann/gann.py
-drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-08 18:31:16.373571 pygad-3.0.0/pygad/helper/
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       54 2023-04-03 22:17:26.000000 pygad-3.0.0/pygad/helper/__init__.py
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    47690 2023-02-28 16:43:38.000000 pygad-3.0.0/pygad/helper/unique.py
-drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-08 18:31:16.373571 pygad-3.0.0/pygad/kerasga/
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       46 2023-04-03 22:17:19.000000 pygad-3.0.0/pygad/kerasga/__init__.py
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)     3243 2023-03-01 16:53:25.000000 pygad-3.0.0/pygad/kerasga/kerasga.py
-drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-08 18:31:16.373571 pygad-3.0.0/pygad/nn/
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       42 2023-02-23 13:33:40.000000 pygad-3.0.0/pygad/nn/__init__.py
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    19363 2023-02-23 13:33:40.000000 pygad-3.0.0/pygad/nn/nn.py
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)   217101 2023-04-03 22:10:55.000000 pygad-3.0.0/pygad/pygad.py
-drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-08 18:31:16.373571 pygad-3.0.0/pygad/torchga/
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       46 2023-04-03 22:17:09.000000 pygad-3.0.0/pygad/torchga/__init__.py
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)     3362 2023-03-01 17:53:14.000000 pygad-3.0.0/pygad/torchga/torchga.py
-drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-08 18:31:16.373571 pygad-3.0.0/pygad/utils/
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)      130 2023-04-03 22:16:41.000000 pygad-3.0.0/pygad/utils/__init__.py
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    13968 2023-03-02 02:30:43.000000 pygad-3.0.0/pygad/utils/crossover.py
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    53487 2023-03-02 02:41:53.000000 pygad-3.0.0/pygad/utils/mutation.py
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    10106 2023-04-03 22:10:06.000000 pygad-3.0.0/pygad/utils/parent_selection.py
-drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-08 18:31:16.373571 pygad-3.0.0/pygad/visualize/
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       55 2023-04-03 22:16:52.000000 pygad-3.0.0/pygad/visualize/__init__.py
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    18572 2023-02-28 16:43:27.000000 pygad-3.0.0/pygad/visualize/plot.py
-drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-08 18:31:16.373571 pygad-3.0.0/pygad.egg-info/
--rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)    18208 2023-04-08 18:31:16.000000 pygad-3.0.0/pygad.egg-info/PKG-INFO
--rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)      664 2023-04-08 18:31:16.000000 pygad-3.0.0/pygad.egg-info/SOURCES.txt
--rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)        1 2023-04-08 18:31:16.000000 pygad-3.0.0/pygad.egg-info/dependency_links.txt
--rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)       29 2023-04-08 18:31:16.000000 pygad-3.0.0/pygad.egg-info/requires.txt
--rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)        6 2023-04-08 18:31:16.000000 pygad-3.0.0/pygad.egg-info/top_level.txt
--rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)       38 2023-04-08 18:31:16.373571 pygad-3.0.0/setup.cfg
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)      637 2023-04-08 18:19:58.000000 pygad-3.0.0/setup.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-20 13:31:16.074518 pygad-3.0.1/
+-rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)    18208 2023-04-20 13:31:16.074518 pygad-3.0.1/PKG-INFO
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    17829 2023-04-08 18:12:48.000000 pygad-3.0.1/README.md
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-20 13:31:16.018519 pygad-3.0.1/pygad/
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       63 2023-04-20 13:25:25.000000 pygad-3.0.1/pygad/__init__.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-20 13:31:16.022519 pygad-3.0.1/pygad/cnn/
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       43 2023-02-23 13:33:40.000000 pygad-3.0.1/pygad/cnn/__init__.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    37968 2023-02-23 13:33:40.000000 pygad-3.0.1/pygad/cnn/cnn.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-20 13:31:16.022519 pygad-3.0.1/pygad/gacnn/
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       45 2023-02-23 13:33:40.000000 pygad-3.0.1/pygad/gacnn/__init__.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)     5166 2023-02-23 13:33:40.000000 pygad-3.0.1/pygad/gacnn/gacnn.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-20 13:31:16.026519 pygad-3.0.1/pygad/gann/
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       44 2023-02-23 13:33:40.000000 pygad-3.0.1/pygad/gann/__init__.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    21058 2023-02-23 13:33:40.000000 pygad-3.0.1/pygad/gann/gann.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-20 13:31:16.026519 pygad-3.0.1/pygad/helper/
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       54 2023-04-03 22:17:26.000000 pygad-3.0.1/pygad/helper/__init__.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    47690 2023-02-28 16:43:38.000000 pygad-3.0.1/pygad/helper/unique.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-20 13:31:16.030519 pygad-3.0.1/pygad/kerasga/
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       46 2023-04-03 22:17:19.000000 pygad-3.0.1/pygad/kerasga/__init__.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)     3243 2023-03-01 16:53:25.000000 pygad-3.0.1/pygad/kerasga/kerasga.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-20 13:31:16.038519 pygad-3.0.1/pygad/nn/
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       42 2023-02-23 13:33:40.000000 pygad-3.0.1/pygad/nn/__init__.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    19363 2023-02-23 13:33:40.000000 pygad-3.0.1/pygad/nn/nn.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)   217095 2023-04-20 13:24:25.000000 pygad-3.0.1/pygad/pygad.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-20 13:31:16.050518 pygad-3.0.1/pygad/torchga/
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       46 2023-04-03 22:17:09.000000 pygad-3.0.1/pygad/torchga/__init__.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)     3362 2023-03-01 17:53:14.000000 pygad-3.0.1/pygad/torchga/torchga.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-20 13:31:16.058518 pygad-3.0.1/pygad/utils/
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)      130 2023-04-03 22:16:41.000000 pygad-3.0.1/pygad/utils/__init__.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    13968 2023-03-02 02:30:43.000000 pygad-3.0.1/pygad/utils/crossover.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    53487 2023-03-02 02:41:53.000000 pygad-3.0.1/pygad/utils/mutation.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    10106 2023-04-03 22:10:06.000000 pygad-3.0.1/pygad/utils/parent_selection.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-20 13:31:16.062518 pygad-3.0.1/pygad/visualize/
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       55 2023-04-03 22:16:52.000000 pygad-3.0.1/pygad/visualize/__init__.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    18572 2023-02-28 16:43:27.000000 pygad-3.0.1/pygad/visualize/plot.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-20 13:31:16.022519 pygad-3.0.1/pygad.egg-info/
+-rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)    18208 2023-04-20 13:31:15.000000 pygad-3.0.1/pygad.egg-info/PKG-INFO
+-rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)      664 2023-04-20 13:31:15.000000 pygad-3.0.1/pygad.egg-info/SOURCES.txt
+-rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)        1 2023-04-20 13:31:15.000000 pygad-3.0.1/pygad.egg-info/dependency_links.txt
+-rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)       29 2023-04-20 13:31:15.000000 pygad-3.0.1/pygad.egg-info/requires.txt
+-rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)        6 2023-04-20 13:31:15.000000 pygad-3.0.1/pygad.egg-info/top_level.txt
+-rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)       38 2023-04-20 13:31:16.074518 pygad-3.0.1/setup.cfg
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)      637 2023-04-20 13:29:39.000000 pygad-3.0.1/setup.py
```

### Comparing `pygad-3.0.0/PKG-INFO` & `pygad-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygad
-Version: 3.0.0
+Version: 3.0.1
 Summary: PyGAD: A Python 3 Library for Building the Genetic Algorithm and Training Machine Learning Algoithms (Keras & PyTorch).
 Home-page: https://github.com/ahmedfgad/GeneticAlgorithmPython
 Author: Ahmed Fawzy Gad
 Author-email: ahmed.f.gad@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pygad-3.0.0/README.md` & `pygad-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pygad-3.0.0/pygad/cnn/cnn.py` & `pygad-3.0.1/pygad/cnn/cnn.py`

 * *Files identical despite different names*

### Comparing `pygad-3.0.0/pygad/gacnn/gacnn.py` & `pygad-3.0.1/pygad/gacnn/gacnn.py`

 * *Files identical despite different names*

### Comparing `pygad-3.0.0/pygad/gann/gann.py` & `pygad-3.0.1/pygad/gann/gann.py`

 * *Files identical despite different names*

### Comparing `pygad-3.0.0/pygad/helper/unique.py` & `pygad-3.0.1/pygad/helper/unique.py`

 * *Files identical despite different names*

### Comparing `pygad-3.0.0/pygad/kerasga/kerasga.py` & `pygad-3.0.1/pygad/kerasga/kerasga.py`

 * *Files identical despite different names*

### Comparing `pygad-3.0.0/pygad/nn/nn.py` & `pygad-3.0.1/pygad/nn/nn.py`

 * *Files identical despite different names*

### Comparing `pygad-3.0.0/pygad/pygad.py` & `pygad-3.0.1/pygad/pygad.py`

 * *Files 0% similar despite different names*

```diff
@@ -1743,17 +1743,17 @@
                 population_as_list = [list(item) for item in population_as_list]
                 self.solutions.extend(population_as_list)
 
                 self.solutions_fitness.extend(self.last_generation_fitness)
 
             # Selecting the best parents in the population for mating.
             if callable(self.parent_selection_type):
-                self.last_generation_parents, self.last_generation_parents_indices = self.select_parents(self, 
-                                                                                                         self.last_generation_fitness, 
-                                                                                                         self.num_parents_mating, self)
+                self.last_generation_parents, self.last_generation_parents_indices = self.select_parents(self.last_generation_fitness, 
+                                                                                                         self.num_parents_mating, 
+                                                                                                         self)
                 if not type(self.last_generation_parents) is numpy.ndarray:
                     self.logger.error("The type of the iterable holding the selected parents is expected to be (numpy.ndarray) but {last_generation_parents_type} found.".format(last_generation_parents_type=type(self.last_generation_parents)))
                     raise TypeError("The type of the iterable holding the selected parents is expected to be (numpy.ndarray) but {last_generation_parents_type} found.".format(last_generation_parents_type=type(self.last_generation_parents)))
                 if not type(self.last_generation_parents_indices) is numpy.ndarray:
                     self.logger.error("The type of the iterable holding the selected parents' indices is expected to be (numpy.ndarray) but {last_generation_parents_indices_type} found.".format(last_generation_parents_indices_type=type(self.last_generation_parents_indices)))
                     raise TypeError("The type of the iterable holding the selected parents' indices is expected to be (numpy.ndarray) but {last_generation_parents_indices_type} found.".format(last_generation_parents_indices_type=type(self.last_generation_parents_indices)))
             else:
```

### Comparing `pygad-3.0.0/pygad/torchga/torchga.py` & `pygad-3.0.1/pygad/torchga/torchga.py`

 * *Files identical despite different names*

### Comparing `pygad-3.0.0/pygad/utils/crossover.py` & `pygad-3.0.1/pygad/utils/crossover.py`

 * *Files identical despite different names*

### Comparing `pygad-3.0.0/pygad/utils/mutation.py` & `pygad-3.0.1/pygad/utils/mutation.py`

 * *Files identical despite different names*

### Comparing `pygad-3.0.0/pygad/utils/parent_selection.py` & `pygad-3.0.1/pygad/utils/parent_selection.py`

 * *Files identical despite different names*

### Comparing `pygad-3.0.0/pygad/visualize/plot.py` & `pygad-3.0.1/pygad/visualize/plot.py`

 * *Files identical despite different names*

### Comparing `pygad-3.0.0/pygad.egg-info/PKG-INFO` & `pygad-3.0.1/pygad.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygad
-Version: 3.0.0
+Version: 3.0.1
 Summary: PyGAD: A Python 3 Library for Building the Genetic Algorithm and Training Machine Learning Algoithms (Keras & PyTorch).
 Home-page: https://github.com/ahmedfgad/GeneticAlgorithmPython
 Author: Ahmed Fawzy Gad
 Author-email: ahmed.f.gad@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pygad-3.0.0/pygad.egg-info/SOURCES.txt` & `pygad-3.0.1/pygad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygad-3.0.0/setup.py` & `pygad-3.0.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools  
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(  
     name="pygad",  
-    version="3.0.0",  
+    version="3.0.1",  
     author="Ahmed Fawzy Gad",
     install_requires=["numpy", "matplotlib","cloudpickle",],
     author_email="ahmed.f.gad@gmail.com",  
     description="PyGAD: A Python 3 Library for Building the Genetic Algorithm and Training Machine Learning Algoithms (Keras & PyTorch).",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ahmedfgad/GeneticAlgorithmPython",
```

