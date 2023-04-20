# Comparing `tmp/scipion-em-imod-3.1.7.tar.gz` & `tmp/scipion-em-imod-3.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-imod-3.1.7.tar", last modified: Thu Mar 30 07:44:39 2023, max compression
+gzip compressed data, was "scipion-em-imod-3.1.8.tar", last modified: Thu Apr 20 07:45:09 2023, max compression
```

## Comparing `scipion-em-imod-3.1.7.tar` & `scipion-em-imod-3.1.8.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 07:44:39.531800 scipion-em-imod-3.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-03-30 07:44:39.531800 scipion-em-imod-3.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 07:44:39.519800 scipion-em-imod-3.1.7/imod/
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/file_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/icon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 07:44:39.527800 scipion-em-imod-3.1.7/imod/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/protocols/protocol_applyTransformationMatrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/protocols/protocol_auto3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    24073 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/protocols/protocol_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13261 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/protocols/protocol_ctfCorrection.py
--rw-r--r--   0 runner    (1001) docker     (123)    24526 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/protocols/protocol_ctfEstimation_automatic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/protocols/protocol_ctfEstimation_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/protocols/protocol_doseFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)    28762 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/protocols/protocol_etomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/protocols/protocol_excludeViews.py
--rw-r--r--   0 runner    (1001) docker     (123)    40520 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/protocols/protocol_fiducialAlignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    26801 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/protocols/protocol_fiducialModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/protocols/protocol_goldBeadEraser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/protocols/protocol_goldBeadPicker3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/protocols/protocol_importSetOfCTFTomoSeries.py
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/protocols/protocol_importSetOfTM.py
--rw-r--r--   0 runner    (1001) docker     (123)    14231 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/protocols/protocol_tomoNormalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/protocols/protocol_tomoProjection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12635 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/protocols/protocol_tomoReconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)    15474 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/protocols/protocol_tsNormalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    14500 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/protocols/protocol_xCorrPrealignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/protocols/protocol_xRaysEraser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/protocols/script_imod_auto3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 07:44:39.527800 scipion-em-imod-3.1.7/imod/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/templates/automatic_tilt_series_alignment.json.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 07:44:39.531800 scipion-em-imod-3.1.7/imod/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38359 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/tests/test_protocols_imod.py
--rw-r--r--   0 runner    (1001) docker     (123)    38742 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 07:44:39.531800 scipion-em-imod-3.1.7/imod/viewers/
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/viewers/viewers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14220 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/imod/viewers/views_tkinter_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 07:44:39.531800 scipion-em-imod-3.1.7/scipion_em_imod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-03-30 07:44:39.000000 scipion-em-imod-3.1.7/scipion_em_imod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-03-30 07:44:39.000000 scipion-em-imod-3.1.7/scipion_em_imod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 07:44:39.000000 scipion-em-imod-3.1.7/scipion_em_imod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-30 07:44:39.000000 scipion-em-imod-3.1.7/scipion_em_imod.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-30 07:44:39.000000 scipion-em-imod-3.1.7/scipion_em_imod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 07:44:39.531800 scipion-em-imod-3.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-03-30 07:42:49.000000 scipion-em-imod-3.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:45:09.096839 scipion-em-imod-3.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-04-20 07:45:09.096839 scipion-em-imod-3.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:45:09.092838 scipion-em-imod-3.1.8/imod/
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/file_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:45:09.092838 scipion-em-imod-3.1.8/imod/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_applyTransformationMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_auto3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24073 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_ctfCorrection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24526 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_ctfEstimation_automatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_ctfEstimation_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_doseFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28762 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_etomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_excludeViews.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40520 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_fiducialAlignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26801 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_fiducialModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_goldBeadEraser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_goldBeadPicker3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_importSetOfCTFTomoSeries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_importSetOfTM.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14231 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_tomoNormalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_tomoProjection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12944 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_tomoReconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15474 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_tsNormalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14500 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_xCorrPrealignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_xRaysEraser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/script_imod_auto3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:45:09.092838 scipion-em-imod-3.1.8/imod/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/templates/automatic_tilt_series_alignment.json.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:45:09.092838 scipion-em-imod-3.1.8/imod/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38359 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/tests/test_protocols_imod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38742 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:45:09.092838 scipion-em-imod-3.1.8/imod/viewers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/viewers/viewers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14220 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/viewers/views_tkinter_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:45:09.096839 scipion-em-imod-3.1.8/scipion_em_imod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-04-20 07:45:09.000000 scipion-em-imod-3.1.8/scipion_em_imod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-20 07:45:09.000000 scipion-em-imod-3.1.8/scipion_em_imod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 07:45:09.000000 scipion-em-imod-3.1.8/scipion_em_imod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-20 07:45:09.000000 scipion-em-imod-3.1.8/scipion_em_imod.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-20 07:45:09.000000 scipion-em-imod-3.1.8/scipion_em_imod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 07:45:09.096839 scipion-em-imod-3.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/setup.py
```

### Comparing `scipion-em-imod-3.1.7/LICENSE` & `scipion-em-imod-3.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/PKG-INFO` & `scipion-em-imod-3.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scipion-em-imod
-Version: 3.1.7
+Version: 3.1.8
 Summary: Plugin to use some of the Tomography tools from IMOD in Scipion
 Home-page: https://github.com/scipion-em/scipion-em-imod
 Author: J.M. De la Rosa, Federico P. de Isidro Gomez
 Author-email: delarosatrevin@scilifelab.se, fp.deisidro@cnb.csic.es
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-imod/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-imod/
```

### Comparing `scipion-em-imod-3.1.7/README.rst` & `scipion-em-imod-3.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/__init__.py` & `scipion-em-imod-3.1.8/imod/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from pyworkflow.gui import FileTreeProvider
 from pyworkflow.gui.project.utils import OS
 import pwem
 
 from .constants import IMOD_HOME, ETOMO_CMD, DEFAULT_VERSION, VERSIONS
 
 
