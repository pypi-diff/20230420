# Comparing `tmp/APtools-0.2.1.tar.gz` & `tmp/APtools-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/APtools/APtools/dist/.tmp-e7wzglaf/APtools-0.2.1.tar", last modified: Fri Mar 10 12:13:25 2023, max compression
+gzip compressed data, was "/home/runner/work/APtools/APtools/dist/.tmp-fhf9qv_0/APtools-0.2.3.tar", last modified: Wed Apr 19 23:20:55 2023, max compression
```

## Comparing `APtools-0.2.1.tar` & `APtools-0.2.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 12:13:25.000000 APtools-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 12:13:25.000000 APtools-0.2.1/APtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1346 2023-03-10 12:13:25.000000 APtools-0.2.1/APtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1127 2023-03-10 12:13:25.000000 APtools-0.2.1/APtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-10 12:13:25.000000 APtools-0.2.1/APtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       48 2023-03-10 12:13:25.000000 APtools-0.2.1/APtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        8 2023-03-10 12:13:25.000000 APtools-0.2.1/APtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)    35147 2023-03-10 12:13:16.000000 APtools-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     1346 2023-03-10 12:13:25.000000 APtools-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      710 2023-03-10 12:13:16.000000 APtools-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 12:13:25.000000 APtools-0.2.1/aptools/
--rw-r--r--   0 runner    (1001) docker     (116)      113 2023-03-10 12:13:16.000000 APtools-0.2.1/aptools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 12:13:25.000000 APtools-0.2.1/aptools/data_analysis/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-10 12:13:16.000000 APtools-0.2.1/aptools/data_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    45145 2023-03-10 12:13:16.000000 APtools-0.2.1/aptools/data_analysis/beam_diagnostics.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 12:13:25.000000 APtools-0.2.1/aptools/data_handling/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-10 12:13:16.000000 APtools-0.2.1/aptools/data_handling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2573 2023-03-10 12:13:16.000000 APtools-0.2.1/aptools/data_handling/conversion.py
--rw-r--r--   0 runner    (1001) docker     (116)    10070 2023-03-10 12:13:16.000000 APtools-0.2.1/aptools/data_handling/reading.py
--rw-r--r--   0 runner    (1001) docker     (116)    17701 2023-03-10 12:13:16.000000 APtools-0.2.1/aptools/data_handling/saving.py
--rw-r--r--   0 runner    (1001) docker     (116)      539 2023-03-10 12:13:16.000000 APtools-0.2.1/aptools/data_handling/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 12:13:25.000000 APtools-0.2.1/aptools/data_processing/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-10 12:13:16.000000 APtools-0.2.1/aptools/data_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2704 2023-03-10 12:13:16.000000 APtools-0.2.1/aptools/data_processing/beam_filtering.py
--rw-r--r--   0 runner    (1001) docker     (116)     5111 2023-03-10 12:13:16.000000 APtools-0.2.1/aptools/data_processing/beam_operations.py
--rw-r--r--   0 runner    (1001) docker     (116)     8331 2023-03-10 12:13:16.000000 APtools-0.2.1/aptools/helper_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 12:13:25.000000 APtools-0.2.1/aptools/particle_distributions/
--rw-r--r--   0 runner    (1001) docker     (116)      207 2023-03-10 12:13:16.000000 APtools-0.2.1/aptools/particle_distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1571 2023-03-10 12:13:16.000000 APtools-0.2.1/aptools/particle_distributions/particle_distribution.py
--rw-r--r--   0 runner    (1001) docker     (116)     6172 2023-03-10 12:13:16.000000 APtools-0.2.1/aptools/particle_distributions/read.py
--rw-r--r--   0 runner    (1001) docker     (116)    10034 2023-03-10 12:13:16.000000 APtools-0.2.1/aptools/particle_distributions/save.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 12:13:25.000000 APtools-0.2.1/aptools/plasma_accel/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-10 12:13:16.000000 APtools-0.2.1/aptools/plasma_accel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    13410 2023-03-10 12:13:16.000000 APtools-0.2.1/aptools/plasma_accel/general_equations.py
--rw-r--r--   0 runner    (1001) docker     (116)       63 2023-03-10 12:13:16.000000 APtools-0.2.1/aptools/plasma_accel/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 12:13:25.000000 APtools-0.2.1/aptools/plotting/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-10 12:13:16.000000 APtools-0.2.1/aptools/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1538 2023-03-10 12:13:16.000000 APtools-0.2.1/aptools/plotting/plot_types.py
--rw-r--r--   0 runner    (1001) docker     (116)    28156 2023-03-10 12:13:16.000000 APtools-0.2.1/aptools/plotting/quick_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (116)      448 2023-03-10 12:13:16.000000 APtools-0.2.1/aptools/plotting/rc_params.py
--rw-r--r--   0 runner    (1001) docker     (116)     2529 2023-03-10 12:13:16.000000 APtools-0.2.1/aptools/plotting/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 12:13:25.000000 APtools-0.2.1/aptools/utilities/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-10 12:13:16.000000 APtools-0.2.1/aptools/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    13015 2023-03-10 12:13:16.000000 APtools-0.2.1/aptools/utilities/bunch_generation.py
--rw-r--r--   0 runner    (1001) docker     (116)       90 2023-03-10 12:13:16.000000 APtools-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)      779 2023-03-10 12:13:25.000000 APtools-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)       69 2023-03-10 12:13:16.000000 APtools-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:20:55.000000 APtools-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:20:55.000000 APtools-0.2.3/APtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-19 23:20:55.000000 APtools-0.2.3/APtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-19 23:20:55.000000 APtools-0.2.3/APtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:20:55.000000 APtools-0.2.3/APtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-19 23:20:55.000000 APtools-0.2.3/APtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 23:20:55.000000 APtools-0.2.3/APtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-19 23:20:42.000000 APtools-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-19 23:20:55.000000 APtools-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-19 23:20:42.000000 APtools-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:20:55.000000 APtools-0.2.3/aptools/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-19 23:20:42.000000 APtools-0.2.3/aptools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:20:55.000000 APtools-0.2.3/aptools/data_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:20:42.000000 APtools-0.2.3/aptools/data_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45145 2023-04-19 23:20:42.000000 APtools-0.2.3/aptools/data_analysis/beam_diagnostics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:20:55.000000 APtools-0.2.3/aptools/data_handling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:20:42.000000 APtools-0.2.3/aptools/data_handling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-19 23:20:42.000000 APtools-0.2.3/aptools/data_handling/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-04-19 23:20:42.000000 APtools-0.2.3/aptools/data_handling/reading.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-04-19 23:20:42.000000 APtools-0.2.3/aptools/data_handling/saving.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-19 23:20:42.000000 APtools-0.2.3/aptools/data_handling/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:20:55.000000 APtools-0.2.3/aptools/data_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:20:42.000000 APtools-0.2.3/aptools/data_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-19 23:20:42.000000 APtools-0.2.3/aptools/data_processing/beam_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-04-19 23:20:42.000000 APtools-0.2.3/aptools/data_processing/beam_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-04-19 23:20:42.000000 APtools-0.2.3/aptools/helper_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:20:55.000000 APtools-0.2.3/aptools/particle_distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-19 23:20:42.000000 APtools-0.2.3/aptools/particle_distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-19 23:20:42.000000 APtools-0.2.3/aptools/particle_distributions/particle_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-04-19 23:20:42.000000 APtools-0.2.3/aptools/particle_distributions/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-04-19 23:20:42.000000 APtools-0.2.3/aptools/particle_distributions/save.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:20:55.000000 APtools-0.2.3/aptools/plasma_accel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:20:42.000000 APtools-0.2.3/aptools/plasma_accel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13410 2023-04-19 23:20:42.000000 APtools-0.2.3/aptools/plasma_accel/general_equations.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-19 23:20:42.000000 APtools-0.2.3/aptools/plasma_accel/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:20:55.000000 APtools-0.2.3/aptools/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:20:42.000000 APtools-0.2.3/aptools/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-19 23:20:42.000000 APtools-0.2.3/aptools/plotting/plot_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28156 2023-04-19 23:20:42.000000 APtools-0.2.3/aptools/plotting/quick_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-19 23:20:42.000000 APtools-0.2.3/aptools/plotting/rc_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-19 23:20:42.000000 APtools-0.2.3/aptools/plotting/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:20:55.000000 APtools-0.2.3/aptools/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:20:42.000000 APtools-0.2.3/aptools/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13015 2023-04-19 23:20:42.000000 APtools-0.2.3/aptools/utilities/bunch_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-19 23:20:42.000000 APtools-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-19 23:20:55.000000 APtools-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-19 23:20:42.000000 APtools-0.2.3/setup.py
```

### Comparing `APtools-0.2.1/APtools.egg-info/PKG-INFO` & `APtools-0.2.3/APtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: APtools
-Version: 0.2.1
+Version: 0.2.3
 Summary: A collection of tools for accelerator physics
 Home-page: https://github.com/AngelFP/APtools
 Author: Angel Ferran Pousa
 Author-email: angel.ferran.pousa@desy.de,
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `APtools-0.2.1/APtools.egg-info/SOURCES.txt` & `APtools-0.2.3/APtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `APtools-0.2.1/LICENSE` & `APtools-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `APtools-0.2.1/PKG-INFO` & `APtools-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: APtools
-Version: 0.2.1
+Version: 0.2.3
 Summary: A collection of tools for accelerator physics
 Home-page: https://github.com/AngelFP/APtools
 Author: Angel Ferran Pousa
 Author-email: angel.ferran.pousa@desy.de,
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `APtools-0.2.1/README.md` & `APtools-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `APtools-0.2.1/aptools/data_analysis/beam_diagnostics.py` & `APtools-0.2.3/aptools/data_analysis/beam_diagnostics.py`

 * *Files identical despite different names*

