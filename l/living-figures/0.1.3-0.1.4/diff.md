# Comparing `tmp/living-figures-0.1.3.tar.gz` & `tmp/living-figures-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "living-figures-0.1.3.tar", last modified: Wed Apr 19 18:33:30 2023, max compression
+gzip compressed data, was "living-figures-0.1.4.tar", last modified: Wed Apr 19 22:49:37 2023, max compression
```

## Comparing `living-figures-0.1.3.tar` & `living-figures-0.1.4.tar`

### file list

```diff
@@ -1,44 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:33:30.743426 living-figures-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-19 18:32:43.000000 living-figures-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-19 18:32:43.000000 living-figures-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-19 18:33:30.743426 living-figures-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-19 18:32:43.000000 living-figures-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-19 18:32:43.000000 living-figures-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-19 18:32:43.000000 living-figures-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 18:33:30.743426 living-figures-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-19 18:32:43.000000 living-figures-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:33:30.739426 living-figures-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:33:30.743426 living-figures-0.1.3/src/living_figures/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:33:30.743426 living-figures-0.1.3/src/living_figures/bio/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/bio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:33:30.743426 living-figures-0.1.3/src/living_figures/bio/epigenome/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/bio/epigenome/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:33:30.743426 living-figures-0.1.3/src/living_figures/bio/epigenome/test_data/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2606 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/bio/epigenome/test_data/download_from_ncbi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:33:30.743426 living-figures-0.1.3/src/living_figures/bio/epigenome/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/bio/epigenome/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/bio/epigenome/utilities/pacbio_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/bio/epigenome/utilities/parse_rebase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/bio/epigenome/utilities/rebase_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:33:30.743426 living-figures-0.1.3/src/living_figures/bio/epigenome/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/bio/epigenome/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27803 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/bio/epigenome/widgets/panepibrowser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:33:30.743426 living-figures-0.1.3/src/living_figures/bio/fom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/bio/fom/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:33:30.743426 living-figures-0.1.3/src/living_figures/bio/volcano/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/bio/volcano/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/bio/volcano/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/bio/volcano/make_test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:33:30.743426 living-figures-0.1.3/src/living_figures/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/helpers/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-19 18:32:43.000000 living-figures-0.1.3/src/living_figures/helpers/sorting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:33:30.743426 living-figures-0.1.3/src/living_figures.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-19 18:33:30.000000 living-figures-0.1.3/src/living_figures.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-19 18:33:30.000000 living-figures-0.1.3/src/living_figures.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:33:30.000000 living-figures-0.1.3/src/living_figures.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-19 18:33:30.000000 living-figures-0.1.3/src/living_figures.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-19 18:33:30.000000 living-figures-0.1.3/src/living_figures.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:33:30.743426 living-figures-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-19 18:32:43.000000 living-figures-0.1.3/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.969930 living-figures-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-19 22:48:45.000000 living-figures-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-19 22:48:45.000000 living-figures-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-19 22:49:37.969930 living-figures-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-19 22:48:45.000000 living-figures-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-19 22:48:45.000000 living-figures-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-19 22:48:45.000000 living-figures-0.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 22:49:37.969930 living-figures-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-19 22:48:45.000000 living-figures-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.965930 living-figures-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.965930 living-figures-0.1.4/src/living_figures/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.965930 living-figures-0.1.4/src/living_figures/bio/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.965930 living-figures-0.1.4/src/living_figures/bio/epigenome/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/epigenome/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.965930 living-figures-0.1.4/src/living_figures/bio/epigenome/test_data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2606 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/epigenome/test_data/download_from_ncbi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.965930 living-figures-0.1.4/src/living_figures/bio/epigenome/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/epigenome/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/epigenome/utilities/pacbio_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/epigenome/utilities/parse_rebase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/epigenome/utilities/rebase_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.965930 living-figures-0.1.4/src/living_figures/bio/epigenome/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/epigenome/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27803 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/epigenome/widgets/panepibrowser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.965930 living-figures-0.1.4/src/living_figures/bio/fom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/fom/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.969930 living-figures-0.1.4/src/living_figures/bio/fom/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/fom/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/fom/utilities/parse_tax_string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.965930 living-figures-0.1.4/src/living_figures/bio/fom/widgets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.969930 living-figures-0.1.4/src/living_figures/bio/fom/widgets/microbiome/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/fom/widgets/microbiome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10528 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/fom/widgets/microbiome/abundant_orgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/fom/widgets/microbiome/base_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/fom/widgets/microbiome/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/fom/widgets/microbiome/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/fom/widgets/microbiome/ordination.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.969930 living-figures-0.1.4/src/living_figures/bio/volcano/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/volcano/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/volcano/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/volcano/make_test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.969930 living-figures-0.1.4/src/living_figures/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/helpers/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/helpers/parse_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/helpers/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/helpers/sorting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.965930 living-figures-0.1.4/src/living_figures.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-19 22:49:37.000000 living-figures-0.1.4/src/living_figures.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-19 22:49:37.000000 living-figures-0.1.4/src/living_figures.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 22:49:37.000000 living-figures-0.1.4/src/living_figures.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-19 22:49:37.000000 living-figures-0.1.4/src/living_figures.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-19 22:49:37.000000 living-figures-0.1.4/src/living_figures.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.969930 living-figures-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-19 22:48:45.000000 living-figures-0.1.4/tests/test_import.py
```

### Comparing `living-figures-0.1.3/LICENSE` & `living-figures-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.3/PKG-INFO` & `living-figures-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: living-figures
-Version: 0.1.3
+Version: 0.1.4
 Summary: Resource of interactive data widgets
 Author-email: Samuel Minot <sminot@fredhutch.org>
 Project-URL: Homepage, https://github.com/FredHutch/widgets-store
 Project-URL: Bug Tracker, https://github.com/FredHutch/widgets-store/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `living-figures-0.1.3/README.md` & `living-figures-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.3/pyproject.toml` & `living-figures-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.3/src/living_figures/bio/epigenome/test_data/download_from_ncbi.py` & `living-figures-0.1.4/src/living_figures/bio/epigenome/test_data/download_from_ncbi.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.3/src/living_figures/bio/epigenome/utilities/pacbio_file.py` & `living-figures-0.1.4/src/living_figures/bio/epigenome/utilities/pacbio_file.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.3/src/living_figures/bio/epigenome/utilities/parse_rebase.py` & `living-figures-0.1.4/src/living_figures/bio/epigenome/utilities/parse_rebase.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.3/src/living_figures/bio/epigenome/utilities/rebase_file.py` & `living-figures-0.1.4/src/living_figures/bio/epigenome/utilities/rebase_file.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.3/src/living_figures/bio/epigenome/widgets/panepibrowser.py` & `living-figures-0.1.4/src/living_figures/bio/epigenome/widgets/panepibrowser.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.3/src/living_figures/bio/volcano/app.py` & `living-figures-0.1.4/src/living_figures/bio/volcano/app.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.3/src/living_figures/bio/volcano/make_test_data.py` & `living-figures-0.1.4/src/living_figures/bio/volcano/make_test_data.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.3/src/living_figures/helpers/sorting.py` & `living-figures-0.1.4/src/living_figures/helpers/sorting.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.3/src/living_figures.egg-info/PKG-INFO` & `living-figures-0.1.4/src/living_figures.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: living-figures