-__version__ = '3.1.7'
+__version__ = '3.1.8'
 _logo = "icon.png"
 _references = ['Kremer1996', 'Mastronarde2017']
 
 
 def getImodEnv():
     """ This function allows to call imod outside this plugin. """
```

### Comparing `scipion-em-imod-3.1.7/imod/bibtex.py` & `scipion-em-imod-3.1.8/imod/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/constants.py` & `scipion-em-imod-3.1.8/imod/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/icon.png` & `scipion-em-imod-3.1.8/imod/icon.png`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/protocols/__init__.py` & `scipion-em-imod-3.1.8/imod/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/protocols/protocol_applyTransformationMatrix.py` & `scipion-em-imod-3.1.8/imod/protocols/protocol_applyTransformationMatrix.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/protocols/protocol_auto3d.py` & `scipion-em-imod-3.1.8/imod/protocols/protocol_auto3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/protocols/protocol_base.py` & `scipion-em-imod-3.1.8/imod/protocols/protocol_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/protocols/protocol_ctfCorrection.py` & `scipion-em-imod-3.1.8/imod/protocols/protocol_ctfCorrection.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,24 +258,14 @@
                             "information! The recommended workflow is to "
                             "estimate CTF on raw tilt-series and then here "
                             "provide tilt-series with alignment "
                             "(non-interpolated).")
 
         return warnings
 
-    def _validate(self):
-        validateMsgs = []
-
-        if self.inputSetOfTiltSeries.get().getSize() != self.inputSetOfCtfTomoSeries.get().getSize():
-            validateMsgs.append("Input tilt-series and CTF tomo "
-                                "estimations must contain the "
-                                "same number of elements.")
-
-        return validateMsgs
-
     def _summary(self):
         summary = []
         if self.TiltSeries:
             summary.append("Input tilt-series: %d\nCTF corrections applied: %d"
                            % (self.inputSetOfCtfTomoSeries.get().getSize(),
                               self.TiltSeries.getSize()))
         else:
```