### Comparing `APtools-0.2.1/aptools/data_handling/conversion.py` & `APtools-0.2.3/aptools/data_handling/conversion.py`

 * *Files identical despite different names*

### Comparing `APtools-0.2.1/aptools/data_handling/reading.py` & `APtools-0.2.3/aptools/data_handling/reading.py`

 * *Files identical despite different names*

### Comparing `APtools-0.2.1/aptools/data_handling/saving.py` & `APtools-0.2.3/aptools/data_handling/saving.py`

 * *Files identical despite different names*

### Comparing `APtools-0.2.1/aptools/data_handling/utilities.py` & `APtools-0.2.3/aptools/data_handling/utilities.py`

 * *Files identical despite different names*

### Comparing `APtools-0.2.1/aptools/data_processing/beam_filtering.py` & `APtools-0.2.3/aptools/data_processing/beam_filtering.py`

 * *Files identical despite different names*

### Comparing `APtools-0.2.1/aptools/data_processing/beam_operations.py` & `APtools-0.2.3/aptools/data_processing/beam_operations.py`

 * *Files identical despite different names*

### Comparing `APtools-0.2.1/aptools/helper_functions.py` & `APtools-0.2.3/aptools/helper_functions.py`

 * *Files identical despite different names*

### Comparing `APtools-0.2.1/aptools/particle_distributions/particle_distribution.py` & `APtools-0.2.3/aptools/particle_distributions/particle_distribution.py`

 * *Files identical despite different names*