-Version: 0.1.3
+Version: 0.1.4
 Summary: Resource of interactive data widgets
 Author-email: Samuel Minot <sminot@fredhutch.org>
 Project-URL: Homepage, https://github.com/FredHutch/widgets-store
 Project-URL: Bug Tracker, https://github.com/FredHutch/widgets-store/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `living-figures-0.1.3/src/living_figures.egg-info/SOURCES.txt` & `living-figures-0.1.4/src/living_figures.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -16,14 +16,24 @@
 src/living_figures/bio/epigenome/utilities/__init__.py
 src/living_figures/bio/epigenome/utilities/pacbio_file.py
 src/living_figures/bio/epigenome/utilities/parse_rebase.py
 src/living_figures/bio/epigenome/utilities/rebase_file.py
 src/living_figures/bio/epigenome/widgets/__init__.py
 src/living_figures/bio/epigenome/widgets/panepibrowser.py
 src/living_figures/bio/fom/__init__.py
+src/living_figures/bio/fom/utilities/__init__.py
+src/living_figures/bio/fom/utilities/parse_tax_string.py
+src/living_figures/bio/fom/widgets/microbiome/__init__.py
+src/living_figures/bio/fom/widgets/microbiome/abundant_orgs.py
+src/living_figures/bio/fom/widgets/microbiome/base_plots.py
+src/living_figures/bio/fom/widgets/microbiome/inputs.py
+src/living_figures/bio/fom/widgets/microbiome/main.py
+src/living_figures/bio/fom/widgets/microbiome/ordination.py
 src/living_figures/bio/volcano/__init__.py
 src/living_figures/bio/volcano/app.py
 src/living_figures/bio/volcano/make_test_data.py
 src/living_figures/helpers/__init__.py
+src/living_figures/helpers/constants.py
+src/living_figures/helpers/parse_numeric.py
 src/living_figures/helpers/scaling.py
 src/living_figures/helpers/sorting.py
 tests/test_import.py
```

### Comparing `living-figures-0.1.3/tests/test_import.py` & `living-figures-0.1.4/tests/test_import.py`

 * *Files identical despite different names*