### Comparing `scipion-em-imod-3.1.7/imod/protocols/protocol_ctfEstimation_automatic.py` & `scipion-em-imod-3.1.8/imod/protocols/protocol_ctfEstimation_automatic.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/protocols/protocol_ctfEstimation_manual.py` & `scipion-em-imod-3.1.8/imod/protocols/protocol_ctfEstimation_manual.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/protocols/protocol_doseFilter.py` & `scipion-em-imod-3.1.8/imod/protocols/protocol_doseFilter.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/protocols/protocol_etomo.py` & `scipion-em-imod-3.1.8/imod/protocols/protocol_etomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/protocols/protocol_excludeViews.py` & `scipion-em-imod-3.1.8/imod/protocols/protocol_excludeViews.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/protocols/protocol_fiducialAlignment.py` & `scipion-em-imod-3.1.8/imod/protocols/protocol_fiducialAlignment.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/protocols/protocol_fiducialModel.py` & `scipion-em-imod-3.1.8/imod/protocols/protocol_fiducialModel.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/protocols/protocol_goldBeadEraser.py` & `scipion-em-imod-3.1.8/imod/protocols/protocol_goldBeadEraser.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/protocols/protocol_goldBeadPicker3d.py` & `scipion-em-imod-3.1.8/imod/protocols/protocol_goldBeadPicker3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/protocols/protocol_importSetOfCTFTomoSeries.py` & `scipion-em-imod-3.1.8/imod/protocols/protocol_importSetOfCTFTomoSeries.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/protocols/protocol_importSetOfTM.py` & `scipion-em-imod-3.1.8/imod/protocols/protocol_importSetOfTM.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/protocols/protocol_tomoNormalization.py` & `scipion-em-imod-3.1.8/imod/protocols/protocol_tomoNormalization.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/protocols/protocol_tomoProjection.py` & `scipion-em-imod-3.1.8/imod/protocols/protocol_tomoProjection.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/protocols/protocol_tomoReconstruction.py` & `scipion-em-imod-3.1.8/imod/protocols/protocol_tomoReconstruction.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,65 +57,63 @@
                       label='Input set of tilt-series')
 
         form.addParam('tomoThickness',
                       params.FloatParam,
                       default=1000,
                       label='Tomogram thickness (voxels)',
                       important=True,
-                      display=params.EnumParam.DISPLAY_HLIST,
                       help='Size in voxels of the tomogram in the z '
                            'axis (beam direction).')
 
         form.addParam('tomoShiftX',
                       params.FloatParam,
                       default=0,
                       label='Tomogram shift in X',
-                      display=params.EnumParam.DISPLAY_HLIST,
                       help='This entry allows one to shift the reconstructed '
                            'slice in X before it is output.  If the X shift '
                            'is positive, the slice will be shifted to the '
                            'right, and the output will contain the left part '
                            'of the whole potentially reconstructable area.')