### Comparing `APtools-0.2.1/aptools/particle_distributions/read.py` & `APtools-0.2.3/aptools/particle_distributions/read.py`

 * *Files identical despite different names*

### Comparing `APtools-0.2.1/aptools/particle_distributions/save.py` & `APtools-0.2.3/aptools/particle_distributions/save.py`

 * *Files identical despite different names*

### Comparing `APtools-0.2.1/aptools/plasma_accel/general_equations.py` & `APtools-0.2.3/aptools/plasma_accel/general_equations.py`

 * *Files identical despite different names*

### Comparing `APtools-0.2.1/aptools/plotting/plot_types.py` & `APtools-0.2.3/aptools/plotting/plot_types.py`

 * *Files identical despite different names*

### Comparing `APtools-0.2.1/aptools/plotting/quick_diagnostics.py` & `APtools-0.2.3/aptools/plotting/quick_diagnostics.py`

 * *Files identical despite different names*

### Comparing `APtools-0.2.1/aptools/plotting/utils.py` & `APtools-0.2.3/aptools/plotting/utils.py`

 * *Files identical despite different names*

### Comparing `APtools-0.2.1/aptools/utilities/bunch_generation.py` & `APtools-0.2.3/aptools/utilities/bunch_generation.py`

 * *Files identical despite different names*

### Comparing `APtools-0.2.1/setup.cfg` & `APtools-0.2.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,14 @@
 
 [options]
 packages = find:
 install_requires = 
 	numpy
 	scipy
 	h5py
-	openpmd-api~=0.14.0
+	openpmd-api~=0.14.0,~=0.15.0
 	deprecated
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