-
+        form.addParam('tomoWidth',
+                      params.IntParam,
+                      default=0,
+                      label='Tomogram width (voxels)',
+                      help='Number of pixels to cut out in X, centered on the middle in X. Leave 0 for default X.')
         form.addParam('tomoShiftZ',
                       params.FloatParam,
                       default=0,
                       label='Tomogram shift in Z',
-                      display=params.EnumParam.DISPLAY_HLIST,
                       help='This entry allows one to shift the reconstructed '
                            'slice in Z before it is output. If the Z '
                            'shift is positive, the slice is shifted upward. '
                            'The Z entry is optional and defaults to 0 '
                            'when omitted.')
 
         form.addParam('angleOffset',
                       params.FloatParam,
                       default=0,
                       label='Angle offset',
-                      display=params.EnumParam.DISPLAY_HLIST,
                       help='Apply an angle offset in degrees to all tilt '
                            'angles. This offset positively rotates the '
                            'reconstructed sections anticlockwise.')
 
         form.addParam('tiltAxisOffset',
                       params.FloatParam,
                       default=0,
                       label='Tilt axis offset',
-                      display=params.EnumParam.DISPLAY_HLIST,
                       help='Apply an offset to the tilt axis in a stack of '
                            'full-sized projection images, cutting the '
                            'X-axis at  NX/2. + offset instead of NX/2. The '
                            'DELXX entry is optional and defaults to 0 '
                            'when omitted.')
 
         form.addParam('fakeInteractionsSIRT',
                       params.IntParam,
                       default=0,
                       label='Iterations of a SIRT-like equivalent filter',
-                      display=params.EnumParam.DISPLAY_HLIST,
                       expertLevel=params.LEVEL_ADVANCED,
                       help='Modify the radial filter to produce a '
                            'reconstruction equivalent to the one produced by '
                            'the given number of iterations of SIRT. The '
                            'Gaussian filter is applied at the high-frequency '
                            'end of the filter. The functioning of this filter '
                            'is described in: \n\t'
@@ -219,18 +217,26 @@
 
         if self.usesGpu():
             argsTilt += f"-UseGPU {self.getGpuList()[0]} " \
                         "-ActionIfGPUFails 2,2 "
 
         Plugin.runImod(self, 'tilt', argsTilt % paramsTilt)
 
+        def getArgs():
+            args = "-rx "
+
+            if self.tomoWidth.get():
+                args += " -nx %s" % self.tomoWidth.get()
+
+            return args
+
         paramsTrimVol = {
             'input': os.path.join(tmpPrefix, firstItem.parseFileName(extension=".rec")),
             'output': os.path.join(extraPrefix, firstItem.parseFileName(extension=".mrc")),
-            'options': "-rx "
+            'options': getArgs()
         }
 
         argsTrimvol = "%(options)s " \
                       "%(input)s " \
                       "%(output)s "
 
         Plugin.runImod(self, 'trimvol', argsTrimvol % paramsTrimVol)
@@ -247,14 +253,19 @@
         newTomogram = Tomogram()
         newTomogram.setLocation(os.path.join(extraPrefix,
                                              firstItem.parseFileName(extension=".mrc")))
         newTomogram.setTsId(tsId)
         newTomogram.setSamplingRate(ts.getSamplingRate())
         # Set default tomogram origin
         newTomogram.setOrigin(newOrigin=None)
+        if self.tomoShiftZ.get():
+            x,y,z = newTomogram.getShiftsFromOrigin()
+            shiftZang= self.tomoShiftZ.get() * newTomogram.getSamplingRate()
+            newTomogram.setShiftsInOrigin(x=x,y=y,z=z+shiftZang)
+
         newTomogram.setAcquisition(ts.getAcquisition())
 
         output.append(newTomogram)
         output.update(newTomogram)
         output.write()
         self._store()
```

### Comparing `scipion-em-imod-3.1.7/imod/protocols/protocol_tsNormalization.py` & `scipion-em-imod-3.1.8/imod/protocols/protocol_tsNormalization.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/protocols/protocol_xCorrPrealignment.py` & `scipion-em-imod-3.1.8/imod/protocols/protocol_xCorrPrealignment.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/protocols/protocol_xRaysEraser.py` & `scipion-em-imod-3.1.8/imod/protocols/protocol_xRaysEraser.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/protocols/script_imod_auto3d.py` & `scipion-em-imod-3.1.8/imod/protocols/script_imod_auto3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/protocols.conf` & `scipion-em-imod-3.1.8/imod/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/templates/automatic_tilt_series_alignment.json.template` & `scipion-em-imod-3.1.8/imod/templates/automatic_tilt_series_alignment.json.template`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/tests/__init__.py` & `scipion-em-imod-3.1.8/imod/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/tests/test_protocols_imod.py` & `scipion-em-imod-3.1.8/imod/tests/test_protocols_imod.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/utils.py` & `scipion-em-imod-3.1.8/imod/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/viewers/__init__.py` & `scipion-em-imod-3.1.8/imod/viewers/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/viewers/viewers.py` & `scipion-em-imod-3.1.8/imod/viewers/viewers.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/imod/viewers/views_tkinter_tree.py` & `scipion-em-imod-3.1.8/imod/viewers/views_tkinter_tree.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/scipion_em_imod.egg-info/PKG-INFO` & `scipion-em-imod-3.1.8/scipion_em_imod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scipion-em-imod
-Version: 3.1.7
+Version: 3.1.8
 Summary: Plugin to use some of the Tomography tools from IMOD in Scipion
 Home-page: https://github.com/scipion-em/scipion-em-imod
 Author: J.M. De la Rosa, Federico P. de Isidro Gomez
 Author-email: delarosatrevin@scilifelab.se, fp.deisidro@cnb.csic.es
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-imod/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-imod/
```

### Comparing `scipion-em-imod-3.1.7/scipion_em_imod.egg-info/SOURCES.txt` & `scipion-em-imod-3.1.8/scipion_em_imod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.7/setup.py` & `scipion-em-imod-3.1.8/setup.py`

 * *Files identical despite different names*

