# Comparing `tmp/KiMoPack-7.0.1.tar.gz` & `tmp/KiMoPack-7.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KiMoPack-7.0.1.tar", last modified: Thu Apr 20 11:01:27 2023, max compression
+gzip compressed data, was "KiMoPack-7.0.2.tar", last modified: Thu Apr 20 16:07:42 2023, max compression
```

## Comparing `KiMoPack-7.0.1.tar` & `KiMoPack-7.0.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 11:01:27.326099 KiMoPack-7.0.1/
--rw-rw-rw-   0        0        0    35823 2021-09-12 20:51:08.000000 KiMoPack-7.0.1/LICENSE
--rw-rw-rw-   0        0        0       51 2022-06-13 14:27:08.000000 KiMoPack-7.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5530 2023-04-20 11:01:27.326099 KiMoPack-7.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4669 2022-12-08 21:00:40.000000 KiMoPack-7.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-20 11:01:27.182421 KiMoPack-7.0.1/Workflow_tools/
-drwxrwxrwx   0        0        0        0 2023-04-20 11:01:27.234228 KiMoPack-7.0.1/Workflow_tools/.ipynb_checkpoints/
--rw-rw-rw-   0        0        0     7627 2023-03-28 09:55:29.000000 KiMoPack-7.0.1/Workflow_tools/.ipynb_checkpoints/TA_Advanced_Fit-checkpoint.ipynb
--rw-rw-rw-   0        0        0     3472 2022-12-08 22:16:07.000000 KiMoPack-7.0.1/Workflow_tools/.ipynb_checkpoints/TA_Kumar-checkpoint.ipynb
--rw-rw-rw-   0        0        0     4808 2023-03-28 09:56:04.000000 KiMoPack-7.0.1/Workflow_tools/.ipynb_checkpoints/TA_Raw_plotting-checkpoint.ipynb
--rw-rw-rw-   0        0        0    11395 2023-04-18 15:07:49.000000 KiMoPack-7.0.1/Workflow_tools/.ipynb_checkpoints/TA_Raw_plotting_and_Simple_Fit-checkpoint.ipynb
--rw-rw-rw-   0        0        0     5442 2023-03-28 09:55:18.000000 KiMoPack-7.0.1/Workflow_tools/.ipynb_checkpoints/TA_comparative_plotting_and_data_extraction-checkpoint.ipynb
--rw-rw-rw-   0        0        0     3897 2023-03-28 09:55:43.000000 KiMoPack-7.0.1/Workflow_tools/.ipynb_checkpoints/TA_single_scan_handling-checkpoint.ipynb
--rw-rw-rw-   0        0        0    14416 2022-11-08 18:55:10.000000 KiMoPack-7.0.1/Workflow_tools/.ipynb_checkpoints/TA_testing-checkpoint.ipynb
-drwxrwxrwx   0        0        0        0 2023-04-20 11:01:27.252232 KiMoPack-7.0.1/Workflow_tools/Data/
--rw-rw-rw-   0        0        0  1263591 2020-05-19 08:45:04.000000 KiMoPack-7.0.1/Workflow_tools/Data/Sample_1.SIA
--rw-rw-rw-   0        0        0  1268547 2020-05-15 07:11:18.000000 KiMoPack-7.0.1/Workflow_tools/Data/Sample_2.SIA
--rw-rw-rw-   0        0        0     8532 2022-07-20 12:02:05.000000 KiMoPack-7.0.1/Workflow_tools/Ivan_horse.ipynb
--rw-rw-rw-   0        0        0    11744 2022-07-08 21:17:55.000000 KiMoPack-7.0.1/Workflow_tools/Streak_camera_analysis.ipynb
--rw-rw-rw-   0        0        0    17958 2022-07-20 10:17:48.000000 KiMoPack-7.0.1/Workflow_tools/TA testing.ipynb
--rw-rw-rw-   0        0        0     8046 2023-04-18 15:49:27.000000 KiMoPack-7.0.1/Workflow_tools/TA_Advanced_Fit.ipynb
--rw-rw-rw-   0        0        0     7794 2022-07-19 10:01:23.000000 KiMoPack-7.0.1/Workflow_tools/TA_Pump_dump.ipynb
--rw-rw-rw-   0        0        0     4808 2023-03-28 09:56:04.000000 KiMoPack-7.0.1/Workflow_tools/TA_Raw_plotting.ipynb
--rw-rw-rw-   0        0        0    11395 2023-04-18 16:23:38.000000 KiMoPack-7.0.1/Workflow_tools/TA_Raw_plotting_and_Simple_Fit.ipynb
--rw-rw-rw-   0        0        0     5442 2023-03-28 09:55:18.000000 KiMoPack-7.0.1/Workflow_tools/TA_comparative_plotting_and_data_extraction.ipynb
--rw-rw-rw-   0        0        0     3897 2023-03-28 09:55:43.000000 KiMoPack-7.0.1/Workflow_tools/TA_single_scan_handling.ipynb
--rw-rw-rw-   0        0        0    14823 2022-12-08 21:48:59.000000 KiMoPack-7.0.1/Workflow_tools/TA_testing.ipynb
-drwxrwxrwx   0        0        0        0 2023-04-20 11:01:27.021874 KiMoPack-7.0.1/Workflow_tools/additional_formats/
-drwxrwxrwx   0        0        0        0 2023-04-20 11:01:27.276234 KiMoPack-7.0.1/Workflow_tools/additional_formats/streak_camera/
-drwxrwxrwx   0        0        0        0 2023-04-20 11:01:27.288231 KiMoPack-7.0.1/Workflow_tools/additional_formats/streak_camera/.ipynb_checkpoints/
--rw-rw-rw-   0        0        0    16723 2022-07-08 19:10:02.000000 KiMoPack-7.0.1/Workflow_tools/additional_formats/streak_camera/.ipynb_checkpoints/Importing and analysis of emission data-checkpoint.ipynb
--rw-rw-rw-   0        0        0    24324 2022-07-08 21:14:23.000000 KiMoPack-7.0.1/Workflow_tools/additional_formats/streak_camera/Analysis of emission data.ipynb
--rw-rw-rw-   0        0        0     1055 2022-07-08 19:34:34.000000 KiMoPack-7.0.1/Workflow_tools/additional_formats/streak_camera/import_library.py
-drwxrwxrwx   0        0        0        0 2023-04-20 11:01:27.308430 KiMoPack-7.0.1/Workflow_tools/additional_functions/
--rw-rw-rw-   0        0        0     1399 2022-11-27 20:54:31.000000 KiMoPack-7.0.1/Workflow_tools/additional_functions/cut.py
--rw-rw-rw-   0        0        0    33184 2022-06-13 13:57:20.000000 KiMoPack-7.0.1/Workflow_tools/additional_functions/standard_functions.py
--rw-rw-rw-   0        0        0    42156 2022-12-08 21:58:00.000000 KiMoPack-7.0.1/Workflow_tools/function_library.py
--rw-rw-rw-   0        0        0     2052 2022-07-20 11:34:37.000000 KiMoPack-7.0.1/Workflow_tools/import_library.py
--rw-rw-rw-   0        0        0      108 2021-09-12 20:51:08.000000 KiMoPack-7.0.1/pyproject.toml
--rw-rw-rw-   0        0        0     1080 2023-04-20 11:01:27.342167 KiMoPack-7.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1103 2022-06-13 14:38:11.000000 KiMoPack-7.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 11:01:27.024732 KiMoPack-7.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-20 11:01:27.318099 KiMoPack-7.0.1/src/KiMoPack/
--rw-rw-rw-   0        0        0     4424 2022-10-03 11:31:41.000000 KiMoPack-7.0.1/src/KiMoPack/__init__.py
--rw-rw-rw-   0        0        0   423466 2023-04-20 10:59:57.000000 KiMoPack-7.0.1/src/KiMoPack/plot_func.py
-drwxrwxrwx   0        0        0        0 2023-04-20 11:01:27.324098 KiMoPack-7.0.1/src/KiMoPack.egg-info/
--rw-rw-rw-   0        0        0     5530 2023-04-20 11:01:26.000000 KiMoPack-7.0.1/src/KiMoPack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1717 2023-04-20 11:01:27.000000 KiMoPack-7.0.1/src/KiMoPack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 11:01:26.000000 KiMoPack-7.0.1/src/KiMoPack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-04-20 11:01:26.000000 KiMoPack-7.0.1/src/KiMoPack.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-20 11:01:26.000000 KiMoPack-7.0.1/src/KiMoPack.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 16:07:42.912613 KiMoPack-7.0.2/
+-rw-rw-rw-   0        0        0    35823 2021-09-12 20:51:08.000000 KiMoPack-7.0.2/LICENSE
+-rw-rw-rw-   0        0        0       51 2022-06-13 14:27:08.000000 KiMoPack-7.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5530 2023-04-20 16:07:42.916912 KiMoPack-7.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4669 2022-12-08 21:00:40.000000 KiMoPack-7.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-20 16:07:42.472214 KiMoPack-7.0.2/Workflow_tools/
+drwxrwxrwx   0        0        0        0 2023-04-20 16:07:42.547405 KiMoPack-7.0.2/Workflow_tools/.ipynb_checkpoints/
+-rw-rw-rw-   0        0        0     7627 2023-03-28 09:55:29.000000 KiMoPack-7.0.2/Workflow_tools/.ipynb_checkpoints/TA_Advanced_Fit-checkpoint.ipynb
+-rw-rw-rw-   0        0        0     3472 2022-12-08 22:16:07.000000 KiMoPack-7.0.2/Workflow_tools/.ipynb_checkpoints/TA_Kumar-checkpoint.ipynb
+-rw-rw-rw-   0        0        0     4808 2023-03-28 09:56:04.000000 KiMoPack-7.0.2/Workflow_tools/.ipynb_checkpoints/TA_Raw_plotting-checkpoint.ipynb
+-rw-rw-rw-   0        0        0    11395 2023-04-18 15:07:49.000000 KiMoPack-7.0.2/Workflow_tools/.ipynb_checkpoints/TA_Raw_plotting_and_Simple_Fit-checkpoint.ipynb
+-rw-rw-rw-   0        0        0     5442 2023-03-28 09:55:18.000000 KiMoPack-7.0.2/Workflow_tools/.ipynb_checkpoints/TA_comparative_plotting_and_data_extraction-checkpoint.ipynb
+-rw-rw-rw-   0        0        0     3897 2023-03-28 09:55:43.000000 KiMoPack-7.0.2/Workflow_tools/.ipynb_checkpoints/TA_single_scan_handling-checkpoint.ipynb
+-rw-rw-rw-   0        0        0    14416 2022-11-08 18:55:10.000000 KiMoPack-7.0.2/Workflow_tools/.ipynb_checkpoints/TA_testing-checkpoint.ipynb
+drwxrwxrwx   0        0        0        0 2023-04-20 16:07:42.593475 KiMoPack-7.0.2/Workflow_tools/Data/
+-rw-rw-rw-   0        0        0  1263591 2020-05-19 08:45:04.000000 KiMoPack-7.0.2/Workflow_tools/Data/Sample_1.SIA
+-rw-rw-rw-   0        0        0  1268547 2020-05-15 07:11:18.000000 KiMoPack-7.0.2/Workflow_tools/Data/Sample_2.SIA
+-rw-rw-rw-   0        0        0     8532 2022-07-20 12:02:05.000000 KiMoPack-7.0.2/Workflow_tools/Ivan_horse.ipynb
+-rw-rw-rw-   0        0        0    11744 2022-07-08 21:17:55.000000 KiMoPack-7.0.2/Workflow_tools/Streak_camera_analysis.ipynb
+-rw-rw-rw-   0        0        0    17958 2022-07-20 10:17:48.000000 KiMoPack-7.0.2/Workflow_tools/TA testing.ipynb
+-rw-rw-rw-   0        0        0     8046 2023-04-18 15:49:27.000000 KiMoPack-7.0.2/Workflow_tools/TA_Advanced_Fit.ipynb
+-rw-rw-rw-   0        0        0     7794 2022-07-19 10:01:23.000000 KiMoPack-7.0.2/Workflow_tools/TA_Pump_dump.ipynb
+-rw-rw-rw-   0        0        0     4808 2023-03-28 09:56:04.000000 KiMoPack-7.0.2/Workflow_tools/TA_Raw_plotting.ipynb
+-rw-rw-rw-   0        0        0    11395 2023-04-18 16:23:38.000000 KiMoPack-7.0.2/Workflow_tools/TA_Raw_plotting_and_Simple_Fit.ipynb
+-rw-rw-rw-   0        0        0     5442 2023-03-28 09:55:18.000000 KiMoPack-7.0.2/Workflow_tools/TA_comparative_plotting_and_data_extraction.ipynb
+-rw-rw-rw-   0        0        0     3897 2023-03-28 09:55:43.000000 KiMoPack-7.0.2/Workflow_tools/TA_single_scan_handling.ipynb
+-rw-rw-rw-   0        0        0    14823 2022-12-08 21:48:59.000000 KiMoPack-7.0.2/Workflow_tools/TA_testing.ipynb
+drwxrwxrwx   0        0        0        0 2023-04-20 16:07:42.113619 KiMoPack-7.0.2/Workflow_tools/additional_formats/
+drwxrwxrwx   0        0        0        0 2023-04-20 16:07:42.683067 KiMoPack-7.0.2/Workflow_tools/additional_formats/streak_camera/
+drwxrwxrwx   0        0        0        0 2023-04-20 16:07:42.719360 KiMoPack-7.0.2/Workflow_tools/additional_formats/streak_camera/.ipynb_checkpoints/
+-rw-rw-rw-   0        0        0    16723 2022-07-08 19:10:02.000000 KiMoPack-7.0.2/Workflow_tools/additional_formats/streak_camera/.ipynb_checkpoints/Importing and analysis of emission data-checkpoint.ipynb
+-rw-rw-rw-   0        0        0    24324 2022-07-08 21:14:23.000000 KiMoPack-7.0.2/Workflow_tools/additional_formats/streak_camera/Analysis of emission data.ipynb
+-rw-rw-rw-   0        0        0     1055 2022-07-08 19:34:34.000000 KiMoPack-7.0.2/Workflow_tools/additional_formats/streak_camera/import_library.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:07:42.789497 KiMoPack-7.0.2/Workflow_tools/additional_functions/
+-rw-rw-rw-   0        0        0     1399 2022-11-27 20:54:31.000000 KiMoPack-7.0.2/Workflow_tools/additional_functions/cut.py
+-rw-rw-rw-   0        0        0    33184 2022-06-13 13:57:20.000000 KiMoPack-7.0.2/Workflow_tools/additional_functions/standard_functions.py
+-rw-rw-rw-   0        0        0    42156 2022-12-08 21:58:00.000000 KiMoPack-7.0.2/Workflow_tools/function_library.py
+-rw-rw-rw-   0        0        0     2052 2022-07-20 11:34:37.000000 KiMoPack-7.0.2/Workflow_tools/import_library.py
+-rw-rw-rw-   0        0        0      108 2021-09-12 20:51:08.000000 KiMoPack-7.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1080 2023-04-20 16:07:42.928500 KiMoPack-7.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1103 2022-06-13 14:38:11.000000 KiMoPack-7.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:07:42.118361 KiMoPack-7.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-20 16:07:42.878090 KiMoPack-7.0.2/src/KiMoPack/
+-rw-rw-rw-   0        0        0     4424 2022-10-03 11:31:41.000000 KiMoPack-7.0.2/src/KiMoPack/__init__.py
+-rw-rw-rw-   0        0        0   423525 2023-04-20 16:05:44.000000 KiMoPack-7.0.2/src/KiMoPack/plot_func.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:07:42.911082 KiMoPack-7.0.2/src/KiMoPack.egg-info/
+-rw-rw-rw-   0        0        0     5530 2023-04-20 16:07:42.000000 KiMoPack-7.0.2/src/KiMoPack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1717 2023-04-20 16:07:42.000000 KiMoPack-7.0.2/src/KiMoPack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 16:07:42.000000 KiMoPack-7.0.2/src/KiMoPack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-04-20 16:07:42.000000 KiMoPack-7.0.2/src/KiMoPack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-20 16:07:42.000000 KiMoPack-7.0.2/src/KiMoPack.egg-info/top_level.txt
```

### Comparing `KiMoPack-7.0.1/LICENSE` & `KiMoPack-7.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `KiMoPack-7.0.1/PKG-INFO` & `KiMoPack-7.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KiMoPack
-Version: 7.0.1
+Version: 7.0.2
 Summary: A comprehensive package for the analysis of kinetic data.
 Home-page: https://github.com/erdzeichen/KiMoPack
 Author: Jens Uhlig
 Author-email: jens.uhlig@chemphys.lu.se
 Project-URL: Bug Tracker, https://github.com/erdzeichen/KiMoPack/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `KiMoPack-7.0.1/README.rst` & `KiMoPack-7.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `KiMoPack-7.0.1/Workflow_tools/.ipynb_checkpoints/TA_Advanced_Fit-checkpoint.ipynb` & `KiMoPack-7.0.2/Workflow_tools/.ipynb_checkpoints/TA_Advanced_Fit-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `KiMoPack-7.0.1/Workflow_tools/.ipynb_checkpoints/TA_Kumar-checkpoint.ipynb` & `KiMoPack-7.0.2/Workflow_tools/.ipynb_checkpoints/TA_Kumar-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `KiMoPack-7.0.1/Workflow_tools/.ipynb_checkpoints/TA_Raw_plotting-checkpoint.ipynb` & `KiMoPack-7.0.2/Workflow_tools/.ipynb_checkpoints/TA_Raw_plotting-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `KiMoPack-7.0.1/Workflow_tools/.ipynb_checkpoints/TA_Raw_plotting_and_Simple_Fit-checkpoint.ipynb` & `KiMoPack-7.0.2/Workflow_tools/.ipynb_checkpoints/TA_Raw_plotting_and_Simple_Fit-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `KiMoPack-7.0.1/Workflow_tools/.ipynb_checkpoints/TA_comparative_plotting_and_data_extraction-checkpoint.ipynb` & `KiMoPack-7.0.2/Workflow_tools/.ipynb_checkpoints/TA_comparative_plotting_and_data_extraction-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `KiMoPack-7.0.1/Workflow_tools/.ipynb_checkpoints/TA_single_scan_handling-checkpoint.ipynb` & `KiMoPack-7.0.2/Workflow_tools/.ipynb_checkpoints/TA_single_scan_handling-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `KiMoPack-7.0.1/Workflow_tools/.ipynb_checkpoints/TA_testing-checkpoint.ipynb` & `KiMoPack-7.0.2/Workflow_tools/.ipynb_checkpoints/TA_testing-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `KiMoPack-7.0.1/Workflow_tools/Data/Sample_1.SIA` & `KiMoPack-7.0.2/Workflow_tools/Data/Sample_1.SIA`

 * *Files identical despite different names*

### Comparing `KiMoPack-7.0.1/Workflow_tools/Data/Sample_2.SIA` & `KiMoPack-7.0.2/Workflow_tools/Data/Sample_2.SIA`

 * *Files identical despite different names*

### Comparing `KiMoPack-7.0.1/Workflow_tools/Ivan_horse.ipynb` & `KiMoPack-7.0.2/Workflow_tools/Ivan_horse.ipynb`

 * *Files identical despite different names*

### Comparing `KiMoPack-7.0.1/Workflow_tools/Streak_camera_analysis.ipynb` & `KiMoPack-7.0.2/Workflow_tools/Streak_camera_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `KiMoPack-7.0.1/Workflow_tools/TA testing.ipynb` & `KiMoPack-7.0.2/Workflow_tools/TA testing.ipynb`

 * *Files identical despite different names*

### Comparing `KiMoPack-7.0.1/Workflow_tools/TA_Advanced_Fit.ipynb` & `KiMoPack-7.0.2/Workflow_tools/TA_Advanced_Fit.ipynb`

 * *Files identical despite different names*

### Comparing `KiMoPack-7.0.1/Workflow_tools/TA_Pump_dump.ipynb` & `KiMoPack-7.0.2/Workflow_tools/TA_Pump_dump.ipynb`

 * *Files identical despite different names*

### Comparing `KiMoPack-7.0.1/Workflow_tools/TA_Raw_plotting.ipynb` & `KiMoPack-7.0.2/Workflow_tools/TA_Raw_plotting.ipynb`

 * *Files identical despite different names*

### Comparing `KiMoPack-7.0.1/Workflow_tools/TA_Raw_plotting_and_Simple_Fit.ipynb` & `KiMoPack-7.0.2/Workflow_tools/TA_Raw_plotting_and_Simple_Fit.ipynb`

 * *Files identical despite different names*

### Comparing `KiMoPack-7.0.1/Workflow_tools/TA_comparative_plotting_and_data_extraction.ipynb` & `KiMoPack-7.0.2/Workflow_tools/TA_comparative_plotting_and_data_extraction.ipynb`

 * *Files identical despite different names*

### Comparing `KiMoPack-7.0.1/Workflow_tools/TA_single_scan_handling.ipynb` & `KiMoPack-7.0.2/Workflow_tools/TA_single_scan_handling.ipynb`

 * *Files identical despite different names*

### Comparing `KiMoPack-7.0.1/Workflow_tools/TA_testing.ipynb` & `KiMoPack-7.0.2/Workflow_tools/TA_testing.ipynb`

 * *Files identical despite different names*

### Comparing `KiMoPack-7.0.1/Workflow_tools/additional_formats/streak_camera/.ipynb_checkpoints/Importing and analysis of emission data-checkpoint.ipynb` & `KiMoPack-7.0.2/Workflow_tools/additional_formats/streak_camera/.ipynb_checkpoints/Importing and analysis of emission data-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `KiMoPack-7.0.1/Workflow_tools/additional_formats/streak_camera/Analysis of emission data.ipynb` & `KiMoPack-7.0.2/Workflow_tools/additional_formats/streak_camera/Analysis of emission data.ipynb`

 * *Files identical despite different names*

### Comparing `KiMoPack-7.0.1/Workflow_tools/additional_formats/streak_camera/import_library.py` & `KiMoPack-7.0.2/Workflow_tools/additional_formats/streak_camera/import_library.py`

 * *Files identical despite different names*

### Comparing `KiMoPack-7.0.1/Workflow_tools/additional_functions/cut.py` & `KiMoPack-7.0.2/Workflow_tools/additional_functions/cut.py`

 * *Files identical despite different names*

### Comparing `KiMoPack-7.0.1/Workflow_tools/additional_functions/standard_functions.py` & `KiMoPack-7.0.2/Workflow_tools/additional_functions/standard_functions.py`

 * *Files identical despite different names*

### Comparing `KiMoPack-7.0.1/Workflow_tools/function_library.py` & `KiMoPack-7.0.2/Workflow_tools/function_library.py`

 * *Files identical despite different names*

### Comparing `KiMoPack-7.0.1/Workflow_tools/import_library.py` & `KiMoPack-7.0.2/Workflow_tools/import_library.py`

 * *Files identical despite different names*

### Comparing `KiMoPack-7.0.1/setup.cfg` & `KiMoPack-7.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 204b 694d 6f50 6163 6b0d 0a76 6572   = KiMoPack..ver
-00000020: 7369 6f6e 203d 2037 2e30 2e31 0d0a 6175  sion = 7.0.1..au
+00000020: 7369 6f6e 203d 2037 2e30 2e32 0d0a 6175  sion = 7.0.2..au
 00000030: 7468 6f72 203d 204a 656e 7320 5568 6c69  thor = Jens Uhli
 00000040: 670d 0a61 7574 686f 725f 656d 6169 6c20  g..author_email 
 00000050: 3d20 6a65 6e73 2e75 686c 6967 4063 6865  = jens.uhlig@che
 00000060: 6d70 6879 732e 6c75 2e73 650d 0a64 6573  mphys.lu.se..des
 00000070: 6372 6970 7469 6f6e 203d 2041 2063 6f6d  cription = A com
 00000080: 7072 6568 656e 7369 7665 2070 6163 6b61  prehensive packa
 00000090: 6765 2066 6f72 2074 6865 2061 6e61 6c79  ge for the analy
```

### Comparing `KiMoPack-7.0.1/setup.py` & `KiMoPack-7.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `KiMoPack-7.0.1/src/KiMoPack/__init__.py` & `KiMoPack-7.0.2/src/KiMoPack/__init__.py`

 * *Files identical despite different names*

### Comparing `KiMoPack-7.0.1/src/KiMoPack/plot_func.py` & `KiMoPack-7.0.2/src/KiMoPack/plot_func.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
 00000010: 662d 3820 2d2a 2d0d 0a76 6572 7369 6f6e  f-8 -*-..version
-00000020: 203d 2022 372e 302e 3122 0d0a 436f 7079   = "7.0.1"..Copy
+00000020: 203d 2022 372e 302e 3222 0d0a 436f 7079   = "7.0.2"..Copy
 00000030: 7269 6768 7420 3d20 2740 4a65 6e73 2055  right = '@Jens U
 00000040: 686c 6967 270d 0a69 6620 313a 2023 4869  hlig'..if 1: #Hi
 00000050: 6465 2069 6d70 6f72 7473 090d 0a09 696d  de imports....im
 00000060: 706f 7274 206f 730d 0a09 6672 6f6d 206f  port os...from o
 00000070: 7320 696d 706f 7274 2077 616c 6b0d 0a09  s import walk...
 00000080: 696d 706f 7274 2073 7973 0d0a 0969 6d70  import sys...imp
 00000090: 6f72 7420 7061 6e64 6173 0d0a 0969 6d70  ort pandas...imp
@@ -21127,5341 +21127,5345 @@
 00052860: 4153 3a0d 0a09 0909 666f 7220 692c 7265  AS:.....for i,re
 00052870: 5f6c 6f63 616c 2069 6e20 656e 756d 6572  _local in enumer
 00052880: 6174 6528 7265 5f6c 6973 7465 6e29 3a0d  ate(re_listen):.
 00052890: 0a09 0909 0966 6f72 206e 616d 6520 696e  .....for name in
 000528a0: 205b 2766 6974 5f6f 7574 7075 7427 2c27   ['fit_output','
 000528b0: 6669 745f 7265 7375 6c74 735f 7261 7465  fit_results_rate
 000528c0: 7327 2c27 6669 745f 7265 7375 6c74 735f  s','fit_results_
-000528d0: 7469 6d65 7327 5d3a 0d0a 0909 0909 0972  times']:.......r
-000528e0: 655f 6c69 7374 656e 5b69 5d5b 6e61 6d65  e_listen[i][name
-000528f0: 5d3d 7265 5b6e 616d 655d 0d0a 0909 0d0a  ]=re[name]......
-00052900: 0909 2323 2323 2323 2323 2323 2323 2323  ..##############
-00052910: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00052920: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00052930: 230d 0a09 0923 2363 6f6e 7665 7274 2065  #....##convert e
-00052940: 6e65 7267 7920 6261 636b 2074 6f20 7761  nergy back to wa
-00052950: 7665 6c65 6e67 7468 2323 2323 2323 2323  velength########
-00052960: 2323 2323 230d 0a09 0923 2323 2323 2323  #####....#######
-00052970: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00052980: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00052990: 2323 2323 2323 2323 230d 0a09 0969 6620  #########....if 
-000529a0: 313a 0d0a 0909 0969 6620 7365 6c66 2e65  1:.....if self.e
-000529b0: 7175 616c 5f65 6e65 7267 795f 6269 6e20  qual_energy_bin 
-000529c0: 6973 206e 6f74 204e 6f6e 653a 0d0a 0909  is not None:....
-000529d0: 0909 6966 2073 616d 655f 4441 533a 0d0a  ..if same_DAS:..
-000529e0: 0909 0909 0966 6f72 2069 2c72 655f 6c6f  .....for i,re_lo
-000529f0: 6361 6c20 696e 2065 6e75 6d65 7261 7465  cal in enumerate
-00052a00: 2872 655f 6c69 7374 656e 293a 0d0a 0909  (re_listen):....
-00052a10: 0909 0909 666f 7220 6e61 6d65 2069 6e20  ....for name in 
-00052a20: 5b27 4127 2c27 4143 272c 2741 4527 5d3a  ['A','AC','AE']:
-00052a30: 0d0a 0909 0909 0909 0972 655f 6c6f 6361  .........re_loca
-00052a40: 6c5b 6e61 6d65 5d2e 636f 6c75 6d6e 733d  l[name].columns=
-00052a50: 2873 6369 7079 2e63 6f6e 7374 616e 7473  (scipy.constants
-00052a60: 2e68 2a73 6369 7079 2e63 6f6e 7374 616e  .h*scipy.constan
-00052a70: 7473 2e63 2f28 7265 5f6c 6f63 616c 5b6e  ts.c/(re_local[n
-00052a80: 616d 655d 2e63 6f6c 756d 6e73 2e76 616c  ame].columns.val
-00052a90: 7565 732a 3165 2d39 2a73 6369 7079 2e63  ues*1e-9*scipy.c
-00052aa0: 6f6e 7374 616e 7473 2e65 6c65 6374 726f  onstants.electro
-00052ab0: 6e5f 766f 6c74 2929 0d0a 0909 0909 0909  n_volt))........
-00052ac0: 0972 655f 6c6f 6361 6c5b 6e61 6d65 5d2e  .re_local[name].
-00052ad0: 636f 6c75 6d6e 732e 6e61 6d65 3d27 7761  columns.name='wa
-00052ae0: 7665 6c65 6e67 7468 2069 6e20 6e6d 270d  velength in nm'.
-00052af0: 0a09 0909 0909 0909 7265 5f6c 6f63 616c  ........re_local
-00052b00: 5b6e 616d 655d 2e73 6f72 745f 696e 6465  [name].sort_inde
-00052b10: 7828 696e 706c 6163 653d 5472 7565 2c61  x(inplace=True,a
-00052b20: 7869 733d 312c 6173 6365 6e64 696e 673d  xis=1,ascending=
-00052b30: 5472 7565 290d 0a09 0909 0909 0972 655f  True)........re_
-00052b40: 6c6f 6361 6c5b 2744 4143 275d 2e69 6e64  local['DAC'].ind
-00052b50: 6578 3d28 7363 6970 792e 636f 6e73 7461  ex=(scipy.consta
-00052b60: 6e74 732e 682a 7363 6970 792e 636f 6e73  nts.h*scipy.cons
-00052b70: 7461 6e74 732e 632f 2872 655f 6c6f 6361  tants.c/(re_loca
-00052b80: 6c5b 2744 4143 275d 2e69 6e64 6578 2e76  l['DAC'].index.v
-00052b90: 616c 7565 732a 3165 2d39 2a73 6369 7079  alues*1e-9*scipy
-00052ba0: 2e63 6f6e 7374 616e 7473 2e65 6c65 6374  .constants.elect
-00052bb0: 726f 6e5f 766f 6c74 2929 0d0a 0909 0909  ron_volt))......
-00052bc0: 0909 7265 5f6c 6f63 616c 5b27 4441 4327  ..re_local['DAC'
-00052bd0: 5d2e 696e 6465 782e 6e61 6d65 3d27 7761  ].index.name='wa
-00052be0: 7665 6c65 6e67 7468 2069 6e20 6e6d 270d  velength in nm'.
-00052bf0: 0a09 0909 0909 0972 655f 6c6f 6361 6c5b  .......re_local[
-00052c00: 2744 4143 275d 2e73 6f72 745f 696e 6465  'DAC'].sort_inde
-00052c10: 7828 696e 706c 6163 653d 5472 7565 2c61  x(inplace=True,a
-00052c20: 7869 733d 302c 6173 6365 6e64 696e 673d  xis=0,ascending=
-00052c30: 5472 7565 290d 0a09 0909 0909 0972 655f  True)........re_
-00052c40: 6c69 7374 656e 5b69 5d3d 7265 5f6c 6f63  listen[i]=re_loc
-00052c50: 616c 0d0a 0909 0909 656c 7365 3a0d 0a09  al......else:...
-00052c60: 0909 0909 666f 7220 6e61 6d65 2069 6e20  ....for name in 
-00052c70: 5b27 4127 2c27 4143 272c 2741 4527 5d3a  ['A','AC','AE']:
-00052c80: 0d0a 0909 0909 0909 7265 5b6e 616d 655d  ........re[name]
-00052c90: 2e63 6f6c 756d 6e73 3d28 7363 6970 792e  .columns=(scipy.
-00052ca0: 636f 6e73 7461 6e74 732e 682a 7363 6970  constants.h*scip
-00052cb0: 792e 636f 6e73 7461 6e74 732e 632f 2872  y.constants.c/(r
-00052cc0: 655b 6e61 6d65 5d2e 636f 6c75 6d6e 732e  e[name].columns.
-00052cd0: 7661 6c75 6573 2a31 652d 392a 7363 6970  values*1e-9*scip
-00052ce0: 792e 636f 6e73 7461 6e74 732e 656c 6563  y.constants.elec
-00052cf0: 7472 6f6e 5f76 6f6c 7429 290d 0a09 0909  tron_volt)).....
-00052d00: 0909 0972 655b 6e61 6d65 5d2e 636f 6c75  ...re[name].colu
-00052d10: 6d6e 732e 6e61 6d65 3d27 7761 7665 6c65  mns.name='wavele
-00052d20: 6e67 7468 2069 6e20 6e6d 270d 0a09 0909  ngth in nm'.....
-00052d30: 0909 0972 655b 6e61 6d65 5d2e 736f 7274  ...re[name].sort
-00052d40: 5f69 6e64 6578 2869 6e70 6c61 6365 3d54  _index(inplace=T
-00052d50: 7275 652c 6178 6973 3d31 2c61 7363 656e  rue,axis=1,ascen
-00052d60: 6469 6e67 3d54 7275 6529 0d0a 0909 0909  ding=True)......
-00052d70: 0972 655b 2744 4143 275d 2e69 6e64 6578  .re['DAC'].index
-00052d80: 3d28 7363 6970 792e 636f 6e73 7461 6e74  =(scipy.constant
-00052d90: 732e 682a 7363 6970 792e 636f 6e73 7461  s.h*scipy.consta
-00052da0: 6e74 732e 632f 2872 655b 2744 4143 275d  nts.c/(re['DAC']
-00052db0: 2e69 6e64 6578 2e76 616c 7565 732a 3165  .index.values*1e
-00052dc0: 2d39 2a73 6369 7079 2e63 6f6e 7374 616e  -9*scipy.constan
-00052dd0: 7473 2e65 6c65 6374 726f 6e5f 766f 6c74  ts.electron_volt
-00052de0: 2929 0d0a 0909 0909 0972 655b 2744 4143  )).......re['DAC
-00052df0: 275d 2e69 6e64 6578 2e6e 616d 653d 2777  '].index.name='w
-00052e00: 6176 656c 656e 6774 6820 696e 206e 6d27  avelength in nm'
-00052e10: 0d0a 0909 0909 0972 655b 2744 4143 275d  .......re['DAC']
-00052e20: 2e73 6f72 745f 696e 6465 7828 696e 706c  .sort_index(inpl
-00052e30: 6163 653d 5472 7565 2c61 7869 733d 302c  ace=True,axis=0,
-00052e40: 6173 6365 6e64 696e 673d 5472 7565 290d  ascending=True).
-00052e50: 0a09 090d 0a09 090d 0a09 0923 2323 2323  ...........#####
-00052e60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00052e70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00052e80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00052e90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00052ea0: 2323 2323 2323 230d 0a09 0923 2d2d 2d70  #######....#---p
-00052eb0: 7269 6e74 2074 6865 206f 7574 7075 742d  rint the output-
-00052ec0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00052ed0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00052ee0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00052ef0: 2d2d 0d0a 0909 2323 2323 2323 2323 2323  --....##########
-00052f00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00052f10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00052f20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00052f30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00052f40: 2323 0d0a 0909 7365 6c66 2e72 653d 7265  ##....self.re=re
-00052f50: 0d0a 0909 6966 2073 616d 655f 4441 533a  ....if same_DAS:
-00052f60: 0d0a 0909 0972 655f 6c69 7374 656e 5b30  .....re_listen[0
-00052f70: 5d3d 7265 0d0a 0909 0973 656c 662e 6d75  ]=re.....self.mu
-00052f80: 6c74 695f 7072 6f6a 6563 7473 3d72 655f  lti_projects=re_
-00052f90: 6c69 7374 656e 0d0a 0d0a 0909 5265 7375  listen......Resu
-00052fa0: 6c74 5f73 7472 696e 673d 275c 6e46 6974  lt_string='\nFit
-00052fb0: 2052 6573 756c 7473 3a5c 6e27 0d0a 0909   Results:\n'....
-00052fc0: 0d0a 0909 6966 2069 7369 6e73 7461 6e63  ....if isinstanc
-00052fd0: 6528 6d6f 642c 7479 7065 2827 6865 6c6c  e(mod,type('hell
-00052fe0: 6f27 2929 3a0d 0a09 0909 5265 7375 6c74  o')):.....Result
-00052ff0: 5f73 7472 696e 672b 3d27 4d6f 6465 6c20  _string+='Model 
-00053000: 5573 6564 3a20 2573 5c6e 5c6e 2725 6d6f  Used: %s\n\n'%mo
-00053010: 640d 0a09 0965 6c73 653a 0d0a 0909 0952  d....else:.....R
-00053020: 6573 756c 745f 7374 7269 6e67 2b3d 274d  esult_string+='M
-00053030: 6f64 656c 2055 7365 643a 2045 7874 6572  odel Used: Exter
-00053040: 6e61 6c20 6675 6e63 7469 6f6e 5c6e 5c6e  nal function\n\n
-00053050: 270d 0a09 090d 0a09 090d 0a09 0969 6620  '............if 
-00053060: 7365 6c66 2e69 676e 6f72 655f 7469 6d65  self.ignore_time
-00053070: 5f72 6567 696f 6e20 6973 206e 6f74 204e  _region is not N
-00053080: 6f6e 653a 0d0a 0909 0974 7279 3a0d 0a09  one:.....try:...
-00053090: 0909 0952 6573 756c 745f 7374 7269 6e67  ...Result_string
-000530a0: 2b3d 2774 6865 2074 696d 6520 6265 7477  +='the time betw
-000530b0: 6565 6e20 252e 3366 2025 7320 616e 6420  een %.3f %s and 
-000530c0: 252e 3366 2025 7320 7761 7320 6578 636c  %.3f %s was excl
-000530d0: 7564 6564 2066 726f 6d20 7468 6520 6f70  uded from the op
-000530e0: 7469 6d69 7a61 7469 6f6e 5c6e 5c6e 2725  timization\n\n'%
-000530f0: 2873 656c 662e 6967 6e6f 7265 5f74 696d  (self.ignore_tim
-00053100: 655f 7265 6769 6f6e 5b30 5d2c 7365 6c66  e_region[0],self
-00053110: 2e62 6173 6575 6e69 742c 7365 6c66 2e69  .baseunit,self.i
-00053120: 676e 6f72 655f 7469 6d65 5f72 6567 696f  gnore_time_regio
-00053130: 6e5b 315d 2c73 656c 662e 6261 7365 756e  n[1],self.baseun
-00053140: 6974 290d 0a09 0909 6578 6365 7074 3a23  it).....except:#
-00053150: 7765 2067 6f74 2061 206c 6973 740d 0a09  we got a list...
-00053160: 0909 0966 6f72 2065 6e74 7279 2069 6e20  ...for entry in 
-00053170: 7365 6c66 2e69 676e 6f72 655f 7469 6d65  self.ignore_time
-00053180: 5f72 6567 696f 6e3a 0d0a 0909 0909 0952  _region:.......R
-00053190: 6573 756c 745f 7374 7269 6e67 2b3d 2774  esult_string+='t
-000531a0: 6865 2074 696d 6520 6265 7477 6565 6e20  he time between 
-000531b0: 252e 3366 2025 7320 616e 6420 252e 3366  %.3f %s and %.3f
-000531c0: 2025 7320 7761 7320 6578 636c 7564 6564   %s was excluded
-000531d0: 2066 726f 6d20 7468 6520 6f70 7469 6d69   from the optimi
-000531e0: 7a61 7469 6f6e 5c6e 5c6e 2725 2865 6e74  zation\n\n'%(ent
-000531f0: 7279 5b30 5d2c 7365 6c66 2e62 6173 6575  ry[0],self.baseu
-00053200: 6e69 742c 656e 7472 795b 315d 2c73 656c  nit,entry[1],sel
-00053210: 662e 6261 7365 756e 6974 290d 0a09 0952  f.baseunit)....R
-00053220: 6573 756c 745f 7374 7269 6e67 2b3d 2754  esult_string+='T
-00053230: 6865 206d 696e 696d 756d 2065 7272 6f72  he minimum error
-00053240: 2069 733a 7b3a 2e38 657d 5c6e 272e 666f   is:{:.8e}\n'.fo
-00053250: 726d 6174 2872 655b 2765 7272 6f72 275d  rmat(re['error']
-00053260: 290d 0a09 0974 7279 3a0d 0a09 0909 5265  )....try:.....Re
-00053270: 7375 6c74 5f73 7472 696e 672b 3d27 5468  sult_string+='Th
-00053280: 6520 6d69 6e69 6d75 6d20 5232 2d76 616c  e minimum R2-val
-00053290: 7565 2069 733a 7b3a 2e38 657d 5c6e 272e  ue is:{:.8e}\n'.
-000532a0: 666f 726d 6174 2872 655b 2772 3227 5d29  format(re['r2'])
-000532b0: 0d0a 0909 6578 6365 7074 3a0d 0a09 0909  ....except:.....
-000532c0: 7061 7373 0d0a 0909 6966 2073 616d 655f  pass....if same_
-000532d0: 4441 533a 0d0a 0909 0952 6573 756c 745f  DAS:.....Result_
-000532e0: 7374 7269 6e67 2b3d 2754 6865 206d 696e  string+='The min
-000532f0: 696d 756d 2067 6c6f 6261 6c20 6572 726f  imum global erro
-00053300: 7220 6973 3a7b 3a2e 3865 7d5c 6e27 2e66  r is:{:.8e}\n'.f
-00053310: 6f72 6d61 7428 7265 5b27 6572 726f 725f  ormat(re['error_
-00053320: 746f 7461 6c27 5d29 0d0a 0909 0952 6573  total']).....Res
-00053330: 756c 745f 7374 7269 6e67 2b3d 2754 6865  ult_string+='The
-00053340: 206d 696e 696d 756d 2067 6c6f 6261 6c20   minimum global 
-00053350: 5232 2d76 616c 7565 2069 733a 7b3a 2e38  R2-value is:{:.8
-00053360: 657d 5c6e 272e 666f 726d 6174 2872 655b  e}\n'.format(re[
-00053370: 2772 325f 746f 7461 6c27 5d29 0d0a 0909  'r2_total'])....
-00053380: 6966 2063 6f6e 6669 6465 6e63 655f 6c65  if confidence_le
-00053390: 7665 6c20 6973 206e 6f74 204e 6f6e 653a  vel is not None:
-000533a0: 0d0a 0909 0952 6573 756c 745f 7374 7269  .....Result_stri
-000533b0: 6e67 2b3d 275c 6e49 6e20 5261 7465 7320  ng+='\nIn Rates 
-000533c0: 7769 7468 2063 6f6e 6669 6465 6e63 6520  with confidence 
-000533d0: 696e 7465 7276 616c 2074 6f20 6c65 7665  interval to leve
-000533e0: 6c20 6f66 2025 2e31 665c 6e5c 6e27 2528  l of %.1f\n\n'%(
-000533f0: 2863 6f6e 6669 6465 6e63 655f 6c65 7665  (confidence_leve
-00053400: 6c29 2a31 3030 290d 0a09 0909 5265 7375  l)*100).....Resu
-00053410: 6c74 5f73 7472 696e 672b 3d70 6172 6466  lt_string+=pardf
-00053420: 2e74 6f5f 7374 7269 6e67 2863 6f6c 756d  .to_string(colum
-00053430: 6e73 3d5b 2776 616c 7565 272c 276c 6f77  ns=['value','low
-00053440: 6572 5f6c 696d 6974 272c 2775 7070 6572  er_limit','upper
-00053450: 5f6c 696d 6974 272c 2769 6e69 745f 7661  _limit','init_va
-00053460: 6c75 6527 2c27 7661 7279 272c 276d 696e  lue','vary','min
-00053470: 272c 276d 6178 272c 2765 7870 7227 5d29  ','max','expr'])
-00053480: 0d0a 0909 0952 6573 756c 745f 7374 7269  .....Result_stri
-00053490: 6e67 2b3d 275c 6e5c 6e54 6865 2072 6174  ng+='\n\nThe rat
-000534a0: 6573 2063 6f6e 7665 7274 6564 2074 6f20  es converted to 
-000534b0: 7469 6d65 7320 7769 7468 2075 6e69 7420  times with unit 
-000534c0: 2573 2077 6974 6820 636f 6e66 6964 656e  %s with confiden
-000534d0: 6365 2069 6e74 6572 7661 6c20 746f 206c  ce interval to l
-000534e0: 6576 656c 206f 6620 252e 3166 5c6e 5c6e  evel of %.1f\n\n
-000534f0: 2725 2873 656c 662e 6261 7365 756e 6974  '%(self.baseunit
-00053500: 2c28 636f 6e66 6964 656e 6365 5f6c 6576  ,(confidence_lev
-00053510: 656c 292a 3130 3029 0d0a 0909 0952 6573  el)*100).....Res
-00053520: 756c 745f 7374 7269 6e67 2b3d 7469 6d65  ult_string+=time
-00053530: 6466 2e74 6f5f 7374 7269 6e67 2863 6f6c  df.to_string(col
-00053540: 756d 6e73 3d5b 2776 616c 7565 272c 276c  umns=['value','l
-00053550: 6f77 6572 5f6c 696d 6974 272c 2775 7070  ower_limit','upp
-00053560: 6572 5f6c 696d 6974 272c 2769 6e69 745f  er_limit','init_
-00053570: 7661 6c75 6527 2c27 7661 7279 272c 276d  value','vary','m
-00053580: 696e 272c 276d 6178 272c 2765 7870 7227  in','max','expr'
-00053590: 5d29 0d0a 0909 656c 7365 3a0d 0a09 0909  ])....else:.....
-000535a0: 5265 7375 6c74 5f73 7472 696e 672b 3d27  Result_string+='
-000535b0: 5c6e 496e 2052 6174 6573 5c6e 5c6e 270d  \nIn Rates\n\n'.
-000535c0: 0a09 0909 5265 7375 6c74 5f73 7472 696e  ....Result_strin
-000535d0: 672b 3d70 6172 6466 2e74 6f5f 7374 7269  g+=pardf.to_stri
-000535e0: 6e67 2863 6f6c 756d 6e73 3d5b 2776 616c  ng(columns=['val
-000535f0: 7565 272c 2769 6e69 745f 7661 6c75 6527  ue','init_value'
-00053600: 2c27 7661 7279 272c 276d 696e 272c 276d  ,'vary','min','m
-00053610: 6178 272c 2765 7870 7227 5d29 0d0a 0909  ax','expr'])....
-00053620: 0952 6573 756c 745f 7374 7269 6e67 2b3d  .Result_string+=
-00053630: 275c 6e5c 6e54 6865 2072 6174 6573 2063  '\n\nThe rates c
-00053640: 6f6e 7665 7274 6564 2074 6f20 7469 6d65  onverted to time
-00053650: 7320 7769 7468 2075 6e69 7420 2573 5c6e  s with unit %s\n
-00053660: 5c6e 2725 7365 6c66 2e62 6173 6575 6e69  \n'%self.baseuni
-00053670: 740d 0a09 0909 5265 7375 6c74 5f73 7472  t.....Result_str
-00053680: 696e 672b 3d74 696d 6564 662e 746f 5f73  ing+=timedf.to_s
-00053690: 7472 696e 6728 636f 6c75 6d6e 733d 5b27  tring(columns=['
-000536a0: 7661 6c75 6527 2c27 696e 6974 5f76 616c  value','init_val
-000536b0: 7565 272c 2776 6172 7927 2c27 6d69 6e27  ue','vary','min'
-000536c0: 2c27 6d61 7827 2c27 6578 7072 275d 290d  ,'max','expr']).
-000536d0: 0a09 0969 6620 7361 6d65 5f44 4153 3a0d  ...if same_DAS:.
-000536e0: 0a09 0909 5265 7375 6c74 5f73 7472 696e  ....Result_strin
-000536f0: 672b 3d27 5c6e 5c6e 7468 6520 6f74 6865  g+='\n\nthe othe
-00053700: 7220 6f62 6a65 6374 7320 7765 7265 206c  r objects were l
-00053710: 6179 6564 2069 6e74 6f20 7365 6c66 2e6d  ayed into self.m
-00053720: 756c 7469 5f70 726f 6a65 6374 7320 6173  ulti_projects as
-00053730: 206c 6973 7420 7769 7468 2074 6865 206c   list with the l
-00053740: 6f63 616c 2072 6520 6f6e 2070 6f73 6974  ocal re on posit
-00053750: 696f 6e20 302e 5c6e 2042 7920 7265 706c  ion 0.\n By repl
-00053760: 6163 696e 6720 6173 7375 6d69 6e67 2074  acing assuming t
-00053770: 6861 7420 7365 6c66 203d 2074 6120 7772  hat self = ta wr
-00053780: 6974 653a 205c 6e20 7461 2e72 6520 3d20  ite: \n ta.re = 
-00053790: 7461 2e6d 756c 7469 5f70 726f 6a65 6374  ta.multi_project
-000537a0: 735b 315d 2061 6e64 2074 6865 6e20 7461  s[1] and then ta
-000537b0: 2e50 6c6f 745f 6669 745f 6f75 7470 7574  .Plot_fit_output
-000537c0: 2074 6f20 6c6f 6f6b 206f 6e20 7468 6520   to look on the 
-000537d0: 6f74 6865 7220 6669 7473 5c6e 2027 0d0a  other fits\n '..
-000537e0: 0909 090d 0a09 0970 7269 6e74 2852 6573  .......print(Res
-000537f0: 756c 745f 7374 7269 6e67 290d 0a09 090d  ult_string).....
-00053800: 0a09 0969 6620 6475 6d70 5f70 6172 6173  ...if dump_paras
-00053810: 3a0d 0a09 0909 7769 7468 206f 7065 6e28  :.....with open(
-00053820: 2246 6974 5f72 6573 756c 7473 5f70 7269  "Fit_results_pri
-00053830: 6e74 2e70 6172 222c 2022 7722 2920 6173  nt.par", "w") as
-00053840: 2074 6578 745f 6669 6c65 3a0d 0a09 0909   text_file:.....
-00053850: 0974 6578 745f 6669 6c65 2e77 7269 7465  .text_file.write
-00053860: 2852 6573 756c 745f 7374 7269 6e67 290d  (Result_string).
-00053870: 0a09 0909 0d0a 0909 090d 0a09 6465 6620  ............def 
-00053880: 506c 6f74 5f66 6974 5f6f 7574 7075 7428  Plot_fit_output(
-00053890: 7365 6c66 2c20 706c 6f74 7469 6e67 203d  self, plotting =
-000538a0: 2072 616e 6765 2836 292c 2070 6174 6820   range(6), path 
-000538b0: 3d20 2772 6573 756c 745f 6669 6775 7265  = 'result_figure
-000538c0: 7327 2c20 7361 7665 7479 7065 203d 2027  s', savetype = '
-000538d0: 706e 6727 2c20 0d0a 0909 0909 0909 6576  png', ........ev
-000538e0: 616c 7561 7469 6f6e 5f73 7479 6c65 203d  aluation_style =
-000538f0: 2046 616c 7365 2c20 7469 746c 6520 3d20   False, title = 
-00053900: 4e6f 6e65 2c20 7363 616c 655f 7479 7065  None, scale_type
-00053910: 203d 2027 7379 6d6c 6f67 272c 200d 0a09   = 'symlog', ...
-00053920: 0909 0909 0970 6174 6368 6573 203d 2046  .....patches = F
-00053930: 616c 7365 2c20 6669 6c65 6e61 6d65 203d  alse, filename =
-00053940: 204e 6f6e 652c 2063 6d61 7020 3d20 4e6f   None, cmap = No
-00053950: 6e65 202c 2070 7269 6e74 5f63 6c69 636b  ne , print_click
-00053960: 5f70 6f73 6974 696f 6e20 3d20 4661 6c73  _position = Fals
-00053970: 652c 0d0a 0909 0909 0909 706c 6f74 5f73  e,........plot_s
-00053980: 6563 6f6e 645f 6173 5f65 6e65 7267 7920  econd_as_energy 
-00053990: 3d20 5472 7565 293a 0d0a 0909 0909 0909  = True):........
-000539a0: 0909 0909 0909 0909 0909 0920 0d0a 0909  ........... ....
-000539b0: 2727 2770 6c6f 7473 2061 6c6c 2074 6865  '''plots all the
-000539c0: 2066 6974 206f 7574 7075 7420 6669 6775   fit output figu
-000539d0: 7265 732e 2054 6865 2066 6967 7572 6573  res. The figures
-000539e0: 2063 616e 2062 6520 6361 6c6c 6564 2073   can be called s
-000539f0: 6570 6172 6174 656c 7920 0d0a 0909 6f72  eparately ....or
-00053a00: 2077 6974 6820 6120 6c69 7374 206f 6620   with a list of 
-00053a10: 706c 6f74 732e 2065 2e67 2e20 7261 6e67  plots. e.g. rang
-00053a20: 6528 3629 2063 616c 6c20 706c 6f74 7320  e(6) call plots 
-00053a30: 302d 3520 4d61 6e75 616c 2070 6c6f 7474  0-5 Manual plott
-00053a40: 696e 6720 6f66 2063 6572 7461 696e 2074  ing of certain t
-00053a50: 7970 653a 0d0a 0909 0d0a 0909 5468 6973  ype:........This
-00053a60: 2069 7320 6120 7772 6170 7065 7220 6675   is a wrapper fu
-00053a70: 6e63 7469 6f6e 2074 6861 7420 7472 6967  nction that trig
-00053a80: 6765 7273 2074 6865 2070 6c6f 7474 696e  gers the plottin
-00053a90: 6720 6f66 2061 6c6c 2074 6865 2066 6974  g of all the fit
-00053aa0: 7465 6420 706c 6f74 732e 0d0a 0909 5468  ted plots.....Th
-00053ab0: 6520 7061 7261 6d65 7465 7220 696e 2074  e parameter in t
-00053ac0: 6869 7320 706c 6f74 2063 616c 6c20 6172  his plot call ar
-00053ad0: 6520 746f 2063 6f6e 7472 6f6c 2074 6865  e to control the
-00053ae0: 2067 656e 6572 616c 206c 6f6f 6b20 616e   general look an
-00053af0: 6420 6665 6174 7572 6573 206f 6620 7468  d features of th
-00053b00: 6520 706c 6f74 2e0d 0a09 0957 6869 6368  e plot.....Which
-00053b10: 2070 6c6f 7473 2061 7265 2070 7269 6e74   plots are print
-00053b20: 6564 2069 7320 6465 6669 6e65 6420 6279  ed is defined by
-00053b30: 2074 6865 2066 6972 7374 2063 6f6d 6d61   the first comma
-00053b40: 6e64 2028 706c 6f74 7469 6e67 290d 0a09  nd (plotting)...
-00053b50: 0954 6865 2070 6c6f 7473 2061 7265 2067  .The plots are g
-00053b60: 656e 6572 6174 6564 2066 726f 6d20 7468  enerated from th
-00053b70: 6520 6669 7474 6564 204d 6174 7269 7865  e fitted Matrixe
-00053b80: 7320 616e 6420 6173 2073 7563 6820 6f6e  s and as such on
-00053b90: 6c79 2077 696c 6c20 776f 726b 2061 6674  ly will work aft
-00053ba0: 6572 2061 2066 6974 2077 6173 2061 6374  er a fit was act
-00053bb0: 7561 6c6c 790d 0a09 0963 6f6d 706c 6574  ually....complet
-00053bc0: 6564 2028 616e 6420 7468 6520 2272 6522  ed (and the "re"
-00053bd0: 2064 6963 7469 6f6e 6172 7920 6174 7461   dictionary atta
-00053be0: 6368 6564 2074 6f20 7468 6520 6f62 6a65  ched to the obje
-00053bf0: 6374 2e29 0d0a 0909 496e 2061 6c6c 2070  ct.)....In all p
-00053c00: 6c6f 7473 2074 6865 2052 4157 2064 6174  lots the RAW dat
-00053c10: 6120 6973 2070 6c6f 7474 6564 2061 7320  a is plotted as 
-00053c20: 646f 7473 2061 6e64 2074 6865 2066 6974  dots and the fit
-00053c30: 2077 6974 6820 6c69 6e65 7320 0d0a 0909   with lines ....
-00053c40: 0d0a 0909 436f 6e74 656e 7473 206f 6620  ....Contents of 
-00053c50: 7468 6520 706c 6f74 730d 0a0d 0a09 0909  the plots.......
-00053c60: 302e 2044 4143 2063 6f6e 7461 696e 7320  0. DAC contains 
-00053c70: 7468 6520 6173 7369 676e 6564 2073 7065  the assigned spe
-00053c80: 6374 7261 2066 6f72 2065 6163 6820 636f  ctra for each co
-00053c90: 6d70 6f6e 656e 7420 6f66 2074 6865 2066  mponent of the f
-00053ca0: 6974 2e20 466f 720d 0a09 0909 2020 2061  it. For.....   a
-00053cb0: 206d 6f64 656c 6c69 6e67 2077 6974 6820   modelling with 
-00053cc0: 696e 6465 7065 6e64 656e 7420 6578 706f  independent expo
-00053cd0: 6e65 6e74 6961 6c20 6465 6361 7973 2074  nential decays t
-00053ce0: 6869 7320 636f 7272 6573 706f 6e64 7320  his corresponds 
-00053cf0: 746f 0d0a 0909 0920 2020 7468 6520 2244  to.....   the "D
-00053d00: 6563 6179 2041 7373 6f63 6961 7465 6420  ecay Associated 
-00053d10: 5370 6563 7472 6122 2028 4441 5329 2e20  Spectra" (DAS). 
-00053d20: 466f 7220 616c 6c20 6f74 6865 7220 6d6f  For all other mo
-00053d30: 6465 6c73 2074 6869 730d 0a09 0909 2020  dels this.....  
-00053d40: 2063 6f6e 7461 696e 7320 7468 6520 2253   contains the "S
-00053d50: 7065 6369 6573 2041 7373 6f63 6961 7465  pecies Associate
-00053d60: 6420 5370 6563 7472 6122 2028 5341 5329  d Spectra" (SAS)
-00053d70: 2e20 4163 636f 7264 696e 6720 746f 2074  . According to t
-00053d80: 6865 0d0a 0909 0920 2020 6d6f 6465 6c20  he.....   model 
-00053d90: 7468 6520 7365 7061 7261 7465 2073 7065  the separate spe
-00053da0: 6374 7261 2061 7265 206c 6162 656c 6564  ctra are labeled
-00053db0: 2062 7920 7469 6d65 2028 7072 6f63 6573   by time (proces
-00053dc0: 7329 206f 7220 6e61 6d65 2c20 6966 0d0a  s) or name, if..
-00053dd0: 0909 0920 2020 6120 6e61 6d65 2069 7320  ...   a name is 
-00053de0: 6173 736f 6369 6174 6564 2069 6e20 7468  associated in th
-00053df0: 6520 6669 7474 696e 6720 6d6f 6465 6c2e  e fitting model.
-00053e00: 2054 6865 2073 7065 6374 7261 2061 7265   The spectra are
-00053e10: 2073 686f 776e 2069 6e0d 0a09 0909 2020   shown in.....  
-00053e20: 2074 6865 2065 7874 7261 6374 6564 2073   the extracted s
-00053e30: 7472 656e 6774 6820 696e 2074 6865 2072  trength in the r
-00053e40: 6967 6874 2070 616e 6520 616e 6420 6e6f  ight pane and no
-00053e50: 726d 616c 697a 6564 2069 6e20 7468 6520  rmalized in the 
-00053e60: 6c65 6674 2e0d 0a09 0909 2020 2045 7874  left......   Ext
-00053e70: 7261 6374 6564 2073 7472 656e 6774 6820  racted strength 
-00053e80: 6d65 616e 7320 7468 6174 2074 6865 206d  means that the m
-00053e90: 6561 7375 7265 6420 7370 6563 7472 616c  easured spectral
-00053ea0: 2073 7472 656e 6774 6820 6973 2074 6865   strength is the
-00053eb0: 0d0a 0909 0920 2020 696e 7465 6e73 6974  .....   intensit
-00053ec0: 7920 2863 6f6e 6365 6e74 7261 7469 6f6e  y (concentration
-00053ed0: 206d 6174 7269 7829 2074 696d 6573 2074   matrix) times t
-00053ee0: 6869 7320 7370 6563 7472 616c 2073 7472  his spectral str
-00053ef0: 656e 6774 682e 2041 7320 7468 650d 0a09  ength. As the...
-00053f00: 0909 2020 2063 6f6e 6365 6e74 7261 7469  ..   concentrati
-00053f10: 6f6e 206d 6178 696d 6120 666f 7220 616c  on maxima for al
-00053f20: 6c20 4441 5320 6172 6520 3120 7468 6973  l DAS are 1 this
-00053f30: 2063 6f72 7265 7370 6f6e 6473 2074 6f20   corresponds to 
-00053f40: 7468 650d 0a09 0909 2020 2073 7065 6374  the.....   spect
-00053f50: 7261 6c20 7374 7265 6e67 7468 2066 6f72  ral strength for
-00053f60: 2074 6865 2044 4153 2e20 2870 6c65 6173   the DAS. (pleas
-00053f70: 6520 7365 6520 7468 6520 646f 6375 6d65  e see the docume
-00053f80: 6e74 6174 696f 6e20 666f 7220 7468 650d  ntation for the.
-00053f90: 0a09 0909 2020 2066 6974 7469 6e67 2061  ....   fitting a
-00053fa0: 6c67 6f72 6974 686d 2066 6f72 2066 7572  lgorithm for fur
-00053fb0: 7468 6572 2064 6574 6169 6c73 292e 0d0a  ther details)...
-00053fc0: 0d0a 0909 0931 2e20 7375 6d6d 6564 2069  .....1. summed i
-00053fd0: 6e74 656e 7369 7479 2e20 416c 6c20 7761  ntensity. All wa
-00053fe0: 7665 6c65 6e67 7468 206f 6620 7468 6520  velength of the 
-00053ff0: 7370 6563 7472 616c 2061 7869 7320 6172  spectral axis ar
-00054000: 6520 7375 6d6d 6564 2066 6f72 0d0a 0909  e summed for....
-00054010: 0920 2020 6461 7461 2061 6e64 2066 6974  .   data and fit
-00054020: 2e20 5468 6520 6461 7461 2069 7320 706c  . The data is pl
-00054030: 6f74 7465 6420 696e 2061 206e 756d 6265  otted in a numbe
-00054040: 7220 6f66 2077 6179 7320 7673 206c 696e  r of ways vs lin
-00054050: 6561 7220 616e 640d 0a09 0909 2020 206c  ear and.....   l
-00054060: 6f67 6172 6974 686d 6963 2061 7869 732e  ogarithmic axis.
-00054070: 2054 6869 7320 706c 6f74 2069 7320 6e6f   This plot is no
-00054080: 7420 6d65 6e74 2066 6f72 2070 7562 6c69  t ment for publi
-00054090: 6361 7469 6f6e 2062 7574 2076 6572 790d  cation but very.
-000540a0: 0a09 0909 2020 2075 7365 6675 6c20 746f  ....   useful to
-000540b0: 2065 7661 6c75 6174 6520 7468 6520 7175   evaluate the qu
-000540c0: 616c 6974 7920 6f66 2061 2066 6974 2e0d  ality of a fit..
-000540d0: 0a0d 0a09 0909 322e 2070 6c6f 7420 6b69  ......2. plot ki
-000540e0: 6e65 7469 6373 2066 6f72 2073 656c 6563  netics for selec
-000540f0: 7465 6420 7761 7665 6c65 6e67 7468 2028  ted wavelength (
-00054100: 7365 6520 636f 7272 6573 706f 6e64 696e  see correspondin
-00054110: 6720 5241 5720 706c 6f74 292e 0d0a 0d0a  g RAW plot).....
-00054120: 0909 0933 2e20 706c 6f74 2073 7065 6374  ...3. plot spect
-00054130: 7261 2061 7420 7365 6c65 6374 6564 2074  ra at selected t
-00054140: 696d 6573 2028 7365 6520 636f 7272 6573  imes (see corres
-00054150: 706f 6e64 696e 6720 5241 5720 706c 6f74  ponding RAW plot
-00054160: 292e 0d0a 0d0a 0909 0934 2e20 706c 6f74  )........4. plot
-00054170: 7320 6d61 7472 6978 2028 6d65 6173 7572  s matrix (measur
-00054180: 6564 2c20 6d6f 6465 6c6c 6564 2061 6e64  ed, modelled and
-00054190: 2065 7272 6f72 204d 6174 7269 7829 2e20   error Matrix). 
-000541a0: 5468 6520 7061 7261 6d65 7465 7220 6172  The parameter ar
-000541b0: 650d 0a09 0909 2020 2074 6865 2073 616d  e.....   the sam
-000541c0: 6520 6173 2075 7365 6420 666f 7220 7468  e as used for th
-000541d0: 6520 636f 7272 6573 706f 6e64 696e 6720  e corresponding 
-000541e0: 5241 5720 706c 6f74 2077 6974 6820 7468  RAW plot with th
-000541f0: 6520 6164 6469 7469 6f6e 206f 660d 0a09  e addition of...
-00054200: 0909 2020 2022 6572 726f 725f 6d61 7472  ..   "error_matr
-00054210: 6978 5f61 6d70 6c69 6669 6361 7469 6f6e  ix_amplification
-00054220: 2220 7768 6963 6820 6973 2061 2073 6361  " which is a sca
-00054230: 6c69 6e67 2066 6163 746f 7220 6d75 6c74  ling factor mult
-00054240: 6970 6c69 6564 0d0a 0909 0920 2020 6f6e  iplied.....   on
-00054250: 746f 2074 6865 2065 7272 6f72 206d 6174  to the error mat
-00054260: 7269 782e 2049 2072 6563 6f6d 6d65 6e64  rix. I recommend
-00054270: 2074 6f20 706c 6179 2077 6974 6820 6469   to play with di
-00054280: 6666 6572 656e 7420 2263 6d61 7022 2c0d  fferent "cmap",.
-00054290: 0a09 0909 2020 2022 6c6f 675f 7363 616c  ....   "log_scal
-000542a0: 6522 2061 6e64 2022 696e 7465 6e73 6974  e" and "intensit
-000542b0: 795f 7363 616c 6522 2074 6f20 6372 6561  y_scale" to crea
-000542c0: 7465 2061 2070 6c65 6173 696e 6720 706c  te a pleasing pl
-000542d0: 6f74 2e0d 0a0d 0a09 0909 352e 2063 6f6e  ot........5. con
-000542e0: 6365 6e74 7261 7469 6f6e 732e 2049 6e20  centrations. In 
-000542f0: 7468 6520 7072 6f67 7265 7373 206f 6620  the progress of 
-00054300: 7468 6520 6d6f 6465 6c6c 696e 672f 6669  the modelling/fi
-00054310: 7474 696e 6720 6120 6d61 7472 6978 2069  tting a matrix i
-00054320: 730d 0a09 0909 2020 2067 656e 6572 6174  s.....   generat
-00054330: 6564 2074 6861 7420 636f 6e74 6169 6e73  ed that contains
-00054340: 2074 6865 2072 656c 6174 6976 6520 636f   the relative co
-00054350: 6e63 656e 7472 6174 696f 6e73 206f 6620  ncentrations of 
-00054360: 7468 6520 7370 6563 6965 730d 0a09 0909  the species.....
-00054370: 2020 206d 6f64 656c 6c65 642e 2054 6869     modelled. Thi
-00054380: 7320 706c 6f74 2069 7320 7368 6f77 696e  s plot is showin
-00054390: 6720 7468 6520 7465 6d70 6f72 616c 2064  g the temporal d
-000543a0: 6576 656c 6f70 6d65 6e74 206f 6620 7468  evelopment of th
-000543b0: 6573 650d 0a09 0909 2020 2073 7065 6369  ese.....   speci
-000543c0: 6573 2e20 4675 7274 6865 7220 6465 7461  es. Further deta
-000543d0: 696c 7320 6f6e 2068 6f77 2074 6869 7320  ils on how this 
-000543e0: 6d61 7472 6978 2069 7320 6765 6e65 7261  matrix is genera
-000543f0: 7465 6420 6361 6e20 6265 2066 6f75 6e64  ted can be found
-00054400: 0d0a 0909 0920 2020 696e 2074 6865 2064  .....   in the d
-00054410: 6f63 756d 656e 7461 7469 6f6e 206f 6620  ocumentation of 
-00054420: 7468 6520 6669 7474 696e 6720 6675 6e63  the fitting func
-00054430: 7469 6f6e 2e20 5468 6520 6d6f 6465 6c65  tion. The modele
-00054440: 6420 7370 6563 7472 6120 6172 650d 0a09  d spectra are...
-00054450: 0909 2020 2074 6865 2063 6f6e 766f 6c75  ..   the convolu
-00054460: 7469 6f6e 206f 6620 7468 6573 6520 7665  tion of these ve
-00054470: 6374 6f72 7320 2867 6976 696e 6720 7468  ctors (giving th
-00054480: 6520 7469 6d65 2d64 6576 656c 6f70 6d65  e time-developme
-00054490: 6e74 2920 616e 640d 0a09 0909 2020 2074  nt) and.....   t
-000544a0: 6865 2044 4153 2f53 4153 2028 6769 7669  he DAS/SAS (givi
-000544b0: 6e67 2074 6865 2073 7065 6374 7261 6c20  ng the spectral 
-000544c0: 6465 7665 6c6f 706d 656e 7429 2e0d 0a09  development)....
-000544d0: 090d 0a09 0950 6172 616d 6574 6572 730d  .....Parameters.
-000544e0: 0a09 092d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ...-------------
-000544f0: 2d2d 0d0a 0909 0d0a 0909 706c 6f74 7469  --........plotti
-00054500: 6e67 203a 2069 6e74 206f 7220 6974 6572  ng : int or iter
-00054510: 6162 6c65 2028 6f66 2069 6e74 6567 6572  able (of integer
-00054520: 7329 2c20 6f70 7469 6f6e 616c 0d0a 0909  s), optional....
-00054530: 0954 6869 7320 7061 7261 6d65 7465 7220  .This parameter 
-00054540: 6465 7465 726d 696e 6573 2077 6869 6368  determines which
-00054550: 2066 6967 7572 6573 2061 7265 2070 6c6f   figures are plo
-00054560: 7474 6564 200d 0a09 0909 7468 6520 6669  tted .....the fi
-00054570: 6775 7265 7320 6361 6e20 6265 2063 616c  gures can be cal
-00054580: 6c65 6420 7365 7061 7261 7465 6c79 2077  led separately w
-00054590: 6974 6820 706c 6f74 7469 6e67 203d 2031  ith plotting = 1
-000545a0: 0d0a 0909 096f 7220 7769 7468 2061 206c  .....or with a l
-000545b0: 6973 7420 6f66 2070 6c6f 7473 2028 4465  ist of plots (De
-000545c0: 6661 756c 7429 2065 2e67 2e20 706c 6f74  fault) e.g. plot
-000545d0: 7469 6e67 3d72 616e 6765 2836 2920 6361  ting=range(6) ca
-000545e0: 6c6c 7320 706c 6f74 7320 302c 312c 322c  lls plots 0,1,2,
-000545f0: 332c 342c 350d 0a09 0909 5468 6520 706c  3,4,5.....The pl
-00054600: 6f74 7320 6861 7665 2074 6865 2066 6f6c  ots have the fol
-00054610: 6c6f 7769 6e67 206e 756d 6265 7273 3a0d  lowing numbers:.
-00054620: 0a09 0909 0d0a 0909 0909 302e 2044 4153  ..........0. DAS
-00054630: 206f 7220 5341 530d 0a09 0909 0931 2e20   or SAS......1. 
-00054640: 7375 6d6d 6564 2069 6e74 656e 7369 7479  summed intensity
-00054650: 0d0a 0909 0909 322e 204b 696e 6574 6963  ......2. Kinetic
-00054660: 730d 0a09 0909 0933 2e20 5370 6563 7472  s......3. Spectr
-00054670: 610d 0a09 0909 0934 2e20 4d61 7472 6978  a......4. Matrix
-00054680: 6573 0d0a 0909 0909 352e 2043 6f6e 6365  es......5. Conce
-00054690: 6e74 7261 7469 6f6e 7320 2874 6865 2063  ntrations (the c
-000546a0: 2d6f 626a 6563 7429 0d0a 0909 090d 0a09  -object)........
-000546b0: 0909 5468 6520 706c 6f74 7469 6e67 2074  ..The plotting t
-000546c0: 616b 6573 2061 6c6c 2070 6172 616d 6574  akes all paramet
-000546d0: 6572 2066 726f 6d20 7468 6520 2274 6122  er from the "ta"
-000546e0: 206f 626a 6563 7420 756e 6c65 7373 206f   object unless o
-000546f0: 7468 6572 7769 7365 2073 7065 6369 6669  therwise specifi
-00054700: 6564 0d0a 0909 0d0a 0909 7061 7468 203a  ed........path :
-00054710: 204e 6f6e 652c 2073 7472 206f 7220 7061   None, str or pa
-00054720: 7468 206f 626a 6563 742c 206f 7074 696f  th object, optio
-00054730: 6e61 6c0d 0a09 0909 5468 6973 2064 6566  nal.....This def
-00054740: 696e 6573 2077 6865 7265 2074 6865 2066  ines where the f
-00054750: 696c 6573 2061 7265 2073 6176 6564 2069  iles are saved i
-00054760: 6620 7468 6520 7361 6665 5f66 6967 7572  f the safe_figur
-00054770: 6573 5f74 6f5f 666f 6c64 6572 2070 6172  es_to_folder par
-00054780: 616d 6574 6572 2069 7320 5472 7565 2c20  ameter is True, 
-00054790: 0d0a 0909 0971 7569 7465 2075 7365 6675  .....quite usefu
-000547a0: 6c20 6966 2061 206c 6f74 206f 6620 6461  l if a lot of da
-000547b0: 7461 2073 6574 7320 6172 6520 746f 2062  ta sets are to b
-000547c0: 6520 7072 696e 7465 6420 6661 7374 2e20  e printed fast. 
-000547d0: 0d0a 0909 0949 6620 6120 7061 7468 2069  .....If a path i
-000547e0: 7320 6769 7665 6e2c 2074 6869 7320 6973  s given, this is
-000547f0: 2075 7365 642e 2049 6620 6120 7374 7269   used. If a stri
-00054800: 6e67 206c 696b 6520 7468 6520 2844 6566  ng like the (Def
-00054810: 6175 6c74 2920 2272 6573 756c 745f 6669  ault) "result_fi
-00054820: 6775 7265 7322 2069 7320 6769 7665 6e2c  gures" is given,
-00054830: 200d 0a09 0909 7468 656e 2061 2073 7562   .....then a sub
-00054840: 666f 6c64 6572 206f 6620 7468 6973 206e  folder of this n
-00054850: 616d 6520 7769 6c6c 2062 6520 7573 6564  ame will be used
-00054860: 2028 616e 2067 656e 6572 6174 6564 2069   (an generated i
-00054870: 6620 6e65 6365 7373 6172 7929 200d 0a09  f necessary) ...
-00054880: 0909 7265 6c61 7469 7665 2074 6f20 7365  ..relative to se
-00054890: 6c66 2e70 6174 682e 2055 7365 2061 6e64  lf.path. Use and
-000548a0: 2065 6d70 7479 2073 7472 696e 6720 746f   empty string to
-000548b0: 2075 7365 2074 6865 2073 656c 662e 7061   use the self.pa
-000548c0: 7468 0d0a 0909 0949 6620 7365 7420 746f  th.....If set to
-000548d0: 204e 6f6e 652c 2074 6865 206c 6f63 6174   None, the locat
-000548e0: 696f 6e20 6f66 2074 6865 2070 6c6f 745f  ion of the plot_
-000548f0: 6675 6e63 2077 696c 6c20 6265 2075 7365  func will be use
-00054900: 6420 616e 640d 0a09 0909 6120 7375 6266  d and.....a subf
-00054910: 6f6c 6465 7220 7769 7468 2074 6974 6c65  older with title
-00054920: 2022 7265 7375 6c74 5f66 6967 7572 6573   "result_figures
-00054930: 2220 6265 2067 656e 6572 6174 6564 2068  " be generated h
-00054940: 6572 650d 0a09 090d 0a09 0973 6176 6574  ere........savet
-00054950: 7970 6520 3a20 7374 7220 6f72 2069 7465  ype : str or ite
-00054960: 7261 626c 6520 286f 6620 7374 7229 2c20  rable (of str), 
-00054970: 6f70 7469 6f6e 616c 200d 0a09 0909 6d61  optional .....ma
-00054980: 7470 6c6f 746c 6962 2061 6c6c 6f77 7320  tplotlib allows 
-00054990: 7468 6520 7361 7669 6e67 206f 6620 6669  the saving of fi
-000549a0: 6775 7265 7320 696e 2076 6172 696f 7573  gures in various
-000549b0: 2066 6f72 6d61 7473 2e20 2844 6566 6175   formats. (Defau
-000549c0: 6c74 2920 2270 6e67 222c 200d 0a09 0909  lt) "png", .....
-000549d0: 7479 7069 6361 6c20 616e 6420 7265 636f  typical and reco
-000549e0: 6d6d 656e 6461 626c 6520 6f70 7469 6f6e  mmendable option
-000549f0: 7320 6172 6520 2273 7667 2220 616e 6420  s are "svg" and 
-00054a00: 2270 6466 222e 2020 0d0a 0909 090d 0a09  "pdf".  ........
-00054a10: 0965 7661 6c75 6174 696f 6e5f 7374 796c  .evaluation_styl
-00054a20: 6520 3a20 626f 6f6c 2c20 6f70 7469 6f6e  e : bool, option
-00054a30: 616c 0d0a 0909 0954 7275 6520 2844 6566  al.....True (Def
-00054a40: 6175 6c74 203d 2046 616c 7365 2920 6164  ault = False) ad
-00054a50: 6473 2061 206c 6f74 206f 6620 6578 7472  ds a lot of extr
-00054a60: 6120 696e 666f 726d 6174 696f 6e20 696e  a information in
-00054a70: 2074 6865 2070 6c6f 740d 0a09 090d 0a09   the plot.......
-00054a80: 0974 6974 6c65 203a 204e 6f6e 6520 6f72  .title : None or
-00054a90: 2073 7472 2c20 6f70 7469 6f6e 616c 0d0a   str, optional..
-00054aa0: 0909 2020 2022 7469 746c 653d 4e6f 6e65  ..   "title=None
-00054ab0: 2220 6973 2069 6e20 6765 6e65 7261 6c20  " is in general 
-00054ac0: 7468 6520 6669 6c65 6e61 6d65 2074 6861  the filename tha
-00054ad0: 7420 7761 7320 6c6f 6164 6564 2e20 5365  t was loaded. Se
-00054ae0: 7474 696e 6720 610d 0a09 0920 2020 7370  tting a....   sp
-00054af0: 6563 6966 6963 2074 6974 6c65 2077 696c  ecific title wil
-00054b00: 6c20 6265 2075 7365 6420 696e 2061 6c6c  l be used in all
-00054b10: 2070 6c6f 7473 2e20 546f 2072 656d 6f76   plots. To remov
-00054b20: 6520 7468 6520 7469 746c 6520 616c 6c0d  e the title all.
-00054b30: 0a09 0920 2020 746f 6765 7468 6572 2073  ...   together s
-00054b40: 6574 2061 6e20 656d 7074 7920 7374 7269  et an empty stri
-00054b50: 6e67 2077 6974 6820 7469 746c 653d 2222  ng with title=""
-00054b60: 0d0a 0909 2020 200d 0a09 0973 6361 6c65  ....   ....scale
-00054b70: 5f74 7970 6520 3a20 7374 722c 206f 7074  _type : str, opt
-00054b80: 696f 6e61 6c0d 0a09 0920 2020 7265 6665  ional....   refe
-00054b90: 7273 2074 6f20 7468 6520 7469 6d65 2d61  rs to the time-a
-00054ba0: 7869 7320 616e 6420 7461 6b65 732c 2022  xis and takes, "
-00054bb0: 7379 6d6c 6f67 2220 2844 6566 6175 6c74  symlog" (Default
-00054bc0: 2928 6c69 6e65 6172 2061 726f 756e 6420  )(linear around 
-00054bd0: 7a65 726f 2061 6e64 206c 6f67 6172 6974  zero and logarit
-00054be0: 686d 6963 206f 7468 6572 7769 7365 290d  hmic otherwise).
-00054bf0: 0a09 0920 2020 616e 6420 226c 696e 2220  ...   and "lin" 
-00054c00: 666f 7220 6c69 6e65 6172 2061 6e64 2020  for linear and  
-00054c10: 226c 6f67 2220 666f 7220 6c6f 6761 7269  "log" for logari
-00054c20: 7468 6d69 632c 2073 7769 7463 6869 6e67  thmic, switching
-00054c30: 2061 6c6c 2074 6865 2074 696d 6520 6178   all the time ax
-00054c40: 6973 2074 6f20 7468 6973 2074 7970 650d  is to this type.
-00054c50: 0a09 090d 0a09 0970 6174 6368 6573 203a  .......patches :
-00054c60: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0d   bool, optional.
-00054c70: 0a09 0909 4966 2046 616c 7365 2028 4465  ....If False (De
-00054c80: 6661 756c 7429 2074 6865 206e 616d 6573  fault) the names
-00054c90: 2022 6d65 6173 7572 6564 2220 2266 6974   "measured" "fit
-00054ca0: 7465 6422 2022 6469 6666 6572 656e 6365  ted" "difference
-00054cb0: 2220 7769 6c6c 2062 6520 706c 6163 6564  " will be placed
-00054cc0: 2061 626f 7665 2074 6865 2069 6d61 6765   above the image
-00054cd0: 732e 0d0a 0909 0949 6620 5472 7565 2c20  s......If True, 
-00054ce0: 7468 656e 2074 6865 7920 7769 6c6c 2062  then they will b
-00054cf0: 6520 696e 636c 7564 6564 2069 6e74 6f20  e included into 
-00054d00: 7468 6520 696d 6167 6520 2864 656e 7365  the image (dense
-00054d10: 7229 0d0a 0d0a 0909 6669 6c65 6e61 6d65  r)......filename
-00054d20: 203a 2073 7472 2c20 6f70 7469 6f6e 616c   : str, optional
-00054d30: 0d0a 0909 096f 6666 6572 7320 746f 2072  .....offers to r
-00054d40: 6570 6c61 6365 2074 6865 2062 6173 652d  eplace the base-
-00054d50: 6e61 6d65 2075 7365 6420 666f 7220 616c  name used for al
-00054d60: 6c20 706c 6f74 7320 2874 6f20 652e 672e  l plots (to e.g.
-00054d70: 7370 6563 6966 7920 7768 6174 2073 616d  specify what sam
-00054d80: 706c 6520 7761 7320 7573 6564 292e 200d  ple was used). .
-00054d90: 0a09 0909 6966 2028 4465 6661 756c 7429  ....if (Default)
-00054da0: 204e 6f6e 6520 6973 2075 7365 642c 2074   None is used, t
-00054db0: 6865 2073 656c 662e 6669 6c65 6e61 6d65  he self.filename
-00054dc0: 2069 7320 7573 6564 2061 7320 6120 6261   is used as a ba
-00054dd0: 7365 206e 616d 652e 2054 6865 2066 696c  se name. The fil
-00054de0: 656e 616d 6520 706c 6179 7320 6f6e 6c79  ename plays only
-00054df0: 2061 200d 0a09 0909 726f 6c65 2064 7572   a .....role dur
-00054e00: 696e 6720 7361 7669 6e67 2c20 6173 2064  ing saving, as d
-00054e10: 6f65 7320 7468 6520 7061 7468 2061 6e64  oes the path and
-00054e20: 2073 6176 6574 7970 6509 0d0a 0909 090d   savetype.......
-00054e30: 0a09 0963 6d61 7020 3a20 4e6f 6e65 206f  ...cmap : None o
-00054e40: 7220 6d61 7470 6c6f 746c 6962 2063 6f6c  r matplotlib col
-00054e50: 6f72 206d 6170 2c20 6f70 7469 6f6e 616c  or map, optional
-00054e60: 0d0a 0909 0969 7320 6120 706f 7765 7266  .....is a powerf
-00054e70: 756c 6c20 7661 7269 6162 6c65 2074 6861  ull variable tha
-00054e80: 7420 6368 6f6f 7365 7320 7468 6520 636f  t chooses the co
-00054e90: 6c6f 7572 206d 6170 2061 7070 6c69 6564  lour map applied
-00054ea0: 2066 6f72 2061 6c6c 2070 6c6f 7473 2e20   for all plots. 
-00054eb0: 4966 2073 6574 2074 6f20 0d0a 0909 094e  If set to .....N
-00054ec0: 6f6e 6520 2844 6566 6175 6c74 2920 7468  one (Default) th
-00054ed0: 656e 2074 6865 2073 656c 662e 636d 6170  en the self.cmap
-00054ee0: 2069 7320 7573 6564 2e0d 0a09 0909 4173   is used......As
-00054ef0: 2073 7461 6e64 6172 6420 4920 7573 6520   standard I use 
-00054f00: 7468 6520 636f 6c6f 7220 6d61 7020 226a  the color map "j
-00054f10: 6574 2220 6672 6f6d 206d 6174 706c 6f74  et" from matplot
-00054f20: 6c69 622e 2054 6865 7265 2061 7265 2061  lib. There are a
-00054f30: 2076 6172 6965 7479 206f 6620 636f 6c6f   variety of colo
-00054f40: 726d 6170 7320 0d0a 0909 0961 7661 696c  rmaps .....avail
-00054f50: 6162 6c65 2074 6861 7420 6172 6520 7665  able that are ve
-00054f60: 7279 2075 7365 6675 6c6c 2e20 4265 7369  ry usefull. Besi
-00054f70: 6465 2022 6a65 7422 2c20 2276 6972 6964  de "jet", "virid
-00054f80: 6973 2220 6973 2061 2067 6f6f 6420 6368  is" is a good ch
-00054f90: 6f69 6365 2061 7320 6974 2069 7320 7765  oice as it is we
-00054fa0: 6c6c 200d 0a09 0909 7669 7369 626c 6520  ll .....visible 
-00054fb0: 756e 6465 7220 7265 642d 6772 6565 6e20  under red-green 
-00054fc0: 626c 696e 646e 6573 732e 204f 7468 6572  blindness. Other
-00054fd0: 2075 7365 6675 6c20 6d61 7073 2061 7265   useful maps are
-00054fe0: 2022 7072 6973 6d22 2066 6f72 2068 6967   "prism" for hig
-00054ff0: 6820 666c 7563 7475 6174 696f 6e73 200d  h fluctuations .
-00055000: 0a09 0909 6f72 2064 6976 6572 6769 6e67  ....or diverging
-00055010: 2063 6f6c 6f72 206d 6170 7320 6c69 6b65   color maps like
-00055020: 2022 7365 6973 6d69 6322 2e20 0d0a 0909   "seismic". ....
-00055030: 0953 6565 2068 7474 7073 3a2f 2f6d 6174  .See https://mat
-00055040: 706c 6f74 6c69 622e 6f72 672f 332e 312e  plotlib.org/3.1.
-00055050: 302f 7475 746f 7269 616c 732f 636f 6c6f  0/tutorials/colo
-00055060: 7273 2f63 6f6c 6f72 6d61 7073 2e68 746d  rs/colormaps.htm
-00055070: 6c20 666f 7220 6120 636f 6d70 7265 6865  l for a comprehe
-00055080: 6e73 6976 6520 0d0a 0909 0973 656c 6563  nsive .....selec
-00055090: 7469 6f6e 2e20 496e 2074 6865 2063 6f64  tion. In the cod
-000550a0: 6520 7468 6520 636f 6c6f 726d 6170 7320  e the colormaps 
-000550b0: 6172 6520 696d 706f 7274 6564 2073 6f20  are imported so 
-000550c0: 6966 2070 6c6f 745f 6675 6e63 2069 7320  if plot_func is 
-000550d0: 696d 706f 7274 6564 2061 7320 7066 2074  imported as pf t
-000550e0: 6865 6e20 0d0a 0909 0973 656c 662e 636d  hen .....self.cm
-000550f0: 6170 3d70 662e 636d 2e76 6972 6964 6973  ap=pf.cm.viridis
-00055100: 2073 6574 7320 7669 7269 6469 7320 6173   sets viridis as
-00055110: 2074 6865 206d 6170 2074 6f20 7573 652e   the map to use.
-00055120: 2049 6e74 6572 6e61 6c6c 7920 7468 6520   Internally the 
-00055130: 636f 6c6f 7273 2061 7265 2063 686f 7365  colors are chose
-00055140: 6e20 0d0a 0909 0977 6974 6820 7468 6520  n .....with the 
-00055150: 2263 6f6c 6d22 2066 756e 6374 696f 6e2e  "colm" function.
-00055160: 2054 6865 2032 6420 706c 6f74 7320 7265   The 2d plots re
-00055170: 7175 6972 6520 6120 636f 6e74 696e 756f  quire a continuo
-00055180: 7573 2063 6f6c 6f72 206d 6170 2073 6f20  us color map so 
-00055190: 6966 2073 6f6d 6574 6869 6e67 200d 0a09  if something ...
-000551a0: 0909 656c 7365 2069 7320 6769 7665 2032  ..else is give 2
-000551b0: 6420 706c 6f74 7320 6172 6520 7368 6f77  d plots are show
-000551c0: 6e20 6175 746f 6d61 7469 6361 6c6c 7920  n automatically 
-000551d0: 7769 7468 2022 6a65 7422 2e20 466f 7220  with "jet". For 
-000551e0: 616c 6c20 6f66 2074 6865 2031 6420 706c  all of the 1d pl
-000551f0: 6f74 7320 686f 7765 7665 7220 0d0a 0909  ots however ....
-00055200: 0949 2066 6972 7374 2073 656c 6563 7420  .I first select 
-00055210: 6120 6e75 6d62 6572 206f 6620 636f 6c6f  a number of colo
-00055220: 7273 2062 6566 6f72 6520 6561 6368 2070  rs before each p
-00055230: 6c6f 742e 2049 6620 636d 6170 2069 7320  lot. If cmap is 
-00055240: 6120 636f 6e74 696e 6f75 7320 6d61 7020  a continous map 
-00055250: 7468 656e 2074 6865 7365 0d0a 0909 0961  then these.....a
-00055260: 7265 2073 616d 706c 6564 2065 7665 6e6c  re sampled evenl
-00055270: 7920 6f76 6572 2074 6865 2063 6f6c 6f75  y over the colou
-00055280: 726d 6170 2e20 4d61 6e75 616c 2069 7465  rmap. Manual ite
-00055290: 7261 626c 6573 206f 6620 636f 6c6f 7572  rables of colour
-000552a0: 7320 0d0a 0909 0963 6d61 703d 5b28 312c  s .....cmap=[(1,
-000552b0: 302c 3029 2c28 302c 312c 3029 2c28 302c  0,0),(0,1,0),(0,
-000552c0: 302c 3129 2c2e 2e2e 5d20 6172 6520 616c  0,1),...] are al
-000552d0: 736f 2061 6363 6570 7465 642c 2061 7320  so accepted, as 
-000552e0: 6172 6520 7665 6374 6f72 7320 6f72 2064  are vectors or d
-000552f0: 6174 6166 7261 6d65 7320 7468 6174 200d  ataframes that .
-00055300: 0a09 0909 636f 6e74 6169 6e20 6173 2072  ....contain as r
-00055310: 6f77 7320 7468 6520 636f 6c6f 7273 2e20  ows the colors. 
-00055320: 5468 6572 6520 6d75 7374 2062 6520 6f66  There must be of
-00055330: 2063 6f75 7273 6520 7375 6666 6963 6965   course sufficie
-00055340: 6e74 2063 6f6c 6f72 7320 7072 6573 656e  nt colors presen
-00055350: 7420 666f 7220 0d0a 0909 0974 6865 206e  t for .....the n
-00055360: 756d 6265 7273 206f 6620 6c69 6e65 7320  umbers of lines 
-00055370: 7468 6174 2077 696c 6c20 6265 2070 6c6f  that will be plo
-00055380: 7474 6564 2e20 536f 2049 2072 6563 6f6d  tted. So I recom
-00055390: 6d65 6e64 2074 6f20 7072 6f76 6964 6520  mend to provide 
-000553a0: 6174 206c 6561 7374 2031 3020 636f 6c6f  at least 10 colo
-000553b0: 7572 7320 0d0a 0909 0928 652e 672e 796f  urs .....(e.g.yo
-000553c0: 7572 2075 6e69 7665 7273 6974 7920 636f  ur university co
-000553d0: 6c6f 7273 292e 2063 6f6c 6f75 7273 2061  lors). colours a
-000553e0: 7265 2061 6c77 6179 7320 6769 7665 6e20  re always given 
-000553f0: 6173 2061 2c20 6c69 7374 206f 7220 7475  as a, list or tu
-00055400: 706c 6520 7769 7468 2052 4741 206f 7220  ple with RGA or 
-00055410: 5247 4241 0d0a 0909 0928 7769 7468 2074  RGBA.....(with t
-00055420: 6865 206c 6173 7420 4120 6265 6569 6e67  he last A beeing
-00055430: 2074 6865 2041 6c70 6861 3d74 7261 6e73   the Alpha=trans
-00055440: 7061 7265 6e63 792e 2041 6c6c 206e 756d  parency. All num
-00055450: 6265 7273 2061 7265 2062 6574 7765 656e  bers are between
-00055460: 2030 2061 6e64 2031 2e20 0d0a 0909 0949   0 and 1. .....I
-00055470: 6620 6120 6c69 7374 2f76 6563 746f 722f  f a list/vector/
-00055480: 4461 7461 4672 616d 6520 6973 2067 6976  DataFrame is giv
-00055490: 656e 2066 6f72 2074 6865 2063 6f6c 6f75  en for the colou
-000554a0: 7273 2074 6865 7920 7769 6c6c 2062 6520  rs they will be 
-000554b0: 7573 6564 2069 6e20 7468 6520 6f72 6465  used in the orde
-000554c0: 7220 7072 6f76 6964 6564 2e09 090d 0a09  r provided......
-000554d0: 090d 0a09 0970 7269 6e74 5f63 6c69 636b  .....print_click
-000554e0: 5f70 6f73 6974 696f 6e20 3a20 626f 6f6c  _position : bool
-000554f0: 2c20 6f70 7469 6f6e 616c 0d0a 0909 0969  , optional.....i
-00055500: 6620 5472 7565 2074 6865 6e20 7468 6520  f True then the 
-00055510: 636c 6963 6b20 706f 7369 7469 6f6e 2069  click position i
-00055520: 7320 7072 696e 7465 6420 666f 7220 7468  s printed for th
-00055530: 6520 7370 6563 7472 616c 2070 6c6f 7473  e spectral plots
-00055540: 200d 0a09 090d 0a09 0945 7861 6d70 6c65   ........Example
-00055550: 730d 0a09 092d 2d2d 2d2d 2d2d 2d2d 2d2d  s....-----------
-00055560: 2d0d 0a09 090d 0a09 0954 7970 6963 616c  -........Typical
-00055570: 6c79 206f 6e65 2077 6f75 6c64 2063 616c  ly one would cal
-00055580: 6c20 7468 6973 2066 756e 6374 696f 6e20  l this function 
-00055590: 656d 7074 7920 666f 7220 616e 206f 7665  empty for an ove
-000555a0: 7276 6965 773a 0d0a 0909 4166 7465 7220  rview:....After 
-000555b0: 7468 6520 6d69 6e69 6d75 6d20 6669 740d  the minimum fit.
-000555c0: 0a09 090d 0a09 093e 3e3e 2074 613d 7066  .......>>> ta=pf
-000555d0: 2e54 4128 2774 6573 7466 696c 652e 5349  .TA('testfile.SI
-000555e0: 4127 290d 0a09 093e 3e3e 2074 612e 7061  A')....>>> ta.pa
-000555f0: 723d 6c6d 6669 742e 5061 7261 6d65 7465  r=lmfit.Paramete
-00055600: 7273 2829 0d0a 0909 3e3e 3e20 7461 2e70  rs()....>>> ta.p
-00055610: 6172 2e61 6464 2827 6b30 272c 7661 6c75  ar.add('k0',valu
-00055620: 653d 312f 302e 312c 7661 7279 3d54 7275  e=1/0.1,vary=Tru
-00055630: 6529 0d0a 0909 3e3e 3e20 7461 2e46 6974  e)....>>> ta.Fit
-00055640: 5f47 6c6f 6261 6c28 290d 0a09 090d 0a09  _Global().......
-00055650: 094f 6e65 2075 7375 616c 6c79 2070 6c6f  .One usually plo
-00055660: 7473 2074 6865 2061 6e20 6f76 6572 7669  ts the an overvi
-00055670: 6577 0d0a 0909 0d0a 0909 3e3e 3e20 7461  ew........>>> ta
-00055680: 2e50 6c6f 745f 6669 745f 6f75 7470 7574  .Plot_fit_output
-00055690: 2829 0d0a 0909 3e3e 3e20 7461 2e50 6c6f  ()....>>> ta.Plo
-000556a0: 745f 6669 745f 6f75 7470 7574 2870 6c6f  t_fit_output(plo
-000556b0: 7474 696e 673d 7261 6e67 6528 3629 2920  tting=range(6)) 
-000556c0: 2369 7320 7468 6520 7361 6d65 2061 7320  #is the same as 
-000556d0: 6265 666f 7265 0d0a 0909 3e3e 3e20 7461  before....>>> ta
-000556e0: 2e50 6c6f 745f 6669 745f 6f75 7470 7574  .Plot_fit_output
-000556f0: 2832 2920 2377 6f75 6c64 2070 6c6f 7420  (2) #would plot 
-00055700: 6f6e 6c79 2074 6865 206b 696e 6574 6963  only the kinetic
-00055710: 730d 0a09 093e 3e3e 2074 612e 506c 6f74  s....>>> ta.Plot
-00055720: 5f66 6974 5f6f 7574 7075 7428 706c 6f74  _fit_output(plot
-00055730: 7469 6e67 203d 2032 2920 2377 6f75 6c64  ting = 2) #would
-00055740: 2070 6c6f 7420 6f6e 6c79 2074 6865 206b   plot only the k
-00055750: 696e 6574 6963 730d 0a09 0909 090d 0a0d  inetics.........
-00055760: 0a09 0927 2727 0d0a 0909 7472 793a 0d0a  ...'''....try:..
-00055770: 0909 0972 653d 7365 6c66 2e72 650d 0a09  ...re=self.re...
-00055780: 0965 7863 6570 743a 0d0a 0909 0970 7269  .except:.....pri
-00055790: 6e74 2827 5765 206e 6565 6420 746f 2068  nt('We need to h
-000557a0: 6176 6520 6669 7474 6564 2073 6f6d 6574  ave fitted somet
-000557b0: 6869 6e67 2073 6f20 7468 6174 2077 6520  hing so that we 
-000557c0: 6361 6e20 706c 6f74 2729 0d0a 0909 0972  can plot').....r
-000557d0: 6574 7572 6e20 4661 6c73 650d 0a09 0970  eturn False....p
-000557e0: 6174 683d 6368 6563 6b5f 666f 6c64 6572  ath=check_folder
-000557f0: 2870 6174 683d 7061 7468 2c63 7572 7265  (path=path,curre
-00055800: 6e74 5f70 6174 683d 7365 6c66 2e70 6174  nt_path=self.pat
-00055810: 6829 0d0a 0909 6966 2073 656c 662e 7361  h)....if self.sa
-00055820: 7665 5f66 6967 7572 6573 5f74 6f5f 666f  ve_figures_to_fo
-00055830: 6c64 6572 3a0d 0a09 0909 7365 6c66 2e66  lder:.....self.f
-00055840: 6967 7572 655f 7061 7468 3d70 6174 680d  igure_path=path.
-00055850: 0a09 0969 6620 636d 6170 2069 7320 4e6f  ...if cmap is No
-00055860: 6e65 3a63 6d61 703d 7365 6c66 2e63 6d61  ne:cmap=self.cma
-00055870: 700d 0a09 0969 6620 6669 6c65 6e61 6d65  p....if filename
-00055880: 2069 7320 4e6f 6e65 3a66 696c 656e 616d   is None:filenam
-00055890: 653d 7365 6c66 2e66 696c 656e 616d 650d  e=self.filename.
-000558a0: 0a09 0969 6620 7469 746c 6520 6973 204e  ...if title is N
-000558b0: 6f6e 653a 0d0a 0909 0969 6620 6669 6c65  one:.....if file
-000558c0: 6e61 6d65 2069 7320 4e6f 6e65 3a0d 0a09  name is None:...
-000558d0: 0909 0974 6974 6c65 3d73 656c 662e 6669  ...title=self.fi
-000558e0: 6c65 6e61 6d65 0d0a 0909 0965 6c73 653a  lename.....else:
-000558f0: 0d0a 0909 0909 7469 746c 653d 6669 6c65  ......title=file
-00055900: 6e61 6d65 0d0a 0909 6966 206e 6f74 2068  name....if not h
-00055910: 6173 6174 7472 2870 6c6f 7474 696e 672c  asattr(plotting,
-00055920: 225f 5f69 7465 725f 5f22 293a 706c 6f74  "__iter__"):plot
-00055930: 7469 6e67 3d5b 706c 6f74 7469 6e67 5d0d  ting=[plotting].
-00055940: 0a09 0970 6c6f 745f 6669 745f 6f75 7470  ...plot_fit_outp
-00055950: 7574 2873 656c 662e 7265 2c20 7365 6c66  ut(self.re, self
-00055960: 2e64 732c 2063 6d61 7020 3d20 7365 6c66  .ds, cmap = self
-00055970: 2e63 6d61 702c 2070 6c6f 7474 696e 6720  .cmap, plotting 
-00055980: 3d20 706c 6f74 7469 6e67 2c20 7469 746c  = plotting, titl
-00055990: 6520 3d20 7469 746c 652c 200d 0a09 0909  e = title, .....
-000559a0: 0909 0970 6174 6820 3d20 7061 7468 2c20  ...path = path, 
-000559b0: 6620 3d20 6669 6c65 6e61 6d65 2c20 696e  f = filename, in
-000559c0: 7465 6e73 6974 795f 7261 6e67 6520 3d20  tensity_range = 
-000559d0: 7365 6c66 2e69 6e74 656e 7369 7479 5f72  self.intensity_r
-000559e0: 616e 6765 2c20 0d0a 0909 0909 0909 6c6f  ange, ........lo
-000559f0: 675f 7363 616c 6520 3d20 7365 6c66 2e6c  g_scale = self.l
-00055a00: 6f67 5f73 6361 6c65 2c20 6261 7365 756e  og_scale, baseun
-00055a10: 6974 203d 2073 656c 662e 6261 7365 756e  it = self.baseun
-00055a20: 6974 2c20 7469 6d65 6c69 6d69 7473 203d  it, timelimits =
-00055a30: 2073 656c 662e 7469 6d65 6c69 6d69 7473   self.timelimits
-00055a40: 2c20 0d0a 0909 0909 0909 7363 6174 7465  , ........scatte
-00055a50: 7263 7574 203d 2073 656c 662e 7363 6174  rcut = self.scat
-00055a60: 7465 7263 7574 2c20 626f 7264 6572 6375  tercut, bordercu
-00055a70: 7420 3d20 7365 6c66 2e62 6f72 6465 7263  t = self.borderc
-00055a80: 7574 2c20 0d0a 0909 0909 0909 6572 726f  ut, ........erro
-00055a90: 725f 6d61 7472 6978 5f61 6d70 6c69 6669  r_matrix_amplifi
-00055aa0: 6361 7469 6f6e 203d 2073 656c 662e 6572  cation = self.er
-00055ab0: 726f 725f 6d61 7472 6978 5f61 6d70 6c69  ror_matrix_ampli
-00055ac0: 6669 6361 7469 6f6e 2c20 0d0a 0909 0909  fication, ......
-00055ad0: 0909 7761 7665 5f6e 6d5f 6269 6e20 3d20  ..wave_nm_bin = 
-00055ae0: 7365 6c66 2e77 6176 655f 6e6d 5f62 696e  self.wave_nm_bin
-00055af0: 2c20 7265 6c5f 7761 7665 203d 2073 656c  , rel_wave = sel
-00055b00: 662e 7265 6c5f 7761 7665 2c20 7769 6474  f.rel_wave, widt
-00055b10: 6820 3d20 7365 6c66 2e77 6176 656c 656e  h = self.wavelen
-00055b20: 6774 685f 6269 6e2c 200d 0a09 0909 0909  gth_bin, .......
-00055b30: 0972 656c 5f74 696d 6520 3d20 7365 6c66  .rel_time = self
-00055b40: 2e72 656c 5f74 696d 652c 2073 6176 655f  .rel_time, save_
-00055b50: 6669 6775 7265 735f 746f 5f66 6f6c 6465  figures_to_folde
-00055b60: 7220 3d20 7365 6c66 2e73 6176 655f 6669  r = self.save_fi
-00055b70: 6775 7265 735f 746f 5f66 6f6c 6465 722c  gures_to_folder,
-00055b80: 200d 0a09 0909 0909 096c 6f67 5f66 6974   ........log_fit
-00055b90: 203d 2073 656c 662e 6c6f 675f 6669 742c   = self.log_fit,
-00055ba0: 6d6f 6420 3d20 7365 6c66 2e6d 6f64 2c20  mod = self.mod, 
-00055bb0: 7361 7665 7479 7065 203d 2073 6176 6574  savetype = savet
-00055bc0: 7970 652c 200d 0a09 0909 0909 0974 696d  ype, ........tim
-00055bd0: 655f 7769 6474 685f 7065 7263 656e 7420  e_width_percent 
-00055be0: 3d20 7365 6c66 2e74 696d 655f 7769 6474  = self.time_widt
-00055bf0: 685f 7065 7263 656e 742c 2065 7661 6c75  h_percent, evalu
-00055c00: 6174 696f 6e5f 7374 796c 6520 3d20 6576  ation_style = ev
-00055c10: 616c 7561 7469 6f6e 5f73 7479 6c65 2c20  aluation_style, 
-00055c20: 0d0a 0909 0909 0909 6669 6c65 6e61 6d65  ........filename
-00055c30: 203d 2073 656c 662e 6669 6c65 6e61 6d65   = self.filename
-00055c40: 2c20 7363 616c 655f 7479 7065 203d 2073  , scale_type = s
-00055c50: 6361 6c65 5f74 7970 652c 2070 6174 6368  cale_type, patch
-00055c60: 6573 203d 2070 6174 6368 6573 2c20 6c69  es = patches, li
-00055c70: 6e74 7265 7368 203d 2073 656c 662e 6c69  ntresh = self.li
-00055c80: 6e74 7265 7368 2c0d 0a09 0909 0909 0970  ntresh,........p
-00055c90: 7269 6e74 5f63 6c69 636b 5f70 6f73 6974  rint_click_posit
-00055ca0: 696f 6e20 3d20 7072 696e 745f 636c 6963  ion = print_clic
-00055cb0: 6b5f 706f 7369 7469 6f6e 2c20 6967 6e6f  k_position, igno
-00055cc0: 7265 5f74 696d 655f 7265 6769 6f6e 203d  re_time_region =
-00055cd0: 2073 656c 662e 6967 6e6f 7265 5f74 696d   self.ignore_tim
-00055ce0: 655f 7265 6769 6f6e 2c0d 0a09 0909 0909  e_region,.......
-00055cf0: 0964 6174 615f 7479 7065 203d 2073 656c  .data_type = sel
-00055d00: 662e 6461 7461 5f74 7970 652c 2070 6c6f  f.data_type, plo
-00055d10: 745f 7365 636f 6e64 5f61 735f 656e 6572  t_second_as_ener
-00055d20: 6779 203d 2070 6c6f 745f 7365 636f 6e64  gy = plot_second
-00055d30: 5f61 735f 656e 6572 6779 2c20 756e 6974  _as_energy, unit
-00055d40: 733d 2073 656c 662e 756e 6974 732c 200d  s= self.units, .
-00055d50: 0a09 0909 0909 0965 7175 616c 5f65 6e65  .......equal_ene
-00055d60: 7267 795f 6269 6e20 3d20 7365 6c66 2e65  rgy_bin = self.e
-00055d70: 7175 616c 5f65 6e65 7267 795f 6269 6e29  qual_energy_bin)
-00055d80: 0d0a 0d0a 0d0a 0d0a 0964 6566 2053 6176  .........def Sav
-00055d90: 655f 6461 7461 2873 656c 662c 2073 6176  e_data(self, sav
-00055da0: 655f 5241 5720 3d20 5472 7565 2c20 7361  e_RAW = True, sa
-00055db0: 7665 5f46 6974 203d 2054 7275 652c 2073  ve_Fit = True, s
-00055dc0: 6176 655f 736c 6963 6573 203d 2054 7275  ave_slices = Tru
-00055dd0: 652c 2073 6176 655f 6269 6e6e 6564 203d  e, save_binned =
-00055de0: 2046 616c 7365 2c20 0d0a 0909 0909 0966   False, .......f
-00055df0: 696c 656e 616d 6520 3d20 4e6f 6e65 2c20  ilename = None, 
-00055e00: 7361 7665 5f66 6974 5f72 6573 756c 7473  save_fit_results
-00055e10: 203d 2054 7275 652c 2070 6174 6820 3d20   = True, path = 
-00055e20: 2744 6174 615f 6578 706f 7274 272c 2073  'Data_export', s
-00055e30: 6570 203d 2073 7472 2827 5c74 2729 293a  ep = str('\t')):
-00055e40: 0d0a 0909 2727 2768 616e 6479 2066 756e  ....'''handy fun
-00055e50: 6374 696f 6e20 746f 2073 6176 6520 7468  ction to save th
-00055e60: 6520 6461 7461 206f 6e20 6469 736b 2061  e data on disk a
-00055e70: 7320 6461 7420 6669 6c65 732e 0d0a 0909  s dat files.....
-00055e80: 5468 6520 5241 5720 6c61 6265 6c65 6420  The RAW labeled 
-00055e90: 6669 6c65 7320 636f 6e74 6169 6e20 7468  files contain th
-00055ea0: 6520 6368 6972 7020 636f 7272 6563 7465  e chirp correcte
-00055eb0: 6420 7661 6c75 6573 2028 7365 6c66 2e64  d values (self.d
-00055ec0: 7329 0d0a 0909 0d0a 0909 7468 6520 7361  s)........the sa
-00055ed0: 7665 5f73 6c69 6365 7320 7377 6974 6368  ve_slices switch
-00055ee0: 2074 7572 6e73 206f 6e20 7468 6520 6475   turns on the du
-00055ef0: 6d70 206f 6620 7468 6520 7365 7061 7261  mp of the separa
-00055f00: 7465 2073 6c69 6365 6420 6669 6775 7265  te sliced figure
-00055f10: 7320 2874 696d 6520 616e 6420 7370 6563  s (time and spec
-00055f20: 7472 616c 2920 0d0a 0d0a 0909 0d0a 0909  tral) ..........
-00055f30: 5061 7261 6d65 7465 7273 0d0a 0909 2d2d  Parameters....--
-00055f40: 2d2d 2d2d 2d2d 2d2d 0d0a 0909 0d0a 0909  --------........
-00055f50: 7361 7665 5f62 696e 6e65 6420 3a20 626f  save_binned : bo
-00055f60: 6f6c 2c20 6f70 7469 6f6e 616c 0d0a 0909  ol, optional....
-00055f70: 0969 7320 616c 736f 2074 6865 2072 652d  .is also the re-
-00055f80: 6269 6e6e 6564 206d 6174 7269 7820 746f  binned matrix to
-00055f90: 2062 6520 7361 7665 642e 0d0a 0909 090d   be saved.......
-00055fa0: 0a09 0973 6176 655f 736c 6963 6573 203a  ...save_slices :
-00055fb0: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0d   bool, optional.
-00055fc0: 0a09 0909 7361 7665 2074 6865 206b 696e  ....save the kin
-00055fd0: 6574 6963 7320 616e 6420 7370 6563 7472  etics and spectr
-00055fe0: 6120 6672 6f6d 2074 6865 2066 6974 7465  a from the fitte
-00055ff0: 6420 6461 7461 2028 7769 7468 2074 6865  d data (with the
-00056000: 2066 6974 7329 0d0a 0909 090d 0a09 0973   fits).........s
-00056010: 6570 203a 2073 7472 2c20 6f70 7469 6f6e  ep : str, option
-00056020: 616c 0d0a 0909 0977 6861 7420 7379 6d62  al.....what symb
-00056030: 6f6c 2069 7320 7573 6564 2074 6f20 7365  ol is used to se
-00056040: 7061 7261 7465 2064 6966 6665 7265 6e74  parate different
-00056050: 206e 756d 6265 722e 2028 7479 7069 6361   number. (typica
-00056060: 6c20 6569 7468 6572 2027 7461 6227 206f  l either 'tab' o
-00056070: 7220 636f 6d6d 610d 0a09 090d 0a09 0973  r comma........s
-00056080: 6176 655f 5241 5720 3a20 626f 6f6c 2c20  ave_RAW : bool, 
-00056090: 6f70 7469 6f6e 616c 0d0a 0909 0928 4465  optional.....(De
-000560a0: 6661 756c 7429 2054 7275 6520 7468 656e  fault) True then
-000560b0: 2074 6865 2066 6972 7374 2073 6c69 6465   the first slide
-000560c0: 2077 6974 6820 7468 6520 5241 5720 6461   with the RAW da
-000560d0: 7461 2069 7320 6372 6561 7465 6420 0d0a  ta is created ..
-000560e0: 0909 0d0a 0909 7361 7665 5f46 6974 203a  ......save_Fit :
-000560f0: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0d   bool, optional.
-00056100: 0a09 0909 2844 6566 6175 6c74 2920 5472  ....(Default) Tr
-00056110: 7565 2074 6865 6e20 7468 6520 7365 636f  ue then the seco
-00056120: 6e64 2073 6c69 6465 2077 6974 6820 7468  nd slide with th
-00056130: 6520 4669 7474 6564 2064 6174 6120 6973  e Fitted data is
-00056140: 2063 7265 6174 6564 200d 0a09 090d 0a09   created .......
-00056150: 0970 6174 6820 3a20 4e6f 6e65 2c20 7374  .path : None, st
-00056160: 7220 6f72 2070 6174 682c 206f 7074 696f  r or path, optio
-00056170: 6e61 6c0d 0a09 0909 2844 6566 6175 6c74  nal.....(Default
-00056180: 2920 4e6f 6e65 2c20 6966 206c 6566 7420  ) None, if left 
-00056190: 6f6e 204e 6f6e 652c 2074 6865 6e20 6120  on None, then a 
-000561a0: 666f 6c64 6572 2022 7265 7375 6c74 5f66  folder "result_f
-000561b0: 6967 7572 6573 2220 6973 2063 7265 6174  igures" is creat
-000561c0: 6564 2069 6e20 7468 6520 666f 6c64 6572  ed in the folder
-000561d0: 200d 0a09 0909 6f66 2074 6865 2064 6174   .....of the dat
-000561e0: 6120 2873 656c 662e 7061 7468 290d 0a09  a (self.path)...
-000561f0: 0909 0d0a 0909 7361 7665 5f66 6974 5f72  ......save_fit_r
-00056200: 6573 756c 7473 203a 2062 6f6f 6c2c 206f  esults : bool, o
-00056210: 7074 696f 6e61 6c0d 0a09 0909 6966 2054  ptional.....if T
-00056220: 7275 6520 2844 6566 6175 6c74 2920 2061  rue (Default)  a
-00056230: 206e 6561 746c 7920 666f 726d 6174 6564   neatly formated
-00056240: 2066 696c 6520 7769 7468 2074 6865 2066   file with the f
-00056250: 6974 2072 6573 756c 7473 2069 7320 6372  it results is cr
-00056260: 6561 7465 6420 616e 6420 7374 6f72 6564  eated and stored
-00056270: 2077 6974 6820 7468 6520 6461 7461 0d0a   with the data..
-00056280: 0909 090d 0a09 0966 696c 656e 616d 6520  .......filename 
-00056290: 3a20 7374 722c 206f 7074 696f 6e61 6c0d  : str, optional.
-000562a0: 0a09 0909 2844 6566 6175 6c74 2920 4e6f  ....(Default) No
-000562b0: 6e65 2c20 4261 7365 206e 616d 6520 666f  ne, Base name fo
-000562c0: 7220 616c 6c20 706c 6f74 732e 2049 6620  r all plots. If 
-000562d0: 4e6f 6e65 2c20 7468 656e 2073 656c 662e  None, then self.
-000562e0: 6669 6c65 6e61 6d65 2077 696c 6c20 6265  filename will be
-000562f0: 2075 7365 640d 0a09 0909 0d0a 0909 4578   used.........Ex
-00056300: 616d 706c 6573 0d0a 0909 2d2d 2d2d 2d2d  amples....------
-00056310: 2d2d 2d0d 0a09 093e 3e3e 2074 612e 5361  ---....>>> ta.Sa
-00056320: 7665 5f44 6174 610d 0a09 090d 0a09 0927  ve_Data........'
-00056330: 2727 0d0a 0909 0d0a 0909 6966 2066 696c  ''........if fil
-00056340: 656e 616d 6520 6973 204e 6f6e 653a 6669  ename is None:fi
-00056350: 6c65 6e61 6d65 203d 2073 656c 662e 6669  lename = self.fi
-00056360: 6c65 6e61 6d65 2e73 706c 6974 2827 2e27  lename.split('.'
-00056370: 295b 305d 0d0a 0909 6966 2073 6176 655f  )[0]....if save_
-00056380: 5241 573a 0d0a 0909 0973 656c 662e 6473  RAW:.....self.ds
-00056390: 2e74 6f5f 6373 7628 6368 6563 6b5f 666f  .to_csv(check_fo
-000563a0: 6c64 6572 2870 6174 6820 3d20 7061 7468  lder(path = path
-000563b0: 2c20 6375 7272 656e 745f 7061 7468 203d  , current_path =
-000563c0: 2073 656c 662e 7061 7468 2c20 0d0a 0909   self.path, ....
-000563d0: 0909 0909 0966 696c 656e 616d 6520 3d20  .....filename = 
-000563e0: 6669 6c65 6e61 6d65 2b27 5f63 6869 7270  filename+'_chirp
-000563f0: 5f63 6f72 7265 6374 6564 5f72 6177 5f6d  _corrected_raw_m
-00056400: 6174 7269 782e 6461 7427 292c 2073 6570  atrix.dat'), sep
-00056410: 203d 2073 6570 290d 0a09 0909 6966 2073   = sep).....if s
-00056420: 6176 655f 6269 6e6e 6564 3a0d 0a09 0909  ave_binned:.....
-00056430: 0973 7562 203d 2073 7562 5f64 7328 7365  .sub = sub_ds(se
-00056440: 6c66 2e64 732c 2073 6361 7474 6572 6375  lf.ds, scattercu
-00056450: 7420 3d20 7365 6c66 2e73 6361 7474 6572  t = self.scatter
-00056460: 6375 742c 2062 6f72 6465 7263 7574 203d  cut, bordercut =
-00056470: 2073 656c 662e 626f 7264 6572 6375 742c   self.bordercut,
-00056480: 200d 0a09 0909 0909 0909 7469 6d65 6c69   .........timeli
-00056490: 6d69 7473 203d 2073 656c 662e 7469 6d65  mits = self.time
-000564a0: 6c69 6d69 7473 2c20 7761 7665 5f6e 6d5f  limits, wave_nm_
-000564b0: 6269 6e20 3d20 7365 6c66 2e77 6176 655f  bin = self.wave_
-000564c0: 6e6d 5f62 696e 2c20 0d0a 0909 0909 0909  nm_bin, ........
-000564d0: 0974 696d 655f 6269 6e20 3d20 7365 6c66  .time_bin = self
-000564e0: 2e74 696d 655f 6269 6e29 0d0a 0909 0909  .time_bin)......
-000564f0: 7375 622e 746f 5f63 7376 2863 6865 636b  sub.to_csv(check
-00056500: 5f66 6f6c 6465 7228 7061 7468 203d 2070  _folder(path = p
-00056510: 6174 682c 2063 7572 7265 6e74 5f70 6174  ath, current_pat
-00056520: 6820 3d20 7365 6c66 2e70 6174 682c 200d  h = self.path, .
-00056530: 0a09 0909 0909 0909 0909 0966 696c 656e  ...........filen
-00056540: 616d 6520 3d20 6669 6c65 6e61 6d65 2b27  ame = filename+'
-00056550: 5f63 6869 7270 5f63 6f72 7265 6374 6564  _chirp_corrected
-00056560: 5f72 6562 696e 6e65 645f 6d61 7472 6978  _rebinned_matrix
-00056570: 2e64 6174 2729 2c20 7365 7020 3d20 7365  .dat'), sep = se
-00056580: 7029 0d0a 0909 0969 6620 7361 7665 5f73  p).....if save_s
-00056590: 6c69 6365 733a 0d0a 0909 0909 7375 6220  lices:......sub 
-000565a0: 3d20 7375 625f 6473 2864 7320 3d20 7365  = sub_ds(ds = se
-000565b0: 6c66 2e64 732e 636f 7079 2829 2c20 7761  lf.ds.copy(), wa
-000565c0: 7665 6c65 6e67 7468 5f62 696e 203d 2073  velength_bin = s
-000565d0: 656c 662e 7761 7665 6c65 6e67 7468 5f62  elf.wavelength_b
-000565e0: 696e 2c20 7761 7665 6c65 6e67 7468 203d  in, wavelength =
-000565f0: 2073 656c 662e 7265 6c5f 7761 7665 290d   self.rel_wave).
-00056600: 0a09 0909 0923 7375 622e 636f 6c75 6d6e  .....#sub.column
-00056610: 732e 6e61 6d65 203d 2027 7761 7665 6c65  s.name = 'wavele
-00056620: 6e67 7468 205b 6e6d 5d20 696e 2025 2e30  ngth [nm] in %.0
-00056630: 6620 6269 6e73 2725 7365 6c66 2e77 6176  f bins'%self.wav
-00056640: 656c 656e 6774 685f 6269 6e0d 0a09 0909  elength_bin.....
-00056650: 0973 7562 2e74 6f5f 6373 7628 6368 6563  .sub.to_csv(chec
-00056660: 6b5f 666f 6c64 6572 2870 6174 6820 3d20  k_folder(path = 
-00056670: 7061 7468 2c20 6375 7272 656e 745f 7061  path, current_pa
-00056680: 7468 203d 2073 656c 662e 7061 7468 2c20  th = self.path, 
-00056690: 0d0a 0909 0909 0909 0966 696c 656e 616d  .........filenam
-000566a0: 6520 3d20 6669 6c65 6e61 6d65 2b27 5f63  e = filename+'_c
-000566b0: 6869 7270 5f63 6f72 7265 6374 6564 5f52  hirp_corrected_R
-000566c0: 4157 5f6b 696e 6574 6963 732e 6461 7427  AW_kinetics.dat'
-000566d0: 292c 2073 6570 203d 2073 6570 290d 0a09  ), sep = sep)...
-000566e0: 0909 0973 7562 203d 2073 7562 5f64 7328  ...sub = sub_ds(
-000566f0: 6473 203d 2073 656c 662e 6473 2e63 6f70  ds = self.ds.cop
-00056700: 7928 292c 2074 696d 6573 203d 2073 656c  y(), times = sel
-00056710: 662e 7265 6c5f 7469 6d65 2c20 7469 6d65  f.rel_time, time
-00056720: 5f77 6964 7468 5f70 6572 6365 6e74 203d  _width_percent =
-00056730: 2073 656c 662e 7469 6d65 5f77 6964 7468   self.time_width
-00056740: 5f70 6572 6365 6e74 2c20 0d0a 0909 0909  _percent, ......
-00056750: 0909 0909 7363 6174 7465 7263 7574 203d  ....scattercut =
-00056760: 2073 656c 662e 7363 6174 7465 7263 7574   self.scattercut
-00056770: 2c20 626f 7264 6572 6375 7420 3d20 7365  , bordercut = se
-00056780: 6c66 2e62 6f72 6465 7263 7574 2c20 7761  lf.bordercut, wa
-00056790: 7665 5f6e 6d5f 6269 6e20 3d20 7365 6c66  ve_nm_bin = self
-000567a0: 2e77 6176 655f 6e6d 5f62 696e 290d 0a09  .wave_nm_bin)...
-000567b0: 0909 0973 7562 2e74 6f5f 6373 7628 6368  ...sub.to_csv(ch
-000567c0: 6563 6b5f 666f 6c64 6572 2870 6174 6820  eck_folder(path 
-000567d0: 3d20 7061 7468 2c20 6375 7272 656e 745f  = path, current_
-000567e0: 7061 7468 203d 2073 656c 662e 7061 7468  path = self.path
-000567f0: 2c20 0d0a 0909 0909 0909 0966 696c 656e  , .........filen
-00056800: 616d 6520 3d20 6669 6c65 6e61 6d65 2b27  ame = filename+'
-00056810: 5f63 6869 7270 5f63 6f72 7265 6374 6564  _chirp_corrected
-00056820: 5f52 4157 5f53 7065 6374 7261 2e64 6174  _RAW_Spectra.dat
-00056830: 2729 2c20 7365 7020 3d20 7365 7029 0d0a  '), sep = sep)..
-00056840: 0909 6966 2073 6176 655f 4669 743a 0d0a  ..if save_Fit:..
-00056850: 0909 0974 7279 3a0d 0a09 0909 0973 656c  ...try:......sel
-00056860: 662e 7265 2e6b 6579 7328 290d 0a09 0909  f.re.keys().....
-00056870: 6578 6365 7074 3a0d 0a09 0909 0970 7269  except:......pri
-00056880: 6e74 2827 6e6f 2066 6974 2069 6e20 6461  nt('no fit in da
-00056890: 7461 2729 0d0a 0909 0909 7361 7665 5f46  ta')......save_F
-000568a0: 6974 203d 2046 616c 7365 0d0a 0909 6966  it = False....if
-000568b0: 2073 6176 655f 4669 743a 0d0a 0909 0973   save_Fit:.....s
-000568c0: 656c 662e 7265 5b27 4127 5d2e 746f 5f63  elf.re['A'].to_c
-000568d0: 7376 2863 6865 636b 5f66 6f6c 6465 7228  sv(check_folder(
-000568e0: 7061 7468 203d 2070 6174 682c 2063 7572  path = path, cur
-000568f0: 7265 6e74 5f70 6174 6820 3d20 7365 6c66  rent_path = self
-00056900: 2e70 6174 682c 200d 0a09 0909 0909 0909  .path, .........
-00056910: 0966 696c 656e 616d 6520 3d20 6669 6c65  .filename = file
-00056920: 6e61 6d65 2b27 5f6d 6174 7269 7820 7573  name+'_matrix us
-00056930: 6564 2061 7320 6669 7420 696e 7075 742e  ed as fit input.
-00056940: 6461 7427 292c 2073 6570 203d 2073 6570  dat'), sep = sep
-00056950: 290d 0a09 0909 7365 6c66 2e72 655b 2741  ).....self.re['A
-00056960: 4327 5d2e 746f 5f63 7376 2863 6865 636b  C'].to_csv(check
-00056970: 5f66 6f6c 6465 7228 7061 7468 203d 2070  _folder(path = p
-00056980: 6174 682c 2063 7572 7265 6e74 5f70 6174  ath, current_pat
-00056990: 6820 3d20 7365 6c66 2e70 6174 682c 200d  h = self.path, .
-000569a0: 0a09 0909 0909 0909 0966 696c 656e 616d  .........filenam
-000569b0: 6520 3d20 6669 6c65 6e61 6d65 2b27 5f6d  e = filename+'_m
-000569c0: 6174 7269 7820 6361 6c63 756c 6174 6564  atrix calculated
-000569d0: 2064 7572 696e 6720 6669 742e 6461 7427   during fit.dat'
-000569e0: 292c 2073 6570 203d 2073 6570 290d 0a09  ), sep = sep)...
-000569f0: 0909 7365 6c66 2e72 655b 2741 4527 5d2e  ..self.re['AE'].
-00056a00: 746f 5f63 7376 2863 6865 636b 5f66 6f6c  to_csv(check_fol
-00056a10: 6465 7228 7061 7468 203d 2070 6174 682c  der(path = path,
-00056a20: 2063 7572 7265 6e74 5f70 6174 6820 3d20   current_path = 
-00056a30: 7365 6c66 2e70 6174 682c 200d 0a09 0909  self.path, .....
-00056a40: 0909 0909 0966 696c 656e 616d 6520 3d20  .....filename = 
-00056a50: 6669 6c65 6e61 6d65 2b27 5f65 7272 6f72  filename+'_error
-00056a60: 5f6d 6174 7269 7820 6361 6c63 756c 6174  _matrix calculat
-00056a70: 6564 2064 7572 696e 6720 6669 742e 6461  ed during fit.da
-00056a80: 7427 292c 2073 6570 203d 2073 6570 290d  t'), sep = sep).
-00056a90: 0a09 0909 6966 2073 6176 655f 736c 6963  ....if save_slic
-00056aa0: 6573 3a09 0d0a 0909 0909 7375 6220 3d20  es:.......sub = 
-00056ab0: 7375 625f 6473 2864 7320 3d20 7365 6c66  sub_ds(ds = self
-00056ac0: 2e72 655b 2741 4327 5d2e 636f 7079 2829  .re['AC'].copy()
-00056ad0: 2c20 7761 7665 6c65 6e67 7468 5f62 696e  , wavelength_bin
-00056ae0: 203d 2073 656c 662e 7761 7665 6c65 6e67   = self.waveleng
-00056af0: 7468 5f62 696e 2c20 7761 7665 6c65 6e67  th_bin, waveleng
-00056b00: 7468 203d 2073 656c 662e 7265 6c5f 7761  th = self.rel_wa
-00056b10: 7665 290d 0a09 0909 0923 7375 622e 636f  ve)......#sub.co
-00056b20: 6c75 6d6e 732e 6e61 6d65 203d 2027 7761  lumns.name = 'wa
-00056b30: 7665 6c65 6e74 6820 5b6e 6d5d 2069 6e20  velenth [nm] in 
-00056b40: 252e 3066 2062 696e 7327 2573 656c 662e  %.0f bins'%self.
-00056b50: 7761 7665 6c65 6e67 7468 5f62 696e 0d0a  wavelength_bin..
-00056b60: 0909 0909 7375 622e 746f 5f63 7376 2863  ....sub.to_csv(c
-00056b70: 6865 636b 5f66 6f6c 6465 7228 7061 7468  heck_folder(path
-00056b80: 203d 2070 6174 682c 2063 7572 7265 6e74   = path, current
-00056b90: 5f70 6174 6820 3d20 7365 6c66 2e70 6174  _path = self.pat
-00056ba0: 682c 200d 0a09 0909 0909 0909 6669 6c65  h, .........file
-00056bb0: 6e61 6d65 203d 2066 696c 656e 616d 652b  name = filename+
-00056bc0: 275f 6669 7474 6564 5f6b 696e 6574 6963  '_fitted_kinetic
-00056bd0: 732e 6461 7427 292c 2073 6570 203d 2073  s.dat'), sep = s
-00056be0: 6570 290d 0a09 0909 0973 7562 203d 2073  ep)......sub = s
-00056bf0: 7562 5f64 7328 6473 203d 2073 656c 662e  ub_ds(ds = self.
-00056c00: 7265 5b27 4127 5d2e 636f 7079 2829 2c20  re['A'].copy(), 
-00056c10: 7761 7665 6c65 6e67 7468 5f62 696e 203d  wavelength_bin =
-00056c20: 2073 656c 662e 7761 7665 6c65 6e67 7468   self.wavelength
-00056c30: 5f62 696e 2c20 7761 7665 6c65 6e67 7468  _bin, wavelength
-00056c40: 203d 2073 656c 662e 7265 6c5f 7761 7665   = self.rel_wave
-00056c50: 290d 0a09 0909 0923 7375 622e 636f 6c75  )......#sub.colu
-00056c60: 6d6e 732e 6e61 6d65 203d 2027 7761 7665  mns.name = 'wave
-00056c70: 6c65 6e74 6820 5b6e 6d5d 2069 6e20 252e  lenth [nm] in %.
-00056c80: 3066 2062 696e 7327 2573 656c 662e 7761  0f bins'%self.wa
-00056c90: 7665 6c65 6e67 7468 5f62 696e 0d0a 0909  velength_bin....
-00056ca0: 0909 7375 622e 746f 5f63 7376 2863 6865  ..sub.to_csv(che
-00056cb0: 636b 5f66 6f6c 6465 7228 7061 7468 203d  ck_folder(path =
-00056cc0: 2070 6174 682c 2063 7572 7265 6e74 5f70   path, current_p
-00056cd0: 6174 6820 3d20 7365 6c66 2e70 6174 682c  ath = self.path,
-00056ce0: 200d 0a09 0909 0909 0909 6669 6c65 6e61   .........filena
-00056cf0: 6d65 203d 2066 696c 656e 616d 652b 275f  me = filename+'_
-00056d00: 6d65 6173 7572 6564 5f6b 696e 6574 6963  measured_kinetic
-00056d10: 732e 6461 7427 292c 2073 6570 203d 2073  s.dat'), sep = s
-00056d20: 6570 290d 0a09 0909 0973 7562 203d 2073  ep)......sub = s
-00056d30: 7562 5f64 7328 6473 203d 2073 656c 662e  ub_ds(ds = self.
-00056d40: 7265 5b27 4143 275d 2e63 6f70 7928 292c  re['AC'].copy(),
-00056d50: 2074 696d 6573 203d 2073 656c 662e 7265   times = self.re
-00056d60: 6c5f 7469 6d65 2c20 0d0a 0909 0909 0909  l_time, ........
-00056d70: 0974 696d 655f 7769 6474 685f 7065 7263  .time_width_perc
-00056d80: 656e 7420 3d20 7365 6c66 2e74 696d 655f  ent = self.time_
-00056d90: 7769 6474 685f 7065 7263 656e 742c 2073  width_percent, s
-00056da0: 6361 7474 6572 6375 7420 3d20 7365 6c66  cattercut = self
-00056db0: 2e73 6361 7474 6572 6375 742c 200d 0a09  .scattercut, ...
-00056dc0: 0909 0909 0909 626f 7264 6572 6375 7420  ......bordercut 
-00056dd0: 3d20 7365 6c66 2e62 6f72 6465 7263 7574  = self.bordercut
-00056de0: 2c20 7761 7665 5f6e 6d5f 6269 6e20 3d20  , wave_nm_bin = 
-00056df0: 7365 6c66 2e77 6176 655f 6e6d 5f62 696e  self.wave_nm_bin
-00056e00: 290d 0a09 0909 0973 7562 2e74 6f5f 6373  )......sub.to_cs
-00056e10: 7628 6368 6563 6b5f 666f 6c64 6572 2870  v(check_folder(p
-00056e20: 6174 6820 3d20 7061 7468 2c20 6375 7272  ath = path, curr
-00056e30: 656e 745f 7061 7468 203d 2073 656c 662e  ent_path = self.
-00056e40: 7061 7468 2c20 0d0a 0909 0909 0909 0966  path, .........f
-00056e50: 696c 656e 616d 6520 3d20 6669 6c65 6e61  ilename = filena
-00056e60: 6d65 2b27 5f66 6974 7465 645f 7370 6563  me+'_fitted_spec
-00056e70: 7472 612e 6461 7427 292c 2073 6570 203d  tra.dat'), sep =
-00056e80: 2073 6570 290d 0a09 0909 0973 7562 203d   sep)......sub =
-00056e90: 2073 7562 5f64 7328 6473 203d 2073 656c   sub_ds(ds = sel
-00056ea0: 662e 7265 5b27 4127 5d2e 636f 7079 2829  f.re['A'].copy()
-00056eb0: 2c20 7469 6d65 7320 3d20 7365 6c66 2e72  , times = self.r
-00056ec0: 656c 5f74 696d 652c 200d 0a09 0909 0909  el_time, .......
-00056ed0: 0909 7469 6d65 5f77 6964 7468 5f70 6572  ..time_width_per
-00056ee0: 6365 6e74 203d 2073 656c 662e 7469 6d65  cent = self.time
-00056ef0: 5f77 6964 7468 5f70 6572 6365 6e74 2c20  _width_percent, 
-00056f00: 7363 6174 7465 7263 7574 203d 2073 656c  scattercut = sel
-00056f10: 662e 7363 6174 7465 7263 7574 2c20 0d0a  f.scattercut, ..
-00056f20: 0909 0909 0909 0962 6f72 6465 7263 7574  .......bordercut
-00056f30: 203d 2073 656c 662e 626f 7264 6572 6375   = self.bordercu
-00056f40: 742c 2077 6176 655f 6e6d 5f62 696e 203d  t, wave_nm_bin =
-00056f50: 2073 656c 662e 7761 7665 5f6e 6d5f 6269   self.wave_nm_bi
-00056f60: 6e29 0d0a 0909 0909 7375 622e 746f 5f63  n)......sub.to_c
-00056f70: 7376 2863 6865 636b 5f66 6f6c 6465 7228  sv(check_folder(
-00056f80: 7061 7468 203d 2070 6174 682c 2063 7572  path = path, cur
-00056f90: 7265 6e74 5f70 6174 6820 3d20 7365 6c66  rent_path = self
-00056fa0: 2e70 6174 682c 200d 0a09 0909 0909 0909  .path, .........
-00056fb0: 6669 6c65 6e61 6d65 203d 2066 696c 656e  filename = filen
-00056fc0: 616d 652b 275f 6d65 6173 7572 6564 5f73  ame+'_measured_s
-00056fd0: 7065 6374 7261 2e64 6174 2729 2c20 7365  pectra.dat'), se
-00056fe0: 7020 3d20 7365 7029 0d0a 0909 0909 7365  p = sep)......se
-00056ff0: 6c66 2e72 655b 2744 4143 275d 2e74 6f5f  lf.re['DAC'].to_
-00057000: 6373 7628 6368 6563 6b5f 666f 6c64 6572  csv(check_folder
-00057010: 2870 6174 6820 3d20 7061 7468 2c20 6375  (path = path, cu
-00057020: 7272 656e 745f 7061 7468 203d 2073 656c  rrent_path = sel
-00057030: 662e 7061 7468 2c20 0d0a 0909 0909 0909  f.path, ........
-00057040: 0966 696c 656e 616d 6520 3d20 6669 6c65  .filename = file
-00057050: 6e61 6d65 2b27 5f44 4153 2d53 4153 2e64  name+'_DAS-SAS.d
-00057060: 6174 2729 2c20 7365 7020 3d20 7365 7029  at'), sep = sep)
-00057070: 0d0a 0909 0d0a 0909 0969 6620 7361 7665  .........if save
-00057080: 5f66 6974 5f72 6573 756c 7473 3a0d 0a09  _fit_results:...
-00057090: 0909 090d 0a09 0909 0952 6573 756c 745f  .........Result_
-000570a0: 7374 7269 6e67 3d27 5c6e 4669 7420 5265  string='\nFit Re
-000570b0: 7375 6c74 733a 5c6e 270d 0a09 0909 090d  sults:\n'.......
-000570c0: 0a09 0909 0969 6620 6973 696e 7374 616e  .....if isinstan
-000570d0: 6365 2873 656c 662e 6d6f 642c 7479 7065  ce(self.mod,type
-000570e0: 2827 6865 6c6c 6f27 2929 3a0d 0a09 0909  ('hello')):.....
-000570f0: 0909 5265 7375 6c74 5f73 7472 696e 672b  ..Result_string+
-00057100: 3d27 4d6f 6465 6c20 5573 6564 3a20 2573  ='Model Used: %s
-00057110: 5c6e 5c6e 2725 7365 6c66 2e6d 6f64 0d0a  \n\n'%self.mod..
-00057120: 0909 0909 656c 7365 3a0d 0a09 0909 0909  ....else:.......
-00057130: 5265 7375 6c74 5f73 7472 696e 672b 3d27  Result_string+='
-00057140: 4d6f 6465 6c20 5573 6564 3a20 4578 7465  Model Used: Exte
-00057150: 726e 616c 2066 756e 6374 696f 6e5c 6e5c  rnal function\n\
-00057160: 6e27 0d0a 0909 0909 0d0a 0909 0909 6966  n'............if
-00057170: 2073 656c 662e 6967 6e6f 7265 5f74 696d   self.ignore_tim
-00057180: 655f 7265 6769 6f6e 2069 7320 6e6f 7420  e_region is not 
-00057190: 4e6f 6e65 3a0d 0a09 0909 0909 5265 7375  None:.......Resu
-000571a0: 6c74 5f73 7472 696e 672b 3d27 7468 6520  lt_string+='the 
-000571b0: 7469 6d65 2062 6574 7765 656e 2025 2e33  time between %.3
-000571c0: 6620 2573 2061 6e64 2025 2e33 6620 2573  f %s and %.3f %s
-000571d0: 2077 6173 2065 7863 6c75 6465 6420 6672   was excluded fr
-000571e0: 6f6d 2074 6865 206f 7074 696d 697a 6174  om the optimizat
-000571f0: 696f 6e5c 6e27 2528 7365 6c66 2e69 676e  ion\n'%(self.ign
-00057200: 6f72 655f 7469 6d65 5f72 6567 696f 6e5b  ore_time_region[
-00057210: 305d 2c73 656c 662e 6261 7365 756e 6974  0],self.baseunit
-00057220: 2c73 656c 662e 6967 6e6f 7265 5f74 696d  ,self.ignore_tim
-00057230: 655f 7265 6769 6f6e 5b31 5d2c 7365 6c66  e_region[1],self
-00057240: 2e62 6173 6575 6e69 7429 090d 0a09 0909  .baseunit)......
-00057250: 0952 6573 756c 745f 7374 7269 6e67 2b3d  .Result_string+=
-00057260: 2754 6865 206d 696e 696d 756d 2065 7272  'The minimum err
-00057270: 6f72 2069 733a 7b3a 2e38 657d 5c6e 272e  or is:{:.8e}\n'.
-00057280: 666f 726d 6174 2873 656c 662e 7265 5b27  format(self.re['
-00057290: 6572 726f 7227 5d29 0d0a 0909 0909 5265  error'])......Re
-000572a0: 7375 6c74 5f73 7472 696e 672b 3d27 5468  sult_string+='Th
-000572b0: 6520 6d69 6e69 6d75 6d20 5232 2d76 616c  e minimum R2-val
-000572c0: 7565 2069 733a 7b3a 2e38 657d 5c6e 272e  ue is:{:.8e}\n'.
-000572d0: 666f 726d 6174 2873 656c 662e 7265 5b27  format(self.re['
-000572e0: 7232 275d 290d 0a09 0909 090d 0a09 0909  r2'])...........
-000572f0: 0969 6620 2763 6f6e 6669 6465 6e63 6527  .if 'confidence'
-00057300: 2069 6e20 7365 6c66 2e72 653a 0d0a 0909   in self.re:....
-00057310: 0909 0952 6573 756c 745f 7374 7269 6e67  ...Result_string
-00057320: 2b3d 275c 6e49 6e20 5261 7465 7320 7769  +='\nIn Rates wi
-00057330: 7468 2063 6f6e 6669 6465 6e63 6520 696e  th confidence in
-00057340: 7465 7276 616c 2074 6f20 6c65 7665 6c20  terval to level 
-00057350: 6f66 2025 735c 6e27 2573 656c 662e 7265  of %s\n'%self.re
-00057360: 5b27 636f 6e66 6964 656e 6365 275d 5b27  ['confidence']['
-00057370: 7461 7267 6574 2d6c 6576 656c 275d 0d0a  target-level']..
-00057380: 0909 0909 0952 6573 756c 745f 7374 7269  .....Result_stri
-00057390: 6e67 2b3d 7365 6c66 2e72 655b 2766 6974  ng+=self.re['fit
-000573a0: 5f72 6573 756c 7473 5f72 6174 6573 275d  _results_rates']
-000573b0: 2e74 6f5f 7374 7269 6e67 2863 6f6c 756d  .to_string(colum
-000573c0: 6e73 3d5b 2776 616c 7565 272c 276c 6f77  ns=['value','low
-000573d0: 6572 5f6c 696d 6974 272c 2775 7070 6572  er_limit','upper
-000573e0: 5f6c 696d 6974 272c 2769 6e69 745f 7661  _limit','init_va
-000573f0: 6c75 6527 2c27 7661 7279 272c 276d 696e  lue','vary','min
-00057400: 272c 276d 6178 272c 2765 7870 7227 5d29  ','max','expr'])
-00057410: 0d0a 0909 0909 0952 6573 756c 745f 7374  .......Result_st
-00057420: 7269 6e67 2b3d 275c 6e5c 6e54 6865 2072  ring+='\n\nThe r
-00057430: 6174 6573 2063 6f6e 7665 7274 6564 2074  ates converted t
-00057440: 6f20 7469 6d65 7320 7769 7468 2075 6e69  o times with uni
-00057450: 7420 2573 2077 6974 6820 636f 6e66 6964  t %s with confid
-00057460: 656e 6365 2069 6e74 6572 7661 6c20 746f  ence interval to
-00057470: 206c 6576 656c 206f 6620 2573 5c6e 2725   level of %s\n'%
-00057480: 2873 656c 662e 6261 7365 756e 6974 2c73  (self.baseunit,s
-00057490: 656c 662e 7265 5b27 636f 6e66 6964 656e  elf.re['confiden
-000574a0: 6365 275d 5b27 7461 7267 6574 2d6c 6576  ce']['target-lev
-000574b0: 656c 275d 290d 0a09 0909 0909 5265 7375  el']).......Resu
-000574c0: 6c74 5f73 7472 696e 672b 3d73 656c 662e  lt_string+=self.
-000574d0: 7265 5b27 6669 745f 7265 7375 6c74 735f  re['fit_results_
-000574e0: 7469 6d65 7327 5d2e 746f 5f73 7472 696e  times'].to_strin
-000574f0: 6728 636f 6c75 6d6e 733d 5b27 7661 6c75  g(columns=['valu
-00057500: 6527 2c27 6c6f 7765 725f 6c69 6d69 7427  e','lower_limit'
-00057510: 2c27 7570 7065 725f 6c69 6d69 7427 2c27  ,'upper_limit','
-00057520: 696e 6974 5f76 616c 7565 272c 2776 6172  init_value','var
-00057530: 7927 2c27 6d69 6e27 2c27 6d61 7827 2c27  y','min','max','
-00057540: 6578 7072 275d 290d 0a09 0909 0965 6c73  expr'])......els
-00057550: 653a 0d0a 0909 0909 0952 6573 756c 745f  e:.......Result_
-00057560: 7374 7269 6e67 2b3d 275c 6e49 6e20 5261  string+='\nIn Ra
-00057570: 7465 735c 6e27 0d0a 0909 0909 0952 6573  tes\n'.......Res
-00057580: 756c 745f 7374 7269 6e67 2b3d 7365 6c66  ult_string+=self
-00057590: 2e72 655b 2766 6974 5f72 6573 756c 7473  .re['fit_results
-000575a0: 5f72 6174 6573 275d 2e74 6f5f 7374 7269  _rates'].to_stri
-000575b0: 6e67 2863 6f6c 756d 6e73 3d5b 2776 616c  ng(columns=['val
-000575c0: 7565 272c 2769 6e69 745f 7661 6c75 6527  ue','init_value'
-000575d0: 2c27 7661 7279 272c 276d 696e 272c 276d  ,'vary','min','m
-000575e0: 6178 272c 2765 7870 7227 5d29 0d0a 0909  ax','expr'])....
-000575f0: 0909 0952 6573 756c 745f 7374 7269 6e67  ...Result_string
-00057600: 2b3d 275c 6e5c 6e54 6865 2072 6174 6573  +='\n\nThe rates
-00057610: 2063 6f6e 7665 7274 6564 2074 6f20 7469   converted to ti
-00057620: 6d65 7320 7769 7468 2075 6e69 7420 2573  mes with unit %s
-00057630: 5c6e 2725 7365 6c66 2e62 6173 6575 6e69  \n'%self.baseuni
-00057640: 740d 0a09 0909 0909 5265 7375 6c74 5f73  t.......Result_s
-00057650: 7472 696e 672b 3d73 656c 662e 7265 5b27  tring+=self.re['
-00057660: 6669 745f 7265 7375 6c74 735f 7469 6d65  fit_results_time
-00057670: 7327 5d2e 746f 5f73 7472 696e 6728 636f  s'].to_string(co
-00057680: 6c75 6d6e 733d 5b27 7661 6c75 6527 2c27  lumns=['value','
-00057690: 696e 6974 5f76 616c 7565 272c 2776 6172  init_value','var
-000576a0: 7927 2c27 6d69 6e27 2c27 6d61 7827 2c27  y','min','max','
-000576b0: 6578 7072 275d 290d 0a0d 0a09 0909 0977  expr'])........w
-000576c0: 6974 6820 6f70 656e 2863 6865 636b 5f66  ith open(check_f
-000576d0: 6f6c 6465 7228 7061 7468 203d 2070 6174  older(path = pat
-000576e0: 682c 2063 7572 7265 6e74 5f70 6174 6820  h, current_path 
-000576f0: 3d20 7365 6c66 2e70 6174 682c 2066 696c  = self.path, fil
-00057700: 656e 616d 6520 3d20 6669 6c65 6e61 6d65  ename = filename
-00057710: 2b27 5f66 6974 5f72 6573 756c 7473 5f70  +'_fit_results_p
-00057720: 6172 616d 6574 6572 2e70 6172 2729 2c20  arameter.par'), 
-00057730: 2277 2229 2061 7320 7465 7874 5f66 696c  "w") as text_fil
-00057740: 653a 0d0a 0909 0909 0974 6578 745f 6669  e:.......text_fi
-00057750: 6c65 2e77 7269 7465 2852 6573 756c 745f  le.write(Result_
-00057760: 7374 7269 6e67 290d 0a0d 0a09 6465 6620  string).....def 
-00057770: 5361 7665 5f50 6f77 6572 706f 696e 7428  Save_Powerpoint(
-00057780: 7365 6c66 2c20 7361 7665 5f52 4157 203d  self, save_RAW =
-00057790: 2054 7275 652c 2073 6176 655f 4669 7420   True, save_Fit 
-000577a0: 3d20 5472 7565 2c20 6669 6c65 6e61 6d65  = True, filename
-000577b0: 203d 204e 6f6e 652c 200d 0a09 0909 0909   = None, .......
-000577c0: 0970 6174 6820 3d20 2772 6573 756c 745f  .path = 'result_
-000577d0: 6669 6775 7265 7327 2c20 7363 616c 655f  figures', scale_
-000577e0: 7479 7065 203d 2027 7379 6d6c 6f67 272c  type = 'symlog',
-000577f0: 2074 6974 6c65 203d 204e 6f6e 652c 2070   title = None, p
-00057800: 6174 6368 6573 203d 2046 616c 7365 2c20  atches = False, 
-00057810: 636d 6170 3d4e 6f6e 6520 2c20 7361 7665  cmap=None , save
-00057820: 7479 7065 203d 2027 7070 7478 2729 3a0d  type = 'pptx'):.
-00057830: 0a09 0927 2727 5468 6973 2066 756e 6374  ...'''This funct
-00057840: 696f 6e20 6372 6561 7465 7320 7477 6f20  ion creates two 
-00057850: 706f 7765 7220 706f 696e 7420 736c 6964  power point slid
-00057860: 6573 2e20 4f6e 2074 6865 2066 6972 7374  es. On the first
-00057870: 2069 7420 7375 6d6d 6172 697a 6573 2074   it summarizes t
-00057880: 6865 2052 4157 2070 6c6f 7473 2061 6e64  he RAW plots and
-00057890: 206f 6e20 0d0a 0909 7468 6520 7365 636f   on ....the seco
-000578a0: 6e64 2028 6966 2065 7869 7374 656e 7429  nd (if existent)
-000578b0: 2069 7420 7375 6d6d 6172 697a 6573 2074   it summarizes t
-000578c0: 6865 2066 6974 7465 6420 7265 7375 6c74  he fitted result
-000578d0: 730d 0a09 090d 0a09 0950 6172 616d 6574  s........Paramet
-000578e0: 6572 730d 0a09 092d 2d2d 2d2d 2d2d 2d2d  ers....---------
-000578f0: 2d0d 0a09 090d 0a09 0973 6176 655f 5241  -........save_RA
-00057900: 5720 3a20 626f 6f6c 2c20 6f70 7469 6f6e  W : bool, option
-00057910: 616c 0d0a 0909 0928 4465 6661 756c 7429  al.....(Default)
-00057920: 2054 7275 6520 7468 656e 2074 6865 2066   True then the f
-00057930: 6972 7374 2073 6c69 6465 2077 6974 6820  irst slide with 
-00057940: 7468 6520 5241 5720 6461 7461 2069 7320  the RAW data is 
-00057950: 6372 6561 7465 6420 0d0a 0909 0d0a 0909  created ........
-00057960: 7361 7665 5f46 6974 203a 2062 6f6f 6c2c  save_Fit : bool,
-00057970: 206f 7074 696f 6e61 6c0d 0a09 0909 2844   optional.....(D
-00057980: 6566 6175 6c74 2920 5472 7565 2074 6865  efault) True the
-00057990: 6e20 7468 6520 7365 636f 6e64 2073 6c69  n the second sli
-000579a0: 6465 2077 6974 6820 7468 6520 4669 7474  de with the Fitt
-000579b0: 6564 2064 6174 6120 6973 2063 7265 6174  ed data is creat
-000579c0: 6564 200d 0a09 090d 0a09 0970 6174 6820  ed ........path 
-000579d0: 3a20 4e6f 6e65 2c20 7374 7220 6f72 2070  : None, str or p
-000579e0: 6174 682c 206f 7074 696f 6e61 6c0d 0a09  ath, optional...
-000579f0: 0909 2844 6566 6175 6c74 2920 4e6f 6e65  ..(Default) None
-00057a00: 2c20 6966 206c 6566 7420 6f6e 204e 6f6e  , if left on Non
-00057a10: 652c 2074 6865 6e20 6120 666f 6c64 6572  e, then a folder
-00057a20: 2022 7265 7375 6c74 5f66 6967 7572 6573   "result_figures
-00057a30: 2220 6973 2063 7265 6174 6564 2069 6e20  " is created in 
-00057a40: 7468 6520 666f 6c64 6572 200d 0a09 0909  the folder .....
-00057a50: 6f66 2074 6865 2064 6174 6120 2873 656c  of the data (sel
-00057a60: 662e 7061 7468 290d 0a09 090d 0a09 0973  f.path)........s
-00057a70: 6176 6574 7970 6520 3a20 7374 7220 6f72  avetype : str or
-00057a80: 2069 7465 7261 626c 6520 286f 6620 7374   iterable (of st
-00057a90: 7229 2c20 6f70 7469 6f6e 616c 200d 0a09  r), optional ...
-00057aa0: 0909 7472 6967 6765 7273 2074 6865 2061  ..triggers the a
-00057ab0: 6464 6974 696f 6e61 6c20 6372 6561 7469  dditional creati
-00057ac0: 6f6e 206f 6620 6120 636f 6d70 6f73 6974  on of a composit
-00057ad0: 6520 6669 6c65 2069 6e20 7468 6973 2066  e file in this f
-00057ae0: 6f72 6d61 742e 0d0a 0909 096d 6174 706c  ormat......matpl
-00057af0: 6f74 6c69 6220 616c 6c6f 7773 2074 6865  otlib allows the
-00057b00: 2073 6176 696e 6720 6f66 2066 6967 7572   saving of figur
-00057b10: 6573 2069 6e20 7661 7269 6f75 7320 666f  es in various fo
-00057b20: 726d 6174 732e 2028 4465 6661 756c 7429  rmats. (Default)
-00057b30: 2022 706e 6722 2c20 0d0a 0909 0974 7970   "png", .....typ
-00057b40: 6963 616c 2061 6e64 2072 6563 6f6d 6d65  ical and recomme
-00057b50: 6e64 6162 6c65 206f 7074 696f 6e73 2061  ndable options a
-00057b60: 7265 2022 7376 6722 2061 6e64 2022 7064  re "svg" and "pd
-00057b70: 6622 2e20 200d 0a09 0909 0d0a 0909 7469  f".  .........ti
-00057b80: 746c 6520 3a20 4e6f 6e65 206f 7220 7374  tle : None or st
-00057b90: 722c 206f 7074 696f 6e61 6c0d 0a09 0909  r, optional.....
-00057ba0: 2844 6566 6175 6c74 2920 4e6f 6e65 2c20  (Default) None, 
-00057bb0: 5573 6520 7468 6973 2074 6974 6c65 206f  Use this title o
-00057bc0: 6e20 616c 6c20 706c 6f74 732e 2069 6620  n all plots. if 
-00057bd0: 4e6f 6e65 2c20 7573 6520 7365 6c66 2e66  None, use self.f
-00057be0: 696c 656e 616d 650d 0a09 0909 0d0a 0909  ilename.........
-00057bf0: 6669 6c65 6e61 6d65 203a 2073 7472 2c20  filename : str, 
-00057c00: 6f70 7469 6f6e 616c 0d0a 0909 0928 4465  optional.....(De
-00057c10: 6661 756c 7429 204e 6f6e 652c 2042 6173  fault) None, Bas
-00057c20: 6520 6e61 6d65 2066 6f72 2061 6c6c 2070  e name for all p
-00057c30: 6c6f 7473 2e20 4966 204e 6f6e 652c 2074  lots. If None, t
-00057c40: 6865 6e20 7365 6c66 2e66 696c 656e 616d  hen self.filenam
-00057c50: 6520 7769 6c6c 2062 6520 7573 6564 0d0a  e will be used..
-00057c60: 0909 090d 0a09 0973 6361 6c65 5f74 7970  .......scale_typ
-00057c70: 6520 3a20 7374 722c 206f 7074 696f 6e61  e : str, optiona
-00057c80: 6c0d 0a09 0909 2773 796d 6c6f 6727 2028  l.....'symlog' (
-00057c90: 4465 6661 756c 7429 2c20 276c 696e 6561  Default), 'linea
-00057ca0: 7227 2c20 276c 6f67 2720 7469 6d65 2061  r', 'log' time a
-00057cb0: 7869 730d 0a09 0909 0d0a 0909 7061 7463  xis.........patc
-00057cc0: 6865 7320 3a20 626f 6f6c 2c20 6f70 7469  hes : bool, opti
-00057cd0: 6f6e 616c 0d0a 0909 0946 6f72 2074 7275  onal.....For tru
-00057ce0: 6520 7573 6520 7768 6974 6520 7061 7463  e use white patc
-00057cf0: 6865 7320 746f 206c 6162 656c 2074 6869  hes to label thi
-00057d00: 6e67 7320 696e 2074 6865 2032 6420 6d61  ngs in the 2d ma
-00057d10: 7472 6978 6573 2c20 746f 2073 6166 650d  trixes, to safe.
-00057d20: 0a09 0909 7370 6163 6520 666f 7220 7075  ....space for pu
-00057d30: 626c 6963 6174 696f 6e0d 0a09 0909 0d0a  blication.......
-00057d40: 0909 636d 6170 203a 204e 6f6e 6520 6f72  ..cmap : None or
-00057d50: 206d 6174 706c 6f74 6c69 6220 636f 6c6f   matplotlib colo
-00057d60: 7220 6d61 702c 206f 7074 696f 6e61 6c0d  r map, optional.
-00057d70: 0a09 0909 6973 2061 2070 6f77 6572 6675  ....is a powerfu
-00057d80: 6c6c 2076 6172 6961 626c 6520 7468 6174  ll variable that
-00057d90: 2063 686f 6f73 6573 2074 6865 2063 6f6c   chooses the col
-00057da0: 6f75 7220 6d61 7020 6170 706c 6965 6420  our map applied 
-00057db0: 666f 7220 616c 6c20 706c 6f74 732e 2049  for all plots. I
-00057dc0: 6620 7365 7420 746f 200d 0a09 0909 4e6f  f set to .....No
-00057dd0: 6e65 2028 4465 6661 756c 7429 2074 6865  ne (Default) the
-00057de0: 6e20 7468 6520 7365 6c66 2e63 6d61 7020  n the self.cmap 
-00057df0: 6973 2075 7365 642e 0d0a 0909 0941 7320  is used......As 
-00057e00: 7374 616e 6461 7264 2049 2075 7365 2074  standard I use t
-00057e10: 6865 2063 6f6c 6f72 206d 6170 2022 6a65  he color map "je
-00057e20: 7422 2066 726f 6d20 6d61 7470 6c6f 746c  t" from matplotl
-00057e30: 6962 2e20 5468 6572 6520 6172 6520 6120  ib. There are a 
-00057e40: 7661 7269 6574 7920 6f66 2063 6f6c 6f72  variety of color
-00057e50: 6d61 7073 200d 0a09 0909 6176 6169 6c61  maps .....availa
-00057e60: 626c 6520 7468 6174 2061 7265 2076 6572  ble that are ver
-00057e70: 7920 7573 6566 756c 6c2e 2042 6573 6964  y usefull. Besid
-00057e80: 6520 226a 6574 222c 2022 7669 7269 6469  e "jet", "viridi
-00057e90: 7322 2069 7320 6120 676f 6f64 2063 686f  s" is a good cho
-00057ea0: 6963 6520 6173 2069 7420 6973 2077 656c  ice as it is wel
-00057eb0: 6c20 0d0a 0909 0976 6973 6962 6c65 2075  l .....visible u
-00057ec0: 6e64 6572 2072 6564 2d67 7265 656e 2062  nder red-green b
-00057ed0: 6c69 6e64 6e65 7373 2e20 4f74 6865 7220  lindness. Other 
-00057ee0: 7573 6566 756c 206d 6170 7320 6172 6520  useful maps are 
-00057ef0: 2270 7269 736d 2220 666f 7220 6869 6768  "prism" for high
-00057f00: 2066 6c75 6374 7561 7469 6f6e 7320 0d0a   fluctuations ..
-00057f10: 0909 096f 7220 6469 7665 7267 696e 6720  ...or diverging 
-00057f20: 636f 6c6f 7220 6d61 7073 206c 696b 6520  color maps like 
-00057f30: 2273 6569 736d 6963 222e 200d 0a09 0909  "seismic". .....
-00057f40: 5365 6520 6874 7470 733a 2f2f 6d61 7470  See https://matp
-00057f50: 6c6f 746c 6962 2e6f 7267 2f33 2e31 2e30  lotlib.org/3.1.0
-00057f60: 2f74 7574 6f72 6961 6c73 2f63 6f6c 6f72  /tutorials/color
-00057f70: 732f 636f 6c6f 726d 6170 732e 6874 6d6c  s/colormaps.html
-00057f80: 2066 6f72 2061 2063 6f6d 7072 6568 656e   for a comprehen
-00057f90: 7369 7665 200d 0a09 0909 7365 6c65 6374  sive .....select
-00057fa0: 696f 6e2e 2049 6e20 7468 6520 636f 6465  ion. In the code
-00057fb0: 2074 6865 2063 6f6c 6f72 6d61 7073 2061   the colormaps a
-00057fc0: 7265 2069 6d70 6f72 7465 6420 736f 2069  re imported so i
-00057fd0: 6620 706c 6f74 5f66 756e 6320 6973 2069  f plot_func is i
-00057fe0: 6d70 6f72 7465 6420 6173 2070 6620 7468  mported as pf th
-00057ff0: 656e 200d 0a09 0909 7365 6c66 2e63 6d61  en .....self.cma
-00058000: 703d 7066 2e63 6d2e 7669 7269 6469 7320  p=pf.cm.viridis 
-00058010: 7365 7473 2076 6972 6964 6973 2061 7320  sets viridis as 
-00058020: 7468 6520 6d61 7020 746f 2075 7365 2e20  the map to use. 
-00058030: 496e 7465 726e 616c 6c79 2074 6865 2063  Internally the c
-00058040: 6f6c 6f72 7320 6172 6520 6368 6f73 656e  olors are chosen
-00058050: 200d 0a09 0909 7769 7468 2074 6865 2022   .....with the "
-00058060: 636f 6c6d 2220 6675 6e63 7469 6f6e 2e20  colm" function. 
-00058070: 5468 6520 3264 2070 6c6f 7473 2072 6571  The 2d plots req
-00058080: 7569 7265 2061 2063 6f6e 7469 6e75 6f75  uire a continuou
-00058090: 7320 636f 6c6f 7220 6d61 7020 736f 2069  s color map so i
-000580a0: 6620 736f 6d65 7468 696e 6720 0d0a 0909  f something ....
-000580b0: 0965 6c73 6520 6973 2067 6976 6520 3264  .else is give 2d
-000580c0: 2070 6c6f 7473 2061 7265 2073 686f 776e   plots are shown
-000580d0: 2061 7574 6f6d 6174 6963 616c 6c79 2077   automatically w
-000580e0: 6974 6820 226a 6574 222e 2046 6f72 2061  ith "jet". For a
-000580f0: 6c6c 206f 6620 7468 6520 3164 2070 6c6f  ll of the 1d plo
-00058100: 7473 2068 6f77 6576 6572 200d 0a09 0909  ts however .....
-00058110: 4920 6669 7273 7420 7365 6c65 6374 2061  I first select a
-00058120: 206e 756d 6265 7220 6f66 2063 6f6c 6f72   number of color
-00058130: 7320 6265 666f 7265 2065 6163 6820 706c  s before each pl
-00058140: 6f74 2e20 4966 2063 6d61 7020 6973 2061  ot. If cmap is a
-00058150: 2063 6f6e 7469 6e6f 7573 206d 6170 2074   continous map t
-00058160: 6865 6e20 7468 6573 650d 0a09 0909 6172  hen these.....ar
-00058170: 6520 7361 6d70 6c65 6420 6576 656e 6c79  e sampled evenly
-00058180: 206f 7665 7220 7468 6520 636f 6c6f 7572   over the colour
-00058190: 6d61 702e 204d 616e 7561 6c20 6974 6572  map. Manual iter
-000581a0: 6162 6c65 7320 6f66 2063 6f6c 6f75 7273  ables of colours
-000581b0: 200d 0a09 0909 636d 6170 3d5b 2831 2c30   .....cmap=[(1,0
-000581c0: 2c30 292c 2830 2c31 2c30 292c 2830 2c30  ,0),(0,1,0),(0,0
-000581d0: 2c31 292c 2e2e 2e5d 2061 7265 2061 6c73  ,1),...] are als
-000581e0: 6f20 6163 6365 7074 6564 2c20 6173 2061  o accepted, as a
-000581f0: 7265 2076 6563 746f 7273 206f 7220 6461  re vectors or da
-00058200: 7461 6672 616d 6573 2074 6861 7420 0d0a  taframes that ..
-00058210: 0909 0963 6f6e 7461 696e 2061 7320 726f  ...contain as ro
-00058220: 7773 2074 6865 2063 6f6c 6f72 732e 2054  ws the colors. T
-00058230: 6865 7265 206d 7573 7420 6265 206f 6620  here must be of 
-00058240: 636f 7572 7365 2073 7566 6669 6369 656e  course sufficien
-00058250: 7420 636f 6c6f 7273 2070 7265 7365 6e74  t colors present
-00058260: 2066 6f72 200d 0a09 0909 7468 6520 6e75   for .....the nu
-00058270: 6d62 6572 7320 6f66 206c 696e 6573 2074  mbers of lines t
-00058280: 6861 7420 7769 6c6c 2062 6520 706c 6f74  hat will be plot
-00058290: 7465 642e 2053 6f20 4920 7265 636f 6d6d  ted. So I recomm
-000582a0: 656e 6420 746f 2070 726f 7669 6465 2061  end to provide a
-000582b0: 7420 6c65 6173 7420 3130 2063 6f6c 6f75  t least 10 colou
-000582c0: 7273 200d 0a09 0909 2865 2e67 2e7e 796f  rs .....(e.g.~yo
-000582d0: 7572 2075 6e69 7665 7273 6974 7920 636f  ur university co
-000582e0: 6c6f 7273 292e 2063 6f6c 6f75 7273 2061  lors). colours a
-000582f0: 7265 2061 6c77 6179 7320 6769 7665 6e20  re always given 
-00058300: 6173 2061 2c20 6c69 7374 206f 7220 7475  as a, list or tu
-00058310: 706c 6520 7769 7468 2052 4741 206f 7220  ple with RGA or 
-00058320: 5247 4241 0d0a 0909 0928 7769 7468 2074  RGBA.....(with t
-00058330: 6865 206c 6173 7420 4120 6265 6569 6e67  he last A beeing
-00058340: 2074 6865 2041 6c70 6861 3d74 7261 6e73   the Alpha=trans
-00058350: 7061 7265 6e63 792e 2041 6c6c 206e 756d  parency. All num
-00058360: 6265 7273 2061 7265 2062 6574 7765 656e  bers are between
-00058370: 2030 2061 6e64 2031 2e20 0d0a 0909 0949   0 and 1. .....I
-00058380: 6620 6120 6c69 7374 2f76 6563 746f 722f  f a list/vector/
-00058390: 4461 7461 4672 616d 6520 6973 2067 6976  DataFrame is giv
-000583a0: 656e 2066 6f72 2074 6865 2063 6f6c 6f75  en for the colou
-000583b0: 7273 2074 6865 7920 7769 6c6c 2062 6520  rs they will be 
-000583c0: 7573 6564 2069 6e20 7468 6520 6f72 6465  used in the orde
-000583d0: 7220 7072 6f76 6964 6564 2e0d 0a09 090d  r provided......
-000583e0: 0a09 0945 7861 6d70 6c65 730d 0a09 092d  ...Examples....-
-000583f0: 2d2d 2d2d 2d2d 2d2d 0d0a 0909 0d0a 0909  --------........
-00058400: 3e3e 3e20 7461 2e53 6176 655f 506f 7765  >>> ta.Save_Powe
-00058410: 7270 6f69 6e74 2829 0d0a 0909 3e3e 3e20  rpoint()....>>> 
-00058420: 7461 2e53 6176 655f 506f 7765 7270 6f69  ta.Save_Powerpoi
-00058430: 6e74 2870 6174 6368 6573 203d 2054 7275  nt(patches = Tru
-00058440: 6529 0d0a 0909 0d0a 0909 2727 2709 0909  e)........'''...
-00058450: 0909 0920 0d0a 0909 6966 2069 7369 6e73  ... ....if isins
-00058460: 7461 6e63 6528 7361 7665 7479 7065 2c74  tance(savetype,t
-00058470: 7970 6528 2768 656c 6c6f 2729 293a 7361  ype('hello')):sa
-00058480: 7665 7479 7065 3d5b 7361 7665 7479 7065  vetype=[savetype
-00058490: 5d0d 0a09 0969 6620 6e6f 7420 6861 7361  ]....if not hasa
-000584a0: 7474 7228 7361 7665 7479 7065 2c22 5f5f  ttr(savetype,"__
-000584b0: 6974 6572 5f5f 2229 3a73 6176 6574 7970  iter__"):savetyp
+000528d0: 7469 6d65 7327 5d3a 0d0a 0909 0909 0974  times']:.......t
+000528e0: 7279 3a0d 0a09 0909 0909 0972 655f 6c69  ry:........re_li
+000528f0: 7374 656e 5b69 5d5b 6e61 6d65 5d3d 7265  sten[i][name]=re
+00052900: 5b6e 616d 655d 0d0a 0909 0909 0965 7863  [name].......exc
+00052910: 6570 743a 0d0a 0909 0909 0909 7072 696e  ept:........prin
+00052920: 7428 6e61 6d65 202b 2027 6e6f 7420 666f  t(name + 'not fo
+00052930: 756e 6427 290d 0a09 090d 0a09 0923 2323  und')........###
+00052940: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00052950: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00052960: 2323 2323 2323 2323 2323 2323 0d0a 0909  ############....
+00052970: 2323 636f 6e76 6572 7420 656e 6572 6779  ##convert energy
+00052980: 2062 6163 6b20 746f 2077 6176 656c 656e   back to wavelen
+00052990: 6774 6823 2323 2323 2323 2323 2323 2323  gth#############
+000529a0: 0d0a 0909 2323 2323 2323 2323 2323 2323  ....############
+000529b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000529c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000529d0: 2323 2323 0d0a 0909 6966 2031 3a0d 0a09  ####....if 1:...
+000529e0: 0909 6966 2073 656c 662e 6571 7561 6c5f  ..if self.equal_
+000529f0: 656e 6572 6779 5f62 696e 2069 7320 6e6f  energy_bin is no
+00052a00: 7420 4e6f 6e65 3a0d 0a09 0909 0969 6620  t None:......if 
+00052a10: 7361 6d65 5f44 4153 3a0d 0a09 0909 0909  same_DAS:.......
+00052a20: 666f 7220 692c 7265 5f6c 6f63 616c 2069  for i,re_local i
+00052a30: 6e20 656e 756d 6572 6174 6528 7265 5f6c  n enumerate(re_l
+00052a40: 6973 7465 6e29 3a0d 0a09 0909 0909 0966  isten):........f
+00052a50: 6f72 206e 616d 6520 696e 205b 2741 272c  or name in ['A',
+00052a60: 2741 4327 2c27 4145 275d 3a0d 0a09 0909  'AC','AE']:.....
+00052a70: 0909 0909 7265 5f6c 6f63 616c 5b6e 616d  ....re_local[nam
+00052a80: 655d 2e63 6f6c 756d 6e73 3d28 7363 6970  e].columns=(scip
+00052a90: 792e 636f 6e73 7461 6e74 732e 682a 7363  y.constants.h*sc
+00052aa0: 6970 792e 636f 6e73 7461 6e74 732e 632f  ipy.constants.c/
+00052ab0: 2872 655f 6c6f 6361 6c5b 6e61 6d65 5d2e  (re_local[name].
+00052ac0: 636f 6c75 6d6e 732e 7661 6c75 6573 2a31  columns.values*1
+00052ad0: 652d 392a 7363 6970 792e 636f 6e73 7461  e-9*scipy.consta
+00052ae0: 6e74 732e 656c 6563 7472 6f6e 5f76 6f6c  nts.electron_vol
+00052af0: 7429 290d 0a09 0909 0909 0909 7265 5f6c  t)).........re_l
+00052b00: 6f63 616c 5b6e 616d 655d 2e63 6f6c 756d  ocal[name].colum
+00052b10: 6e73 2e6e 616d 653d 2777 6176 656c 656e  ns.name='wavelen
+00052b20: 6774 6820 696e 206e 6d27 0d0a 0909 0909  gth in nm'......
+00052b30: 0909 0972 655f 6c6f 6361 6c5b 6e61 6d65  ...re_local[name
+00052b40: 5d2e 736f 7274 5f69 6e64 6578 2869 6e70  ].sort_index(inp
+00052b50: 6c61 6365 3d54 7275 652c 6178 6973 3d31  lace=True,axis=1
+00052b60: 2c61 7363 656e 6469 6e67 3d54 7275 6529  ,ascending=True)
+00052b70: 0d0a 0909 0909 0909 7265 5f6c 6f63 616c  ........re_local
+00052b80: 5b27 4441 4327 5d2e 696e 6465 783d 2873  ['DAC'].index=(s
+00052b90: 6369 7079 2e63 6f6e 7374 616e 7473 2e68  cipy.constants.h
+00052ba0: 2a73 6369 7079 2e63 6f6e 7374 616e 7473  *scipy.constants
+00052bb0: 2e63 2f28 7265 5f6c 6f63 616c 5b27 4441  .c/(re_local['DA
+00052bc0: 4327 5d2e 696e 6465 782e 7661 6c75 6573  C'].index.values
+00052bd0: 2a31 652d 392a 7363 6970 792e 636f 6e73  *1e-9*scipy.cons
+00052be0: 7461 6e74 732e 656c 6563 7472 6f6e 5f76  tants.electron_v
+00052bf0: 6f6c 7429 290d 0a09 0909 0909 0972 655f  olt))........re_
+00052c00: 6c6f 6361 6c5b 2744 4143 275d 2e69 6e64  local['DAC'].ind
+00052c10: 6578 2e6e 616d 653d 2777 6176 656c 656e  ex.name='wavelen
+00052c20: 6774 6820 696e 206e 6d27 0d0a 0909 0909  gth in nm'......
+00052c30: 0909 7265 5f6c 6f63 616c 5b27 4441 4327  ..re_local['DAC'
+00052c40: 5d2e 736f 7274 5f69 6e64 6578 2869 6e70  ].sort_index(inp
+00052c50: 6c61 6365 3d54 7275 652c 6178 6973 3d30  lace=True,axis=0
+00052c60: 2c61 7363 656e 6469 6e67 3d54 7275 6529  ,ascending=True)
+00052c70: 0d0a 0909 0909 0909 7265 5f6c 6973 7465  ........re_liste
+00052c80: 6e5b 695d 3d72 655f 6c6f 6361 6c0d 0a09  n[i]=re_local...
+00052c90: 0909 0965 6c73 653a 0d0a 0909 0909 0966  ...else:.......f
+00052ca0: 6f72 206e 616d 6520 696e 205b 2741 272c  or name in ['A',
+00052cb0: 2741 4327 2c27 4145 275d 3a0d 0a09 0909  'AC','AE']:.....
+00052cc0: 0909 0972 655b 6e61 6d65 5d2e 636f 6c75  ...re[name].colu
+00052cd0: 6d6e 733d 2873 6369 7079 2e63 6f6e 7374  mns=(scipy.const
+00052ce0: 616e 7473 2e68 2a73 6369 7079 2e63 6f6e  ants.h*scipy.con
+00052cf0: 7374 616e 7473 2e63 2f28 7265 5b6e 616d  stants.c/(re[nam
+00052d00: 655d 2e63 6f6c 756d 6e73 2e76 616c 7565  e].columns.value
+00052d10: 732a 3165 2d39 2a73 6369 7079 2e63 6f6e  s*1e-9*scipy.con
+00052d20: 7374 616e 7473 2e65 6c65 6374 726f 6e5f  stants.electron_
+00052d30: 766f 6c74 2929 0d0a 0909 0909 0909 7265  volt))........re
+00052d40: 5b6e 616d 655d 2e63 6f6c 756d 6e73 2e6e  [name].columns.n
+00052d50: 616d 653d 2777 6176 656c 656e 6774 6820  ame='wavelength 
+00052d60: 696e 206e 6d27 0d0a 0909 0909 0909 7265  in nm'........re
+00052d70: 5b6e 616d 655d 2e73 6f72 745f 696e 6465  [name].sort_inde
+00052d80: 7828 696e 706c 6163 653d 5472 7565 2c61  x(inplace=True,a
+00052d90: 7869 733d 312c 6173 6365 6e64 696e 673d  xis=1,ascending=
+00052da0: 5472 7565 290d 0a09 0909 0909 7265 5b27  True).......re['
+00052db0: 4441 4327 5d2e 696e 6465 783d 2873 6369  DAC'].index=(sci
+00052dc0: 7079 2e63 6f6e 7374 616e 7473 2e68 2a73  py.constants.h*s
+00052dd0: 6369 7079 2e63 6f6e 7374 616e 7473 2e63  cipy.constants.c
+00052de0: 2f28 7265 5b27 4441 4327 5d2e 696e 6465  /(re['DAC'].inde
+00052df0: 782e 7661 6c75 6573 2a31 652d 392a 7363  x.values*1e-9*sc
+00052e00: 6970 792e 636f 6e73 7461 6e74 732e 656c  ipy.constants.el
+00052e10: 6563 7472 6f6e 5f76 6f6c 7429 290d 0a09  ectron_volt))...
+00052e20: 0909 0909 7265 5b27 4441 4327 5d2e 696e  ....re['DAC'].in
+00052e30: 6465 782e 6e61 6d65 3d27 7761 7665 6c65  dex.name='wavele
+00052e40: 6e67 7468 2069 6e20 6e6d 270d 0a09 0909  ngth in nm'.....
+00052e50: 0909 7265 5b27 4441 4327 5d2e 736f 7274  ..re['DAC'].sort
+00052e60: 5f69 6e64 6578 2869 6e70 6c61 6365 3d54  _index(inplace=T
+00052e70: 7275 652c 6178 6973 3d30 2c61 7363 656e  rue,axis=0,ascen
+00052e80: 6469 6e67 3d54 7275 6529 0d0a 0909 0d0a  ding=True)......
+00052e90: 0909 0d0a 0909 2323 2323 2323 2323 2323  ......##########
+00052ea0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00052eb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00052ec0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00052ed0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00052ee0: 2323 0d0a 0909 232d 2d2d 7072 696e 7420  ##....#---print 
+00052ef0: 7468 6520 6f75 7470 7574 2d2d 2d2d 2d2d  the output------
+00052f00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00052f10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00052f20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a09  -------------...
+00052f30: 0923 2323 2323 2323 2323 2323 2323 2323  .###############
+00052f40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00052f50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00052f60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00052f70: 2323 2323 2323 2323 2323 2323 230d 0a09  #############...
+00052f80: 0973 656c 662e 7265 3d72 650d 0a09 0969  .self.re=re....i
+00052f90: 6620 7361 6d65 5f44 4153 3a0d 0a09 0909  f same_DAS:.....
+00052fa0: 7265 5f6c 6973 7465 6e5b 305d 3d72 650d  re_listen[0]=re.
+00052fb0: 0a09 0909 7365 6c66 2e6d 756c 7469 5f70  ....self.multi_p
+00052fc0: 726f 6a65 6374 733d 7265 5f6c 6973 7465  rojects=re_liste
+00052fd0: 6e0d 0a0d 0a09 0952 6573 756c 745f 7374  n......Result_st
+00052fe0: 7269 6e67 3d27 5c6e 4669 7420 5265 7375  ring='\nFit Resu
+00052ff0: 6c74 733a 5c6e 270d 0a09 090d 0a09 0969  lts:\n'........i
+00053000: 6620 6973 696e 7374 616e 6365 286d 6f64  f isinstance(mod
+00053010: 2c74 7970 6528 2768 656c 6c6f 2729 293a  ,type('hello')):
+00053020: 0d0a 0909 0952 6573 756c 745f 7374 7269  .....Result_stri
+00053030: 6e67 2b3d 274d 6f64 656c 2055 7365 643a  ng+='Model Used:
+00053040: 2025 735c 6e5c 6e27 256d 6f64 0d0a 0909   %s\n\n'%mod....
+00053050: 656c 7365 3a0d 0a09 0909 5265 7375 6c74  else:.....Result
+00053060: 5f73 7472 696e 672b 3d27 4d6f 6465 6c20  _string+='Model 
+00053070: 5573 6564 3a20 4578 7465 726e 616c 2066  Used: External f
+00053080: 756e 6374 696f 6e5c 6e5c 6e27 0d0a 0909  unction\n\n'....
+00053090: 0d0a 0909 0d0a 0909 6966 2073 656c 662e  ........if self.
+000530a0: 6967 6e6f 7265 5f74 696d 655f 7265 6769  ignore_time_regi
+000530b0: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 3a0d  on is not None:.
+000530c0: 0a09 0909 7472 793a 0d0a 0909 0909 5265  ....try:......Re
+000530d0: 7375 6c74 5f73 7472 696e 672b 3d27 7468  sult_string+='th
+000530e0: 6520 7469 6d65 2062 6574 7765 656e 2025  e time between %
+000530f0: 2e33 6620 2573 2061 6e64 2025 2e33 6620  .3f %s and %.3f 
+00053100: 2573 2077 6173 2065 7863 6c75 6465 6420  %s was excluded 
+00053110: 6672 6f6d 2074 6865 206f 7074 696d 697a  from the optimiz
+00053120: 6174 696f 6e5c 6e5c 6e27 2528 7365 6c66  ation\n\n'%(self
+00053130: 2e69 676e 6f72 655f 7469 6d65 5f72 6567  .ignore_time_reg
+00053140: 696f 6e5b 305d 2c73 656c 662e 6261 7365  ion[0],self.base
+00053150: 756e 6974 2c73 656c 662e 6967 6e6f 7265  unit,self.ignore
+00053160: 5f74 696d 655f 7265 6769 6f6e 5b31 5d2c  _time_region[1],
+00053170: 7365 6c66 2e62 6173 6575 6e69 7429 0d0a  self.baseunit)..
+00053180: 0909 0965 7863 6570 743a 2377 6520 676f  ...except:#we go
+00053190: 7420 6120 6c69 7374 0d0a 0909 0909 666f  t a list......fo
+000531a0: 7220 656e 7472 7920 696e 2073 656c 662e  r entry in self.
+000531b0: 6967 6e6f 7265 5f74 696d 655f 7265 6769  ignore_time_regi
+000531c0: 6f6e 3a0d 0a09 0909 0909 5265 7375 6c74  on:.......Result
+000531d0: 5f73 7472 696e 672b 3d27 7468 6520 7469  _string+='the ti
+000531e0: 6d65 2062 6574 7765 656e 2025 2e33 6620  me between %.3f 
+000531f0: 2573 2061 6e64 2025 2e33 6620 2573 2077  %s and %.3f %s w
+00053200: 6173 2065 7863 6c75 6465 6420 6672 6f6d  as excluded from
+00053210: 2074 6865 206f 7074 696d 697a 6174 696f   the optimizatio
+00053220: 6e5c 6e5c 6e27 2528 656e 7472 795b 305d  n\n\n'%(entry[0]
+00053230: 2c73 656c 662e 6261 7365 756e 6974 2c65  ,self.baseunit,e
+00053240: 6e74 7279 5b31 5d2c 7365 6c66 2e62 6173  ntry[1],self.bas
+00053250: 6575 6e69 7429 0d0a 0909 5265 7375 6c74  eunit)....Result
+00053260: 5f73 7472 696e 672b 3d27 5468 6520 6d69  _string+='The mi
+00053270: 6e69 6d75 6d20 6572 726f 7220 6973 3a7b  nimum error is:{
+00053280: 3a2e 3865 7d5c 6e27 2e66 6f72 6d61 7428  :.8e}\n'.format(
+00053290: 7265 5b27 6572 726f 7227 5d29 0d0a 0909  re['error'])....
+000532a0: 7472 793a 0d0a 0909 0952 6573 756c 745f  try:.....Result_
+000532b0: 7374 7269 6e67 2b3d 2754 6865 206d 696e  string+='The min
+000532c0: 696d 756d 2052 322d 7661 6c75 6520 6973  imum R2-value is
+000532d0: 3a7b 3a2e 3865 7d5c 6e27 2e66 6f72 6d61  :{:.8e}\n'.forma
+000532e0: 7428 7265 5b27 7232 275d 290d 0a09 0965  t(re['r2'])....e
+000532f0: 7863 6570 743a 0d0a 0909 0970 6173 730d  xcept:.....pass.
+00053300: 0a09 0969 6620 7361 6d65 5f44 4153 3a0d  ...if same_DAS:.
+00053310: 0a09 0909 5265 7375 6c74 5f73 7472 696e  ....Result_strin
+00053320: 672b 3d27 5468 6520 6d69 6e69 6d75 6d20  g+='The minimum 
+00053330: 676c 6f62 616c 2065 7272 6f72 2069 733a  global error is:
+00053340: 7b3a 2e38 657d 5c6e 272e 666f 726d 6174  {:.8e}\n'.format
+00053350: 2872 655b 2765 7272 6f72 5f74 6f74 616c  (re['error_total
+00053360: 275d 290d 0a09 0909 5265 7375 6c74 5f73  ']).....Result_s
+00053370: 7472 696e 672b 3d27 5468 6520 6d69 6e69  tring+='The mini
+00053380: 6d75 6d20 676c 6f62 616c 2052 322d 7661  mum global R2-va
+00053390: 6c75 6520 6973 3a7b 3a2e 3865 7d5c 6e27  lue is:{:.8e}\n'
+000533a0: 2e66 6f72 6d61 7428 7265 5b27 7232 5f74  .format(re['r2_t
+000533b0: 6f74 616c 275d 290d 0a09 0969 6620 636f  otal'])....if co
+000533c0: 6e66 6964 656e 6365 5f6c 6576 656c 2069  nfidence_level i
+000533d0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a09 0909  s not None:.....
+000533e0: 5265 7375 6c74 5f73 7472 696e 672b 3d27  Result_string+='
+000533f0: 5c6e 496e 2052 6174 6573 2077 6974 6820  \nIn Rates with 
+00053400: 636f 6e66 6964 656e 6365 2069 6e74 6572  confidence inter
+00053410: 7661 6c20 746f 206c 6576 656c 206f 6620  val to level of 
+00053420: 252e 3166 5c6e 5c6e 2725 2828 636f 6e66  %.1f\n\n'%((conf
+00053430: 6964 656e 6365 5f6c 6576 656c 292a 3130  idence_level)*10
+00053440: 3029 0d0a 0909 0952 6573 756c 745f 7374  0).....Result_st
+00053450: 7269 6e67 2b3d 7061 7264 662e 746f 5f73  ring+=pardf.to_s
+00053460: 7472 696e 6728 636f 6c75 6d6e 733d 5b27  tring(columns=['
+00053470: 7661 6c75 6527 2c27 6c6f 7765 725f 6c69  value','lower_li
+00053480: 6d69 7427 2c27 7570 7065 725f 6c69 6d69  mit','upper_limi
+00053490: 7427 2c27 696e 6974 5f76 616c 7565 272c  t','init_value',
+000534a0: 2776 6172 7927 2c27 6d69 6e27 2c27 6d61  'vary','min','ma
+000534b0: 7827 2c27 6578 7072 275d 290d 0a09 0909  x','expr']).....
+000534c0: 5265 7375 6c74 5f73 7472 696e 672b 3d27  Result_string+='
+000534d0: 5c6e 5c6e 5468 6520 7261 7465 7320 636f  \n\nThe rates co
+000534e0: 6e76 6572 7465 6420 746f 2074 696d 6573  nverted to times
+000534f0: 2077 6974 6820 756e 6974 2025 7320 7769   with unit %s wi
+00053500: 7468 2063 6f6e 6669 6465 6e63 6520 696e  th confidence in
+00053510: 7465 7276 616c 2074 6f20 6c65 7665 6c20  terval to level 
+00053520: 6f66 2025 2e31 665c 6e5c 6e27 2528 7365  of %.1f\n\n'%(se
+00053530: 6c66 2e62 6173 6575 6e69 742c 2863 6f6e  lf.baseunit,(con
+00053540: 6669 6465 6e63 655f 6c65 7665 6c29 2a31  fidence_level)*1
+00053550: 3030 290d 0a09 0909 5265 7375 6c74 5f73  00).....Result_s
+00053560: 7472 696e 672b 3d74 696d 6564 662e 746f  tring+=timedf.to
+00053570: 5f73 7472 696e 6728 636f 6c75 6d6e 733d  _string(columns=
+00053580: 5b27 7661 6c75 6527 2c27 6c6f 7765 725f  ['value','lower_
+00053590: 6c69 6d69 7427 2c27 7570 7065 725f 6c69  limit','upper_li
+000535a0: 6d69 7427 2c27 696e 6974 5f76 616c 7565  mit','init_value
+000535b0: 272c 2776 6172 7927 2c27 6d69 6e27 2c27  ','vary','min','
+000535c0: 6d61 7827 2c27 6578 7072 275d 290d 0a09  max','expr'])...
+000535d0: 0965 6c73 653a 0d0a 0909 0952 6573 756c  .else:.....Resul
+000535e0: 745f 7374 7269 6e67 2b3d 275c 6e49 6e20  t_string+='\nIn 
+000535f0: 5261 7465 735c 6e5c 6e27 0d0a 0909 0952  Rates\n\n'.....R
+00053600: 6573 756c 745f 7374 7269 6e67 2b3d 7061  esult_string+=pa
+00053610: 7264 662e 746f 5f73 7472 696e 6728 636f  rdf.to_string(co
+00053620: 6c75 6d6e 733d 5b27 7661 6c75 6527 2c27  lumns=['value','
+00053630: 696e 6974 5f76 616c 7565 272c 2776 6172  init_value','var
+00053640: 7927 2c27 6d69 6e27 2c27 6d61 7827 2c27  y','min','max','
+00053650: 6578 7072 275d 290d 0a09 0909 5265 7375  expr']).....Resu
+00053660: 6c74 5f73 7472 696e 672b 3d27 5c6e 5c6e  lt_string+='\n\n
+00053670: 5468 6520 7261 7465 7320 636f 6e76 6572  The rates conver
+00053680: 7465 6420 746f 2074 696d 6573 2077 6974  ted to times wit
+00053690: 6820 756e 6974 2025 735c 6e5c 6e27 2573  h unit %s\n\n'%s
+000536a0: 656c 662e 6261 7365 756e 6974 0d0a 0909  elf.baseunit....
+000536b0: 0952 6573 756c 745f 7374 7269 6e67 2b3d  .Result_string+=
+000536c0: 7469 6d65 6466 2e74 6f5f 7374 7269 6e67  timedf.to_string
+000536d0: 2863 6f6c 756d 6e73 3d5b 2776 616c 7565  (columns=['value
+000536e0: 272c 2769 6e69 745f 7661 6c75 6527 2c27  ','init_value','
+000536f0: 7661 7279 272c 276d 696e 272c 276d 6178  vary','min','max
+00053700: 272c 2765 7870 7227 5d29 0d0a 0909 6966  ','expr'])....if
+00053710: 2073 616d 655f 4441 533a 0d0a 0909 0952   same_DAS:.....R
+00053720: 6573 756c 745f 7374 7269 6e67 2b3d 275c  esult_string+='\
+00053730: 6e5c 6e74 6865 206f 7468 6572 206f 626a  n\nthe other obj
+00053740: 6563 7473 2077 6572 6520 6c61 7965 6420  ects were layed 
+00053750: 696e 746f 2073 656c 662e 6d75 6c74 695f  into self.multi_
+00053760: 7072 6f6a 6563 7473 2061 7320 6c69 7374  projects as list
+00053770: 2077 6974 6820 7468 6520 6c6f 6361 6c20   with the local 
+00053780: 7265 206f 6e20 706f 7369 7469 6f6e 2030  re on position 0
+00053790: 2e5c 6e20 4279 2072 6570 6c61 6369 6e67  .\n By replacing
+000537a0: 2061 7373 756d 696e 6720 7468 6174 2073   assuming that s
+000537b0: 656c 6620 3d20 7461 2077 7269 7465 3a20  elf = ta write: 
+000537c0: 5c6e 2074 612e 7265 203d 2074 612e 6d75  \n ta.re = ta.mu
+000537d0: 6c74 695f 7072 6f6a 6563 7473 5b31 5d20  lti_projects[1] 
+000537e0: 616e 6420 7468 656e 2074 612e 506c 6f74  and then ta.Plot
+000537f0: 5f66 6974 5f6f 7574 7075 7420 746f 206c  _fit_output to l
+00053800: 6f6f 6b20 6f6e 2074 6865 206f 7468 6572  ook on the other
+00053810: 2066 6974 735c 6e20 270d 0a09 0909 0d0a   fits\n '.......
+00053820: 0909 7072 696e 7428 5265 7375 6c74 5f73  ..print(Result_s
+00053830: 7472 696e 6729 0d0a 0909 0d0a 0909 6966  tring)........if
+00053840: 2064 756d 705f 7061 7261 733a 0d0a 0909   dump_paras:....
+00053850: 0977 6974 6820 6f70 656e 2822 4669 745f  .with open("Fit_
+00053860: 7265 7375 6c74 735f 7072 696e 742e 7061  results_print.pa
+00053870: 7222 2c20 2277 2229 2061 7320 7465 7874  r", "w") as text
+00053880: 5f66 696c 653a 0d0a 0909 0909 7465 7874  _file:......text
+00053890: 5f66 696c 652e 7772 6974 6528 5265 7375  _file.write(Resu
+000538a0: 6c74 5f73 7472 696e 6729 0d0a 0909 090d  lt_string)......
+000538b0: 0a09 0909 0d0a 0964 6566 2050 6c6f 745f  .......def Plot_
+000538c0: 6669 745f 6f75 7470 7574 2873 656c 662c  fit_output(self,
+000538d0: 2070 6c6f 7474 696e 6720 3d20 7261 6e67   plotting = rang
+000538e0: 6528 3629 2c20 7061 7468 203d 2027 7265  e(6), path = 're
+000538f0: 7375 6c74 5f66 6967 7572 6573 272c 2073  sult_figures', s
+00053900: 6176 6574 7970 6520 3d20 2770 6e67 272c  avetype = 'png',
+00053910: 200d 0a09 0909 0909 0965 7661 6c75 6174   ........evaluat
+00053920: 696f 6e5f 7374 796c 6520 3d20 4661 6c73  ion_style = Fals
+00053930: 652c 2074 6974 6c65 203d 204e 6f6e 652c  e, title = None,
+00053940: 2073 6361 6c65 5f74 7970 6520 3d20 2773   scale_type = 's
+00053950: 796d 6c6f 6727 2c20 0d0a 0909 0909 0909  ymlog', ........
+00053960: 7061 7463 6865 7320 3d20 4661 6c73 652c  patches = False,
+00053970: 2066 696c 656e 616d 6520 3d20 4e6f 6e65   filename = None
+00053980: 2c20 636d 6170 203d 204e 6f6e 6520 2c20  , cmap = None , 
+00053990: 7072 696e 745f 636c 6963 6b5f 706f 7369  print_click_posi
+000539a0: 7469 6f6e 203d 2046 616c 7365 2c0d 0a09  tion = False,...
+000539b0: 0909 0909 0970 6c6f 745f 7365 636f 6e64  .....plot_second
+000539c0: 5f61 735f 656e 6572 6779 203d 2054 7275  _as_energy = Tru
+000539d0: 6529 3a0d 0a09 0909 0909 0909 0909 0909  e):.............
+000539e0: 0909 0909 0909 200d 0a09 0927 2727 706c  ...... ....'''pl
+000539f0: 6f74 7320 616c 6c20 7468 6520 6669 7420  ots all the fit 
+00053a00: 6f75 7470 7574 2066 6967 7572 6573 2e20  output figures. 
+00053a10: 5468 6520 6669 6775 7265 7320 6361 6e20  The figures can 
+00053a20: 6265 2063 616c 6c65 6420 7365 7061 7261  be called separa
+00053a30: 7465 6c79 200d 0a09 096f 7220 7769 7468  tely ....or with
+00053a40: 2061 206c 6973 7420 6f66 2070 6c6f 7473   a list of plots
+00053a50: 2e20 652e 672e 2072 616e 6765 2836 2920  . e.g. range(6) 
+00053a60: 6361 6c6c 2070 6c6f 7473 2030 2d35 204d  call plots 0-5 M
+00053a70: 616e 7561 6c20 706c 6f74 7469 6e67 206f  anual plotting o
+00053a80: 6620 6365 7274 6169 6e20 7479 7065 3a0d  f certain type:.
+00053a90: 0a09 090d 0a09 0954 6869 7320 6973 2061  .......This is a
+00053aa0: 2077 7261 7070 6572 2066 756e 6374 696f   wrapper functio
+00053ab0: 6e20 7468 6174 2074 7269 6767 6572 7320  n that triggers 
+00053ac0: 7468 6520 706c 6f74 7469 6e67 206f 6620  the plotting of 
+00053ad0: 616c 6c20 7468 6520 6669 7474 6564 2070  all the fitted p
+00053ae0: 6c6f 7473 2e0d 0a09 0954 6865 2070 6172  lots.....The par
+00053af0: 616d 6574 6572 2069 6e20 7468 6973 2070  ameter in this p
+00053b00: 6c6f 7420 6361 6c6c 2061 7265 2074 6f20  lot call are to 
+00053b10: 636f 6e74 726f 6c20 7468 6520 6765 6e65  control the gene
+00053b20: 7261 6c20 6c6f 6f6b 2061 6e64 2066 6561  ral look and fea
+00053b30: 7475 7265 7320 6f66 2074 6865 2070 6c6f  tures of the plo
+00053b40: 742e 0d0a 0909 5768 6963 6820 706c 6f74  t.....Which plot
+00053b50: 7320 6172 6520 7072 696e 7465 6420 6973  s are printed is
+00053b60: 2064 6566 696e 6564 2062 7920 7468 6520   defined by the 
+00053b70: 6669 7273 7420 636f 6d6d 616e 6420 2870  first command (p
+00053b80: 6c6f 7474 696e 6729 0d0a 0909 5468 6520  lotting)....The 
+00053b90: 706c 6f74 7320 6172 6520 6765 6e65 7261  plots are genera
+00053ba0: 7465 6420 6672 6f6d 2074 6865 2066 6974  ted from the fit
+00053bb0: 7465 6420 4d61 7472 6978 6573 2061 6e64  ted Matrixes and
+00053bc0: 2061 7320 7375 6368 206f 6e6c 7920 7769   as such only wi
+00053bd0: 6c6c 2077 6f72 6b20 6166 7465 7220 6120  ll work after a 
+00053be0: 6669 7420 7761 7320 6163 7475 616c 6c79  fit was actually
+00053bf0: 0d0a 0909 636f 6d70 6c65 7465 6420 2861  ....completed (a
+00053c00: 6e64 2074 6865 2022 7265 2220 6469 6374  nd the "re" dict
+00053c10: 696f 6e61 7279 2061 7474 6163 6865 6420  ionary attached 
+00053c20: 746f 2074 6865 206f 626a 6563 742e 290d  to the object.).
+00053c30: 0a09 0949 6e20 616c 6c20 706c 6f74 7320  ...In all plots 
+00053c40: 7468 6520 5241 5720 6461 7461 2069 7320  the RAW data is 
+00053c50: 706c 6f74 7465 6420 6173 2064 6f74 7320  plotted as dots 
+00053c60: 616e 6420 7468 6520 6669 7420 7769 7468  and the fit with
+00053c70: 206c 696e 6573 200d 0a09 090d 0a09 0943   lines ........C
+00053c80: 6f6e 7465 6e74 7320 6f66 2074 6865 2070  ontents of the p
+00053c90: 6c6f 7473 0d0a 0d0a 0909 0930 2e20 4441  lots.......0. DA
+00053ca0: 4320 636f 6e74 6169 6e73 2074 6865 2061  C contains the a
+00053cb0: 7373 6967 6e65 6420 7370 6563 7472 6120  ssigned spectra 
+00053cc0: 666f 7220 6561 6368 2063 6f6d 706f 6e65  for each compone
+00053cd0: 6e74 206f 6620 7468 6520 6669 742e 2046  nt of the fit. F
+00053ce0: 6f72 0d0a 0909 0920 2020 6120 6d6f 6465  or.....   a mode
+00053cf0: 6c6c 696e 6720 7769 7468 2069 6e64 6570  lling with indep
+00053d00: 656e 6465 6e74 2065 7870 6f6e 656e 7469  endent exponenti
+00053d10: 616c 2064 6563 6179 7320 7468 6973 2063  al decays this c
+00053d20: 6f72 7265 7370 6f6e 6473 2074 6f0d 0a09  orresponds to...
+00053d30: 0909 2020 2074 6865 2022 4465 6361 7920  ..   the "Decay 
+00053d40: 4173 736f 6369 6174 6564 2053 7065 6374  Associated Spect
+00053d50: 7261 2220 2844 4153 292e 2046 6f72 2061  ra" (DAS). For a
+00053d60: 6c6c 206f 7468 6572 206d 6f64 656c 7320  ll other models 
+00053d70: 7468 6973 0d0a 0909 0920 2020 636f 6e74  this.....   cont
+00053d80: 6169 6e73 2074 6865 2022 5370 6563 6965  ains the "Specie
+00053d90: 7320 4173 736f 6369 6174 6564 2053 7065  s Associated Spe
+00053da0: 6374 7261 2220 2853 4153 292e 2041 6363  ctra" (SAS). Acc
+00053db0: 6f72 6469 6e67 2074 6f20 7468 650d 0a09  ording to the...
+00053dc0: 0909 2020 206d 6f64 656c 2074 6865 2073  ..   model the s
+00053dd0: 6570 6172 6174 6520 7370 6563 7472 6120  eparate spectra 
+00053de0: 6172 6520 6c61 6265 6c65 6420 6279 2074  are labeled by t
+00053df0: 696d 6520 2870 726f 6365 7373 2920 6f72  ime (process) or
+00053e00: 206e 616d 652c 2069 660d 0a09 0909 2020   name, if.....  
+00053e10: 2061 206e 616d 6520 6973 2061 7373 6f63   a name is assoc
+00053e20: 6961 7465 6420 696e 2074 6865 2066 6974  iated in the fit
+00053e30: 7469 6e67 206d 6f64 656c 2e20 5468 6520  ting model. The 
+00053e40: 7370 6563 7472 6120 6172 6520 7368 6f77  spectra are show
+00053e50: 6e20 696e 0d0a 0909 0920 2020 7468 6520  n in.....   the 
+00053e60: 6578 7472 6163 7465 6420 7374 7265 6e67  extracted streng
+00053e70: 7468 2069 6e20 7468 6520 7269 6768 7420  th in the right 
+00053e80: 7061 6e65 2061 6e64 206e 6f72 6d61 6c69  pane and normali
+00053e90: 7a65 6420 696e 2074 6865 206c 6566 742e  zed in the left.
+00053ea0: 0d0a 0909 0920 2020 4578 7472 6163 7465  .....   Extracte
+00053eb0: 6420 7374 7265 6e67 7468 206d 6561 6e73  d strength means
+00053ec0: 2074 6861 7420 7468 6520 6d65 6173 7572   that the measur
+00053ed0: 6564 2073 7065 6374 7261 6c20 7374 7265  ed spectral stre
+00053ee0: 6e67 7468 2069 7320 7468 650d 0a09 0909  ngth is the.....
+00053ef0: 2020 2069 6e74 656e 7369 7479 2028 636f     intensity (co
+00053f00: 6e63 656e 7472 6174 696f 6e20 6d61 7472  ncentration matr
+00053f10: 6978 2920 7469 6d65 7320 7468 6973 2073  ix) times this s
+00053f20: 7065 6374 7261 6c20 7374 7265 6e67 7468  pectral strength
+00053f30: 2e20 4173 2074 6865 0d0a 0909 0920 2020  . As the.....   
+00053f40: 636f 6e63 656e 7472 6174 696f 6e20 6d61  concentration ma
+00053f50: 7869 6d61 2066 6f72 2061 6c6c 2044 4153  xima for all DAS
+00053f60: 2061 7265 2031 2074 6869 7320 636f 7272   are 1 this corr
+00053f70: 6573 706f 6e64 7320 746f 2074 6865 0d0a  esponds to the..
+00053f80: 0909 0920 2020 7370 6563 7472 616c 2073  ...   spectral s
+00053f90: 7472 656e 6774 6820 666f 7220 7468 6520  trength for the 
+00053fa0: 4441 532e 2028 706c 6561 7365 2073 6565  DAS. (please see
+00053fb0: 2074 6865 2064 6f63 756d 656e 7461 7469   the documentati
+00053fc0: 6f6e 2066 6f72 2074 6865 0d0a 0909 0920  on for the..... 
+00053fd0: 2020 6669 7474 696e 6720 616c 676f 7269    fitting algori
+00053fe0: 7468 6d20 666f 7220 6675 7274 6865 7220  thm for further 
+00053ff0: 6465 7461 696c 7329 2e0d 0a0d 0a09 0909  details)........
+00054000: 312e 2073 756d 6d65 6420 696e 7465 6e73  1. summed intens
+00054010: 6974 792e 2041 6c6c 2077 6176 656c 656e  ity. All wavelen
+00054020: 6774 6820 6f66 2074 6865 2073 7065 6374  gth of the spect
+00054030: 7261 6c20 6178 6973 2061 7265 2073 756d  ral axis are sum
+00054040: 6d65 6420 666f 720d 0a09 0909 2020 2064  med for.....   d
+00054050: 6174 6120 616e 6420 6669 742e 2054 6865  ata and fit. The
+00054060: 2064 6174 6120 6973 2070 6c6f 7474 6564   data is plotted
+00054070: 2069 6e20 6120 6e75 6d62 6572 206f 6620   in a number of 
+00054080: 7761 7973 2076 7320 6c69 6e65 6172 2061  ways vs linear a
+00054090: 6e64 0d0a 0909 0920 2020 6c6f 6761 7269  nd.....   logari
+000540a0: 7468 6d69 6320 6178 6973 2e20 5468 6973  thmic axis. This
+000540b0: 2070 6c6f 7420 6973 206e 6f74 206d 656e   plot is not men
+000540c0: 7420 666f 7220 7075 626c 6963 6174 696f  t for publicatio
+000540d0: 6e20 6275 7420 7665 7279 0d0a 0909 0920  n but very..... 
+000540e0: 2020 7573 6566 756c 2074 6f20 6576 616c    useful to eval
+000540f0: 7561 7465 2074 6865 2071 7561 6c69 7479  uate the quality
+00054100: 206f 6620 6120 6669 742e 0d0a 0d0a 0909   of a fit.......
+00054110: 0932 2e20 706c 6f74 206b 696e 6574 6963  .2. plot kinetic
+00054120: 7320 666f 7220 7365 6c65 6374 6564 2077  s for selected w
+00054130: 6176 656c 656e 6774 6820 2873 6565 2063  avelength (see c
+00054140: 6f72 7265 7370 6f6e 6469 6e67 2052 4157  orresponding RAW
+00054150: 2070 6c6f 7429 2e0d 0a0d 0a09 0909 332e   plot)........3.
+00054160: 2070 6c6f 7420 7370 6563 7472 6120 6174   plot spectra at
+00054170: 2073 656c 6563 7465 6420 7469 6d65 7320   selected times 
+00054180: 2873 6565 2063 6f72 7265 7370 6f6e 6469  (see correspondi
+00054190: 6e67 2052 4157 2070 6c6f 7429 2e0d 0a0d  ng RAW plot)....
+000541a0: 0a09 0909 342e 2070 6c6f 7473 206d 6174  ....4. plots mat
+000541b0: 7269 7820 286d 6561 7375 7265 642c 206d  rix (measured, m
+000541c0: 6f64 656c 6c65 6420 616e 6420 6572 726f  odelled and erro
+000541d0: 7220 4d61 7472 6978 292e 2054 6865 2070  r Matrix). The p
+000541e0: 6172 616d 6574 6572 2061 7265 0d0a 0909  arameter are....
+000541f0: 0920 2020 7468 6520 7361 6d65 2061 7320  .   the same as 
+00054200: 7573 6564 2066 6f72 2074 6865 2063 6f72  used for the cor
+00054210: 7265 7370 6f6e 6469 6e67 2052 4157 2070  responding RAW p
+00054220: 6c6f 7420 7769 7468 2074 6865 2061 6464  lot with the add
+00054230: 6974 696f 6e20 6f66 0d0a 0909 0920 2020  ition of.....   
+00054240: 2265 7272 6f72 5f6d 6174 7269 785f 616d  "error_matrix_am
+00054250: 706c 6966 6963 6174 696f 6e22 2077 6869  plification" whi
+00054260: 6368 2069 7320 6120 7363 616c 696e 6720  ch is a scaling 
+00054270: 6661 6374 6f72 206d 756c 7469 706c 6965  factor multiplie
+00054280: 640d 0a09 0909 2020 206f 6e74 6f20 7468  d.....   onto th
+00054290: 6520 6572 726f 7220 6d61 7472 6978 2e20  e error matrix. 
+000542a0: 4920 7265 636f 6d6d 656e 6420 746f 2070  I recommend to p
+000542b0: 6c61 7920 7769 7468 2064 6966 6665 7265  lay with differe
+000542c0: 6e74 2022 636d 6170 222c 0d0a 0909 0920  nt "cmap",..... 
+000542d0: 2020 226c 6f67 5f73 6361 6c65 2220 616e    "log_scale" an
+000542e0: 6420 2269 6e74 656e 7369 7479 5f73 6361  d "intensity_sca
+000542f0: 6c65 2220 746f 2063 7265 6174 6520 6120  le" to create a 
+00054300: 706c 6561 7369 6e67 2070 6c6f 742e 0d0a  pleasing plot...
+00054310: 0d0a 0909 0935 2e20 636f 6e63 656e 7472  .....5. concentr
+00054320: 6174 696f 6e73 2e20 496e 2074 6865 2070  ations. In the p
+00054330: 726f 6772 6573 7320 6f66 2074 6865 206d  rogress of the m
+00054340: 6f64 656c 6c69 6e67 2f66 6974 7469 6e67  odelling/fitting
+00054350: 2061 206d 6174 7269 7820 6973 0d0a 0909   a matrix is....
+00054360: 0920 2020 6765 6e65 7261 7465 6420 7468  .   generated th
+00054370: 6174 2063 6f6e 7461 696e 7320 7468 6520  at contains the 
+00054380: 7265 6c61 7469 7665 2063 6f6e 6365 6e74  relative concent
+00054390: 7261 7469 6f6e 7320 6f66 2074 6865 2073  rations of the s
+000543a0: 7065 6369 6573 0d0a 0909 0920 2020 6d6f  pecies.....   mo
+000543b0: 6465 6c6c 6564 2e20 5468 6973 2070 6c6f  delled. This plo
+000543c0: 7420 6973 2073 686f 7769 6e67 2074 6865  t is showing the
+000543d0: 2074 656d 706f 7261 6c20 6465 7665 6c6f   temporal develo
+000543e0: 706d 656e 7420 6f66 2074 6865 7365 0d0a  pment of these..
+000543f0: 0909 0920 2020 7370 6563 6965 732e 2046  ...   species. F
+00054400: 7572 7468 6572 2064 6574 6169 6c73 206f  urther details o
+00054410: 6e20 686f 7720 7468 6973 206d 6174 7269  n how this matri
+00054420: 7820 6973 2067 656e 6572 6174 6564 2063  x is generated c
+00054430: 616e 2062 6520 666f 756e 640d 0a09 0909  an be found.....
+00054440: 2020 2069 6e20 7468 6520 646f 6375 6d65     in the docume
+00054450: 6e74 6174 696f 6e20 6f66 2074 6865 2066  ntation of the f
+00054460: 6974 7469 6e67 2066 756e 6374 696f 6e2e  itting function.
+00054470: 2054 6865 206d 6f64 656c 6564 2073 7065   The modeled spe
+00054480: 6374 7261 2061 7265 0d0a 0909 0920 2020  ctra are.....   
+00054490: 7468 6520 636f 6e76 6f6c 7574 696f 6e20  the convolution 
+000544a0: 6f66 2074 6865 7365 2076 6563 746f 7273  of these vectors
+000544b0: 2028 6769 7669 6e67 2074 6865 2074 696d   (giving the tim
+000544c0: 652d 6465 7665 6c6f 706d 656e 7429 2061  e-development) a
+000544d0: 6e64 0d0a 0909 0920 2020 7468 6520 4441  nd.....   the DA
+000544e0: 532f 5341 5320 2867 6976 696e 6720 7468  S/SAS (giving th
+000544f0: 6520 7370 6563 7472 616c 2064 6576 656c  e spectral devel
+00054500: 6f70 6d65 6e74 292e 0d0a 0909 0d0a 0909  opment).........
+00054510: 5061 7261 6d65 7465 7273 0d0a 0909 2d2d  Parameters....--
+00054520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a09  -------------...
+00054530: 090d 0a09 0970 6c6f 7474 696e 6720 3a20  .....plotting : 
+00054540: 696e 7420 6f72 2069 7465 7261 626c 6520  int or iterable 
+00054550: 286f 6620 696e 7465 6765 7273 292c 206f  (of integers), o
+00054560: 7074 696f 6e61 6c0d 0a09 0909 5468 6973  ptional.....This
+00054570: 2070 6172 616d 6574 6572 2064 6574 6572   parameter deter
+00054580: 6d69 6e65 7320 7768 6963 6820 6669 6775  mines which figu
+00054590: 7265 7320 6172 6520 706c 6f74 7465 6420  res are plotted 
+000545a0: 0d0a 0909 0974 6865 2066 6967 7572 6573  .....the figures
+000545b0: 2063 616e 2062 6520 6361 6c6c 6564 2073   can be called s
+000545c0: 6570 6172 6174 656c 7920 7769 7468 2070  eparately with p
+000545d0: 6c6f 7474 696e 6720 3d20 310d 0a09 0909  lotting = 1.....
+000545e0: 6f72 2077 6974 6820 6120 6c69 7374 206f  or with a list o
+000545f0: 6620 706c 6f74 7320 2844 6566 6175 6c74  f plots (Default
+00054600: 2920 652e 672e 2070 6c6f 7474 696e 673d  ) e.g. plotting=
+00054610: 7261 6e67 6528 3629 2063 616c 6c73 2070  range(6) calls p
+00054620: 6c6f 7473 2030 2c31 2c32 2c33 2c34 2c35  lots 0,1,2,3,4,5
+00054630: 0d0a 0909 0954 6865 2070 6c6f 7473 2068  .....The plots h
+00054640: 6176 6520 7468 6520 666f 6c6c 6f77 696e  ave the followin
+00054650: 6720 6e75 6d62 6572 733a 0d0a 0909 090d  g numbers:......
+00054660: 0a09 0909 0930 2e20 4441 5320 6f72 2053  .....0. DAS or S
+00054670: 4153 0d0a 0909 0909 312e 2073 756d 6d65  AS......1. summe
+00054680: 6420 696e 7465 6e73 6974 790d 0a09 0909  d intensity.....
+00054690: 0932 2e20 4b69 6e65 7469 6373 0d0a 0909  .2. Kinetics....
+000546a0: 0909 332e 2053 7065 6374 7261 0d0a 0909  ..3. Spectra....
+000546b0: 0909 342e 204d 6174 7269 7865 730d 0a09  ..4. Matrixes...
+000546c0: 0909 0935 2e20 436f 6e63 656e 7472 6174  ...5. Concentrat
+000546d0: 696f 6e73 2028 7468 6520 632d 6f62 6a65  ions (the c-obje
+000546e0: 6374 290d 0a09 0909 0d0a 0909 0954 6865  ct)..........The
+000546f0: 2070 6c6f 7474 696e 6720 7461 6b65 7320   plotting takes 
+00054700: 616c 6c20 7061 7261 6d65 7465 7220 6672  all parameter fr
+00054710: 6f6d 2074 6865 2022 7461 2220 6f62 6a65  om the "ta" obje
+00054720: 6374 2075 6e6c 6573 7320 6f74 6865 7277  ct unless otherw
+00054730: 6973 6520 7370 6563 6966 6965 640d 0a09  ise specified...
+00054740: 090d 0a09 0970 6174 6820 3a20 4e6f 6e65  .....path : None
+00054750: 2c20 7374 7220 6f72 2070 6174 6820 6f62  , str or path ob
+00054760: 6a65 6374 2c20 6f70 7469 6f6e 616c 0d0a  ject, optional..
+00054770: 0909 0954 6869 7320 6465 6669 6e65 7320  ...This defines 
+00054780: 7768 6572 6520 7468 6520 6669 6c65 7320  where the files 
+00054790: 6172 6520 7361 7665 6420 6966 2074 6865  are saved if the
+000547a0: 2073 6166 655f 6669 6775 7265 735f 746f   safe_figures_to
+000547b0: 5f66 6f6c 6465 7220 7061 7261 6d65 7465  _folder paramete
+000547c0: 7220 6973 2054 7275 652c 200d 0a09 0909  r is True, .....
+000547d0: 7175 6974 6520 7573 6566 756c 2069 6620  quite useful if 
+000547e0: 6120 6c6f 7420 6f66 2064 6174 6120 7365  a lot of data se
+000547f0: 7473 2061 7265 2074 6f20 6265 2070 7269  ts are to be pri
+00054800: 6e74 6564 2066 6173 742e 200d 0a09 0909  nted fast. .....
+00054810: 4966 2061 2070 6174 6820 6973 2067 6976  If a path is giv
+00054820: 656e 2c20 7468 6973 2069 7320 7573 6564  en, this is used
+00054830: 2e20 4966 2061 2073 7472 696e 6720 6c69  . If a string li
+00054840: 6b65 2074 6865 2028 4465 6661 756c 7429  ke the (Default)
+00054850: 2022 7265 7375 6c74 5f66 6967 7572 6573   "result_figures
+00054860: 2220 6973 2067 6976 656e 2c20 0d0a 0909  " is given, ....
+00054870: 0974 6865 6e20 6120 7375 6266 6f6c 6465  .then a subfolde
+00054880: 7220 6f66 2074 6869 7320 6e61 6d65 2077  r of this name w
+00054890: 696c 6c20 6265 2075 7365 6420 2861 6e20  ill be used (an 
+000548a0: 6765 6e65 7261 7465 6420 6966 206e 6563  generated if nec
+000548b0: 6573 7361 7279 2920 0d0a 0909 0972 656c  essary) .....rel
+000548c0: 6174 6976 6520 746f 2073 656c 662e 7061  ative to self.pa
+000548d0: 7468 2e20 5573 6520 616e 6420 656d 7074  th. Use and empt
+000548e0: 7920 7374 7269 6e67 2074 6f20 7573 6520  y string to use 
+000548f0: 7468 6520 7365 6c66 2e70 6174 680d 0a09  the self.path...
+00054900: 0909 4966 2073 6574 2074 6f20 4e6f 6e65  ..If set to None
+00054910: 2c20 7468 6520 6c6f 6361 7469 6f6e 206f  , the location o
+00054920: 6620 7468 6520 706c 6f74 5f66 756e 6320  f the plot_func 
+00054930: 7769 6c6c 2062 6520 7573 6564 2061 6e64  will be used and
+00054940: 0d0a 0909 0961 2073 7562 666f 6c64 6572  .....a subfolder
+00054950: 2077 6974 6820 7469 746c 6520 2272 6573   with title "res
+00054960: 756c 745f 6669 6775 7265 7322 2062 6520  ult_figures" be 
+00054970: 6765 6e65 7261 7465 6420 6865 7265 0d0a  generated here..
+00054980: 0909 0d0a 0909 7361 7665 7479 7065 203a  ......savetype :
+00054990: 2073 7472 206f 7220 6974 6572 6162 6c65   str or iterable
+000549a0: 2028 6f66 2073 7472 292c 206f 7074 696f   (of str), optio
+000549b0: 6e61 6c20 0d0a 0909 096d 6174 706c 6f74  nal .....matplot
+000549c0: 6c69 6220 616c 6c6f 7773 2074 6865 2073  lib allows the s
+000549d0: 6176 696e 6720 6f66 2066 6967 7572 6573  aving of figures
+000549e0: 2069 6e20 7661 7269 6f75 7320 666f 726d   in various form
+000549f0: 6174 732e 2028 4465 6661 756c 7429 2022  ats. (Default) "
+00054a00: 706e 6722 2c20 0d0a 0909 0974 7970 6963  png", .....typic
+00054a10: 616c 2061 6e64 2072 6563 6f6d 6d65 6e64  al and recommend
+00054a20: 6162 6c65 206f 7074 696f 6e73 2061 7265  able options are
+00054a30: 2022 7376 6722 2061 6e64 2022 7064 6622   "svg" and "pdf"
+00054a40: 2e20 200d 0a09 0909 0d0a 0909 6576 616c  .  .........eval
+00054a50: 7561 7469 6f6e 5f73 7479 6c65 203a 2062  uation_style : b
+00054a60: 6f6f 6c2c 206f 7074 696f 6e61 6c0d 0a09  ool, optional...
+00054a70: 0909 5472 7565 2028 4465 6661 756c 7420  ..True (Default 
+00054a80: 3d20 4661 6c73 6529 2061 6464 7320 6120  = False) adds a 
+00054a90: 6c6f 7420 6f66 2065 7874 7261 2069 6e66  lot of extra inf
+00054aa0: 6f72 6d61 7469 6f6e 2069 6e20 7468 6520  ormation in the 
+00054ab0: 706c 6f74 0d0a 0909 0d0a 0909 7469 746c  plot........titl
+00054ac0: 6520 3a20 4e6f 6e65 206f 7220 7374 722c  e : None or str,
+00054ad0: 206f 7074 696f 6e61 6c0d 0a09 0920 2020   optional....   
+00054ae0: 2274 6974 6c65 3d4e 6f6e 6522 2069 7320  "title=None" is 
+00054af0: 696e 2067 656e 6572 616c 2074 6865 2066  in general the f
+00054b00: 696c 656e 616d 6520 7468 6174 2077 6173  ilename that was
+00054b10: 206c 6f61 6465 642e 2053 6574 7469 6e67   loaded. Setting
+00054b20: 2061 0d0a 0909 2020 2073 7065 6369 6669   a....   specifi
+00054b30: 6320 7469 746c 6520 7769 6c6c 2062 6520  c title will be 
+00054b40: 7573 6564 2069 6e20 616c 6c20 706c 6f74  used in all plot
+00054b50: 732e 2054 6f20 7265 6d6f 7665 2074 6865  s. To remove the
+00054b60: 2074 6974 6c65 2061 6c6c 0d0a 0909 2020   title all....  
+00054b70: 2074 6f67 6574 6865 7220 7365 7420 616e   together set an
+00054b80: 2065 6d70 7479 2073 7472 696e 6720 7769   empty string wi
+00054b90: 7468 2074 6974 6c65 3d22 220d 0a09 0920  th title="".... 
+00054ba0: 2020 0d0a 0909 7363 616c 655f 7479 7065    ....scale_type
+00054bb0: 203a 2073 7472 2c20 6f70 7469 6f6e 616c   : str, optional
+00054bc0: 0d0a 0909 2020 2072 6566 6572 7320 746f  ....   refers to
+00054bd0: 2074 6865 2074 696d 652d 6178 6973 2061   the time-axis a
+00054be0: 6e64 2074 616b 6573 2c20 2273 796d 6c6f  nd takes, "symlo
+00054bf0: 6722 2028 4465 6661 756c 7429 286c 696e  g" (Default)(lin
+00054c00: 6561 7220 6172 6f75 6e64 207a 6572 6f20  ear around zero 
+00054c10: 616e 6420 6c6f 6761 7269 7468 6d69 6320  and logarithmic 
+00054c20: 6f74 6865 7277 6973 6529 0d0a 0909 2020  otherwise)....  
+00054c30: 2061 6e64 2022 6c69 6e22 2066 6f72 206c   and "lin" for l
+00054c40: 696e 6561 7220 616e 6420 2022 6c6f 6722  inear and  "log"
+00054c50: 2066 6f72 206c 6f67 6172 6974 686d 6963   for logarithmic
+00054c60: 2c20 7377 6974 6368 696e 6720 616c 6c20  , switching all 
+00054c70: 7468 6520 7469 6d65 2061 7869 7320 746f  the time axis to
+00054c80: 2074 6869 7320 7479 7065 0d0a 0909 0d0a   this type......
+00054c90: 0909 7061 7463 6865 7320 3a20 626f 6f6c  ..patches : bool
+00054ca0: 2c20 6f70 7469 6f6e 616c 0d0a 0909 0949  , optional.....I
+00054cb0: 6620 4661 6c73 6520 2844 6566 6175 6c74  f False (Default
+00054cc0: 2920 7468 6520 6e61 6d65 7320 226d 6561  ) the names "mea
+00054cd0: 7375 7265 6422 2022 6669 7474 6564 2220  sured" "fitted" 
+00054ce0: 2264 6966 6665 7265 6e63 6522 2077 696c  "difference" wil
+00054cf0: 6c20 6265 2070 6c61 6365 6420 6162 6f76  l be placed abov
+00054d00: 6520 7468 6520 696d 6167 6573 2e0d 0a09  e the images....
+00054d10: 0909 4966 2054 7275 652c 2074 6865 6e20  ..If True, then 
+00054d20: 7468 6579 2077 696c 6c20 6265 2069 6e63  they will be inc
+00054d30: 6c75 6465 6420 696e 746f 2074 6865 2069  luded into the i
+00054d40: 6d61 6765 2028 6465 6e73 6572 290d 0a0d  mage (denser)...
+00054d50: 0a09 0966 696c 656e 616d 6520 3a20 7374  ...filename : st
+00054d60: 722c 206f 7074 696f 6e61 6c0d 0a09 0909  r, optional.....
+00054d70: 6f66 6665 7273 2074 6f20 7265 706c 6163  offers to replac
+00054d80: 6520 7468 6520 6261 7365 2d6e 616d 6520  e the base-name 
+00054d90: 7573 6564 2066 6f72 2061 6c6c 2070 6c6f  used for all plo
+00054da0: 7473 2028 746f 2065 2e67 2e73 7065 6369  ts (to e.g.speci
+00054db0: 6679 2077 6861 7420 7361 6d70 6c65 2077  fy what sample w
+00054dc0: 6173 2075 7365 6429 2e20 0d0a 0909 0969  as used). .....i
+00054dd0: 6620 2844 6566 6175 6c74 2920 4e6f 6e65  f (Default) None
+00054de0: 2069 7320 7573 6564 2c20 7468 6520 7365   is used, the se
+00054df0: 6c66 2e66 696c 656e 616d 6520 6973 2075  lf.filename is u
+00054e00: 7365 6420 6173 2061 2062 6173 6520 6e61  sed as a base na
+00054e10: 6d65 2e20 5468 6520 6669 6c65 6e61 6d65  me. The filename
+00054e20: 2070 6c61 7973 206f 6e6c 7920 6120 0d0a   plays only a ..
+00054e30: 0909 0972 6f6c 6520 6475 7269 6e67 2073  ...role during s
+00054e40: 6176 696e 672c 2061 7320 646f 6573 2074  aving, as does t
+00054e50: 6865 2070 6174 6820 616e 6420 7361 7665  he path and save
+00054e60: 7479 7065 090d 0a09 0909 0d0a 0909 636d  type..........cm
+00054e70: 6170 203a 204e 6f6e 6520 6f72 206d 6174  ap : None or mat
+00054e80: 706c 6f74 6c69 6220 636f 6c6f 7220 6d61  plotlib color ma
+00054e90: 702c 206f 7074 696f 6e61 6c0d 0a09 0909  p, optional.....
+00054ea0: 6973 2061 2070 6f77 6572 6675 6c6c 2076  is a powerfull v
+00054eb0: 6172 6961 626c 6520 7468 6174 2063 686f  ariable that cho
+00054ec0: 6f73 6573 2074 6865 2063 6f6c 6f75 7220  oses the colour 
+00054ed0: 6d61 7020 6170 706c 6965 6420 666f 7220  map applied for 
+00054ee0: 616c 6c20 706c 6f74 732e 2049 6620 7365  all plots. If se
+00054ef0: 7420 746f 200d 0a09 0909 4e6f 6e65 2028  t to .....None (
+00054f00: 4465 6661 756c 7429 2074 6865 6e20 7468  Default) then th
+00054f10: 6520 7365 6c66 2e63 6d61 7020 6973 2075  e self.cmap is u
+00054f20: 7365 642e 0d0a 0909 0941 7320 7374 616e  sed......As stan
+00054f30: 6461 7264 2049 2075 7365 2074 6865 2063  dard I use the c
+00054f40: 6f6c 6f72 206d 6170 2022 6a65 7422 2066  olor map "jet" f
+00054f50: 726f 6d20 6d61 7470 6c6f 746c 6962 2e20  rom matplotlib. 
+00054f60: 5468 6572 6520 6172 6520 6120 7661 7269  There are a vari
+00054f70: 6574 7920 6f66 2063 6f6c 6f72 6d61 7073  ety of colormaps
+00054f80: 200d 0a09 0909 6176 6169 6c61 626c 6520   .....available 
+00054f90: 7468 6174 2061 7265 2076 6572 7920 7573  that are very us
+00054fa0: 6566 756c 6c2e 2042 6573 6964 6520 226a  efull. Beside "j
+00054fb0: 6574 222c 2022 7669 7269 6469 7322 2069  et", "viridis" i
+00054fc0: 7320 6120 676f 6f64 2063 686f 6963 6520  s a good choice 
+00054fd0: 6173 2069 7420 6973 2077 656c 6c20 0d0a  as it is well ..
+00054fe0: 0909 0976 6973 6962 6c65 2075 6e64 6572  ...visible under
+00054ff0: 2072 6564 2d67 7265 656e 2062 6c69 6e64   red-green blind
+00055000: 6e65 7373 2e20 4f74 6865 7220 7573 6566  ness. Other usef
+00055010: 756c 206d 6170 7320 6172 6520 2270 7269  ul maps are "pri
+00055020: 736d 2220 666f 7220 6869 6768 2066 6c75  sm" for high flu
+00055030: 6374 7561 7469 6f6e 7320 0d0a 0909 096f  ctuations .....o
+00055040: 7220 6469 7665 7267 696e 6720 636f 6c6f  r diverging colo
+00055050: 7220 6d61 7073 206c 696b 6520 2273 6569  r maps like "sei
+00055060: 736d 6963 222e 200d 0a09 0909 5365 6520  smic". .....See 
+00055070: 6874 7470 733a 2f2f 6d61 7470 6c6f 746c  https://matplotl
+00055080: 6962 2e6f 7267 2f33 2e31 2e30 2f74 7574  ib.org/3.1.0/tut
+00055090: 6f72 6961 6c73 2f63 6f6c 6f72 732f 636f  orials/colors/co
+000550a0: 6c6f 726d 6170 732e 6874 6d6c 2066 6f72  lormaps.html for
+000550b0: 2061 2063 6f6d 7072 6568 656e 7369 7665   a comprehensive
+000550c0: 200d 0a09 0909 7365 6c65 6374 696f 6e2e   .....selection.
+000550d0: 2049 6e20 7468 6520 636f 6465 2074 6865   In the code the
+000550e0: 2063 6f6c 6f72 6d61 7073 2061 7265 2069   colormaps are i
+000550f0: 6d70 6f72 7465 6420 736f 2069 6620 706c  mported so if pl
+00055100: 6f74 5f66 756e 6320 6973 2069 6d70 6f72  ot_func is impor
+00055110: 7465 6420 6173 2070 6620 7468 656e 200d  ted as pf then .
+00055120: 0a09 0909 7365 6c66 2e63 6d61 703d 7066  ....self.cmap=pf
+00055130: 2e63 6d2e 7669 7269 6469 7320 7365 7473  .cm.viridis sets
+00055140: 2076 6972 6964 6973 2061 7320 7468 6520   viridis as the 
+00055150: 6d61 7020 746f 2075 7365 2e20 496e 7465  map to use. Inte
+00055160: 726e 616c 6c79 2074 6865 2063 6f6c 6f72  rnally the color
+00055170: 7320 6172 6520 6368 6f73 656e 200d 0a09  s are chosen ...
+00055180: 0909 7769 7468 2074 6865 2022 636f 6c6d  ..with the "colm
+00055190: 2220 6675 6e63 7469 6f6e 2e20 5468 6520  " function. The 
+000551a0: 3264 2070 6c6f 7473 2072 6571 7569 7265  2d plots require
+000551b0: 2061 2063 6f6e 7469 6e75 6f75 7320 636f   a continuous co
+000551c0: 6c6f 7220 6d61 7020 736f 2069 6620 736f  lor map so if so
+000551d0: 6d65 7468 696e 6720 0d0a 0909 0965 6c73  mething .....els
+000551e0: 6520 6973 2067 6976 6520 3264 2070 6c6f  e is give 2d plo
+000551f0: 7473 2061 7265 2073 686f 776e 2061 7574  ts are shown aut
+00055200: 6f6d 6174 6963 616c 6c79 2077 6974 6820  omatically with 
+00055210: 226a 6574 222e 2046 6f72 2061 6c6c 206f  "jet". For all o
+00055220: 6620 7468 6520 3164 2070 6c6f 7473 2068  f the 1d plots h
+00055230: 6f77 6576 6572 200d 0a09 0909 4920 6669  owever .....I fi
+00055240: 7273 7420 7365 6c65 6374 2061 206e 756d  rst select a num
+00055250: 6265 7220 6f66 2063 6f6c 6f72 7320 6265  ber of colors be
+00055260: 666f 7265 2065 6163 6820 706c 6f74 2e20  fore each plot. 
+00055270: 4966 2063 6d61 7020 6973 2061 2063 6f6e  If cmap is a con
+00055280: 7469 6e6f 7573 206d 6170 2074 6865 6e20  tinous map then 
+00055290: 7468 6573 650d 0a09 0909 6172 6520 7361  these.....are sa
+000552a0: 6d70 6c65 6420 6576 656e 6c79 206f 7665  mpled evenly ove
+000552b0: 7220 7468 6520 636f 6c6f 7572 6d61 702e  r the colourmap.
+000552c0: 204d 616e 7561 6c20 6974 6572 6162 6c65   Manual iterable
+000552d0: 7320 6f66 2063 6f6c 6f75 7273 200d 0a09  s of colours ...
+000552e0: 0909 636d 6170 3d5b 2831 2c30 2c30 292c  ..cmap=[(1,0,0),
+000552f0: 2830 2c31 2c30 292c 2830 2c30 2c31 292c  (0,1,0),(0,0,1),
+00055300: 2e2e 2e5d 2061 7265 2061 6c73 6f20 6163  ...] are also ac
+00055310: 6365 7074 6564 2c20 6173 2061 7265 2076  cepted, as are v
+00055320: 6563 746f 7273 206f 7220 6461 7461 6672  ectors or datafr
+00055330: 616d 6573 2074 6861 7420 0d0a 0909 0963  ames that .....c
+00055340: 6f6e 7461 696e 2061 7320 726f 7773 2074  ontain as rows t
+00055350: 6865 2063 6f6c 6f72 732e 2054 6865 7265  he colors. There
+00055360: 206d 7573 7420 6265 206f 6620 636f 7572   must be of cour
+00055370: 7365 2073 7566 6669 6369 656e 7420 636f  se sufficient co
+00055380: 6c6f 7273 2070 7265 7365 6e74 2066 6f72  lors present for
+00055390: 200d 0a09 0909 7468 6520 6e75 6d62 6572   .....the number
+000553a0: 7320 6f66 206c 696e 6573 2074 6861 7420  s of lines that 
+000553b0: 7769 6c6c 2062 6520 706c 6f74 7465 642e  will be plotted.
+000553c0: 2053 6f20 4920 7265 636f 6d6d 656e 6420   So I recommend 
+000553d0: 746f 2070 726f 7669 6465 2061 7420 6c65  to provide at le
+000553e0: 6173 7420 3130 2063 6f6c 6f75 7273 200d  ast 10 colours .
+000553f0: 0a09 0909 2865 2e67 2e79 6f75 7220 756e  ....(e.g.your un
+00055400: 6976 6572 7369 7479 2063 6f6c 6f72 7329  iversity colors)
+00055410: 2e20 636f 6c6f 7572 7320 6172 6520 616c  . colours are al
+00055420: 7761 7973 2067 6976 656e 2061 7320 612c  ways given as a,
+00055430: 206c 6973 7420 6f72 2074 7570 6c65 2077   list or tuple w
+00055440: 6974 6820 5247 4120 6f72 2052 4742 410d  ith RGA or RGBA.
+00055450: 0a09 0909 2877 6974 6820 7468 6520 6c61  ....(with the la
+00055460: 7374 2041 2062 6565 696e 6720 7468 6520  st A beeing the 
+00055470: 416c 7068 613d 7472 616e 7370 6172 656e  Alpha=transparen
+00055480: 6379 2e20 416c 6c20 6e75 6d62 6572 7320  cy. All numbers 
+00055490: 6172 6520 6265 7477 6565 6e20 3020 616e  are between 0 an
+000554a0: 6420 312e 200d 0a09 0909 4966 2061 206c  d 1. .....If a l
+000554b0: 6973 742f 7665 6374 6f72 2f44 6174 6146  ist/vector/DataF
+000554c0: 7261 6d65 2069 7320 6769 7665 6e20 666f  rame is given fo
+000554d0: 7220 7468 6520 636f 6c6f 7572 7320 7468  r the colours th
+000554e0: 6579 2077 696c 6c20 6265 2075 7365 6420  ey will be used 
+000554f0: 696e 2074 6865 206f 7264 6572 2070 726f  in the order pro
+00055500: 7669 6465 642e 0909 0d0a 0909 0d0a 0909  vided...........
+00055510: 7072 696e 745f 636c 6963 6b5f 706f 7369  print_click_posi
+00055520: 7469 6f6e 203a 2062 6f6f 6c2c 206f 7074  tion : bool, opt
+00055530: 696f 6e61 6c0d 0a09 0909 6966 2054 7275  ional.....if Tru
+00055540: 6520 7468 656e 2074 6865 2063 6c69 636b  e then the click
+00055550: 2070 6f73 6974 696f 6e20 6973 2070 7269   position is pri
+00055560: 6e74 6564 2066 6f72 2074 6865 2073 7065  nted for the spe
+00055570: 6374 7261 6c20 706c 6f74 7320 0d0a 0909  ctral plots ....
+00055580: 0d0a 0909 4578 616d 706c 6573 0d0a 0909  ....Examples....
+00055590: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 0909  ------------....
+000555a0: 0d0a 0909 5479 7069 6361 6c6c 7920 6f6e  ....Typically on
+000555b0: 6520 776f 756c 6420 6361 6c6c 2074 6869  e would call thi
+000555c0: 7320 6675 6e63 7469 6f6e 2065 6d70 7479  s function empty
+000555d0: 2066 6f72 2061 6e20 6f76 6572 7669 6577   for an overview
+000555e0: 3a0d 0a09 0941 6674 6572 2074 6865 206d  :....After the m
+000555f0: 696e 696d 756d 2066 6974 0d0a 0909 0d0a  inimum fit......
+00055600: 0909 3e3e 3e20 7461 3d70 662e 5441 2827  ..>>> ta=pf.TA('
+00055610: 7465 7374 6669 6c65 2e53 4941 2729 0d0a  testfile.SIA')..
+00055620: 0909 3e3e 3e20 7461 2e70 6172 3d6c 6d66  ..>>> ta.par=lmf
+00055630: 6974 2e50 6172 616d 6574 6572 7328 290d  it.Parameters().
+00055640: 0a09 093e 3e3e 2074 612e 7061 722e 6164  ...>>> ta.par.ad
+00055650: 6428 276b 3027 2c76 616c 7565 3d31 2f30  d('k0',value=1/0
+00055660: 2e31 2c76 6172 793d 5472 7565 290d 0a09  .1,vary=True)...
+00055670: 093e 3e3e 2074 612e 4669 745f 476c 6f62  .>>> ta.Fit_Glob
+00055680: 616c 2829 0d0a 0909 0d0a 0909 4f6e 6520  al()........One 
+00055690: 7573 7561 6c6c 7920 706c 6f74 7320 7468  usually plots th
+000556a0: 6520 616e 206f 7665 7276 6965 770d 0a09  e an overview...
+000556b0: 090d 0a09 093e 3e3e 2074 612e 506c 6f74  .....>>> ta.Plot
+000556c0: 5f66 6974 5f6f 7574 7075 7428 290d 0a09  _fit_output()...
+000556d0: 093e 3e3e 2074 612e 506c 6f74 5f66 6974  .>>> ta.Plot_fit
+000556e0: 5f6f 7574 7075 7428 706c 6f74 7469 6e67  _output(plotting
+000556f0: 3d72 616e 6765 2836 2929 2023 6973 2074  =range(6)) #is t
+00055700: 6865 2073 616d 6520 6173 2062 6566 6f72  he same as befor
+00055710: 650d 0a09 093e 3e3e 2074 612e 506c 6f74  e....>>> ta.Plot
+00055720: 5f66 6974 5f6f 7574 7075 7428 3229 2023  _fit_output(2) #
+00055730: 776f 756c 6420 706c 6f74 206f 6e6c 7920  would plot only 
+00055740: 7468 6520 6b69 6e65 7469 6373 0d0a 0909  the kinetics....
+00055750: 3e3e 3e20 7461 2e50 6c6f 745f 6669 745f  >>> ta.Plot_fit_
+00055760: 6f75 7470 7574 2870 6c6f 7474 696e 6720  output(plotting 
+00055770: 3d20 3229 2023 776f 756c 6420 706c 6f74  = 2) #would plot
+00055780: 206f 6e6c 7920 7468 6520 6b69 6e65 7469   only the kineti
+00055790: 6373 0d0a 0909 0909 0d0a 0d0a 0909 2727  cs............''
+000557a0: 270d 0a09 0974 7279 3a0d 0a09 0909 7265  '....try:.....re
+000557b0: 3d73 656c 662e 7265 0d0a 0909 6578 6365  =self.re....exce
+000557c0: 7074 3a0d 0a09 0909 7072 696e 7428 2757  pt:.....print('W
+000557d0: 6520 6e65 6564 2074 6f20 6861 7665 2066  e need to have f
+000557e0: 6974 7465 6420 736f 6d65 7468 696e 6720  itted something 
+000557f0: 736f 2074 6861 7420 7765 2063 616e 2070  so that we can p
+00055800: 6c6f 7427 290d 0a09 0909 7265 7475 726e  lot').....return
+00055810: 2046 616c 7365 0d0a 0909 7061 7468 3d63   False....path=c
+00055820: 6865 636b 5f66 6f6c 6465 7228 7061 7468  heck_folder(path
+00055830: 3d70 6174 682c 6375 7272 656e 745f 7061  =path,current_pa
+00055840: 7468 3d73 656c 662e 7061 7468 290d 0a09  th=self.path)...
+00055850: 0969 6620 7365 6c66 2e73 6176 655f 6669  .if self.save_fi
+00055860: 6775 7265 735f 746f 5f66 6f6c 6465 723a  gures_to_folder:
+00055870: 0d0a 0909 0973 656c 662e 6669 6775 7265  .....self.figure
+00055880: 5f70 6174 683d 7061 7468 0d0a 0909 6966  _path=path....if
+00055890: 2063 6d61 7020 6973 204e 6f6e 653a 636d   cmap is None:cm
+000558a0: 6170 3d73 656c 662e 636d 6170 0d0a 0909  ap=self.cmap....
+000558b0: 6966 2066 696c 656e 616d 6520 6973 204e  if filename is N
+000558c0: 6f6e 653a 6669 6c65 6e61 6d65 3d73 656c  one:filename=sel
+000558d0: 662e 6669 6c65 6e61 6d65 0d0a 0909 6966  f.filename....if
+000558e0: 2074 6974 6c65 2069 7320 4e6f 6e65 3a0d   title is None:.
+000558f0: 0a09 0909 6966 2066 696c 656e 616d 6520  ....if filename 
+00055900: 6973 204e 6f6e 653a 0d0a 0909 0909 7469  is None:......ti
+00055910: 746c 653d 7365 6c66 2e66 696c 656e 616d  tle=self.filenam
+00055920: 650d 0a09 0909 656c 7365 3a0d 0a09 0909  e.....else:.....
+00055930: 0974 6974 6c65 3d66 696c 656e 616d 650d  .title=filename.
+00055940: 0a09 0969 6620 6e6f 7420 6861 7361 7474  ...if not hasatt
+00055950: 7228 706c 6f74 7469 6e67 2c22 5f5f 6974  r(plotting,"__it
+00055960: 6572 5f5f 2229 3a70 6c6f 7474 696e 673d  er__"):plotting=
+00055970: 5b70 6c6f 7474 696e 675d 0d0a 0909 706c  [plotting]....pl
+00055980: 6f74 5f66 6974 5f6f 7574 7075 7428 7365  ot_fit_output(se
+00055990: 6c66 2e72 652c 2073 656c 662e 6473 2c20  lf.re, self.ds, 
+000559a0: 636d 6170 203d 2073 656c 662e 636d 6170  cmap = self.cmap
+000559b0: 2c20 706c 6f74 7469 6e67 203d 2070 6c6f  , plotting = plo
+000559c0: 7474 696e 672c 2074 6974 6c65 203d 2074  tting, title = t
+000559d0: 6974 6c65 2c20 0d0a 0909 0909 0909 7061  itle, ........pa
+000559e0: 7468 203d 2070 6174 682c 2066 203d 2066  th = path, f = f
+000559f0: 696c 656e 616d 652c 2069 6e74 656e 7369  ilename, intensi
+00055a00: 7479 5f72 616e 6765 203d 2073 656c 662e  ty_range = self.
+00055a10: 696e 7465 6e73 6974 795f 7261 6e67 652c  intensity_range,
+00055a20: 200d 0a09 0909 0909 096c 6f67 5f73 6361   ........log_sca
+00055a30: 6c65 203d 2073 656c 662e 6c6f 675f 7363  le = self.log_sc
+00055a40: 616c 652c 2062 6173 6575 6e69 7420 3d20  ale, baseunit = 
+00055a50: 7365 6c66 2e62 6173 6575 6e69 742c 2074  self.baseunit, t
+00055a60: 696d 656c 696d 6974 7320 3d20 7365 6c66  imelimits = self
+00055a70: 2e74 696d 656c 696d 6974 732c 200d 0a09  .timelimits, ...
+00055a80: 0909 0909 0973 6361 7474 6572 6375 7420  .....scattercut 
+00055a90: 3d20 7365 6c66 2e73 6361 7474 6572 6375  = self.scattercu
+00055aa0: 742c 2062 6f72 6465 7263 7574 203d 2073  t, bordercut = s
+00055ab0: 656c 662e 626f 7264 6572 6375 742c 200d  elf.bordercut, .
+00055ac0: 0a09 0909 0909 0965 7272 6f72 5f6d 6174  .......error_mat
+00055ad0: 7269 785f 616d 706c 6966 6963 6174 696f  rix_amplificatio
+00055ae0: 6e20 3d20 7365 6c66 2e65 7272 6f72 5f6d  n = self.error_m
+00055af0: 6174 7269 785f 616d 706c 6966 6963 6174  atrix_amplificat
+00055b00: 696f 6e2c 200d 0a09 0909 0909 0977 6176  ion, ........wav
+00055b10: 655f 6e6d 5f62 696e 203d 2073 656c 662e  e_nm_bin = self.
+00055b20: 7761 7665 5f6e 6d5f 6269 6e2c 2072 656c  wave_nm_bin, rel
+00055b30: 5f77 6176 6520 3d20 7365 6c66 2e72 656c  _wave = self.rel
+00055b40: 5f77 6176 652c 2077 6964 7468 203d 2073  _wave, width = s
+00055b50: 656c 662e 7761 7665 6c65 6e67 7468 5f62  elf.wavelength_b
+00055b60: 696e 2c20 0d0a 0909 0909 0909 7265 6c5f  in, ........rel_
+00055b70: 7469 6d65 203d 2073 656c 662e 7265 6c5f  time = self.rel_
+00055b80: 7469 6d65 2c20 7361 7665 5f66 6967 7572  time, save_figur
+00055b90: 6573 5f74 6f5f 666f 6c64 6572 203d 2073  es_to_folder = s
+00055ba0: 656c 662e 7361 7665 5f66 6967 7572 6573  elf.save_figures
+00055bb0: 5f74 6f5f 666f 6c64 6572 2c20 0d0a 0909  _to_folder, ....
+00055bc0: 0909 0909 6c6f 675f 6669 7420 3d20 7365  ....log_fit = se
+00055bd0: 6c66 2e6c 6f67 5f66 6974 2c6d 6f64 203d  lf.log_fit,mod =
+00055be0: 2073 656c 662e 6d6f 642c 2073 6176 6574   self.mod, savet
+00055bf0: 7970 6520 3d20 7361 7665 7479 7065 2c20  ype = savetype, 
+00055c00: 0d0a 0909 0909 0909 7469 6d65 5f77 6964  ........time_wid
+00055c10: 7468 5f70 6572 6365 6e74 203d 2073 656c  th_percent = sel
+00055c20: 662e 7469 6d65 5f77 6964 7468 5f70 6572  f.time_width_per
+00055c30: 6365 6e74 2c20 6576 616c 7561 7469 6f6e  cent, evaluation
+00055c40: 5f73 7479 6c65 203d 2065 7661 6c75 6174  _style = evaluat
+00055c50: 696f 6e5f 7374 796c 652c 200d 0a09 0909  ion_style, .....
+00055c60: 0909 0966 696c 656e 616d 6520 3d20 7365  ...filename = se
+00055c70: 6c66 2e66 696c 656e 616d 652c 2073 6361  lf.filename, sca
+00055c80: 6c65 5f74 7970 6520 3d20 7363 616c 655f  le_type = scale_
+00055c90: 7479 7065 2c20 7061 7463 6865 7320 3d20  type, patches = 
+00055ca0: 7061 7463 6865 732c 206c 696e 7472 6573  patches, lintres
+00055cb0: 6820 3d20 7365 6c66 2e6c 696e 7472 6573  h = self.lintres
+00055cc0: 682c 0d0a 0909 0909 0909 7072 696e 745f  h,........print_
+00055cd0: 636c 6963 6b5f 706f 7369 7469 6f6e 203d  click_position =
+00055ce0: 2070 7269 6e74 5f63 6c69 636b 5f70 6f73   print_click_pos
+00055cf0: 6974 696f 6e2c 2069 676e 6f72 655f 7469  ition, ignore_ti
+00055d00: 6d65 5f72 6567 696f 6e20 3d20 7365 6c66  me_region = self
+00055d10: 2e69 676e 6f72 655f 7469 6d65 5f72 6567  .ignore_time_reg
+00055d20: 696f 6e2c 0d0a 0909 0909 0909 6461 7461  ion,........data
+00055d30: 5f74 7970 6520 3d20 7365 6c66 2e64 6174  _type = self.dat
+00055d40: 615f 7479 7065 2c20 706c 6f74 5f73 6563  a_type, plot_sec
+00055d50: 6f6e 645f 6173 5f65 6e65 7267 7920 3d20  ond_as_energy = 
+00055d60: 706c 6f74 5f73 6563 6f6e 645f 6173 5f65  plot_second_as_e
+00055d70: 6e65 7267 792c 2075 6e69 7473 3d20 7365  nergy, units= se
+00055d80: 6c66 2e75 6e69 7473 2c20 0d0a 0909 0909  lf.units, ......
+00055d90: 0909 6571 7561 6c5f 656e 6572 6779 5f62  ..equal_energy_b
+00055da0: 696e 203d 2073 656c 662e 6571 7561 6c5f  in = self.equal_
+00055db0: 656e 6572 6779 5f62 696e 290d 0a0d 0a0d  energy_bin).....
+00055dc0: 0a0d 0a09 6465 6620 5361 7665 5f64 6174  ....def Save_dat
+00055dd0: 6128 7365 6c66 2c20 7361 7665 5f52 4157  a(self, save_RAW
+00055de0: 203d 2054 7275 652c 2073 6176 655f 4669   = True, save_Fi
+00055df0: 7420 3d20 5472 7565 2c20 7361 7665 5f73  t = True, save_s
+00055e00: 6c69 6365 7320 3d20 5472 7565 2c20 7361  lices = True, sa
+00055e10: 7665 5f62 696e 6e65 6420 3d20 4661 6c73  ve_binned = Fals
+00055e20: 652c 200d 0a09 0909 0909 6669 6c65 6e61  e, .......filena
+00055e30: 6d65 203d 204e 6f6e 652c 2073 6176 655f  me = None, save_
+00055e40: 6669 745f 7265 7375 6c74 7320 3d20 5472  fit_results = Tr
+00055e50: 7565 2c20 7061 7468 203d 2027 4461 7461  ue, path = 'Data
+00055e60: 5f65 7870 6f72 7427 2c20 7365 7020 3d20  _export', sep = 
+00055e70: 7374 7228 275c 7427 2929 3a0d 0a09 0927  str('\t')):....'
+00055e80: 2727 6861 6e64 7920 6675 6e63 7469 6f6e  ''handy function
+00055e90: 2074 6f20 7361 7665 2074 6865 2064 6174   to save the dat
+00055ea0: 6120 6f6e 2064 6973 6b20 6173 2064 6174  a on disk as dat
+00055eb0: 2066 696c 6573 2e0d 0a09 0954 6865 2052   files.....The R
+00055ec0: 4157 206c 6162 656c 6564 2066 696c 6573  AW labeled files
+00055ed0: 2063 6f6e 7461 696e 2074 6865 2063 6869   contain the chi
+00055ee0: 7270 2063 6f72 7265 6374 6564 2076 616c  rp corrected val
+00055ef0: 7565 7320 2873 656c 662e 6473 290d 0a09  ues (self.ds)...
+00055f00: 090d 0a09 0974 6865 2073 6176 655f 736c  .....the save_sl
+00055f10: 6963 6573 2073 7769 7463 6820 7475 726e  ices switch turn
+00055f20: 7320 6f6e 2074 6865 2064 756d 7020 6f66  s on the dump of
+00055f30: 2074 6865 2073 6570 6172 6174 6520 736c   the separate sl
+00055f40: 6963 6564 2066 6967 7572 6573 2028 7469  iced figures (ti
+00055f50: 6d65 2061 6e64 2073 7065 6374 7261 6c29  me and spectral)
+00055f60: 200d 0a0d 0a09 090d 0a09 0950 6172 616d   ..........Param
+00055f70: 6574 6572 730d 0a09 092d 2d2d 2d2d 2d2d  eters....-------
+00055f80: 2d2d 2d0d 0a09 090d 0a09 0973 6176 655f  ---........save_
+00055f90: 6269 6e6e 6564 203a 2062 6f6f 6c2c 206f  binned : bool, o
+00055fa0: 7074 696f 6e61 6c0d 0a09 0909 6973 2061  ptional.....is a
+00055fb0: 6c73 6f20 7468 6520 7265 2d62 696e 6e65  lso the re-binne
+00055fc0: 6420 6d61 7472 6978 2074 6f20 6265 2073  d matrix to be s
+00055fd0: 6176 6564 2e0d 0a09 0909 0d0a 0909 7361  aved..........sa
+00055fe0: 7665 5f73 6c69 6365 7320 3a20 626f 6f6c  ve_slices : bool
+00055ff0: 2c20 6f70 7469 6f6e 616c 0d0a 0909 0973  , optional.....s
+00056000: 6176 6520 7468 6520 6b69 6e65 7469 6373  ave the kinetics
+00056010: 2061 6e64 2073 7065 6374 7261 2066 726f   and spectra fro
+00056020: 6d20 7468 6520 6669 7474 6564 2064 6174  m the fitted dat
+00056030: 6120 2877 6974 6820 7468 6520 6669 7473  a (with the fits
+00056040: 290d 0a09 0909 0d0a 0909 7365 7020 3a20  ).........sep : 
+00056050: 7374 722c 206f 7074 696f 6e61 6c0d 0a09  str, optional...
+00056060: 0909 7768 6174 2073 796d 626f 6c20 6973  ..what symbol is
+00056070: 2075 7365 6420 746f 2073 6570 6172 6174   used to separat
+00056080: 6520 6469 6666 6572 656e 7420 6e75 6d62  e different numb
+00056090: 6572 2e20 2874 7970 6963 616c 2065 6974  er. (typical eit
+000560a0: 6865 7220 2774 6162 2720 6f72 2063 6f6d  her 'tab' or com
+000560b0: 6d61 0d0a 0909 0d0a 0909 7361 7665 5f52  ma........save_R
+000560c0: 4157 203a 2062 6f6f 6c2c 206f 7074 696f  AW : bool, optio
+000560d0: 6e61 6c0d 0a09 0909 2844 6566 6175 6c74  nal.....(Default
+000560e0: 2920 5472 7565 2074 6865 6e20 7468 6520  ) True then the 
+000560f0: 6669 7273 7420 736c 6964 6520 7769 7468  first slide with
+00056100: 2074 6865 2052 4157 2064 6174 6120 6973   the RAW data is
+00056110: 2063 7265 6174 6564 200d 0a09 090d 0a09   created .......
+00056120: 0973 6176 655f 4669 7420 3a20 626f 6f6c  .save_Fit : bool
+00056130: 2c20 6f70 7469 6f6e 616c 0d0a 0909 0928  , optional.....(
+00056140: 4465 6661 756c 7429 2054 7275 6520 7468  Default) True th
+00056150: 656e 2074 6865 2073 6563 6f6e 6420 736c  en the second sl
+00056160: 6964 6520 7769 7468 2074 6865 2046 6974  ide with the Fit
+00056170: 7465 6420 6461 7461 2069 7320 6372 6561  ted data is crea
+00056180: 7465 6420 0d0a 0909 0d0a 0909 7061 7468  ted ........path
+00056190: 203a 204e 6f6e 652c 2073 7472 206f 7220   : None, str or 
+000561a0: 7061 7468 2c20 6f70 7469 6f6e 616c 0d0a  path, optional..
+000561b0: 0909 0928 4465 6661 756c 7429 204e 6f6e  ...(Default) Non
+000561c0: 652c 2069 6620 6c65 6674 206f 6e20 4e6f  e, if left on No
+000561d0: 6e65 2c20 7468 656e 2061 2066 6f6c 6465  ne, then a folde
+000561e0: 7220 2272 6573 756c 745f 6669 6775 7265  r "result_figure
+000561f0: 7322 2069 7320 6372 6561 7465 6420 696e  s" is created in
+00056200: 2074 6865 2066 6f6c 6465 7220 0d0a 0909   the folder ....
+00056210: 096f 6620 7468 6520 6461 7461 2028 7365  .of the data (se
+00056220: 6c66 2e70 6174 6829 0d0a 0909 090d 0a09  lf.path)........
+00056230: 0973 6176 655f 6669 745f 7265 7375 6c74  .save_fit_result
+00056240: 7320 3a20 626f 6f6c 2c20 6f70 7469 6f6e  s : bool, option
+00056250: 616c 0d0a 0909 0969 6620 5472 7565 2028  al.....if True (
+00056260: 4465 6661 756c 7429 2020 6120 6e65 6174  Default)  a neat
+00056270: 6c79 2066 6f72 6d61 7465 6420 6669 6c65  ly formated file
+00056280: 2077 6974 6820 7468 6520 6669 7420 7265   with the fit re
+00056290: 7375 6c74 7320 6973 2063 7265 6174 6564  sults is created
+000562a0: 2061 6e64 2073 746f 7265 6420 7769 7468   and stored with
+000562b0: 2074 6865 2064 6174 610d 0a09 0909 0d0a   the data.......
+000562c0: 0909 6669 6c65 6e61 6d65 203a 2073 7472  ..filename : str
+000562d0: 2c20 6f70 7469 6f6e 616c 0d0a 0909 0928  , optional.....(
+000562e0: 4465 6661 756c 7429 204e 6f6e 652c 2042  Default) None, B
+000562f0: 6173 6520 6e61 6d65 2066 6f72 2061 6c6c  ase name for all
+00056300: 2070 6c6f 7473 2e20 4966 204e 6f6e 652c   plots. If None,
+00056310: 2074 6865 6e20 7365 6c66 2e66 696c 656e   then self.filen
+00056320: 616d 6520 7769 6c6c 2062 6520 7573 6564  ame will be used
+00056330: 0d0a 0909 090d 0a09 0945 7861 6d70 6c65  .........Example
+00056340: 730d 0a09 092d 2d2d 2d2d 2d2d 2d2d 0d0a  s....---------..
+00056350: 0909 3e3e 3e20 7461 2e53 6176 655f 4461  ..>>> ta.Save_Da
+00056360: 7461 0d0a 0909 0d0a 0909 2727 270d 0a09  ta........'''...
+00056370: 090d 0a09 0969 6620 6669 6c65 6e61 6d65  .....if filename
+00056380: 2069 7320 4e6f 6e65 3a66 696c 656e 616d   is None:filenam
+00056390: 6520 3d20 7365 6c66 2e66 696c 656e 616d  e = self.filenam
+000563a0: 652e 7370 6c69 7428 272e 2729 5b30 5d0d  e.split('.')[0].
+000563b0: 0a09 0969 6620 7361 7665 5f52 4157 3a0d  ...if save_RAW:.
+000563c0: 0a09 0909 7365 6c66 2e64 732e 746f 5f63  ....self.ds.to_c
+000563d0: 7376 2863 6865 636b 5f66 6f6c 6465 7228  sv(check_folder(
+000563e0: 7061 7468 203d 2070 6174 682c 2063 7572  path = path, cur
+000563f0: 7265 6e74 5f70 6174 6820 3d20 7365 6c66  rent_path = self
+00056400: 2e70 6174 682c 200d 0a09 0909 0909 0909  .path, .........
+00056410: 6669 6c65 6e61 6d65 203d 2066 696c 656e  filename = filen
+00056420: 616d 652b 275f 6368 6972 705f 636f 7272  ame+'_chirp_corr
+00056430: 6563 7465 645f 7261 775f 6d61 7472 6978  ected_raw_matrix
+00056440: 2e64 6174 2729 2c20 7365 7020 3d20 7365  .dat'), sep = se
+00056450: 7029 0d0a 0909 0969 6620 7361 7665 5f62  p).....if save_b
+00056460: 696e 6e65 643a 0d0a 0909 0909 7375 6220  inned:......sub 
+00056470: 3d20 7375 625f 6473 2873 656c 662e 6473  = sub_ds(self.ds
+00056480: 2c20 7363 6174 7465 7263 7574 203d 2073  , scattercut = s
+00056490: 656c 662e 7363 6174 7465 7263 7574 2c20  elf.scattercut, 
+000564a0: 626f 7264 6572 6375 7420 3d20 7365 6c66  bordercut = self
+000564b0: 2e62 6f72 6465 7263 7574 2c20 0d0a 0909  .bordercut, ....
+000564c0: 0909 0909 0974 696d 656c 696d 6974 7320  .....timelimits 
+000564d0: 3d20 7365 6c66 2e74 696d 656c 696d 6974  = self.timelimit
+000564e0: 732c 2077 6176 655f 6e6d 5f62 696e 203d  s, wave_nm_bin =
+000564f0: 2073 656c 662e 7761 7665 5f6e 6d5f 6269   self.wave_nm_bi
+00056500: 6e2c 200d 0a09 0909 0909 0909 7469 6d65  n, .........time
+00056510: 5f62 696e 203d 2073 656c 662e 7469 6d65  _bin = self.time
+00056520: 5f62 696e 290d 0a09 0909 0973 7562 2e74  _bin)......sub.t
+00056530: 6f5f 6373 7628 6368 6563 6b5f 666f 6c64  o_csv(check_fold
+00056540: 6572 2870 6174 6820 3d20 7061 7468 2c20  er(path = path, 
+00056550: 6375 7272 656e 745f 7061 7468 203d 2073  current_path = s
+00056560: 656c 662e 7061 7468 2c20 0d0a 0909 0909  elf.path, ......
+00056570: 0909 0909 0909 6669 6c65 6e61 6d65 203d  ......filename =
+00056580: 2066 696c 656e 616d 652b 275f 6368 6972   filename+'_chir
+00056590: 705f 636f 7272 6563 7465 645f 7265 6269  p_corrected_rebi
+000565a0: 6e6e 6564 5f6d 6174 7269 782e 6461 7427  nned_matrix.dat'
+000565b0: 292c 2073 6570 203d 2073 6570 290d 0a09  ), sep = sep)...
+000565c0: 0909 6966 2073 6176 655f 736c 6963 6573  ..if save_slices
+000565d0: 3a0d 0a09 0909 0973 7562 203d 2073 7562  :......sub = sub
+000565e0: 5f64 7328 6473 203d 2073 656c 662e 6473  _ds(ds = self.ds
+000565f0: 2e63 6f70 7928 292c 2077 6176 656c 656e  .copy(), wavelen
+00056600: 6774 685f 6269 6e20 3d20 7365 6c66 2e77  gth_bin = self.w
+00056610: 6176 656c 656e 6774 685f 6269 6e2c 2077  avelength_bin, w
+00056620: 6176 656c 656e 6774 6820 3d20 7365 6c66  avelength = self
+00056630: 2e72 656c 5f77 6176 6529 0d0a 0909 0909  .rel_wave)......
+00056640: 2373 7562 2e63 6f6c 756d 6e73 2e6e 616d  #sub.columns.nam
+00056650: 6520 3d20 2777 6176 656c 656e 6774 6820  e = 'wavelength 
+00056660: 5b6e 6d5d 2069 6e20 252e 3066 2062 696e  [nm] in %.0f bin
+00056670: 7327 2573 656c 662e 7761 7665 6c65 6e67  s'%self.waveleng
+00056680: 7468 5f62 696e 0d0a 0909 0909 7375 622e  th_bin......sub.
+00056690: 746f 5f63 7376 2863 6865 636b 5f66 6f6c  to_csv(check_fol
+000566a0: 6465 7228 7061 7468 203d 2070 6174 682c  der(path = path,
+000566b0: 2063 7572 7265 6e74 5f70 6174 6820 3d20   current_path = 
+000566c0: 7365 6c66 2e70 6174 682c 200d 0a09 0909  self.path, .....
+000566d0: 0909 0909 6669 6c65 6e61 6d65 203d 2066  ....filename = f
+000566e0: 696c 656e 616d 652b 275f 6368 6972 705f  ilename+'_chirp_
+000566f0: 636f 7272 6563 7465 645f 5241 575f 6b69  corrected_RAW_ki
+00056700: 6e65 7469 6373 2e64 6174 2729 2c20 7365  netics.dat'), se
+00056710: 7020 3d20 7365 7029 0d0a 0909 0909 7375  p = sep)......su
+00056720: 6220 3d20 7375 625f 6473 2864 7320 3d20  b = sub_ds(ds = 
+00056730: 7365 6c66 2e64 732e 636f 7079 2829 2c20  self.ds.copy(), 
+00056740: 7469 6d65 7320 3d20 7365 6c66 2e72 656c  times = self.rel
+00056750: 5f74 696d 652c 2074 696d 655f 7769 6474  _time, time_widt
+00056760: 685f 7065 7263 656e 7420 3d20 7365 6c66  h_percent = self
+00056770: 2e74 696d 655f 7769 6474 685f 7065 7263  .time_width_perc
+00056780: 656e 742c 200d 0a09 0909 0909 0909 0973  ent, ..........s
+00056790: 6361 7474 6572 6375 7420 3d20 7365 6c66  cattercut = self
+000567a0: 2e73 6361 7474 6572 6375 742c 2062 6f72  .scattercut, bor
+000567b0: 6465 7263 7574 203d 2073 656c 662e 626f  dercut = self.bo
+000567c0: 7264 6572 6375 742c 2077 6176 655f 6e6d  rdercut, wave_nm
+000567d0: 5f62 696e 203d 2073 656c 662e 7761 7665  _bin = self.wave
+000567e0: 5f6e 6d5f 6269 6e29 0d0a 0909 0909 7375  _nm_bin)......su
+000567f0: 622e 746f 5f63 7376 2863 6865 636b 5f66  b.to_csv(check_f
+00056800: 6f6c 6465 7228 7061 7468 203d 2070 6174  older(path = pat
+00056810: 682c 2063 7572 7265 6e74 5f70 6174 6820  h, current_path 
+00056820: 3d20 7365 6c66 2e70 6174 682c 200d 0a09  = self.path, ...
+00056830: 0909 0909 0909 6669 6c65 6e61 6d65 203d  ......filename =
+00056840: 2066 696c 656e 616d 652b 275f 6368 6972   filename+'_chir
+00056850: 705f 636f 7272 6563 7465 645f 5241 575f  p_corrected_RAW_
+00056860: 5370 6563 7472 612e 6461 7427 292c 2073  Spectra.dat'), s
+00056870: 6570 203d 2073 6570 290d 0a09 0969 6620  ep = sep)....if 
+00056880: 7361 7665 5f46 6974 3a0d 0a09 0909 7472  save_Fit:.....tr
+00056890: 793a 0d0a 0909 0909 7365 6c66 2e72 652e  y:......self.re.
+000568a0: 6b65 7973 2829 0d0a 0909 0965 7863 6570  keys().....excep
+000568b0: 743a 0d0a 0909 0909 7072 696e 7428 276e  t:......print('n
+000568c0: 6f20 6669 7420 696e 2064 6174 6127 290d  o fit in data').
+000568d0: 0a09 0909 0973 6176 655f 4669 7420 3d20  .....save_Fit = 
+000568e0: 4661 6c73 650d 0a09 0969 6620 7361 7665  False....if save
+000568f0: 5f46 6974 3a0d 0a09 0909 7365 6c66 2e72  _Fit:.....self.r
+00056900: 655b 2741 275d 2e74 6f5f 6373 7628 6368  e['A'].to_csv(ch
+00056910: 6563 6b5f 666f 6c64 6572 2870 6174 6820  eck_folder(path 
+00056920: 3d20 7061 7468 2c20 6375 7272 656e 745f  = path, current_
+00056930: 7061 7468 203d 2073 656c 662e 7061 7468  path = self.path
+00056940: 2c20 0d0a 0909 0909 0909 0909 6669 6c65  , ..........file
+00056950: 6e61 6d65 203d 2066 696c 656e 616d 652b  name = filename+
+00056960: 275f 6d61 7472 6978 2075 7365 6420 6173  '_matrix used as
+00056970: 2066 6974 2069 6e70 7574 2e64 6174 2729   fit input.dat')
+00056980: 2c20 7365 7020 3d20 7365 7029 0d0a 0909  , sep = sep)....
+00056990: 0973 656c 662e 7265 5b27 4143 275d 2e74  .self.re['AC'].t
+000569a0: 6f5f 6373 7628 6368 6563 6b5f 666f 6c64  o_csv(check_fold
+000569b0: 6572 2870 6174 6820 3d20 7061 7468 2c20  er(path = path, 
+000569c0: 6375 7272 656e 745f 7061 7468 203d 2073  current_path = s
+000569d0: 656c 662e 7061 7468 2c20 0d0a 0909 0909  elf.path, ......
+000569e0: 0909 0909 6669 6c65 6e61 6d65 203d 2066  ....filename = f
+000569f0: 696c 656e 616d 652b 275f 6d61 7472 6978  ilename+'_matrix
+00056a00: 2063 616c 6375 6c61 7465 6420 6475 7269   calculated duri
+00056a10: 6e67 2066 6974 2e64 6174 2729 2c20 7365  ng fit.dat'), se
+00056a20: 7020 3d20 7365 7029 0d0a 0909 0973 656c  p = sep).....sel
+00056a30: 662e 7265 5b27 4145 275d 2e74 6f5f 6373  f.re['AE'].to_cs
+00056a40: 7628 6368 6563 6b5f 666f 6c64 6572 2870  v(check_folder(p
+00056a50: 6174 6820 3d20 7061 7468 2c20 6375 7272  ath = path, curr
+00056a60: 656e 745f 7061 7468 203d 2073 656c 662e  ent_path = self.
+00056a70: 7061 7468 2c20 0d0a 0909 0909 0909 0909  path, ..........
+00056a80: 6669 6c65 6e61 6d65 203d 2066 696c 656e  filename = filen
+00056a90: 616d 652b 275f 6572 726f 725f 6d61 7472  ame+'_error_matr
+00056aa0: 6978 2063 616c 6375 6c61 7465 6420 6475  ix calculated du
+00056ab0: 7269 6e67 2066 6974 2e64 6174 2729 2c20  ring fit.dat'), 
+00056ac0: 7365 7020 3d20 7365 7029 0d0a 0909 0969  sep = sep).....i
+00056ad0: 6620 7361 7665 5f73 6c69 6365 733a 090d  f save_slices:..
+00056ae0: 0a09 0909 0973 7562 203d 2073 7562 5f64  .....sub = sub_d
+00056af0: 7328 6473 203d 2073 656c 662e 7265 5b27  s(ds = self.re['
+00056b00: 4143 275d 2e63 6f70 7928 292c 2077 6176  AC'].copy(), wav
+00056b10: 656c 656e 6774 685f 6269 6e20 3d20 7365  elength_bin = se
+00056b20: 6c66 2e77 6176 656c 656e 6774 685f 6269  lf.wavelength_bi
+00056b30: 6e2c 2077 6176 656c 656e 6774 6820 3d20  n, wavelength = 
+00056b40: 7365 6c66 2e72 656c 5f77 6176 6529 0d0a  self.rel_wave)..
+00056b50: 0909 0909 2373 7562 2e63 6f6c 756d 6e73  ....#sub.columns
+00056b60: 2e6e 616d 6520 3d20 2777 6176 656c 656e  .name = 'wavelen
+00056b70: 7468 205b 6e6d 5d20 696e 2025 2e30 6620  th [nm] in %.0f 
+00056b80: 6269 6e73 2725 7365 6c66 2e77 6176 656c  bins'%self.wavel
+00056b90: 656e 6774 685f 6269 6e0d 0a09 0909 0973  ength_bin......s
+00056ba0: 7562 2e74 6f5f 6373 7628 6368 6563 6b5f  ub.to_csv(check_
+00056bb0: 666f 6c64 6572 2870 6174 6820 3d20 7061  folder(path = pa
+00056bc0: 7468 2c20 6375 7272 656e 745f 7061 7468  th, current_path
+00056bd0: 203d 2073 656c 662e 7061 7468 2c20 0d0a   = self.path, ..
+00056be0: 0909 0909 0909 0966 696c 656e 616d 6520  .......filename 
+00056bf0: 3d20 6669 6c65 6e61 6d65 2b27 5f66 6974  = filename+'_fit
+00056c00: 7465 645f 6b69 6e65 7469 6373 2e64 6174  ted_kinetics.dat
+00056c10: 2729 2c20 7365 7020 3d20 7365 7029 0d0a  '), sep = sep)..
+00056c20: 0909 0909 7375 6220 3d20 7375 625f 6473  ....sub = sub_ds
+00056c30: 2864 7320 3d20 7365 6c66 2e72 655b 2741  (ds = self.re['A
+00056c40: 275d 2e63 6f70 7928 292c 2077 6176 656c  '].copy(), wavel
+00056c50: 656e 6774 685f 6269 6e20 3d20 7365 6c66  ength_bin = self
+00056c60: 2e77 6176 656c 656e 6774 685f 6269 6e2c  .wavelength_bin,
+00056c70: 2077 6176 656c 656e 6774 6820 3d20 7365   wavelength = se
+00056c80: 6c66 2e72 656c 5f77 6176 6529 0d0a 0909  lf.rel_wave)....
+00056c90: 0909 2373 7562 2e63 6f6c 756d 6e73 2e6e  ..#sub.columns.n
+00056ca0: 616d 6520 3d20 2777 6176 656c 656e 7468  ame = 'wavelenth
+00056cb0: 205b 6e6d 5d20 696e 2025 2e30 6620 6269   [nm] in %.0f bi
+00056cc0: 6e73 2725 7365 6c66 2e77 6176 656c 656e  ns'%self.wavelen
+00056cd0: 6774 685f 6269 6e0d 0a09 0909 0973 7562  gth_bin......sub
+00056ce0: 2e74 6f5f 6373 7628 6368 6563 6b5f 666f  .to_csv(check_fo
+00056cf0: 6c64 6572 2870 6174 6820 3d20 7061 7468  lder(path = path
+00056d00: 2c20 6375 7272 656e 745f 7061 7468 203d  , current_path =
+00056d10: 2073 656c 662e 7061 7468 2c20 0d0a 0909   self.path, ....
+00056d20: 0909 0909 0966 696c 656e 616d 6520 3d20  .....filename = 
+00056d30: 6669 6c65 6e61 6d65 2b27 5f6d 6561 7375  filename+'_measu
+00056d40: 7265 645f 6b69 6e65 7469 6373 2e64 6174  red_kinetics.dat
+00056d50: 2729 2c20 7365 7020 3d20 7365 7029 0d0a  '), sep = sep)..
+00056d60: 0909 0909 7375 6220 3d20 7375 625f 6473  ....sub = sub_ds
+00056d70: 2864 7320 3d20 7365 6c66 2e72 655b 2741  (ds = self.re['A
+00056d80: 4327 5d2e 636f 7079 2829 2c20 7469 6d65  C'].copy(), time
+00056d90: 7320 3d20 7365 6c66 2e72 656c 5f74 696d  s = self.rel_tim
+00056da0: 652c 200d 0a09 0909 0909 0909 7469 6d65  e, .........time
+00056db0: 5f77 6964 7468 5f70 6572 6365 6e74 203d  _width_percent =
+00056dc0: 2073 656c 662e 7469 6d65 5f77 6964 7468   self.time_width
+00056dd0: 5f70 6572 6365 6e74 2c20 7363 6174 7465  _percent, scatte
+00056de0: 7263 7574 203d 2073 656c 662e 7363 6174  rcut = self.scat
+00056df0: 7465 7263 7574 2c20 0d0a 0909 0909 0909  tercut, ........
+00056e00: 0962 6f72 6465 7263 7574 203d 2073 656c  .bordercut = sel
+00056e10: 662e 626f 7264 6572 6375 742c 2077 6176  f.bordercut, wav
+00056e20: 655f 6e6d 5f62 696e 203d 2073 656c 662e  e_nm_bin = self.
+00056e30: 7761 7665 5f6e 6d5f 6269 6e29 0d0a 0909  wave_nm_bin)....
+00056e40: 0909 7375 622e 746f 5f63 7376 2863 6865  ..sub.to_csv(che
+00056e50: 636b 5f66 6f6c 6465 7228 7061 7468 203d  ck_folder(path =
+00056e60: 2070 6174 682c 2063 7572 7265 6e74 5f70   path, current_p
+00056e70: 6174 6820 3d20 7365 6c66 2e70 6174 682c  ath = self.path,
+00056e80: 200d 0a09 0909 0909 0909 6669 6c65 6e61   .........filena
+00056e90: 6d65 203d 2066 696c 656e 616d 652b 275f  me = filename+'_
+00056ea0: 6669 7474 6564 5f73 7065 6374 7261 2e64  fitted_spectra.d
+00056eb0: 6174 2729 2c20 7365 7020 3d20 7365 7029  at'), sep = sep)
+00056ec0: 0d0a 0909 0909 7375 6220 3d20 7375 625f  ......sub = sub_
+00056ed0: 6473 2864 7320 3d20 7365 6c66 2e72 655b  ds(ds = self.re[
+00056ee0: 2741 275d 2e63 6f70 7928 292c 2074 696d  'A'].copy(), tim
+00056ef0: 6573 203d 2073 656c 662e 7265 6c5f 7469  es = self.rel_ti
+00056f00: 6d65 2c20 0d0a 0909 0909 0909 0974 696d  me, .........tim
+00056f10: 655f 7769 6474 685f 7065 7263 656e 7420  e_width_percent 
+00056f20: 3d20 7365 6c66 2e74 696d 655f 7769 6474  = self.time_widt
+00056f30: 685f 7065 7263 656e 742c 2073 6361 7474  h_percent, scatt
+00056f40: 6572 6375 7420 3d20 7365 6c66 2e73 6361  ercut = self.sca
+00056f50: 7474 6572 6375 742c 200d 0a09 0909 0909  ttercut, .......
+00056f60: 0909 626f 7264 6572 6375 7420 3d20 7365  ..bordercut = se
+00056f70: 6c66 2e62 6f72 6465 7263 7574 2c20 7761  lf.bordercut, wa
+00056f80: 7665 5f6e 6d5f 6269 6e20 3d20 7365 6c66  ve_nm_bin = self
+00056f90: 2e77 6176 655f 6e6d 5f62 696e 290d 0a09  .wave_nm_bin)...
+00056fa0: 0909 0973 7562 2e74 6f5f 6373 7628 6368  ...sub.to_csv(ch
+00056fb0: 6563 6b5f 666f 6c64 6572 2870 6174 6820  eck_folder(path 
+00056fc0: 3d20 7061 7468 2c20 6375 7272 656e 745f  = path, current_
+00056fd0: 7061 7468 203d 2073 656c 662e 7061 7468  path = self.path
+00056fe0: 2c20 0d0a 0909 0909 0909 0966 696c 656e  , .........filen
+00056ff0: 616d 6520 3d20 6669 6c65 6e61 6d65 2b27  ame = filename+'
+00057000: 5f6d 6561 7375 7265 645f 7370 6563 7472  _measured_spectr
+00057010: 612e 6461 7427 292c 2073 6570 203d 2073  a.dat'), sep = s
+00057020: 6570 290d 0a09 0909 0973 656c 662e 7265  ep)......self.re
+00057030: 5b27 4441 4327 5d2e 746f 5f63 7376 2863  ['DAC'].to_csv(c
+00057040: 6865 636b 5f66 6f6c 6465 7228 7061 7468  heck_folder(path
+00057050: 203d 2070 6174 682c 2063 7572 7265 6e74   = path, current
+00057060: 5f70 6174 6820 3d20 7365 6c66 2e70 6174  _path = self.pat
+00057070: 682c 200d 0a09 0909 0909 0909 6669 6c65  h, .........file
+00057080: 6e61 6d65 203d 2066 696c 656e 616d 652b  name = filename+
+00057090: 275f 4441 532d 5341 532e 6461 7427 292c  '_DAS-SAS.dat'),
+000570a0: 2073 6570 203d 2073 6570 290d 0a09 090d   sep = sep).....
+000570b0: 0a09 0909 6966 2073 6176 655f 6669 745f  ....if save_fit_
+000570c0: 7265 7375 6c74 733a 0d0a 0909 0909 0d0a  results:........
+000570d0: 0909 0909 5265 7375 6c74 5f73 7472 696e  ....Result_strin
+000570e0: 673d 275c 6e46 6974 2052 6573 756c 7473  g='\nFit Results
+000570f0: 3a5c 6e27 0d0a 0909 0909 0d0a 0909 0909  :\n'............
+00057100: 6966 2069 7369 6e73 7461 6e63 6528 7365  if isinstance(se
+00057110: 6c66 2e6d 6f64 2c74 7970 6528 2768 656c  lf.mod,type('hel
+00057120: 6c6f 2729 293a 0d0a 0909 0909 0952 6573  lo')):.......Res
+00057130: 756c 745f 7374 7269 6e67 2b3d 274d 6f64  ult_string+='Mod
+00057140: 656c 2055 7365 643a 2025 735c 6e5c 6e27  el Used: %s\n\n'
+00057150: 2573 656c 662e 6d6f 640d 0a09 0909 0965  %self.mod......e
+00057160: 6c73 653a 0d0a 0909 0909 0952 6573 756c  lse:.......Resul
+00057170: 745f 7374 7269 6e67 2b3d 274d 6f64 656c  t_string+='Model
+00057180: 2055 7365 643a 2045 7874 6572 6e61 6c20   Used: External 
+00057190: 6675 6e63 7469 6f6e 5c6e 5c6e 270d 0a09  function\n\n'...
+000571a0: 0909 090d 0a09 0909 0969 6620 7365 6c66  .........if self
+000571b0: 2e69 676e 6f72 655f 7469 6d65 5f72 6567  .ignore_time_reg
+000571c0: 696f 6e20 6973 206e 6f74 204e 6f6e 653a  ion is not None:
+000571d0: 0d0a 0909 0909 0952 6573 756c 745f 7374  .......Result_st
+000571e0: 7269 6e67 2b3d 2774 6865 2074 696d 6520  ring+='the time 
+000571f0: 6265 7477 6565 6e20 252e 3366 2025 7320  between %.3f %s 
+00057200: 616e 6420 252e 3366 2025 7320 7761 7320  and %.3f %s was 
+00057210: 6578 636c 7564 6564 2066 726f 6d20 7468  excluded from th
+00057220: 6520 6f70 7469 6d69 7a61 7469 6f6e 5c6e  e optimization\n
+00057230: 2725 2873 656c 662e 6967 6e6f 7265 5f74  '%(self.ignore_t
+00057240: 696d 655f 7265 6769 6f6e 5b30 5d2c 7365  ime_region[0],se
+00057250: 6c66 2e62 6173 6575 6e69 742c 7365 6c66  lf.baseunit,self
+00057260: 2e69 676e 6f72 655f 7469 6d65 5f72 6567  .ignore_time_reg
+00057270: 696f 6e5b 315d 2c73 656c 662e 6261 7365  ion[1],self.base
+00057280: 756e 6974 2909 0d0a 0909 0909 5265 7375  unit).......Resu
+00057290: 6c74 5f73 7472 696e 672b 3d27 5468 6520  lt_string+='The 
+000572a0: 6d69 6e69 6d75 6d20 6572 726f 7220 6973  minimum error is
+000572b0: 3a7b 3a2e 3865 7d5c 6e27 2e66 6f72 6d61  :{:.8e}\n'.forma
+000572c0: 7428 7365 6c66 2e72 655b 2765 7272 6f72  t(self.re['error
+000572d0: 275d 290d 0a09 0909 0952 6573 756c 745f  '])......Result_
+000572e0: 7374 7269 6e67 2b3d 2754 6865 206d 696e  string+='The min
+000572f0: 696d 756d 2052 322d 7661 6c75 6520 6973  imum R2-value is
+00057300: 3a7b 3a2e 3865 7d5c 6e27 2e66 6f72 6d61  :{:.8e}\n'.forma
+00057310: 7428 7365 6c66 2e72 655b 2772 3227 5d29  t(self.re['r2'])
+00057320: 0d0a 0909 0909 0d0a 0909 0909 6966 2027  ............if '
+00057330: 636f 6e66 6964 656e 6365 2720 696e 2073  confidence' in s
+00057340: 656c 662e 7265 3a0d 0a09 0909 0909 5265  elf.re:.......Re
+00057350: 7375 6c74 5f73 7472 696e 672b 3d27 5c6e  sult_string+='\n
+00057360: 496e 2052 6174 6573 2077 6974 6820 636f  In Rates with co
+00057370: 6e66 6964 656e 6365 2069 6e74 6572 7661  nfidence interva
+00057380: 6c20 746f 206c 6576 656c 206f 6620 2573  l to level of %s
+00057390: 5c6e 2725 7365 6c66 2e72 655b 2763 6f6e  \n'%self.re['con
+000573a0: 6669 6465 6e63 6527 5d5b 2774 6172 6765  fidence']['targe
+000573b0: 742d 6c65 7665 6c27 5d0d 0a09 0909 0909  t-level'].......
+000573c0: 5265 7375 6c74 5f73 7472 696e 672b 3d73  Result_string+=s
+000573d0: 656c 662e 7265 5b27 6669 745f 7265 7375  elf.re['fit_resu
+000573e0: 6c74 735f 7261 7465 7327 5d2e 746f 5f73  lts_rates'].to_s
+000573f0: 7472 696e 6728 636f 6c75 6d6e 733d 5b27  tring(columns=['
+00057400: 7661 6c75 6527 2c27 6c6f 7765 725f 6c69  value','lower_li
+00057410: 6d69 7427 2c27 7570 7065 725f 6c69 6d69  mit','upper_limi
+00057420: 7427 2c27 696e 6974 5f76 616c 7565 272c  t','init_value',
+00057430: 2776 6172 7927 2c27 6d69 6e27 2c27 6d61  'vary','min','ma
+00057440: 7827 2c27 6578 7072 275d 290d 0a09 0909  x','expr']).....
+00057450: 0909 5265 7375 6c74 5f73 7472 696e 672b  ..Result_string+
+00057460: 3d27 5c6e 5c6e 5468 6520 7261 7465 7320  ='\n\nThe rates 
+00057470: 636f 6e76 6572 7465 6420 746f 2074 696d  converted to tim
+00057480: 6573 2077 6974 6820 756e 6974 2025 7320  es with unit %s 
+00057490: 7769 7468 2063 6f6e 6669 6465 6e63 6520  with confidence 
+000574a0: 696e 7465 7276 616c 2074 6f20 6c65 7665  interval to leve
+000574b0: 6c20 6f66 2025 735c 6e27 2528 7365 6c66  l of %s\n'%(self
+000574c0: 2e62 6173 6575 6e69 742c 7365 6c66 2e72  .baseunit,self.r
+000574d0: 655b 2763 6f6e 6669 6465 6e63 6527 5d5b  e['confidence'][
+000574e0: 2774 6172 6765 742d 6c65 7665 6c27 5d29  'target-level'])
+000574f0: 0d0a 0909 0909 0952 6573 756c 745f 7374  .......Result_st
+00057500: 7269 6e67 2b3d 7365 6c66 2e72 655b 2766  ring+=self.re['f
+00057510: 6974 5f72 6573 756c 7473 5f74 696d 6573  it_results_times
+00057520: 275d 2e74 6f5f 7374 7269 6e67 2863 6f6c  '].to_string(col
+00057530: 756d 6e73 3d5b 2776 616c 7565 272c 276c  umns=['value','l
+00057540: 6f77 6572 5f6c 696d 6974 272c 2775 7070  ower_limit','upp
+00057550: 6572 5f6c 696d 6974 272c 2769 6e69 745f  er_limit','init_
+00057560: 7661 6c75 6527 2c27 7661 7279 272c 276d  value','vary','m
+00057570: 696e 272c 276d 6178 272c 2765 7870 7227  in','max','expr'
+00057580: 5d29 0d0a 0909 0909 656c 7365 3a0d 0a09  ])......else:...
+00057590: 0909 0909 5265 7375 6c74 5f73 7472 696e  ....Result_strin
+000575a0: 672b 3d27 5c6e 496e 2052 6174 6573 5c6e  g+='\nIn Rates\n
+000575b0: 270d 0a09 0909 0909 5265 7375 6c74 5f73  '.......Result_s
+000575c0: 7472 696e 672b 3d73 656c 662e 7265 5b27  tring+=self.re['
+000575d0: 6669 745f 7265 7375 6c74 735f 7261 7465  fit_results_rate
+000575e0: 7327 5d2e 746f 5f73 7472 696e 6728 636f  s'].to_string(co
+000575f0: 6c75 6d6e 733d 5b27 7661 6c75 6527 2c27  lumns=['value','
+00057600: 696e 6974 5f76 616c 7565 272c 2776 6172  init_value','var
+00057610: 7927 2c27 6d69 6e27 2c27 6d61 7827 2c27  y','min','max','
+00057620: 6578 7072 275d 290d 0a09 0909 0909 5265  expr']).......Re
+00057630: 7375 6c74 5f73 7472 696e 672b 3d27 5c6e  sult_string+='\n
+00057640: 5c6e 5468 6520 7261 7465 7320 636f 6e76  \nThe rates conv
+00057650: 6572 7465 6420 746f 2074 696d 6573 2077  erted to times w
+00057660: 6974 6820 756e 6974 2025 735c 6e27 2573  ith unit %s\n'%s
+00057670: 656c 662e 6261 7365 756e 6974 0d0a 0909  elf.baseunit....
+00057680: 0909 0952 6573 756c 745f 7374 7269 6e67  ...Result_string
+00057690: 2b3d 7365 6c66 2e72 655b 2766 6974 5f72  +=self.re['fit_r
+000576a0: 6573 756c 7473 5f74 696d 6573 275d 2e74  esults_times'].t
+000576b0: 6f5f 7374 7269 6e67 2863 6f6c 756d 6e73  o_string(columns
+000576c0: 3d5b 2776 616c 7565 272c 2769 6e69 745f  =['value','init_
+000576d0: 7661 6c75 6527 2c27 7661 7279 272c 276d  value','vary','m
+000576e0: 696e 272c 276d 6178 272c 2765 7870 7227  in','max','expr'
+000576f0: 5d29 0d0a 0d0a 0909 0909 7769 7468 206f  ])........with o
+00057700: 7065 6e28 6368 6563 6b5f 666f 6c64 6572  pen(check_folder
+00057710: 2870 6174 6820 3d20 7061 7468 2c20 6375  (path = path, cu
+00057720: 7272 656e 745f 7061 7468 203d 2073 656c  rrent_path = sel
+00057730: 662e 7061 7468 2c20 6669 6c65 6e61 6d65  f.path, filename
+00057740: 203d 2066 696c 656e 616d 652b 275f 6669   = filename+'_fi
+00057750: 745f 7265 7375 6c74 735f 7061 7261 6d65  t_results_parame
+00057760: 7465 722e 7061 7227 292c 2022 7722 2920  ter.par'), "w") 
+00057770: 6173 2074 6578 745f 6669 6c65 3a0d 0a09  as text_file:...
+00057780: 0909 0909 7465 7874 5f66 696c 652e 7772  ....text_file.wr
+00057790: 6974 6528 5265 7375 6c74 5f73 7472 696e  ite(Result_strin
+000577a0: 6729 0d0a 0d0a 0964 6566 2053 6176 655f  g).....def Save_
+000577b0: 506f 7765 7270 6f69 6e74 2873 656c 662c  Powerpoint(self,
+000577c0: 2073 6176 655f 5241 5720 3d20 5472 7565   save_RAW = True
+000577d0: 2c20 7361 7665 5f46 6974 203d 2054 7275  , save_Fit = Tru
+000577e0: 652c 2066 696c 656e 616d 6520 3d20 4e6f  e, filename = No
+000577f0: 6e65 2c20 0d0a 0909 0909 0909 7061 7468  ne, ........path
+00057800: 203d 2027 7265 7375 6c74 5f66 6967 7572   = 'result_figur
+00057810: 6573 272c 2073 6361 6c65 5f74 7970 6520  es', scale_type 
+00057820: 3d20 2773 796d 6c6f 6727 2c20 7469 746c  = 'symlog', titl
+00057830: 6520 3d20 4e6f 6e65 2c20 7061 7463 6865  e = None, patche
+00057840: 7320 3d20 4661 6c73 652c 2063 6d61 703d  s = False, cmap=
+00057850: 4e6f 6e65 202c 2073 6176 6574 7970 6520  None , savetype 
+00057860: 3d20 2770 7074 7827 293a 0d0a 0909 2727  = 'pptx'):....''
+00057870: 2754 6869 7320 6675 6e63 7469 6f6e 2063  'This function c
+00057880: 7265 6174 6573 2074 776f 2070 6f77 6572  reates two power
+00057890: 2070 6f69 6e74 2073 6c69 6465 732e 204f   point slides. O
+000578a0: 6e20 7468 6520 6669 7273 7420 6974 2073  n the first it s
+000578b0: 756d 6d61 7269 7a65 7320 7468 6520 5241  ummarizes the RA
+000578c0: 5720 706c 6f74 7320 616e 6420 6f6e 200d  W plots and on .
+000578d0: 0a09 0974 6865 2073 6563 6f6e 6420 2869  ...the second (i
+000578e0: 6620 6578 6973 7465 6e74 2920 6974 2073  f existent) it s
+000578f0: 756d 6d61 7269 7a65 7320 7468 6520 6669  ummarizes the fi
+00057900: 7474 6564 2072 6573 756c 7473 0d0a 0909  tted results....
+00057910: 0d0a 0909 5061 7261 6d65 7465 7273 0d0a  ....Parameters..
+00057920: 0909 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 0909  ..----------....
+00057930: 0d0a 0909 7361 7665 5f52 4157 203a 2062  ....save_RAW : b
+00057940: 6f6f 6c2c 206f 7074 696f 6e61 6c0d 0a09  ool, optional...
+00057950: 0909 2844 6566 6175 6c74 2920 5472 7565  ..(Default) True
+00057960: 2074 6865 6e20 7468 6520 6669 7273 7420   then the first 
+00057970: 736c 6964 6520 7769 7468 2074 6865 2052  slide with the R
+00057980: 4157 2064 6174 6120 6973 2063 7265 6174  AW data is creat
+00057990: 6564 200d 0a09 090d 0a09 0973 6176 655f  ed ........save_
+000579a0: 4669 7420 3a20 626f 6f6c 2c20 6f70 7469  Fit : bool, opti
+000579b0: 6f6e 616c 0d0a 0909 0928 4465 6661 756c  onal.....(Defaul
+000579c0: 7429 2054 7275 6520 7468 656e 2074 6865  t) True then the
+000579d0: 2073 6563 6f6e 6420 736c 6964 6520 7769   second slide wi
+000579e0: 7468 2074 6865 2046 6974 7465 6420 6461  th the Fitted da
+000579f0: 7461 2069 7320 6372 6561 7465 6420 0d0a  ta is created ..
+00057a00: 0909 0d0a 0909 7061 7468 203a 204e 6f6e  ......path : Non
+00057a10: 652c 2073 7472 206f 7220 7061 7468 2c20  e, str or path, 
+00057a20: 6f70 7469 6f6e 616c 0d0a 0909 0928 4465  optional.....(De
+00057a30: 6661 756c 7429 204e 6f6e 652c 2069 6620  fault) None, if 
+00057a40: 6c65 6674 206f 6e20 4e6f 6e65 2c20 7468  left on None, th
+00057a50: 656e 2061 2066 6f6c 6465 7220 2272 6573  en a folder "res
+00057a60: 756c 745f 6669 6775 7265 7322 2069 7320  ult_figures" is 
+00057a70: 6372 6561 7465 6420 696e 2074 6865 2066  created in the f
+00057a80: 6f6c 6465 7220 0d0a 0909 096f 6620 7468  older .....of th
+00057a90: 6520 6461 7461 2028 7365 6c66 2e70 6174  e data (self.pat
+00057aa0: 6829 0d0a 0909 0d0a 0909 7361 7665 7479  h)........savety
+00057ab0: 7065 203a 2073 7472 206f 7220 6974 6572  pe : str or iter
+00057ac0: 6162 6c65 2028 6f66 2073 7472 292c 206f  able (of str), o
+00057ad0: 7074 696f 6e61 6c20 0d0a 0909 0974 7269  ptional .....tri
+00057ae0: 6767 6572 7320 7468 6520 6164 6469 7469  ggers the additi
+00057af0: 6f6e 616c 2063 7265 6174 696f 6e20 6f66  onal creation of
+00057b00: 2061 2063 6f6d 706f 7369 7465 2066 696c   a composite fil
+00057b10: 6520 696e 2074 6869 7320 666f 726d 6174  e in this format
+00057b20: 2e0d 0a09 0909 6d61 7470 6c6f 746c 6962  ......matplotlib
+00057b30: 2061 6c6c 6f77 7320 7468 6520 7361 7669   allows the savi
+00057b40: 6e67 206f 6620 6669 6775 7265 7320 696e  ng of figures in
+00057b50: 2076 6172 696f 7573 2066 6f72 6d61 7473   various formats
+00057b60: 2e20 2844 6566 6175 6c74 2920 2270 6e67  . (Default) "png
+00057b70: 222c 200d 0a09 0909 7479 7069 6361 6c20  ", .....typical 
+00057b80: 616e 6420 7265 636f 6d6d 656e 6461 626c  and recommendabl
+00057b90: 6520 6f70 7469 6f6e 7320 6172 6520 2273  e options are "s
+00057ba0: 7667 2220 616e 6420 2270 6466 222e 2020  vg" and "pdf".  
+00057bb0: 0d0a 0909 090d 0a09 0974 6974 6c65 203a  .........title :
+00057bc0: 204e 6f6e 6520 6f72 2073 7472 2c20 6f70   None or str, op
+00057bd0: 7469 6f6e 616c 0d0a 0909 0928 4465 6661  tional.....(Defa
+00057be0: 756c 7429 204e 6f6e 652c 2055 7365 2074  ult) None, Use t
+00057bf0: 6869 7320 7469 746c 6520 6f6e 2061 6c6c  his title on all
+00057c00: 2070 6c6f 7473 2e20 6966 204e 6f6e 652c   plots. if None,
+00057c10: 2075 7365 2073 656c 662e 6669 6c65 6e61   use self.filena
+00057c20: 6d65 0d0a 0909 090d 0a09 0966 696c 656e  me.........filen
+00057c30: 616d 6520 3a20 7374 722c 206f 7074 696f  ame : str, optio
+00057c40: 6e61 6c0d 0a09 0909 2844 6566 6175 6c74  nal.....(Default
+00057c50: 2920 4e6f 6e65 2c20 4261 7365 206e 616d  ) None, Base nam
+00057c60: 6520 666f 7220 616c 6c20 706c 6f74 732e  e for all plots.
+00057c70: 2049 6620 4e6f 6e65 2c20 7468 656e 2073   If None, then s
+00057c80: 656c 662e 6669 6c65 6e61 6d65 2077 696c  elf.filename wil
+00057c90: 6c20 6265 2075 7365 640d 0a09 0909 0d0a  l be used.......
+00057ca0: 0909 7363 616c 655f 7479 7065 203a 2073  ..scale_type : s
+00057cb0: 7472 2c20 6f70 7469 6f6e 616c 0d0a 0909  tr, optional....
+00057cc0: 0927 7379 6d6c 6f67 2720 2844 6566 6175  .'symlog' (Defau
+00057cd0: 6c74 292c 2027 6c69 6e65 6172 272c 2027  lt), 'linear', '
+00057ce0: 6c6f 6727 2074 696d 6520 6178 6973 0d0a  log' time axis..
+00057cf0: 0909 090d 0a09 0970 6174 6368 6573 203a  .......patches :
+00057d00: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0d   bool, optional.
+00057d10: 0a09 0909 466f 7220 7472 7565 2075 7365  ....For true use
+00057d20: 2077 6869 7465 2070 6174 6368 6573 2074   white patches t
+00057d30: 6f20 6c61 6265 6c20 7468 696e 6773 2069  o label things i
+00057d40: 6e20 7468 6520 3264 206d 6174 7269 7865  n the 2d matrixe
+00057d50: 732c 2074 6f20 7361 6665 0d0a 0909 0973  s, to safe.....s
+00057d60: 7061 6365 2066 6f72 2070 7562 6c69 6361  pace for publica
+00057d70: 7469 6f6e 0d0a 0909 090d 0a09 0963 6d61  tion.........cma
+00057d80: 7020 3a20 4e6f 6e65 206f 7220 6d61 7470  p : None or matp
+00057d90: 6c6f 746c 6962 2063 6f6c 6f72 206d 6170  lotlib color map
+00057da0: 2c20 6f70 7469 6f6e 616c 0d0a 0909 0969  , optional.....i
+00057db0: 7320 6120 706f 7765 7266 756c 6c20 7661  s a powerfull va
+00057dc0: 7269 6162 6c65 2074 6861 7420 6368 6f6f  riable that choo
+00057dd0: 7365 7320 7468 6520 636f 6c6f 7572 206d  ses the colour m
+00057de0: 6170 2061 7070 6c69 6564 2066 6f72 2061  ap applied for a
+00057df0: 6c6c 2070 6c6f 7473 2e20 4966 2073 6574  ll plots. If set
+00057e00: 2074 6f20 0d0a 0909 094e 6f6e 6520 2844   to .....None (D
+00057e10: 6566 6175 6c74 2920 7468 656e 2074 6865  efault) then the
+00057e20: 2073 656c 662e 636d 6170 2069 7320 7573   self.cmap is us
+00057e30: 6564 2e0d 0a09 0909 4173 2073 7461 6e64  ed......As stand
+00057e40: 6172 6420 4920 7573 6520 7468 6520 636f  ard I use the co
+00057e50: 6c6f 7220 6d61 7020 226a 6574 2220 6672  lor map "jet" fr
+00057e60: 6f6d 206d 6174 706c 6f74 6c69 622e 2054  om matplotlib. T
+00057e70: 6865 7265 2061 7265 2061 2076 6172 6965  here are a varie
+00057e80: 7479 206f 6620 636f 6c6f 726d 6170 7320  ty of colormaps 
+00057e90: 0d0a 0909 0961 7661 696c 6162 6c65 2074  .....available t
+00057ea0: 6861 7420 6172 6520 7665 7279 2075 7365  hat are very use
+00057eb0: 6675 6c6c 2e20 4265 7369 6465 2022 6a65  full. Beside "je
+00057ec0: 7422 2c20 2276 6972 6964 6973 2220 6973  t", "viridis" is
+00057ed0: 2061 2067 6f6f 6420 6368 6f69 6365 2061   a good choice a
+00057ee0: 7320 6974 2069 7320 7765 6c6c 200d 0a09  s it is well ...
+00057ef0: 0909 7669 7369 626c 6520 756e 6465 7220  ..visible under 
+00057f00: 7265 642d 6772 6565 6e20 626c 696e 646e  red-green blindn
+00057f10: 6573 732e 204f 7468 6572 2075 7365 6675  ess. Other usefu
+00057f20: 6c20 6d61 7073 2061 7265 2022 7072 6973  l maps are "pris
+00057f30: 6d22 2066 6f72 2068 6967 6820 666c 7563  m" for high fluc
+00057f40: 7475 6174 696f 6e73 200d 0a09 0909 6f72  tuations .....or
+00057f50: 2064 6976 6572 6769 6e67 2063 6f6c 6f72   diverging color
+00057f60: 206d 6170 7320 6c69 6b65 2022 7365 6973   maps like "seis
+00057f70: 6d69 6322 2e20 0d0a 0909 0953 6565 2068  mic". .....See h
+00057f80: 7474 7073 3a2f 2f6d 6174 706c 6f74 6c69  ttps://matplotli
+00057f90: 622e 6f72 672f 332e 312e 302f 7475 746f  b.org/3.1.0/tuto
+00057fa0: 7269 616c 732f 636f 6c6f 7273 2f63 6f6c  rials/colors/col
+00057fb0: 6f72 6d61 7073 2e68 746d 6c20 666f 7220  ormaps.html for 
+00057fc0: 6120 636f 6d70 7265 6865 6e73 6976 6520  a comprehensive 
+00057fd0: 0d0a 0909 0973 656c 6563 7469 6f6e 2e20  .....selection. 
+00057fe0: 496e 2074 6865 2063 6f64 6520 7468 6520  In the code the 
+00057ff0: 636f 6c6f 726d 6170 7320 6172 6520 696d  colormaps are im
+00058000: 706f 7274 6564 2073 6f20 6966 2070 6c6f  ported so if plo
+00058010: 745f 6675 6e63 2069 7320 696d 706f 7274  t_func is import
+00058020: 6564 2061 7320 7066 2074 6865 6e20 0d0a  ed as pf then ..
+00058030: 0909 0973 656c 662e 636d 6170 3d70 662e  ...self.cmap=pf.
+00058040: 636d 2e76 6972 6964 6973 2073 6574 7320  cm.viridis sets 
+00058050: 7669 7269 6469 7320 6173 2074 6865 206d  viridis as the m
+00058060: 6170 2074 6f20 7573 652e 2049 6e74 6572  ap to use. Inter
+00058070: 6e61 6c6c 7920 7468 6520 636f 6c6f 7273  nally the colors
+00058080: 2061 7265 2063 686f 7365 6e20 0d0a 0909   are chosen ....
+00058090: 0977 6974 6820 7468 6520 2263 6f6c 6d22  .with the "colm"
+000580a0: 2066 756e 6374 696f 6e2e 2054 6865 2032   function. The 2
+000580b0: 6420 706c 6f74 7320 7265 7175 6972 6520  d plots require 
+000580c0: 6120 636f 6e74 696e 756f 7573 2063 6f6c  a continuous col
+000580d0: 6f72 206d 6170 2073 6f20 6966 2073 6f6d  or map so if som
+000580e0: 6574 6869 6e67 200d 0a09 0909 656c 7365  ething .....else
+000580f0: 2069 7320 6769 7665 2032 6420 706c 6f74   is give 2d plot
+00058100: 7320 6172 6520 7368 6f77 6e20 6175 746f  s are shown auto
+00058110: 6d61 7469 6361 6c6c 7920 7769 7468 2022  matically with "
+00058120: 6a65 7422 2e20 466f 7220 616c 6c20 6f66  jet". For all of
+00058130: 2074 6865 2031 6420 706c 6f74 7320 686f   the 1d plots ho
+00058140: 7765 7665 7220 0d0a 0909 0949 2066 6972  wever .....I fir
+00058150: 7374 2073 656c 6563 7420 6120 6e75 6d62  st select a numb
+00058160: 6572 206f 6620 636f 6c6f 7273 2062 6566  er of colors bef
+00058170: 6f72 6520 6561 6368 2070 6c6f 742e 2049  ore each plot. I
+00058180: 6620 636d 6170 2069 7320 6120 636f 6e74  f cmap is a cont
+00058190: 696e 6f75 7320 6d61 7020 7468 656e 2074  inous map then t
+000581a0: 6865 7365 0d0a 0909 0961 7265 2073 616d  hese.....are sam
+000581b0: 706c 6564 2065 7665 6e6c 7920 6f76 6572  pled evenly over
+000581c0: 2074 6865 2063 6f6c 6f75 726d 6170 2e20   the colourmap. 
+000581d0: 4d61 6e75 616c 2069 7465 7261 626c 6573  Manual iterables
+000581e0: 206f 6620 636f 6c6f 7572 7320 0d0a 0909   of colours ....
+000581f0: 0963 6d61 703d 5b28 312c 302c 3029 2c28  .cmap=[(1,0,0),(
+00058200: 302c 312c 3029 2c28 302c 302c 3129 2c2e  0,1,0),(0,0,1),.
+00058210: 2e2e 5d20 6172 6520 616c 736f 2061 6363  ..] are also acc
+00058220: 6570 7465 642c 2061 7320 6172 6520 7665  epted, as are ve
+00058230: 6374 6f72 7320 6f72 2064 6174 6166 7261  ctors or datafra
+00058240: 6d65 7320 7468 6174 200d 0a09 0909 636f  mes that .....co
+00058250: 6e74 6169 6e20 6173 2072 6f77 7320 7468  ntain as rows th
+00058260: 6520 636f 6c6f 7273 2e20 5468 6572 6520  e colors. There 
+00058270: 6d75 7374 2062 6520 6f66 2063 6f75 7273  must be of cours
+00058280: 6520 7375 6666 6963 6965 6e74 2063 6f6c  e sufficient col
+00058290: 6f72 7320 7072 6573 656e 7420 666f 7220  ors present for 
+000582a0: 0d0a 0909 0974 6865 206e 756d 6265 7273  .....the numbers
+000582b0: 206f 6620 6c69 6e65 7320 7468 6174 2077   of lines that w
+000582c0: 696c 6c20 6265 2070 6c6f 7474 6564 2e20  ill be plotted. 
+000582d0: 536f 2049 2072 6563 6f6d 6d65 6e64 2074  So I recommend t
+000582e0: 6f20 7072 6f76 6964 6520 6174 206c 6561  o provide at lea
+000582f0: 7374 2031 3020 636f 6c6f 7572 7320 0d0a  st 10 colours ..
+00058300: 0909 0928 652e 672e 7e79 6f75 7220 756e  ...(e.g.~your un
+00058310: 6976 6572 7369 7479 2063 6f6c 6f72 7329  iversity colors)
+00058320: 2e20 636f 6c6f 7572 7320 6172 6520 616c  . colours are al
+00058330: 7761 7973 2067 6976 656e 2061 7320 612c  ways given as a,
+00058340: 206c 6973 7420 6f72 2074 7570 6c65 2077   list or tuple w
+00058350: 6974 6820 5247 4120 6f72 2052 4742 410d  ith RGA or RGBA.
+00058360: 0a09 0909 2877 6974 6820 7468 6520 6c61  ....(with the la
+00058370: 7374 2041 2062 6565 696e 6720 7468 6520  st A beeing the 
+00058380: 416c 7068 613d 7472 616e 7370 6172 656e  Alpha=transparen
+00058390: 6379 2e20 416c 6c20 6e75 6d62 6572 7320  cy. All numbers 
+000583a0: 6172 6520 6265 7477 6565 6e20 3020 616e  are between 0 an
+000583b0: 6420 312e 200d 0a09 0909 4966 2061 206c  d 1. .....If a l
+000583c0: 6973 742f 7665 6374 6f72 2f44 6174 6146  ist/vector/DataF
+000583d0: 7261 6d65 2069 7320 6769 7665 6e20 666f  rame is given fo
+000583e0: 7220 7468 6520 636f 6c6f 7572 7320 7468  r the colours th
+000583f0: 6579 2077 696c 6c20 6265 2075 7365 6420  ey will be used 
+00058400: 696e 2074 6865 206f 7264 6572 2070 726f  in the order pro
+00058410: 7669 6465 642e 0d0a 0909 0d0a 0909 4578  vided.........Ex
+00058420: 616d 706c 6573 0d0a 0909 2d2d 2d2d 2d2d  amples....------
+00058430: 2d2d 2d0d 0a09 090d 0a09 093e 3e3e 2074  ---........>>> t
+00058440: 612e 5361 7665 5f50 6f77 6572 706f 696e  a.Save_Powerpoin
+00058450: 7428 290d 0a09 093e 3e3e 2074 612e 5361  t()....>>> ta.Sa
+00058460: 7665 5f50 6f77 6572 706f 696e 7428 7061  ve_Powerpoint(pa
+00058470: 7463 6865 7320 3d20 5472 7565 290d 0a09  tches = True)...
+00058480: 090d 0a09 0927 2727 0909 0909 0909 200d  .....'''...... .
+00058490: 0a09 0969 6620 6973 696e 7374 616e 6365  ...if isinstance
+000584a0: 2873 6176 6574 7970 652c 7479 7065 2827  (savetype,type('
+000584b0: 6865 6c6c 6f27 2929 3a73 6176 6574 7970  hello')):savetyp
 000584c0: 653d 5b73 6176 6574 7970 655d 0d0a 0909  e=[savetype]....
-000584d0: 7261 775f 6e61 6d65 733d 5b22 4d41 5422  raw_names=["MAT"
-000584e0: 2c22 5345 4c22 2c22 5350 454b 222c 2253  ,"SEL","SPEK","S
-000584f0: 5644 225d 0d0a 0909 7261 775f 6e61 6d65  VD"]....raw_name
-00058500: 733d 5b63 6865 636b 5f66 6f6c 6465 7228  s=[check_folder(
-00058510: 6375 7272 656e 745f 7061 7468 3d73 656c  current_path=sel
-00058520: 662e 7061 7468 2c20 7061 7468 3d70 6174  f.path, path=pat
-00058530: 682c 2066 696c 656e 616d 653d 7365 6c66  h, filename=self
-00058540: 2e66 696c 656e 616d 652e 7370 6c69 7428  .filename.split(
-00058550: 272e 2729 5b30 5d20 2b20 225f 5241 575f  '.')[0] + "_RAW_
-00058560: 222b 7374 7228 6129 202b 222e 706e 6722  "+str(a) +".png"
-00058570: 2920 666f 7220 6120 696e 2072 6177 5f6e  ) for a in raw_n
-00058580: 616d 6573 5d0d 0a09 0966 6974 5f6e 616d  ames]....fit_nam
-00058590: 6573 3d5b 2246 4947 5f4d 4154 222c 2253  es=["FIG_MAT","S
-000585a0: 5045 4322 2c22 5345 4c22 2c22 5355 4d22  PEC","SEL","SUM"
-000585b0: 2c22 4441 4322 5d0d 0a09 0966 6974 5f6e  ,"DAC"]....fit_n
-000585c0: 616d 6573 3d5b 6368 6563 6b5f 666f 6c64  ames=[check_fold
-000585d0: 6572 2863 7572 7265 6e74 5f70 6174 683d  er(current_path=
-000585e0: 7365 6c66 2e70 6174 682c 2070 6174 683d  self.path, path=
-000585f0: 7061 7468 2c20 6669 6c65 6e61 6d65 3d73  path, filename=s
-00058600: 656c 662e 6669 6c65 6e61 6d65 2e73 706c  elf.filename.spl
-00058610: 6974 2827 2e27 295b 305d 202b 2022 5f22  it('.')[0] + "_"
-00058620: 202b 7374 7228 6129 202b 222e 706e 6722   +str(a) +".png"
-00058630: 2920 666f 7220 6120 696e 2066 6974 5f6e  ) for a in fit_n
-00058640: 616d 6573 5d0d 0a09 0970 6c74 2e63 6c6f  ames]....plt.clo
-00058650: 7365 2827 616c 6c27 290d 0a09 096f 7269  se('all')....ori
-00058660: 6769 6e3d 7365 6c66 2e73 6176 655f 6669  gin=self.save_fi
-00058670: 6775 7265 735f 746f 5f66 6f6c 6465 720d  gures_to_folder.
-00058680: 0a09 0969 6620 6669 6c65 6e61 6d65 2069  ...if filename i
-00058690: 7320 4e6f 6e65 3a0d 0a09 0909 6669 6c65  s None:.....file
-000586a0: 6e61 6d65 3d73 656c 662e 6669 6c65 6e61  name=self.filena
-000586b0: 6d65 0d0a 0909 0966 696c 656e 616d 653d  me.....filename=
-000586c0: 6669 6c65 6e61 6d65 2e73 706c 6974 2827  filename.split('
-000586d0: 2e27 295b 305d 0d0a 0909 6966 2073 6176  .')[0]....if sav
-000586e0: 655f 5241 573a 0d0a 0909 0973 656c 662e  e_RAW:.....self.
-000586f0: 7361 7665 5f66 6967 7572 6573 5f74 6f5f  save_figures_to_
-00058700: 666f 6c64 6572 3d54 7275 650d 0a09 0909  folder=True.....
-00058710: 7365 6c66 2e50 6c6f 745f 5241 5728 7361  self.Plot_RAW(sa
-00058720: 7665 7479 7065 203d 2027 706e 6727 2c20  vetype = 'png', 
-00058730: 7363 616c 655f 7479 7065 203d 2073 6361  scale_type = sca
-00058740: 6c65 5f74 7970 652c 2074 6974 6c65 203d  le_type, title =
-00058750: 2074 6974 6c65 2c20 636d 6170 203d 2063   title, cmap = c
-00058760: 6d61 702c 2070 6174 6820 3d20 7061 7468  map, path = path
-00058770: 2909 0d0a 0909 0970 6c74 2e63 6c6f 7365  )......plt.close
-00058780: 2827 616c 6c27 290d 0a09 0969 6620 7361  ('all')....if sa
-00058790: 7665 5f46 6974 3a0d 0a09 0909 7472 793a  ve_Fit:.....try:
-000587a0: 0d0a 0909 0909 7365 6c66 2e73 6176 655f  ......self.save_
-000587b0: 6669 6775 7265 735f 746f 5f66 6f6c 6465  figures_to_folde
-000587c0: 723d 5472 7565 0d0a 0909 0909 7365 6c66  r=True......self
-000587d0: 2e50 6c6f 745f 6669 745f 6f75 7470 7574  .Plot_fit_output
-000587e0: 2873 6176 6574 7970 6520 3d20 2770 6e67  (savetype = 'png
-000587f0: 272c 2073 6361 6c65 5f74 7970 6520 3d20  ', scale_type = 
-00058800: 7363 616c 655f 7479 7065 2c20 7469 746c  scale_type, titl
-00058810: 6520 3d20 7469 746c 652c 2070 6174 6368  e = title, patch
-00058820: 6573 203d 2070 6174 6368 6573 2c20 636d  es = patches, cm
-00058830: 6170 203d 2063 6d61 7020 2c20 7061 7468  ap = cmap , path
-00058840: 203d 2070 6174 6829 0d0a 0909 0909 706c   = path)......pl
-00058850: 742e 636c 6f73 6528 2761 6c6c 2729 0d0a  t.close('all')..
-00058860: 0909 0965 7863 6570 743a 0d0a 0909 0909  ...except:......
-00058870: 7361 7665 5f46 6974 203d 2046 616c 7365  save_Fit = False
-00058880: 0d0a 0909 0909 7072 696e 7428 2772 756e  ......print('run
-00058890: 2069 6e74 6f20 7072 6f62 6c65 6d73 2077   into problems w
-000588a0: 6974 6820 6164 6469 6e67 2074 6865 2066  ith adding the f
-000588b0: 6974 2072 6573 756c 7473 2e20 4861 7665  it results. Have
-000588c0: 2079 6f75 2066 6974 7465 6420 736f 6d65   you fitted some
-000588d0: 7468 696e 673f 2729 0d0a 0909 0974 7279  thing?').....try
-000588e0: 3a0d 0a09 0909 0952 6573 756c 745f 7374  :......Result_st
-000588f0: 7269 6e67 3d27 5c6e 4669 7420 5265 7375  ring='\nFit Resu
-00058900: 6c74 733a 5c6e 270d 0a09 0909 0969 6620  lts:\n'......if 
-00058910: 6973 696e 7374 616e 6365 2873 656c 662e  isinstance(self.
-00058920: 6d6f 642c 7479 7065 2827 6865 6c6c 6f27  mod,type('hello'
-00058930: 2929 3a0d 0a09 0909 0909 5265 7375 6c74  )):.......Result
-00058940: 5f73 7472 696e 672b 3d27 4d6f 6465 6c20  _string+='Model 
-00058950: 5573 6564 3a20 2573 5c6e 5c6e 2725 7365  Used: %s\n\n'%se
-00058960: 6c66 2e6d 6f64 0d0a 0909 0909 656c 7365  lf.mod......else
-00058970: 3a0d 0a09 0909 0909 5265 7375 6c74 5f73  :.......Result_s
-00058980: 7472 696e 672b 3d27 4d6f 6465 6c20 5573  tring+='Model Us
-00058990: 6564 3a20 4578 7465 726e 616c 2066 756e  ed: External fun
-000589a0: 6374 696f 6e5c 6e5c 6e27 0d0a 0909 0909  ction\n\n'......
-000589b0: 6966 2073 656c 662e 6967 6e6f 7265 5f74  if self.ignore_t
-000589c0: 696d 655f 7265 6769 6f6e 2069 7320 6e6f  ime_region is no
-000589d0: 7420 4e6f 6e65 3a0d 0a09 0909 0909 5265  t None:.......Re
-000589e0: 7375 6c74 5f73 7472 696e 672b 3d27 7468  sult_string+='th
-000589f0: 6520 7469 6d65 2062 6574 7765 656e 2025  e time between %
-00058a00: 2e33 6620 2573 2061 6e64 2025 2e33 6620  .3f %s and %.3f 
-00058a10: 2573 205c 6e20 7761 7320 6578 636c 7564  %s \n was exclud
-00058a20: 6564 2066 726f 6d20 7468 6520 6f70 7469  ed from the opti
-00058a30: 6d69 7a61 7469 6f6e 5c6e 2725 2873 656c  mization\n'%(sel
-00058a40: 662e 6967 6e6f 7265 5f74 696d 655f 7265  f.ignore_time_re
-00058a50: 6769 6f6e 5b30 5d2c 7365 6c66 2e62 6173  gion[0],self.bas
-00058a60: 6575 6e69 742c 7365 6c66 2e69 676e 6f72  eunit,self.ignor
-00058a70: 655f 7469 6d65 5f72 6567 696f 6e5b 315d  e_time_region[1]
-00058a80: 2c73 656c 662e 6261 7365 756e 6974 2909  ,self.baseunit).
-00058a90: 0d0a 0909 0909 5265 7375 6c74 5f73 7472  ......Result_str
-00058aa0: 696e 672b 3d27 5468 6520 6d69 6e69 6d75  ing+='The minimu
-00058ab0: 6d20 6572 726f 7220 6973 3a7b 3a2e 3865  m error is:{:.8e
-00058ac0: 7d5c 6e27 2e66 6f72 6d61 7428 7365 6c66  }\n'.format(self
-00058ad0: 2e72 655b 2765 7272 6f72 275d 290d 0a09  .re['error'])...
-00058ae0: 0909 0952 6573 756c 745f 7374 7269 6e67  ...Result_string
-00058af0: 2b3d 2754 6865 206d 696e 696d 756d 2052  +='The minimum R
-00058b00: 322d 7661 6c75 6520 6973 3a7b 3a2e 3865  2-value is:{:.8e
-00058b10: 7d5c 6e27 2e66 6f72 6d61 7428 7365 6c66  }\n'.format(self
-00058b20: 2e72 655b 2772 3227 5d29 0d0a 0909 0909  .re['r2'])......
-00058b30: 6966 2027 636f 6e66 6964 656e 6365 2720  if 'confidence' 
-00058b40: 696e 2073 656c 662e 7265 3a0d 0a09 0909  in self.re:.....
-00058b50: 0909 5265 7375 6c74 5f73 7472 696e 672b  ..Result_string+
-00058b60: 3d27 5c6e 496e 2052 6174 6573 2077 6974  ='\nIn Rates wit
-00058b70: 6820 636f 6e66 6964 656e 6365 2069 6e74  h confidence int
-00058b80: 6572 7661 6c20 746f 206c 6576 656c 206f  erval to level o
-00058b90: 6620 2573 5c6e 2725 7365 6c66 2e72 655b  f %s\n'%self.re[
-00058ba0: 2763 6f6e 6669 6465 6e63 6527 5d5b 2774  'confidence']['t
-00058bb0: 6172 6765 742d 6c65 7665 6c27 5d0d 0a09  arget-level']...
-00058bc0: 0909 0909 5265 7375 6c74 5f73 7472 696e  ....Result_strin
-00058bd0: 672b 3d73 656c 662e 7265 5b27 6669 745f  g+=self.re['fit_
-00058be0: 7265 7375 6c74 735f 7261 7465 7327 5d2e  results_rates'].
-00058bf0: 746f 5f73 7472 696e 6728 636f 6c75 6d6e  to_string(column
-00058c00: 733d 5b27 7661 6c75 6527 2c27 6c6f 7765  s=['value','lowe
-00058c10: 725f 6c69 6d69 7427 2c27 7570 7065 725f  r_limit','upper_
-00058c20: 6c69 6d69 7427 2c27 696e 6974 5f76 616c  limit','init_val
-00058c30: 7565 272c 2776 6172 7927 2c27 6d69 6e27  ue','vary','min'
-00058c40: 2c27 6d61 7827 2c27 6578 7072 275d 290d  ,'max','expr']).
-00058c50: 0a09 0909 0909 5265 7375 6c74 5f73 7472  ......Result_str
-00058c60: 696e 672b 3d27 5c6e 5c6e 5468 6520 7261  ing+='\n\nThe ra
-00058c70: 7465 7320 636f 6e76 6572 7465 6420 746f  tes converted to
-00058c80: 2074 696d 6573 2077 6974 6820 756e 6974   times with unit
-00058c90: 2025 735c 6e20 7769 7468 2063 6f6e 6669   %s\n with confi
-00058ca0: 6465 6e63 6520 696e 7465 7276 616c 2074  dence interval t
-00058cb0: 6f20 6c65 7665 6c20 6f66 2025 735c 6e27  o level of %s\n'
-00058cc0: 2528 7365 6c66 2e62 6173 6575 6e69 742c  %(self.baseunit,
-00058cd0: 7365 6c66 2e72 655b 2763 6f6e 6669 6465  self.re['confide
-00058ce0: 6e63 6527 5d5b 2774 6172 6765 742d 6c65  nce']['target-le
-00058cf0: 7665 6c27 5d29 0d0a 0909 0909 0952 6573  vel']).......Res
-00058d00: 756c 745f 7374 7269 6e67 2b3d 7365 6c66  ult_string+=self
-00058d10: 2e72 655b 2766 6974 5f72 6573 756c 7473  .re['fit_results
-00058d20: 5f74 696d 6573 275d 2e74 6f5f 7374 7269  _times'].to_stri
-00058d30: 6e67 2863 6f6c 756d 6e73 3d5b 2776 616c  ng(columns=['val
-00058d40: 7565 272c 276c 6f77 6572 5f6c 696d 6974  ue','lower_limit
-00058d50: 272c 2775 7070 6572 5f6c 696d 6974 272c  ','upper_limit',
-00058d60: 2769 6e69 745f 7661 6c75 6527 2c27 7661  'init_value','va
-00058d70: 7279 272c 276d 696e 272c 276d 6178 272c  ry','min','max',
-00058d80: 2765 7870 7227 5d29 0d0a 0909 0909 656c  'expr'])......el
-00058d90: 7365 3a0d 0a09 0909 0909 5265 7375 6c74  se:.......Result
-00058da0: 5f73 7472 696e 672b 3d27 5c6e 496e 2052  _string+='\nIn R
-00058db0: 6174 6573 5c6e 270d 0a09 0909 0909 5265  ates\n'.......Re
-00058dc0: 7375 6c74 5f73 7472 696e 672b 3d73 656c  sult_string+=sel
-00058dd0: 662e 7265 5b27 6669 745f 7265 7375 6c74  f.re['fit_result
-00058de0: 735f 7261 7465 7327 5d2e 746f 5f73 7472  s_rates'].to_str
-00058df0: 696e 6728 636f 6c75 6d6e 733d 5b27 7661  ing(columns=['va
-00058e00: 6c75 6527 2c27 696e 6974 5f76 616c 7565  lue','init_value
-00058e10: 272c 2776 6172 7927 2c27 6d69 6e27 2c27  ','vary','min','
-00058e20: 6d61 7827 2c27 6578 7072 275d 290d 0a09  max','expr'])...
-00058e30: 0909 0909 5265 7375 6c74 5f73 7472 696e  ....Result_strin
-00058e40: 672b 3d27 5c6e 5c6e 5468 6520 7261 7465  g+='\n\nThe rate
-00058e50: 7320 636f 6e76 6572 7465 6420 746f 2074  s converted to t
-00058e60: 696d 6573 2077 6974 6820 756e 6974 2025  imes with unit %
-00058e70: 735c 6e27 2573 656c 662e 6261 7365 756e  s\n'%self.baseun
-00058e80: 6974 0d0a 0909 0909 0952 6573 756c 745f  it.......Result_
-00058e90: 7374 7269 6e67 2b3d 7365 6c66 2e72 655b  string+=self.re[
-00058ea0: 2766 6974 5f72 6573 756c 7473 5f74 696d  'fit_results_tim
-00058eb0: 6573 275d 2e74 6f5f 7374 7269 6e67 2863  es'].to_string(c
-00058ec0: 6f6c 756d 6e73 3d5b 2776 616c 7565 272c  olumns=['value',
-00058ed0: 2769 6e69 745f 7661 6c75 6527 2c27 7661  'init_value','va
-00058ee0: 7279 272c 276d 696e 272c 276d 6178 272c  ry','min','max',
-00058ef0: 2765 7870 7227 5d29 0d0a 0909 0965 7863  'expr']).....exc
-00058f00: 6570 743a 0d0a 0909 0909 7061 7373 0d0a  ept:......pass..
-00058f10: 0909 6966 2028 2770 6466 2720 696e 2073  ..if ('pdf' in s
-00058f20: 6176 6574 7970 6529 206f 7220 2827 706e  avetype) or ('pn
-00058f30: 6727 2069 6e20 7361 7665 7479 7065 2920  g' in savetype) 
-00058f40: 6f72 2028 2773 7667 2720 696e 2073 6176  or ('svg' in sav
-00058f50: 6574 7970 6529 3a0d 0a09 0909 6966 2073  etype):.....if s
-00058f60: 6176 655f 5241 573a 0d0a 0909 0909 6669  ave_RAW:......fi
-00058f70: 672c 6178 3d70 6c74 2e73 7562 706c 6f74  g,ax=plt.subplot
-00058f80: 7328 6e72 6f77 733d 322c 6e63 6f6c 733d  s(nrows=2,ncols=
-00058f90: 322c 6669 6773 697a 653d 2831 302c 372e  2,figsize=(10,7.
-00058fa0: 3529 290d 0a09 0909 0961 785b 302c 315d  5))......ax[0,1]
-00058fb0: 2e69 6d73 686f 7728 6d70 696d 672e 696d  .imshow(mpimg.im
-00058fc0: 7265 6164 2873 7472 2872 6177 5f6e 616d  read(str(raw_nam
-00058fd0: 6573 5b30 5d29 2929 0d0a 0909 0909 6178  es[0])))......ax
-00058fe0: 5b30 2c30 5d2e 696d 7368 6f77 286d 7069  [0,0].imshow(mpi
-00058ff0: 6d67 2e69 6d72 6561 6428 7374 7228 7261  mg.imread(str(ra
-00059000: 775f 6e61 6d65 735b 315d 2929 290d 0a09  w_names[1])))...
-00059010: 0909 0961 785b 312c 305d 2e69 6d73 686f  ...ax[1,0].imsho
-00059020: 7728 6d70 696d 672e 696d 7265 6164 2873  w(mpimg.imread(s
-00059030: 7472 2872 6177 5f6e 616d 6573 5b32 5d29  tr(raw_names[2])
-00059040: 2929 0d0a 0909 0909 6178 5b31 2c31 5d2e  ))......ax[1,1].
-00059050: 696d 7368 6f77 286d 7069 6d67 2e69 6d72  imshow(mpimg.imr
-00059060: 6561 6428 7374 7228 7261 775f 6e61 6d65  ead(str(raw_name
-00059070: 735b 335d 2929 290d 0a09 0909 0961 785b  s[3])))......ax[
-00059080: 302c 305d 2e61 7869 7328 276f 6666 2729  0,0].axis('off')
-00059090: 3b61 785b 312c 305d 2e61 7869 7328 276f  ;ax[1,0].axis('o
-000590a0: 6666 2729 3b61 785b 302c 315d 2e61 7869  ff');ax[0,1].axi
-000590b0: 7328 276f 6666 2729 3b61 785b 312c 315d  s('off');ax[1,1]
-000590c0: 2e61 7869 7328 276f 6666 2729 0d0a 0909  .axis('off')....
-000590d0: 0909 666f 7220 656e 7472 7920 696e 2073  ..for entry in s
-000590e0: 6176 6574 7970 653a 0d0a 0909 0909 0969  avetype:.......i
-000590f0: 6620 656e 7472 7920 3d3d 2022 7070 7478  f entry == "pptx
-00059100: 223a 636f 6e74 696e 7565 0d0a 0909 0909  ":continue......
-00059110: 0974 7279 3a0d 0a09 0909 0909 0966 6967  .try:........fig
-00059120: 2e74 6967 6874 5f6c 6179 6f75 7428 290d  .tight_layout().
-00059130: 0a09 0909 0909 0966 6967 2e73 6176 6566  .......fig.savef
-00059140: 6967 2863 6865 636b 5f66 6f6c 6465 7228  ig(check_folder(
-00059150: 7061 7468 3d70 6174 682c 6375 7272 656e  path=path,curren
-00059160: 745f 7061 7468 3d73 656c 662e 7061 7468  t_path=self.path
-00059170: 2c66 696c 656e 616d 653d 7365 6c66 2e66  ,filename=self.f
-00059180: 696c 656e 616d 652e 7370 6c69 7428 272e  ilename.split('.
-00059190: 2729 5b30 5d20 2b20 275f 5241 572d 7375  ')[0] + '_RAW-su
-000591a0: 6d6d 6172 792e 2573 2725 656e 7472 7929  mmary.%s'%entry)
-000591b0: 2c64 7069 3d36 3030 290d 0a09 0909 0909  ,dpi=600).......
-000591c0: 6578 6365 7074 3a0d 0a09 0909 0909 0970  except:........p
-000591d0: 7269 6e74 2822 7361 7669 6e67 2069 6e22  rint("saving in"
-000591e0: 202b 2065 6e74 7279 202b 2266 6169 6c65   + entry +"faile
-000591f0: 6422 290d 0a09 0909 6966 2073 6176 655f  d").....if save_
-00059200: 4669 743a 0d0a 0909 0909 4720 3d20 4772  Fit:......G = Gr
-00059210: 6964 5370 6563 2834 2c20 3829 0d0a 0909  idSpec(4, 8)....
-00059220: 0909 6669 6731 3d70 6c74 2e66 6967 7572  ..fig1=plt.figur
-00059230: 6528 6669 6773 697a 653d 2831 302c 372e  e(figsize=(10,7.
-00059240: 3529 290d 0a09 0909 0961 7831 3d66 6967  5))......ax1=fig
-00059250: 312e 6164 645f 7375 6270 6c6f 7428 475b  1.add_subplot(G[
-00059260: 302c 3a36 5d29 0d0a 0909 0909 6178 323d  0,:6])......ax2=
-00059270: 6669 6731 2e61 6464 5f73 7562 706c 6f74  fig1.add_subplot
-00059280: 2847 5b31 2c3a 365d 290d 0a09 0909 0961  (G[1,:6])......a
-00059290: 7833 3d66 6967 312e 6164 645f 7375 6270  x3=fig1.add_subp
-000592a0: 6c6f 7428 475b 322c 3a36 5d29 0d0a 0909  lot(G[2,:6])....
-000592b0: 0909 6178 343d 6669 6731 2e61 6464 5f73  ..ax4=fig1.add_s
-000592c0: 7562 706c 6f74 2847 5b33 2c3a 365d 290d  ubplot(G[3,:6]).
-000592d0: 0a09 0909 0961 7835 3d66 6967 312e 6164  .....ax5=fig1.ad
-000592e0: 645f 7375 6270 6c6f 7428 475b 303a 322c  d_subplot(G[0:2,
-000592f0: 353a 5d29 0d0a 0909 0909 6178 363d 6669  5:])......ax6=fi
-00059300: 6731 2e61 6464 5f73 7562 706c 6f74 2847  g1.add_subplot(G
-00059310: 5b32 3a2c 363a 5d29 0d0a 0909 0909 6178  [2:,6:])......ax
-00059320: 312e 696d 7368 6f77 286d 7069 6d67 2e69  1.imshow(mpimg.i
-00059330: 6d72 6561 6428 7374 7228 6669 745f 6e61  mread(str(fit_na
-00059340: 6d65 735b 315d 2929 290d 0a09 0909 0961  mes[1])))......a
-00059350: 7832 2e69 6d73 686f 7728 6d70 696d 672e  x2.imshow(mpimg.
-00059360: 696d 7265 6164 2873 7472 2866 6974 5f6e  imread(str(fit_n
-00059370: 616d 6573 5b32 5d29 2929 0d0a 0909 0909  ames[2])))......
-00059380: 6178 332e 696d 7368 6f77 286d 7069 6d67  ax3.imshow(mpimg
-00059390: 2e69 6d72 6561 6428 7374 7228 6669 745f  .imread(str(fit_
-000593a0: 6e61 6d65 735b 335d 2929 290d 0a09 0909  names[3]))).....
-000593b0: 0961 7834 2e69 6d73 686f 7728 6d70 696d  .ax4.imshow(mpim
-000593c0: 672e 696d 7265 6164 2873 7472 2866 6974  g.imread(str(fit
-000593d0: 5f6e 616d 6573 5b34 5d29 2929 0d0a 0909  _names[4])))....
-000593e0: 0909 6178 352e 696d 7368 6f77 286d 7069  ..ax5.imshow(mpi
-000593f0: 6d67 2e69 6d72 6561 6428 7374 7228 6669  mg.imread(str(fi
-00059400: 745f 6e61 6d65 735b 305d 2929 290d 0a09  t_names[0])))...
-00059410: 0909 0961 7836 2e74 6578 7428 302c 302c  ...ax6.text(0,0,
-00059420: 5265 7375 6c74 5f73 7472 696e 672c 666f  Result_string,fo
-00059430: 6e74 7369 7a65 3d37 2c66 6f6e 7477 6569  ntsize=7,fontwei
-00059440: 6768 743d 276e 6f72 6d61 6c27 290d 0a09  ght='normal')...
-00059450: 0909 0961 7831 2e61 7869 7328 276f 6666  ...ax1.axis('off
-00059460: 2729 3b61 7832 2e61 7869 7328 276f 6666  ');ax2.axis('off
-00059470: 2729 3b61 7833 2e61 7869 7328 276f 6666  ');ax3.axis('off
-00059480: 2729 3b61 7834 2e61 7869 7328 276f 6666  ');ax4.axis('off
-00059490: 2729 3b61 7835 2e61 7869 7328 276f 6666  ');ax5.axis('off
-000594a0: 2729 3b61 7836 2e61 7869 7328 276f 6666  ');ax6.axis('off
-000594b0: 2729 0d0a 0909 0909 666f 7220 656e 7472  ')......for entr
-000594c0: 7920 696e 2073 6176 6574 7970 653a 0d0a  y in savetype:..
-000594d0: 0909 0909 0969 6620 656e 7472 7920 3d3d  .....if entry ==
-000594e0: 2022 7070 7478 223a 2063 6f6e 7469 6e75   "pptx": continu
-000594f0: 650d 0a09 0909 0909 7472 793a 0d0a 0909  e.......try:....
-00059500: 0909 0909 6669 6731 2e74 6967 6874 5f6c  ....fig1.tight_l
-00059510: 6179 6f75 7428 290d 0a09 0909 0909 0966  ayout()........f
-00059520: 6967 312e 7361 7665 6669 6728 6368 6563  ig1.savefig(chec
-00059530: 6b5f 666f 6c64 6572 2870 6174 683d 7061  k_folder(path=pa
-00059540: 7468 2c63 7572 7265 6e74 5f70 6174 683d  th,current_path=
-00059550: 7365 6c66 2e70 6174 682c 6669 6c65 6e61  self.path,filena
-00059560: 6d65 3d73 656c 662e 6669 6c65 6e61 6d65  me=self.filename
-00059570: 2e73 706c 6974 2827 2e27 295b 305d 202b  .split('.')[0] +
-00059580: 2027 5f46 6974 2d73 756d 6d61 7279 2e25   '_Fit-summary.%
-00059590: 7327 2565 6e74 7279 292c 6470 693d 3630  s'%entry),dpi=60
-000595a0: 3029 0d0a 0909 0909 0965 7863 6570 743a  0).......except:
-000595b0: 0d0a 0909 0909 0909 7072 696e 7428 2273  ........print("s
-000595c0: 6176 696e 6720 696e 2220 2b20 656e 7472  aving in" + entr
-000595d0: 7920 2b22 6661 696c 6564 2229 0d0a 0909  y +"failed")....
-000595e0: 6966 2028 2770 7074 7827 2069 6e20 7361  if ('pptx' in sa
-000595f0: 7665 7479 7065 2920 6f72 2028 2770 7074  vetype) or ('ppt
-00059600: 2720 696e 2073 6176 6574 7970 6529 3a0d  ' in savetype):.
-00059610: 0a09 0909 6c65 6674 3d49 6e63 6865 7328  ....left=Inches(
-00059620: 302e 3229 0d0a 0909 0974 6f70 3d49 6e63  0.2).....top=Inc
-00059630: 6865 7328 302e 3229 0d0a 0909 0970 7273  hes(0.2).....prs
-00059640: 203d 2050 7265 7365 6e74 6174 696f 6e28   = Presentation(
-00059650: 290d 0a09 0909 626c 616e 6b5f 736c 6964  ).....blank_slid
-00059660: 655f 6c61 796f 7574 203d 2070 7273 2e73  e_layout = prs.s
-00059670: 6c69 6465 5f6c 6179 6f75 7473 5b36 5d0d  lide_layouts[6].
-00059680: 0a09 0909 736c 6964 6520 3d20 7072 732e  ....slide = prs.
-00059690: 736c 6964 6573 2e61 6464 5f73 6c69 6465  slides.add_slide
-000596a0: 2862 6c61 6e6b 5f73 6c69 6465 5f6c 6179  (blank_slide_lay
-000596b0: 6f75 7429 0d0a 0909 0969 6620 7361 7665  out).....if save
-000596c0: 5f52 4157 3a0d 0a09 0909 096c 6566 7420  _RAW:......left 
-000596d0: 3d20 746f 7020 3d20 496e 6368 6573 2830  = top = Inches(0
-000596e0: 2e35 290d 0a09 0909 0970 6963 203d 2073  .5)......pic = s
-000596f0: 6c69 6465 2e73 6861 7065 732e 6164 645f  lide.shapes.add_
-00059700: 7069 6374 7572 6528 7374 7228 7261 775f  picture(str(raw_
-00059710: 6e61 6d65 735b 305d 2e72 6573 6f6c 7665  names[0].resolve
-00059720: 2829 292c 206c 6566 743d 6c65 6674 2b49  ()), left=left+I
-00059730: 6e63 6865 7328 342e 3529 2c20 746f 703d  nches(4.5), top=
-00059740: 746f 702c 2077 6964 7468 3d49 6e63 6865  top, width=Inche
-00059750: 7328 342e 3529 290d 0a09 0909 0970 6963  s(4.5))......pic
-00059760: 203d 2073 6c69 6465 2e73 6861 7065 732e   = slide.shapes.
-00059770: 6164 645f 7069 6374 7572 6528 7374 7228  add_picture(str(
-00059780: 7261 775f 6e61 6d65 735b 315d 2e72 6573  raw_names[1].res
-00059790: 6f6c 7665 2829 292c 206c 6566 743d 6c65  olve()), left=le
-000597a0: 6674 2c20 746f 703d 746f 702c 2077 6964  ft, top=top, wid
-000597b0: 7468 3d49 6e63 6865 7328 342e 3529 290d  th=Inches(4.5)).
-000597c0: 0a09 0909 0970 6963 203d 2073 6c69 6465  .....pic = slide
-000597d0: 2e73 6861 7065 732e 6164 645f 7069 6374  .shapes.add_pict
-000597e0: 7572 6528 7374 7228 7261 775f 6e61 6d65  ure(str(raw_name
-000597f0: 735b 325d 2e72 6573 6f6c 7665 2829 292c  s[2].resolve()),
-00059800: 206c 6566 743d 6c65 6674 2c20 746f 703d   left=left, top=
-00059810: 746f 702b 496e 6368 6573 2833 292c 2077  top+Inches(3), w
-00059820: 6964 7468 3d49 6e63 6865 7328 342e 3529  idth=Inches(4.5)
-00059830: 290d 0a09 0909 0974 7279 3a0d 0a09 0909  )......try:.....
-00059840: 0909 7069 6320 3d20 736c 6964 652e 7368  ..pic = slide.sh
-00059850: 6170 6573 2e61 6464 5f70 6963 7475 7265  apes.add_picture
-00059860: 2873 7472 2872 6177 5f6e 616d 6573 5b33  (str(raw_names[3
-00059870: 5d2e 7265 736f 6c76 6528 2929 2c20 6c65  ].resolve()), le
-00059880: 6674 3d6c 6566 742b 496e 6368 6573 2834  ft=left+Inches(4
-00059890: 2e35 292c 2074 6f70 3d74 6f70 2b49 6e63  .5), top=top+Inc
-000598a0: 6865 7328 3329 2c20 6865 6967 6874 3d49  hes(3), height=I
-000598b0: 6e63 6865 7328 332e 3429 290d 0a09 0909  nches(3.4)).....
-000598c0: 0965 7863 6570 743a 0d0a 0909 0909 0970  .except:.......p
-000598d0: 6173 730d 0a09 0909 6966 2073 6176 655f  ass.....if save_
-000598e0: 4669 743a 0d0a 0909 0909 7472 793a 0d0a  Fit:......try:..
-000598f0: 0909 0909 0973 6c69 6465 3220 3d20 7072  .....slide2 = pr
-00059900: 732e 736c 6964 6573 2e61 6464 5f73 6c69  s.slides.add_sli
-00059910: 6465 2862 6c61 6e6b 5f73 6c69 6465 5f6c  de(blank_slide_l
-00059920: 6179 6f75 7429 0d0a 0909 0909 096c 6566  ayout).......lef
-00059930: 7420 3d20 746f 7020 3d20 496e 6368 6573  t = top = Inches
-00059940: 2830 2e31 290d 0a09 0909 0909 7069 6320  (0.1).......pic 
-00059950: 3d20 736c 6964 6532 2e73 6861 7065 732e  = slide2.shapes.
-00059960: 6164 645f 7069 6374 7572 6528 7374 7228  add_picture(str(
-00059970: 6669 745f 6e61 6d65 735b 305d 2e72 6573  fit_names[0].res
-00059980: 6f6c 7665 2829 292c 206c 6566 743d 6c65  olve()), left=le
-00059990: 6674 2b49 6e63 6865 7328 352e 3529 2c20  ft+Inches(5.5), 
-000599a0: 746f 703d 746f 702c 2068 6569 6768 743d  top=top, height=
-000599b0: 496e 6368 6573 2833 2e35 2929 234d 6174  Inches(3.5))#Mat
-000599c0: 7269 780d 0a09 0909 0909 7069 6320 3d20  rix.......pic = 
-000599d0: 736c 6964 6532 2e73 6861 7065 732e 6164  slide2.shapes.ad
-000599e0: 645f 7069 6374 7572 6528 7374 7228 6669  d_picture(str(fi
-000599f0: 745f 6e61 6d65 735b 315d 2e72 6573 6f6c  t_names[1].resol
-00059a00: 7665 2829 292c 206c 6566 743d 6c65 6674  ve()), left=left
-00059a10: 2c20 746f 703d 746f 702c 2068 6569 6768  , top=top, heigh
-00059a20: 743d 496e 6368 6573 2832 2929 0d0a 0909  t=Inches(2))....
-00059a30: 0909 0970 6963 203d 2073 6c69 6465 322e  ...pic = slide2.
-00059a40: 7368 6170 6573 2e61 6464 5f70 6963 7475  shapes.add_pictu
-00059a50: 7265 2873 7472 2866 6974 5f6e 616d 6573  re(str(fit_names
-00059a60: 5b32 5d2e 7265 736f 6c76 6528 2929 2c20  [2].resolve()), 
-00059a70: 6c65 6674 3d6c 6566 742c 2074 6f70 3d74  left=left, top=t
-00059a80: 6f70 2b49 6e63 6865 7328 3229 2c20 6865  op+Inches(2), he
-00059a90: 6967 6874 3d49 6e63 6865 7328 3229 290d  ight=Inches(2)).
-00059aa0: 0a09 0909 0909 7069 6320 3d20 736c 6964  ......pic = slid
-00059ab0: 6532 2e73 6861 7065 732e 6164 645f 7069  e2.shapes.add_pi
-00059ac0: 6374 7572 6528 7374 7228 6669 745f 6e61  cture(str(fit_na
-00059ad0: 6d65 735b 335d 2e72 6573 6f6c 7665 2829  mes[3].resolve()
-00059ae0: 292c 206c 6566 743d 6c65 6674 2c20 746f  ), left=left, to
-00059af0: 703d 746f 702b 496e 6368 6573 2833 2e39  p=top+Inches(3.9
-00059b00: 292c 2068 6569 6768 743d 496e 6368 6573  ), height=Inches
-00059b10: 2831 2e34 2929 0d0a 0909 0909 0970 6963  (1.4)).......pic
-00059b20: 203d 2073 6c69 6465 322e 7368 6170 6573   = slide2.shapes
-00059b30: 2e61 6464 5f70 6963 7475 7265 2873 7472  .add_picture(str
-00059b40: 2866 6974 5f6e 616d 6573 5b34 5d2e 7265  (fit_names[4].re
-00059b50: 736f 6c76 6528 2929 2c20 6c65 6674 3d6c  solve()), left=l
-00059b60: 6566 742c 2074 6f70 3d74 6f70 2b49 6e63  eft, top=top+Inc
-00059b70: 6865 7328 352e 3429 2c20 6865 6967 6874  hes(5.4), height
-00059b80: 3d49 6e63 6865 7328 3229 290d 0a09 0909  =Inches(2)).....
-00059b90: 0909 0d0a 0909 0909 0974 6578 7431 203d  .........text1 =
-00059ba0: 2073 6c69 6465 322e 7368 6170 6573 2e61   slide2.shapes.a
-00059bb0: 6464 5f74 6578 7462 6f78 286c 6566 743d  dd_textbox(left=
-00059bc0: 6c65 6674 2b49 6e63 6865 7328 352e 3529  left+Inches(5.5)
-00059bd0: 2c20 746f 703d 746f 702b 496e 6368 6573  , top=top+Inches
-00059be0: 2833 2e35 292c 2077 6964 7468 3d49 6e63  (3.5), width=Inc
-00059bf0: 6865 7328 342e 3529 2c20 6865 6967 6874  hes(4.5), height
-00059c00: 3d49 6e63 6865 7328 3429 290d 0a09 0909  =Inches(4)).....
-00059c10: 0909 7465 7874 312e 7465 7874 203d 2052  ..text1.text = R
-00059c20: 6573 756c 745f 7374 7269 6e67 0d0a 0909  esult_string....
-00059c30: 0909 0974 6578 7431 2e74 6578 745f 6672  ...text1.text_fr
-00059c40: 616d 652e 6669 745f 7465 7874 2866 6f6e  ame.fit_text(fon
-00059c50: 745f 6661 6d69 6c79 3d75 2741 7269 616c  t_family=u'Arial
-00059c60: 272c 206d 6178 5f73 697a 653d 382c 2062  ', max_size=8, b
-00059c70: 6f6c 643d 4661 6c73 652c 2069 7461 6c69  old=False, itali
-00059c80: 633d 4661 6c73 6529 0d0a 0909 0909 6578  c=False)......ex
-00059c90: 6365 7074 3a0d 0a09 0909 0909 7072 696e  cept:.......prin
-00059ca0: 7428 2765 7869 7465 6420 7768 656e 2073  t('exited when s
-00059cb0: 6176 696e 6720 7468 6520 6669 7420 706c  aving the fit pl
-00059cc0: 6f74 7327 290d 0a09 0909 090d 0a0d 0a09  ots')...........
-00059cd0: 0909 706c 742e 636c 6f73 6528 2761 6c6c  ..plt.close('all
-00059ce0: 2729 0d0a 0909 0973 656c 662e 7361 7665  ').....self.save
-00059cf0: 5f66 6967 7572 6573 5f74 6f5f 666f 6c64  _figures_to_fold
-00059d00: 6572 3d6f 7269 6769 6e0d 0a09 0909 7072  er=origin.....pr
-00059d10: 732e 7361 7665 2863 6865 636b 5f66 6f6c  s.save(check_fol
-00059d20: 6465 7228 7061 7468 3d70 6174 682c 6375  der(path=path,cu
-00059d30: 7272 656e 745f 7061 7468 3d73 656c 662e  rrent_path=self.
-00059d40: 7061 7468 2c66 696c 656e 616d 653d 7365  path,filename=se
-00059d50: 6c66 2e66 696c 656e 616d 652e 7370 6c69  lf.filename.spli
-00059d60: 7428 272e 2729 5b30 5d20 2b20 272e 7070  t('.')[0] + '.pp
-00059d70: 7478 2729 290d 0a09 0909 7072 696e 7428  tx')).....print(
-00059d80: 2741 6c6c 2064 6174 6120 7761 7320 7361  'All data was sa
-00059d90: 7665 6420 746f 2025 7327 2563 6865 636b  ved to %s'%check
-00059da0: 5f66 6f6c 6465 7228 7061 7468 3d70 6174  _folder(path=pat
-00059db0: 682c 6375 7272 656e 745f 7061 7468 3d73  h,current_path=s
-00059dc0: 656c 662e 7061 7468 2929 0d0a 0909 0d0a  elf.path))......
-00059dd0: 090d 0a0d 0a0d 0a09 6465 6620 5361 7665  ........def Save
-00059de0: 5f70 726f 6a65 6374 2873 656c 662c 2066  _project(self, f
-00059df0: 696c 656e 616d 653d 4e6f 6e65 2c70 6174  ilename=None,pat
-00059e00: 683d 4e6f 6e65 293a 0d0a 0909 2727 2766  h=None):....'''f
-00059e10: 756e 6374 696f 6e20 746f 2064 756d 7020  unction to dump 
-00059e20: 616c 6c20 7468 6520 7061 7261 6d65 7465  all the paramete
-00059e30: 7220 6f66 2061 6e20 616e 616c 7973 6973  r of an analysis
-00059e40: 2069 6e74 6f20 616e 2068 6466 3520 6669   into an hdf5 fi
-00059e50: 6c65 2e20 0d0a 0909 5468 6973 2066 696c  le. ....This fil
-00059e60: 6520 636f 6e74 6169 6e73 2074 6865 2064  e contains the d
-00059e70: 735f 6f72 6920 616e 6420 616c 6c20 7468  s_ori and all th
-00059e80: 6520 7061 7261 6d65 7465 722c 2069 6e63  e parameter, inc
-00059e90: 6c75 6469 6e67 2066 6974 7469 6e67 2070  luding fitting p
-00059ea0: 6172 616d 6574 6572 0d0a 0909 616e 6420  arameter....and 
-00059eb0: 7265 7375 6c74 732e 0d0a 0909 4f6e 6520  results.....One 
-00059ec0: 6c69 6d69 7461 7469 6f6e 2069 7320 7468  limitation is th
-00059ed0: 6520 6669 7474 696e 6720 6d6f 6465 6c2e  e fitting model.
-00059ee0: 2049 6620 7468 6520 6d6f 6465 6c20 6973   If the model is
-00059ef0: 2062 7569 6c64 2069 6e2c 2073 6f20 7468   build in, so th
-00059f00: 6520 6d6f 6465 6c20 6973 0d0a 0909 2765  e model is....'e
-00059f10: 7870 6f6e 656e 7469 616c 2720 6f72 2027  xponential' or '
-00059f20: 7061 7261 6c6c 656c 2720 7468 656e 2074  parallel' then t
-00059f30: 6865 2073 6166 696e 6720 776f 726b 732e  he safing works.
-00059f40: 2049 6620 616e 2065 7874 6572 6e61 6c20   If an external 
-00059f50: 6d6f 6465 6c20 6973 2075 7365 6420 7468  model is used th
-00059f60: 656e 2074 6865 200d 0a09 0964 6f73 7472  en the ....dostr
-00059f70: 696e 6720 6f66 2074 6865 2065 7874 6572  ing of the exter
-00059f80: 6e61 6c20 6675 6e63 7469 6f6e 2069 7320  nal function is 
-00059f90: 7374 6f72 6564 2c20 6275 7420 6e6f 7420  stored, but not 
-00059fa0: 7468 6520 6675 6e63 7469 6f6e 2069 7473  the function its
-00059fb0: 656c 662e 0d0a 0909 0909 0d0a 0909 5061  elf...........Pa
-00059fc0: 7261 6d65 7465 7273 0d0a 0909 2d2d 2d2d  rameters....----
-00059fd0: 2d2d 2d2d 2d2d 0d0a 0909 0d0a 0909 7061  ------........pa
-00059fe0: 7468 203a 204e 6f6e 652c 2073 7472 206f  th : None, str o
-00059ff0: 7220 7061 7468 2c20 6f70 7469 6f6e 616c  r path, optional
-0005a000: 0d0a 0909 0928 4465 6661 756c 7429 204e  .....(Default) N
-0005a010: 6f6e 652c 2069 6620 6c65 6674 206f 6e20  one, if left on 
-0005a020: 4e6f 6e65 2c20 7468 656e 2061 2066 6f6c  None, then a fol
-0005a030: 6465 7220 2244 6174 6122 2069 7320 6372  der "Data" is cr
-0005a040: 6561 7465 6420 696e 2074 6865 2066 6f6c  eated in the fol
-0005a050: 6465 7220 0d0a 0909 096f 6620 7468 6520  der .....of the 
-0005a060: 7072 6f6a 6563 7420 2873 656c 662e 7061  project (self.pa
-0005a070: 7468 290d 0a09 0909 090d 0a09 0966 696c  th)..........fil
-0005a080: 656e 616d 6520 3a20 7374 722c 206f 7074  ename : str, opt
-0005a090: 696f 6e61 6c0d 0a09 0909 2844 6566 6175  ional.....(Defau
-0005a0a0: 6c74 2920 4e6f 6e65 2c20 4261 7365 206e  lt) None, Base n
-0005a0b0: 616d 6520 666f 7220 616c 6c20 706c 6f74  ame for all plot
-0005a0c0: 732e 2049 6620 4e6f 6e65 2c20 7468 656e  s. If None, then
-0005a0d0: 2073 656c 662e 6669 6c65 6e61 6d65 2077   self.filename w
-0005a0e0: 696c 6c20 6265 2075 7365 640d 0a09 0909  ill be used.....
-0005a0f0: 0d0a 0909 4578 616d 706c 6573 0d0a 0909  ....Examples....
-0005a100: 2d2d 2d2d 2d2d 2d2d 0d0a 0909 0d0a 0909  --------........
-0005a110: 3e3e 3e20 7461 2e53 6176 655f 7072 6f6a  >>> ta.Save_proj
-0005a120: 6563 7428 290d 0a09 090d 0a09 0927 2727  ect()........'''
-0005a130: 0d0a 0909 0d0a 0909 6966 2066 696c 656e  ........if filen
-0005a140: 616d 6520 6973 204e 6f6e 653a 0d0a 0909  ame is None:....
-0005a150: 0966 696c 656e 616d 6520 3d20 7365 6c66  .filename = self
-0005a160: 2e66 696c 656e 616d 650d 0a09 0968 6466  .filename....hdf
-0005a170: 355f 6e61 6d65 203d 6368 6563 6b5f 666f  5_name =check_fo
-0005a180: 6c64 6572 2870 6174 6820 3d20 7061 7468  lder(path = path
-0005a190: 2c20 6375 7272 656e 745f 7061 7468 203d  , current_path =
-0005a1a0: 2073 656c 662e 7061 7468 2c20 6669 6c65   self.path, file
-0005a1b0: 6e61 6d65 203d 2066 696c 656e 616d 652e  name = filename.
-0005a1c0: 7370 6c69 7428 272e 2729 5b30 5d2b 272e  split('.')[0]+'.
-0005a1d0: 6864 6635 2729 0d0a 0909 6966 206f 732e  hdf5')....if os.
-0005a1e0: 7061 7468 2e65 7869 7374 7328 6864 6635  path.exists(hdf5
-0005a1f0: 5f6e 616d 6529 3a0d 0a09 0909 7472 793a  _name):.....try:
-0005a200: 0d0a 0909 0909 6f73 2e72 656d 6f76 6528  ......os.remove(
-0005a210: 6864 6635 5f6e 616d 6529 0d0a 0909 0965  hdf5_name).....e
-0005a220: 7863 6570 743a 0d0a 0909 0909 7472 793a  xcept:......try:
-0005a230: 0d0a 0909 0909 0968 6466 355f 6e61 6d65  .......hdf5_name
-0005a240: 2e63 6c6f 7365 2829 0d0a 0909 0909 096f  .close().......o
-0005a250: 732e 7265 6d6f 7665 2868 6466 355f 6e61  s.remove(hdf5_na
-0005a260: 6d65 290d 0a09 0909 0965 7863 6570 743a  me)......except:
-0005a270: 0d0a 0909 0909 0970 7269 6e74 2827 4669  .......print('Fi
-0005a280: 6c65 2065 7869 7374 7320 6275 7420 6361  le exists but ca
-0005a290: 6e20 6e6f 7420 6265 2064 656c 6574 6564  n not be deleted
-0005a2a0: 2729 0d0a 0909 7265 5f73 7769 7463 6820  ')....re_switch 
-0005a2b0: 3d20 4661 6c73 650d 0a09 0977 6974 6820  = False....with 
-0005a2c0: 6835 7079 2e46 696c 6528 6864 6635 5f6e  h5py.File(hdf5_n
-0005a2d0: 616d 652c 2027 7727 2920 6173 2066 3a0d  ame, 'w') as f:.
-0005a2e0: 0a09 0909 666f 7220 6b65 7920 696e 2073  ....for key in s
-0005a2f0: 656c 662e 5f5f 6469 6374 5f5f 2e6b 6579  elf.__dict__.key
-0005a300: 7328 293a 0d0a 0909 0909 6966 206b 6579  s():......if key
-0005a310: 203d 3d20 276d 6f64 273a 0d0a 0909 0909   == 'mod':......
-0005a320: 0969 6620 7365 6c66 2e5f 5f64 6963 745f  .if self.__dict_
-0005a330: 5f5b 6b65 795d 2069 6e20 5b27 7061 7261  _[key] in ['para
-0005a340: 6c27 2c27 6578 706f 6e65 6e74 6961 6c27  l','exponential'
-0005a350: 2c27 636f 6e73 6563 7574 6976 6527 2c27  ,'consecutive','
-0005a360: 6675 6c6c 5f63 6f6e 7365 6375 7469 7665  full_consecutive
-0005a370: 275d 3a0d 0a09 0909 0909 0966 2e63 7265  ']:........f.cre
-0005a380: 6174 655f 6461 7461 7365 7428 6e61 6d65  ate_dataset(name
-0005a390: 3d6b 6579 2c20 6461 7461 3d73 656c 662e  =key, data=self.
-0005a3a0: 5f5f 6469 6374 5f5f 5b6b 6579 5d29 0d0a  __dict__[key])..
-0005a3b0: 0909 0909 0965 6c73 653a 0d0a 0909 0909  .....else:......
-0005a3c0: 0909 7472 793a 0d0a 0909 0909 0909 0964  ..try:.........d
-0005a3d0: 6f63 7374 7269 6e67 3d73 656c 662e 5f5f  ocstring=self.__
-0005a3e0: 6469 6374 5f5f 5b6b 6579 5d2e 5f5f 646f  dict__[key].__do
-0005a3f0: 635f 5f0d 0a09 0909 0909 0909 6966 2069  c__.........if i
-0005a400: 7369 6e73 7461 6e63 6528 646f 6373 7472  sinstance(docstr
-0005a410: 696e 672c 7479 7065 2827 6865 6c6c 6f27  ing,type('hello'
-0005a420: 2929 3a0d 0a09 0909 0909 0909 0966 2e63  )):..........f.c
-0005a430: 7265 6174 655f 6461 7461 7365 7428 6e61  reate_dataset(na
-0005a440: 6d65 3d6b 6579 2c20 6461 7461 3d64 6f63  me=key, data=doc
-0005a450: 7374 7269 6e67 290d 0a09 0909 0909 0965  string)........e
-0005a460: 7863 6570 743a 0d0a 0909 0909 0909 0966  xcept:.........f
-0005a470: 2e63 7265 6174 655f 6461 7461 7365 7428  .create_dataset(
-0005a480: 6e61 6d65 3d6b 6579 2c20 6461 7461 3d27  name=key, data='
-0005a490: 6578 7465 726e 616c 5f66 756e 6374 696f  external_functio
-0005a4a0: 6e5f 7769 7468 6f75 745f 646f 6373 7472  n_without_docstr
-0005a4b0: 696e 6727 290d 0a09 0909 0965 6c69 6620  ing')......elif 
-0005a4c0: 6b65 7920 696e 205b 2772 656c 5f77 6176  key in ['rel_wav
-0005a4d0: 6527 2c27 7265 6c5f 7469 6d65 275d 3a23  e','rel_time']:#
-0005a4e0: 6e65 6564 2065 7874 7261 2c20 6173 2069  need extra, as i
-0005a4f0: 7420 6973 2062 7970 6173 7365 6420 6279  t is bypassed by
-0005a500: 2074 6865 2072 652d 7377 6974 6368 0d0a   the re-switch..
-0005a510: 0909 0909 0966 2e63 7265 6174 655f 6461  .....f.create_da
-0005a520: 7461 7365 7428 6e61 6d65 3d6b 6579 2c20  taset(name=key, 
-0005a530: 6461 7461 3d73 656c 662e 5f5f 6469 6374  data=self.__dict
-0005a540: 5f5f 5b6b 6579 5d29 0d0a 0909 0909 656c  __[key])......el
-0005a550: 6966 206b 6579 5b3a 325d 203d 3d20 2772  if key[:2] == 'r
-0005a560: 6527 203a 0d0a 0909 0909 0972 655f 7377  e' :.......re_sw
-0005a570: 6974 6368 203d 2054 7275 650d 0a09 0909  itch = True.....
-0005a580: 0909 666f 7220 6b65 7932 2069 6e20 7365  ..for key2 in se
-0005a590: 6c66 2e5f 5f64 6963 745f 5f5b 2772 6527  lf.__dict__['re'
-0005a5a0: 5d3a 0d0a 0909 0909 0909 6966 206b 6579  ]:........if key
-0005a5b0: 3220 3d3d 2027 6669 745f 6f75 7470 7574  2 == 'fit_output
-0005a5c0: 273a 636f 6e74 696e 7565 0d0a 0909 0909  ':continue......
-0005a5d0: 0909 6461 7461 203d 2073 656c 662e 5f5f  ..data = self.__
-0005a5e0: 6469 6374 5f5f 5b27 7265 275d 5b6b 6579  dict__['re'][key
-0005a5f0: 325d 0d0a 0909 0909 0909 6966 206b 6579  2]........if key
-0005a600: 3220 3d3d 2027 6572 726f 7227 3a0d 0a09  2 == 'error':...
-0005a610: 0909 0909 0909 7472 793a 0d0a 0909 0909  ......try:......
-0005a620: 0909 0909 662e 6372 6561 7465 5f64 6174  ....f.create_dat
-0005a630: 6173 6574 286e 616d 653d 2772 655f 6572  aset(name='re_er
-0005a640: 726f 7227 2c20 6461 7461 3d64 6174 6129  ror', data=data)
-0005a650: 0d0a 0909 0909 0909 0965 7863 6570 743a  .........except:
-0005a660: 0d0a 0909 0909 0909 0909 7072 696e 7428  ..........print(
-0005a670: 2773 6176 696e 6720 6f66 2027 202b 206b  'saving of ' + k
-0005a680: 6579 3220 2b20 2720 6661 696c 6564 2720  ey2 + ' failed' 
-0005a690: 290d 0a09 0909 0909 0965 6c69 6620 6973  )........elif is
-0005a6a0: 696e 7374 616e 6365 2864 6174 612c 2070  instance(data, p
-0005a6b0: 616e 6461 732e 4461 7461 4672 616d 6529  andas.DataFrame)
-0005a6c0: 3a0d 0a09 0909 0909 0909 7061 7373 0d0a  :.........pass..
-0005a6d0: 0909 0909 0909 656c 7365 3a0d 0a09 0909  ......else:.....
-0005a6e0: 0909 0909 7472 793a 0d0a 0909 0909 0909  ....try:........
-0005a6f0: 0909 662e 6372 6561 7465 5f64 6174 6173  ..f.create_datas
-0005a700: 6574 286e 616d 653d 2772 655f 2720 2b20  et(name='re_' + 
-0005a710: 6b65 7932 2c20 6461 7461 3d64 6174 6129  key2, data=data)
-0005a720: 0d0a 0909 0909 0909 0965 7863 6570 743a  .........except:
-0005a730: 0d0a 0909 0909 0909 0909 7072 696e 7428  ..........print(
-0005a740: 2773 6176 696e 6720 6f66 2027 202b 206b  'saving of ' + k
-0005a750: 6579 3220 2b20 2720 6661 696c 6564 2720  ey2 + ' failed' 
-0005a760: 290d 0a09 0909 0965 6c69 6620 6b65 7920  )......elif key 
-0005a770: 3d3d 2027 636d 6170 273a 0d0a 0909 0909  == 'cmap':......
-0005a780: 0970 6173 730d 0a09 0909 0965 6c69 6620  .pass......elif 
-0005a790: 6b65 7920 3d3d 2027 696e 7465 6e73 6974  key == 'intensit
-0005a7a0: 795f 7261 6e67 6527 3a0d 0a09 0909 0909  y_range':.......
-0005a7b0: 6461 7461 3d73 656c 662e 5f5f 6469 6374  data=self.__dict
-0005a7c0: 5f5f 5b27 696e 7465 6e73 6974 795f 7261  __['intensity_ra
-0005a7d0: 6e67 6527 5d0d 0a09 0909 0909 6966 2069  nge'].......if i
-0005a7e0: 7369 6e73 7461 6e63 6528 6461 7461 2c20  sinstance(data, 
-0005a7f0: 7479 7065 2831 652d 3329 293a 0d0a 0909  type(1e-3)):....
-0005a800: 0909 0909 6461 7461 3d5b 2d64 6174 612c  ....data=[-data,
-0005a810: 6461 7461 5d0d 0a09 0909 0909 6966 2064  data].......if d
-0005a820: 6174 6120 6973 204e 6f6e 653a 0d0a 0909  ata is None:....
-0005a830: 0909 0909 662e 6372 6561 7465 5f64 6174  ....f.create_dat
-0005a840: 6173 6574 286e 616d 653d 2769 6e74 656e  aset(name='inten
-0005a850: 7369 7479 5f72 616e 6765 272c 2064 6174  sity_range', dat
-0005a860: 613d 274e 6f6e 6527 290d 0a09 0909 0909  a='None').......
-0005a870: 656c 7365 3a0d 0a09 0909 0909 0966 2e63  else:........f.c
-0005a880: 7265 6174 655f 6461 7461 7365 7428 6e61  reate_dataset(na
-0005a890: 6d65 3d27 696e 7465 6e73 6974 795f 7261  me='intensity_ra
-0005a8a0: 6e67 6527 2c20 6461 7461 3d64 6174 6129  nge', data=data)
-0005a8b0: 090d 0a09 0909 0965 6c69 6620 6b65 7920  .......elif key 
-0005a8c0: 3d3d 2027 6261 636b 6772 6f75 6e64 5f70  == 'background_p
-0005a8d0: 6172 273a 0d0a 0909 0909 0966 2e63 7265  ar':.......f.cre
-0005a8e0: 6174 655f 6461 7461 7365 7428 6e61 6d65  ate_dataset(name
-0005a8f0: 3d27 6261 636b 272c 2064 6174 613d 7365  ='back', data=se
-0005a900: 6c66 2e5f 5f64 6963 745f 5f5b 2762 6163  lf.__dict__['bac
-0005a910: 6b67 726f 756e 645f 7061 7227 5d5b 335d  kground_par'][3]
-0005a920: 290d 0a09 0909 090d 0a09 0909 0965 6c69  )............eli
-0005a930: 6620 6b65 7920 696e 205b 2770 6172 272c  f key in ['par',
-0005a940: 2770 6172 5f66 6974 275d 3a0d 0a09 0909  'par_fit']:.....
-0005a950: 0909 0909 0909 200d 0a09 0909 0909 6466  ...... .......df
-0005a960: 3d70 6172 5f74 6f5f 7061 7264 6628 7365  =par_to_pardf(se
-0005a970: 6c66 2e5f 5f64 6963 745f 5f5b 6b65 795d  lf.__dict__[key]
-0005a980: 2923 7061 6e64 6173 2068 6173 2061 2062  )#pandas has a b
-0005a990: 7567 2061 6e64 2070 726f 626c 656d 7320  ug and problems 
-0005a9a0: 6861 6e64 6c69 6e67 206d 6978 6564 2074  handling mixed t
-0005a9b0: 7970 6520 636f 6c75 6d6e 7320 7768 656e  ype columns when
-0005a9c0: 2073 6176 696e 672e 2053 6f20 7765 2063   saving. So we c
-0005a9d0: 6c65 616e 2075 702e 0d0a 0909 0909 0966  lean up........f
-0005a9e0: 6f72 2073 7562 5f6b 6579 2069 6e20 5b27  or sub_key in ['
-0005a9f0: 6d69 6e27 2c27 6d61 7827 2c27 7661 6c75  min','max','valu
-0005aa00: 6527 5d3a 0d0a 0909 0909 0909 7472 793a  e']:........try:
-0005aa10: 0d0a 0909 0909 0909 0964 665b 7375 625f  .........df[sub_
-0005aa20: 6b65 795d 3d64 665b 7375 625f 6b65 795d  key]=df[sub_key]
-0005aa30: 2e61 7374 7970 6528 666c 6f61 7429 0d0a  .astype(float)..
-0005aa40: 0909 0909 0909 6578 6365 7074 3a0d 0a09  ......except:...
-0005aa50: 0909 0909 0909 7061 7373 0d0a 0909 0909  ......pass......
-0005aa60: 0964 665b 2769 735f 7261 7465 275d 3d64  .df['is_rate']=d
-0005aa70: 665b 2769 735f 7261 7465 275d 2e61 7374  f['is_rate'].ast
-0005aa80: 7970 6528 626f 6f6c 290d 0a09 0909 0909  ype(bool).......
-0005aa90: 6466 5b27 7661 7279 275d 3d64 665b 2776  df['vary']=df['v
-0005aaa0: 6172 7927 5d2e 6173 7479 7065 2862 6f6f  ary'].astype(boo
-0005aab0: 6c29 0d0a 0909 0909 0964 665b 2765 7870  l).......df['exp
-0005aac0: 7227 5d3d 6466 5b27 6578 7072 275d 2e61  r']=df['expr'].a
-0005aad0: 7070 6c79 286c 616d 6264 6120 783a 2725  pply(lambda x:'%
-0005aae0: 7327 2578 290d 0a09 0909 0909 6466 2e74  s'%x).......df.t
-0005aaf0: 6f5f 6864 6628 7374 7228 6864 6635 5f6e  o_hdf(str(hdf5_n
-0005ab00: 616d 652e 7265 736f 6c76 6528 2929 2c20  ame.resolve()), 
-0005ab10: 6b65 793d 6b65 792c 2061 7070 656e 643d  key=key, append=
-0005ab20: 5472 7565 2c20 6d6f 6465 3d27 722b 272c  True, mode='r+',
-0005ab30: 2066 6f72 6d61 743d 2774 2729 0d0a 0909   format='t')....
-0005ab40: 0909 656c 7365 3a0d 0a09 0909 0909 6461  ..else:.......da
-0005ab50: 7461 203d 2073 656c 662e 5f5f 6469 6374  ta = self.__dict
-0005ab60: 5f5f 5b6b 6579 5d0d 0a09 0909 0909 6966  __[key].......if
-0005ab70: 2064 6174 6120 6973 204e 6f6e 653a 0d0a   data is None:..
-0005ab80: 0909 0909 0909 662e 6372 6561 7465 5f64  ......f.create_d
-0005ab90: 6174 6173 6574 286e 616d 653d 6b65 792c  ataset(name=key,
-0005aba0: 2064 6174 613d 274e 6f6e 6527 290d 0a09   data='None')...
-0005abb0: 0909 0909 656c 7365 3a0d 0a09 0909 0909  ....else:.......
-0005abc0: 0969 6620 6973 696e 7374 616e 6365 2864  .if isinstance(d
-0005abd0: 6174 612c 2070 616e 6461 732e 4461 7461  ata, pandas.Data
-0005abe0: 4672 616d 6529 3a0d 0a09 0909 0909 0909  Frame):.........
-0005abf0: 7061 7373 0d0a 0909 0909 0909 656c 7365  pass........else
-0005ac00: 3a0d 0a09 0909 0909 0909 7472 793a 0d0a  :.........try:..
-0005ac10: 0909 0909 0909 0909 662e 6372 6561 7465  ........f.create
-0005ac20: 5f64 6174 6173 6574 286e 616d 653d 6b65  _dataset(name=ke
-0005ac30: 792c 2064 6174 613d 6461 7461 290d 0a09  y, data=data)...
-0005ac40: 0909 0909 0909 6578 6365 7074 3a0d 0a09  ......except:...
-0005ac50: 0909 0909 0909 0969 6620 6b65 7920 3d3d  .......if key ==
-0005ac60: 2027 7061 7468 273a 0d0a 0909 0909 0909   'path':........
-0005ac70: 0909 0970 6173 730d 0a09 0909 0909 0909  ...pass.........
-0005ac80: 0965 6c69 6620 6b65 7920 3d3d 2027 6669  .elif key == 'fi
-0005ac90: 6775 7265 5f70 6174 6827 3a0d 0a09 0909  gure_path':.....
-0005aca0: 0909 0909 0909 7061 7373 0d0a 0909 0909  ......pass......
-0005acb0: 0909 0909 656c 7365 3a0d 0a09 0909 0909  ....else:.......
-0005acc0: 0909 0909 7072 696e 7428 2774 6865 2073  ....print('the s
-0005acd0: 6176 696e 6720 6f66 2020 2573 2020 6661  aving of  %s  fa
-0005ace0: 696c 6564 2725 6b65 7929 0d0a 0909 0969  iled'%key).....i
-0005acf0: 6620 6e6f 7420 2766 6974 636f 6566 6627  f not 'fitcoeff'
-0005ad00: 2069 6e20 663a 0d0a 0909 0909 7472 793a   in f:......try:
-0005ad10: 0d0a 0909 0909 0966 2e63 7265 6174 655f  .......f.create_
-0005ad20: 6461 7461 7365 7428 6e61 6d65 3d27 6669  dataset(name='fi
-0005ad30: 7463 6f65 6666 272c 2064 6174 613d 7365  tcoeff', data=se
-0005ad40: 6c66 2e66 6974 636f 6566 6629 0d0a 0909  lf.fitcoeff)....
-0005ad50: 0909 6578 6365 7074 3a0d 0a09 0909 0909  ..except:.......
-0005ad60: 7472 793a 0d0a 0909 0909 0909 7769 7468  try:........with
-0005ad70: 206f 7065 6e28 7365 6c66 2e63 6869 7270   open(self.chirp
-0005ad80: 5f66 696c 652c 2772 2729 2061 7320 6632  _file,'r') as f2
-0005ad90: 3a0d 0a09 0909 0909 0909 6669 7463 6f65  :.........fitcoe
-0005ada0: 6666 3d66 322e 7265 6164 6c69 6e65 2829  ff=f2.readline()
-0005adb0: 0d0a 0909 0909 0909 0966 2e63 7265 6174  .........f.creat
-0005adc0: 655f 6461 7461 7365 7428 6e61 6d65 3d27  e_dataset(name='
-0005add0: 6669 7463 6f65 6666 272c 2064 6174 613d  fitcoeff', data=
-0005ade0: 6669 7463 6f65 6666 290d 0a09 0909 0909  fitcoeff).......
-0005adf0: 6578 6365 7074 3a0d 0a09 0909 0909 0970  except:........p
-0005ae00: 6173 730d 0a09 0973 656c 662e 6473 5f6f  ass....self.ds_o
-0005ae10: 7269 2e74 6f5f 6864 6628 7374 7228 6864  ri.to_hdf(str(hd
-0005ae20: 6635 5f6e 616d 652e 7265 736f 6c76 6528  f5_name.resolve(
-0005ae30: 2929 2c20 6b65 793d 2764 735f 6f72 6927  )), key='ds_ori'
-0005ae40: 2c20 6170 7065 6e64 3d54 7275 652c 206d  , append=True, m
-0005ae50: 6f64 653d 2772 2b27 2c20 666f 726d 6174  ode='r+', format
-0005ae60: 3d27 7427 2923 7361 7665 5f72 6177 5f64  ='t')#save_raw_d
-0005ae70: 6174 610d 0a09 0969 6620 7265 5f73 7769  ata....if re_swi
-0005ae80: 7463 683a 0d0a 0909 0923 7072 696e 7428  tch:.....#print(
-0005ae90: 2772 652d 7377 6974 6368 6564 2729 0d0a  're-switched')..
-0005aea0: 0909 0966 6f72 206b 6579 2069 6e20 5b27  ...for key in ['
-0005aeb0: 4127 2c20 2741 4327 2c20 2741 4527 2c20  A', 'AC', 'AE', 
-0005aec0: 2744 4143 272c 2027 6327 5d3a 0d0a 0909  'DAC', 'c']:....
-0005aed0: 0909 7365 6c66 2e72 655b 6b65 795d 2e74  ..self.re[key].t
-0005aee0: 6f5f 6864 6628 7374 7228 6864 6635 5f6e  o_hdf(str(hdf5_n
-0005aef0: 616d 652e 7265 736f 6c76 6528 2929 2c20  ame.resolve()), 
-0005af00: 6b65 793d 2772 655f 2720 2b20 6b65 792c  key='re_' + key,
-0005af10: 2061 7070 656e 643d 5472 7565 2c20 6d6f   append=True, mo
-0005af20: 6465 3d27 722b 272c 2066 6f72 6d61 743d  de='r+', format=
-0005af30: 2774 2729 0d0a 0909 7472 793a 0d0a 0909  't')....try:....
-0005af40: 0966 2e63 6c6f 7365 2829 0d0a 0909 6578  .f.close()....ex
-0005af50: 6365 7074 3a0d 0a09 0909 7061 7373 0d0a  cept:.....pass..
-0005af60: 0909 0d0a 0909 7072 696e 7428 2754 6865  ......print('The
-0005af70: 2070 726f 6a65 6374 2077 6173 2073 6176   project was sav
-0005af80: 6564 2074 6f20 2573 2725 6368 6563 6b5f  ed to %s'%check_
-0005af90: 666f 6c64 6572 2870 6174 6820 3d20 7061  folder(path = pa
-0005afa0: 7468 2c20 6375 7272 656e 745f 7061 7468  th, current_path
-0005afb0: 203d 2073 656c 662e 7061 7468 2929 0d0a   = self.path))..
-0005afc0: 0d0a 0d0a 0964 6566 205f 5f72 6561 645f  .....def __read_
-0005afd0: 7072 6f6a 6563 7428 7365 6c66 2c20 7361  project(self, sa
-0005afe0: 7665 645f 7072 6f6a 6563 743d 4e6f 6e65  ved_project=None
-0005aff0: 2c63 7572 7265 6e74 5f70 6174 683d 4e6f  ,current_path=No
-0005b000: 6e65 293a 0d0a 0909 2727 2766 756e 6374  ne):....'''funct
-0005b010: 696f 6e20 746f 2072 652d 7265 6164 2061  ion to re-read a
-0005b020: 6c6c 2074 6865 2070 6172 616d 6574 6572  ll the parameter
-0005b030: 206f 6620 6120 7072 6576 696f 7573 2061   of a previous a
-0005b040: 6e61 6c79 7369 7320 0d0a 0909 696e 746f  nalysis ....into
-0005b050: 2061 6e20 6864 6635 2066 696c 652c 2063   an hdf5 file, c
-0005b060: 7572 7265 6e74 2070 6174 6820 6973 2074  urrent path is t
-0005b070: 6865 2070 6174 6820 7468 6174 2074 6865  he path that the
-0005b080: 2066 696c 6520 7368 6f75 6c64 200d 0a09   file should ...
-0005b090: 0961 7373 756d 6520 6973 2069 7473 2022  .assume is its "
-0005b0a0: 686f 6d65 2064 6972 6563 746f 7279 2220  home directory" 
-0005b0b0: 6166 7465 7220 7375 6363 6573 7366 756c  after successful
-0005b0c0: 206c 6f61 6469 6e67 2e20 4966 206e 6f74   loading. If not
-0005b0d0: 200d 0a09 0973 6574 2077 6520 7461 6b65   ....set we take
-0005b0e0: 2074 6865 2066 696c 6570 6174 6820 6174   the filepath at
-0005b0f0: 2077 6869 6368 2074 6865 2066 696c 6520   which the file 
-0005b100: 6973 2063 7572 7265 6e74 6c79 2073 746f  is currently sto
-0005b110: 7265 6420 6173 2070 6174 6827 2727 0d0a  red as path'''..
-0005b120: 0909 6966 2073 6176 6564 5f70 726f 6a65  ..if saved_proje
-0005b130: 6374 2069 7320 4e6f 6e65 3a0d 0a09 0909  ct is None:.....
-0005b140: 7261 6973 6520 496d 706f 7274 4572 726f  raise ImportErro
-0005b150: 7228 2757 6520 646f 206e 6565 6420 6120  r('We do need a 
-0005b160: 7072 6f6a 6563 7420 746f 2069 6d70 6f72  project to impor
-0005b170: 7427 290d 0a09 0969 6620 6375 7272 656e  t')....if curren
-0005b180: 745f 7061 7468 2069 7320 4e6f 6e65 3a63  t_path is None:c
-0005b190: 7572 7265 6e74 5f70 6174 683d 6f73 2e70  urrent_path=os.p
-0005b1a0: 6174 682e 6469 726e 616d 6528 6f73 2e70  ath.dirname(os.p
-0005b1b0: 6174 682e 6162 7370 6174 6828 7361 7665  ath.abspath(save
-0005b1c0: 645f 7072 6f6a 6563 7429 290d 0a09 0974  d_project))....t
-0005b1d0: 7279 3a0d 0a09 0909 696d 706f 7274 2068  ry:.....import h
-0005b1e0: 3570 790d 0a09 0965 7863 6570 743a 0d0a  5py....except:..
-0005b1f0: 0909 200d 0a09 0909 7072 696e 7428 2763  .. .....print('c
-0005b200: 6f75 6c64 206e 6f74 2069 6d70 6f72 7420  ould not import 
-0005b210: 6864 6635 2c20 6375 7272 656e 7420 7665  hdf5, current ve
-0005b220: 7273 696f 6e20 7265 7175 6972 6573 2074  rsion requires t
-0005b230: 6861 7420 7468 6973 2069 7320 696e 7374  hat this is inst
-0005b240: 616c 6c65 642e 2049 4620 7275 6e6e 696e  alled. IF runnin
-0005b250: 6720 416e 6163 6f6e 6461 206f 7065 6e20  g Anaconda open 
-0005b260: 436f 6e64 6120 7072 6f6d 7420 616e 6420  Conda promt and 
-0005b270: 7479 7065 3a20 636f 6e64 6120 696e 7374  type: conda inst
-0005b280: 616c 6c20 6835 7079 2729 0d0a 0909 6461  all h5py')....da
-0005b290: 7461 5f66 7261 6d65 5f6c 6973 743d 5b5d  ta_frame_list=[]
-0005b2a0: 0d0a 0d0a 0909 2320 7765 2068 6176 2074  ......# we hav t
-0005b2b0: 6f20 6861 6e64 6c65 2074 6865 206f 6c64  o handle the old
-0005b2c0: 2061 6e64 206e 6577 2074 7970 6520 6f66   and new type of
-0005b2d0: 2073 6176 696e 670d 0a09 0977 6974 6820   saving....with 
-0005b2e0: 6835 7079 2e46 696c 6528 7361 7665 645f  h5py.File(saved_
-0005b2f0: 7072 6f6a 6563 742c 2027 7227 2920 6173  project, 'r') as
-0005b300: 2066 3a0d 0a09 0909 6966 2027 7265 5f66   f:.....if 're_f
-0005b310: 696e 616c 5f73 6574 7570 5f70 6172 2720  inal_setup_par' 
-0005b320: 696e 2066 2e6b 6579 7328 293a 6f6c 645f  in f.keys():old_
-0005b330: 7377 6974 6368 3d54 7275 650d 0a09 0909  switch=True.....
-0005b340: 0909 200d 0a09 090d 0a09 0909 656c 7365  .. .........else
-0005b350: 3a6f 6c64 5f73 7769 7463 683d 4661 6c73  :old_switch=Fals
-0005b360: 650d 0a09 0909 0909 2020 200d 0a09 0969  e.......   ....i
-0005b370: 6620 6f6c 645f 7377 6974 6368 3a70 7269  f old_switch:pri
-0005b380: 6e74 2827 7765 2072 6561 6420 616e 206f  nt('we read an o
-0005b390: 6c64 2073 7479 6c65 2064 6174 615f 6669  ld style data_fi
-0005b3a0: 6c65 2061 6e64 2064 6972 6563 746c 7920  le and directly 
-0005b3b0: 7570 6461 7465 2069 7420 696e 746f 2074  update it into t
-0005b3c0: 6865 206e 6577 2066 696c 655f 7479 7065  he new file_type
-0005b3d0: 2061 6674 6572 206c 6f61 6469 6e67 2729   after loading')
-0005b3e0: 0d0a 0909 7769 7468 2068 3570 792e 4669  ....with h5py.Fi
-0005b3f0: 6c65 2873 6176 6564 5f70 726f 6a65 6374  le(saved_project
-0005b400: 2c20 2772 2729 2061 7320 663a 0d0a 0909  , 'r') as f:....
-0005b410: 0966 6f72 206b 6579 2069 6e20 662e 6b65  .for key in f.ke
-0005b420: 7973 2829 3a0d 0a09 0909 0974 7279 3a0d  ys():......try:.
-0005b430: 0a09 0909 0909 6966 2022 7265 5f22 2069  ......if "re_" i
-0005b440: 6e20 6b65 795b 3a33 5d3a 0d0a 0909 0909  n key[:3]:......
-0005b450: 0909 6966 206e 6f74 2027 7265 2720 696e  ..if not 're' in
-0005b460: 2073 656c 662e 5f5f 6469 6374 5f5f 2e6b   self.__dict__.k
-0005b470: 6579 7328 293a 0d0a 0909 0909 0909 0973  eys():.........s
-0005b480: 656c 662e 5f5f 6469 6374 5f5f 5b27 7265  elf.__dict__['re
-0005b490: 275d 3d7b 7d0d 0a09 0909 0909 0973 656c  ']={}........sel
-0005b4a0: 662e 5f5f 6469 6374 5f5f 5b27 7265 275d  f.__dict__['re']
-0005b4b0: 5b6b 6579 5b33 3a5d 5d3d 665b 6b65 795d  [key[3:]]=f[key]
-0005b4c0: 5b28 295d 0d0a 0909 0909 0965 6c69 6620  [()].......elif 
-0005b4d0: 2262 6163 6b22 2069 6e20 6b65 795b 3a34  "back" in key[:4
-0005b4e0: 5d3a 0d0a 0909 0909 0909 7265 613d 665b  ]:........rea=f[
-0005b4f0: 6b65 795d 5b28 295d 0d0a 0909 0909 0909  key][()]........
-0005b500: 7365 6c66 2e5f 5f64 6963 745f 5f5b 2762  self.__dict__['b
-0005b510: 6163 6b67 726f 756e 645f 7061 7227 5d3d  ackground_par']=
-0005b520: 5b4e 6f6e 652c 2d31 2c46 616c 7365 5d0d  [None,-1,False].
-0005b530: 0a09 0909 0909 0973 656c 662e 5f5f 6469  .......self.__di
-0005b540: 6374 5f5f 5b27 6261 636b 6772 6f75 6e64  ct__['background
-0005b550: 5f70 6172 275d 2e61 7070 656e 6428 7265  _par'].append(re
-0005b560: 6129 0d0a 0909 0909 0965 6c69 6620 2270  a).......elif "p
-0005b570: 6172 2220 696e 206b 6579 5b3a 335d 3a0d  ar" in key[:3]:.
-0005b580: 0a09 0909 0909 0969 6620 6f6c 645f 7377  .......if old_sw
-0005b590: 6974 6368 3a23 6f6c 6420 7479 7065 206f  itch:#old type o
-0005b5a0: 6620 7361 7665 6420 6461 7461 0d0a 0909  f saved data....
-0005b5b0: 0909 0909 0974 7279 3a0d 0a09 0909 0909  .....try:.......
-0005b5c0: 0909 096f 732e 7265 6d6f 7665 2827 7465  ...os.remove('te
-0005b5d0: 6d70 5f66 696c 652e 6a73 6f6e 2729 0d0a  mp_file.json')..
-0005b5e0: 0909 0909 0909 0965 7863 6570 743a 0d0a  .......except:..
-0005b5f0: 0909 0909 0909 0909 7061 7373 0d0a 0909  ........pass....
-0005b600: 0909 0909 0977 6974 6820 6f70 656e 2827  .....with open('
-0005b610: 7465 6d70 5f66 696c 652e 6a73 6f6e 272c  temp_file.json',
-0005b620: 2777 2729 2061 7320 673a 0d0a 0909 0909  'w') as g:......
-0005b630: 0909 0909 672e 7772 6974 6528 665b 6b65  ....g.write(f[ke
-0005b640: 795d 5b28 295d 290d 0a09 0909 0909 0909  y][()]).........
-0005b650: 7769 7468 206f 7065 6e28 2774 656d 705f  with open('temp_
-0005b660: 6669 6c65 2e6a 736f 6e27 2c27 7227 2920  file.json','r') 
-0005b670: 6173 2067 3a0d 0a09 0909 0909 0909 0973  as g:..........s
-0005b680: 656c 662e 7061 723d 6c6d 6669 742e 5061  elf.par=lmfit.Pa
-0005b690: 7261 6d65 7465 7273 2829 0d0a 0909 0909  rameters()......
-0005b6a0: 0909 0909 7365 6c66 2e70 6172 2e6c 6f61  ....self.par.loa
-0005b6b0: 6428 6729 0d0a 0909 0909 0909 0974 7279  d(g).........try
-0005b6c0: 3a0d 0a09 0909 0909 0909 096f 732e 7265  :..........os.re
-0005b6d0: 6d6f 7665 2827 7465 6d70 5f66 696c 652e  move('temp_file.
-0005b6e0: 6a73 6f6e 2729 0d0a 0909 0909 0909 0965  json').........e
-0005b6f0: 7863 6570 743a 0d0a 0909 0909 0909 0909  xcept:..........
-0005b700: 7061 7373 0d0a 0909 0909 0909 656c 7365  pass........else
-0005b710: 3a23 6e65 7720 7479 7065 206f 6620 6461  :#new type of da
-0005b720: 7461 0d0a 0909 0909 0909 0972 6169 7365  ta.........raise
-0005b730: 0909 0d0a 0909 0909 0965 6c73 653a 0d0a  .........else:..
-0005b740: 0909 0909 0909 7265 6164 3d66 5b6b 6579  ......read=f[key
-0005b750: 5d5b 2829 5d0d 0a09 0909 0909 0969 6620  ][()]........if 
-0005b760: 6973 696e 7374 616e 6365 2872 6561 642c  isinstance(read,
-0005b770: 6279 7465 7329 3a0d 0a09 0909 0909 0909  bytes):.........
-0005b780: 7265 6164 3d66 5b6b 6579 5d2e 6173 7374  read=f[key].asst
-0005b790: 7228 295b 2829 5d20 0d0a 0909 0909 0909  r()[()] ........
-0005b7a0: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
-0005b7b0: 7265 6164 2c74 7970 6528 2768 656c 6c6f  read,type('hello
-0005b7c0: 2729 293a 0d0a 0909 0909 0909 0969 6620  ')):.........if 
-0005b7d0: 2872 6561 643d 3d27 4e6f 6e65 2729 206f  (read=='None') o
-0005b7e0: 7220 2872 6561 643d 3d27 6e6f 6e65 2729  r (read=='none')
-0005b7f0: 3a0d 0a09 0909 0909 0909 0972 6561 643d  :..........read=
-0005b800: 4e6f 6e65 0d0a 0909 0909 0909 656c 6966  None........elif
-0005b810: 206b 6579 2069 6e20 5b27 626f 7264 6572   key in ['border
-0005b820: 6375 7427 2c27 7469 6d65 6c69 6d69 7473  cut','timelimits
-0005b830: 272c 2766 6974 636f 6566 6627 2c27 7363  ','fitcoeff','sc
-0005b840: 6174 7465 7263 7574 275d 3a0d 0a09 0909  attercut']:.....
-0005b850: 0909 0909 7265 6164 3d5b 666c 6f61 7428  ....read=[float(
-0005b860: 6129 2066 6f72 2061 2069 6e20 7265 6164  a) for a in read
-0005b870: 5d0d 0a09 0909 0909 0965 6c69 6620 6b65  ]........elif ke
-0005b880: 7920 3d3d 2769 6e74 656e 7369 7479 5f72  y =='intensity_r
-0005b890: 616e 6765 273a 0d0a 0909 0909 0909 0972  ange':.........r
-0005b8a0: 6561 643d 5b66 6c6f 6174 2861 2920 666f  ead=[float(a) fo
-0005b8b0: 7220 6120 696e 2072 6561 645d 0d0a 0909  r a in read]....
-0005b8c0: 0909 0909 656c 6966 206b 6579 2069 6e20  ....elif key in 
-0005b8d0: 5b27 7265 6c5f 7469 6d65 272c 2772 656c  ['rel_time','rel
-0005b8e0: 5f77 6176 6527 5d3a 0d0a 0909 0909 0909  _wave']:........
-0005b8f0: 0972 6561 643d 6e70 2e61 7272 6179 2872  .read=np.array(r
-0005b900: 6561 642c 6474 7970 653d 6e70 2e66 6c6f  ead,dtype=np.flo
-0005b910: 6174 3634 290d 0a09 0909 0909 0965 6c69  at64)........eli
-0005b920: 6620 6b65 7920 696e 205b 2773 6361 7474  f key in ['scatt
-0005b930: 6572 6375 7427 5d3a 0d0a 0909 0909 0909  ercut']:........
-0005b940: 0974 7279 3a0d 0a09 0909 0909 0909 0972  .try:..........r
-0005b950: 6561 643d 5b66 6c6f 6174 2861 2920 666f  ead=[float(a) fo
-0005b960: 7220 6120 696e 2072 6561 645d 0d0a 0909  r a in read]....
-0005b970: 0909 0909 0965 7863 6570 743a 236d 6179  .....except:#may
-0005b980: 6265 2077 6520 6861 7665 2020 6120 6c69  be we have  a li
-0005b990: 7374 206f 6620 7363 6174 7465 7263 7574  st of scattercut
-0005b9a0: 730d 0a09 0909 0909 0909 0974 7279 3a0d  s..........try:.
-0005b9b0: 0a09 0909 0909 0909 0909 6f75 745f 6c69  ..........out_li
-0005b9c0: 7374 656e 3d5b 5d0d 0a09 0909 0909 0909  sten=[].........
-0005b9d0: 0909 666f 7220 6c69 7374 656e 2069 6e20  ..for listen in 
-0005b9e0: 7265 6164 3a0d 0a09 0909 0909 0909 0909  read:...........
-0005b9f0: 096f 7574 6c69 7374 656e 2e61 7070 656e  .outlisten.appen
-0005ba00: 6428 5b66 6c6f 6174 2861 2920 666f 7220  d([float(a) for 
-0005ba10: 6120 696e 206c 6973 7465 6e5d 290d 0a09  a in listen])...
-0005ba20: 0909 0909 0909 0965 7863 6570 743a 236e  .......except:#n
-0005ba30: 6f20 6964 6561 206c 6574 7320 7365 6520  o idea lets see 
-0005ba40: 7768 6174 2068 6170 7065 6e73 0d0a 0909  what happens....
-0005ba50: 0909 0909 0909 0970 6173 730d 0a09 0909  .......pass.....
-0005ba60: 0909 0973 656c 662e 5f5f 6469 6374 5f5f  ...self.__dict__
-0005ba70: 5b6b 6579 5d3d 7265 6164 0d0a 0909 0909  [key]=read......
-0005ba80: 6578 6365 7074 3a23 7765 276c 6c20 6765  except:#we'll ge
-0005ba90: 7420 616e 2065 7863 6570 7469 6f6e 2065  t an exception e
-0005baa0: 7665 7279 2074 696d 6520 7468 6572 6520  very time there 
-0005bab0: 6973 2061 6e20 6461 7461 6672 616d 650d  is an dataframe.
-0005bac0: 0a09 0909 0909 2370 7269 6e74 2827 4672  ......#print('Fr
-0005bad0: 616d 653a 272b 6b65 7929 0d0a 0909 0909  ame:'+key)......
-0005bae0: 0964 6174 615f 6672 616d 655f 6c69 7374  .data_frame_list
-0005baf0: 2e61 7070 656e 6428 6b65 7929 0d0a 0d0a  .append(key)....
-0005bb00: 0909 7472 793a 0d0a 0909 0966 2e63 6c6f  ..try:.....f.clo
-0005bb10: 7365 2829 0d0a 0909 6578 6365 7074 3a0d  se()....except:.
-0005bb20: 0a09 0909 7061 7373 0d0a 0909 666f 7220  ....pass....for 
-0005bb30: 6b65 7920 696e 2064 6174 615f 6672 616d  key in data_fram
-0005bb40: 655f 6c69 7374 3a0d 0a09 0909 7472 793a  e_list:.....try:
-0005bb50: 0d0a 0909 0909 6966 2022 7265 5f22 2069  ......if "re_" i
-0005bb60: 6e20 6b65 795b 3a33 5d3a 0d0a 0909 0909  n key[:3]:......
-0005bb70: 0923 7072 696e 7428 2772 6520 696e 206c  .#print('re in l
-0005bb80: 6973 7427 290d 0a09 0909 0909 7365 6c66  ist').......self
-0005bb90: 2e5f 5f64 6963 745f 5f5b 2772 6527 5d5b  .__dict__['re'][
-0005bba0: 6b65 795b 333a 5d5d 3d70 616e 6461 732e  key[3:]]=pandas.
-0005bbb0: 7265 6164 5f68 6466 2873 6176 6564 5f70  read_hdf(saved_p
-0005bbc0: 726f 6a65 6374 2c6b 6579 3d6b 6579 2c6d  roject,key=key,m
-0005bbd0: 6f64 653d 2772 272c 6461 7461 5f63 6f6c  ode='r',data_col
-0005bbe0: 756d 6e73 3d54 7275 6529 0d0a 0909 0909  umns=True)......
-0005bbf0: 656c 6966 206b 6579 2069 6e20 5b27 6473  elif key in ['ds
-0005bc00: 5f6f 7269 272c 2770 6172 5f66 6974 272c  _ori','par_fit',
-0005bc10: 2770 6172 275d 3a0d 0a09 0909 0909 7365  'par']:.......se
-0005bc20: 6c66 2e5f 5f64 6963 745f 5f5b 6b65 795d  lf.__dict__[key]
-0005bc30: 3d70 616e 6461 732e 7265 6164 5f68 6466  =pandas.read_hdf
-0005bc40: 2873 6176 6564 5f70 726f 6a65 6374 2c6b  (saved_project,k
-0005bc50: 6579 3d6b 6579 2c6d 6f64 653d 2772 272c  ey=key,mode='r',
-0005bc60: 6461 7461 5f63 6f6c 756d 6e73 3d54 7275  data_columns=Tru
-0005bc70: 6529 0d0a 0909 0909 656c 7365 3a0d 0a09  e)......else:...
-0005bc80: 0909 0909 7072 696e 7428 226d 6973 7369  ....print("missi
-0005bc90: 6e67 206b 6579 3a22 202b 206b 6579 290d  ng key:" + key).
-0005bca0: 0a09 0909 6578 6365 7074 3a0d 0a09 0909  ....except:.....
-0005bcb0: 0969 6620 6b65 7920 3d3d 2027 7061 7227  .if key == 'par'
-0005bcc0: 2061 6e64 206f 6c64 5f73 7769 7463 683a   and old_switch:
-0005bcd0: 7061 7373 2023 2077 6520 6861 7665 2072  pass # we have r
-0005bce0: 6561 6420 6974 2062 6566 6f72 6520 616c  ead it before al
-0005bcf0: 7265 6164 7920 616e 6420 7468 6520 6572  ready and the er
-0005bd00: 726f 7220 6973 206f 6b0d 0a09 0920 0d0a  ror is ok.... ..
-0005bd10: 0909 0909 656c 7365 3a70 7269 6e74 2822  ....else:print("
-0005bd20: 6572 726f 7220 696e 206b 6579 3a22 202b  error in key:" +
-0005bd30: 206b 6579 290d 0a09 090d 0a09 0974 7279   key)........try
-0005bd40: 3a0d 0a09 0909 7365 6c66 2e5f 5f64 6963  :.....self.__dic
-0005bd50: 745f 5f5b 2772 6527 5d5b 2766 6974 5f72  t__['re']['fit_r
-0005bd60: 6573 756c 7473 5f72 6174 6573 275d 3d73  esults_rates']=s
-0005bd70: 656c 662e 5f5f 6469 6374 5f5f 5b27 7061  elf.__dict__['pa
-0005bd80: 725f 6669 7427 5d0d 0a09 0909 7365 6c66  r_fit'].....self
-0005bd90: 2e5f 5f64 6963 745f 5f5b 2772 6527 5d5b  .__dict__['re'][
-0005bda0: 2766 6974 5f72 6573 756c 7473 5f74 696d  'fit_results_tim
-0005bdb0: 6573 275d 3d70 6172 6466 5f74 6f5f 7469  es']=pardf_to_ti
-0005bdc0: 6d65 6466 2873 656c 662e 5f5f 6469 6374  medf(self.__dict
-0005bdd0: 5f5f 5b27 7265 275d 5b27 6669 745f 7265  __['re']['fit_re
-0005bde0: 7375 6c74 735f 7261 7465 7327 5d29 0d0a  sults_rates'])..
-0005bdf0: 0909 6578 6365 7074 3a0d 0a09 0909 7061  ..except:.....pa
-0005be00: 7373 0d0a 0909 0d0a 0909 2374 6865 2070  ss........#the p
-0005be10: 6172 2063 6f6e 7665 7273 696f 6e20 6675  ar conversion fu
-0005be20: 6e63 7469 6f6e 2066 6169 6c65 642c 2071  nction failed, q
-0005be30: 7569 636b 6669 780d 0a09 0966 6f72 206f  uickfix....for o
-0005be40: 7665 725f 6b65 7920 696e 205b 2770 6172  ver_key in ['par
-0005be50: 5f66 6974 272c 2770 6172 275d 3a0d 0a09  _fit','par']:...
-0005be60: 0909 7472 793a 0d0a 0909 0909 7061 725f  ..try:......par_
-0005be70: 6466 3d73 656c 662e 5f5f 6469 6374 5f5f  df=self.__dict__
-0005be80: 5b6f 7665 725f 6b65 795d 2e6c 6f63 5b3a  [over_key].loc[:
-0005be90: 2c5b 2776 616c 7565 272c 276d 696e 272c  ,['value','min',
-0005bea0: 276d 6178 272c 2776 6172 7927 2c27 6578  'max','vary','ex
-0005beb0: 7072 275d 5d0d 0a09 0909 0970 6172 3d6c  pr']]......par=l
-0005bec0: 6d66 6974 2e50 6172 616d 6574 6572 7328  mfit.Parameters(
-0005bed0: 290d 0a09 0909 0966 6f72 206b 6579 2069  )......for key i
-0005bee0: 6e20 7061 725f 6466 2e69 6e64 6578 2e76  n par_df.index.v
-0005bef0: 616c 7565 733a 0d0a 0909 0909 0970 6172  alues:.......par
-0005bf00: 2e61 6464 286b 6579 2c20 7661 6c75 653d  .add(key, value=
-0005bf10: 7061 725f 6466 2e6c 6f63 5b6b 6579 2c27  par_df.loc[key,'
-0005bf20: 7661 6c75 6527 5d2c 2076 6172 793d 7061  value'], vary=pa
-0005bf30: 725f 6466 2e6c 6f63 5b6b 6579 2c27 7661  r_df.loc[key,'va
-0005bf40: 7279 275d 2c20 6d69 6e3d 7061 725f 6466  ry'], min=par_df
-0005bf50: 2e6c 6f63 5b6b 6579 2c27 6d69 6e27 5d2c  .loc[key,'min'],
-0005bf60: 206d 6178 3d70 6172 5f64 662e 6c6f 635b   max=par_df.loc[
-0005bf70: 6b65 792c 276d 6178 275d 290d 0a09 0909  key,'max']).....
-0005bf80: 0909 0909 0909 0909 0909 0909 2020 0d0a  ............  ..
-0005bf90: 0909 0909 7365 6c66 2e5f 5f64 6963 745f  ....self.__dict_
-0005bfa0: 5f5b 6f76 6572 5f6b 6579 5d3d 7061 720d  _[over_key]=par.
-0005bfb0: 0a09 0909 6578 6365 7074 3a0d 0a09 0909  ....except:.....
-0005bfc0: 0970 6173 730d 0a09 0969 6620 6f6c 645f  .pass....if old_
-0005bfd0: 7377 6974 6368 3a0d 0a09 0909 7472 793a  switch:.....try:
-0005bfe0: 0d0a 0909 0909 7365 6c66 2e5f 5f64 6963  ......self.__dic
-0005bff0: 745f 5f5b 2772 6527 5d5b 2766 6974 5f72  t__['re']['fit_r
-0005c000: 6573 756c 7473 5f72 6174 6573 275d 3d70  esults_rates']=p
-0005c010: 6172 5f74 6f5f 7061 7264 6628 7365 6c66  ar_to_pardf(self
-0005c020: 2e70 6172 290d 0a09 0909 0973 656c 662e  .par)......self.
-0005c030: 5f5f 6469 6374 5f5f 5b27 7265 275d 5b27  __dict__['re']['
-0005c040: 6669 745f 7265 7375 6c74 735f 7469 6d65  fit_results_time
-0005c050: 7327 5d3d 7061 7264 665f 746f 5f74 696d  s']=pardf_to_tim
-0005c060: 6564 6628 7061 725f 746f 5f70 6172 6466  edf(par_to_pardf
-0005c070: 2873 656c 662e 7061 7229 290d 0a09 0909  (self.par)).....
-0005c080: 0973 656c 662e 5f5f 6469 6374 5f5f 5b27  .self.__dict__['
-0005c090: 7061 725f 6669 7427 5d3d 7365 6c66 2e70  par_fit']=self.p
-0005c0a0: 6172 0d0a 0909 0965 7863 6570 743a 0d0a  ar.....except:..
-0005c0b0: 0909 0909 7061 7373 0d0a 0909 7365 6c66  ....pass....self
-0005c0c0: 2e73 6176 655f 6669 6775 7265 735f 746f  .save_figures_to
-0005c0d0: 5f66 6f6c 6465 723d 4661 6c73 650d 0a09  _folder=False...
-0005c0e0: 0973 656c 662e 7061 7468 3d63 7572 7265  .self.path=curre
-0005c0f0: 6e74 5f70 6174 680d 0a09 0969 6620 6f6c  nt_path....if ol
-0005c100: 645f 7377 6974 6368 3a23 636f 6e76 6572  d_switch:#conver
-0005c110: 7420 7072 6f6a 6563 7420 696e 746f 206e  t project into n
-0005c120: 6577 2074 7970 650d 0a09 0909 2363 6c65  ew type.....#cle
-0005c130: 616e 206f 6c64 2066 696c 6573 2074 6861  an old files tha
-0005c140: 7420 7765 7265 2072 6561 6420 7772 6f6e  t were read wron
-0005c150: 670d 0a09 0909 666f 7220 6b65 7920 696e  g.....for key in
-0005c160: 205b 2772 655f 6669 6e61 6c5f 696e 745f   ['re_final_int_
-0005c170: 7061 7227 2c27 7265 5f66 696e 616c 5f73  par','re_final_s
-0005c180: 6574 7570 5f70 6172 272c 2772 655f 6669  etup_par','re_fi
-0005c190: 6e61 6c5f 7469 6d65 5f70 6172 272c 2772  nal_time_par','r
-0005c1a0: 655f 696e 745f 6572 726f 7227 5d3a 0d0a  e_int_error']:..
-0005c1b0: 0909 0909 7472 793a 0d0a 0909 0909 0964  ....try:.......d
-0005c1c0: 656c 2073 656c 662e 5f5f 6469 6374 5f5f  el self.__dict__
-0005c1d0: 5b6b 6579 5d0d 0a09 0909 0965 7863 6570  [key]......excep
-0005c1e0: 7420 4b65 7945 7272 6f72 3a0d 0a09 0909  t KeyError:.....
-0005c1f0: 0909 7072 696e 7428 6627 4b65 7920 7b6b  ..print(f'Key {k
-0005c200: 6579 7d20 6973 206e 6f74 2069 6e20 7468  ey} is not in th
-0005c210: 6520 6469 6374 696f 6e61 7279 2729 0d0a  e dictionary')..
-0005c220: 0909 0966 6f72 206b 6579 2069 6e20 5b27  ...for key in ['
-0005c230: 6669 6e61 6c5f 696e 745f 7061 7227 2c27  final_int_par','
-0005c240: 6669 6e61 6c5f 7365 7475 705f 7061 7227  final_setup_par'
-0005c250: 2c27 6669 6e61 6c5f 7469 6d65 5f70 6172  ,'final_time_par
-0005c260: 272c 2769 6e74 5f65 7272 6f72 275d 3a0d  ','int_error']:.
-0005c270: 0a09 0909 0974 7279 3a0d 0a09 0909 0909  .....try:.......
-0005c280: 6465 6c20 7365 6c66 2e5f 5f64 6963 745f  del self.__dict_
-0005c290: 5f5b 2772 6527 5d5b 6b65 795d 0d0a 0909  _['re'][key]....
-0005c2a0: 0909 6578 6365 7074 204b 6579 4572 726f  ..except KeyErro
-0005c2b0: 723a 0d0a 0909 0909 0970 7269 6e74 2866  r:.......print(f
-0005c2c0: 274b 6579 207b 6b65 797d 2069 7320 6e6f  'Key {key} is no
-0005c2d0: 7420 696e 2074 6865 2064 6963 7469 6f6e  t in the diction
-0005c2e0: 6172 7927 290d 0a09 0909 7472 793a 0d0a  ary').....try:..
-0005c2f0: 0909 0909 7365 6c66 2e73 6176 655f 7072  ....self.save_pr
-0005c300: 6f6a 6563 7428 290d 0a09 0909 0970 7269  oject()......pri
-0005c310: 6e74 2822 7072 6f6a 6563 7420 636f 6e76  nt("project conv
-0005c320: 6572 7465 6420 696e 746f 206e 6577 2064  erted into new d
-0005c330: 6174 6120 7479 7065 2061 6e64 2073 6176  ata type and sav
-0005c340: 6564 2061 6761 696e 2229 0d0a 0909 0965  ed again").....e
-0005c350: 7863 6570 743a 0d0a 0909 0909 7072 696e  xcept:......prin
-0005c360: 7428 2270 726f 6a65 6374 2063 6f6e 7665  t("project conve
-0005c370: 7274 6564 2069 6275 7420 636f 756c 6420  rted ibut could 
-0005c380: 6e6f 7420 6265 2073 6176 6564 2229 0d0a  not be saved")..
-0005c390: 0909 7365 6c66 2e70 6174 683d 6375 7272  ..self.path=curr
-0005c3a0: 656e 745f 7061 7468 0d0a 0909 666f 7220  ent_path....for 
-0005c3b0: 6b65 7920 696e 205b 2774 696d 655f 6269  key in ['time_bi
-0005c3c0: 6e27 2c27 7265 6c5f 7761 7665 272c 2772  n','rel_wave','r
-0005c3d0: 656c 5f74 696d 6527 2c27 7363 6174 7465  el_time','scatte
-0005c3e0: 7263 7574 272c 2762 6f72 6465 7263 7574  rcut','bordercut
-0005c3f0: 272c 2774 696d 656c 696d 6974 7327 2c27  ','timelimits','
-0005c400: 696e 7465 6e73 6974 795f 7261 6e67 6527  intensity_range'
-0005c410: 2c27 7761 7665 5f6e 6d5f 6269 6e27 2c27  ,'wave_nm_bin','
-0005c420: 7761 7665 6c65 6e67 7468 5f62 696e 272c  wavelength_bin',
-0005c430: 2769 676e 6f72 655f 7469 6d65 5f72 6567  'ignore_time_reg
-0005c440: 696f 6e27 5d3a 0d0a 0909 0974 7279 3a0d  ion']:.....try:.
-0005c450: 0a09 0909 0969 6620 6973 696e 7374 616e  .....if isinstan
-0005c460: 6365 2873 656c 662e 5f5f 6469 6374 5f5f  ce(self.__dict__
-0005c470: 5b6b 6579 5d2c 6279 7465 7329 3a0d 0a09  [key],bytes):...
-0005c480: 0909 0909 2370 7269 6e74 286b 6579 202b  ....#print(key +
-0005c490: 2027 2073 6574 2074 6f20 4e6f 6e65 2729   ' set to None')
-0005c4a0: 0d0a 0909 0909 0973 656c 662e 5f5f 6469  .......self.__di
-0005c4b0: 6374 5f5f 5b6b 6579 5d3d 4e6f 6e65 0d0a  ct__[key]=None..
-0005c4c0: 0909 0909 656c 6966 2069 7369 6e73 7461  ....elif isinsta
-0005c4d0: 6e63 6528 7365 6c66 2e5f 5f64 6963 745f  nce(self.__dict_
-0005c4e0: 5f5b 6b65 795d 2c73 7472 293a 0d0a 0909  _[key],str):....
-0005c4f0: 0909 0969 6620 7365 6c66 2e5f 5f64 6963  ...if self.__dic
-0005c500: 745f 5f5b 6b65 795d 3d3d 274e 6f6e 6527  t__[key]=='None'
-0005c510: 3a0d 0a09 0909 0909 0973 656c 662e 5f5f  :........self.__
-0005c520: 6469 6374 5f5f 5b6b 6579 5d3d 4e6f 6e65  dict__[key]=None
-0005c530: 0d0a 0909 0965 7863 6570 743a 0d0a 0909  .....except:....
-0005c540: 0909 636f 6e74 696e 7565 0d0a 0909 7472  ..continue....tr
-0005c550: 793a 0d0a 0909 0973 656c 662e 6669 6775  y:.....self.figu
-0005c560: 7265 5f70 6174 683d 7374 7228 7365 6c66  re_path=str(self
-0005c570: 2e66 6967 7572 655f 7061 7468 290d 0a09  .figure_path)...
-0005c580: 0909 6966 2027 4e6f 6e65 2720 696e 2073  ..if 'None' in s
-0005c590: 656c 662e 6669 6775 7265 5f70 6174 683a  elf.figure_path:
-0005c5a0: 0d0a 0909 0909 7365 6c66 2e66 6967 7572  ......self.figur
-0005c5b0: 655f 7061 7468 3d4e 6f6e 650d 0a09 0965  e_path=None....e
-0005c5c0: 7863 6570 743a 0d0a 0909 0970 6173 730d  xcept:.....pass.
-0005c5d0: 0a0d 0a09 6465 6620 436f 7079 2873 656c  ....def Copy(sel
-0005c5e0: 6629 3a0d 0a09 0927 2727 7265 7475 726e  f):....'''return
-0005c5f0: 7320 6120 6465 6570 2063 6f70 7920 6f66  s a deep copy of
-0005c600: 2074 6865 206f 626a 6563 742e 0d0a 0909   the object.....
-0005c610: 0d0a 0909 4578 616d 706c 6573 0d0a 0909  ....Examples....
-0005c620: 2d2d 2d2d 2d2d 2d2d 0d0a 0909 3e3e 3e74  --------....>>>t
-0005c630: 613d 706c 6f74 5f66 756e 632e 5441 2827  a=plot_func.TA('
-0005c640: 7465 7374 6669 6c65 2e68 6466 3527 2920  testfile.hdf5') 
-0005c650: 236f 7065 6e20 6120 7072 6f6a 6563 740d  #open a project.
-0005c660: 0a09 093e 3e3e 7461 313d 7461 2e43 6f70  ...>>>ta1=ta.Cop
-0005c670: 7928 2920 236d 616b 6520 6120 636f 7079  y() #make a copy
-0005c680: 2066 6f72 2073 6f6d 6520 7465 7374 7320   for some tests 
-0005c690: 6f72 2061 2064 6966 6665 726e 6574 2066  or a differnet f
-0005c6a0: 6974 0d0a 0909 0d0a 0909 2727 2720 0d0a  it........''' ..
-0005c6b0: 0909 696d 706f 7274 2063 6f70 790d 0a09  ..import copy...
-0005c6c0: 0972 6574 7572 6e20 636f 7079 2e64 6565  .return copy.dee
-0005c6d0: 7063 6f70 7928 7365 6c66 290d 0a0d 0a0d  pcopy(self).....
-0005c6e0: 0a09 6465 6620 436f 6d70 6172 655f 6174  ..def Compare_at
-0005c6f0: 5f74 696d 6528 7365 6c66 2c20 7265 6c5f  _time(self, rel_
-0005c700: 7469 6d65 203d 204e 6f6e 652c 206f 7468  time = None, oth
-0005c710: 6572 203d 204e 6f6e 652c 2066 6974 7465  er = None, fitte
-0005c720: 6420 3d20 4661 6c73 652c 206e 6f72 6d5f  d = False, norm_
-0005c730: 7769 6e64 6f77 203d 204e 6f6e 652c 0d0a  window = None,..
-0005c740: 0909 0909 0909 7469 6d65 5f77 6964 7468  ......time_width
-0005c750: 5f70 6572 6365 6e74 203d 204e 6f6e 652c  _percent = None,
-0005c760: 2073 7065 6374 7261 203d 204e 6f6e 652c   spectra = None,
-0005c770: 2064 6174 615f 616e 645f 6669 7420 3d20   data_and_fit = 
-0005c780: 4661 6c73 652c 2063 6d61 7020 3d20 4e6f  False, cmap = No
-0005c790: 6e65 202c 200d 0a09 0909 0909 0970 7269  ne , ........pri
-0005c7a0: 6e74 5f63 6c69 636b 5f70 6f73 6974 696f  nt_click_positio
-0005c7b0: 6e20 3d20 4661 6c73 652c 206c 696e 6577  n = False, linew
-0005c7c0: 6964 7468 203d 2031 2c20 7469 746c 653d  idth = 1, title=
-0005c7d0: 2727 2c20 706c 6f74 5f73 6563 6f6e 645f  '', plot_second_
-0005c7e0: 6173 5f65 6e65 7267 7920 3d20 5472 7565  as_energy = True
-0005c7f0: 293a 0d0a 0909 2727 2754 6869 7320 6675  ):....'''This fu
-0005c800: 6e63 7469 6f6e 2070 6c6f 7473 206d 756c  nction plots mul
-0005c810: 7469 706c 6520 7370 6563 7472 6120 696e  tiple spectra in
-0005c820: 746f 2074 6865 2073 616d 6520 6669 6775  to the same figu
-0005c830: 7265 2061 7420 6120 6769 7665 6e20 7265  re at a given re
-0005c840: 6c5f 7469 6d65 2028 7469 6d65 706f 696e  l_time (timepoin
-0005c850: 7473 2920 616e 6420 0d0a 0909 616c 6c6f  ts) and ....allo
-0005c860: 7773 2066 6f72 206e 6f72 6d61 6c69 7a61  ws for normaliza
-0005c870: 7469 6f6e 2e20 5665 7279 2075 7365 6675  tion. Very usefu
-0005c880: 6c20 746f 2063 6f6d 7061 7265 2074 6865  l to compare the
-0005c890: 2073 7065 6374 7261 2066 6f72 2064 6966   spectra for dif
-0005c8a0: 6665 7265 6e74 2073 6f6c 7665 6e74 7320  ferent solvents 
-0005c8b0: 6f72 2071 7565 6e63 6865 7273 2c20 6f72  or quenchers, or
-0005c8c0: 0d0a 0909 652e 672e 2064 6966 6665 7265  ....e.g. differe
-0005c8d0: 6e74 2066 6974 732e 2054 6865 2074 612e  nt fits. The ta.
-0005c8e0: 7469 6d65 5f77 6964 7468 5f70 6572 6365  time_width_perce
-0005c8f0: 6e74 2070 6172 616d 6574 6572 2064 6566  nt parameter def
-0005c900: 696e 6573 2069 6620 7468 6973 2069 7320  ines if this is 
-0005c910: 610d 0a09 0973 696e 676c 6520 7469 6d65  a....single time
-0005c920: 2028 6966 2074 696d 655f 7769 6474 685f   (if time_width_
-0005c930: 7065 7263 656e 7420 3d20 3029 206f 7220  percent = 0) or 
-0005c940: 616e 2069 6e74 6567 7261 7465 6420 7769  an integrated wi
-0005c950: 6e64 6f77 2e0d 0a09 094f 6e6c 7920 2272  ndow.....Only "r
-0005c960: 656c 5f74 696d 6522 2069 7320 6120 6d61  el_time" is a ma
-0005c970: 6e64 6174 6f72 792c 2074 6865 2072 6573  ndatory, the res
-0005c980: 7420 6361 6e20 6265 2074 616b 656e 2066  t can be taken f
-0005c990: 726f 6d20 7468 6520 6f72 6967 696e 616c  rom the original
-0005c9a0: 2070 726f 6a65 6374 2028 7461 292e 0d0a   project (ta)...
-0005c9b0: 0909 0d0a 0909 5468 6520 6e6f 726d 616c  ......The normal
-0005c9c0: 697a 6174 696f 6e20 6973 2072 6561 6c69  ization is reali
-0005c9d0: 7a65 6420 6279 2067 6976 696e 6720 6120  zed by giving a 
-0005c9e0: 6e6f 726d 5f77 696e 646f 7720 0d0a 0909  norm_window ....
-0005c9f0: 6174 2077 6869 6368 2074 6865 2069 6e74  at which the int
-0005ca00: 656e 7369 7479 2069 6e20 7468 6520 7472  ensity in the tr
-0005ca10: 6967 6765 7269 6e67 206f 626a 6563 7420  iggering object 
-0005ca20: 6973 2069 6e74 6567 7261 7465 6420 2869  is integrated (i
-0005ca30: 6e20 7461 2e43 6f6d 7061 7265 5f61 745f  n ta.Compare_at_
-0005ca40: 7469 6d65 286f 7468 6572 2e2e 2920 0d0a  time(other..) ..
-0005ca50: 0909 2274 6122 2069 7320 7468 6520 7472  .."ta" is the tr
-0005ca60: 6967 6765 7269 6e67 206f 626a 6563 742e  iggering object.
-0005ca70: 2054 6865 2069 6e20 6561 6368 206f 6620   The in each of 
-0005ca80: 7468 6520 6f74 6865 7220 6375 7276 6573  the other curves
-0005ca90: 2074 6865 2073 616d 6520 7769 6e64 6f77   the same window
-0005caa0: 2069 730d 0a09 0969 6e74 6567 7261 7465   is....integrate
-0005cab0: 6420 616e 6420 7468 6520 6375 7276 6520  d and the curve 
-0005cac0: 7363 616c 6564 2062 7920 7468 6973 2076  scaled by this v
-0005cad0: 616c 7565 2e20 496d 706f 7274 616e 7420  alue. Important 
-0005cae0: 746f 206e 6f74 6520 6973 2074 6861 7420  to note is that 
-0005caf0: 7468 6973 2077 696e 646f 770d 0a09 0964  this window....d
-0005cb00: 6f65 7320 6e6f 7420 6e65 6564 2074 6f20  oes not need to 
-0005cb10: 6265 2069 6e20 7468 6520 706c 6f74 2e20  be in the plot. 
-0005cb20: 652e 672e 2074 6865 206e 6f72 6d61 6c69  e.g. the normali
-0005cb30: 7a61 7469 6f6e 2063 616e 2062 6520 646f  zation can be do
-0005cb40: 6e65 2061 7420 6120 6469 6666 6572 656e  ne at a differen
-0005cb50: 7420 7469 6d65 2e0d 0a09 090d 0a09 0956  t time.........V
-0005cb60: 6572 7920 6f66 7465 6e20 6f6e 6520 776f  ery often one wo
-0005cb70: 756c 6420 6c69 6b65 2074 6f20 636f 6d70  uld like to comp
-0005cb80: 6172 6520 7468 6520 6d65 6173 7572 6564  are the measured
-0005cb90: 2073 7065 6374 7261 2061 7420 6120 6365   spectra at a ce
-0005cba0: 7274 6169 6e0d 0a09 0974 696d 6520 746f  rtain....time to
-0005cbb0: 2061 6e20 6578 7465 726e 616c 2073 7065   an external spe
-0005cbc0: 6374 7275 6d20 2865 2e67 2e20 7370 6563  ctrum (e.g. spec
-0005cbd0: 7472 6f2d 656c 6563 7472 6f2d 6368 656d  tro-electro-chem
-0005cbe0: 6973 7472 7920 6f72 2073 7465 6164 790d  istry or steady.
-0005cbf0: 0a09 0973 7461 7465 2061 6273 6f72 7074  ...state absorpt
-0005cc00: 696f 6e29 2e20 5468 6973 2063 616e 2062  ion). This can b
-0005cc10: 6520 646f 6e65 2062 7920 6c6f 6164 696e  e done by loadin
-0005cc20: 6720 6120 7370 6563 6966 6963 2073 7065  g a specific spe
-0005cc30: 6374 7275 6d20 696e 746f 0d0a 0909 6120  ctrum into....a 
-0005cc40: 4461 7461 4672 616d 6520 616e 6420 6861  DataFrame and ha
-0005cc50: 6e64 696e 6720 7468 6973 2064 6174 6120  nding this data 
-0005cc60: 4672 616d 6520 746f 2074 6865 2063 6f6d  Frame to the com
-0005cc70: 7061 7269 7369 6f6e 2066 756e 6374 696f  parision functio
-0005cc80: 6e2e 2054 6865 0d0a 0909 6675 6e63 7469  n. The....functi
-0005cc90: 6f6e 2063 616e 2061 6c73 6f20 6265 2075  on can also be u
-0005cca0: 7365 6420 746f 2070 6c6f 7420 652e 672e  sed to plot e.g.
-0005ccb0: 2074 6865 206d 6561 7375 7265 6420 7370   the measured sp
-0005ccc0: 6563 7472 6120 7673 2e20 616e 0d0a 0909  ectra vs. an....
-0005ccd0: 6578 7465 726e 616c 2073 7065 6374 7275  external spectru
-0005cce0: 6d20 7769 7468 6f75 7420 6769 7669 6e67  m without giving
-0005ccf0: 2061 6e79 2022 6f74 6865 7222 2050 726f   any "other" Pro
-0005cd00: 6a65 6374 732e 2028 7665 7279 2075 7365  jects. (very use
-0005cd10: 6675 6c20 666f 720d 0a09 0963 6f6d 7061  ful for....compa
-0005cd20: 7269 7369 6f6e 7329 2e0d 0a09 0920 0d0a  risions)..... ..
-0005cd30: 0909 5061 7261 6d65 7465 7273 0d0a 0909  ..Parameters....
-0005cd40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a09  -------------...
-0005cd50: 090d 0a09 0972 656c 5f74 696d 6520 3a20  .....rel_time : 
-0005cd60: 666c 6f61 7420 6f72 206c 6973 742f 7665  float or list/ve
-0005cd70: 6374 6f72 2028 6f66 2066 6c6f 6174 7329  ctor (of floats)
-0005cd80: 0d0a 0909 0953 7065 6369 6679 2074 6865  .....Specify the
-0005cd90: 2074 696d 6573 2077 6865 7265 2074 6f20   times where to 
-0005cda0: 706c 6f74 2c20 7369 6e67 6c65 2076 616c  plot, single val
-0005cdb0: 7565 206f 7220 6c69 7374 2f76 6563 746f  ue or list/vecto
-0005cdc0: 7220 6f66 2076 616c 7565 732e 200d 0a09  r of values. ...
-0005cdd0: 0909 466f 7220 6561 6368 2065 6e74 7279  ..For each entry
-0005cde0: 2069 6e20 7265 6c5f 7469 6d65 2061 2073   in rel_time a s
-0005cdf0: 7065 6374 7275 6d20 6973 2070 6c6f 7474  pectrum is plott
-0005ce00: 6564 2e20 0d0a 0909 0949 6620 7469 6d65  ed. .....If time
-0005ce10: 5f77 6964 7468 5f70 6572 6365 6e74 3d30  _width_percent=0
-0005ce20: 2028 4465 6661 756c 7429 2074 6865 206e   (Default) the n
-0005ce30: 6561 7265 7374 206d 6561 7375 7265 6420  earest measured 
-0005ce40: 0d0a 0909 0974 696d 6570 6f69 6e74 2069  .....timepoint i
-0005ce50: 7320 6368 6f73 656e 2e20 466f 7220 6f74  s chosen. For ot
-0005ce60: 6865 7220 7661 6c75 6573 2073 6565 2070  her values see p
-0005ce70: 6172 616d 6574 6572 2022 7469 6d65 5f77  arameter "time_w
-0005ce80: 6964 7468 5f70 6572 6365 6e74 222e 0d0a  idth_percent"...
-0005ce90: 0909 090d 0a09 096f 7468 6572 203a 2054  .......other : T
-0005cea0: 4120 6f62 6a65 6374 206f 7220 6c69 7374  A object or list
-0005ceb0: 206f 6620 7468 6f73 652c 206f 7074 696f   of those, optio
-0005cec0: 6e61 6c20 0d0a 0909 0973 686f 756c 6420  nal .....should 
-0005ced0: 6265 2074 612e 706c 6f74 5f66 756e 6320  be ta.plot_func 
-0005cee0: 6f62 6a65 6374 7320 286c 6f61 6465 6420  objects (loaded 
-0005cef0: 6f72 2063 6f70 6965 6429 2061 6e64 2069  or copied) and i
-0005cf00: 7320 7768 6174 200d 0a09 0909 6973 2070  s what .....is p
-0005cf10: 6c6f 7474 6564 2061 6761 696e 7374 2074  lotted against t
-0005cf20: 6865 2064 6174 6120 7573 6520 6120 6c69  he data use a li
-0005cf30: 7374 205b 7461 312c 7461 322c 2e2e 2e20  st [ta1,ta2,... 
-0005cf40: 5d20 6f72 2067 656e 6572 6174 6520 7468  ] or generate th
-0005cf50: 6973 0d0a 0909 096c 6973 7420 7573 696e  is.....list usin
-0005cf60: 6720 7468 6520 4775 6920 6675 6e63 7469  g the Gui functi
-0005cf70: 6f6e 2e20 5365 6520 7365 6374 696f 6e20  on. See section 
-0005cf80: 3a72 6566 3a60 4f70 656e 696e 6720 6d75  :ref:`Opening mu
-0005cf90: 6c74 6970 6c65 2066 696c 6573 6020 696e  ltiple files` in
-0005cfa0: 200d 0a09 0909 7468 6520 646f 6375 6d65   .....the docume
-0005cfb0: 6e74 6174 696f 6e0d 0a09 090d 0a09 0966  ntation........f
-0005cfc0: 6974 7465 6420 3a20 626f 6f6c 2c20 6f70  itted : bool, op
-0005cfd0: 7469 6f6e 616c 0d0a 0909 0954 7275 652f  tional.....True/
-0005cfe0: 4661 6c73 6520 2844 6566 6175 6c74 2920  False (Default) 
-0005cff0: 2d20 7573 6520 6669 7474 6564 2064 6174  - use fitted dat
-0005d000: 6120 696e 7374 6561 6420 6f66 2072 6177  a instead of raw
-0005d010: 2064 6174 612e 200d 0a09 0909 4966 2054   data. .....If T
-0005d020: 7275 652c 2074 6865 2066 6974 7465 6420  rue, the fitted 
-0005d030: 6461 7461 706f 696e 7473 2028 7769 7468  datapoints (with
-0005d040: 6f75 7420 696e 7465 7270 6f6c 6174 696f  out interpolatio
-0005d050: 6e29 2061 7265 2075 7365 642e 200d 0a09  n) are used. ...
-0005d060: 0909 5468 6973 2069 7320 696e 7465 6e64  ..This is intend
-0005d070: 6564 2066 6f72 2063 6f6d 7061 7269 6e67  ed for comparing
-0005d080: 2065 2e67 2e20 6469 6666 6572 656e 7420   e.g. different 
-0005d090: 6669 7473 0d0a 0909 0d0a 0909 6e6f 726d  fits........norm
-0005d0a0: 5f77 696e 646f 7720 3a20 4e6f 6e65 206f  _window : None o
-0005d0b0: 7220 6c69 7374 2f76 6563 746f 7220 2877  r list/vector (w
-0005d0c0: 6974 6820 3420 666c 6f61 7473 292c 206f  ith 4 floats), o
-0005d0d0: 7074 696f 6e61 6c0d 0a09 0909 6e6f 726d  ptional.....norm
-0005d0e0: 5f77 696e 646f 7720 4769 7665 2061 206c  _window Give a l
-0005d0f0: 6973 742f 7475 7065 6c2f 7665 6374 6f72  ist/tupel/vector
-0005d100: 2077 6974 6820 3420 656e 7472 6965 7320   with 4 entries 
-0005d110: 696e 2074 6865 206f 7264 6572 200d 0a09  in the order ...
-0005d120: 0909 5b53 7461 7274 202d 2074 696d 652c  ..[Start - time,
-0005d130: 2045 6e64 202d 2074 696d 652c 2053 7461   End - time, Sta
-0005d140: 7274 202d 2077 6176 656c 656e 6774 682c  rt - wavelength,
-0005d150: 2045 6e64 202d 2057 6176 656c 656e 6774   End - Wavelengt
-0005d160: 685d 2c20 0d0a 0909 0973 6565 2073 6563  h], .....see sec
-0005d170: 7469 6f6e 2020 3a72 6566 3a60 4e6f 726d  tion  :ref:`Norm
-0005d180: 616c 697a 6174 696f 6e20 616e 6420 5363  alization and Sc
-0005d190: 616c 696e 6760 2020 696e 2074 6865 2064  aling`  in the d
-0005d1a0: 6f63 756d 656e 7461 7469 6f6e 2e0d 0a09  ocumentation....
-0005d1b0: 0909 4966 204e 6f6e 6520 2844 6566 6175  ..If None (Defau
-0005d1c0: 6c74 2920 6e6f 206e 6f72 6d61 6c69 7a61  lt) no normaliza
-0005d1d0: 7469 6f6e 2069 7320 646f 6e65 2e0d 0a09  tion is done....
-0005d1e0: 090d 0a09 096c 696e 6577 6964 7468 203a  .....linewidth :
-0005d1f0: 2066 6c6f 6174 2c20 6f70 7469 6f6e 616c   float, optional
-0005d200: 0d0a 0909 096c 696e 6577 6964 7468 2074  .....linewidth t
-0005d210: 6f20 6265 2075 7365 6420 666f 7220 706c  o be used for pl
-0005d220: 6f74 7469 6e67 0909 0d0a 0909 0d0a 0909  otting..........
-0005d230: 7469 6d65 5f77 6964 7468 5f70 6572 6365  time_width_perce
-0005d240: 6e74 203a 204e 6f6e 6520 6f72 2066 6c6f  nt : None or flo
-0005d250: 6174 2c20 6f70 7469 6f6e 616c 0d0a 0909  at, optional....
-0005d260: 0922 7265 6c5f 7469 6d65 2220 616e 6420  ."rel_time" and 
-0005d270: 2274 696d 655f 7769 6474 685f 7065 7263  "time_width_perc
-0005d280: 656e 7422 2077 6f72 6b20 746f 6765 7468  ent" work togeth
-0005d290: 6572 2066 6f72 2063 7265 6174 696e 6720  er for creating 
-0005d2a0: 7370 6563 7472 616c 2070 6c6f 7473 2061  spectral plots a
-0005d2b0: 7420 0d0a 0909 0973 7065 6369 6669 6320  t .....specific 
-0005d2c0: 7469 6d65 706f 696e 7473 2e20 466f 7220  timepoints. For 
-0005d2d0: 6561 6368 2065 6e74 7279 2069 6e20 7265  each entry in re
-0005d2e0: 6c5f 7469 6d65 2061 2073 7065 6374 7275  l_time a spectru
-0005d2f0: 6d20 6973 2070 6c6f 7474 6564 2e20 0d0a  m is plotted. ..
-0005d300: 0909 0949 6620 686f 7765 7665 7220 652e  ...If however e.
-0005d310: 672e 2074 696d 655f 7769 6474 685f 7065  g. time_width_pe
-0005d320: 7263 656e 743d 3130 2074 6865 2072 6567  rcent=10 the reg
-0005d330: 696f 6e20 6265 7477 6565 6e20 7468 6520  ion between the 
-0005d340: 7469 6d65 706f 696e 7420 636c 6f73 6573  timepoint closes
-0005d350: 7420 0d0a 0909 0974 6f20 3a6d 6174 683a  t .....to :math:
-0005d360: 6074 696d 6570 6f69 6e74 2b30 2e31 7874  `timepoint+0.1xt
-0005d370: 696d 6570 6f69 6e74 c2b4 2061 6e64 203a  imepoint.. and :
-0005d380: 6d61 7468 3a60 7469 6d65 706f 696e 742d  math:`timepoint-
-0005d390: 302e 3178 7469 6d65 706f 696e 7460 2069  0.1xtimepoint` i
-0005d3a0: 7320 6176 6572 6167 6564 2061 6e64 2073  s averaged and s
-0005d3b0: 686f 776e 200d 0a09 0909 2861 6e64 2074  hown .....(and t
-0005d3c0: 6865 206c 6567 656e 6420 6164 6a75 7374  he legend adjust
-0005d3d0: 6564 2061 6363 6f72 6469 6e67 6c79 292e  ed accordingly).
-0005d3e0: 2049 6620 4e6f 6e65 2028 4465 6661 756c   If None (Defaul
-0005d3f0: 7429 2069 7320 6769 7665 6e2c 2074 6865  t) is given, the
-0005d400: 2076 616c 7565 2069 7320 0d0a 0909 0974   value is .....t
-0005d410: 616b 656e 2066 726f 6d20 7468 6520 7472  aken from the tr
-0005d420: 6967 6765 7269 6e67 206f 626a 6563 7420  iggering object 
-0005d430: 2873 656c 662e 7469 6d65 5f77 6964 7468  (self.time_width
-0005d440: 5f70 6572 6365 6e74 2920 5468 6973 2069  _percent) This i
-0005d450: 7320 7061 7274 6963 756c 6172 6c79 2075  s particularly u
-0005d460: 7365 6675 6c20 666f 7220 7468 6520 6465  seful for the de
-0005d470: 6e73 6c79 0d0a 0909 0973 616d 706c 6564  nsly.....sampled
-0005d480: 2072 6567 696f 6e20 636c 6f73 6520 746f   region close to
-0005d490: 2074 3d30 2e20 5479 7069 6361 6c6c 7920   t=0. Typically 
-0005d4a0: 666f 7220 6120 6c6f 6761 7269 7468 6d69  for a logarithmi
-0005d4b0: 6320 7265 636f 7264 6564 206b 696e 6574  c recorded kinet
-0005d4c0: 6963 732c 2074 6865 200d 0a09 0909 7469  ics, the .....ti
-0005d4d0: 6d65 706f 696e 7473 2061 7420 6c61 7465  mepoints at late
-0005d4e0: 7220 7469 6d65 7320 7769 6c6c 2062 6520  r times will be 
-0005d4f0: 6675 7274 6865 7220 6170 7061 7274 2074  further appart t
-0005d500: 6861 6e20 3130 2070 6572 6365 6e74 206f  han 10 percent o
-0005d510: 6620 7468 6520 7661 6c75 652c 200d 0a09  f the value, ...
-0005d520: 0909 6275 7420 7468 6973 2061 6c6c 6f77  ..but this allow
-0005d530: 7320 746f 2065 6c65 6761 6e74 6c79 2063  s to elegantly c
-0005d540: 6f6d 6269 6e65 2076 616c 7565 7320 6172  ombine values ar
-0005d550: 6f75 6e64 2074 696d 653d 3020 666f 7220  ound time=0 for 
-0005d560: 6265 7474 6572 2073 7461 7469 7374 6963  better statistic
-0005d570: 732e 200d 0a09 0909 5468 6973 2061 7665  s. .....This ave
-0005d580: 7261 6769 6e67 2069 7320 6f6e 6c79 2061  raging is only a
-0005d590: 7070 6c69 6564 2066 6f72 2074 6865 2070  pplied for the p
-0005d5a0: 6c6f 7474 696e 6720 6675 6e63 7469 6f6e  lotting function
-0005d5b0: 2061 6e64 206e 6f74 2066 6f72 2074 6865   and not for the
-0005d5c0: 2066 6974 732e 0d0a 0909 0d0a 0909 7370   fits.........sp
-0005d5d0: 6563 7472 6120 3a20 4e6f 6e65 206f 7220  ectra : None or 
-0005d5e0: 4461 7461 4672 616d 652c 206f 7074 696f  DataFrame, optio
-0005d5f0: 6e61 6c0d 0a09 0909 4966 2061 6e20 4461  nal.....If an Da
-0005d600: 7461 4672 616d 6520 7769 7468 2074 6865  taFrame with the
-0005d610: 2077 6176 656c 656e 6774 6820 6173 2069   wavelength as i
-0005d620: 6e64 6578 2069 7320 7072 6f76 6964 6564  ndex is provided
-0005d630: 2c20 5468 656e 2074 6865 2073 7065 6374  , Then the spect
-0005d640: 7261 206f 6620 6561 6368 2063 6f6c 756d  ra of each colum
-0005d650: 6e0d 0a09 0909 6973 2070 6c6f 7474 6564  n.....is plotted
-0005d660: 2069 6e74 6f20 7468 6520 6469 6666 6572   into the differ
-0005d670: 656e 7469 616c 2073 7065 6374 7261 2031  ential spectra 1
-0005d680: 2d31 2061 6e64 2074 6865 2063 6f6c 756d  -1 and the colum
-0005d690: 6e20 6e61 6d65 7320 6172 6520 7573 6564  n names are used
-0005d6a0: 2069 6e20 7468 6520 6c65 6765 6e64 0d0a   in the legend..
-0005d6b0: 0909 0950 7269 6f72 2073 6361 6c69 6e67  ...Prior scaling
-0005d6c0: 2069 7320 6869 6768 6c79 2073 7567 6765   is highly sugge
-0005d6d0: 7374 6564 2e20 5468 6573 6520 7370 6563  sted. These spec
-0005d6e0: 7472 6120 6172 6520 6e6f 7420 2869 6e20  tra are not (in 
-0005d6f0: 6765 6e65 7261 6c29 2073 6361 6c65 6420  general) scaled 
-0005d700: 7769 7468 2074 6865 200d 0a09 0909 6e6f  with the .....no
-0005d710: 726d 2077 696e 646f 772e 2028 7365 6520  rm window. (see 
-0005d720: 6578 616d 706c 6573 292e 0d0a 0909 0d0a  examples).......
-0005d730: 0909 6461 7461 5f61 6e64 5f66 6974 203a  ..data_and_fit :
-0005d740: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0d   bool, optional.
-0005d750: 0a09 0909 5472 7565 206f 7220 4661 6c73  ....True or Fals
-0005d760: 6520 2844 6566 6175 6c74 292c 2063 686f  e (Default), cho
-0005d770: 6f73 6520 6966 2066 6f72 2074 6865 2046  ose if for the F
-0005d780: 6974 7465 6420 706c 6f74 2074 6865 2072  itted plot the r
-0005d790: 6177 2064 6174 6120 6f66 2074 6865 200d  aw data of the .
-0005d7a0: 0a09 0909 6f74 6865 7220 7072 6f6a 6563  ....other projec
-0005d7b0: 7473 2069 7320 746f 2062 6520 706c 6f74  ts is to be plot
-0005d7c0: 7469 6e67 2069 6e20 6164 6469 7469 6f6e  ting in addition
-0005d7d0: 2074 6f20 7468 6520 6669 7474 6564 206c   to the fitted l
-0005d7e0: 696e 652e 2046 6f72 2046 616c 7365 2028  ine. For False (
-0005d7f0: 4465 6661 756c 7429 0d0a 0909 094f 6e6c  Default).....Onl
-0005d800: 7920 7468 6520 6669 7420 6973 2070 6c6f  y the fit is plo
-0005d810: 7474 6564 2e20 0d0a 0909 0d0a 0909 636d  tted. ........cm
-0005d820: 6170 203a 204e 6f6e 6520 6f72 206d 6174  ap : None or mat
-0005d830: 706c 6f74 6c69 6220 636f 6c6f 7220 6d61  plotlib color ma
-0005d840: 702c 206f 7074 696f 6e61 6c0d 0a09 0909  p, optional.....
-0005d850: 6973 2061 2070 6f77 6572 6675 6c6c 2076  is a powerfull v
-0005d860: 6172 6961 626c 6520 7468 6174 2063 686f  ariable that cho
-0005d870: 6f73 6573 2074 6865 2063 6f6c 6f75 7220  oses the colour 
-0005d880: 6d61 7020 6170 706c 6965 6420 666f 7220  map applied for 
-0005d890: 616c 6c20 706c 6f74 732e 2049 6620 7365  all plots. If se
-0005d8a0: 7420 746f 200d 0a09 0909 4e6f 6e65 2028  t to .....None (
-0005d8b0: 4465 6661 756c 7429 2074 6865 6e20 7468  Default) then th
-0005d8c0: 6520 7365 6c66 2e63 6d61 7020 6973 2075  e self.cmap is u
-0005d8d0: 7365 642e 0d0a 0909 0941 7320 7374 616e  sed......As stan
-0005d8e0: 6461 7264 2049 2075 7365 2074 6865 2063  dard I use the c
-0005d8f0: 6f6c 6f72 206d 6170 2022 6a65 7422 2066  olor map "jet" f
-0005d900: 726f 6d20 6d61 7470 6c6f 746c 6962 2e20  rom matplotlib. 
-0005d910: 5468 6572 6520 6172 6520 6120 7661 7269  There are a vari
-0005d920: 6574 7920 6f66 2063 6f6c 6f72 6d61 7073  ety of colormaps
-0005d930: 200d 0a09 0909 6176 6169 6c61 626c 6520   .....available 
-0005d940: 7468 6174 2061 7265 2076 6572 7920 7573  that are very us
-0005d950: 6566 756c 6c2e 2042 6573 6964 6520 226a  efull. Beside "j
-0005d960: 6574 222c 2022 7669 7269 6469 7322 2069  et", "viridis" i
-0005d970: 7320 6120 676f 6f64 2063 686f 6963 6520  s a good choice 
-0005d980: 6173 2069 7420 6973 2077 656c 6c20 0d0a  as it is well ..
-0005d990: 0909 0976 6973 6962 6c65 2075 6e64 6572  ...visible under
-0005d9a0: 2072 6564 2d67 7265 656e 2062 6c69 6e64   red-green blind
-0005d9b0: 6e65 7373 2e20 4f74 6865 7220 7573 6566  ness. Other usef
-0005d9c0: 756c 206d 6170 7320 6172 6520 2270 7269  ul maps are "pri
-0005d9d0: 736d 2220 666f 7220 6869 6768 2066 6c75  sm" for high flu
-0005d9e0: 6374 7561 7469 6f6e 7320 0d0a 0909 096f  ctuations .....o
-0005d9f0: 7220 6469 7665 7267 696e 6720 636f 6c6f  r diverging colo
-0005da00: 7220 6d61 7073 206c 696b 6520 2273 6569  r maps like "sei
-0005da10: 736d 6963 222e 200d 0a09 0909 5365 6520  smic". .....See 
-0005da20: 6874 7470 733a 2f2f 6d61 7470 6c6f 746c  https://matplotl
-0005da30: 6962 2e6f 7267 2f33 2e31 2e30 2f74 7574  ib.org/3.1.0/tut
-0005da40: 6f72 6961 6c73 2f63 6f6c 6f72 732f 636f  orials/colors/co
-0005da50: 6c6f 726d 6170 732e 6874 6d6c 2066 6f72  lormaps.html for
-0005da60: 2061 2063 6f6d 7072 6568 656e 7369 7665   a comprehensive
-0005da70: 200d 0a09 0909 7365 6c65 6374 696f 6e2e   .....selection.
-0005da80: 2049 6e20 7468 6520 636f 6465 2074 6865   In the code the
-0005da90: 2063 6f6c 6f72 6d61 7073 2061 7265 2069   colormaps are i
-0005daa0: 6d70 6f72 7465 6420 736f 2069 6620 706c  mported so if pl
-0005dab0: 6f74 5f66 756e 6320 6973 2069 6d70 6f72  ot_func is impor
-0005dac0: 7465 6420 6173 2070 6620 7468 656e 200d  ted as pf then .
-0005dad0: 0a09 0909 7365 6c66 2e63 6d61 703d 7066  ....self.cmap=pf
-0005dae0: 2e63 6d2e 7669 7269 6469 7320 7365 7473  .cm.viridis sets
-0005daf0: 2076 6972 6964 6973 2061 7320 7468 6520   viridis as the 
-0005db00: 6d61 7020 746f 2075 7365 2e20 496e 7465  map to use. Inte
-0005db10: 726e 616c 6c79 2074 6865 2063 6f6c 6f72  rnally the color
-0005db20: 7320 6172 6520 6368 6f73 656e 200d 0a09  s are chosen ...
-0005db30: 0909 7769 7468 2074 6865 2022 636f 6c6d  ..with the "colm
-0005db40: 2220 6675 6e63 7469 6f6e 2e20 5468 6520  " function. The 
-0005db50: 3264 2070 6c6f 7473 2072 6571 7569 7265  2d plots require
-0005db60: 2061 2063 6f6e 7469 6e75 6f75 7320 636f   a continuous co
-0005db70: 6c6f 7220 6d61 7020 736f 2069 6620 736f  lor map so if so
-0005db80: 6d65 7468 696e 6720 0d0a 0909 0965 6c73  mething .....els
-0005db90: 6520 6973 2067 6976 6520 3264 2070 6c6f  e is give 2d plo
-0005dba0: 7473 2061 7265 2073 686f 776e 2061 7574  ts are shown aut
-0005dbb0: 6f6d 6174 6963 616c 6c79 2077 6974 6820  omatically with 
-0005dbc0: 226a 6574 222e 2046 6f72 2061 6c6c 206f  "jet". For all o
-0005dbd0: 6620 7468 6520 3164 2070 6c6f 7473 2068  f the 1d plots h
-0005dbe0: 6f77 6576 6572 200d 0a09 0909 4920 6669  owever .....I fi
-0005dbf0: 7273 7420 7365 6c65 6374 2061 206e 756d  rst select a num
-0005dc00: 6265 7220 6f66 2063 6f6c 6f72 7320 6265  ber of colors be
-0005dc10: 666f 7265 2065 6163 6820 706c 6f74 2e20  fore each plot. 
-0005dc20: 4966 2063 6d61 7020 6973 2061 2063 6f6e  If cmap is a con
-0005dc30: 7469 6e6f 7573 206d 6170 2074 6865 6e20  tinous map then 
-0005dc40: 7468 6573 650d 0a09 0909 6172 6520 7361  these.....are sa
-0005dc50: 6d70 6c65 6420 6576 656e 6c79 206f 7665  mpled evenly ove
-0005dc60: 7220 7468 6520 636f 6c6f 7572 6d61 702e  r the colourmap.
-0005dc70: 204d 616e 7561 6c20 6974 6572 6162 6c65   Manual iterable
-0005dc80: 7320 6f66 2063 6f6c 6f75 7273 200d 0a09  s of colours ...
-0005dc90: 0909 636d 6170 3d5b 2831 2c30 2c30 292c  ..cmap=[(1,0,0),
-0005dca0: 2830 2c31 2c30 292c 2830 2c30 2c31 292c  (0,1,0),(0,0,1),
-0005dcb0: 2e2e 2e5d 2061 7265 2061 6c73 6f20 6163  ...] are also ac
-0005dcc0: 6365 7074 6564 2c20 6173 2061 7265 2076  cepted, as are v
-0005dcd0: 6563 746f 7273 206f 7220 6461 7461 6672  ectors or datafr
-0005dce0: 616d 6573 2074 6861 7420 0d0a 0909 0963  ames that .....c
-0005dcf0: 6f6e 7461 696e 2061 7320 726f 7773 2074  ontain as rows t
-0005dd00: 6865 2063 6f6c 6f72 732e 2054 6865 7265  he colors. There
-0005dd10: 206d 7573 7420 6265 206f 6620 636f 7572   must be of cour
-0005dd20: 7365 2073 7566 6669 6369 656e 7420 636f  se sufficient co
-0005dd30: 6c6f 7273 2070 7265 7365 6e74 2066 6f72  lors present for
-0005dd40: 200d 0a09 0909 7468 6520 6e75 6d62 6572   .....the number
-0005dd50: 7320 6f66 206c 696e 6573 2074 6861 7420  s of lines that 
-0005dd60: 7769 6c6c 2062 6520 706c 6f74 7465 642e  will be plotted.
-0005dd70: 2053 6f20 4920 7265 636f 6d6d 656e 6420   So I recommend 
-0005dd80: 746f 2070 726f 7669 6465 2061 7420 6c65  to provide at le
-0005dd90: 6173 7420 3130 2063 6f6c 6f75 7273 200d  ast 10 colours .
-0005dda0: 0a09 0909 2865 2e67 2e7e 796f 7572 2075  ....(e.g.~your u
-0005ddb0: 6e69 7665 7273 6974 7920 636f 6c6f 7273  niversity colors
-0005ddc0: 292e 2063 6f6c 6f75 7273 2061 7265 2061  ). colours are a
-0005ddd0: 6c77 6179 7320 6769 7665 6e20 6173 2061  lways given as a
-0005dde0: 2c20 6c69 7374 206f 7220 7475 706c 6520  , list or tuple 
-0005ddf0: 7769 7468 2052 4741 206f 7220 5247 4241  with RGA or RGBA
-0005de00: 0d0a 0909 0928 7769 7468 2074 6865 206c  .....(with the l
-0005de10: 6173 7420 4120 6265 6569 6e67 2074 6865  ast A beeing the
-0005de20: 2041 6c70 6861 3d74 7261 6e73 7061 7265   Alpha=transpare
-0005de30: 6e63 792e 2041 6c6c 206e 756d 6265 7273  ncy. All numbers
-0005de40: 2061 7265 2062 6574 7765 656e 2030 2061   are between 0 a
-0005de50: 6e64 2031 2e20 0d0a 0909 0949 6620 6120  nd 1. .....If a 
-0005de60: 6c69 7374 2f76 6563 746f 722f 4461 7461  list/vector/Data
-0005de70: 4672 616d 6520 6973 2067 6976 656e 2066  Frame is given f
-0005de80: 6f72 2074 6865 2063 6f6c 6f75 7273 2074  or the colours t
-0005de90: 6865 7920 7769 6c6c 2062 6520 7573 6564  hey will be used
-0005dea0: 2069 6e20 7468 6520 6f72 6465 7220 7072   in the order pr
-0005deb0: 6f76 6964 6564 2e0d 0a09 0970 6c6f 745f  ovided.....plot_
-0005dec0: 7365 636f 6e64 5f61 735f 656e 6572 6779  second_as_energy
-0005ded0: 203a 2062 6f6f 6c2c 206f 7074 696f 6e61   : bool, optiona
-0005dee0: 6c0d 0a09 0909 466f 7220 2844 6566 6175  l.....For (Defau
-0005def0: 6c74 2920 5472 7565 2061 2073 6563 6f6e  lt) True a secon
-0005df00: 6420 782d 6178 6973 2069 7320 706c 6f74  d x-axis is plot
-0005df10: 7465 6420 2077 6974 6820 2265 5622 2061  ted  with "eV" a
-0005df20: 7320 756e 6974 0d0a 0d0a 0909 7072 696e  s unit......prin
-0005df30: 745f 636c 6963 6b5f 706f 7369 7469 6f6e  t_click_position
-0005df40: 203a 2062 6f6f 6c2c 206f 7074 696f 6e61   : bool, optiona
-0005df50: 6c0d 0a09 0909 6966 2054 7275 6520 7468  l.....if True th
-0005df60: 656e 2074 6865 2063 6c69 636b 2070 6f73  en the click pos
-0005df70: 6974 696f 6e20 6973 2070 7269 6e74 6564  ition is printed
-0005df80: 2066 6f72 2074 6865 2073 7065 6374 7261   for the spectra
-0005df90: 6c20 706c 6f74 7320 0d0a 0d0a 0909 4578  l plots ......Ex
-0005dfa0: 616d 706c 6573 0d0a 0909 2d2d 2d2d 2d2d  amples....------
-0005dfb0: 2d2d 2d2d 0d0a 0909 0d0a 0909 3e3e 3e20  ----........>>> 
-0005dfc0: 696d 706f 7274 2070 6c6f 745f 6675 6e63  import plot_func
-0005dfd0: 2061 7320 7066 0d0a 0909 3e3e 3e20 7461   as pf....>>> ta
-0005dfe0: 203d 2070 662e 5441 2822 7465 7374 312e   = pf.TA("test1.
-0005dff0: 6864 6635 2229 2023 6f70 656e 2074 6865  hdf5") #open the
-0005e000: 206f 7269 6769 6e61 6c20 7072 6f6a 6563   original projec
-0005e010: 740d 0a09 090d 0a09 094e 6f77 206f 7065  t........Now ope
-0005e020: 6e20 6120 6275 6e63 6820 6f66 206f 7468  n a bunch of oth
-0005e030: 6572 2070 6f72 6a65 6374 7320 746f 2063  er porjects to c
-0005e040: 6f6d 6172 6520 6167 6169 6e73 740d 0a09  omare against...
-0005e050: 090d 0a09 093e 3e3e 206f 7468 6572 5f70  .....>>> other_p
-0005e060: 726f 6a65 6374 7320 3d20 7066 2e47 5549  rojects = pf.GUI
-0005e070: 5f6f 7065 6e28 7072 6f6a 6563 745f 6c69  _open(project_li
-0005e080: 7374 203d 205b 2266 696c 6531 2e53 4941  st = ["file1.SIA
-0005e090: 222c 2022 6669 6c65 322e 5349 4122 5d29  ", "file2.SIA"])
-0005e0a0: 0d0a 0909 0d0a 0909 5479 7069 6361 6c20  ........Typical 
-0005e0b0: 7573 6520 6973 2063 6f6d 7061 7265 2074  use is compare t
-0005e0c0: 6865 2072 6177 2064 6174 6120 7769 7468  he raw data with
-0005e0d0: 6f75 7420 6e6f 726d 616c 697a 6174 696f  out normalizatio
-0005e0e0: 6e20 6174 2031 7073 2061 6e64 2036 7073  n at 1ps and 6ps
-0005e0f0: 2e0d 0a09 090d 0a09 093e 3e3e 2074 612e  .........>>> ta.
-0005e100: 436f 6d70 6172 655f 6174 5f74 696d 6528  Compare_at_time(
-0005e110: 7265 6c5f 7469 6d65 203d 205b 312c 365d  rel_time = [1,6]
-0005e120: 2c20 6f74 6865 7273 203d 206f 7468 6572  , others = other
-0005e130: 5f70 726f 6a65 6374 290d 0a09 090d 0a09  _project).......
-0005e140: 0943 6f6d 7061 7265 2074 6865 2066 6974  .Compare the fit
-0005e150: 2077 6974 6870 7574 206e 6f72 6d61 6c69   withput normali
-0005e160: 7a61 7469 6f6e 2061 7420 3170 7320 616e  zation at 1ps an
-0005e170: 6420 3670 732e 0d0a 0909 0d0a 0909 3e3e  d 6ps.........>>
-0005e180: 3e20 7461 2e43 6f6d 7061 7265 5f61 745f  > ta.Compare_at_
-0005e190: 7469 6d65 2872 656c 5f74 696d 6520 3d20  time(rel_time = 
-0005e1a0: 5b31 2c36 5d2c 206f 7468 6572 7320 3d20  [1,6], others = 
-0005e1b0: 6f74 6865 725f 7072 6f6a 6563 742c 2066  other_project, f
-0005e1c0: 6974 7465 6420 3d20 5472 7565 290d 0a09  itted = True)...
-0005e1d0: 090d 0a09 0943 6f6d 7061 7265 2077 6974  .....Compare wit
-0005e1e0: 6820 6e6f 726d 616c 697a 6174 696f 6e20  h normalization 
-0005e1f0: 7769 6e64 6f77 2062 6574 7765 656e 2031  window between 1
-0005e200: 7073 2061 6e64 2032 7073 2061 6e64 2034  ps and 2ps and 4
-0005e210: 3030 6e6d 2061 6e64 2034 3530 6e6d 2e0d  00nm and 450nm..
-0005e220: 0a09 090d 0a09 093e 3e3e 206e 6f72 6d5f  .......>>> norm_
-0005e230: 7769 6e64 6f77 3d5b 312c 322c 3430 302c  window=[1,2,400,
-0005e240: 3435 305d 0d0a 0909 3e3e 3e20 7461 2e43  450]....>>> ta.C
-0005e250: 6f6d 7061 7265 5f61 745f 7469 6d65 2872  ompare_at_time(r
-0005e260: 656c 5f74 696d 6520 3d20 5b31 2c36 5d2c  el_time = [1,6],
-0005e270: 206f 7468 6572 7320 3d20 6f74 6865 725f   others = other_
-0005e280: 7072 6f6a 6563 742c 206e 6f72 6d5f 7769  project, norm_wi
-0005e290: 6e64 6f77 203d 206e 6f72 6d5f 7769 6e64  ndow = norm_wind
-0005e2a0: 6f77 290d 0a09 090d 0a09 0943 6f6d 7061  ow)........Compa
-0005e2b0: 7265 2074 6865 2073 7065 6374 7275 6d20  re the spectrum 
-0005e2c0: 6174 2031 7073 2061 6e64 2036 7073 2077  at 1ps and 6ps w
-0005e2d0: 6974 6820 616e 2065 7874 6572 6e61 6c20  ith an external 
-0005e2e0: 7370 6563 7472 756d 2e0d 0a09 090d 0a09  spectrum........
-0005e2f0: 093e 3e3e 2065 7874 5f73 7065 6320 3d20  .>>> ext_spec = 
-0005e300: 7064 2e72 6561 645f 6373 7628 2241 7363  pd.read_csv("Asc
-0005e310: 6969 5f73 7065 6374 7275 6d2e 6461 7422  ii_spectrum.dat"
-0005e320: 2c20 7365 7020 3d20 222c 2229 0d0a 0909  , sep = ",")....
-0005e330: 3e3e 3e20 7461 2e43 6f6d 7061 7265 5f61  >>> ta.Compare_a
-0005e340: 745f 7469 6d65 2872 656c 5f74 696d 6520  t_time(rel_time 
-0005e350: 3d20 5b31 2c36 5d2c 2073 7065 6374 7261  = [1,6], spectra
-0005e360: 203d 2065 7874 5f73 7065 6329 0d0a 0d0a   = ext_spec)....
-0005e370: 0909 5573 6520 6578 616d 706c 6520 2d20  ..Use example - 
-0005e380: 204f 6674 656e 2074 6865 7265 2061 7265   Often there are
-0005e390: 2061 206c 6f74 206f 6620 6469 6666 6572   a lot of differ
-0005e3a0: 656e 7420 6d65 6173 7572 656d 656e 7473  ent measurements
-0005e3b0: 2074 6f20 0d0a 0909 636f 6d70 6172 6520   to ....compare 
-0005e3c0: 6174 206d 756c 7469 706c 6520 7469 6d65  at multiple time
-0005e3d0: 2e20 5468 6520 6e6f 726d 6c69 7a61 7469  . The normlizati
-0005e3e0: 6f6e 2069 7320 7065 7266 6f72 6d65 6420  on is performed 
-0005e3f0: 6174 2074 6865 2067 726f 756e 6420 7374  at the ground st
-0005e400: 6174 6520 626c 6561 6368 0d0a 0909 3436  ate bleach....46
-0005e410: 3020 6e6d 2061 6e64 2065 6172 6c79 2069  0 nm and early i
-0005e420: 6e20 7469 6d65 2e20 5468 656e 2069 7420  n time. Then it 
-0005e430: 6973 2062 6574 7465 7220 746f 206d 616b  is better to mak
-0005e440: 6520 6120 6e65 7720 706c 6f74 2066 6f72  e a new plot for
-0005e450: 2065 6163 6820 0d0a 0909 7469 6d65 706f   each ....timepo
-0005e460: 696e 742e 2054 6865 206e 6f72 6d61 6c69  int. The normali
-0005e470: 7a61 7469 6f6e 2077 696e 646f 7720 7374  zation window st
-0005e480: 6179 7320 6669 7865 642e 0d0a 0909 0d0a  ays fixed.......
-0005e490: 0909 3e3e 3e20 706c 742e 636c 6f73 6528  ..>>> plt.close(
-0005e4a0: 2261 6c6c 2229 2023 6d61 6b65 2073 6f6d  "all") #make som
-0005e4b0: 6520 7370 6163 650d 0a09 093e 3e3e 206e  e space....>>> n
-0005e4c0: 6f72 6d5f 7769 6e64 6f77 3d5b 302e 332c  orm_window=[0.3,
-0005e4d0: 302e 352c 3435 302c 3437 305d 2023 6465  0.5,450,470] #de
-0005e4e0: 6669 6e65 2077 696e 646f 7720 696e 2067  fine window in g
-0005e4f0: 726f 756e 6420 7374 6174 6520 626c 6561  round state blea
-0005e500: 6368 0d0a 0909 3e3e 3e20 666f 7220 7420  ch....>>> for t 
-0005e510: 696e 205b 302e 332c 302e 352c 312c 332c  in [0.3,0.5,1,3,
-0005e520: 3130 2c33 305d 3a20 2369 7465 7261 7465  10,30]: #iterate
-0005e530: 206f 7665 7220 7468 6520 7761 7665 6c65   over the wavele
-0005e540: 6e67 7468 200d 0a09 093e 3e3e 2009 7461  ngth ....>>> .ta
-0005e550: 2e43 6f6d 7061 7265 5f61 745f 7469 6d65  .Compare_at_time
-0005e560: 2872 656c 5f74 696d 6520 3d20 742c 206f  (rel_time = t, o
-0005e570: 7468 6572 7320 3d20 6f74 6865 725f 7072  thers = other_pr
-0005e580: 6f6a 6563 742c 206e 6f72 6d5f 7769 6e64  oject, norm_wind
-0005e590: 6f77 203d 206e 6f72 6d5f 7769 6e64 6f77  ow = norm_window
-0005e5a0: 290d 0a09 090d 0a09 0927 2727 0d0a 0909  )........'''....
-0005e5b0: 0d0a 0909 6966 2073 656c 662e 7361 7665  ....if self.save
-0005e5c0: 5f66 6967 7572 6573 5f74 6f5f 666f 6c64  _figures_to_fold
-0005e5d0: 6572 3a73 656c 662e 6669 6775 7265 5f70  er:self.figure_p
-0005e5e0: 6174 683d 6368 6563 6b5f 666f 6c64 6572  ath=check_folder
-0005e5f0: 2870 6174 683d 2772 6573 756c 745f 6669  (path='result_fi
-0005e600: 6775 7265 7327 2c63 7572 7265 6e74 5f70  gures',current_p
-0005e610: 6174 683d 7365 6c66 2e70 6174 6829 0d0a  ath=self.path)..
-0005e620: 0909 6966 2074 696d 655f 7769 6474 685f  ..if time_width_
-0005e630: 7065 7263 656e 7420 6973 204e 6f6e 653a  percent is None:
-0005e640: 7469 6d65 5f77 6964 7468 5f70 6572 6365  time_width_perce
-0005e650: 6e74 3d73 656c 662e 7469 6d65 5f77 6964  nt=self.time_wid
-0005e660: 7468 5f70 6572 6365 6e74 0d0a 0909 6966  th_percent....if
-0005e670: 2072 656c 5f74 696d 6520 6973 204e 6f6e   rel_time is Non
-0005e680: 653a 7265 6c5f 7469 6d65 3d73 656c 662e  e:rel_time=self.
-0005e690: 7265 6c5f 7469 6d65 0d0a 0909 6966 206f  rel_time....if o
-0005e6a0: 7468 6572 2069 7320 6e6f 7420 4e6f 6e65  ther is not None
-0005e6b0: 3a0d 0a09 0909 6966 206e 6f74 2068 6173  :.....if not has
-0005e6c0: 6174 7472 286f 7468 6572 2c27 5f5f 6974  attr(other,'__it
-0005e6d0: 6572 5f5f 2729 3a6f 7468 6572 3d5b 6f74  er__'):other=[ot
-0005e6e0: 6865 725d 0d0a 0909 6966 2072 656c 5f74  her]....if rel_t
-0005e6f0: 696d 6520 6973 206e 6f74 204e 6f6e 653a  ime is not None:
-0005e700: 0d0a 0909 0969 6620 6e6f 7420 6861 7361  .....if not hasa
-0005e710: 7474 7228 7265 6c5f 7469 6d65 2c27 5f5f  ttr(rel_time,'__
-0005e720: 6974 6572 5f5f 2729 3a72 656c 5f74 696d  iter__'):rel_tim
-0005e730: 653d 5b72 656c 5f74 696d 655d 0909 0d0a  e=[rel_time]....
-0005e740: 0909 656c 7365 3a0d 0a09 0909 7265 6c5f  ..else:.....rel_
-0005e750: 7469 6d65 3d5b 315d 0d0a 0909 6966 2063  time=[1]....if c
-0005e760: 6d61 7020 6973 204e 6f6e 653a 636d 6170  map is None:cmap
-0005e770: 3d73 656c 662e 636d 6170 0d0a 0909 6966  =self.cmap....if
-0005e780: 2066 6974 7465 643a 0d0a 0909 0974 7279   fitted:.....try
-0005e790: 3a0d 0a09 0909 0972 653d 7365 6c66 2e72  :......re=self.r
-0005e7a0: 650d 0a09 0909 6578 6365 7074 3a0d 0a09  e.....except:...
-0005e7b0: 0909 0970 7269 6e74 2822 4e6f 2066 6974  ...print("No fit
-0005e7c0: 7465 6420 7265 7375 6c74 7320 7072 6573  ted results pres
-0005e7d0: 656e 7422 290d 0a09 0909 0972 6574 7572  ent")......retur
-0005e7e0: 6e20 4661 6c73 650d 0a09 0909 6966 206e  n False.....if n
-0005e7f0: 6f72 6d5f 7769 6e64 6f77 2069 7320 6e6f  orm_window is no
-0005e800: 7420 4e6f 6e65 3a0d 0a09 0909 0972 6566  t None:......ref
-0005e810: 5f73 6361 6c65 3d72 655b 2741 275d 2e6c  _scale=re['A'].l
-0005e820: 6f63 5b6e 6f72 6d5f 7769 6e64 6f77 5b30  oc[norm_window[0
-0005e830: 5d3a 6e6f 726d 5f77 696e 646f 775b 315d  ]:norm_window[1]
-0005e840: 2c6e 6f72 6d5f 7769 6e64 6f77 5b32 5d3a  ,norm_window[2]:
-0005e850: 6e6f 726d 5f77 696e 646f 775b 335d 5d2e  norm_window[3]].
-0005e860: 6d65 616e 2829 2e6d 6561 6e28 290d 0a09  mean().mean()...
-0005e870: 0909 6669 672c 6178 3d70 6c74 2e73 7562  ..fig,ax=plt.sub
-0005e880: 706c 6f74 7328 6669 6773 697a 653d 2831  plots(figsize=(1
-0005e890: 302c 3629 2c64 7069 3d31 3030 290d 0a09  0,6),dpi=100)...
-0005e8a0: 0909 6f62 6a65 6374 733d 6c65 6e28 7265  ..objects=len(re
-0005e8b0: 6c5f 7469 6d65 292a 2831 2b6c 656e 286f  l_time)*(1+len(o
-0005e8c0: 7468 6572 2929 0d0a 0909 0963 6f6c 6f72  ther)).....color
-0005e8d0: 733d 636f 6c6d 2863 6d61 703d 636d 6170  s=colm(cmap=cmap
-0005e8e0: 2c6b 3d72 616e 6765 286f 626a 6563 7473  ,k=range(objects
-0005e8f0: 2929 0d0a 0909 095f 3d70 6c6f 745f 7469  ))....._=plot_ti
-0005e900: 6d65 2872 655b 2741 275d 2c20 6178 203d  me(re['A'], ax =
-0005e910: 2061 782c 2072 656c 5f74 696d 6520 3d20   ax, rel_time = 
-0005e920: 7265 6c5f 7469 6d65 2c20 7469 6d65 5f77  rel_time, time_w
-0005e930: 6964 7468 5f70 6572 6365 6e74 203d 2074  idth_percent = t
-0005e940: 696d 655f 7769 6474 685f 7065 7263 656e  ime_width_percen
-0005e950: 742c 200d 0a09 0909 0909 0962 6173 6575  t, ........baseu
-0005e960: 6e69 7420 3d20 7365 6c66 2e62 6173 6575  nit = self.baseu
-0005e970: 6e69 742c 206c 696e 6573 5f61 7265 203d  nit, lines_are =
-0005e980: 2027 6461 7461 272c 2063 6d61 7020 3d20   'data', cmap = 
-0005e990: 636f 6c6f 7273 5b3a 6c65 6e28 7265 6c5f  colors[:len(rel_
-0005e9a0: 7469 6d65 295d 2c20 7469 746c 6520 3d20  time)], title = 
-0005e9b0: 2727 2c20 6c69 6e65 7769 6474 6820 3d20  '', linewidth = 
-0005e9c0: 6c69 6e65 7769 6474 682c 2073 7562 706c  linewidth, subpl
-0005e9d0: 6f74 3d20 5472 7565 2c20 7363 6174 7465  ot= True, scatte
-0005e9e0: 7263 7574 203d 2073 656c 662e 7363 6174  rcut = self.scat
-0005e9f0: 7465 7263 7574 290d 0a09 0909 5f3d 706c  tercut)....._=pl
-0005ea00: 6f74 5f74 696d 6528 7265 5b27 4143 275d  ot_time(re['AC']
-0005ea10: 2c20 6178 203d 2061 782c 2072 656c 5f74  , ax = ax, rel_t
-0005ea20: 696d 6520 3d20 7265 6c5f 7469 6d65 2c20  ime = rel_time, 
-0005ea30: 7469 6d65 5f77 6964 7468 5f70 6572 6365  time_width_perce
-0005ea40: 6e74 203d 2074 696d 655f 7769 6474 685f  nt = time_width_
-0005ea50: 7065 7263 656e 742c 200d 0a09 0909 0909  percent, .......
-0005ea60: 0962 6173 6575 6e69 7420 3d20 7365 6c66  .baseunit = self
-0005ea70: 2e62 6173 6575 6e69 742c 206c 696e 6573  .baseunit, lines
-0005ea80: 5f61 7265 203d 2027 6669 7474 6564 272c  _are = 'fitted',
-0005ea90: 2063 6d61 7020 3d20 636f 6c6f 7273 5b3a   cmap = colors[:
-0005eaa0: 6c65 6e28 7265 6c5f 7469 6d65 295d 2c20  len(rel_time)], 
-0005eab0: 7469 746c 6520 3d20 2727 2c20 7375 6270  title = '', subp
-0005eac0: 6c6f 7420 3d20 4661 6c73 652c 206c 696e  lot = False, lin
-0005ead0: 6577 6964 7468 203d 206c 696e 6577 6964  ewidth = linewid
-0005eae0: 7468 2c20 7363 6174 7465 7263 7574 203d  th, scattercut =
-0005eaf0: 2073 656c 662e 7363 6174 7465 7263 7574   self.scattercut
-0005eb00: 290d 0a09 0909 6861 6e64 6c65 732c 206c  ).....handles, l
-0005eb10: 6162 656c 733d 6178 2e67 6574 5f6c 6567  abels=ax.get_leg
-0005eb20: 656e 645f 6861 6e64 6c65 735f 6c61 6265  end_handles_labe
-0005eb30: 6c73 2829 0d0a 0909 096c 6162 3d5b 2725  ls().....lab=['%
-0005eb40: 6720 2573 2725 2865 6e74 2c73 656c 662e  g %s'%(ent,self.
-0005eb50: 6261 7365 756e 6974 2920 2b20 275f 2720  baseunit) + '_' 
-0005eb60: 2b20 7374 7228 7365 6c66 2e66 696c 656e  + str(self.filen
-0005eb70: 616d 6529 2066 6f72 2065 6e74 2069 6e20  ame) for ent in 
-0005eb80: 7265 6c5f 7469 6d65 5d0d 0a09 0909 6861  rel_time].....ha
-0005eb90: 6e3d 6861 6e64 6c65 735b 3a6c 656e 2872  n=handles[:len(r
-0005eba0: 656c 5f74 696d 6529 2a32 5d0d 0a09 0909  el_time)*2].....
+000584d0: 6966 206e 6f74 2068 6173 6174 7472 2873  if not hasattr(s
+000584e0: 6176 6574 7970 652c 225f 5f69 7465 725f  avetype,"__iter_
+000584f0: 5f22 293a 7361 7665 7479 7065 3d5b 7361  _"):savetype=[sa
+00058500: 7665 7479 7065 5d0d 0a09 0972 6177 5f6e  vetype]....raw_n
+00058510: 616d 6573 3d5b 224d 4154 222c 2253 454c  ames=["MAT","SEL
+00058520: 222c 2253 5045 4b22 2c22 5356 4422 5d0d  ","SPEK","SVD"].
+00058530: 0a09 0972 6177 5f6e 616d 6573 3d5b 6368  ...raw_names=[ch
+00058540: 6563 6b5f 666f 6c64 6572 2863 7572 7265  eck_folder(curre
+00058550: 6e74 5f70 6174 683d 7365 6c66 2e70 6174  nt_path=self.pat
+00058560: 682c 2070 6174 683d 7061 7468 2c20 6669  h, path=path, fi
+00058570: 6c65 6e61 6d65 3d73 656c 662e 6669 6c65  lename=self.file
+00058580: 6e61 6d65 2e73 706c 6974 2827 2e27 295b  name.split('.')[
+00058590: 305d 202b 2022 5f52 4157 5f22 2b73 7472  0] + "_RAW_"+str
+000585a0: 2861 2920 2b22 2e70 6e67 2229 2066 6f72  (a) +".png") for
+000585b0: 2061 2069 6e20 7261 775f 6e61 6d65 735d   a in raw_names]
+000585c0: 0d0a 0909 6669 745f 6e61 6d65 733d 5b22  ....fit_names=["
+000585d0: 4649 475f 4d41 5422 2c22 5350 4543 222c  FIG_MAT","SPEC",
+000585e0: 2253 454c 222c 2253 554d 222c 2244 4143  "SEL","SUM","DAC
+000585f0: 225d 0d0a 0909 6669 745f 6e61 6d65 733d  "]....fit_names=
+00058600: 5b63 6865 636b 5f66 6f6c 6465 7228 6375  [check_folder(cu
+00058610: 7272 656e 745f 7061 7468 3d73 656c 662e  rrent_path=self.
+00058620: 7061 7468 2c20 7061 7468 3d70 6174 682c  path, path=path,
+00058630: 2066 696c 656e 616d 653d 7365 6c66 2e66   filename=self.f
+00058640: 696c 656e 616d 652e 7370 6c69 7428 272e  ilename.split('.
+00058650: 2729 5b30 5d20 2b20 225f 2220 2b73 7472  ')[0] + "_" +str
+00058660: 2861 2920 2b22 2e70 6e67 2229 2066 6f72  (a) +".png") for
+00058670: 2061 2069 6e20 6669 745f 6e61 6d65 735d   a in fit_names]
+00058680: 0d0a 0909 706c 742e 636c 6f73 6528 2761  ....plt.close('a
+00058690: 6c6c 2729 0d0a 0909 6f72 6967 696e 3d73  ll')....origin=s
+000586a0: 656c 662e 7361 7665 5f66 6967 7572 6573  elf.save_figures
+000586b0: 5f74 6f5f 666f 6c64 6572 0d0a 0909 6966  _to_folder....if
+000586c0: 2066 696c 656e 616d 6520 6973 204e 6f6e   filename is Non
+000586d0: 653a 0d0a 0909 0966 696c 656e 616d 653d  e:.....filename=
+000586e0: 7365 6c66 2e66 696c 656e 616d 650d 0a09  self.filename...
+000586f0: 0909 6669 6c65 6e61 6d65 3d66 696c 656e  ..filename=filen
+00058700: 616d 652e 7370 6c69 7428 272e 2729 5b30  ame.split('.')[0
+00058710: 5d0d 0a09 0969 6620 7361 7665 5f52 4157  ]....if save_RAW
+00058720: 3a0d 0a09 0909 7365 6c66 2e73 6176 655f  :.....self.save_
+00058730: 6669 6775 7265 735f 746f 5f66 6f6c 6465  figures_to_folde
+00058740: 723d 5472 7565 0d0a 0909 0973 656c 662e  r=True.....self.
+00058750: 506c 6f74 5f52 4157 2873 6176 6574 7970  Plot_RAW(savetyp
+00058760: 6520 3d20 2770 6e67 272c 2073 6361 6c65  e = 'png', scale
+00058770: 5f74 7970 6520 3d20 7363 616c 655f 7479  _type = scale_ty
+00058780: 7065 2c20 7469 746c 6520 3d20 7469 746c  pe, title = titl
+00058790: 652c 2063 6d61 7020 3d20 636d 6170 2c20  e, cmap = cmap, 
+000587a0: 7061 7468 203d 2070 6174 6829 090d 0a09  path = path)....
+000587b0: 0909 706c 742e 636c 6f73 6528 2761 6c6c  ..plt.close('all
+000587c0: 2729 0d0a 0909 6966 2073 6176 655f 4669  ')....if save_Fi
+000587d0: 743a 0d0a 0909 0974 7279 3a0d 0a09 0909  t:.....try:.....
+000587e0: 0973 656c 662e 7361 7665 5f66 6967 7572  .self.save_figur
+000587f0: 6573 5f74 6f5f 666f 6c64 6572 3d54 7275  es_to_folder=Tru
+00058800: 650d 0a09 0909 0973 656c 662e 506c 6f74  e......self.Plot
+00058810: 5f66 6974 5f6f 7574 7075 7428 7361 7665  _fit_output(save
+00058820: 7479 7065 203d 2027 706e 6727 2c20 7363  type = 'png', sc
+00058830: 616c 655f 7479 7065 203d 2073 6361 6c65  ale_type = scale
+00058840: 5f74 7970 652c 2074 6974 6c65 203d 2074  _type, title = t
+00058850: 6974 6c65 2c20 7061 7463 6865 7320 3d20  itle, patches = 
+00058860: 7061 7463 6865 732c 2063 6d61 7020 3d20  patches, cmap = 
+00058870: 636d 6170 202c 2070 6174 6820 3d20 7061  cmap , path = pa
+00058880: 7468 290d 0a09 0909 0970 6c74 2e63 6c6f  th)......plt.clo
+00058890: 7365 2827 616c 6c27 290d 0a09 0909 6578  se('all').....ex
+000588a0: 6365 7074 3a0d 0a09 0909 0973 6176 655f  cept:......save_
+000588b0: 4669 7420 3d20 4661 6c73 650d 0a09 0909  Fit = False.....
+000588c0: 0970 7269 6e74 2827 7275 6e20 696e 746f  .print('run into
+000588d0: 2070 726f 626c 656d 7320 7769 7468 2061   problems with a
+000588e0: 6464 696e 6720 7468 6520 6669 7420 7265  dding the fit re
+000588f0: 7375 6c74 732e 2048 6176 6520 796f 7520  sults. Have you 
+00058900: 6669 7474 6564 2073 6f6d 6574 6869 6e67  fitted something
+00058910: 3f27 290d 0a09 0909 7472 793a 0d0a 0909  ?').....try:....
+00058920: 0909 5265 7375 6c74 5f73 7472 696e 673d  ..Result_string=
+00058930: 275c 6e46 6974 2052 6573 756c 7473 3a5c  '\nFit Results:\
+00058940: 6e27 0d0a 0909 0909 6966 2069 7369 6e73  n'......if isins
+00058950: 7461 6e63 6528 7365 6c66 2e6d 6f64 2c74  tance(self.mod,t
+00058960: 7970 6528 2768 656c 6c6f 2729 293a 0d0a  ype('hello')):..
+00058970: 0909 0909 0952 6573 756c 745f 7374 7269  .....Result_stri
+00058980: 6e67 2b3d 274d 6f64 656c 2055 7365 643a  ng+='Model Used:
+00058990: 2025 735c 6e5c 6e27 2573 656c 662e 6d6f   %s\n\n'%self.mo
+000589a0: 640d 0a09 0909 0965 6c73 653a 0d0a 0909  d......else:....
+000589b0: 0909 0952 6573 756c 745f 7374 7269 6e67  ...Result_string
+000589c0: 2b3d 274d 6f64 656c 2055 7365 643a 2045  +='Model Used: E
+000589d0: 7874 6572 6e61 6c20 6675 6e63 7469 6f6e  xternal function
+000589e0: 5c6e 5c6e 270d 0a09 0909 0969 6620 7365  \n\n'......if se
+000589f0: 6c66 2e69 676e 6f72 655f 7469 6d65 5f72  lf.ignore_time_r
+00058a00: 6567 696f 6e20 6973 206e 6f74 204e 6f6e  egion is not Non
+00058a10: 653a 0d0a 0909 0909 0952 6573 756c 745f  e:.......Result_
+00058a20: 7374 7269 6e67 2b3d 2774 6865 2074 696d  string+='the tim
+00058a30: 6520 6265 7477 6565 6e20 252e 3366 2025  e between %.3f %
+00058a40: 7320 616e 6420 252e 3366 2025 7320 5c6e  s and %.3f %s \n
+00058a50: 2077 6173 2065 7863 6c75 6465 6420 6672   was excluded fr
+00058a60: 6f6d 2074 6865 206f 7074 696d 697a 6174  om the optimizat
+00058a70: 696f 6e5c 6e27 2528 7365 6c66 2e69 676e  ion\n'%(self.ign
+00058a80: 6f72 655f 7469 6d65 5f72 6567 696f 6e5b  ore_time_region[
+00058a90: 305d 2c73 656c 662e 6261 7365 756e 6974  0],self.baseunit
+00058aa0: 2c73 656c 662e 6967 6e6f 7265 5f74 696d  ,self.ignore_tim
+00058ab0: 655f 7265 6769 6f6e 5b31 5d2c 7365 6c66  e_region[1],self
+00058ac0: 2e62 6173 6575 6e69 7429 090d 0a09 0909  .baseunit)......
+00058ad0: 0952 6573 756c 745f 7374 7269 6e67 2b3d  .Result_string+=
+00058ae0: 2754 6865 206d 696e 696d 756d 2065 7272  'The minimum err
+00058af0: 6f72 2069 733a 7b3a 2e38 657d 5c6e 272e  or is:{:.8e}\n'.
+00058b00: 666f 726d 6174 2873 656c 662e 7265 5b27  format(self.re['
+00058b10: 6572 726f 7227 5d29 0d0a 0909 0909 5265  error'])......Re
+00058b20: 7375 6c74 5f73 7472 696e 672b 3d27 5468  sult_string+='Th
+00058b30: 6520 6d69 6e69 6d75 6d20 5232 2d76 616c  e minimum R2-val
+00058b40: 7565 2069 733a 7b3a 2e38 657d 5c6e 272e  ue is:{:.8e}\n'.
+00058b50: 666f 726d 6174 2873 656c 662e 7265 5b27  format(self.re['
+00058b60: 7232 275d 290d 0a09 0909 0969 6620 2763  r2'])......if 'c
+00058b70: 6f6e 6669 6465 6e63 6527 2069 6e20 7365  onfidence' in se
+00058b80: 6c66 2e72 653a 0d0a 0909 0909 0952 6573  lf.re:.......Res
+00058b90: 756c 745f 7374 7269 6e67 2b3d 275c 6e49  ult_string+='\nI
+00058ba0: 6e20 5261 7465 7320 7769 7468 2063 6f6e  n Rates with con
+00058bb0: 6669 6465 6e63 6520 696e 7465 7276 616c  fidence interval
+00058bc0: 2074 6f20 6c65 7665 6c20 6f66 2025 735c   to level of %s\
+00058bd0: 6e27 2573 656c 662e 7265 5b27 636f 6e66  n'%self.re['conf
+00058be0: 6964 656e 6365 275d 5b27 7461 7267 6574  idence']['target
+00058bf0: 2d6c 6576 656c 275d 0d0a 0909 0909 0952  -level'].......R
+00058c00: 6573 756c 745f 7374 7269 6e67 2b3d 7365  esult_string+=se
+00058c10: 6c66 2e72 655b 2766 6974 5f72 6573 756c  lf.re['fit_resul
+00058c20: 7473 5f72 6174 6573 275d 2e74 6f5f 7374  ts_rates'].to_st
+00058c30: 7269 6e67 2863 6f6c 756d 6e73 3d5b 2776  ring(columns=['v
+00058c40: 616c 7565 272c 276c 6f77 6572 5f6c 696d  alue','lower_lim
+00058c50: 6974 272c 2775 7070 6572 5f6c 696d 6974  it','upper_limit
+00058c60: 272c 2769 6e69 745f 7661 6c75 6527 2c27  ','init_value','
+00058c70: 7661 7279 272c 276d 696e 272c 276d 6178  vary','min','max
+00058c80: 272c 2765 7870 7227 5d29 0d0a 0909 0909  ','expr'])......
+00058c90: 0952 6573 756c 745f 7374 7269 6e67 2b3d  .Result_string+=
+00058ca0: 275c 6e5c 6e54 6865 2072 6174 6573 2063  '\n\nThe rates c
+00058cb0: 6f6e 7665 7274 6564 2074 6f20 7469 6d65  onverted to time
+00058cc0: 7320 7769 7468 2075 6e69 7420 2573 5c6e  s with unit %s\n
+00058cd0: 2077 6974 6820 636f 6e66 6964 656e 6365   with confidence
+00058ce0: 2069 6e74 6572 7661 6c20 746f 206c 6576   interval to lev
+00058cf0: 656c 206f 6620 2573 5c6e 2725 2873 656c  el of %s\n'%(sel
+00058d00: 662e 6261 7365 756e 6974 2c73 656c 662e  f.baseunit,self.
+00058d10: 7265 5b27 636f 6e66 6964 656e 6365 275d  re['confidence']
+00058d20: 5b27 7461 7267 6574 2d6c 6576 656c 275d  ['target-level']
+00058d30: 290d 0a09 0909 0909 5265 7375 6c74 5f73  ).......Result_s
+00058d40: 7472 696e 672b 3d73 656c 662e 7265 5b27  tring+=self.re['
+00058d50: 6669 745f 7265 7375 6c74 735f 7469 6d65  fit_results_time
+00058d60: 7327 5d2e 746f 5f73 7472 696e 6728 636f  s'].to_string(co
+00058d70: 6c75 6d6e 733d 5b27 7661 6c75 6527 2c27  lumns=['value','
+00058d80: 6c6f 7765 725f 6c69 6d69 7427 2c27 7570  lower_limit','up
+00058d90: 7065 725f 6c69 6d69 7427 2c27 696e 6974  per_limit','init
+00058da0: 5f76 616c 7565 272c 2776 6172 7927 2c27  _value','vary','
+00058db0: 6d69 6e27 2c27 6d61 7827 2c27 6578 7072  min','max','expr
+00058dc0: 275d 290d 0a09 0909 0965 6c73 653a 0d0a  '])......else:..
+00058dd0: 0909 0909 0952 6573 756c 745f 7374 7269  .....Result_stri
+00058de0: 6e67 2b3d 275c 6e49 6e20 5261 7465 735c  ng+='\nIn Rates\
+00058df0: 6e27 0d0a 0909 0909 0952 6573 756c 745f  n'.......Result_
+00058e00: 7374 7269 6e67 2b3d 7365 6c66 2e72 655b  string+=self.re[
+00058e10: 2766 6974 5f72 6573 756c 7473 5f72 6174  'fit_results_rat
+00058e20: 6573 275d 2e74 6f5f 7374 7269 6e67 2863  es'].to_string(c
+00058e30: 6f6c 756d 6e73 3d5b 2776 616c 7565 272c  olumns=['value',
+00058e40: 2769 6e69 745f 7661 6c75 6527 2c27 7661  'init_value','va
+00058e50: 7279 272c 276d 696e 272c 276d 6178 272c  ry','min','max',
+00058e60: 2765 7870 7227 5d29 0d0a 0909 0909 0952  'expr']).......R
+00058e70: 6573 756c 745f 7374 7269 6e67 2b3d 275c  esult_string+='\
+00058e80: 6e5c 6e54 6865 2072 6174 6573 2063 6f6e  n\nThe rates con
+00058e90: 7665 7274 6564 2074 6f20 7469 6d65 7320  verted to times 
+00058ea0: 7769 7468 2075 6e69 7420 2573 5c6e 2725  with unit %s\n'%
+00058eb0: 7365 6c66 2e62 6173 6575 6e69 740d 0a09  self.baseunit...
+00058ec0: 0909 0909 5265 7375 6c74 5f73 7472 696e  ....Result_strin
+00058ed0: 672b 3d73 656c 662e 7265 5b27 6669 745f  g+=self.re['fit_
+00058ee0: 7265 7375 6c74 735f 7469 6d65 7327 5d2e  results_times'].
+00058ef0: 746f 5f73 7472 696e 6728 636f 6c75 6d6e  to_string(column
+00058f00: 733d 5b27 7661 6c75 6527 2c27 696e 6974  s=['value','init
+00058f10: 5f76 616c 7565 272c 2776 6172 7927 2c27  _value','vary','
+00058f20: 6d69 6e27 2c27 6d61 7827 2c27 6578 7072  min','max','expr
+00058f30: 275d 290d 0a09 0909 6578 6365 7074 3a0d  ']).....except:.
+00058f40: 0a09 0909 0970 6173 730d 0a09 0969 6620  .....pass....if 
+00058f50: 2827 7064 6627 2069 6e20 7361 7665 7479  ('pdf' in savety
+00058f60: 7065 2920 6f72 2028 2770 6e67 2720 696e  pe) or ('png' in
+00058f70: 2073 6176 6574 7970 6529 206f 7220 2827   savetype) or ('
+00058f80: 7376 6727 2069 6e20 7361 7665 7479 7065  svg' in savetype
+00058f90: 293a 0d0a 0909 0969 6620 7361 7665 5f52  ):.....if save_R
+00058fa0: 4157 3a0d 0a09 0909 0966 6967 2c61 783d  AW:......fig,ax=
+00058fb0: 706c 742e 7375 6270 6c6f 7473 286e 726f  plt.subplots(nro
+00058fc0: 7773 3d32 2c6e 636f 6c73 3d32 2c66 6967  ws=2,ncols=2,fig
+00058fd0: 7369 7a65 3d28 3130 2c37 2e35 2929 0d0a  size=(10,7.5))..
+00058fe0: 0909 0909 6178 5b30 2c31 5d2e 696d 7368  ....ax[0,1].imsh
+00058ff0: 6f77 286d 7069 6d67 2e69 6d72 6561 6428  ow(mpimg.imread(
+00059000: 7374 7228 7261 775f 6e61 6d65 735b 305d  str(raw_names[0]
+00059010: 2929 290d 0a09 0909 0961 785b 302c 305d  )))......ax[0,0]
+00059020: 2e69 6d73 686f 7728 6d70 696d 672e 696d  .imshow(mpimg.im
+00059030: 7265 6164 2873 7472 2872 6177 5f6e 616d  read(str(raw_nam
+00059040: 6573 5b31 5d29 2929 0d0a 0909 0909 6178  es[1])))......ax
+00059050: 5b31 2c30 5d2e 696d 7368 6f77 286d 7069  [1,0].imshow(mpi
+00059060: 6d67 2e69 6d72 6561 6428 7374 7228 7261  mg.imread(str(ra
+00059070: 775f 6e61 6d65 735b 325d 2929 290d 0a09  w_names[2])))...
+00059080: 0909 0961 785b 312c 315d 2e69 6d73 686f  ...ax[1,1].imsho
+00059090: 7728 6d70 696d 672e 696d 7265 6164 2873  w(mpimg.imread(s
+000590a0: 7472 2872 6177 5f6e 616d 6573 5b33 5d29  tr(raw_names[3])
+000590b0: 2929 0d0a 0909 0909 6178 5b30 2c30 5d2e  ))......ax[0,0].
+000590c0: 6178 6973 2827 6f66 6627 293b 6178 5b31  axis('off');ax[1
+000590d0: 2c30 5d2e 6178 6973 2827 6f66 6627 293b  ,0].axis('off');
+000590e0: 6178 5b30 2c31 5d2e 6178 6973 2827 6f66  ax[0,1].axis('of
+000590f0: 6627 293b 6178 5b31 2c31 5d2e 6178 6973  f');ax[1,1].axis
+00059100: 2827 6f66 6627 290d 0a09 0909 0966 6f72  ('off')......for
+00059110: 2065 6e74 7279 2069 6e20 7361 7665 7479   entry in savety
+00059120: 7065 3a0d 0a09 0909 0909 6966 2065 6e74  pe:.......if ent
+00059130: 7279 203d 3d20 2270 7074 7822 3a63 6f6e  ry == "pptx":con
+00059140: 7469 6e75 650d 0a09 0909 0909 7472 793a  tinue.......try:
+00059150: 0d0a 0909 0909 0909 6669 672e 7469 6768  ........fig.tigh
+00059160: 745f 6c61 796f 7574 2829 0d0a 0909 0909  t_layout()......
+00059170: 0909 6669 672e 7361 7665 6669 6728 6368  ..fig.savefig(ch
+00059180: 6563 6b5f 666f 6c64 6572 2870 6174 683d  eck_folder(path=
+00059190: 7061 7468 2c63 7572 7265 6e74 5f70 6174  path,current_pat
+000591a0: 683d 7365 6c66 2e70 6174 682c 6669 6c65  h=self.path,file
+000591b0: 6e61 6d65 3d73 656c 662e 6669 6c65 6e61  name=self.filena
+000591c0: 6d65 2e73 706c 6974 2827 2e27 295b 305d  me.split('.')[0]
+000591d0: 202b 2027 5f52 4157 2d73 756d 6d61 7279   + '_RAW-summary
+000591e0: 2e25 7327 2565 6e74 7279 292c 6470 693d  .%s'%entry),dpi=
+000591f0: 3630 3029 0d0a 0909 0909 0965 7863 6570  600).......excep
+00059200: 743a 0d0a 0909 0909 0909 7072 696e 7428  t:........print(
+00059210: 2273 6176 696e 6720 696e 2220 2b20 656e  "saving in" + en
+00059220: 7472 7920 2b22 6661 696c 6564 2229 0d0a  try +"failed")..
+00059230: 0909 0969 6620 7361 7665 5f46 6974 3a0d  ...if save_Fit:.
+00059240: 0a09 0909 0947 203d 2047 7269 6453 7065  .....G = GridSpe
+00059250: 6328 342c 2038 290d 0a09 0909 0966 6967  c(4, 8)......fig
+00059260: 313d 706c 742e 6669 6775 7265 2866 6967  1=plt.figure(fig
+00059270: 7369 7a65 3d28 3130 2c37 2e35 2929 0d0a  size=(10,7.5))..
+00059280: 0909 0909 6178 313d 6669 6731 2e61 6464  ....ax1=fig1.add
+00059290: 5f73 7562 706c 6f74 2847 5b30 2c3a 365d  _subplot(G[0,:6]
+000592a0: 290d 0a09 0909 0961 7832 3d66 6967 312e  )......ax2=fig1.
+000592b0: 6164 645f 7375 6270 6c6f 7428 475b 312c  add_subplot(G[1,
+000592c0: 3a36 5d29 0d0a 0909 0909 6178 333d 6669  :6])......ax3=fi
+000592d0: 6731 2e61 6464 5f73 7562 706c 6f74 2847  g1.add_subplot(G
+000592e0: 5b32 2c3a 365d 290d 0a09 0909 0961 7834  [2,:6])......ax4
+000592f0: 3d66 6967 312e 6164 645f 7375 6270 6c6f  =fig1.add_subplo
+00059300: 7428 475b 332c 3a36 5d29 0d0a 0909 0909  t(G[3,:6])......
+00059310: 6178 353d 6669 6731 2e61 6464 5f73 7562  ax5=fig1.add_sub
+00059320: 706c 6f74 2847 5b30 3a32 2c35 3a5d 290d  plot(G[0:2,5:]).
+00059330: 0a09 0909 0961 7836 3d66 6967 312e 6164  .....ax6=fig1.ad
+00059340: 645f 7375 6270 6c6f 7428 475b 323a 2c36  d_subplot(G[2:,6
+00059350: 3a5d 290d 0a09 0909 0961 7831 2e69 6d73  :])......ax1.ims
+00059360: 686f 7728 6d70 696d 672e 696d 7265 6164  how(mpimg.imread
+00059370: 2873 7472 2866 6974 5f6e 616d 6573 5b31  (str(fit_names[1
+00059380: 5d29 2929 0d0a 0909 0909 6178 322e 696d  ])))......ax2.im
+00059390: 7368 6f77 286d 7069 6d67 2e69 6d72 6561  show(mpimg.imrea
+000593a0: 6428 7374 7228 6669 745f 6e61 6d65 735b  d(str(fit_names[
+000593b0: 325d 2929 290d 0a09 0909 0961 7833 2e69  2])))......ax3.i
+000593c0: 6d73 686f 7728 6d70 696d 672e 696d 7265  mshow(mpimg.imre
+000593d0: 6164 2873 7472 2866 6974 5f6e 616d 6573  ad(str(fit_names
+000593e0: 5b33 5d29 2929 0d0a 0909 0909 6178 342e  [3])))......ax4.
+000593f0: 696d 7368 6f77 286d 7069 6d67 2e69 6d72  imshow(mpimg.imr
+00059400: 6561 6428 7374 7228 6669 745f 6e61 6d65  ead(str(fit_name
+00059410: 735b 345d 2929 290d 0a09 0909 0961 7835  s[4])))......ax5
+00059420: 2e69 6d73 686f 7728 6d70 696d 672e 696d  .imshow(mpimg.im
+00059430: 7265 6164 2873 7472 2866 6974 5f6e 616d  read(str(fit_nam
+00059440: 6573 5b30 5d29 2929 0d0a 0909 0909 6178  es[0])))......ax
+00059450: 362e 7465 7874 2830 2c30 2c52 6573 756c  6.text(0,0,Resul
+00059460: 745f 7374 7269 6e67 2c66 6f6e 7473 697a  t_string,fontsiz
+00059470: 653d 372c 666f 6e74 7765 6967 6874 3d27  e=7,fontweight='
+00059480: 6e6f 726d 616c 2729 0d0a 0909 0909 6178  normal')......ax
+00059490: 312e 6178 6973 2827 6f66 6627 293b 6178  1.axis('off');ax
+000594a0: 322e 6178 6973 2827 6f66 6627 293b 6178  2.axis('off');ax
+000594b0: 332e 6178 6973 2827 6f66 6627 293b 6178  3.axis('off');ax
+000594c0: 342e 6178 6973 2827 6f66 6627 293b 6178  4.axis('off');ax
+000594d0: 352e 6178 6973 2827 6f66 6627 293b 6178  5.axis('off');ax
+000594e0: 362e 6178 6973 2827 6f66 6627 290d 0a09  6.axis('off')...
+000594f0: 0909 0966 6f72 2065 6e74 7279 2069 6e20  ...for entry in 
+00059500: 7361 7665 7479 7065 3a0d 0a09 0909 0909  savetype:.......
+00059510: 6966 2065 6e74 7279 203d 3d20 2270 7074  if entry == "ppt
+00059520: 7822 3a20 636f 6e74 696e 7565 0d0a 0909  x": continue....
+00059530: 0909 0974 7279 3a0d 0a09 0909 0909 0966  ...try:........f
+00059540: 6967 312e 7469 6768 745f 6c61 796f 7574  ig1.tight_layout
+00059550: 2829 0d0a 0909 0909 0909 6669 6731 2e73  ()........fig1.s
+00059560: 6176 6566 6967 2863 6865 636b 5f66 6f6c  avefig(check_fol
+00059570: 6465 7228 7061 7468 3d70 6174 682c 6375  der(path=path,cu
+00059580: 7272 656e 745f 7061 7468 3d73 656c 662e  rrent_path=self.
+00059590: 7061 7468 2c66 696c 656e 616d 653d 7365  path,filename=se
+000595a0: 6c66 2e66 696c 656e 616d 652e 7370 6c69  lf.filename.spli
+000595b0: 7428 272e 2729 5b30 5d20 2b20 275f 4669  t('.')[0] + '_Fi
+000595c0: 742d 7375 6d6d 6172 792e 2573 2725 656e  t-summary.%s'%en
+000595d0: 7472 7929 2c64 7069 3d36 3030 290d 0a09  try),dpi=600)...
+000595e0: 0909 0909 6578 6365 7074 3a0d 0a09 0909  ....except:.....
+000595f0: 0909 0970 7269 6e74 2822 7361 7669 6e67  ...print("saving
+00059600: 2069 6e22 202b 2065 6e74 7279 202b 2266   in" + entry +"f
+00059610: 6169 6c65 6422 290d 0a09 0969 6620 2827  ailed")....if ('
+00059620: 7070 7478 2720 696e 2073 6176 6574 7970  pptx' in savetyp
+00059630: 6529 206f 7220 2827 7070 7427 2069 6e20  e) or ('ppt' in 
+00059640: 7361 7665 7479 7065 293a 0d0a 0909 096c  savetype):.....l
+00059650: 6566 743d 496e 6368 6573 2830 2e32 290d  eft=Inches(0.2).
+00059660: 0a09 0909 746f 703d 496e 6368 6573 2830  ....top=Inches(0
+00059670: 2e32 290d 0a09 0909 7072 7320 3d20 5072  .2).....prs = Pr
+00059680: 6573 656e 7461 7469 6f6e 2829 0d0a 0909  esentation()....
+00059690: 0962 6c61 6e6b 5f73 6c69 6465 5f6c 6179  .blank_slide_lay
+000596a0: 6f75 7420 3d20 7072 732e 736c 6964 655f  out = prs.slide_
+000596b0: 6c61 796f 7574 735b 365d 0d0a 0909 0973  layouts[6].....s
+000596c0: 6c69 6465 203d 2070 7273 2e73 6c69 6465  lide = prs.slide
+000596d0: 732e 6164 645f 736c 6964 6528 626c 616e  s.add_slide(blan
+000596e0: 6b5f 736c 6964 655f 6c61 796f 7574 290d  k_slide_layout).
+000596f0: 0a09 0909 6966 2073 6176 655f 5241 573a  ....if save_RAW:
+00059700: 0d0a 0909 0909 6c65 6674 203d 2074 6f70  ......left = top
+00059710: 203d 2049 6e63 6865 7328 302e 3529 0d0a   = Inches(0.5)..
+00059720: 0909 0909 7069 6320 3d20 736c 6964 652e  ....pic = slide.
+00059730: 7368 6170 6573 2e61 6464 5f70 6963 7475  shapes.add_pictu
+00059740: 7265 2873 7472 2872 6177 5f6e 616d 6573  re(str(raw_names
+00059750: 5b30 5d2e 7265 736f 6c76 6528 2929 2c20  [0].resolve()), 
+00059760: 6c65 6674 3d6c 6566 742b 496e 6368 6573  left=left+Inches
+00059770: 2834 2e35 292c 2074 6f70 3d74 6f70 2c20  (4.5), top=top, 
+00059780: 7769 6474 683d 496e 6368 6573 2834 2e35  width=Inches(4.5
+00059790: 2929 0d0a 0909 0909 7069 6320 3d20 736c  ))......pic = sl
+000597a0: 6964 652e 7368 6170 6573 2e61 6464 5f70  ide.shapes.add_p
+000597b0: 6963 7475 7265 2873 7472 2872 6177 5f6e  icture(str(raw_n
+000597c0: 616d 6573 5b31 5d2e 7265 736f 6c76 6528  ames[1].resolve(
+000597d0: 2929 2c20 6c65 6674 3d6c 6566 742c 2074  )), left=left, t
+000597e0: 6f70 3d74 6f70 2c20 7769 6474 683d 496e  op=top, width=In
+000597f0: 6368 6573 2834 2e35 2929 0d0a 0909 0909  ches(4.5))......
+00059800: 7069 6320 3d20 736c 6964 652e 7368 6170  pic = slide.shap
+00059810: 6573 2e61 6464 5f70 6963 7475 7265 2873  es.add_picture(s
+00059820: 7472 2872 6177 5f6e 616d 6573 5b32 5d2e  tr(raw_names[2].
+00059830: 7265 736f 6c76 6528 2929 2c20 6c65 6674  resolve()), left
+00059840: 3d6c 6566 742c 2074 6f70 3d74 6f70 2b49  =left, top=top+I
+00059850: 6e63 6865 7328 3329 2c20 7769 6474 683d  nches(3), width=
+00059860: 496e 6368 6573 2834 2e35 2929 0d0a 0909  Inches(4.5))....
+00059870: 0909 7472 793a 0d0a 0909 0909 0970 6963  ..try:.......pic
+00059880: 203d 2073 6c69 6465 2e73 6861 7065 732e   = slide.shapes.
+00059890: 6164 645f 7069 6374 7572 6528 7374 7228  add_picture(str(
+000598a0: 7261 775f 6e61 6d65 735b 335d 2e72 6573  raw_names[3].res
+000598b0: 6f6c 7665 2829 292c 206c 6566 743d 6c65  olve()), left=le
+000598c0: 6674 2b49 6e63 6865 7328 342e 3529 2c20  ft+Inches(4.5), 
+000598d0: 746f 703d 746f 702b 496e 6368 6573 2833  top=top+Inches(3
+000598e0: 292c 2068 6569 6768 743d 496e 6368 6573  ), height=Inches
+000598f0: 2833 2e34 2929 0d0a 0909 0909 6578 6365  (3.4))......exce
+00059900: 7074 3a0d 0a09 0909 0909 7061 7373 0d0a  pt:.......pass..
+00059910: 0909 0969 6620 7361 7665 5f46 6974 3a0d  ...if save_Fit:.
+00059920: 0a09 0909 0974 7279 3a0d 0a09 0909 0909  .....try:.......
+00059930: 736c 6964 6532 203d 2070 7273 2e73 6c69  slide2 = prs.sli
+00059940: 6465 732e 6164 645f 736c 6964 6528 626c  des.add_slide(bl
+00059950: 616e 6b5f 736c 6964 655f 6c61 796f 7574  ank_slide_layout
+00059960: 290d 0a09 0909 0909 6c65 6674 203d 2074  ).......left = t
+00059970: 6f70 203d 2049 6e63 6865 7328 302e 3129  op = Inches(0.1)
+00059980: 0d0a 0909 0909 0970 6963 203d 2073 6c69  .......pic = sli
+00059990: 6465 322e 7368 6170 6573 2e61 6464 5f70  de2.shapes.add_p
+000599a0: 6963 7475 7265 2873 7472 2866 6974 5f6e  icture(str(fit_n
+000599b0: 616d 6573 5b30 5d2e 7265 736f 6c76 6528  ames[0].resolve(
+000599c0: 2929 2c20 6c65 6674 3d6c 6566 742b 496e  )), left=left+In
+000599d0: 6368 6573 2835 2e35 292c 2074 6f70 3d74  ches(5.5), top=t
+000599e0: 6f70 2c20 6865 6967 6874 3d49 6e63 6865  op, height=Inche
+000599f0: 7328 332e 3529 2923 4d61 7472 6978 0d0a  s(3.5))#Matrix..
+00059a00: 0909 0909 0970 6963 203d 2073 6c69 6465  .....pic = slide
+00059a10: 322e 7368 6170 6573 2e61 6464 5f70 6963  2.shapes.add_pic
+00059a20: 7475 7265 2873 7472 2866 6974 5f6e 616d  ture(str(fit_nam
+00059a30: 6573 5b31 5d2e 7265 736f 6c76 6528 2929  es[1].resolve())
+00059a40: 2c20 6c65 6674 3d6c 6566 742c 2074 6f70  , left=left, top
+00059a50: 3d74 6f70 2c20 6865 6967 6874 3d49 6e63  =top, height=Inc
+00059a60: 6865 7328 3229 290d 0a09 0909 0909 7069  hes(2)).......pi
+00059a70: 6320 3d20 736c 6964 6532 2e73 6861 7065  c = slide2.shape
+00059a80: 732e 6164 645f 7069 6374 7572 6528 7374  s.add_picture(st
+00059a90: 7228 6669 745f 6e61 6d65 735b 325d 2e72  r(fit_names[2].r
+00059aa0: 6573 6f6c 7665 2829 292c 206c 6566 743d  esolve()), left=
+00059ab0: 6c65 6674 2c20 746f 703d 746f 702b 496e  left, top=top+In
+00059ac0: 6368 6573 2832 292c 2068 6569 6768 743d  ches(2), height=
+00059ad0: 496e 6368 6573 2832 2929 0d0a 0909 0909  Inches(2))......
+00059ae0: 0970 6963 203d 2073 6c69 6465 322e 7368  .pic = slide2.sh
+00059af0: 6170 6573 2e61 6464 5f70 6963 7475 7265  apes.add_picture
+00059b00: 2873 7472 2866 6974 5f6e 616d 6573 5b33  (str(fit_names[3
+00059b10: 5d2e 7265 736f 6c76 6528 2929 2c20 6c65  ].resolve()), le
+00059b20: 6674 3d6c 6566 742c 2074 6f70 3d74 6f70  ft=left, top=top
+00059b30: 2b49 6e63 6865 7328 332e 3929 2c20 6865  +Inches(3.9), he
+00059b40: 6967 6874 3d49 6e63 6865 7328 312e 3429  ight=Inches(1.4)
+00059b50: 290d 0a09 0909 0909 7069 6320 3d20 736c  ).......pic = sl
+00059b60: 6964 6532 2e73 6861 7065 732e 6164 645f  ide2.shapes.add_
+00059b70: 7069 6374 7572 6528 7374 7228 6669 745f  picture(str(fit_
+00059b80: 6e61 6d65 735b 345d 2e72 6573 6f6c 7665  names[4].resolve
+00059b90: 2829 292c 206c 6566 743d 6c65 6674 2c20  ()), left=left, 
+00059ba0: 746f 703d 746f 702b 496e 6368 6573 2835  top=top+Inches(5
+00059bb0: 2e34 292c 2068 6569 6768 743d 496e 6368  .4), height=Inch
+00059bc0: 6573 2832 2929 0d0a 0909 0909 090d 0a09  es(2))..........
+00059bd0: 0909 0909 7465 7874 3120 3d20 736c 6964  ....text1 = slid
+00059be0: 6532 2e73 6861 7065 732e 6164 645f 7465  e2.shapes.add_te
+00059bf0: 7874 626f 7828 6c65 6674 3d6c 6566 742b  xtbox(left=left+
+00059c00: 496e 6368 6573 2835 2e35 292c 2074 6f70  Inches(5.5), top
+00059c10: 3d74 6f70 2b49 6e63 6865 7328 332e 3529  =top+Inches(3.5)
+00059c20: 2c20 7769 6474 683d 496e 6368 6573 2834  , width=Inches(4
+00059c30: 2e35 292c 2068 6569 6768 743d 496e 6368  .5), height=Inch
+00059c40: 6573 2834 2929 0d0a 0909 0909 0974 6578  es(4)).......tex
+00059c50: 7431 2e74 6578 7420 3d20 5265 7375 6c74  t1.text = Result
+00059c60: 5f73 7472 696e 670d 0a09 0909 0909 7465  _string.......te
+00059c70: 7874 312e 7465 7874 5f66 7261 6d65 2e66  xt1.text_frame.f
+00059c80: 6974 5f74 6578 7428 666f 6e74 5f66 616d  it_text(font_fam
+00059c90: 696c 793d 7527 4172 6961 6c27 2c20 6d61  ily=u'Arial', ma
+00059ca0: 785f 7369 7a65 3d38 2c20 626f 6c64 3d46  x_size=8, bold=F
+00059cb0: 616c 7365 2c20 6974 616c 6963 3d46 616c  alse, italic=Fal
+00059cc0: 7365 290d 0a09 0909 0965 7863 6570 743a  se)......except:
+00059cd0: 0d0a 0909 0909 0970 7269 6e74 2827 6578  .......print('ex
+00059ce0: 6974 6564 2077 6865 6e20 7361 7669 6e67  ited when saving
+00059cf0: 2074 6865 2066 6974 2070 6c6f 7473 2729   the fit plots')
+00059d00: 0d0a 0909 0909 0d0a 0d0a 0909 0970 6c74  .............plt
+00059d10: 2e63 6c6f 7365 2827 616c 6c27 290d 0a09  .close('all')...
+00059d20: 0909 7365 6c66 2e73 6176 655f 6669 6775  ..self.save_figu
+00059d30: 7265 735f 746f 5f66 6f6c 6465 723d 6f72  res_to_folder=or
+00059d40: 6967 696e 0d0a 0909 0970 7273 2e73 6176  igin.....prs.sav
+00059d50: 6528 6368 6563 6b5f 666f 6c64 6572 2870  e(check_folder(p
+00059d60: 6174 683d 7061 7468 2c63 7572 7265 6e74  ath=path,current
+00059d70: 5f70 6174 683d 7365 6c66 2e70 6174 682c  _path=self.path,
+00059d80: 6669 6c65 6e61 6d65 3d73 656c 662e 6669  filename=self.fi
+00059d90: 6c65 6e61 6d65 2e73 706c 6974 2827 2e27  lename.split('.'
+00059da0: 295b 305d 202b 2027 2e70 7074 7827 2929  )[0] + '.pptx'))
+00059db0: 0d0a 0909 0970 7269 6e74 2827 416c 6c20  .....print('All 
+00059dc0: 6461 7461 2077 6173 2073 6176 6564 2074  data was saved t
+00059dd0: 6f20 2573 2725 6368 6563 6b5f 666f 6c64  o %s'%check_fold
+00059de0: 6572 2870 6174 683d 7061 7468 2c63 7572  er(path=path,cur
+00059df0: 7265 6e74 5f70 6174 683d 7365 6c66 2e70  rent_path=self.p
+00059e00: 6174 6829 290d 0a09 090d 0a09 0d0a 0d0a  ath))...........
+00059e10: 0d0a 0964 6566 2053 6176 655f 7072 6f6a  ...def Save_proj
+00059e20: 6563 7428 7365 6c66 2c20 6669 6c65 6e61  ect(self, filena
+00059e30: 6d65 3d4e 6f6e 652c 7061 7468 3d4e 6f6e  me=None,path=Non
+00059e40: 6529 3a0d 0a09 0927 2727 6675 6e63 7469  e):....'''functi
+00059e50: 6f6e 2074 6f20 6475 6d70 2061 6c6c 2074  on to dump all t
+00059e60: 6865 2070 6172 616d 6574 6572 206f 6620  he parameter of 
+00059e70: 616e 2061 6e61 6c79 7369 7320 696e 746f  an analysis into
+00059e80: 2061 6e20 6864 6635 2066 696c 652e 200d   an hdf5 file. .
+00059e90: 0a09 0954 6869 7320 6669 6c65 2063 6f6e  ...This file con
+00059ea0: 7461 696e 7320 7468 6520 6473 5f6f 7269  tains the ds_ori
+00059eb0: 2061 6e64 2061 6c6c 2074 6865 2070 6172   and all the par
+00059ec0: 616d 6574 6572 2c20 696e 636c 7564 696e  ameter, includin
+00059ed0: 6720 6669 7474 696e 6720 7061 7261 6d65  g fitting parame
+00059ee0: 7465 720d 0a09 0961 6e64 2072 6573 756c  ter....and resul
+00059ef0: 7473 2e0d 0a09 094f 6e65 206c 696d 6974  ts.....One limit
+00059f00: 6174 696f 6e20 6973 2074 6865 2066 6974  ation is the fit
+00059f10: 7469 6e67 206d 6f64 656c 2e20 4966 2074  ting model. If t
+00059f20: 6865 206d 6f64 656c 2069 7320 6275 696c  he model is buil
+00059f30: 6420 696e 2c20 736f 2074 6865 206d 6f64  d in, so the mod
+00059f40: 656c 2069 730d 0a09 0927 6578 706f 6e65  el is....'expone
+00059f50: 6e74 6961 6c27 206f 7220 2770 6172 616c  ntial' or 'paral
+00059f60: 6c65 6c27 2074 6865 6e20 7468 6520 7361  lel' then the sa
+00059f70: 6669 6e67 2077 6f72 6b73 2e20 4966 2061  fing works. If a
+00059f80: 6e20 6578 7465 726e 616c 206d 6f64 656c  n external model
+00059f90: 2069 7320 7573 6564 2074 6865 6e20 7468   is used then th
+00059fa0: 6520 0d0a 0909 646f 7374 7269 6e67 206f  e ....dostring o
+00059fb0: 6620 7468 6520 6578 7465 726e 616c 2066  f the external f
+00059fc0: 756e 6374 696f 6e20 6973 2073 746f 7265  unction is store
+00059fd0: 642c 2062 7574 206e 6f74 2074 6865 2066  d, but not the f
+00059fe0: 756e 6374 696f 6e20 6974 7365 6c66 2e0d  unction itself..
+00059ff0: 0a09 0909 090d 0a09 0950 6172 616d 6574  .........Paramet
+0005a000: 6572 730d 0a09 092d 2d2d 2d2d 2d2d 2d2d  ers....---------
+0005a010: 2d0d 0a09 090d 0a09 0970 6174 6820 3a20  -........path : 
+0005a020: 4e6f 6e65 2c20 7374 7220 6f72 2070 6174  None, str or pat
+0005a030: 682c 206f 7074 696f 6e61 6c0d 0a09 0909  h, optional.....
+0005a040: 2844 6566 6175 6c74 2920 4e6f 6e65 2c20  (Default) None, 
+0005a050: 6966 206c 6566 7420 6f6e 204e 6f6e 652c  if left on None,
+0005a060: 2074 6865 6e20 6120 666f 6c64 6572 2022   then a folder "
+0005a070: 4461 7461 2220 6973 2063 7265 6174 6564  Data" is created
+0005a080: 2069 6e20 7468 6520 666f 6c64 6572 200d   in the folder .
+0005a090: 0a09 0909 6f66 2074 6865 2070 726f 6a65  ....of the proje
+0005a0a0: 6374 2028 7365 6c66 2e70 6174 6829 0d0a  ct (self.path)..
+0005a0b0: 0909 0909 0d0a 0909 6669 6c65 6e61 6d65  ........filename
+0005a0c0: 203a 2073 7472 2c20 6f70 7469 6f6e 616c   : str, optional
+0005a0d0: 0d0a 0909 0928 4465 6661 756c 7429 204e  .....(Default) N
+0005a0e0: 6f6e 652c 2042 6173 6520 6e61 6d65 2066  one, Base name f
+0005a0f0: 6f72 2061 6c6c 2070 6c6f 7473 2e20 4966  or all plots. If
+0005a100: 204e 6f6e 652c 2074 6865 6e20 7365 6c66   None, then self
+0005a110: 2e66 696c 656e 616d 6520 7769 6c6c 2062  .filename will b
+0005a120: 6520 7573 6564 0d0a 0909 090d 0a09 0945  e used.........E
+0005a130: 7861 6d70 6c65 730d 0a09 092d 2d2d 2d2d  xamples....-----
+0005a140: 2d2d 2d0d 0a09 090d 0a09 093e 3e3e 2074  ---........>>> t
+0005a150: 612e 5361 7665 5f70 726f 6a65 6374 2829  a.Save_project()
+0005a160: 0d0a 0909 0d0a 0909 2727 270d 0a09 090d  ........'''.....
+0005a170: 0a09 0969 6620 6669 6c65 6e61 6d65 2069  ...if filename i
+0005a180: 7320 4e6f 6e65 3a0d 0a09 0909 6669 6c65  s None:.....file
+0005a190: 6e61 6d65 203d 2073 656c 662e 6669 6c65  name = self.file
+0005a1a0: 6e61 6d65 0d0a 0909 6864 6635 5f6e 616d  name....hdf5_nam
+0005a1b0: 6520 3d63 6865 636b 5f66 6f6c 6465 7228  e =check_folder(
+0005a1c0: 7061 7468 203d 2070 6174 682c 2063 7572  path = path, cur
+0005a1d0: 7265 6e74 5f70 6174 6820 3d20 7365 6c66  rent_path = self
+0005a1e0: 2e70 6174 682c 2066 696c 656e 616d 6520  .path, filename 
+0005a1f0: 3d20 6669 6c65 6e61 6d65 2e73 706c 6974  = filename.split
+0005a200: 2827 2e27 295b 305d 2b27 2e68 6466 3527  ('.')[0]+'.hdf5'
+0005a210: 290d 0a09 0969 6620 6f73 2e70 6174 682e  )....if os.path.
+0005a220: 6578 6973 7473 2868 6466 355f 6e61 6d65  exists(hdf5_name
+0005a230: 293a 0d0a 0909 0974 7279 3a0d 0a09 0909  ):.....try:.....
+0005a240: 096f 732e 7265 6d6f 7665 2868 6466 355f  .os.remove(hdf5_
+0005a250: 6e61 6d65 290d 0a09 0909 6578 6365 7074  name).....except
+0005a260: 3a0d 0a09 0909 0974 7279 3a0d 0a09 0909  :......try:.....
+0005a270: 0909 6864 6635 5f6e 616d 652e 636c 6f73  ..hdf5_name.clos
+0005a280: 6528 290d 0a09 0909 0909 6f73 2e72 656d  e().......os.rem
+0005a290: 6f76 6528 6864 6635 5f6e 616d 6529 0d0a  ove(hdf5_name)..
+0005a2a0: 0909 0909 6578 6365 7074 3a0d 0a09 0909  ....except:.....
+0005a2b0: 0909 7072 696e 7428 2746 696c 6520 6578  ..print('File ex
+0005a2c0: 6973 7473 2062 7574 2063 616e 206e 6f74  ists but can not
+0005a2d0: 2062 6520 6465 6c65 7465 6427 290d 0a09   be deleted')...
+0005a2e0: 0972 655f 7377 6974 6368 203d 2046 616c  .re_switch = Fal
+0005a2f0: 7365 0d0a 0909 7769 7468 2068 3570 792e  se....with h5py.
+0005a300: 4669 6c65 2868 6466 355f 6e61 6d65 2c20  File(hdf5_name, 
+0005a310: 2777 2729 2061 7320 663a 0d0a 0909 0966  'w') as f:.....f
+0005a320: 6f72 206b 6579 2069 6e20 7365 6c66 2e5f  or key in self._
+0005a330: 5f64 6963 745f 5f2e 6b65 7973 2829 3a0d  _dict__.keys():.
+0005a340: 0a09 0909 0969 6620 6b65 7920 3d3d 2027  .....if key == '
+0005a350: 6d6f 6427 3a0d 0a09 0909 0909 6966 2073  mod':.......if s
+0005a360: 656c 662e 5f5f 6469 6374 5f5f 5b6b 6579  elf.__dict__[key
+0005a370: 5d20 696e 205b 2770 6172 616c 272c 2765  ] in ['paral','e
+0005a380: 7870 6f6e 656e 7469 616c 272c 2763 6f6e  xponential','con
+0005a390: 7365 6375 7469 7665 272c 2766 756c 6c5f  secutive','full_
+0005a3a0: 636f 6e73 6563 7574 6976 6527 5d3a 0d0a  consecutive']:..
+0005a3b0: 0909 0909 0909 662e 6372 6561 7465 5f64  ......f.create_d
+0005a3c0: 6174 6173 6574 286e 616d 653d 6b65 792c  ataset(name=key,
+0005a3d0: 2064 6174 613d 7365 6c66 2e5f 5f64 6963   data=self.__dic
+0005a3e0: 745f 5f5b 6b65 795d 290d 0a09 0909 0909  t__[key]).......
+0005a3f0: 656c 7365 3a0d 0a09 0909 0909 0974 7279  else:........try
+0005a400: 3a0d 0a09 0909 0909 0909 646f 6373 7472  :.........docstr
+0005a410: 696e 673d 7365 6c66 2e5f 5f64 6963 745f  ing=self.__dict_
+0005a420: 5f5b 6b65 795d 2e5f 5f64 6f63 5f5f 0d0a  _[key].__doc__..
+0005a430: 0909 0909 0909 0969 6620 6973 696e 7374  .......if isinst
+0005a440: 616e 6365 2864 6f63 7374 7269 6e67 2c74  ance(docstring,t
+0005a450: 7970 6528 2768 656c 6c6f 2729 293a 0d0a  ype('hello')):..
+0005a460: 0909 0909 0909 0909 662e 6372 6561 7465  ........f.create
+0005a470: 5f64 6174 6173 6574 286e 616d 653d 6b65  _dataset(name=ke
+0005a480: 792c 2064 6174 613d 646f 6373 7472 696e  y, data=docstrin
+0005a490: 6729 0d0a 0909 0909 0909 6578 6365 7074  g)........except
+0005a4a0: 3a0d 0a09 0909 0909 0909 662e 6372 6561  :.........f.crea
+0005a4b0: 7465 5f64 6174 6173 6574 286e 616d 653d  te_dataset(name=
+0005a4c0: 6b65 792c 2064 6174 613d 2765 7874 6572  key, data='exter
+0005a4d0: 6e61 6c5f 6675 6e63 7469 6f6e 5f77 6974  nal_function_wit
+0005a4e0: 686f 7574 5f64 6f63 7374 7269 6e67 2729  hout_docstring')
+0005a4f0: 0d0a 0909 0909 656c 6966 206b 6579 2069  ......elif key i
+0005a500: 6e20 5b27 7265 6c5f 7761 7665 272c 2772  n ['rel_wave','r
+0005a510: 656c 5f74 696d 6527 5d3a 236e 6565 6420  el_time']:#need 
+0005a520: 6578 7472 612c 2061 7320 6974 2069 7320  extra, as it is 
+0005a530: 6279 7061 7373 6564 2062 7920 7468 6520  bypassed by the 
+0005a540: 7265 2d73 7769 7463 680d 0a09 0909 0909  re-switch.......
+0005a550: 662e 6372 6561 7465 5f64 6174 6173 6574  f.create_dataset
+0005a560: 286e 616d 653d 6b65 792c 2064 6174 613d  (name=key, data=
+0005a570: 7365 6c66 2e5f 5f64 6963 745f 5f5b 6b65  self.__dict__[ke
+0005a580: 795d 290d 0a09 0909 0965 6c69 6620 6b65  y])......elif ke
+0005a590: 795b 3a32 5d20 3d3d 2027 7265 2720 3a0d  y[:2] == 're' :.
+0005a5a0: 0a09 0909 0909 7265 5f73 7769 7463 6820  ......re_switch 
+0005a5b0: 3d20 5472 7565 0d0a 0909 0909 0966 6f72  = True.......for
+0005a5c0: 206b 6579 3220 696e 2073 656c 662e 5f5f   key2 in self.__
+0005a5d0: 6469 6374 5f5f 5b27 7265 275d 3a0d 0a09  dict__['re']:...
+0005a5e0: 0909 0909 0969 6620 6b65 7932 203d 3d20  .....if key2 == 
+0005a5f0: 2766 6974 5f6f 7574 7075 7427 3a63 6f6e  'fit_output':con
+0005a600: 7469 6e75 650d 0a09 0909 0909 0964 6174  tinue........dat
+0005a610: 6120 3d20 7365 6c66 2e5f 5f64 6963 745f  a = self.__dict_
+0005a620: 5f5b 2772 6527 5d5b 6b65 7932 5d0d 0a09  _['re'][key2]...
+0005a630: 0909 0909 0969 6620 6b65 7932 203d 3d20  .....if key2 == 
+0005a640: 2765 7272 6f72 273a 0d0a 0909 0909 0909  'error':........
+0005a650: 0974 7279 3a0d 0a09 0909 0909 0909 0966  .try:..........f
+0005a660: 2e63 7265 6174 655f 6461 7461 7365 7428  .create_dataset(
+0005a670: 6e61 6d65 3d27 7265 5f65 7272 6f72 272c  name='re_error',
+0005a680: 2064 6174 613d 6461 7461 290d 0a09 0909   data=data).....
+0005a690: 0909 0909 6578 6365 7074 3a0d 0a09 0909  ....except:.....
+0005a6a0: 0909 0909 0970 7269 6e74 2827 7361 7669  .....print('savi
+0005a6b0: 6e67 206f 6620 2720 2b20 6b65 7932 202b  ng of ' + key2 +
+0005a6c0: 2027 2066 6169 6c65 6427 2029 0d0a 0909   ' failed' )....
+0005a6d0: 0909 0909 656c 6966 2069 7369 6e73 7461  ....elif isinsta
+0005a6e0: 6e63 6528 6461 7461 2c20 7061 6e64 6173  nce(data, pandas
+0005a6f0: 2e44 6174 6146 7261 6d65 293a 0d0a 0909  .DataFrame):....
+0005a700: 0909 0909 0970 6173 730d 0a09 0909 0909  .....pass.......
+0005a710: 0965 6c73 653a 0d0a 0909 0909 0909 0974  .else:.........t
+0005a720: 7279 3a0d 0a09 0909 0909 0909 0966 2e63  ry:..........f.c
+0005a730: 7265 6174 655f 6461 7461 7365 7428 6e61  reate_dataset(na
+0005a740: 6d65 3d27 7265 5f27 202b 206b 6579 322c  me='re_' + key2,
+0005a750: 2064 6174 613d 6461 7461 290d 0a09 0909   data=data).....
+0005a760: 0909 0909 6578 6365 7074 3a0d 0a09 0909  ....except:.....
+0005a770: 0909 0909 0970 7269 6e74 2827 7361 7669  .....print('savi
+0005a780: 6e67 206f 6620 2720 2b20 6b65 7932 202b  ng of ' + key2 +
+0005a790: 2027 2066 6169 6c65 6427 2029 0d0a 0909   ' failed' )....
+0005a7a0: 0909 656c 6966 206b 6579 203d 3d20 2763  ..elif key == 'c
+0005a7b0: 6d61 7027 3a0d 0a09 0909 0909 7061 7373  map':.......pass
+0005a7c0: 0d0a 0909 0909 656c 6966 206b 6579 203d  ......elif key =
+0005a7d0: 3d20 2769 6e74 656e 7369 7479 5f72 616e  = 'intensity_ran
+0005a7e0: 6765 273a 0d0a 0909 0909 0964 6174 613d  ge':.......data=
+0005a7f0: 7365 6c66 2e5f 5f64 6963 745f 5f5b 2769  self.__dict__['i
+0005a800: 6e74 656e 7369 7479 5f72 616e 6765 275d  ntensity_range']
+0005a810: 0d0a 0909 0909 0969 6620 6973 696e 7374  .......if isinst
+0005a820: 616e 6365 2864 6174 612c 2074 7970 6528  ance(data, type(
+0005a830: 3165 2d33 2929 3a0d 0a09 0909 0909 0964  1e-3)):........d
+0005a840: 6174 613d 5b2d 6461 7461 2c64 6174 615d  ata=[-data,data]
+0005a850: 0d0a 0909 0909 0969 6620 6461 7461 2069  .......if data i
+0005a860: 7320 4e6f 6e65 3a0d 0a09 0909 0909 0966  s None:........f
+0005a870: 2e63 7265 6174 655f 6461 7461 7365 7428  .create_dataset(
+0005a880: 6e61 6d65 3d27 696e 7465 6e73 6974 795f  name='intensity_
+0005a890: 7261 6e67 6527 2c20 6461 7461 3d27 4e6f  range', data='No
+0005a8a0: 6e65 2729 0d0a 0909 0909 0965 6c73 653a  ne').......else:
+0005a8b0: 0d0a 0909 0909 0909 662e 6372 6561 7465  ........f.create
+0005a8c0: 5f64 6174 6173 6574 286e 616d 653d 2769  _dataset(name='i
+0005a8d0: 6e74 656e 7369 7479 5f72 616e 6765 272c  ntensity_range',
+0005a8e0: 2064 6174 613d 6461 7461 2909 0d0a 0909   data=data).....
+0005a8f0: 0909 656c 6966 206b 6579 203d 3d20 2762  ..elif key == 'b
+0005a900: 6163 6b67 726f 756e 645f 7061 7227 3a0d  ackground_par':.
+0005a910: 0a09 0909 0909 662e 6372 6561 7465 5f64  ......f.create_d
+0005a920: 6174 6173 6574 286e 616d 653d 2762 6163  ataset(name='bac
+0005a930: 6b27 2c20 6461 7461 3d73 656c 662e 5f5f  k', data=self.__
+0005a940: 6469 6374 5f5f 5b27 6261 636b 6772 6f75  dict__['backgrou
+0005a950: 6e64 5f70 6172 275d 5b33 5d29 0d0a 0909  nd_par'][3])....
+0005a960: 0909 0d0a 0909 0909 656c 6966 206b 6579  ........elif key
+0005a970: 2069 6e20 5b27 7061 7227 2c27 7061 725f   in ['par','par_
+0005a980: 6669 7427 5d3a 0d0a 0909 0909 0909 0909  fit']:..........
+0005a990: 0920 0d0a 0909 0909 0964 663d 7061 725f  . .......df=par_
+0005a9a0: 746f 5f70 6172 6466 2873 656c 662e 5f5f  to_pardf(self.__
+0005a9b0: 6469 6374 5f5f 5b6b 6579 5d29 2370 616e  dict__[key])#pan
+0005a9c0: 6461 7320 6861 7320 6120 6275 6720 616e  das has a bug an
+0005a9d0: 6420 7072 6f62 6c65 6d73 2068 616e 646c  d problems handl
+0005a9e0: 696e 6720 6d69 7865 6420 7479 7065 2063  ing mixed type c
+0005a9f0: 6f6c 756d 6e73 2077 6865 6e20 7361 7669  olumns when savi
+0005aa00: 6e67 2e20 536f 2077 6520 636c 6561 6e20  ng. So we clean 
+0005aa10: 7570 2e0d 0a09 0909 0909 666f 7220 7375  up........for su
+0005aa20: 625f 6b65 7920 696e 205b 276d 696e 272c  b_key in ['min',
+0005aa30: 276d 6178 272c 2776 616c 7565 275d 3a0d  'max','value']:.
+0005aa40: 0a09 0909 0909 0974 7279 3a0d 0a09 0909  .......try:.....
+0005aa50: 0909 0909 6466 5b73 7562 5f6b 6579 5d3d  ....df[sub_key]=
+0005aa60: 6466 5b73 7562 5f6b 6579 5d2e 6173 7479  df[sub_key].asty
+0005aa70: 7065 2866 6c6f 6174 290d 0a09 0909 0909  pe(float).......
+0005aa80: 0965 7863 6570 743a 0d0a 0909 0909 0909  .except:........
+0005aa90: 0970 6173 730d 0a09 0909 0909 6466 5b27  .pass.......df['
+0005aaa0: 6973 5f72 6174 6527 5d3d 6466 5b27 6973  is_rate']=df['is
+0005aab0: 5f72 6174 6527 5d2e 6173 7479 7065 2862  _rate'].astype(b
+0005aac0: 6f6f 6c29 0d0a 0909 0909 0964 665b 2776  ool).......df['v
+0005aad0: 6172 7927 5d3d 6466 5b27 7661 7279 275d  ary']=df['vary']
+0005aae0: 2e61 7374 7970 6528 626f 6f6c 290d 0a09  .astype(bool)...
+0005aaf0: 0909 0909 6466 5b27 6578 7072 275d 3d64  ....df['expr']=d
+0005ab00: 665b 2765 7870 7227 5d2e 6170 706c 7928  f['expr'].apply(
+0005ab10: 6c61 6d62 6461 2078 3a27 2573 2725 7829  lambda x:'%s'%x)
+0005ab20: 0d0a 0909 0909 0964 662e 746f 5f68 6466  .......df.to_hdf
+0005ab30: 2873 7472 2868 6466 355f 6e61 6d65 2e72  (str(hdf5_name.r
+0005ab40: 6573 6f6c 7665 2829 292c 206b 6579 3d6b  esolve()), key=k
+0005ab50: 6579 2c20 6170 7065 6e64 3d54 7275 652c  ey, append=True,
+0005ab60: 206d 6f64 653d 2772 2b27 2c20 666f 726d   mode='r+', form
+0005ab70: 6174 3d27 7427 290d 0a09 0909 0965 6c73  at='t')......els
+0005ab80: 653a 0d0a 0909 0909 0964 6174 6120 3d20  e:.......data = 
+0005ab90: 7365 6c66 2e5f 5f64 6963 745f 5f5b 6b65  self.__dict__[ke
+0005aba0: 795d 0d0a 0909 0909 0969 6620 6461 7461  y].......if data
+0005abb0: 2069 7320 4e6f 6e65 3a0d 0a09 0909 0909   is None:.......
+0005abc0: 0966 2e63 7265 6174 655f 6461 7461 7365  .f.create_datase
+0005abd0: 7428 6e61 6d65 3d6b 6579 2c20 6461 7461  t(name=key, data
+0005abe0: 3d27 4e6f 6e65 2729 0d0a 0909 0909 0965  ='None').......e
+0005abf0: 6c73 653a 0d0a 0909 0909 0909 6966 2069  lse:........if i
+0005ac00: 7369 6e73 7461 6e63 6528 6461 7461 2c20  sinstance(data, 
+0005ac10: 7061 6e64 6173 2e44 6174 6146 7261 6d65  pandas.DataFrame
+0005ac20: 293a 0d0a 0909 0909 0909 0970 6173 730d  ):.........pass.
+0005ac30: 0a09 0909 0909 0965 6c73 653a 0d0a 0909  .......else:....
+0005ac40: 0909 0909 0974 7279 3a0d 0a09 0909 0909  .....try:.......
+0005ac50: 0909 0966 2e63 7265 6174 655f 6461 7461  ...f.create_data
+0005ac60: 7365 7428 6e61 6d65 3d6b 6579 2c20 6461  set(name=key, da
+0005ac70: 7461 3d64 6174 6129 0d0a 0909 0909 0909  ta=data)........
+0005ac80: 0965 7863 6570 743a 0d0a 0909 0909 0909  .except:........
+0005ac90: 0909 6966 206b 6579 203d 3d20 2770 6174  ..if key == 'pat
+0005aca0: 6827 3a0d 0a09 0909 0909 0909 0909 7061  h':...........pa
+0005acb0: 7373 0d0a 0909 0909 0909 0909 656c 6966  ss..........elif
+0005acc0: 206b 6579 203d 3d20 2766 6967 7572 655f   key == 'figure_
+0005acd0: 7061 7468 273a 0d0a 0909 0909 0909 0909  path':..........
+0005ace0: 0970 6173 730d 0a09 0909 0909 0909 0965  .pass..........e
+0005acf0: 6c73 653a 0d0a 0909 0909 0909 0909 0970  lse:...........p
+0005ad00: 7269 6e74 2827 7468 6520 7361 7669 6e67  rint('the saving
+0005ad10: 206f 6620 2025 7320 2066 6169 6c65 6427   of  %s  failed'
+0005ad20: 256b 6579 290d 0a09 0909 6966 206e 6f74  %key).....if not
+0005ad30: 2027 6669 7463 6f65 6666 2720 696e 2066   'fitcoeff' in f
+0005ad40: 3a0d 0a09 0909 0974 7279 3a0d 0a09 0909  :......try:.....
+0005ad50: 0909 662e 6372 6561 7465 5f64 6174 6173  ..f.create_datas
+0005ad60: 6574 286e 616d 653d 2766 6974 636f 6566  et(name='fitcoef
+0005ad70: 6627 2c20 6461 7461 3d73 656c 662e 6669  f', data=self.fi
+0005ad80: 7463 6f65 6666 290d 0a09 0909 0965 7863  tcoeff)......exc
+0005ad90: 6570 743a 0d0a 0909 0909 0974 7279 3a0d  ept:.......try:.
+0005ada0: 0a09 0909 0909 0977 6974 6820 6f70 656e  .......with open
+0005adb0: 2873 656c 662e 6368 6972 705f 6669 6c65  (self.chirp_file
+0005adc0: 2c27 7227 2920 6173 2066 323a 0d0a 0909  ,'r') as f2:....
+0005add0: 0909 0909 0966 6974 636f 6566 663d 6632  .....fitcoeff=f2
+0005ade0: 2e72 6561 646c 696e 6528 290d 0a09 0909  .readline().....
+0005adf0: 0909 0909 662e 6372 6561 7465 5f64 6174  ....f.create_dat
+0005ae00: 6173 6574 286e 616d 653d 2766 6974 636f  aset(name='fitco
+0005ae10: 6566 6627 2c20 6461 7461 3d66 6974 636f  eff', data=fitco
+0005ae20: 6566 6629 0d0a 0909 0909 0965 7863 6570  eff).......excep
+0005ae30: 743a 0d0a 0909 0909 0909 7061 7373 0d0a  t:........pass..
+0005ae40: 0909 7365 6c66 2e64 735f 6f72 692e 746f  ..self.ds_ori.to
+0005ae50: 5f68 6466 2873 7472 2868 6466 355f 6e61  _hdf(str(hdf5_na
+0005ae60: 6d65 2e72 6573 6f6c 7665 2829 292c 206b  me.resolve()), k
+0005ae70: 6579 3d27 6473 5f6f 7269 272c 2061 7070  ey='ds_ori', app
+0005ae80: 656e 643d 5472 7565 2c20 6d6f 6465 3d27  end=True, mode='
+0005ae90: 722b 272c 2066 6f72 6d61 743d 2774 2729  r+', format='t')
+0005aea0: 2373 6176 655f 7261 775f 6461 7461 0d0a  #save_raw_data..
+0005aeb0: 0909 6966 2072 655f 7377 6974 6368 3a0d  ..if re_switch:.
+0005aec0: 0a09 0909 2370 7269 6e74 2827 7265 2d73  ....#print('re-s
+0005aed0: 7769 7463 6865 6427 290d 0a09 0909 666f  witched').....fo
+0005aee0: 7220 6b65 7920 696e 205b 2741 272c 2027  r key in ['A', '
+0005aef0: 4143 272c 2027 4145 272c 2027 4441 4327  AC', 'AE', 'DAC'
+0005af00: 2c20 2763 275d 3a0d 0a09 0909 0973 656c  , 'c']:......sel
+0005af10: 662e 7265 5b6b 6579 5d2e 746f 5f68 6466  f.re[key].to_hdf
+0005af20: 2873 7472 2868 6466 355f 6e61 6d65 2e72  (str(hdf5_name.r
+0005af30: 6573 6f6c 7665 2829 292c 206b 6579 3d27  esolve()), key='
+0005af40: 7265 5f27 202b 206b 6579 2c20 6170 7065  re_' + key, appe
+0005af50: 6e64 3d54 7275 652c 206d 6f64 653d 2772  nd=True, mode='r
+0005af60: 2b27 2c20 666f 726d 6174 3d27 7427 290d  +', format='t').
+0005af70: 0a09 0974 7279 3a0d 0a09 0909 662e 636c  ...try:.....f.cl
+0005af80: 6f73 6528 290d 0a09 0965 7863 6570 743a  ose()....except:
+0005af90: 0d0a 0909 0970 6173 730d 0a09 090d 0a09  .....pass.......
+0005afa0: 0970 7269 6e74 2827 5468 6520 7072 6f6a  .print('The proj
+0005afb0: 6563 7420 7761 7320 7361 7665 6420 746f  ect was saved to
+0005afc0: 2025 7327 2563 6865 636b 5f66 6f6c 6465   %s'%check_folde
+0005afd0: 7228 7061 7468 203d 2070 6174 682c 2063  r(path = path, c
+0005afe0: 7572 7265 6e74 5f70 6174 6820 3d20 7365  urrent_path = se
+0005aff0: 6c66 2e70 6174 6829 290d 0a0d 0a0d 0a09  lf.path)).......
+0005b000: 6465 6620 5f5f 7265 6164 5f70 726f 6a65  def __read_proje
+0005b010: 6374 2873 656c 662c 2073 6176 6564 5f70  ct(self, saved_p
+0005b020: 726f 6a65 6374 3d4e 6f6e 652c 6375 7272  roject=None,curr
+0005b030: 656e 745f 7061 7468 3d4e 6f6e 6529 3a0d  ent_path=None):.
+0005b040: 0a09 0927 2727 6675 6e63 7469 6f6e 2074  ...'''function t
+0005b050: 6f20 7265 2d72 6561 6420 616c 6c20 7468  o re-read all th
+0005b060: 6520 7061 7261 6d65 7465 7220 6f66 2061  e parameter of a
+0005b070: 2070 7265 7669 6f75 7320 616e 616c 7973   previous analys
+0005b080: 6973 200d 0a09 0969 6e74 6f20 616e 2068  is ....into an h
+0005b090: 6466 3520 6669 6c65 2c20 6375 7272 656e  df5 file, curren
+0005b0a0: 7420 7061 7468 2069 7320 7468 6520 7061  t path is the pa
+0005b0b0: 7468 2074 6861 7420 7468 6520 6669 6c65  th that the file
+0005b0c0: 2073 686f 756c 6420 0d0a 0909 6173 7375   should ....assu
+0005b0d0: 6d65 2069 7320 6974 7320 2268 6f6d 6520  me is its "home 
+0005b0e0: 6469 7265 6374 6f72 7922 2061 6674 6572  directory" after
+0005b0f0: 2073 7563 6365 7373 6675 6c20 6c6f 6164   successful load
+0005b100: 696e 672e 2049 6620 6e6f 7420 0d0a 0909  ing. If not ....
+0005b110: 7365 7420 7765 2074 616b 6520 7468 6520  set we take the 
+0005b120: 6669 6c65 7061 7468 2061 7420 7768 6963  filepath at whic
+0005b130: 6820 7468 6520 6669 6c65 2069 7320 6375  h the file is cu
+0005b140: 7272 656e 746c 7920 7374 6f72 6564 2061  rrently stored a
+0005b150: 7320 7061 7468 2727 270d 0a09 0969 6620  s path'''....if 
+0005b160: 7361 7665 645f 7072 6f6a 6563 7420 6973  saved_project is
+0005b170: 204e 6f6e 653a 0d0a 0909 0972 6169 7365   None:.....raise
+0005b180: 2049 6d70 6f72 7445 7272 6f72 2827 5765   ImportError('We
+0005b190: 2064 6f20 6e65 6564 2061 2070 726f 6a65   do need a proje
+0005b1a0: 6374 2074 6f20 696d 706f 7274 2729 0d0a  ct to import')..
+0005b1b0: 0909 6966 2063 7572 7265 6e74 5f70 6174  ..if current_pat
+0005b1c0: 6820 6973 204e 6f6e 653a 6375 7272 656e  h is None:curren
+0005b1d0: 745f 7061 7468 3d6f 732e 7061 7468 2e64  t_path=os.path.d
+0005b1e0: 6972 6e61 6d65 286f 732e 7061 7468 2e61  irname(os.path.a
+0005b1f0: 6273 7061 7468 2873 6176 6564 5f70 726f  bspath(saved_pro
+0005b200: 6a65 6374 2929 0d0a 0909 7472 793a 0d0a  ject))....try:..
+0005b210: 0909 0969 6d70 6f72 7420 6835 7079 0d0a  ...import h5py..
+0005b220: 0909 6578 6365 7074 3a0d 0a09 0920 0d0a  ..except:.... ..
+0005b230: 0909 0970 7269 6e74 2827 636f 756c 6420  ...print('could 
+0005b240: 6e6f 7420 696d 706f 7274 2068 6466 352c  not import hdf5,
+0005b250: 2063 7572 7265 6e74 2076 6572 7369 6f6e   current version
+0005b260: 2072 6571 7569 7265 7320 7468 6174 2074   requires that t
+0005b270: 6869 7320 6973 2069 6e73 7461 6c6c 6564  his is installed
+0005b280: 2e20 4946 2072 756e 6e69 6e67 2041 6e61  . IF running Ana
+0005b290: 636f 6e64 6120 6f70 656e 2043 6f6e 6461  conda open Conda
+0005b2a0: 2070 726f 6d74 2061 6e64 2074 7970 653a   promt and type:
+0005b2b0: 2063 6f6e 6461 2069 6e73 7461 6c6c 2068   conda install h
+0005b2c0: 3570 7927 290d 0a09 0964 6174 615f 6672  5py')....data_fr
+0005b2d0: 616d 655f 6c69 7374 3d5b 5d0d 0a0d 0a09  ame_list=[].....
+0005b2e0: 0923 2077 6520 6861 7620 746f 2068 616e  .# we hav to han
+0005b2f0: 646c 6520 7468 6520 6f6c 6420 616e 6420  dle the old and 
+0005b300: 6e65 7720 7479 7065 206f 6620 7361 7669  new type of savi
+0005b310: 6e67 0d0a 0909 7769 7468 2068 3570 792e  ng....with h5py.
+0005b320: 4669 6c65 2873 6176 6564 5f70 726f 6a65  File(saved_proje
+0005b330: 6374 2c20 2772 2729 2061 7320 663a 0d0a  ct, 'r') as f:..
+0005b340: 0909 0969 6620 2772 655f 6669 6e61 6c5f  ...if 're_final_
+0005b350: 7365 7475 705f 7061 7227 2069 6e20 662e  setup_par' in f.
+0005b360: 6b65 7973 2829 3a6f 6c64 5f73 7769 7463  keys():old_switc
+0005b370: 683d 5472 7565 0d0a 0909 0909 0920 0d0a  h=True....... ..
+0005b380: 0909 0d0a 0909 0965 6c73 653a 6f6c 645f  .......else:old_
+0005b390: 7377 6974 6368 3d46 616c 7365 0d0a 0909  switch=False....
+0005b3a0: 0909 0920 2020 0d0a 0909 6966 206f 6c64  ...   ....if old
+0005b3b0: 5f73 7769 7463 683a 7072 696e 7428 2777  _switch:print('w
+0005b3c0: 6520 7265 6164 2061 6e20 6f6c 6420 7374  e read an old st
+0005b3d0: 796c 6520 6461 7461 5f66 696c 6520 616e  yle data_file an
+0005b3e0: 6420 6469 7265 6374 6c79 2075 7064 6174  d directly updat
+0005b3f0: 6520 6974 2069 6e74 6f20 7468 6520 6e65  e it into the ne
+0005b400: 7720 6669 6c65 5f74 7970 6520 6166 7465  w file_type afte
+0005b410: 7220 6c6f 6164 696e 6727 290d 0a09 0977  r loading')....w
+0005b420: 6974 6820 6835 7079 2e46 696c 6528 7361  ith h5py.File(sa
+0005b430: 7665 645f 7072 6f6a 6563 742c 2027 7227  ved_project, 'r'
+0005b440: 2920 6173 2066 3a0d 0a09 0909 666f 7220  ) as f:.....for 
+0005b450: 6b65 7920 696e 2066 2e6b 6579 7328 293a  key in f.keys():
+0005b460: 0d0a 0909 0909 7472 793a 0d0a 0909 0909  ......try:......
+0005b470: 0969 6620 2272 655f 2220 696e 206b 6579  .if "re_" in key
+0005b480: 5b3a 335d 3a0d 0a09 0909 0909 0969 6620  [:3]:........if 
+0005b490: 6e6f 7420 2772 6527 2069 6e20 7365 6c66  not 're' in self
+0005b4a0: 2e5f 5f64 6963 745f 5f2e 6b65 7973 2829  .__dict__.keys()
+0005b4b0: 3a0d 0a09 0909 0909 0909 7365 6c66 2e5f  :.........self._
+0005b4c0: 5f64 6963 745f 5f5b 2772 6527 5d3d 7b7d  _dict__['re']={}
+0005b4d0: 0d0a 0909 0909 0909 7365 6c66 2e5f 5f64  ........self.__d
+0005b4e0: 6963 745f 5f5b 2772 6527 5d5b 6b65 795b  ict__['re'][key[
+0005b4f0: 333a 5d5d 3d66 5b6b 6579 5d5b 2829 5d0d  3:]]=f[key][()].
+0005b500: 0a09 0909 0909 656c 6966 2022 6261 636b  ......elif "back
+0005b510: 2220 696e 206b 6579 5b3a 345d 3a0d 0a09  " in key[:4]:...
+0005b520: 0909 0909 0972 6561 3d66 5b6b 6579 5d5b  .....rea=f[key][
+0005b530: 2829 5d0d 0a09 0909 0909 0973 656c 662e  ()]........self.
+0005b540: 5f5f 6469 6374 5f5f 5b27 6261 636b 6772  __dict__['backgr
+0005b550: 6f75 6e64 5f70 6172 275d 3d5b 4e6f 6e65  ound_par']=[None
+0005b560: 2c2d 312c 4661 6c73 655d 0d0a 0909 0909  ,-1,False]......
+0005b570: 0909 7365 6c66 2e5f 5f64 6963 745f 5f5b  ..self.__dict__[
+0005b580: 2762 6163 6b67 726f 756e 645f 7061 7227  'background_par'
+0005b590: 5d2e 6170 7065 6e64 2872 6561 290d 0a09  ].append(rea)...
+0005b5a0: 0909 0909 656c 6966 2022 7061 7222 2069  ....elif "par" i
+0005b5b0: 6e20 6b65 795b 3a33 5d3a 0d0a 0909 0909  n key[:3]:......
+0005b5c0: 0909 6966 206f 6c64 5f73 7769 7463 683a  ..if old_switch:
+0005b5d0: 236f 6c64 2074 7970 6520 6f66 2073 6176  #old type of sav
+0005b5e0: 6564 2064 6174 610d 0a09 0909 0909 0909  ed data.........
+0005b5f0: 7472 793a 0d0a 0909 0909 0909 0909 6f73  try:..........os
+0005b600: 2e72 656d 6f76 6528 2774 656d 705f 6669  .remove('temp_fi
+0005b610: 6c65 2e6a 736f 6e27 290d 0a09 0909 0909  le.json').......
+0005b620: 0909 6578 6365 7074 3a0d 0a09 0909 0909  ..except:.......
+0005b630: 0909 0970 6173 730d 0a09 0909 0909 0909  ...pass.........
+0005b640: 7769 7468 206f 7065 6e28 2774 656d 705f  with open('temp_
+0005b650: 6669 6c65 2e6a 736f 6e27 2c27 7727 2920  file.json','w') 
+0005b660: 6173 2067 3a0d 0a09 0909 0909 0909 0967  as g:..........g
+0005b670: 2e77 7269 7465 2866 5b6b 6579 5d5b 2829  .write(f[key][()
+0005b680: 5d29 0d0a 0909 0909 0909 0977 6974 6820  ]).........with 
+0005b690: 6f70 656e 2827 7465 6d70 5f66 696c 652e  open('temp_file.
+0005b6a0: 6a73 6f6e 272c 2772 2729 2061 7320 673a  json','r') as g:
+0005b6b0: 0d0a 0909 0909 0909 0909 7365 6c66 2e70  ..........self.p
+0005b6c0: 6172 3d6c 6d66 6974 2e50 6172 616d 6574  ar=lmfit.Paramet
+0005b6d0: 6572 7328 290d 0a09 0909 0909 0909 0973  ers()..........s
+0005b6e0: 656c 662e 7061 722e 6c6f 6164 2867 290d  elf.par.load(g).
+0005b6f0: 0a09 0909 0909 0909 7472 793a 0d0a 0909  ........try:....
+0005b700: 0909 0909 0909 6f73 2e72 656d 6f76 6528  ......os.remove(
+0005b710: 2774 656d 705f 6669 6c65 2e6a 736f 6e27  'temp_file.json'
+0005b720: 290d 0a09 0909 0909 0909 6578 6365 7074  ).........except
+0005b730: 3a0d 0a09 0909 0909 0909 0970 6173 730d  :..........pass.
+0005b740: 0a09 0909 0909 0965 6c73 653a 236e 6577  .......else:#new
+0005b750: 2074 7970 6520 6f66 2064 6174 610d 0a09   type of data...
+0005b760: 0909 0909 0909 7261 6973 6509 090d 0a09  ......raise.....
+0005b770: 0909 0909 656c 7365 3a0d 0a09 0909 0909  ....else:.......
+0005b780: 0972 6561 643d 665b 6b65 795d 5b28 295d  .read=f[key][()]
+0005b790: 0d0a 0909 0909 0909 6966 2069 7369 6e73  ........if isins
+0005b7a0: 7461 6e63 6528 7265 6164 2c62 7974 6573  tance(read,bytes
+0005b7b0: 293a 0d0a 0909 0909 0909 0972 6561 643d  ):.........read=
+0005b7c0: 665b 6b65 795d 2e61 7373 7472 2829 5b28  f[key].asstr()[(
+0005b7d0: 295d 200d 0a09 0909 0909 0965 6c69 6620  )] ........elif 
+0005b7e0: 6973 696e 7374 616e 6365 2872 6561 642c  isinstance(read,
+0005b7f0: 7479 7065 2827 6865 6c6c 6f27 2929 3a0d  type('hello')):.
+0005b800: 0a09 0909 0909 0909 6966 2028 7265 6164  ........if (read
+0005b810: 3d3d 274e 6f6e 6527 2920 6f72 2028 7265  =='None') or (re
+0005b820: 6164 3d3d 276e 6f6e 6527 293a 0d0a 0909  ad=='none'):....
+0005b830: 0909 0909 0909 7265 6164 3d4e 6f6e 650d  ......read=None.
+0005b840: 0a09 0909 0909 0965 6c69 6620 6b65 7920  .......elif key 
+0005b850: 696e 205b 2762 6f72 6465 7263 7574 272c  in ['bordercut',
+0005b860: 2774 696d 656c 696d 6974 7327 2c27 6669  'timelimits','fi
+0005b870: 7463 6f65 6666 272c 2773 6361 7474 6572  tcoeff','scatter
+0005b880: 6375 7427 5d3a 0d0a 0909 0909 0909 0972  cut']:.........r
+0005b890: 6561 643d 5b66 6c6f 6174 2861 2920 666f  ead=[float(a) fo
+0005b8a0: 7220 6120 696e 2072 6561 645d 0d0a 0909  r a in read]....
+0005b8b0: 0909 0909 656c 6966 206b 6579 203d 3d27  ....elif key =='
+0005b8c0: 696e 7465 6e73 6974 795f 7261 6e67 6527  intensity_range'
+0005b8d0: 3a0d 0a09 0909 0909 0909 7265 6164 3d5b  :.........read=[
+0005b8e0: 666c 6f61 7428 6129 2066 6f72 2061 2069  float(a) for a i
+0005b8f0: 6e20 7265 6164 5d0d 0a09 0909 0909 0965  n read]........e
+0005b900: 6c69 6620 6b65 7920 696e 205b 2772 656c  lif key in ['rel
+0005b910: 5f74 696d 6527 2c27 7265 6c5f 7761 7665  _time','rel_wave
+0005b920: 275d 3a0d 0a09 0909 0909 0909 7265 6164  ']:.........read
+0005b930: 3d6e 702e 6172 7261 7928 7265 6164 2c64  =np.array(read,d
+0005b940: 7479 7065 3d6e 702e 666c 6f61 7436 3429  type=np.float64)
+0005b950: 0d0a 0909 0909 0909 656c 6966 206b 6579  ........elif key
+0005b960: 2069 6e20 5b27 7363 6174 7465 7263 7574   in ['scattercut
+0005b970: 275d 3a0d 0a09 0909 0909 0909 7472 793a  ']:.........try:
+0005b980: 0d0a 0909 0909 0909 0909 7265 6164 3d5b  ..........read=[
+0005b990: 666c 6f61 7428 6129 2066 6f72 2061 2069  float(a) for a i
+0005b9a0: 6e20 7265 6164 5d0d 0a09 0909 0909 0909  n read].........
+0005b9b0: 6578 6365 7074 3a23 6d61 7962 6520 7765  except:#maybe we
+0005b9c0: 2068 6176 6520 2061 206c 6973 7420 6f66   have  a list of
+0005b9d0: 2073 6361 7474 6572 6375 7473 0d0a 0909   scattercuts....
+0005b9e0: 0909 0909 0909 7472 793a 0d0a 0909 0909  ......try:......
+0005b9f0: 0909 0909 096f 7574 5f6c 6973 7465 6e3d  .....out_listen=
+0005ba00: 5b5d 0d0a 0909 0909 0909 0909 0966 6f72  []...........for
+0005ba10: 206c 6973 7465 6e20 696e 2072 6561 643a   listen in read:
+0005ba20: 0d0a 0909 0909 0909 0909 0909 6f75 746c  ............outl
+0005ba30: 6973 7465 6e2e 6170 7065 6e64 285b 666c  isten.append([fl
+0005ba40: 6f61 7428 6129 2066 6f72 2061 2069 6e20  oat(a) for a in 
+0005ba50: 6c69 7374 656e 5d29 0d0a 0909 0909 0909  listen])........
+0005ba60: 0909 6578 6365 7074 3a23 6e6f 2069 6465  ..except:#no ide
+0005ba70: 6120 6c65 7473 2073 6565 2077 6861 7420  a lets see what 
+0005ba80: 6861 7070 656e 730d 0a09 0909 0909 0909  happens.........
+0005ba90: 0909 7061 7373 0d0a 0909 0909 0909 7365  ..pass........se
+0005baa0: 6c66 2e5f 5f64 6963 745f 5f5b 6b65 795d  lf.__dict__[key]
+0005bab0: 3d72 6561 640d 0a09 0909 0965 7863 6570  =read......excep
+0005bac0: 743a 2377 6527 6c6c 2067 6574 2061 6e20  t:#we'll get an 
+0005bad0: 6578 6365 7074 696f 6e20 6576 6572 7920  exception every 
+0005bae0: 7469 6d65 2074 6865 7265 2069 7320 616e  time there is an
+0005baf0: 2064 6174 6166 7261 6d65 0d0a 0909 0909   dataframe......
+0005bb00: 0923 7072 696e 7428 2746 7261 6d65 3a27  .#print('Frame:'
+0005bb10: 2b6b 6579 290d 0a09 0909 0909 6461 7461  +key).......data
+0005bb20: 5f66 7261 6d65 5f6c 6973 742e 6170 7065  _frame_list.appe
+0005bb30: 6e64 286b 6579 290d 0a0d 0a09 0974 7279  nd(key)......try
+0005bb40: 3a0d 0a09 0909 662e 636c 6f73 6528 290d  :.....f.close().
+0005bb50: 0a09 0965 7863 6570 743a 0d0a 0909 0970  ...except:.....p
+0005bb60: 6173 730d 0a09 0966 6f72 206b 6579 2069  ass....for key i
+0005bb70: 6e20 6461 7461 5f66 7261 6d65 5f6c 6973  n data_frame_lis
+0005bb80: 743a 0d0a 0909 0974 7279 3a0d 0a09 0909  t:.....try:.....
+0005bb90: 0969 6620 2272 655f 2220 696e 206b 6579  .if "re_" in key
+0005bba0: 5b3a 335d 3a0d 0a09 0909 0909 2370 7269  [:3]:.......#pri
+0005bbb0: 6e74 2827 7265 2069 6e20 6c69 7374 2729  nt('re in list')
+0005bbc0: 0d0a 0909 0909 0973 656c 662e 5f5f 6469  .......self.__di
+0005bbd0: 6374 5f5f 5b27 7265 275d 5b6b 6579 5b33  ct__['re'][key[3
+0005bbe0: 3a5d 5d3d 7061 6e64 6173 2e72 6561 645f  :]]=pandas.read_
+0005bbf0: 6864 6628 7361 7665 645f 7072 6f6a 6563  hdf(saved_projec
+0005bc00: 742c 6b65 793d 6b65 792c 6d6f 6465 3d27  t,key=key,mode='
+0005bc10: 7227 2c64 6174 615f 636f 6c75 6d6e 733d  r',data_columns=
+0005bc20: 5472 7565 290d 0a09 0909 0965 6c69 6620  True)......elif 
+0005bc30: 6b65 7920 696e 205b 2764 735f 6f72 6927  key in ['ds_ori'
+0005bc40: 2c27 7061 725f 6669 7427 2c27 7061 7227  ,'par_fit','par'
+0005bc50: 5d3a 0d0a 0909 0909 0973 656c 662e 5f5f  ]:.......self.__
+0005bc60: 6469 6374 5f5f 5b6b 6579 5d3d 7061 6e64  dict__[key]=pand
+0005bc70: 6173 2e72 6561 645f 6864 6628 7361 7665  as.read_hdf(save
+0005bc80: 645f 7072 6f6a 6563 742c 6b65 793d 6b65  d_project,key=ke
+0005bc90: 792c 6d6f 6465 3d27 7227 2c64 6174 615f  y,mode='r',data_
+0005bca0: 636f 6c75 6d6e 733d 5472 7565 290d 0a09  columns=True)...
+0005bcb0: 0909 0965 6c73 653a 0d0a 0909 0909 0970  ...else:.......p
+0005bcc0: 7269 6e74 2822 6d69 7373 696e 6720 6b65  rint("missing ke
+0005bcd0: 793a 2220 2b20 6b65 7929 0d0a 0909 0965  y:" + key).....e
+0005bce0: 7863 6570 743a 0d0a 0909 0909 6966 206b  xcept:......if k
+0005bcf0: 6579 203d 3d20 2770 6172 2720 616e 6420  ey == 'par' and 
+0005bd00: 6f6c 645f 7377 6974 6368 3a70 6173 7320  old_switch:pass 
+0005bd10: 2320 7765 2068 6176 6520 7265 6164 2069  # we have read i
+0005bd20: 7420 6265 666f 7265 2061 6c72 6561 6479  t before already
+0005bd30: 2061 6e64 2074 6865 2065 7272 6f72 2069   and the error i
+0005bd40: 7320 6f6b 0d0a 0909 200d 0a09 0909 0965  s ok.... ......e
+0005bd50: 6c73 653a 7072 696e 7428 2265 7272 6f72  lse:print("error
+0005bd60: 2069 6e20 6b65 793a 2220 2b20 6b65 7929   in key:" + key)
+0005bd70: 0d0a 0909 0d0a 0909 7472 793a 0d0a 0909  ........try:....
+0005bd80: 0973 656c 662e 5f5f 6469 6374 5f5f 5b27  .self.__dict__['
+0005bd90: 7265 275d 5b27 6669 745f 7265 7375 6c74  re']['fit_result
+0005bda0: 735f 7261 7465 7327 5d3d 7365 6c66 2e5f  s_rates']=self._
+0005bdb0: 5f64 6963 745f 5f5b 2770 6172 5f66 6974  _dict__['par_fit
+0005bdc0: 275d 0d0a 0909 0973 656c 662e 5f5f 6469  '].....self.__di
+0005bdd0: 6374 5f5f 5b27 7265 275d 5b27 6669 745f  ct__['re']['fit_
+0005bde0: 7265 7375 6c74 735f 7469 6d65 7327 5d3d  results_times']=
+0005bdf0: 7061 7264 665f 746f 5f74 696d 6564 6628  pardf_to_timedf(
+0005be00: 7365 6c66 2e5f 5f64 6963 745f 5f5b 2772  self.__dict__['r
+0005be10: 6527 5d5b 2766 6974 5f72 6573 756c 7473  e']['fit_results
+0005be20: 5f72 6174 6573 275d 290d 0a09 0965 7863  _rates'])....exc
+0005be30: 6570 743a 0d0a 0909 0970 6173 730d 0a09  ept:.....pass...
+0005be40: 090d 0a09 0923 7468 6520 7061 7220 636f  .....#the par co
+0005be50: 6e76 6572 7369 6f6e 2066 756e 6374 696f  nversion functio
+0005be60: 6e20 6661 696c 6564 2c20 7175 6963 6b66  n failed, quickf
+0005be70: 6978 0d0a 0909 666f 7220 6f76 6572 5f6b  ix....for over_k
+0005be80: 6579 2069 6e20 5b27 7061 725f 6669 7427  ey in ['par_fit'
+0005be90: 2c27 7061 7227 5d3a 0d0a 0909 0974 7279  ,'par']:.....try
+0005bea0: 3a0d 0a09 0909 0970 6172 5f64 663d 7365  :......par_df=se
+0005beb0: 6c66 2e5f 5f64 6963 745f 5f5b 6f76 6572  lf.__dict__[over
+0005bec0: 5f6b 6579 5d2e 6c6f 635b 3a2c 5b27 7661  _key].loc[:,['va
+0005bed0: 6c75 6527 2c27 6d69 6e27 2c27 6d61 7827  lue','min','max'
+0005bee0: 2c27 7661 7279 272c 2765 7870 7227 5d5d  ,'vary','expr']]
+0005bef0: 0d0a 0909 0909 7061 723d 6c6d 6669 742e  ......par=lmfit.
+0005bf00: 5061 7261 6d65 7465 7273 2829 0d0a 0909  Parameters()....
+0005bf10: 0909 666f 7220 6b65 7920 696e 2070 6172  ..for key in par
+0005bf20: 5f64 662e 696e 6465 782e 7661 6c75 6573  _df.index.values
+0005bf30: 3a0d 0a09 0909 0909 7061 722e 6164 6428  :.......par.add(
+0005bf40: 6b65 792c 2076 616c 7565 3d70 6172 5f64  key, value=par_d
+0005bf50: 662e 6c6f 635b 6b65 792c 2776 616c 7565  f.loc[key,'value
+0005bf60: 275d 2c20 7661 7279 3d70 6172 5f64 662e  '], vary=par_df.
+0005bf70: 6c6f 635b 6b65 792c 2776 6172 7927 5d2c  loc[key,'vary'],
+0005bf80: 206d 696e 3d70 6172 5f64 662e 6c6f 635b   min=par_df.loc[
+0005bf90: 6b65 792c 276d 696e 275d 2c20 6d61 783d  key,'min'], max=
+0005bfa0: 7061 725f 6466 2e6c 6f63 5b6b 6579 2c27  par_df.loc[key,'
+0005bfb0: 6d61 7827 5d29 0d0a 0909 0909 0909 0909  max'])..........
+0005bfc0: 0909 0909 0909 0920 200d 0a09 0909 0973  .......  ......s
+0005bfd0: 656c 662e 5f5f 6469 6374 5f5f 5b6f 7665  elf.__dict__[ove
+0005bfe0: 725f 6b65 795d 3d70 6172 0d0a 0909 0965  r_key]=par.....e
+0005bff0: 7863 6570 743a 0d0a 0909 0909 7061 7373  xcept:......pass
+0005c000: 0d0a 0909 6966 206f 6c64 5f73 7769 7463  ....if old_switc
+0005c010: 683a 0d0a 0909 0974 7279 3a0d 0a09 0909  h:.....try:.....
+0005c020: 0973 656c 662e 5f5f 6469 6374 5f5f 5b27  .self.__dict__['
+0005c030: 7265 275d 5b27 6669 745f 7265 7375 6c74  re']['fit_result
+0005c040: 735f 7261 7465 7327 5d3d 7061 725f 746f  s_rates']=par_to
+0005c050: 5f70 6172 6466 2873 656c 662e 7061 7229  _pardf(self.par)
+0005c060: 0d0a 0909 0909 7365 6c66 2e5f 5f64 6963  ......self.__dic
+0005c070: 745f 5f5b 2772 6527 5d5b 2766 6974 5f72  t__['re']['fit_r
+0005c080: 6573 756c 7473 5f74 696d 6573 275d 3d70  esults_times']=p
+0005c090: 6172 6466 5f74 6f5f 7469 6d65 6466 2870  ardf_to_timedf(p
+0005c0a0: 6172 5f74 6f5f 7061 7264 6628 7365 6c66  ar_to_pardf(self
+0005c0b0: 2e70 6172 2929 0d0a 0909 0909 7365 6c66  .par))......self
+0005c0c0: 2e5f 5f64 6963 745f 5f5b 2770 6172 5f66  .__dict__['par_f
+0005c0d0: 6974 275d 3d73 656c 662e 7061 720d 0a09  it']=self.par...
+0005c0e0: 0909 6578 6365 7074 3a0d 0a09 0909 0970  ..except:......p
+0005c0f0: 6173 730d 0a09 0973 656c 662e 7361 7665  ass....self.save
+0005c100: 5f66 6967 7572 6573 5f74 6f5f 666f 6c64  _figures_to_fold
+0005c110: 6572 3d46 616c 7365 0d0a 0909 7365 6c66  er=False....self
+0005c120: 2e70 6174 683d 6375 7272 656e 745f 7061  .path=current_pa
+0005c130: 7468 0d0a 0909 6966 206f 6c64 5f73 7769  th....if old_swi
+0005c140: 7463 683a 2363 6f6e 7665 7274 2070 726f  tch:#convert pro
+0005c150: 6a65 6374 2069 6e74 6f20 6e65 7720 7479  ject into new ty
+0005c160: 7065 0d0a 0909 0923 636c 6561 6e20 6f6c  pe.....#clean ol
+0005c170: 6420 6669 6c65 7320 7468 6174 2077 6572  d files that wer
+0005c180: 6520 7265 6164 2077 726f 6e67 0d0a 0909  e read wrong....
+0005c190: 0966 6f72 206b 6579 2069 6e20 5b27 7265  .for key in ['re
+0005c1a0: 5f66 696e 616c 5f69 6e74 5f70 6172 272c  _final_int_par',
+0005c1b0: 2772 655f 6669 6e61 6c5f 7365 7475 705f  're_final_setup_
+0005c1c0: 7061 7227 2c27 7265 5f66 696e 616c 5f74  par','re_final_t
+0005c1d0: 696d 655f 7061 7227 2c27 7265 5f69 6e74  ime_par','re_int
+0005c1e0: 5f65 7272 6f72 275d 3a0d 0a09 0909 0974  _error']:......t
+0005c1f0: 7279 3a0d 0a09 0909 0909 6465 6c20 7365  ry:.......del se
+0005c200: 6c66 2e5f 5f64 6963 745f 5f5b 6b65 795d  lf.__dict__[key]
+0005c210: 0d0a 0909 0909 6578 6365 7074 204b 6579  ......except Key
+0005c220: 4572 726f 723a 0d0a 0909 0909 0970 7269  Error:.......pri
+0005c230: 6e74 2866 274b 6579 207b 6b65 797d 2069  nt(f'Key {key} i
+0005c240: 7320 6e6f 7420 696e 2074 6865 2064 6963  s not in the dic
+0005c250: 7469 6f6e 6172 7927 290d 0a09 0909 666f  tionary').....fo
+0005c260: 7220 6b65 7920 696e 205b 2766 696e 616c  r key in ['final
+0005c270: 5f69 6e74 5f70 6172 272c 2766 696e 616c  _int_par','final
+0005c280: 5f73 6574 7570 5f70 6172 272c 2766 696e  _setup_par','fin
+0005c290: 616c 5f74 696d 655f 7061 7227 2c27 696e  al_time_par','in
+0005c2a0: 745f 6572 726f 7227 5d3a 0d0a 0909 0909  t_error']:......
+0005c2b0: 7472 793a 0d0a 0909 0909 0964 656c 2073  try:.......del s
+0005c2c0: 656c 662e 5f5f 6469 6374 5f5f 5b27 7265  elf.__dict__['re
+0005c2d0: 275d 5b6b 6579 5d0d 0a09 0909 0965 7863  '][key]......exc
+0005c2e0: 6570 7420 4b65 7945 7272 6f72 3a0d 0a09  ept KeyError:...
+0005c2f0: 0909 0909 7072 696e 7428 6627 4b65 7920  ....print(f'Key 
+0005c300: 7b6b 6579 7d20 6973 206e 6f74 2069 6e20  {key} is not in 
+0005c310: 7468 6520 6469 6374 696f 6e61 7279 2729  the dictionary')
+0005c320: 0d0a 0909 0974 7279 3a0d 0a09 0909 0973  .....try:......s
+0005c330: 656c 662e 7361 7665 5f70 726f 6a65 6374  elf.save_project
+0005c340: 2829 0d0a 0909 0909 7072 696e 7428 2270  ()......print("p
+0005c350: 726f 6a65 6374 2063 6f6e 7665 7274 6564  roject converted
+0005c360: 2069 6e74 6f20 6e65 7720 6461 7461 2074   into new data t
+0005c370: 7970 6520 616e 6420 7361 7665 6420 6167  ype and saved ag
+0005c380: 6169 6e22 290d 0a09 0909 6578 6365 7074  ain").....except
+0005c390: 3a0d 0a09 0909 0970 7269 6e74 2822 7072  :......print("pr
+0005c3a0: 6f6a 6563 7420 636f 6e76 6572 7465 6420  oject converted 
+0005c3b0: 6962 7574 2063 6f75 6c64 206e 6f74 2062  ibut could not b
+0005c3c0: 6520 7361 7665 6422 290d 0a09 0973 656c  e saved")....sel
+0005c3d0: 662e 7061 7468 3d63 7572 7265 6e74 5f70  f.path=current_p
+0005c3e0: 6174 680d 0a09 0966 6f72 206b 6579 2069  ath....for key i
+0005c3f0: 6e20 5b27 7469 6d65 5f62 696e 272c 2772  n ['time_bin','r
+0005c400: 656c 5f77 6176 6527 2c27 7265 6c5f 7469  el_wave','rel_ti
+0005c410: 6d65 272c 2773 6361 7474 6572 6375 7427  me','scattercut'
+0005c420: 2c27 626f 7264 6572 6375 7427 2c27 7469  ,'bordercut','ti
+0005c430: 6d65 6c69 6d69 7473 272c 2769 6e74 656e  melimits','inten
+0005c440: 7369 7479 5f72 616e 6765 272c 2777 6176  sity_range','wav
+0005c450: 655f 6e6d 5f62 696e 272c 2777 6176 656c  e_nm_bin','wavel
+0005c460: 656e 6774 685f 6269 6e27 2c27 6967 6e6f  ength_bin','igno
+0005c470: 7265 5f74 696d 655f 7265 6769 6f6e 275d  re_time_region']
+0005c480: 3a0d 0a09 0909 7472 793a 0d0a 0909 0909  :.....try:......
+0005c490: 6966 2069 7369 6e73 7461 6e63 6528 7365  if isinstance(se
+0005c4a0: 6c66 2e5f 5f64 6963 745f 5f5b 6b65 795d  lf.__dict__[key]
+0005c4b0: 2c62 7974 6573 293a 0d0a 0909 0909 0923  ,bytes):.......#
+0005c4c0: 7072 696e 7428 6b65 7920 2b20 2720 7365  print(key + ' se
+0005c4d0: 7420 746f 204e 6f6e 6527 290d 0a09 0909  t to None').....
+0005c4e0: 0909 7365 6c66 2e5f 5f64 6963 745f 5f5b  ..self.__dict__[
+0005c4f0: 6b65 795d 3d4e 6f6e 650d 0a09 0909 0965  key]=None......e
+0005c500: 6c69 6620 6973 696e 7374 616e 6365 2873  lif isinstance(s
+0005c510: 656c 662e 5f5f 6469 6374 5f5f 5b6b 6579  elf.__dict__[key
+0005c520: 5d2c 7374 7229 3a0d 0a09 0909 0909 6966  ],str):.......if
+0005c530: 2073 656c 662e 5f5f 6469 6374 5f5f 5b6b   self.__dict__[k
+0005c540: 6579 5d3d 3d27 4e6f 6e65 273a 0d0a 0909  ey]=='None':....
+0005c550: 0909 0909 7365 6c66 2e5f 5f64 6963 745f  ....self.__dict_
+0005c560: 5f5b 6b65 795d 3d4e 6f6e 650d 0a09 0909  _[key]=None.....
+0005c570: 6578 6365 7074 3a0d 0a09 0909 0963 6f6e  except:......con
+0005c580: 7469 6e75 650d 0a09 0974 7279 3a0d 0a09  tinue....try:...
+0005c590: 0909 7365 6c66 2e66 6967 7572 655f 7061  ..self.figure_pa
+0005c5a0: 7468 3d73 7472 2873 656c 662e 6669 6775  th=str(self.figu
+0005c5b0: 7265 5f70 6174 6829 0d0a 0909 0969 6620  re_path).....if 
+0005c5c0: 274e 6f6e 6527 2069 6e20 7365 6c66 2e66  'None' in self.f
+0005c5d0: 6967 7572 655f 7061 7468 3a0d 0a09 0909  igure_path:.....
+0005c5e0: 0973 656c 662e 6669 6775 7265 5f70 6174  .self.figure_pat
+0005c5f0: 683d 4e6f 6e65 0d0a 0909 6578 6365 7074  h=None....except
+0005c600: 3a0d 0a09 0909 7061 7373 0d0a 0d0a 0964  :.....pass.....d
+0005c610: 6566 2043 6f70 7928 7365 6c66 293a 0d0a  ef Copy(self):..
+0005c620: 0909 2727 2772 6574 7572 6e73 2061 2064  ..'''returns a d
+0005c630: 6565 7020 636f 7079 206f 6620 7468 6520  eep copy of the 
+0005c640: 6f62 6a65 6374 2e0d 0a09 090d 0a09 0945  object.........E
+0005c650: 7861 6d70 6c65 730d 0a09 092d 2d2d 2d2d  xamples....-----
+0005c660: 2d2d 2d0d 0a09 093e 3e3e 7461 3d70 6c6f  ---....>>>ta=plo
+0005c670: 745f 6675 6e63 2e54 4128 2774 6573 7466  t_func.TA('testf
+0005c680: 696c 652e 6864 6635 2729 2023 6f70 656e  ile.hdf5') #open
+0005c690: 2061 2070 726f 6a65 6374 0d0a 0909 3e3e   a project....>>
+0005c6a0: 3e74 6131 3d74 612e 436f 7079 2829 2023  >ta1=ta.Copy() #
+0005c6b0: 6d61 6b65 2061 2063 6f70 7920 666f 7220  make a copy for 
+0005c6c0: 736f 6d65 2074 6573 7473 206f 7220 6120  some tests or a 
+0005c6d0: 6469 6666 6572 6e65 7420 6669 740d 0a09  differnet fit...
+0005c6e0: 090d 0a09 0927 2727 200d 0a09 0969 6d70  .....''' ....imp
+0005c6f0: 6f72 7420 636f 7079 0d0a 0909 7265 7475  ort copy....retu
+0005c700: 726e 2063 6f70 792e 6465 6570 636f 7079  rn copy.deepcopy
+0005c710: 2873 656c 6629 0d0a 0d0a 0d0a 0964 6566  (self).......def
+0005c720: 2043 6f6d 7061 7265 5f61 745f 7469 6d65   Compare_at_time
+0005c730: 2873 656c 662c 2072 656c 5f74 696d 6520  (self, rel_time 
+0005c740: 3d20 4e6f 6e65 2c20 6f74 6865 7220 3d20  = None, other = 
+0005c750: 4e6f 6e65 2c20 6669 7474 6564 203d 2046  None, fitted = F
+0005c760: 616c 7365 2c20 6e6f 726d 5f77 696e 646f  alse, norm_windo
+0005c770: 7720 3d20 4e6f 6e65 2c0d 0a09 0909 0909  w = None,.......
+0005c780: 0974 696d 655f 7769 6474 685f 7065 7263  .time_width_perc
+0005c790: 656e 7420 3d20 4e6f 6e65 2c20 7370 6563  ent = None, spec
+0005c7a0: 7472 6120 3d20 4e6f 6e65 2c20 6461 7461  tra = None, data
+0005c7b0: 5f61 6e64 5f66 6974 203d 2046 616c 7365  _and_fit = False
+0005c7c0: 2c20 636d 6170 203d 204e 6f6e 6520 2c20  , cmap = None , 
+0005c7d0: 0d0a 0909 0909 0909 7072 696e 745f 636c  ........print_cl
+0005c7e0: 6963 6b5f 706f 7369 7469 6f6e 203d 2046  ick_position = F
+0005c7f0: 616c 7365 2c20 6c69 6e65 7769 6474 6820  alse, linewidth 
+0005c800: 3d20 312c 2074 6974 6c65 3d27 272c 2070  = 1, title='', p
+0005c810: 6c6f 745f 7365 636f 6e64 5f61 735f 656e  lot_second_as_en
+0005c820: 6572 6779 203d 2054 7275 6529 3a0d 0a09  ergy = True):...
+0005c830: 0927 2727 5468 6973 2066 756e 6374 696f  .'''This functio
+0005c840: 6e20 706c 6f74 7320 6d75 6c74 6970 6c65  n plots multiple
+0005c850: 2073 7065 6374 7261 2069 6e74 6f20 7468   spectra into th
+0005c860: 6520 7361 6d65 2066 6967 7572 6520 6174  e same figure at
+0005c870: 2061 2067 6976 656e 2072 656c 5f74 696d   a given rel_tim
+0005c880: 6520 2874 696d 6570 6f69 6e74 7329 2061  e (timepoints) a
+0005c890: 6e64 200d 0a09 0961 6c6c 6f77 7320 666f  nd ....allows fo
+0005c8a0: 7220 6e6f 726d 616c 697a 6174 696f 6e2e  r normalization.
+0005c8b0: 2056 6572 7920 7573 6566 756c 2074 6f20   Very useful to 
+0005c8c0: 636f 6d70 6172 6520 7468 6520 7370 6563  compare the spec
+0005c8d0: 7472 6120 666f 7220 6469 6666 6572 656e  tra for differen
+0005c8e0: 7420 736f 6c76 656e 7473 206f 7220 7175  t solvents or qu
+0005c8f0: 656e 6368 6572 732c 206f 720d 0a09 0965  enchers, or....e
+0005c900: 2e67 2e20 6469 6666 6572 656e 7420 6669  .g. different fi
+0005c910: 7473 2e20 5468 6520 7461 2e74 696d 655f  ts. The ta.time_
+0005c920: 7769 6474 685f 7065 7263 656e 7420 7061  width_percent pa
+0005c930: 7261 6d65 7465 7220 6465 6669 6e65 7320  rameter defines 
+0005c940: 6966 2074 6869 7320 6973 2061 0d0a 0909  if this is a....
+0005c950: 7369 6e67 6c65 2074 696d 6520 2869 6620  single time (if 
+0005c960: 7469 6d65 5f77 6964 7468 5f70 6572 6365  time_width_perce
+0005c970: 6e74 203d 2030 2920 6f72 2061 6e20 696e  nt = 0) or an in
+0005c980: 7465 6772 6174 6564 2077 696e 646f 772e  tegrated window.
+0005c990: 0d0a 0909 4f6e 6c79 2022 7265 6c5f 7469  ....Only "rel_ti
+0005c9a0: 6d65 2220 6973 2061 206d 616e 6461 746f  me" is a mandato
+0005c9b0: 7279 2c20 7468 6520 7265 7374 2063 616e  ry, the rest can
+0005c9c0: 2062 6520 7461 6b65 6e20 6672 6f6d 2074   be taken from t
+0005c9d0: 6865 206f 7269 6769 6e61 6c20 7072 6f6a  he original proj
+0005c9e0: 6563 7420 2874 6129 2e0d 0a09 090d 0a09  ect (ta)........
+0005c9f0: 0954 6865 206e 6f72 6d61 6c69 7a61 7469  .The normalizati
+0005ca00: 6f6e 2069 7320 7265 616c 697a 6564 2062  on is realized b
+0005ca10: 7920 6769 7669 6e67 2061 206e 6f72 6d5f  y giving a norm_
+0005ca20: 7769 6e64 6f77 200d 0a09 0961 7420 7768  window ....at wh
+0005ca30: 6963 6820 7468 6520 696e 7465 6e73 6974  ich the intensit
+0005ca40: 7920 696e 2074 6865 2074 7269 6767 6572  y in the trigger
+0005ca50: 696e 6720 6f62 6a65 6374 2069 7320 696e  ing object is in
+0005ca60: 7465 6772 6174 6564 2028 696e 2074 612e  tegrated (in ta.
+0005ca70: 436f 6d70 6172 655f 6174 5f74 696d 6528  Compare_at_time(
+0005ca80: 6f74 6865 722e 2e29 200d 0a09 0922 7461  other..) ...."ta
+0005ca90: 2220 6973 2074 6865 2074 7269 6767 6572  " is the trigger
+0005caa0: 696e 6720 6f62 6a65 6374 2e20 5468 6520  ing object. The 
+0005cab0: 696e 2065 6163 6820 6f66 2074 6865 206f  in each of the o
+0005cac0: 7468 6572 2063 7572 7665 7320 7468 6520  ther curves the 
+0005cad0: 7361 6d65 2077 696e 646f 7720 6973 0d0a  same window is..
+0005cae0: 0909 696e 7465 6772 6174 6564 2061 6e64  ..integrated and
+0005caf0: 2074 6865 2063 7572 7665 2073 6361 6c65   the curve scale
+0005cb00: 6420 6279 2074 6869 7320 7661 6c75 652e  d by this value.
+0005cb10: 2049 6d70 6f72 7461 6e74 2074 6f20 6e6f   Important to no
+0005cb20: 7465 2069 7320 7468 6174 2074 6869 7320  te is that this 
+0005cb30: 7769 6e64 6f77 0d0a 0909 646f 6573 206e  window....does n
+0005cb40: 6f74 206e 6565 6420 746f 2062 6520 696e  ot need to be in
+0005cb50: 2074 6865 2070 6c6f 742e 2065 2e67 2e20   the plot. e.g. 
+0005cb60: 7468 6520 6e6f 726d 616c 697a 6174 696f  the normalizatio
+0005cb70: 6e20 6361 6e20 6265 2064 6f6e 6520 6174  n can be done at
+0005cb80: 2061 2064 6966 6665 7265 6e74 2074 696d   a different tim
+0005cb90: 652e 0d0a 0909 0d0a 0909 5665 7279 206f  e.........Very o
+0005cba0: 6674 656e 206f 6e65 2077 6f75 6c64 206c  ften one would l
+0005cbb0: 696b 6520 746f 2063 6f6d 7061 7265 2074  ike to compare t
+0005cbc0: 6865 206d 6561 7375 7265 6420 7370 6563  he measured spec
+0005cbd0: 7472 6120 6174 2061 2063 6572 7461 696e  tra at a certain
+0005cbe0: 0d0a 0909 7469 6d65 2074 6f20 616e 2065  ....time to an e
+0005cbf0: 7874 6572 6e61 6c20 7370 6563 7472 756d  xternal spectrum
+0005cc00: 2028 652e 672e 2073 7065 6374 726f 2d65   (e.g. spectro-e
+0005cc10: 6c65 6374 726f 2d63 6865 6d69 7374 7279  lectro-chemistry
+0005cc20: 206f 7220 7374 6561 6479 0d0a 0909 7374   or steady....st
+0005cc30: 6174 6520 6162 736f 7270 7469 6f6e 292e  ate absorption).
+0005cc40: 2054 6869 7320 6361 6e20 6265 2064 6f6e   This can be don
+0005cc50: 6520 6279 206c 6f61 6469 6e67 2061 2073  e by loading a s
+0005cc60: 7065 6369 6669 6320 7370 6563 7472 756d  pecific spectrum
+0005cc70: 2069 6e74 6f0d 0a09 0961 2044 6174 6146   into....a DataF
+0005cc80: 7261 6d65 2061 6e64 2068 616e 6469 6e67  rame and handing
+0005cc90: 2074 6869 7320 6461 7461 2046 7261 6d65   this data Frame
+0005cca0: 2074 6f20 7468 6520 636f 6d70 6172 6973   to the comparis
+0005ccb0: 696f 6e20 6675 6e63 7469 6f6e 2e20 5468  ion function. Th
+0005ccc0: 650d 0a09 0966 756e 6374 696f 6e20 6361  e....function ca
+0005ccd0: 6e20 616c 736f 2062 6520 7573 6564 2074  n also be used t
+0005cce0: 6f20 706c 6f74 2065 2e67 2e20 7468 6520  o plot e.g. the 
+0005ccf0: 6d65 6173 7572 6564 2073 7065 6374 7261  measured spectra
+0005cd00: 2076 732e 2061 6e0d 0a09 0965 7874 6572   vs. an....exter
+0005cd10: 6e61 6c20 7370 6563 7472 756d 2077 6974  nal spectrum wit
+0005cd20: 686f 7574 2067 6976 696e 6720 616e 7920  hout giving any 
+0005cd30: 226f 7468 6572 2220 5072 6f6a 6563 7473  "other" Projects
+0005cd40: 2e20 2876 6572 7920 7573 6566 756c 2066  . (very useful f
+0005cd50: 6f72 0d0a 0909 636f 6d70 6172 6973 696f  or....comparisio
+0005cd60: 6e73 292e 0d0a 0909 200d 0a09 0950 6172  ns)..... ....Par
+0005cd70: 616d 6574 6572 730d 0a09 092d 2d2d 2d2d  ameters....-----
+0005cd80: 2d2d 2d2d 2d2d 2d2d 0d0a 0909 0d0a 0909  --------........
+0005cd90: 7265 6c5f 7469 6d65 203a 2066 6c6f 6174  rel_time : float
+0005cda0: 206f 7220 6c69 7374 2f76 6563 746f 7220   or list/vector 
+0005cdb0: 286f 6620 666c 6f61 7473 290d 0a09 0909  (of floats).....
+0005cdc0: 5370 6563 6966 7920 7468 6520 7469 6d65  Specify the time
+0005cdd0: 7320 7768 6572 6520 746f 2070 6c6f 742c  s where to plot,
+0005cde0: 2073 696e 676c 6520 7661 6c75 6520 6f72   single value or
+0005cdf0: 206c 6973 742f 7665 6374 6f72 206f 6620   list/vector of 
+0005ce00: 7661 6c75 6573 2e20 0d0a 0909 0946 6f72  values. .....For
+0005ce10: 2065 6163 6820 656e 7472 7920 696e 2072   each entry in r
+0005ce20: 656c 5f74 696d 6520 6120 7370 6563 7472  el_time a spectr
+0005ce30: 756d 2069 7320 706c 6f74 7465 642e 200d  um is plotted. .
+0005ce40: 0a09 0909 4966 2074 696d 655f 7769 6474  ....If time_widt
+0005ce50: 685f 7065 7263 656e 743d 3020 2844 6566  h_percent=0 (Def
+0005ce60: 6175 6c74 2920 7468 6520 6e65 6172 6573  ault) the neares
+0005ce70: 7420 6d65 6173 7572 6564 200d 0a09 0909  t measured .....
+0005ce80: 7469 6d65 706f 696e 7420 6973 2063 686f  timepoint is cho
+0005ce90: 7365 6e2e 2046 6f72 206f 7468 6572 2076  sen. For other v
+0005cea0: 616c 7565 7320 7365 6520 7061 7261 6d65  alues see parame
+0005ceb0: 7465 7220 2274 696d 655f 7769 6474 685f  ter "time_width_
+0005cec0: 7065 7263 656e 7422 2e0d 0a09 0909 0d0a  percent"........
+0005ced0: 0909 6f74 6865 7220 3a20 5441 206f 626a  ..other : TA obj
+0005cee0: 6563 7420 6f72 206c 6973 7420 6f66 2074  ect or list of t
+0005cef0: 686f 7365 2c20 6f70 7469 6f6e 616c 200d  hose, optional .
+0005cf00: 0a09 0909 7368 6f75 6c64 2062 6520 7461  ....should be ta
+0005cf10: 2e70 6c6f 745f 6675 6e63 206f 626a 6563  .plot_func objec
+0005cf20: 7473 2028 6c6f 6164 6564 206f 7220 636f  ts (loaded or co
+0005cf30: 7069 6564 2920 616e 6420 6973 2077 6861  pied) and is wha
+0005cf40: 7420 0d0a 0909 0969 7320 706c 6f74 7465  t .....is plotte
+0005cf50: 6420 6167 6169 6e73 7420 7468 6520 6461  d against the da
+0005cf60: 7461 2075 7365 2061 206c 6973 7420 5b74  ta use a list [t
+0005cf70: 6131 2c74 6132 2c2e 2e2e 205d 206f 7220  a1,ta2,... ] or 
+0005cf80: 6765 6e65 7261 7465 2074 6869 730d 0a09  generate this...
+0005cf90: 0909 6c69 7374 2075 7369 6e67 2074 6865  ..list using the
+0005cfa0: 2047 7569 2066 756e 6374 696f 6e2e 2053   Gui function. S
+0005cfb0: 6565 2073 6563 7469 6f6e 203a 7265 663a  ee section :ref:
+0005cfc0: 604f 7065 6e69 6e67 206d 756c 7469 706c  `Opening multipl
+0005cfd0: 6520 6669 6c65 7360 2069 6e20 0d0a 0909  e files` in ....
+0005cfe0: 0974 6865 2064 6f63 756d 656e 7461 7469  .the documentati
+0005cff0: 6f6e 0d0a 0909 0d0a 0909 6669 7474 6564  on........fitted
+0005d000: 203a 2062 6f6f 6c2c 206f 7074 696f 6e61   : bool, optiona
+0005d010: 6c0d 0a09 0909 5472 7565 2f46 616c 7365  l.....True/False
+0005d020: 2028 4465 6661 756c 7429 202d 2075 7365   (Default) - use
+0005d030: 2066 6974 7465 6420 6461 7461 2069 6e73   fitted data ins
+0005d040: 7465 6164 206f 6620 7261 7720 6461 7461  tead of raw data
+0005d050: 2e20 0d0a 0909 0949 6620 5472 7565 2c20  . .....If True, 
+0005d060: 7468 6520 6669 7474 6564 2064 6174 6170  the fitted datap
+0005d070: 6f69 6e74 7320 2877 6974 686f 7574 2069  oints (without i
+0005d080: 6e74 6572 706f 6c61 7469 6f6e 2920 6172  nterpolation) ar
+0005d090: 6520 7573 6564 2e20 0d0a 0909 0954 6869  e used. .....Thi
+0005d0a0: 7320 6973 2069 6e74 656e 6465 6420 666f  s is intended fo
+0005d0b0: 7220 636f 6d70 6172 696e 6720 652e 672e  r comparing e.g.
+0005d0c0: 2064 6966 6665 7265 6e74 2066 6974 730d   different fits.
+0005d0d0: 0a09 090d 0a09 096e 6f72 6d5f 7769 6e64  .......norm_wind
+0005d0e0: 6f77 203a 204e 6f6e 6520 6f72 206c 6973  ow : None or lis
+0005d0f0: 742f 7665 6374 6f72 2028 7769 7468 2034  t/vector (with 4
+0005d100: 2066 6c6f 6174 7329 2c20 6f70 7469 6f6e   floats), option
+0005d110: 616c 0d0a 0909 096e 6f72 6d5f 7769 6e64  al.....norm_wind
+0005d120: 6f77 2047 6976 6520 6120 6c69 7374 2f74  ow Give a list/t
+0005d130: 7570 656c 2f76 6563 746f 7220 7769 7468  upel/vector with
+0005d140: 2034 2065 6e74 7269 6573 2069 6e20 7468   4 entries in th
+0005d150: 6520 6f72 6465 7220 0d0a 0909 095b 5374  e order .....[St
+0005d160: 6172 7420 2d20 7469 6d65 2c20 456e 6420  art - time, End 
+0005d170: 2d20 7469 6d65 2c20 5374 6172 7420 2d20  - time, Start - 
+0005d180: 7761 7665 6c65 6e67 7468 2c20 456e 6420  wavelength, End 
+0005d190: 2d20 5761 7665 6c65 6e67 7468 5d2c 200d  - Wavelength], .
+0005d1a0: 0a09 0909 7365 6520 7365 6374 696f 6e20  ....see section 
+0005d1b0: 203a 7265 663a 604e 6f72 6d61 6c69 7a61   :ref:`Normaliza
+0005d1c0: 7469 6f6e 2061 6e64 2053 6361 6c69 6e67  tion and Scaling
+0005d1d0: 6020 2069 6e20 7468 6520 646f 6375 6d65  `  in the docume
+0005d1e0: 6e74 6174 696f 6e2e 0d0a 0909 0949 6620  ntation......If 
+0005d1f0: 4e6f 6e65 2028 4465 6661 756c 7429 206e  None (Default) n
+0005d200: 6f20 6e6f 726d 616c 697a 6174 696f 6e20  o normalization 
+0005d210: 6973 2064 6f6e 652e 0d0a 0909 0d0a 0909  is done.........
+0005d220: 6c69 6e65 7769 6474 6820 3a20 666c 6f61  linewidth : floa
+0005d230: 742c 206f 7074 696f 6e61 6c0d 0a09 0909  t, optional.....
+0005d240: 6c69 6e65 7769 6474 6820 746f 2062 6520  linewidth to be 
+0005d250: 7573 6564 2066 6f72 2070 6c6f 7474 696e  used for plottin
+0005d260: 6709 090d 0a09 090d 0a09 0974 696d 655f  g..........time_
+0005d270: 7769 6474 685f 7065 7263 656e 7420 3a20  width_percent : 
+0005d280: 4e6f 6e65 206f 7220 666c 6f61 742c 206f  None or float, o
+0005d290: 7074 696f 6e61 6c0d 0a09 0909 2272 656c  ptional....."rel
+0005d2a0: 5f74 696d 6522 2061 6e64 2022 7469 6d65  _time" and "time
+0005d2b0: 5f77 6964 7468 5f70 6572 6365 6e74 2220  _width_percent" 
+0005d2c0: 776f 726b 2074 6f67 6574 6865 7220 666f  work together fo
+0005d2d0: 7220 6372 6561 7469 6e67 2073 7065 6374  r creating spect
+0005d2e0: 7261 6c20 706c 6f74 7320 6174 200d 0a09  ral plots at ...
+0005d2f0: 0909 7370 6563 6966 6963 2074 696d 6570  ..specific timep
+0005d300: 6f69 6e74 732e 2046 6f72 2065 6163 6820  oints. For each 
+0005d310: 656e 7472 7920 696e 2072 656c 5f74 696d  entry in rel_tim
+0005d320: 6520 6120 7370 6563 7472 756d 2069 7320  e a spectrum is 
+0005d330: 706c 6f74 7465 642e 200d 0a09 0909 4966  plotted. .....If
+0005d340: 2068 6f77 6576 6572 2065 2e67 2e20 7469   however e.g. ti
+0005d350: 6d65 5f77 6964 7468 5f70 6572 6365 6e74  me_width_percent
+0005d360: 3d31 3020 7468 6520 7265 6769 6f6e 2062  =10 the region b
+0005d370: 6574 7765 656e 2074 6865 2074 696d 6570  etween the timep
+0005d380: 6f69 6e74 2063 6c6f 7365 7374 200d 0a09  oint closest ...
+0005d390: 0909 746f 203a 6d61 7468 3a60 7469 6d65  ..to :math:`time
+0005d3a0: 706f 696e 742b 302e 3178 7469 6d65 706f  point+0.1xtimepo
+0005d3b0: 696e 74c2 b420 616e 6420 3a6d 6174 683a  int.. and :math:
+0005d3c0: 6074 696d 6570 6f69 6e74 2d30 2e31 7874  `timepoint-0.1xt
+0005d3d0: 696d 6570 6f69 6e74 6020 6973 2061 7665  imepoint` is ave
+0005d3e0: 7261 6765 6420 616e 6420 7368 6f77 6e20  raged and shown 
+0005d3f0: 0d0a 0909 0928 616e 6420 7468 6520 6c65  .....(and the le
+0005d400: 6765 6e64 2061 646a 7573 7465 6420 6163  gend adjusted ac
+0005d410: 636f 7264 696e 676c 7929 2e20 4966 204e  cordingly). If N
+0005d420: 6f6e 6520 2844 6566 6175 6c74 2920 6973  one (Default) is
+0005d430: 2067 6976 656e 2c20 7468 6520 7661 6c75   given, the valu
+0005d440: 6520 6973 200d 0a09 0909 7461 6b65 6e20  e is .....taken 
+0005d450: 6672 6f6d 2074 6865 2074 7269 6767 6572  from the trigger
+0005d460: 696e 6720 6f62 6a65 6374 2028 7365 6c66  ing object (self
+0005d470: 2e74 696d 655f 7769 6474 685f 7065 7263  .time_width_perc
+0005d480: 656e 7429 2054 6869 7320 6973 2070 6172  ent) This is par
+0005d490: 7469 6375 6c61 726c 7920 7573 6566 756c  ticularly useful
+0005d4a0: 2066 6f72 2074 6865 2064 656e 736c 790d   for the densly.
+0005d4b0: 0a09 0909 7361 6d70 6c65 6420 7265 6769  ....sampled regi
+0005d4c0: 6f6e 2063 6c6f 7365 2074 6f20 743d 302e  on close to t=0.
+0005d4d0: 2054 7970 6963 616c 6c79 2066 6f72 2061   Typically for a
+0005d4e0: 206c 6f67 6172 6974 686d 6963 2072 6563   logarithmic rec
+0005d4f0: 6f72 6465 6420 6b69 6e65 7469 6373 2c20  orded kinetics, 
+0005d500: 7468 6520 0d0a 0909 0974 696d 6570 6f69  the .....timepoi
+0005d510: 6e74 7320 6174 206c 6174 6572 2074 696d  nts at later tim
+0005d520: 6573 2077 696c 6c20 6265 2066 7572 7468  es will be furth
+0005d530: 6572 2061 7070 6172 7420 7468 616e 2031  er appart than 1
+0005d540: 3020 7065 7263 656e 7420 6f66 2074 6865  0 percent of the
+0005d550: 2076 616c 7565 2c20 0d0a 0909 0962 7574   value, .....but
+0005d560: 2074 6869 7320 616c 6c6f 7773 2074 6f20   this allows to 
+0005d570: 656c 6567 616e 746c 7920 636f 6d62 696e  elegantly combin
+0005d580: 6520 7661 6c75 6573 2061 726f 756e 6420  e values around 
+0005d590: 7469 6d65 3d30 2066 6f72 2062 6574 7465  time=0 for bette
+0005d5a0: 7220 7374 6174 6973 7469 6373 2e20 0d0a  r statistics. ..
+0005d5b0: 0909 0954 6869 7320 6176 6572 6167 696e  ...This averagin
+0005d5c0: 6720 6973 206f 6e6c 7920 6170 706c 6965  g is only applie
+0005d5d0: 6420 666f 7220 7468 6520 706c 6f74 7469  d for the plotti
+0005d5e0: 6e67 2066 756e 6374 696f 6e20 616e 6420  ng function and 
+0005d5f0: 6e6f 7420 666f 7220 7468 6520 6669 7473  not for the fits
+0005d600: 2e0d 0a09 090d 0a09 0973 7065 6374 7261  .........spectra
+0005d610: 203a 204e 6f6e 6520 6f72 2044 6174 6146   : None or DataF
+0005d620: 7261 6d65 2c20 6f70 7469 6f6e 616c 0d0a  rame, optional..
+0005d630: 0909 0949 6620 616e 2044 6174 6146 7261  ...If an DataFra
+0005d640: 6d65 2077 6974 6820 7468 6520 7761 7665  me with the wave
+0005d650: 6c65 6e67 7468 2061 7320 696e 6465 7820  length as index 
+0005d660: 6973 2070 726f 7669 6465 642c 2054 6865  is provided, The
+0005d670: 6e20 7468 6520 7370 6563 7472 6120 6f66  n the spectra of
+0005d680: 2065 6163 6820 636f 6c75 6d6e 0d0a 0909   each column....
+0005d690: 0969 7320 706c 6f74 7465 6420 696e 746f  .is plotted into
+0005d6a0: 2074 6865 2064 6966 6665 7265 6e74 6961   the differentia
+0005d6b0: 6c20 7370 6563 7472 6120 312d 3120 616e  l spectra 1-1 an
+0005d6c0: 6420 7468 6520 636f 6c75 6d6e 206e 616d  d the column nam
+0005d6d0: 6573 2061 7265 2075 7365 6420 696e 2074  es are used in t
+0005d6e0: 6865 206c 6567 656e 640d 0a09 0909 5072  he legend.....Pr
+0005d6f0: 696f 7220 7363 616c 696e 6720 6973 2068  ior scaling is h
+0005d700: 6967 686c 7920 7375 6767 6573 7465 642e  ighly suggested.
+0005d710: 2054 6865 7365 2073 7065 6374 7261 2061   These spectra a
+0005d720: 7265 206e 6f74 2028 696e 2067 656e 6572  re not (in gener
+0005d730: 616c 2920 7363 616c 6564 2077 6974 6820  al) scaled with 
+0005d740: 7468 6520 0d0a 0909 096e 6f72 6d20 7769  the .....norm wi
+0005d750: 6e64 6f77 2e20 2873 6565 2065 7861 6d70  ndow. (see examp
+0005d760: 6c65 7329 2e0d 0a09 090d 0a09 0964 6174  les).........dat
+0005d770: 615f 616e 645f 6669 7420 3a20 626f 6f6c  a_and_fit : bool
+0005d780: 2c20 6f70 7469 6f6e 616c 0d0a 0909 0954  , optional.....T
+0005d790: 7275 6520 6f72 2046 616c 7365 2028 4465  rue or False (De
+0005d7a0: 6661 756c 7429 2c20 6368 6f6f 7365 2069  fault), choose i
+0005d7b0: 6620 666f 7220 7468 6520 4669 7474 6564  f for the Fitted
+0005d7c0: 2070 6c6f 7420 7468 6520 7261 7720 6461   plot the raw da
+0005d7d0: 7461 206f 6620 7468 6520 0d0a 0909 096f  ta of the .....o
+0005d7e0: 7468 6572 2070 726f 6a65 6374 7320 6973  ther projects is
+0005d7f0: 2074 6f20 6265 2070 6c6f 7474 696e 6720   to be plotting 
+0005d800: 696e 2061 6464 6974 696f 6e20 746f 2074  in addition to t
+0005d810: 6865 2066 6974 7465 6420 6c69 6e65 2e20  he fitted line. 
+0005d820: 466f 7220 4661 6c73 6520 2844 6566 6175  For False (Defau
+0005d830: 6c74 290d 0a09 0909 4f6e 6c79 2074 6865  lt).....Only the
+0005d840: 2066 6974 2069 7320 706c 6f74 7465 642e   fit is plotted.
+0005d850: 200d 0a09 090d 0a09 0963 6d61 7020 3a20   ........cmap : 
+0005d860: 4e6f 6e65 206f 7220 6d61 7470 6c6f 746c  None or matplotl
+0005d870: 6962 2063 6f6c 6f72 206d 6170 2c20 6f70  ib color map, op
+0005d880: 7469 6f6e 616c 0d0a 0909 0969 7320 6120  tional.....is a 
+0005d890: 706f 7765 7266 756c 6c20 7661 7269 6162  powerfull variab
+0005d8a0: 6c65 2074 6861 7420 6368 6f6f 7365 7320  le that chooses 
+0005d8b0: 7468 6520 636f 6c6f 7572 206d 6170 2061  the colour map a
+0005d8c0: 7070 6c69 6564 2066 6f72 2061 6c6c 2070  pplied for all p
+0005d8d0: 6c6f 7473 2e20 4966 2073 6574 2074 6f20  lots. If set to 
+0005d8e0: 0d0a 0909 094e 6f6e 6520 2844 6566 6175  .....None (Defau
+0005d8f0: 6c74 2920 7468 656e 2074 6865 2073 656c  lt) then the sel
+0005d900: 662e 636d 6170 2069 7320 7573 6564 2e0d  f.cmap is used..
+0005d910: 0a09 0909 4173 2073 7461 6e64 6172 6420  ....As standard 
+0005d920: 4920 7573 6520 7468 6520 636f 6c6f 7220  I use the color 
+0005d930: 6d61 7020 226a 6574 2220 6672 6f6d 206d  map "jet" from m
+0005d940: 6174 706c 6f74 6c69 622e 2054 6865 7265  atplotlib. There
+0005d950: 2061 7265 2061 2076 6172 6965 7479 206f   are a variety o
+0005d960: 6620 636f 6c6f 726d 6170 7320 0d0a 0909  f colormaps ....
+0005d970: 0961 7661 696c 6162 6c65 2074 6861 7420  .available that 
+0005d980: 6172 6520 7665 7279 2075 7365 6675 6c6c  are very usefull
+0005d990: 2e20 4265 7369 6465 2022 6a65 7422 2c20  . Beside "jet", 
+0005d9a0: 2276 6972 6964 6973 2220 6973 2061 2067  "viridis" is a g
+0005d9b0: 6f6f 6420 6368 6f69 6365 2061 7320 6974  ood choice as it
+0005d9c0: 2069 7320 7765 6c6c 200d 0a09 0909 7669   is well .....vi
+0005d9d0: 7369 626c 6520 756e 6465 7220 7265 642d  sible under red-
+0005d9e0: 6772 6565 6e20 626c 696e 646e 6573 732e  green blindness.
+0005d9f0: 204f 7468 6572 2075 7365 6675 6c20 6d61   Other useful ma
+0005da00: 7073 2061 7265 2022 7072 6973 6d22 2066  ps are "prism" f
+0005da10: 6f72 2068 6967 6820 666c 7563 7475 6174  or high fluctuat
+0005da20: 696f 6e73 200d 0a09 0909 6f72 2064 6976  ions .....or div
+0005da30: 6572 6769 6e67 2063 6f6c 6f72 206d 6170  erging color map
+0005da40: 7320 6c69 6b65 2022 7365 6973 6d69 6322  s like "seismic"
+0005da50: 2e20 0d0a 0909 0953 6565 2068 7474 7073  . .....See https
+0005da60: 3a2f 2f6d 6174 706c 6f74 6c69 622e 6f72  ://matplotlib.or
+0005da70: 672f 332e 312e 302f 7475 746f 7269 616c  g/3.1.0/tutorial
+0005da80: 732f 636f 6c6f 7273 2f63 6f6c 6f72 6d61  s/colors/colorma
+0005da90: 7073 2e68 746d 6c20 666f 7220 6120 636f  ps.html for a co
+0005daa0: 6d70 7265 6865 6e73 6976 6520 0d0a 0909  mprehensive ....
+0005dab0: 0973 656c 6563 7469 6f6e 2e20 496e 2074  .selection. In t
+0005dac0: 6865 2063 6f64 6520 7468 6520 636f 6c6f  he code the colo
+0005dad0: 726d 6170 7320 6172 6520 696d 706f 7274  rmaps are import
+0005dae0: 6564 2073 6f20 6966 2070 6c6f 745f 6675  ed so if plot_fu
+0005daf0: 6e63 2069 7320 696d 706f 7274 6564 2061  nc is imported a
+0005db00: 7320 7066 2074 6865 6e20 0d0a 0909 0973  s pf then .....s
+0005db10: 656c 662e 636d 6170 3d70 662e 636d 2e76  elf.cmap=pf.cm.v
+0005db20: 6972 6964 6973 2073 6574 7320 7669 7269  iridis sets viri
+0005db30: 6469 7320 6173 2074 6865 206d 6170 2074  dis as the map t
+0005db40: 6f20 7573 652e 2049 6e74 6572 6e61 6c6c  o use. Internall
+0005db50: 7920 7468 6520 636f 6c6f 7273 2061 7265  y the colors are
+0005db60: 2063 686f 7365 6e20 0d0a 0909 0977 6974   chosen .....wit
+0005db70: 6820 7468 6520 2263 6f6c 6d22 2066 756e  h the "colm" fun
+0005db80: 6374 696f 6e2e 2054 6865 2032 6420 706c  ction. The 2d pl
+0005db90: 6f74 7320 7265 7175 6972 6520 6120 636f  ots require a co
+0005dba0: 6e74 696e 756f 7573 2063 6f6c 6f72 206d  ntinuous color m
+0005dbb0: 6170 2073 6f20 6966 2073 6f6d 6574 6869  ap so if somethi
+0005dbc0: 6e67 200d 0a09 0909 656c 7365 2069 7320  ng .....else is 
+0005dbd0: 6769 7665 2032 6420 706c 6f74 7320 6172  give 2d plots ar
+0005dbe0: 6520 7368 6f77 6e20 6175 746f 6d61 7469  e shown automati
+0005dbf0: 6361 6c6c 7920 7769 7468 2022 6a65 7422  cally with "jet"
+0005dc00: 2e20 466f 7220 616c 6c20 6f66 2074 6865  . For all of the
+0005dc10: 2031 6420 706c 6f74 7320 686f 7765 7665   1d plots howeve
+0005dc20: 7220 0d0a 0909 0949 2066 6972 7374 2073  r .....I first s
+0005dc30: 656c 6563 7420 6120 6e75 6d62 6572 206f  elect a number o
+0005dc40: 6620 636f 6c6f 7273 2062 6566 6f72 6520  f colors before 
+0005dc50: 6561 6368 2070 6c6f 742e 2049 6620 636d  each plot. If cm
+0005dc60: 6170 2069 7320 6120 636f 6e74 696e 6f75  ap is a continou
+0005dc70: 7320 6d61 7020 7468 656e 2074 6865 7365  s map then these
+0005dc80: 0d0a 0909 0961 7265 2073 616d 706c 6564  .....are sampled
+0005dc90: 2065 7665 6e6c 7920 6f76 6572 2074 6865   evenly over the
+0005dca0: 2063 6f6c 6f75 726d 6170 2e20 4d61 6e75   colourmap. Manu
+0005dcb0: 616c 2069 7465 7261 626c 6573 206f 6620  al iterables of 
+0005dcc0: 636f 6c6f 7572 7320 0d0a 0909 0963 6d61  colours .....cma
+0005dcd0: 703d 5b28 312c 302c 3029 2c28 302c 312c  p=[(1,0,0),(0,1,
+0005dce0: 3029 2c28 302c 302c 3129 2c2e 2e2e 5d20  0),(0,0,1),...] 
+0005dcf0: 6172 6520 616c 736f 2061 6363 6570 7465  are also accepte
+0005dd00: 642c 2061 7320 6172 6520 7665 6374 6f72  d, as are vector
+0005dd10: 7320 6f72 2064 6174 6166 7261 6d65 7320  s or dataframes 
+0005dd20: 7468 6174 200d 0a09 0909 636f 6e74 6169  that .....contai
+0005dd30: 6e20 6173 2072 6f77 7320 7468 6520 636f  n as rows the co
+0005dd40: 6c6f 7273 2e20 5468 6572 6520 6d75 7374  lors. There must
+0005dd50: 2062 6520 6f66 2063 6f75 7273 6520 7375   be of course su
+0005dd60: 6666 6963 6965 6e74 2063 6f6c 6f72 7320  fficient colors 
+0005dd70: 7072 6573 656e 7420 666f 7220 0d0a 0909  present for ....
+0005dd80: 0974 6865 206e 756d 6265 7273 206f 6620  .the numbers of 
+0005dd90: 6c69 6e65 7320 7468 6174 2077 696c 6c20  lines that will 
+0005dda0: 6265 2070 6c6f 7474 6564 2e20 536f 2049  be plotted. So I
+0005ddb0: 2072 6563 6f6d 6d65 6e64 2074 6f20 7072   recommend to pr
+0005ddc0: 6f76 6964 6520 6174 206c 6561 7374 2031  ovide at least 1
+0005ddd0: 3020 636f 6c6f 7572 7320 0d0a 0909 0928  0 colours .....(
+0005dde0: 652e 672e 7e79 6f75 7220 756e 6976 6572  e.g.~your univer
+0005ddf0: 7369 7479 2063 6f6c 6f72 7329 2e20 636f  sity colors). co
+0005de00: 6c6f 7572 7320 6172 6520 616c 7761 7973  lours are always
+0005de10: 2067 6976 656e 2061 7320 612c 206c 6973   given as a, lis
+0005de20: 7420 6f72 2074 7570 6c65 2077 6974 6820  t or tuple with 
+0005de30: 5247 4120 6f72 2052 4742 410d 0a09 0909  RGA or RGBA.....
+0005de40: 2877 6974 6820 7468 6520 6c61 7374 2041  (with the last A
+0005de50: 2062 6565 696e 6720 7468 6520 416c 7068   beeing the Alph
+0005de60: 613d 7472 616e 7370 6172 656e 6379 2e20  a=transparency. 
+0005de70: 416c 6c20 6e75 6d62 6572 7320 6172 6520  All numbers are 
+0005de80: 6265 7477 6565 6e20 3020 616e 6420 312e  between 0 and 1.
+0005de90: 200d 0a09 0909 4966 2061 206c 6973 742f   .....If a list/
+0005dea0: 7665 6374 6f72 2f44 6174 6146 7261 6d65  vector/DataFrame
+0005deb0: 2069 7320 6769 7665 6e20 666f 7220 7468   is given for th
+0005dec0: 6520 636f 6c6f 7572 7320 7468 6579 2077  e colours they w
+0005ded0: 696c 6c20 6265 2075 7365 6420 696e 2074  ill be used in t
+0005dee0: 6865 206f 7264 6572 2070 726f 7669 6465  he order provide
+0005def0: 642e 0d0a 0909 706c 6f74 5f73 6563 6f6e  d.....plot_secon
+0005df00: 645f 6173 5f65 6e65 7267 7920 3a20 626f  d_as_energy : bo
+0005df10: 6f6c 2c20 6f70 7469 6f6e 616c 0d0a 0909  ol, optional....
+0005df20: 0946 6f72 2028 4465 6661 756c 7429 2054  .For (Default) T
+0005df30: 7275 6520 6120 7365 636f 6e64 2078 2d61  rue a second x-a
+0005df40: 7869 7320 6973 2070 6c6f 7474 6564 2020  xis is plotted  
+0005df50: 7769 7468 2022 6556 2220 6173 2075 6e69  with "eV" as uni
+0005df60: 740d 0a0d 0a09 0970 7269 6e74 5f63 6c69  t......print_cli
+0005df70: 636b 5f70 6f73 6974 696f 6e20 3a20 626f  ck_position : bo
+0005df80: 6f6c 2c20 6f70 7469 6f6e 616c 0d0a 0909  ol, optional....
+0005df90: 0969 6620 5472 7565 2074 6865 6e20 7468  .if True then th
+0005dfa0: 6520 636c 6963 6b20 706f 7369 7469 6f6e  e click position
+0005dfb0: 2069 7320 7072 696e 7465 6420 666f 7220   is printed for 
+0005dfc0: 7468 6520 7370 6563 7472 616c 2070 6c6f  the spectral plo
+0005dfd0: 7473 200d 0a0d 0a09 0945 7861 6d70 6c65  ts ......Example
+0005dfe0: 730d 0a09 092d 2d2d 2d2d 2d2d 2d2d 2d0d  s....----------.
+0005dff0: 0a09 090d 0a09 093e 3e3e 2069 6d70 6f72  .......>>> impor
+0005e000: 7420 706c 6f74 5f66 756e 6320 6173 2070  t plot_func as p
+0005e010: 660d 0a09 093e 3e3e 2074 6120 3d20 7066  f....>>> ta = pf
+0005e020: 2e54 4128 2274 6573 7431 2e68 6466 3522  .TA("test1.hdf5"
+0005e030: 2920 236f 7065 6e20 7468 6520 6f72 6967  ) #open the orig
+0005e040: 696e 616c 2070 726f 6a65 6374 0d0a 0909  inal project....
+0005e050: 0d0a 0909 4e6f 7720 6f70 656e 2061 2062  ....Now open a b
+0005e060: 756e 6368 206f 6620 6f74 6865 7220 706f  unch of other po
+0005e070: 726a 6563 7473 2074 6f20 636f 6d61 7265  rjects to comare
+0005e080: 2061 6761 696e 7374 0d0a 0909 0d0a 0909   against........
+0005e090: 3e3e 3e20 6f74 6865 725f 7072 6f6a 6563  >>> other_projec
+0005e0a0: 7473 203d 2070 662e 4755 495f 6f70 656e  ts = pf.GUI_open
+0005e0b0: 2870 726f 6a65 6374 5f6c 6973 7420 3d20  (project_list = 
+0005e0c0: 5b22 6669 6c65 312e 5349 4122 2c20 2266  ["file1.SIA", "f
+0005e0d0: 696c 6532 2e53 4941 225d 290d 0a09 090d  ile2.SIA"]).....
+0005e0e0: 0a09 0954 7970 6963 616c 2075 7365 2069  ...Typical use i
+0005e0f0: 7320 636f 6d70 6172 6520 7468 6520 7261  s compare the ra
+0005e100: 7720 6461 7461 2077 6974 686f 7574 206e  w data without n
+0005e110: 6f72 6d61 6c69 7a61 7469 6f6e 2061 7420  ormalization at 
+0005e120: 3170 7320 616e 6420 3670 732e 0d0a 0909  1ps and 6ps.....
+0005e130: 0d0a 0909 3e3e 3e20 7461 2e43 6f6d 7061  ....>>> ta.Compa
+0005e140: 7265 5f61 745f 7469 6d65 2872 656c 5f74  re_at_time(rel_t
+0005e150: 696d 6520 3d20 5b31 2c36 5d2c 206f 7468  ime = [1,6], oth
+0005e160: 6572 7320 3d20 6f74 6865 725f 7072 6f6a  ers = other_proj
+0005e170: 6563 7429 0d0a 0909 0d0a 0909 436f 6d70  ect)........Comp
+0005e180: 6172 6520 7468 6520 6669 7420 7769 7468  are the fit with
+0005e190: 7075 7420 6e6f 726d 616c 697a 6174 696f  put normalizatio
+0005e1a0: 6e20 6174 2031 7073 2061 6e64 2036 7073  n at 1ps and 6ps
+0005e1b0: 2e0d 0a09 090d 0a09 093e 3e3e 2074 612e  .........>>> ta.
+0005e1c0: 436f 6d70 6172 655f 6174 5f74 696d 6528  Compare_at_time(
+0005e1d0: 7265 6c5f 7469 6d65 203d 205b 312c 365d  rel_time = [1,6]
+0005e1e0: 2c20 6f74 6865 7273 203d 206f 7468 6572  , others = other
+0005e1f0: 5f70 726f 6a65 6374 2c20 6669 7474 6564  _project, fitted
+0005e200: 203d 2054 7275 6529 0d0a 0909 0d0a 0909   = True)........
+0005e210: 436f 6d70 6172 6520 7769 7468 206e 6f72  Compare with nor
+0005e220: 6d61 6c69 7a61 7469 6f6e 2077 696e 646f  malization windo
+0005e230: 7720 6265 7477 6565 6e20 3170 7320 616e  w between 1ps an
+0005e240: 6420 3270 7320 616e 6420 3430 306e 6d20  d 2ps and 400nm 
+0005e250: 616e 6420 3435 306e 6d2e 0d0a 0909 0d0a  and 450nm.......
+0005e260: 0909 3e3e 3e20 6e6f 726d 5f77 696e 646f  ..>>> norm_windo
+0005e270: 773d 5b31 2c32 2c34 3030 2c34 3530 5d0d  w=[1,2,400,450].
+0005e280: 0a09 093e 3e3e 2074 612e 436f 6d70 6172  ...>>> ta.Compar
+0005e290: 655f 6174 5f74 696d 6528 7265 6c5f 7469  e_at_time(rel_ti
+0005e2a0: 6d65 203d 205b 312c 365d 2c20 6f74 6865  me = [1,6], othe
+0005e2b0: 7273 203d 206f 7468 6572 5f70 726f 6a65  rs = other_proje
+0005e2c0: 6374 2c20 6e6f 726d 5f77 696e 646f 7720  ct, norm_window 
+0005e2d0: 3d20 6e6f 726d 5f77 696e 646f 7729 0d0a  = norm_window)..
+0005e2e0: 0909 0d0a 0909 436f 6d70 6172 6520 7468  ......Compare th
+0005e2f0: 6520 7370 6563 7472 756d 2061 7420 3170  e spectrum at 1p
+0005e300: 7320 616e 6420 3670 7320 7769 7468 2061  s and 6ps with a
+0005e310: 6e20 6578 7465 726e 616c 2073 7065 6374  n external spect
+0005e320: 7275 6d2e 0d0a 0909 0d0a 0909 3e3e 3e20  rum.........>>> 
+0005e330: 6578 745f 7370 6563 203d 2070 642e 7265  ext_spec = pd.re
+0005e340: 6164 5f63 7376 2822 4173 6369 695f 7370  ad_csv("Ascii_sp
+0005e350: 6563 7472 756d 2e64 6174 222c 2073 6570  ectrum.dat", sep
+0005e360: 203d 2022 2c22 290d 0a09 093e 3e3e 2074   = ",")....>>> t
+0005e370: 612e 436f 6d70 6172 655f 6174 5f74 696d  a.Compare_at_tim
+0005e380: 6528 7265 6c5f 7469 6d65 203d 205b 312c  e(rel_time = [1,
+0005e390: 365d 2c20 7370 6563 7472 6120 3d20 6578  6], spectra = ex
+0005e3a0: 745f 7370 6563 290d 0a0d 0a09 0955 7365  t_spec)......Use
+0005e3b0: 2065 7861 6d70 6c65 202d 2020 4f66 7465   example -  Ofte
+0005e3c0: 6e20 7468 6572 6520 6172 6520 6120 6c6f  n there are a lo
+0005e3d0: 7420 6f66 2064 6966 6665 7265 6e74 206d  t of different m
+0005e3e0: 6561 7375 7265 6d65 6e74 7320 746f 200d  easurements to .
+0005e3f0: 0a09 0963 6f6d 7061 7265 2061 7420 6d75  ...compare at mu
+0005e400: 6c74 6970 6c65 2074 696d 652e 2054 6865  ltiple time. The
+0005e410: 206e 6f72 6d6c 697a 6174 696f 6e20 6973   normlization is
+0005e420: 2070 6572 666f 726d 6564 2061 7420 7468   performed at th
+0005e430: 6520 6772 6f75 6e64 2073 7461 7465 2062  e ground state b
+0005e440: 6c65 6163 680d 0a09 0934 3630 206e 6d20  leach....460 nm 
+0005e450: 616e 6420 6561 726c 7920 696e 2074 696d  and early in tim
+0005e460: 652e 2054 6865 6e20 6974 2069 7320 6265  e. Then it is be
+0005e470: 7474 6572 2074 6f20 6d61 6b65 2061 206e  tter to make a n
+0005e480: 6577 2070 6c6f 7420 666f 7220 6561 6368  ew plot for each
+0005e490: 200d 0a09 0974 696d 6570 6f69 6e74 2e20   ....timepoint. 
+0005e4a0: 5468 6520 6e6f 726d 616c 697a 6174 696f  The normalizatio
+0005e4b0: 6e20 7769 6e64 6f77 2073 7461 7973 2066  n window stays f
+0005e4c0: 6978 6564 2e0d 0a09 090d 0a09 093e 3e3e  ixed.........>>>
+0005e4d0: 2070 6c74 2e63 6c6f 7365 2822 616c 6c22   plt.close("all"
+0005e4e0: 2920 236d 616b 6520 736f 6d65 2073 7061  ) #make some spa
+0005e4f0: 6365 0d0a 0909 3e3e 3e20 6e6f 726d 5f77  ce....>>> norm_w
+0005e500: 696e 646f 773d 5b30 2e33 2c30 2e35 2c34  indow=[0.3,0.5,4
+0005e510: 3530 2c34 3730 5d20 2364 6566 696e 6520  50,470] #define 
+0005e520: 7769 6e64 6f77 2069 6e20 6772 6f75 6e64  window in ground
+0005e530: 2073 7461 7465 2062 6c65 6163 680d 0a09   state bleach...
+0005e540: 093e 3e3e 2066 6f72 2074 2069 6e20 5b30  .>>> for t in [0
+0005e550: 2e33 2c30 2e35 2c31 2c33 2c31 302c 3330  .3,0.5,1,3,10,30
+0005e560: 5d3a 2023 6974 6572 6174 6520 6f76 6572  ]: #iterate over
+0005e570: 2074 6865 2077 6176 656c 656e 6774 6820   the wavelength 
+0005e580: 0d0a 0909 3e3e 3e20 0974 612e 436f 6d70  ....>>> .ta.Comp
+0005e590: 6172 655f 6174 5f74 696d 6528 7265 6c5f  are_at_time(rel_
+0005e5a0: 7469 6d65 203d 2074 2c20 6f74 6865 7273  time = t, others
+0005e5b0: 203d 206f 7468 6572 5f70 726f 6a65 6374   = other_project
+0005e5c0: 2c20 6e6f 726d 5f77 696e 646f 7720 3d20  , norm_window = 
+0005e5d0: 6e6f 726d 5f77 696e 646f 7729 0d0a 0909  norm_window)....
+0005e5e0: 0d0a 0909 2727 270d 0a09 090d 0a09 0969  ....'''........i
+0005e5f0: 6620 7365 6c66 2e73 6176 655f 6669 6775  f self.save_figu
+0005e600: 7265 735f 746f 5f66 6f6c 6465 723a 7365  res_to_folder:se
+0005e610: 6c66 2e66 6967 7572 655f 7061 7468 3d63  lf.figure_path=c
+0005e620: 6865 636b 5f66 6f6c 6465 7228 7061 7468  heck_folder(path
+0005e630: 3d27 7265 7375 6c74 5f66 6967 7572 6573  ='result_figures
+0005e640: 272c 6375 7272 656e 745f 7061 7468 3d73  ',current_path=s
+0005e650: 656c 662e 7061 7468 290d 0a09 0969 6620  elf.path)....if 
+0005e660: 7469 6d65 5f77 6964 7468 5f70 6572 6365  time_width_perce
+0005e670: 6e74 2069 7320 4e6f 6e65 3a74 696d 655f  nt is None:time_
+0005e680: 7769 6474 685f 7065 7263 656e 743d 7365  width_percent=se
+0005e690: 6c66 2e74 696d 655f 7769 6474 685f 7065  lf.time_width_pe
+0005e6a0: 7263 656e 740d 0a09 0969 6620 7265 6c5f  rcent....if rel_
+0005e6b0: 7469 6d65 2069 7320 4e6f 6e65 3a72 656c  time is None:rel
+0005e6c0: 5f74 696d 653d 7365 6c66 2e72 656c 5f74  _time=self.rel_t
+0005e6d0: 696d 650d 0a09 0969 6620 6f74 6865 7220  ime....if other 
+0005e6e0: 6973 206e 6f74 204e 6f6e 653a 0d0a 0909  is not None:....
+0005e6f0: 0969 6620 6e6f 7420 6861 7361 7474 7228  .if not hasattr(
+0005e700: 6f74 6865 722c 275f 5f69 7465 725f 5f27  other,'__iter__'
+0005e710: 293a 6f74 6865 723d 5b6f 7468 6572 5d0d  ):other=[other].
+0005e720: 0a09 0969 6620 7265 6c5f 7469 6d65 2069  ...if rel_time i
+0005e730: 7320 6e6f 7420 4e6f 6e65 3a0d 0a09 0909  s not None:.....
+0005e740: 6966 206e 6f74 2068 6173 6174 7472 2872  if not hasattr(r
+0005e750: 656c 5f74 696d 652c 275f 5f69 7465 725f  el_time,'__iter_
+0005e760: 5f27 293a 7265 6c5f 7469 6d65 3d5b 7265  _'):rel_time=[re
+0005e770: 6c5f 7469 6d65 5d09 090d 0a09 0965 6c73  l_time]......els
+0005e780: 653a 0d0a 0909 0972 656c 5f74 696d 653d  e:.....rel_time=
+0005e790: 5b31 5d0d 0a09 0969 6620 636d 6170 2069  [1]....if cmap i
+0005e7a0: 7320 4e6f 6e65 3a63 6d61 703d 7365 6c66  s None:cmap=self
+0005e7b0: 2e63 6d61 700d 0a09 0969 6620 6669 7474  .cmap....if fitt
+0005e7c0: 6564 3a0d 0a09 0909 7472 793a 0d0a 0909  ed:.....try:....
+0005e7d0: 0909 7265 3d73 656c 662e 7265 0d0a 0909  ..re=self.re....
+0005e7e0: 0965 7863 6570 743a 0d0a 0909 0909 7072  .except:......pr
+0005e7f0: 696e 7428 224e 6f20 6669 7474 6564 2072  int("No fitted r
+0005e800: 6573 756c 7473 2070 7265 7365 6e74 2229  esults present")
+0005e810: 0d0a 0909 0909 7265 7475 726e 2046 616c  ......return Fal
+0005e820: 7365 0d0a 0909 0969 6620 6e6f 726d 5f77  se.....if norm_w
+0005e830: 696e 646f 7720 6973 206e 6f74 204e 6f6e  indow is not Non
+0005e840: 653a 0d0a 0909 0909 7265 665f 7363 616c  e:......ref_scal
+0005e850: 653d 7265 5b27 4127 5d2e 6c6f 635b 6e6f  e=re['A'].loc[no
+0005e860: 726d 5f77 696e 646f 775b 305d 3a6e 6f72  rm_window[0]:nor
+0005e870: 6d5f 7769 6e64 6f77 5b31 5d2c 6e6f 726d  m_window[1],norm
+0005e880: 5f77 696e 646f 775b 325d 3a6e 6f72 6d5f  _window[2]:norm_
+0005e890: 7769 6e64 6f77 5b33 5d5d 2e6d 6561 6e28  window[3]].mean(
+0005e8a0: 292e 6d65 616e 2829 0d0a 0909 0966 6967  ).mean().....fig
+0005e8b0: 2c61 783d 706c 742e 7375 6270 6c6f 7473  ,ax=plt.subplots
+0005e8c0: 2866 6967 7369 7a65 3d28 3130 2c36 292c  (figsize=(10,6),
+0005e8d0: 6470 693d 3130 3029 0d0a 0909 096f 626a  dpi=100).....obj
+0005e8e0: 6563 7473 3d6c 656e 2872 656c 5f74 696d  ects=len(rel_tim
+0005e8f0: 6529 2a28 312b 6c65 6e28 6f74 6865 7229  e)*(1+len(other)
+0005e900: 290d 0a09 0909 636f 6c6f 7273 3d63 6f6c  ).....colors=col
+0005e910: 6d28 636d 6170 3d63 6d61 702c 6b3d 7261  m(cmap=cmap,k=ra
+0005e920: 6e67 6528 6f62 6a65 6374 7329 290d 0a09  nge(objects))...
+0005e930: 0909 5f3d 706c 6f74 5f74 696d 6528 7265  .._=plot_time(re
+0005e940: 5b27 4127 5d2c 2061 7820 3d20 6178 2c20  ['A'], ax = ax, 
+0005e950: 7265 6c5f 7469 6d65 203d 2072 656c 5f74  rel_time = rel_t
+0005e960: 696d 652c 2074 696d 655f 7769 6474 685f  ime, time_width_
+0005e970: 7065 7263 656e 7420 3d20 7469 6d65 5f77  percent = time_w
+0005e980: 6964 7468 5f70 6572 6365 6e74 2c20 0d0a  idth_percent, ..
+0005e990: 0909 0909 0909 6261 7365 756e 6974 203d  ......baseunit =
+0005e9a0: 2073 656c 662e 6261 7365 756e 6974 2c20   self.baseunit, 
+0005e9b0: 6c69 6e65 735f 6172 6520 3d20 2764 6174  lines_are = 'dat
+0005e9c0: 6127 2c20 636d 6170 203d 2063 6f6c 6f72  a', cmap = color
+0005e9d0: 735b 3a6c 656e 2872 656c 5f74 696d 6529  s[:len(rel_time)
+0005e9e0: 5d2c 2074 6974 6c65 203d 2027 272c 206c  ], title = '', l
+0005e9f0: 696e 6577 6964 7468 203d 206c 696e 6577  inewidth = linew
+0005ea00: 6964 7468 2c20 7375 6270 6c6f 743d 2054  idth, subplot= T
+0005ea10: 7275 652c 2073 6361 7474 6572 6375 7420  rue, scattercut 
+0005ea20: 3d20 7365 6c66 2e73 6361 7474 6572 6375  = self.scattercu
+0005ea30: 7429 0d0a 0909 095f 3d70 6c6f 745f 7469  t)....._=plot_ti
+0005ea40: 6d65 2872 655b 2741 4327 5d2c 2061 7820  me(re['AC'], ax 
+0005ea50: 3d20 6178 2c20 7265 6c5f 7469 6d65 203d  = ax, rel_time =
+0005ea60: 2072 656c 5f74 696d 652c 2074 696d 655f   rel_time, time_
+0005ea70: 7769 6474 685f 7065 7263 656e 7420 3d20  width_percent = 
+0005ea80: 7469 6d65 5f77 6964 7468 5f70 6572 6365  time_width_perce
+0005ea90: 6e74 2c20 0d0a 0909 0909 0909 6261 7365  nt, ........base
+0005eaa0: 756e 6974 203d 2073 656c 662e 6261 7365  unit = self.base
+0005eab0: 756e 6974 2c20 6c69 6e65 735f 6172 6520  unit, lines_are 
+0005eac0: 3d20 2766 6974 7465 6427 2c20 636d 6170  = 'fitted', cmap
+0005ead0: 203d 2063 6f6c 6f72 735b 3a6c 656e 2872   = colors[:len(r
+0005eae0: 656c 5f74 696d 6529 5d2c 2074 6974 6c65  el_time)], title
+0005eaf0: 203d 2027 272c 2073 7562 706c 6f74 203d   = '', subplot =
+0005eb00: 2046 616c 7365 2c20 6c69 6e65 7769 6474   False, linewidt
+0005eb10: 6820 3d20 6c69 6e65 7769 6474 682c 2073  h = linewidth, s
+0005eb20: 6361 7474 6572 6375 7420 3d20 7365 6c66  cattercut = self
+0005eb30: 2e73 6361 7474 6572 6375 7429 0d0a 0909  .scattercut)....
+0005eb40: 0968 616e 646c 6573 2c20 6c61 6265 6c73  .handles, labels
+0005eb50: 3d61 782e 6765 745f 6c65 6765 6e64 5f68  =ax.get_legend_h
+0005eb60: 616e 646c 6573 5f6c 6162 656c 7328 290d  andles_labels().
+0005eb70: 0a09 0909 6c61 623d 5b27 2567 2025 7327  ....lab=['%g %s'
+0005eb80: 2528 656e 742c 7365 6c66 2e62 6173 6575  %(ent,self.baseu
+0005eb90: 6e69 7429 202b 2027 5f27 202b 2073 7472  nit) + '_' + str
+0005eba0: 2873 656c 662e 6669 6c65 6e61 6d65 2920  (self.filename) 
 0005ebb0: 666f 7220 656e 7420 696e 2072 656c 5f74  for ent in rel_t
-0005ebc0: 696d 653a 0d0a 0909 0909 6c61 622e 6170  ime:......lab.ap
-0005ebd0: 7065 6e64 2827 2567 2025 7320 6669 7427  pend('%g %s fit'
-0005ebe0: 2528 656e 742c 7365 6c66 2e62 6173 6575  %(ent,self.baseu
-0005ebf0: 6e69 7429 202b 2027 5f27 202b 2073 7472  nit) + '_' + str
-0005ec00: 2873 656c 662e 6669 6c65 6e61 6d65 2929  (self.filename))
-0005ec10: 0d0a 0909 0969 6620 6f74 6865 7220 6973  .....if other is
-0005ec20: 206e 6f74 204e 6f6e 653a 0d0a 0909 0909   not None:......
-0005ec30: 666f 7220 692c 6f20 696e 2065 6e75 6d65  for i,o in enume
-0005ec40: 7261 7465 286f 7468 6572 293a 0d0a 0909  rate(other):....
-0005ec50: 0909 0974 7279 3a0d 0a09 0909 0909 0972  ...try:........r
-0005ec60: 653d 6f2e 7265 0d0a 0909 0909 0965 7863  e=o.re.......exc
-0005ec70: 6570 743a 0d0a 0909 0909 0909 7072 696e  ept:........prin
-0005ec80: 7428 2725 7320 6861 7320 6e6f 2066 6974  t('%s has no fit
-0005ec90: 7465 6420 7265 7375 6c74 7327 256f 2e66  ted results'%o.f
-0005eca0: 696c 656e 616d 6529 0d0a 0909 0909 0909  ilename)........
-0005ecb0: 636f 6e74 696e 7565 0d0a 0909 0909 0969  continue.......i
-0005ecc0: 6620 6e6f 726d 5f77 696e 646f 7720 6973  f norm_window is
-0005ecd0: 206e 6f74 204e 6f6e 653a 0d0a 0909 0909   not None:......
-0005ece0: 0909 7265 6c5f 7363 616c 653d 7265 5b27  ..rel_scale=re['
-0005ecf0: 4127 5d2e 6c6f 635b 6e6f 726d 5f77 696e  A'].loc[norm_win
-0005ed00: 646f 775b 305d 3a6e 6f72 6d5f 7769 6e64  dow[0]:norm_wind
-0005ed10: 6f77 5b31 5d2c 6e6f 726d 5f77 696e 646f  ow[1],norm_windo
-0005ed20: 775b 325d 3a6e 6f72 6d5f 7769 6e64 6f77  w[2]:norm_window
-0005ed30: 5b33 5d5d 2e6d 6561 6e28 292e 6d65 616e  [3]].mean().mean
-0005ed40: 2829 0d0a 0909 0909 0909 7472 793a 0d0a  ()........try:..
-0005ed50: 0909 0909 0909 0973 6361 6c69 6e67 3d28  .......scaling=(
-0005ed60: 7265 6c5f 7363 616c 652f 7265 665f 7363  rel_scale/ref_sc
-0005ed70: 616c 6529 0d0a 0909 0909 0909 0961 783d  ale).........ax=
-0005ed80: 706c 6f74 5f74 696d 6528 7265 5b27 4143  plot_time(re['AC
-0005ed90: 275d 2f73 6361 6c69 6e67 2c20 636d 6170  ']/scaling, cmap
-0005eda0: 203d 2063 6f6c 6f72 732c 2061 7820 3d20   = colors, ax = 
-0005edb0: 6178 2c20 7265 6c5f 7469 6d65 203d 2072  ax, rel_time = r
-0005edc0: 656c 5f74 696d 652c 200d 0a09 0909 0909  el_time, .......
-0005edd0: 0909 0909 0974 696d 655f 7769 6474 685f  .....time_width_
-0005ede0: 7065 7263 656e 7420 3d20 7469 6d65 5f77  percent = time_w
-0005edf0: 6964 7468 5f70 6572 6365 6e74 2c20 7469  idth_percent, ti
-0005ee00: 746c 6520 3d20 2727 2c20 6c69 6e65 735f  tle = '', lines_
-0005ee10: 6172 6520 3d20 2766 6974 7465 6427 2c20  are = 'fitted', 
-0005ee20: 0d0a 0909 0909 0909 0909 0909 7375 6270  ............subp
-0005ee30: 6c6f 7420 3d20 5472 7565 2c20 636f 6c6f  lot = True, colo
-0005ee40: 725f 6f66 6673 6574 203d 206c 656e 2872  r_offset = len(r
-0005ee50: 656c 5f74 696d 6529 2a28 692b 3129 2c20  el_time)*(i+1), 
-0005ee60: 6c69 6e65 7769 6474 6820 3d20 6c69 6e65  linewidth = line
-0005ee70: 7769 6474 682c 2073 6361 7474 6572 6375  width, scattercu
-0005ee80: 7420 3d20 6f2e 7363 6174 7465 7263 7574  t = o.scattercut
-0005ee90: 290d 0a09 0909 0909 0909 6861 6e64 6c65  ).........handle
-0005eea0: 732c 206c 6162 656c 733d 6178 2e67 6574  s, labels=ax.get
-0005eeb0: 5f6c 6567 656e 645f 6861 6e64 6c65 735f  _legend_handles_
-0005eec0: 6c61 6265 6c73 2829 0d0a 0909 0909 0909  labels()........
-0005eed0: 0966 6f72 2065 6e74 2069 6e20 7265 6c5f  .for ent in rel_
-0005eee0: 7469 6d65 3a0d 0a09 0909 0909 0909 096c  time:..........l
-0005eef0: 6162 2e61 7070 656e 6428 2725 6720 2573  ab.append('%g %s
-0005ef00: 2066 6974 2725 2865 6e74 2c6f 2e62 6173   fit'%(ent,o.bas
-0005ef10: 6575 6e69 7429 202b 2027 5f27 202b 2073  eunit) + '_' + s
-0005ef20: 7472 286f 2e66 696c 656e 616d 6529 290d  tr(o.filename)).
-0005ef30: 0a09 0909 0909 0909 666f 7220 6120 696e  ........for a in
-0005ef40: 2068 616e 646c 6573 5b2d 6c65 6e28 7265   handles[-len(re
-0005ef50: 6c5f 7469 6d65 293a 5d3a 0d0a 0909 0909  l_time):]:......
-0005ef60: 0909 0909 6861 6e2e 6170 7065 6e64 2861  ....han.append(a
-0005ef70: 290d 0a09 0909 0909 0909 0d0a 0909 0909  )...............
-0005ef80: 0909 0969 6620 6461 7461 5f61 6e64 5f66  ...if data_and_f
-0005ef90: 6974 3a0d 0a09 0909 0909 0909 0961 783d  it:..........ax=
-0005efa0: 706c 6f74 5f74 696d 6528 7265 5b27 4127  plot_time(re['A'
-0005efb0: 5d2f 7363 616c 696e 672c 2063 6d61 7020  ]/scaling, cmap 
-0005efc0: 3d20 7365 6c66 2e63 6d61 702c 2061 7820  = self.cmap, ax 
-0005efd0: 3d20 6178 2c20 7265 6c5f 7469 6d65 203d  = ax, rel_time =
-0005efe0: 2072 656c 5f74 696d 652c 200d 0a09 0909   rel_time, .....
-0005eff0: 0909 0909 0909 0909 7469 6d65 5f77 6964  ........time_wid
-0005f000: 7468 5f70 6572 6365 6e74 203d 2074 696d  th_percent = tim
-0005f010: 655f 7769 6474 685f 7065 7263 656e 742c  e_width_percent,
-0005f020: 2074 6974 6c65 203d 206f 2e66 696c 656e   title = o.filen
-0005f030: 616d 652c 200d 0a09 0909 0909 0909 0909  ame, ...........
-0005f040: 0909 6261 7365 756e 6974 203d 2073 656c  ..baseunit = sel
-0005f050: 662e 6261 7365 756e 6974 2c20 6c69 6e65  f.baseunit, line
-0005f060: 735f 6172 6520 3d20 2764 6174 6127 2c20  s_are = 'data', 
-0005f070: 7375 6270 6c6f 7420 3d20 5472 7565 2c20  subplot = True, 
-0005f080: 0d0a 0909 0909 0909 0909 0909 0963 6f6c  .............col
-0005f090: 6f72 5f6f 6666 7365 7420 3d20 6c65 6e28  or_offset = len(
-0005f0a0: 7265 6c5f 7469 6d65 292a 2869 2b31 292c  rel_time)*(i+1),
-0005f0b0: 206c 696e 6577 6964 7468 203d 206c 696e   linewidth = lin
-0005f0c0: 6577 6964 7468 2c20 7363 6174 7465 7263  ewidth, scatterc
-0005f0d0: 7574 203d 206f 2e73 6361 7474 6572 6375  ut = o.scattercu
-0005f0e0: 7429 0d0a 0909 0909 0909 0909 6861 6e64  t)..........hand
-0005f0f0: 6c65 732c 206c 6162 656c 733d 6178 2e67  les, labels=ax.g
-0005f100: 6574 5f6c 6567 656e 645f 6861 6e64 6c65  et_legend_handle
-0005f110: 735f 6c61 6265 6c73 2829 0d0a 0909 0909  s_labels()......
-0005f120: 0909 0909 666f 7220 656e 7420 696e 2072  ....for ent in r
-0005f130: 656c 5f74 696d 653a 0d0a 0909 0909 0909  el_time:........
-0005f140: 0909 096c 6162 2e61 7070 656e 6428 2725  ...lab.append('%
-0005f150: 6720 2573 2725 2865 6e74 2c6f 2e62 6173  g %s'%(ent,o.bas
-0005f160: 6575 6e69 7429 202b 2027 5f27 202b 2073  eunit) + '_' + s
-0005f170: 7472 286f 2e66 696c 656e 616d 6529 290d  tr(o.filename)).
-0005f180: 0a09 0909 0909 0909 0966 6f72 2061 2069  .........for a i
-0005f190: 6e20 6861 6e64 6c65 735b 2d6c 656e 2872  n handles[-len(r
-0005f1a0: 656c 5f74 696d 6529 3a5d 3a0d 0a09 0909  el_time):]:.....
-0005f1b0: 0909 0909 0909 6861 6e2e 6170 7065 6e64  ......han.append
-0005f1c0: 2861 290d 0a09 0909 0909 0909 6e6f 726d  (a).........norm
-0005f1d0: 5f66 6169 6c65 6420 3d20 4661 6c73 650d  _failed = False.
-0005f1e0: 0a09 0909 0909 0965 7863 6570 743a 0d0a  .......except:..
-0005f1f0: 0909 0909 0909 0970 7269 6e74 2827 7363  .......print('sc
-0005f200: 616c 696e 6720 4661 696c 6564 2127 290d  aling Failed!').
-0005f210: 0a09 0909 0909 0909 6e6f 726d 5f66 6169  ........norm_fai
-0005f220: 6c65 6420 3d20 5472 7565 0d0a 0909 0909  led = True......
-0005f230: 0965 6c73 653a 206e 6f72 6d5f 6661 696c  .else: norm_fail
-0005f240: 6564 3d54 7275 6509 0d0a 0909 0909 0969  ed=True........i
-0005f250: 6620 6e6f 726d 5f66 6169 6c65 643a 0d0a  f norm_failed:..
-0005f260: 0909 0909 0909 6178 3d70 6c6f 745f 7469  ......ax=plot_ti
-0005f270: 6d65 2872 655b 2741 4327 5d2c 2063 6d61  me(re['AC'], cma
-0005f280: 7020 3d20 636f 6c6f 7273 2c20 6178 203d  p = colors, ax =
-0005f290: 2061 782c 2072 656c 5f74 696d 6520 3d20   ax, rel_time = 
-0005f2a0: 7265 6c5f 7469 6d65 2c20 0d0a 0909 0909  rel_time, ......
-0005f2b0: 0909 0909 0909 7469 6d65 5f77 6964 7468  ......time_width
-0005f2c0: 5f70 6572 6365 6e74 203d 2074 696d 655f  _percent = time_
-0005f2d0: 7769 6474 685f 7065 7263 656e 742c 2074  width_percent, t
-0005f2e0: 6974 6c65 203d 2027 272c 206c 696e 6573  itle = '', lines
-0005f2f0: 5f61 7265 203d 2027 6669 7474 6564 272c  _are = 'fitted',
-0005f300: 200d 0a09 0909 0909 0909 0909 0973 7562   ............sub
-0005f310: 706c 6f74 203d 2054 7275 652c 2063 6f6c  plot = True, col
-0005f320: 6f72 5f6f 6666 7365 7420 3d20 6c65 6e28  or_offset = len(
-0005f330: 7265 6c5f 7469 6d65 292a 2869 2b31 292c  rel_time)*(i+1),
-0005f340: 206c 696e 6577 6964 7468 203d 206c 696e   linewidth = lin
-0005f350: 6577 6964 7468 2c20 7363 6174 7465 7263  ewidth, scatterc
-0005f360: 7574 203d 206f 2e73 6361 7474 6572 6375  ut = o.scattercu
-0005f370: 7429 0d0a 0909 0909 0909 6861 6e64 6c65  t)........handle
-0005f380: 732c 206c 6162 656c 733d 6178 2e67 6574  s, labels=ax.get
-0005f390: 5f6c 6567 656e 645f 6861 6e64 6c65 735f  _legend_handles_
-0005f3a0: 6c61 6265 6c73 2829 0d0a 0909 0909 0909  labels()........
-0005f3b0: 666f 7220 656e 7420 696e 2072 656c 5f74  for ent in rel_t
-0005f3c0: 696d 653a 0d0a 0909 0909 0909 096c 6162  ime:.........lab
-0005f3d0: 2e61 7070 656e 6428 2725 6720 2573 2066  .append('%g %s f
-0005f3e0: 6974 2725 2865 6e74 2c6f 2e62 6173 6575  it'%(ent,o.baseu
-0005f3f0: 6e69 7429 202b 2027 5f27 202b 2073 7472  nit) + '_' + str
-0005f400: 286f 2e66 696c 656e 616d 6529 290d 0a09  (o.filename))...
-0005f410: 0909 0909 0966 6f72 2061 2069 6e20 6861  .....for a in ha
-0005f420: 6e64 6c65 735b 2d6c 656e 2872 656c 5f74  ndles[-len(rel_t
-0005f430: 696d 6529 3a5d 3a0d 0a09 0909 0909 0909  ime):]:.........
-0005f440: 6861 6e2e 6170 7065 6e64 2861 290d 0a09  han.append(a)...
-0005f450: 0909 0909 090d 0a09 0909 0909 0969 6620  .............if 
-0005f460: 6461 7461 5f61 6e64 5f66 6974 3a0d 0a09  data_and_fit:...
-0005f470: 0909 0909 0909 6178 3d70 6c6f 745f 7469  ......ax=plot_ti
-0005f480: 6d65 2872 655b 2741 275d 2c20 636d 6170  me(re['A'], cmap
-0005f490: 203d 2073 656c 662e 636d 6170 2c20 6178   = self.cmap, ax
-0005f4a0: 203d 2061 782c 2072 656c 5f74 696d 6520   = ax, rel_time 
-0005f4b0: 3d20 7265 6c5f 7469 6d65 2c20 0d0a 0909  = rel_time, ....
-0005f4c0: 0909 0909 0909 0909 7469 6d65 5f77 6964  ........time_wid
-0005f4d0: 7468 5f70 6572 6365 6e74 203d 2074 696d  th_percent = tim
-0005f4e0: 655f 7769 6474 685f 7065 7263 656e 742c  e_width_percent,
-0005f4f0: 2074 6974 6c65 203d 206f 2e66 696c 656e   title = o.filen
-0005f500: 616d 652c 200d 0a09 0909 0909 0909 0909  ame, ...........
-0005f510: 0962 6173 6575 6e69 7420 3d20 7365 6c66  .baseunit = self
-0005f520: 2e62 6173 6575 6e69 742c 206c 696e 6573  .baseunit, lines
-0005f530: 5f61 7265 203d 2027 6461 7461 272c 2073  _are = 'data', s
-0005f540: 7562 706c 6f74 203d 2054 7275 652c 200d  ubplot = True, .
-0005f550: 0a09 0909 0909 0909 0909 0963 6f6c 6f72  ...........color
-0005f560: 5f6f 6666 7365 7420 3d20 6c65 6e28 7265  _offset = len(re
-0005f570: 6c5f 7469 6d65 292a 2869 2b31 292c 206c  l_time)*(i+1), l
-0005f580: 696e 6577 6964 7468 203d 206c 696e 6577  inewidth = linew
-0005f590: 6964 7468 2c20 7363 6174 7465 7263 7574  idth, scattercut
-0005f5a0: 203d 206f 2e73 6361 7474 6572 6375 7429   = o.scattercut)
-0005f5b0: 0d0a 0909 0909 0909 0968 616e 646c 6573  .........handles
-0005f5c0: 2c20 6c61 6265 6c73 3d61 782e 6765 745f  , labels=ax.get_
-0005f5d0: 6c65 6765 6e64 5f68 616e 646c 6573 5f6c  legend_handles_l
-0005f5e0: 6162 656c 7328 290d 0a09 0909 0909 0909  abels().........
-0005f5f0: 666f 7220 656e 7420 696e 2072 656c 5f74  for ent in rel_t
-0005f600: 696d 653a 0d0a 0909 0909 0909 0909 6c61  ime:..........la
-0005f610: 622e 6170 7065 6e64 2827 2567 2025 7327  b.append('%g %s'
-0005f620: 2528 656e 742c 6f2e 6261 7365 756e 6974  %(ent,o.baseunit
-0005f630: 2920 2b20 275f 2720 2b20 7374 7228 6f2e  ) + '_' + str(o.
-0005f640: 6669 6c65 6e61 6d65 2929 0d0a 0909 0909  filename))......
-0005f650: 0909 0966 6f72 2061 2069 6e20 6861 6e64  ...for a in hand
-0005f660: 6c65 735b 2d6c 656e 2872 656c 5f74 696d  les[-len(rel_tim
-0005f670: 6529 3a5d 3a0d 0a09 0909 0909 0909 0968  e):]:..........h
-0005f680: 616e 2e61 7070 656e 6428 6129 0d0a 0909  an.append(a)....
-0005f690: 0969 6620 6e6f 7420 6e6f 726d 5f66 6169  .if not norm_fai
-0005f6a0: 6c65 643a 0d0a 0909 0909 6178 2e73 6574  led:......ax.set
-0005f6b0: 5f74 6974 6c65 2827 636f 6d70 6172 6520  _title('compare 
-0005f6c0: 6d65 6173 7572 6564 2061 6e64 2066 6974  measured and fit
-0005f6d0: 7465 6420 6461 7461 2061 7420 6769 7665  ted data at give
-0005f6e0: 6e20 7469 6d65 735c 6e20 7363 616c 6564  n times\n scaled
-0005f6f0: 2074 6f20 743d 2567 2070 7320 3a20 2567   to t=%g ps : %g
-0005f700: 2070 7320 2c20 776c 3d20 2567 206e 6d3a   ps , wl= %g nm:
-0005f710: 2025 6720 6e6d 2725 286e 6f72 6d5f 7769   %g nm'%(norm_wi
-0005f720: 6e64 6f77 5b30 5d2c 6e6f 726d 5f77 696e  ndow[0],norm_win
-0005f730: 646f 775b 315d 2c6e 6f72 6d5f 7769 6e64  dow[1],norm_wind
-0005f740: 6f77 5b32 5d2c 6e6f 726d 5f77 696e 646f  ow[2],norm_windo
-0005f750: 775b 335d 2929 0d0a 0909 0965 6c73 653a  w[3])).....else:
-0005f760: 0d0a 0909 0909 6178 2e73 6574 5f74 6974  ......ax.set_tit
-0005f770: 6c65 2827 636f 6d70 6172 6520 6d65 6173  le('compare meas
-0005f780: 7572 6564 2061 6e64 2066 6974 7465 6420  ured and fitted 
-0005f790: 6461 7461 2061 7420 6769 7665 6e20 7469  data at given ti
-0005f7a0: 6d65 7327 290d 0a09 0909 6178 2e73 6574  mes').....ax.set
-0005f7b0: 5f78 6c69 6d28 7265 5b27 4127 5d2e 636f  _xlim(re['A'].co
-0005f7c0: 6c75 6d6e 732e 7661 6c75 6573 5b30 5d2c  lumns.values[0],
-0005f7d0: 7265 5b27 4127 5d2e 636f 6c75 6d6e 732e  re['A'].columns.
-0005f7e0: 7661 6c75 6573 5b2d 315d 290d 0a09 0909  values[-1]).....
-0005f7f0: 6178 2e6c 6567 656e 6428 6861 6e2c 206c  ax.legend(han, l
-0005f800: 6162 202c 6c61 6265 6c73 7061 6369 6e67  ab ,labelspacing
-0005f810: 203d 2030 2c20 6e63 6f6c 203d 2032 2c20   = 0, ncol = 2, 
-0005f820: 636f 6c75 6d6e 7370 6163 696e 6720 3d20  columnspacing = 
-0005f830: 312c 2068 616e 646c 656c 656e 6774 6820  1, handlelength 
-0005f840: 3d20 312c 2066 7261 6d65 6f6e 203d 2046  = 1, frameon = F
-0005f850: 616c 7365 290d 0a09 0965 6c73 653a 0d0a  alse)....else:..
-0005f860: 0909 0969 6620 6e6f 726d 5f77 696e 646f  ...if norm_windo
-0005f870: 7720 6973 206e 6f74 204e 6f6e 653a 0d0a  w is not None:..
-0005f880: 0909 0909 7265 665f 7363 616c 653d 7365  ....ref_scale=se
-0005f890: 6c66 2e64 732e 6c6f 635b 6e6f 726d 5f77  lf.ds.loc[norm_w
-0005f8a0: 696e 646f 775b 305d 3a6e 6f72 6d5f 7769  indow[0]:norm_wi
-0005f8b0: 6e64 6f77 5b31 5d2c 6e6f 726d 5f77 696e  ndow[1],norm_win
-0005f8c0: 646f 775b 325d 3a6e 6f72 6d5f 7769 6e64  dow[2]:norm_wind
-0005f8d0: 6f77 5b33 5d5d 2e6d 6561 6e28 292e 6d65  ow[3]].mean().me
-0005f8e0: 616e 2829 0d0a 0909 096f 626a 6563 7473  an().....objects
-0005f8f0: 3d6c 656e 2872 656c 5f74 696d 6529 2a28  =len(rel_time)*(
-0005f900: 312b 6c65 6e28 6f74 6865 7229 290d 0a09  1+len(other))...
-0005f910: 0909 636f 6c6f 7273 3d63 6f6c 6d28 636d  ..colors=colm(cm
-0005f920: 6170 3d63 6d61 702c 6b3d 7261 6e67 6528  ap=cmap,k=range(
-0005f930: 6f62 6a65 6374 7329 290d 0a09 0909 6669  objects)).....fi
-0005f940: 672c 6178 3d70 6c74 2e73 7562 706c 6f74  g,ax=plt.subplot
-0005f950: 7328 6669 6773 697a 653d 2831 302c 3629  s(figsize=(10,6)
-0005f960: 2c64 7069 3d31 3030 290d 0a09 0909 5f3d  ,dpi=100)....._=
-0005f970: 706c 6f74 5f74 696d 6528 7365 6c66 2e64  plot_time(self.d
-0005f980: 732c 2061 7820 3d20 6178 2c20 7265 6c5f  s, ax = ax, rel_
-0005f990: 7469 6d65 203d 2072 656c 5f74 696d 652c  time = rel_time,
-0005f9a0: 2074 696d 655f 7769 6474 685f 7065 7263   time_width_perc
-0005f9b0: 656e 7420 3d20 7469 6d65 5f77 6964 7468  ent = time_width
-0005f9c0: 5f70 6572 6365 6e74 2c20 0d0a 0909 0909  _percent, ......
-0005f9d0: 0909 7469 746c 6520 3d20 7469 746c 652c  ..title = title,
-0005f9e0: 206c 696e 6573 5f61 7265 203d 2027 6461   lines_are = 'da
-0005f9f0: 7461 272c 2073 6361 7474 6572 6375 7420  ta', scattercut 
-0005fa00: 3d20 7365 6c66 2e73 6361 7474 6572 6375  = self.scattercu
-0005fa10: 742c 2062 6f72 6465 7263 7574 203d 2073  t, bordercut = s
-0005fa20: 656c 662e 626f 7264 6572 6375 742c 200d  elf.bordercut, .
-0005fa30: 0a09 0909 0909 0977 6176 655f 6e6d 5f62  .......wave_nm_b
-0005fa40: 696e 203d 2073 656c 662e 7761 7665 5f6e  in = self.wave_n
-0005fa50: 6d5f 6269 6e2c 2063 6d61 7020 3d20 636f  m_bin, cmap = co
-0005fa60: 6c6f 7273 2c20 7375 6270 6c6f 7420 3d20  lors, subplot = 
-0005fa70: 5472 7565 2c20 6c69 6e65 7769 6474 6820  True, linewidth 
-0005fa80: 3d20 6c69 6e65 7769 6474 682c 2062 6173  = linewidth, bas
-0005fa90: 6575 6e69 743d 7365 6c66 2e62 6173 6575  eunit=self.baseu
-0005faa0: 6e69 7429 0d0a 0909 0969 6620 313a 0d0a  nit).....if 1:..
-0005fab0: 0909 0909 5f3d 706c 6f74 5f74 696d 6528  ...._=plot_time(
-0005fac0: 7365 6c66 2e64 732c 2061 7820 3d20 6178  self.ds, ax = ax
-0005fad0: 2c20 7265 6c5f 7469 6d65 203d 2072 656c  , rel_time = rel
-0005fae0: 5f74 696d 652c 2074 696d 655f 7769 6474  _time, time_widt
-0005faf0: 685f 7065 7263 656e 7420 3d20 7469 6d65  h_percent = time
-0005fb00: 5f77 6964 7468 5f70 6572 6365 6e74 2c20  _width_percent, 
-0005fb10: 0d0a 0909 0909 0909 0974 6974 6c65 203d  .........title =
-0005fb20: 2074 6974 6c65 2c20 6c69 6e65 735f 6172   title, lines_ar
-0005fb30: 6520 3d20 2773 6d6f 6f74 6865 6427 2c20  e = 'smoothed', 
-0005fb40: 7363 6174 7465 7263 7574 203d 2073 656c  scattercut = sel
-0005fb50: 662e 7363 6174 7465 7263 7574 2c20 626f  f.scattercut, bo
-0005fb60: 7264 6572 6375 7420 3d20 7365 6c66 2e62  rdercut = self.b
-0005fb70: 6f72 6465 7263 7574 2c77 6176 655f 6e6d  ordercut,wave_nm
-0005fb80: 5f62 696e 203d 2073 656c 662e 7761 7665  _bin = self.wave
-0005fb90: 5f6e 6d5f 6269 6e2c 2063 6d61 7020 3d20  _nm_bin, cmap = 
-0005fba0: 636f 6c6f 7273 2c20 7375 6270 6c6f 7420  colors, subplot 
-0005fbb0: 3d20 4661 6c73 652c 206c 696e 6577 6964  = False, linewid
-0005fbc0: 7468 203d 206c 696e 6577 6964 7468 2c20  th = linewidth, 
-0005fbd0: 6261 7365 756e 6974 203d 2073 656c 662e  baseunit = self.
-0005fbe0: 6261 7365 756e 6974 290d 0a09 0909 6861  baseunit).....ha
-0005fbf0: 6e64 6c65 732c 206c 6162 656c 733d 6178  ndles, labels=ax
-0005fc00: 2e67 6574 5f6c 6567 656e 645f 6861 6e64  .get_legend_hand
-0005fc10: 6c65 735f 6c61 6265 6c73 2829 0d0a 0909  les_labels()....
-0005fc20: 096c 6162 3d5b 2725 6720 2573 2725 2865  .lab=['%g %s'%(e
-0005fc30: 6e74 2c73 656c 662e 6261 7365 756e 6974  nt,self.baseunit
-0005fc40: 2920 2b20 275f 2720 2b20 7374 7228 7365  ) + '_' + str(se
-0005fc50: 6c66 2e66 696c 656e 616d 6529 2066 6f72  lf.filename) for
-0005fc60: 2065 6e74 2069 6e20 7265 6c5f 7469 6d65   ent in rel_time
-0005fc70: 5d0d 0a09 0909 6861 6e3d 6861 6e64 6c65  ].....han=handle
-0005fc80: 735b 3a6c 656e 2872 656c 5f74 696d 6529  s[:len(rel_time)
-0005fc90: 5d0d 0a09 0909 6966 206f 7468 6572 2069  ].....if other i
-0005fca0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a09 0909  s not None:.....
-0005fcb0: 0966 6f72 2069 2c6f 2069 6e20 656e 756d  .for i,o in enum
-0005fcc0: 6572 6174 6528 6f74 6865 7229 3a0d 0a09  erate(other):...
-0005fcd0: 0909 0909 6966 206e 6f72 6d5f 7769 6e64  ....if norm_wind
-0005fce0: 6f77 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ow is not None:.
-0005fcf0: 0a09 0909 0909 0972 656c 5f73 6361 6c65  .......rel_scale
-0005fd00: 3d6f 2e64 732e 6c6f 635b 6e6f 726d 5f77  =o.ds.loc[norm_w
-0005fd10: 696e 646f 775b 305d 3a6e 6f72 6d5f 7769  indow[0]:norm_wi
-0005fd20: 6e64 6f77 5b31 5d2c 6e6f 726d 5f77 696e  ndow[1],norm_win
-0005fd30: 646f 775b 325d 3a6e 6f72 6d5f 7769 6e64  dow[2]:norm_wind
-0005fd40: 6f77 5b33 5d5d 2e6d 6561 6e28 292e 6d65  ow[3]].mean().me
-0005fd50: 616e 2829 0d0a 0909 0909 0909 7472 793a  an()........try:
-0005fd60: 0d0a 0909 0909 0909 0973 6361 6c69 6e67  .........scaling
-0005fd70: 203d 2028 7265 6c5f 7363 616c 652f 7265   = (rel_scale/re
-0005fd80: 665f 7363 616c 6529 0d0a 0909 0909 0909  f_scale)........
-0005fd90: 0961 783d 706c 6f74 5f74 696d 6528 6f2e  .ax=plot_time(o.
-0005fda0: 6473 2f73 6361 6c69 6e67 2c20 636d 6170  ds/scaling, cmap
-0005fdb0: 203d 2063 6f6c 6f72 732c 2061 7820 3d20   = colors, ax = 
-0005fdc0: 6178 2c20 7265 6c5f 7469 6d65 203d 2072  ax, rel_time = r
-0005fdd0: 656c 5f74 696d 652c 200d 0a09 0909 0909  el_time, .......
-0005fde0: 0909 0909 0974 696d 655f 7769 6474 685f  .....time_width_
-0005fdf0: 7065 7263 656e 7420 3d20 7469 6d65 5f77  percent = time_w
-0005fe00: 6964 7468 5f70 6572 6365 6e74 2c20 7469  idth_percent, ti
-0005fe10: 746c 6520 3d20 7469 746c 652c 206c 696e  tle = title, lin
-0005fe20: 6573 5f61 7265 203d 2027 6461 7461 272c  es_are = 'data',
-0005fe30: 200d 0a09 0909 0909 0909 0909 0973 6361   ............sca
-0005fe40: 7474 6572 6375 7420 3d20 6f2e 7363 6174  ttercut = o.scat
-0005fe50: 7465 7263 7574 2c20 626f 7264 6572 6375  tercut, bordercu
-0005fe60: 7420 3d20 6f2e 626f 7264 6572 6375 742c  t = o.bordercut,
-0005fe70: 206c 696e 6577 6964 7468 203d 206c 696e   linewidth = lin
-0005fe80: 6577 6964 7468 2c20 0d0a 0909 0909 0909  ewidth, ........
-0005fe90: 0909 0909 7761 7665 5f6e 6d5f 6269 6e20  ....wave_nm_bin 
-0005fea0: 3d20 6f2e 7761 7665 5f6e 6d5f 6269 6e2c  = o.wave_nm_bin,
-0005feb0: 2073 7562 706c 6f74 203d 2054 7275 652c   subplot = True,
-0005fec0: 2063 6f6c 6f72 5f6f 6666 7365 7420 3d20   color_offset = 
-0005fed0: 6c65 6e28 7265 6c5f 7469 6d65 292a 2869  len(rel_time)*(i
-0005fee0: 2b31 2929 0d0a 0909 0909 0909 0968 616e  +1)).........han
-0005fef0: 646c 6573 2c20 6c61 6265 6c73 3d61 782e  dles, labels=ax.
-0005ff00: 6765 745f 6c65 6765 6e64 5f68 616e 646c  get_legend_handl
-0005ff10: 6573 5f6c 6162 656c 7328 290d 0a09 0909  es_labels().....
-0005ff20: 0909 0909 666f 7220 656e 7420 696e 2072  ....for ent in r
-0005ff30: 656c 5f74 696d 653a 0d0a 0909 0909 0909  el_time:........
-0005ff40: 0909 6c61 622e 6170 7065 6e64 2827 2567  ..lab.append('%g
-0005ff50: 2025 7327 2528 656e 742c 6f2e 6261 7365   %s'%(ent,o.base
-0005ff60: 756e 6974 2920 2b20 275f 2720 2b20 7374  unit) + '_' + st
-0005ff70: 7228 6f2e 6669 6c65 6e61 6d65 2929 0d0a  r(o.filename))..
-0005ff80: 0909 0909 0909 0966 6f72 2061 2069 6e20  .......for a in 
-0005ff90: 6861 6e64 6c65 735b 2d6c 656e 2872 656c  handles[-len(rel
-0005ffa0: 5f74 696d 6529 3a5d 3a0d 0a09 0909 0909  _time):]:.......
-0005ffb0: 0909 0968 616e 2e61 7070 656e 6428 6129  ...han.append(a)
-0005ffc0: 0d0a 0d0a 0909 0909 0909 0969 6620 6461  ...........if da
-0005ffd0: 7461 5f61 6e64 5f66 6974 3a0d 0a09 0909  ta_and_fit:.....
-0005ffe0: 0909 0909 0961 783d 706c 6f74 5f74 696d  .....ax=plot_tim
-0005fff0: 6528 6f2e 6473 2f73 6361 6c69 6e67 2c20  e(o.ds/scaling, 
-00060000: 636d 6170 203d 2063 6f6c 6f72 732c 2061  cmap = colors, a
-00060010: 7820 3d20 6178 2c20 7265 6c5f 7469 6d65  x = ax, rel_time
-00060020: 203d 2072 656c 5f74 696d 652c 200d 0a09   = rel_time, ...
-00060030: 0909 0909 0909 0909 0974 696d 655f 7769  .........time_wi
-00060040: 6474 685f 7065 7263 656e 7420 3d20 7469  dth_percent = ti
-00060050: 6d65 5f77 6964 7468 5f70 6572 6365 6e74  me_width_percent
-00060060: 2c20 7469 746c 6520 3d20 7469 746c 652c  , title = title,
-00060070: 206c 696e 6573 5f61 7265 203d 2027 736d   lines_are = 'sm
-00060080: 6f6f 7468 6564 272c 200d 0a09 0909 0909  oothed', .......
-00060090: 0909 0909 0973 6361 7474 6572 6375 7420  .....scattercut 
-000600a0: 3d20 6f2e 7363 6174 7465 7263 7574 2c20  = o.scattercut, 
-000600b0: 626f 7264 6572 6375 7420 3d20 6f2e 626f  bordercut = o.bo
-000600c0: 7264 6572 6375 742c 206c 696e 6577 6964  rdercut, linewid
-000600d0: 7468 203d 206c 696e 6577 6964 7468 2c20  th = linewidth, 
-000600e0: 0d0a 0909 0909 0909 0909 0909 7761 7665  ............wave
-000600f0: 5f6e 6d5f 6269 6e20 3d20 6f2e 7761 7665  _nm_bin = o.wave
-00060100: 5f6e 6d5f 6269 6e2c 2073 7562 706c 6f74  _nm_bin, subplot
-00060110: 203d 2054 7275 652c 2063 6f6c 6f72 5f6f   = True, color_o
-00060120: 6666 7365 7420 3d20 6c65 6e28 7265 6c5f  ffset = len(rel_
-00060130: 7469 6d65 292a 2869 2b31 2929 0d0a 0909  time)*(i+1))....
-00060140: 0909 0909 0973 6361 6c69 6e67 5f66 6169  .....scaling_fai
-00060150: 6c65 643d 4661 6c73 650d 0a09 0909 0909  led=False.......
-00060160: 0965 7863 6570 743a 0d0a 0909 0909 0909  .except:........
-00060170: 0970 7269 6e74 2827 7363 616c 696e 6720  .print('scaling 
-00060180: 4661 696c 6564 2127 290d 0a09 0909 0909  Failed!').......
-00060190: 0909 7363 616c 696e 675f 6661 696c 6564  ..scaling_failed
-000601a0: 3d54 7275 650d 0a09 0909 0909 656c 7365  =True.......else
-000601b0: 3a0d 0a09 0909 0909 0973 6361 6c69 6e67  :........scaling
-000601c0: 5f66 6169 6c65 643d 5472 7565 0d0a 0909  _failed=True....
-000601d0: 0909 0969 6620 7363 616c 696e 675f 6661  ...if scaling_fa
-000601e0: 696c 6564 3a0d 0a09 0909 0909 0961 783d  iled:........ax=
-000601f0: 706c 6f74 5f74 696d 6528 6f2e 6473 2c20  plot_time(o.ds, 
-00060200: 636d 6170 203d 2063 6f6c 6f72 732c 2061  cmap = colors, a
-00060210: 7820 3d20 6178 2c20 7265 6c5f 7469 6d65  x = ax, rel_time
-00060220: 203d 2072 656c 5f74 696d 652c 200d 0a09   = rel_time, ...
-00060230: 0909 0909 0909 0909 7469 6d65 5f77 6964  ........time_wid
-00060240: 7468 5f70 6572 6365 6e74 203d 2074 696d  th_percent = tim
-00060250: 655f 7769 6474 685f 7065 7263 656e 742c  e_width_percent,
-00060260: 2074 6974 6c65 203d 2074 6974 6c65 2c20   title = title, 
-00060270: 6c69 6e65 735f 6172 6520 3d20 2764 6174  lines_are = 'dat
-00060280: 6127 2c20 0d0a 0909 0909 0909 0909 0973  a', ...........s
-00060290: 6361 7474 6572 6375 7420 3d20 6f2e 7363  cattercut = o.sc
-000602a0: 6174 7465 7263 7574 2c20 626f 7264 6572  attercut, border
-000602b0: 6375 7420 3d20 6f2e 626f 7264 6572 6375  cut = o.bordercu
-000602c0: 742c 206c 696e 6577 6964 7468 203d 206c  t, linewidth = l
-000602d0: 696e 6577 6964 7468 2c20 0d0a 0909 0909  inewidth, ......
-000602e0: 0909 0909 0977 6176 655f 6e6d 5f62 696e  .....wave_nm_bin
-000602f0: 203d 206f 2e77 6176 655f 6e6d 5f62 696e   = o.wave_nm_bin
-00060300: 2c20 7375 6270 6c6f 7420 3d20 5472 7565  , subplot = True
-00060310: 2c20 636f 6c6f 725f 6f66 6673 6574 203d  , color_offset =
-00060320: 206c 656e 2872 656c 5f74 696d 6529 2a28   len(rel_time)*(
-00060330: 692b 3129 290d 0a09 0909 0909 0968 616e  i+1))........han
-00060340: 646c 6573 2c20 6c61 6265 6c73 3d61 782e  dles, labels=ax.
-00060350: 6765 745f 6c65 6765 6e64 5f68 616e 646c  get_legend_handl
-00060360: 6573 5f6c 6162 656c 7328 290d 0a09 0909  es_labels().....
-00060370: 0909 0966 6f72 2065 6e74 2069 6e20 7265  ...for ent in re
-00060380: 6c5f 7469 6d65 3a0d 0a09 0909 0909 0909  l_time:.........
-00060390: 6c61 622e 6170 7065 6e64 2827 2567 2025  lab.append('%g %
-000603a0: 7327 2528 656e 742c 6f2e 6261 7365 756e  s'%(ent,o.baseun
-000603b0: 6974 2920 2b20 275f 2720 2b20 7374 7228  it) + '_' + str(
-000603c0: 6f2e 6669 6c65 6e61 6d65 2929 0d0a 0909  o.filename))....
-000603d0: 0909 0909 666f 7220 6120 696e 2068 616e  ....for a in han
-000603e0: 646c 6573 5b2d 6c65 6e28 7265 6c5f 7469  dles[-len(rel_ti
-000603f0: 6d65 293a 5d3a 0d0a 0909 0909 0909 0968  me):]:.........h
-00060400: 616e 2e61 7070 656e 6428 6129 0d0a 0909  an.append(a)....
-00060410: 0909 0909 6966 2064 6174 615f 616e 645f  ....if data_and_
-00060420: 6669 743a 0d0a 0909 0909 0909 0961 783d  fit:.........ax=
-00060430: 706c 6f74 5f74 696d 6528 6f2e 6473 2c20  plot_time(o.ds, 
-00060440: 636d 6170 203d 2063 6f6c 6f72 732c 2061  cmap = colors, a
-00060450: 7820 3d20 6178 2c20 7265 6c5f 7469 6d65  x = ax, rel_time
-00060460: 203d 2072 656c 5f74 696d 652c 200d 0a09   = rel_time, ...
-00060470: 0909 0909 0909 0909 7469 6d65 5f77 6964  ........time_wid
-00060480: 7468 5f70 6572 6365 6e74 203d 2074 696d  th_percent = tim
-00060490: 655f 7769 6474 685f 7065 7263 656e 742c  e_width_percent,
-000604a0: 2074 6974 6c65 203d 2074 6974 6c65 2c20   title = title, 
-000604b0: 6c69 6e65 735f 6172 6520 3d20 2773 6d6f  lines_are = 'smo
-000604c0: 6f74 6865 6427 2c20 0d0a 0909 0909 0909  othed', ........
-000604d0: 0909 0973 6361 7474 6572 6375 7420 3d20  ...scattercut = 
-000604e0: 6f2e 7363 6174 7465 7263 7574 2c20 626f  o.scattercut, bo
-000604f0: 7264 6572 6375 7420 3d20 6f2e 626f 7264  rdercut = o.bord
-00060500: 6572 6375 742c 206c 696e 6577 6964 7468  ercut, linewidth
-00060510: 203d 206c 696e 6577 6964 7468 2c20 0d0a   = linewidth, ..
-00060520: 0909 0909 0909 0909 0977 6176 655f 6e6d  .........wave_nm
-00060530: 5f62 696e 203d 206f 2e77 6176 655f 6e6d  _bin = o.wave_nm
-00060540: 5f62 696e 2c20 7375 6270 6c6f 7420 3d20  _bin, subplot = 
-00060550: 5472 7565 2c20 636f 6c6f 725f 6f66 6673  True, color_offs
-00060560: 6574 203d 206c 656e 2872 656c 5f74 696d  et = len(rel_tim
-00060570: 6529 2a28 692b 3129 290d 0a09 0909 0909  e)*(i+1)).......
-00060580: 0909 0909 0d0a 0909 0969 6620 6e6f 7420  .........if not 
-00060590: 7363 616c 696e 675f 6661 696c 6564 3a0d  scaling_failed:.
-000605a0: 0a09 0909 0961 782e 7365 745f 7469 746c  .....ax.set_titl
-000605b0: 6528 2763 6f6d 7061 7265 206d 6561 7375  e('compare measu
-000605c0: 7265 6420 616e 6420 736d 6f6f 7468 6564  red and smoothed
-000605d0: 2064 6174 6120 6174 2067 6976 656e 2074   data at given t
-000605e0: 696d 6573 5c6e 2073 6361 6c65 6420 746f  imes\n scaled to
-000605f0: 2074 3d25 6720 7073 203a 2025 6720 7073   t=%g ps : %g ps
-00060600: 202c 2077 6c3d 2025 6720 6e6d 3a20 2567   , wl= %g nm: %g
-00060610: 206e 6d27 2528 6e6f 726d 5f77 696e 646f   nm'%(norm_windo
-00060620: 775b 305d 2c6e 6f72 6d5f 7769 6e64 6f77  w[0],norm_window
-00060630: 5b31 5d2c 6e6f 726d 5f77 696e 646f 775b  [1],norm_window[
-00060640: 325d 2c6e 6f72 6d5f 7769 6e64 6f77 5b33  2],norm_window[3
-00060650: 5d29 290d 0a09 0909 656c 7365 3a0d 0a09  ])).....else:...
-00060660: 0909 0961 782e 7365 745f 7469 746c 6528  ...ax.set_title(
-00060670: 2763 6f6d 7061 7265 206d 6561 7375 7265  'compare measure
-00060680: 6420 616e 6420 736d 6f6f 7468 6564 2064  d and smoothed d
-00060690: 6174 6120 6174 2067 6976 656e 2074 696d  ata at given tim
-000606a0: 6573 2729 0d0a 0909 0961 782e 6c65 6765  es').....ax.lege
-000606b0: 6e64 2868 616e 2c20 6c61 622c 206c 6162  nd(han, lab, lab
-000606c0: 656c 7370 6163 696e 6720 3d20 302c 206e  elspacing = 0, n
-000606d0: 636f 6c20 3d20 322c 2063 6f6c 756d 6e73  col = 2, columns
-000606e0: 7061 6369 6e67 203d 2031 2c20 6861 6e64  pacing = 1, hand
-000606f0: 6c65 6c65 6e67 7468 203d 2031 2c20 6672  lelength = 1, fr
-00060700: 616d 656f 6e20 3d20 4661 6c73 6529 0d0a  ameon = False)..
-00060710: 0909 0969 6620 7365 6c66 2e62 6f72 6465  ...if self.borde
-00060720: 7263 7574 2069 7320 4e6f 6e65 3a0d 0a09  rcut is None:...
-00060730: 0909 0961 782e 7365 745f 786c 696d 2873  ...ax.set_xlim(s
-00060740: 656c 662e 6473 2e63 6f6c 756d 6e73 2e76  elf.ds.columns.v
-00060750: 616c 7565 735b 305d 2c73 656c 662e 6473  alues[0],self.ds
-00060760: 2e63 6f6c 756d 6e73 2e76 616c 7565 735b  .columns.values[
-00060770: 2d31 5d29 0d0a 0909 0965 6c73 653a 0d0a  -1]).....else:..
-00060780: 0909 0909 6178 2e73 6574 5f78 6c69 6d28  ....ax.set_xlim(
-00060790: 7365 6c66 2e62 6f72 6465 7263 7574 290d  self.bordercut).
-000607a0: 0a09 0969 6620 7370 6563 7472 6120 6973  ...if spectra is
-000607b0: 206e 6f74 204e 6f6e 653a 0d0a 0909 0973   not None:.....s
-000607c0: 7065 6374 7261 2e70 6c6f 7428 6178 3d61  pectra.plot(ax=a
-000607d0: 782c 6c65 6765 6e64 3d46 616c 7365 290d  x,legend=False).
-000607e0: 0a09 0909 6861 6e64 6c65 732c 206c 6162  ....handles, lab
-000607f0: 656c 733d 6178 2e67 6574 5f6c 6567 656e  els=ax.get_legen
-00060800: 645f 6861 6e64 6c65 735f 6c61 6265 6c73  d_handles_labels
-00060810: 2829 0d0a 0909 0968 616e 2e61 7070 656e  ().....han.appen
-00060820: 6428 6861 6e64 6c65 735b 2d31 5d29 0d0a  d(handles[-1])..
-00060830: 0909 096c 6162 2e61 7070 656e 6428 6c61  ...lab.append(la
-00060840: 6265 6c73 5b2d 315d 290d 0a09 0909 6178  bels[-1]).....ax
-00060850: 2e6c 6567 656e 6428 6861 6e2c 206c 6162  .legend(han, lab
-00060860: 202c 6c61 6265 6c73 7061 6369 6e67 203d   ,labelspacing =
-00060870: 2030 2c20 6e63 6f6c 203d 2032 2c20 636f   0, ncol = 2, co
-00060880: 6c75 6d6e 7370 6163 696e 6720 3d20 312c  lumnspacing = 1,
-00060890: 2068 616e 646c 656c 656e 6774 6820 3d20   handlelength = 
-000608a0: 312c 2066 7261 6d65 6f6e 203d 2046 616c  1, frameon = Fal
-000608b0: 7365 290d 0a09 0969 6620 706c 6f74 5f73  se)....if plot_s
-000608c0: 6563 6f6e 645f 6173 5f65 6e65 7267 793a  econd_as_energy:
-000608d0: 0d0a 0909 0961 7832 3d61 782e 7477 696e  .....ax2=ax.twin
-000608e0: 7928 290d 0a09 0909 6178 322e 7365 745f  y().....ax2.set_
-000608f0: 786c 696d 2861 782e 6765 745f 786c 696d  xlim(ax.get_xlim
-00060900: 2829 290d 0a09 0909 6178 322e 7365 745f  ()).....ax2.set_
-00060910: 7874 6963 6b73 2861 782e 6765 745f 7874  xticks(ax.get_xt
-00060920: 6963 6b73 2829 290d 0a09 0909 6c61 6265  icks()).....labe
-00060930: 6c73 3d5b 2725 2e32 6627 2528 7363 6970  ls=['%.2f'%(scip
-00060940: 792e 636f 6e73 7461 6e74 732e 682a 7363  y.constants.h*sc
-00060950: 6970 792e 636f 6e73 7461 6e74 732e 632f  ipy.constants.c/
-00060960: 2861 2a31 652d 392a 7363 6970 792e 636f  (a*1e-9*scipy.co
-00060970: 6e73 7461 6e74 732e 656c 6563 7472 6f6e  nstants.electron
-00060980: 5f76 6f6c 7429 2920 666f 7220 6120 696e  _volt)) for a in
-00060990: 2061 7832 2e67 6574 5f78 7469 636b 7328   ax2.get_xticks(
-000609a0: 295d 0d0a 0909 095f 3d61 7832 2e73 6574  )]....._=ax2.set
-000609b0: 5f78 7469 636b 6c61 6265 6c73 286c 6162  _xticklabels(lab
-000609c0: 656c 7329 0d0a 0909 095f 3d61 7832 2e73  els)....._=ax2.s
-000609d0: 6574 5f78 6c61 6265 6c28 2745 6e65 7267  et_xlabel('Energ
-000609e0: 7920 696e 2065 5627 290d 0a09 0909 6178  y in eV').....ax
-000609f0: 2e73 6574 5f7a 6f72 6465 7228 6178 322e  .set_zorder(ax2.
-00060a00: 6765 745f 7a6f 7264 6572 2829 2b31 290d  get_zorder()+1).
-00060a10: 0a09 0966 6967 3d70 6c74 2e67 6366 2829  ...fig=plt.gcf()
-00060a20: 0d0a 0909 6669 672e 7469 6768 745f 6c61  ....fig.tight_la
-00060a30: 796f 7574 2829 0d0a 0909 6966 2073 656c  yout()....if sel
-00060a40: 662e 7361 7665 5f66 6967 7572 6573 5f74  f.save_figures_t
-00060a50: 6f5f 666f 6c64 6572 3a0d 0a09 0909 6669  o_folder:.....fi
-00060a60: 672e 7361 7665 6669 6728 6368 6563 6b5f  g.savefig(check_
-00060a70: 666f 6c64 6572 2870 6174 683d 7365 6c66  folder(path=self
-00060a80: 2e66 6967 7572 655f 7061 7468 2c66 696c  .figure_path,fil
-00060a90: 656e 616d 653d 2763 6f6d 7061 7265 5f61  ename='compare_a
-00060aa0: 745f 7469 6d65 5f25 732e 706e 6727 2527  t_time_%s.png'%'
-00060ab0: 5f27 2e6a 6f69 6e28 5b27 2567 2725 6120  _'.join(['%g'%a 
-00060ac0: 666f 7220 6120 696e 2072 656c 5f74 696d  for a in rel_tim
-00060ad0: 655d 2929 2c62 626f 785f 696e 6368 6573  e])),bbox_inches
-00060ae0: 3d27 7469 6768 7427 290d 0a09 0909 0909  ='tight').......
-00060af0: 0920 200d 0a0d 0a09 6465 6620 436f 6d70  .  .....def Comp
-00060b00: 6172 655f 6174 5f77 6176 6528 7365 6c66  are_at_wave(self
-00060b10: 2c20 7265 6c5f 7761 7665 203d 204e 6f6e  , rel_wave = Non
-00060b20: 652c 206f 7468 6572 203d 204e 6f6e 652c  e, other = None,
-00060b30: 2066 6974 7465 6420 3d20 4661 6c73 652c   fitted = False,
-00060b40: 206e 6f72 6d5f 7769 6e64 6f77 203d 204e   norm_window = N
-00060b50: 6f6e 652c 0d0a 0909 0909 0909 7769 6474  one,........widt
-00060b60: 6820 3d20 4e6f 6e65 2c20 636d 6170 203d  h = None, cmap =
-00060b70: 204e 6f6e 652c 2064 6174 615f 616e 645f   None, data_and_
-00060b80: 6669 7420 3d20 4661 6c73 652c 2073 6361  fit = False, sca
-00060b90: 6c65 5f74 7970 6520 3d20 2773 796d 6c6f  le_type = 'symlo
-00060ba0: 6727 2c20 6c69 6e65 7769 6474 6820 3d20  g', linewidth = 
-00060bb0: 3129 3a0d 0a09 0927 2727 5468 6973 2066  1):....'''This f
-00060bc0: 756e 6374 696f 6e20 706c 6f74 7320 6d75  unction plots mu
-00060bd0: 6c74 6970 6c65 206b 696e 6574 6963 7320  ltiple kinetics 
-00060be0: 696e 746f 2074 6865 2073 616d 6520 6669  into the same fi
-00060bf0: 6775 7265 2061 7420 6f6e 6520 6f72 0d0a  gure at one or..
-00060c00: 0909 6d75 6c74 6970 6c65 2067 6976 656e  ..multiple given
-00060c10: 2077 6176 656c 656e 6774 6820 2872 656c   wavelength (rel
-00060c20: 5f77 6176 6529 2061 6e64 2020 616c 6c6f  _wave) and  allo
-00060c30: 7773 2066 6f72 200d 0a09 093a 7265 663a  ws for ....:ref:
-00060c40: 604e 6f72 6d61 6c69 7a61 7469 6f6e 2061  `Normalization a
-00060c50: 6e64 2053 6361 6c69 6e67 6020 5665 7279  nd Scaling` Very
-00060c60: 2075 7365 6675 6c20 746f 2063 6f6d 7061   useful to compa
-00060c70: 7265 2074 6865 200d 0a09 096b 696e 6574  re the ....kinet
-00060c80: 6963 7320 666f 7220 6469 6666 6572 656e  ics for differen
-00060c90: 7420 7175 656e 6368 6572 2063 6f6e 6365  t quencher conce
-00060ca0: 6e74 7261 7469 6f6e 7320 6f72 2070 756d  ntrations or pum
-00060cb0: 7020 706f 7765 7273 2c20 0d0a 0909 6f72  p powers, ....or
-00060cc0: 2065 2e67 2e20 6469 6666 6572 656e 7420   e.g. different 
-00060cd0: 6669 7473 2e20 5468 6520 7061 7261 6d65  fits. The parame
-00060ce0: 7465 7220 7769 6474 6820 6f72 2074 6865  ter width or the
-00060cf0: 2067 656e 6572 616c 2073 656c 662e 7761   general self.wa
-00060d00: 7665 6c65 6e67 7468 5f62 696e 0d0a 0909  velength_bin....
-00060d10: 7768 6963 6820 6973 2075 7365 6420 6966  which is used if
-00060d20: 2077 6964 7468 2069 7320 4e6f 6e65 2028   width is None (
-00060d30: 4465 6661 756c 7429 2064 6566 696e 6573  Default) defines
-00060d40: 2074 6865 2077 6964 7468 206f 660d 0a09   the width of...
-00060d50: 0974 6865 2073 7065 6374 7261 6c20 7769  .the spectral wi
-00060d60: 6e64 6f77 2074 6861 7420 6973 2069 6e74  ndow that is int
-00060d70: 6567 7261 7465 6420 616e 6420 7368 6f77  egrated and show
-00060d80: 6e2e 0d0a 0d0a 0909 4120 6e6f 726d 616c  n.......A normal
-00060d90: 697a 6174 696f 6e20 7769 6e64 6f77 2063  ization window c
-00060da0: 616e 2062 6520 6769 7665 6e20 6174 2077  an be given at w
-00060db0: 6869 6368 2061 6c6c 2074 6865 2070 6c6f  hich all the plo
-00060dc0: 7474 6564 2063 7572 7665 7320 6172 6520  tted curves are 
-00060dd0: 6e6f 726d 616c 697a 6564 2074 6f2e 200d  normalized to. .
-00060de0: 0a09 0954 6869 7320 7769 6e64 6f77 2064  ...This window d
-00060df0: 6f65 7320 6e6f 7420 6861 7665 2074 6f20  oes not have to 
-00060e00: 6265 2069 6e20 7468 6520 706c 6f74 7465  be in the plotte
-00060e10: 6420 7265 6769 6f6e 2e20 5365 6520 3a72  d region. See :r
-00060e20: 6566 3a60 4e6f 726d 616c 697a 6174 696f  ef:`Normalizatio
-00060e30: 6e20 616e 6420 5363 616c 696e 6760 0d0a  n and Scaling`..
-00060e40: 0909 0d0a 0909 5061 7261 6d65 7465 7273  ......Parameters
-00060e50: 0d0a 0909 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ....------------
-00060e60: 2d2d 0d0a 0909 0d0a 0909 7265 6c5f 7761  --........rel_wa
-00060e70: 7665 203a 2066 6c6f 6174 206f 7220 6c69  ve : float or li
-00060e80: 7374 2f76 6563 746f 7220 286f 6620 666c  st/vector (of fl
-00060e90: 6f61 7473 290d 0a09 0909 5370 6563 6966  oats).....Specif
-00060ea0: 7920 7468 6520 7761 7665 6c65 6e67 7468  y the wavelength
-00060eb0: 2077 6865 7265 2074 6f20 706c 6f74 2074   where to plot t
-00060ec0: 6865 206b 696e 6574 6963 732c 2073 696e  he kinetics, sin
-00060ed0: 676c 6520 7661 6c75 6520 6f72 0d0a 0909  gle value or....
-00060ee0: 096c 6973 742f 7665 6374 6f72 206f 6620  .list/vector of 
-00060ef0: 7661 6c75 6573 2028 6f6e 6c79 206d 616e  values (only man
-00060f00: 6461 746f 7279 2065 6e74 7279 2920 466f  datory entry) Fo
-00060f10: 7220 6561 6368 2065 6e74 7279 2069 6e20  r each entry in 
-00060f20: 0d0a 0909 0972 656c 5f77 6176 6520 6120  .....rel_wave a 
-00060f30: 6b69 6e65 7469 6320 6973 2070 6c6f 7474  kinetic is plott
-00060f40: 6564 2e20 2772 656c 5f77 6176 6527 2061  ed. 'rel_wave' a
-00060f50: 6e64 2027 7769 6474 6827 200d 0a09 0909  nd 'width' .....
-00060f60: 2869 6e20 7468 6520 6f62 6a65 6374 2063  (in the object c
-00060f70: 616c 6c65 6420 2777 6176 656c 656e 6774  alled 'wavelengt
-00060f80: 685f 6269 6e27 2077 6f72 6b20 746f 6765  h_bin' work toge
-00060f90: 7468 6572 2066 6f72 2074 6865 2063 7265  ther for the cre
-00060fa0: 6174 696f 6e20 0d0a 0909 096f 6620 6b69  ation .....of ki
-00060fb0: 6e65 7469 6320 706c 6f74 732e 2041 7420  netic plots. At 
-00060fc0: 6561 6368 2073 656c 6563 7465 6420 7761  each selected wa
-00060fd0: 7665 6c65 6e67 7468 2074 6865 2064 6174  velength the dat
-00060fe0: 6120 6265 7477 6565 6e20 0d0a 0909 0977  a between .....w
-00060ff0: 6176 656c 656e 6774 682b 7769 6474 682f  avelength+width/
-00061000: 3220 616e 6420 7761 7665 6c65 6e67 7468  2 and wavelength
-00061010: 2d77 6964 7468 2f32 2069 7320 6176 6572  -width/2 is aver
-00061020: 6167 6564 200d 0a09 0909 666f 7220 6561  aged .....for ea
-00061030: 6368 2074 696d 6570 6f69 6e74 0d0a 0909  ch timepoint....
-00061040: 090d 0a09 096f 7468 6572 203a 2054 4120  .....other : TA 
-00061050: 6f62 6a65 6374 206f 7220 6c69 7374 206f  object or list o
-00061060: 6620 7468 6f73 652c 206f 7074 696f 6e61  f those, optiona
-00061070: 6c20 0d0a 0909 0973 686f 756c 6420 6265  l .....should be
-00061080: 2074 612e 706c 6f74 5f66 756e 6320 6f62   ta.plot_func ob
-00061090: 6a65 6374 7320 286c 6f61 6465 6420 6f72  jects (loaded or
-000610a0: 2063 6f70 6965 6429 2061 6e64 2069 7320   copied) and is 
-000610b0: 7768 6174 200d 0a09 0909 6973 2070 6c6f  what .....is plo
-000610c0: 7474 6564 2061 6761 696e 7374 2074 6865  tted against the
-000610d0: 2064 6174 6120 7573 6520 6120 6c69 7374   data use a list
-000610e0: 205b 7461 312c 7461 322c 2e2e 2e20 5d20   [ta1,ta2,... ] 
-000610f0: 6f72 2067 656e 6572 6174 6520 7468 6973  or generate this
-00061100: 0d0a 0909 096c 6973 7420 7573 696e 6720  .....list using 
-00061110: 7468 6520 4775 6920 6675 6e63 7469 6f6e  the Gui function
-00061120: 2e20 5365 6520 7365 6374 696f 6e20 3a72  . See section :r
-00061130: 6566 3a60 4f70 656e 696e 6720 6d75 6c74  ef:`Opening mult
-00061140: 6970 6c65 2066 696c 6573 6020 696e 200d  iple files` in .
-00061150: 0a09 0909 7468 6520 646f 6375 6d65 6e74  ....the document
-00061160: 6174 696f 6e0d 0a0d 0a09 0966 6974 7465  ation......fitte
-00061170: 6420 3a20 626f 6f6c 2c20 6f70 7469 6f6e  d : bool, option
-00061180: 616c 0d0a 0909 0954 7275 652f 4661 6c73  al.....True/Fals
-00061190: 6520 2844 6566 6175 6c74 2920 2d20 7573  e (Default) - us
-000611a0: 6520 6669 7474 6564 2064 6174 6120 696e  e fitted data in
-000611b0: 7374 6561 6420 6f66 2072 6177 2064 6174  stead of raw dat
-000611c0: 612e 200d 0a09 0909 4966 2054 7275 652c  a. .....If True,
-000611d0: 2074 6865 2066 6974 7465 6420 6461 7461   the fitted data
-000611e0: 706f 696e 7473 2028 7769 7468 6f75 7420  points (without 
-000611f0: 696e 7465 7270 6f6c 6174 696f 6e29 2061  interpolation) a
-00061200: 7265 2075 7365 642e 200d 0a09 0909 5468  re used. .....Th
-00061210: 6973 2069 7320 696e 7465 6e64 6564 2066  is is intended f
-00061220: 6f72 2063 6f6d 7061 7269 6e67 2065 2e67  or comparing e.g
-00061230: 2e20 6469 6666 6572 656e 7420 6669 7473  . different fits
-00061240: 0d0a 0d0a 0909 6e6f 726d 5f77 696e 646f  ......norm_windo
-00061250: 7720 3a20 4e6f 6e65 206f 7220 6c69 7374  w : None or list
-00061260: 2f76 6563 746f 7220 2877 6974 6820 3420  /vector (with 4 
-00061270: 666c 6f61 7473 292c 206f 7074 696f 6e61  floats), optiona
-00061280: 6c0d 0a09 0909 6e6f 726d 5f77 696e 646f  l.....norm_windo
-00061290: 7720 4769 7665 2061 206c 6973 742f 7475  w Give a list/tu
-000612a0: 7065 6c2f 7665 6374 6f72 2077 6974 6820  pel/vector with 
-000612b0: 3420 656e 7472 6965 7320 696e 2074 6865  4 entries in the
-000612c0: 206f 7264 6572 200d 0a09 0909 5b53 7461   order .....[Sta
-000612d0: 7274 202d 2074 696d 652c 2045 6e64 202d  rt - time, End -
-000612e0: 2074 696d 652c 2053 7461 7274 202d 2077   time, Start - w
-000612f0: 6176 656c 656e 6774 682c 2045 6e64 202d  avelength, End -
-00061300: 2057 6176 656c 656e 6774 685d 2c20 0d0a   Wavelength], ..
-00061310: 0909 0973 6565 2073 6563 7469 6f6e 203a  ...see section :
-00061320: 7265 663a 604e 6f72 6d61 6c69 7a61 7469  ref:`Normalizati
-00061330: 6f6e 2061 6e64 2053 6361 6c69 6e67 6020  on and Scaling` 
-00061340: 696e 2074 6865 2064 6f63 756d 656e 7461  in the documenta
-00061350: 7469 6f6e 2e0d 0a09 0909 4966 204e 6f6e  tion......If Non
-00061360: 6520 2844 6566 6175 6c74 2920 6e6f 206e  e (Default) no n
-00061370: 6f72 6d61 6c69 7a61 7469 6f6e 2069 7320  ormalization is 
-00061380: 646f 6e65 2e0d 0a0d 0a09 0977 6964 7468  done.......width
-00061390: 0d0a 0909 2020 2053 7065 6369 6679 2074  ....   Specify t
-000613a0: 6865 2077 6964 7468 2061 626f 7665 2061  he width above a
-000613b0: 6e64 2062 656c 6f77 2074 6865 2067 6976  nd below the giv
-000613c0: 656e 2077 6176 656c 656e 6774 6820 7468  en wavelength th
-000613d0: 6174 2069 730d 0a09 0920 2020 696e 7465  at is....   inte
-000613e0: 6772 6174 6564 2061 7320 7769 6e64 6f77  grated as window
-000613f0: 2e20 4966 206c 6566 7420 746f 2028 4465  . If left to (De
-00061400: 6661 756c 7429 2022 4e6f 6e65 2220 7468  fault) "None" th
-00061410: 6520 7661 6c75 6520 6672 6f6d 2074 6120  e value from ta 
-00061420: 6973 0d0a 0909 2020 2075 7365 642e 0d0a  is....   used...
-00061430: 0d0a 0909 6461 7461 5f61 6e64 5f66 6974  ....data_and_fit
-00061440: 203a 2062 6f6f 6c2c 206f 7074 696f 6e61   : bool, optiona
-00061450: 6c0d 0a09 0909 5472 7565 206f 7220 4661  l.....True or Fa
-00061460: 6c73 6520 2844 6566 6175 6c74 292c 2063  lse (Default), c
-00061470: 686f 6f73 6520 6966 2066 6f72 2074 6865  hoose if for the
-00061480: 2046 6974 7465 6420 706c 6f74 2074 6865   Fitted plot the
-00061490: 2072 6177 2064 6174 6120 6f66 2074 6865   raw data of the
-000614a0: 200d 0a09 0909 6f74 6865 7220 7072 6f6a   .....other proj
-000614b0: 6563 7473 2069 7320 746f 2062 6520 706c  ects is to be pl
-000614c0: 6f74 7469 6e67 2069 6e20 6164 6469 7469  otting in additi
-000614d0: 6f6e 2074 6f20 7468 6520 6669 7474 6564  on to the fitted
-000614e0: 206c 696e 652e 2046 6f72 2046 616c 7365   line. For False
-000614f0: 2028 4465 6661 756c 7429 0d0a 0909 094f   (Default).....O
-00061500: 6e6c 7920 7468 6520 6669 7420 6973 2070  nly the fit is p
-00061510: 6c6f 7474 6564 2e0d 0a09 0909 0d0a 0909  lotted..........
-00061520: 6c69 6e65 7769 6474 6820 3a20 666c 6f61  linewidth : floa
-00061530: 742c 206f 7074 696f 6e61 6c0d 0a09 0909  t, optional.....
-00061540: 6c69 6e65 7769 6474 6820 746f 2062 6520  linewidth to be 
-00061550: 7573 6564 2066 6f72 2070 6c6f 7474 696e  used for plottin
-00061560: 670d 0a09 0909 090d 0a09 0963 6d61 7020  g..........cmap 
-00061570: 3a20 4e6f 6e65 206f 7220 6d61 7470 6c6f  : None or matplo
-00061580: 746c 6962 2063 6f6c 6f72 206d 6170 2c20  tlib color map, 
-00061590: 6f70 7469 6f6e 616c 0d0a 0909 0969 7320  optional.....is 
-000615a0: 6120 706f 7765 7266 756c 6c20 7661 7269  a powerfull vari
-000615b0: 6162 6c65 2074 6861 7420 6368 6f6f 7365  able that choose
-000615c0: 7320 7468 6520 636f 6c6f 7572 206d 6170  s the colour map
-000615d0: 2061 7070 6c69 6564 2066 6f72 2061 6c6c   applied for all
-000615e0: 2070 6c6f 7473 2e20 4966 2073 6574 2074   plots. If set t
-000615f0: 6f20 0d0a 0909 094e 6f6e 6520 2844 6566  o .....None (Def
-00061600: 6175 6c74 2920 7468 656e 2074 6865 2073  ault) then the s
-00061610: 656c 662e 636d 6170 2069 7320 7573 6564  elf.cmap is used
-00061620: 2e0d 0a09 0909 4173 2073 7461 6e64 6172  ......As standar
-00061630: 6420 4920 7573 6520 7468 6520 636f 6c6f  d I use the colo
-00061640: 7220 6d61 7020 226a 6574 2220 6672 6f6d  r map "jet" from
-00061650: 206d 6174 706c 6f74 6c69 622e 2054 6865   matplotlib. The
-00061660: 7265 2061 7265 2061 2076 6172 6965 7479  re are a variety
-00061670: 206f 6620 636f 6c6f 726d 6170 7320 0d0a   of colormaps ..
-00061680: 0909 0961 7661 696c 6162 6c65 2074 6861  ...available tha
-00061690: 7420 6172 6520 7665 7279 2075 7365 6675  t are very usefu
-000616a0: 6c6c 2e20 4265 7369 6465 2022 6a65 7422  ll. Beside "jet"
-000616b0: 2c20 2276 6972 6964 6973 2220 6973 2061  , "viridis" is a
-000616c0: 2067 6f6f 6420 6368 6f69 6365 2061 7320   good choice as 
-000616d0: 6974 2069 7320 7765 6c6c 200d 0a09 0909  it is well .....
-000616e0: 7669 7369 626c 6520 756e 6465 7220 7265  visible under re
-000616f0: 642d 6772 6565 6e20 626c 696e 646e 6573  d-green blindnes
-00061700: 732e 204f 7468 6572 2075 7365 6675 6c20  s. Other useful 
-00061710: 6d61 7073 2061 7265 2022 7072 6973 6d22  maps are "prism"
-00061720: 2066 6f72 2068 6967 6820 666c 7563 7475   for high fluctu
-00061730: 6174 696f 6e73 200d 0a09 0909 6f72 2064  ations .....or d
-00061740: 6976 6572 6769 6e67 2063 6f6c 6f72 206d  iverging color m
-00061750: 6170 7320 6c69 6b65 2022 7365 6973 6d69  aps like "seismi
-00061760: 6322 2e20 0d0a 0909 0953 6565 2068 7474  c". .....See htt
-00061770: 7073 3a2f 2f6d 6174 706c 6f74 6c69 622e  ps://matplotlib.
-00061780: 6f72 672f 332e 312e 302f 7475 746f 7269  org/3.1.0/tutori
-00061790: 616c 732f 636f 6c6f 7273 2f63 6f6c 6f72  als/colors/color
-000617a0: 6d61 7073 2e68 746d 6c20 666f 7220 6120  maps.html for a 
-000617b0: 636f 6d70 7265 6865 6e73 6976 6520 0d0a  comprehensive ..
-000617c0: 0909 0973 656c 6563 7469 6f6e 2e20 496e  ...selection. In
-000617d0: 2074 6865 2063 6f64 6520 7468 6520 636f   the code the co
-000617e0: 6c6f 726d 6170 7320 6172 6520 696d 706f  lormaps are impo
-000617f0: 7274 6564 2073 6f20 6966 2070 6c6f 745f  rted so if plot_
-00061800: 6675 6e63 2069 7320 696d 706f 7274 6564  func is imported
-00061810: 2061 7320 7066 2074 6865 6e20 0d0a 0909   as pf then ....
-00061820: 0973 656c 662e 636d 6170 3d70 662e 636d  .self.cmap=pf.cm
-00061830: 2e76 6972 6964 6973 2073 6574 7320 7669  .viridis sets vi
-00061840: 7269 6469 7320 6173 2074 6865 206d 6170  ridis as the map
-00061850: 2074 6f20 7573 652e 2049 6e74 6572 6e61   to use. Interna
-00061860: 6c6c 7920 7468 6520 636f 6c6f 7273 2061  lly the colors a
-00061870: 7265 2063 686f 7365 6e20 0d0a 0909 0977  re chosen .....w
-00061880: 6974 6820 7468 6520 2263 6f6c 6d22 2066  ith the "colm" f
-00061890: 756e 6374 696f 6e2e 2054 6865 2032 6420  unction. The 2d 
-000618a0: 706c 6f74 7320 7265 7175 6972 6520 6120  plots require a 
-000618b0: 636f 6e74 696e 756f 7573 2063 6f6c 6f72  continuous color
-000618c0: 206d 6170 2073 6f20 6966 2073 6f6d 6574   map so if somet
-000618d0: 6869 6e67 200d 0a09 0909 656c 7365 2069  hing .....else i
-000618e0: 7320 6769 7665 2032 6420 706c 6f74 7320  s give 2d plots 
-000618f0: 6172 6520 7368 6f77 6e20 6175 746f 6d61  are shown automa
-00061900: 7469 6361 6c6c 7920 7769 7468 2022 6a65  tically with "je
-00061910: 7422 2e20 466f 7220 616c 6c20 6f66 2074  t". For all of t
-00061920: 6865 2031 6420 706c 6f74 7320 686f 7765  he 1d plots howe
-00061930: 7665 7220 0d0a 0909 0949 2066 6972 7374  ver .....I first
-00061940: 2073 656c 6563 7420 6120 6e75 6d62 6572   select a number
-00061950: 206f 6620 636f 6c6f 7273 2062 6566 6f72   of colors befor
-00061960: 6520 6561 6368 2070 6c6f 742e 2049 6620  e each plot. If 
-00061970: 636d 6170 2069 7320 6120 636f 6e74 696e  cmap is a contin
-00061980: 6f75 7320 6d61 7020 7468 656e 2074 6865  ous map then the
-00061990: 7365 0d0a 0909 0961 7265 2073 616d 706c  se.....are sampl
-000619a0: 6564 2065 7665 6e6c 7920 6f76 6572 2074  ed evenly over t
-000619b0: 6865 2063 6f6c 6f75 726d 6170 2e20 4d61  he colourmap. Ma
-000619c0: 6e75 616c 2069 7465 7261 626c 6573 206f  nual iterables o
-000619d0: 6620 636f 6c6f 7572 7320 0d0a 0909 0963  f colours .....c
-000619e0: 6d61 703d 5b28 312c 302c 3029 2c28 302c  map=[(1,0,0),(0,
-000619f0: 312c 3029 2c28 302c 302c 3129 2c2e 2e2e  1,0),(0,0,1),...
-00061a00: 5d20 6172 6520 616c 736f 2061 6363 6570  ] are also accep
-00061a10: 7465 642c 2061 7320 6172 6520 7665 6374  ted, as are vect
-00061a20: 6f72 7320 6f72 2064 6174 6166 7261 6d65  ors or dataframe
-00061a30: 7320 7468 6174 200d 0a09 0909 636f 6e74  s that .....cont
-00061a40: 6169 6e20 6173 2072 6f77 7320 7468 6520  ain as rows the 
-00061a50: 636f 6c6f 7273 2e20 5468 6572 6520 6d75  colors. There mu
-00061a60: 7374 2062 6520 6f66 2063 6f75 7273 6520  st be of course 
-00061a70: 7375 6666 6963 6965 6e74 2063 6f6c 6f72  sufficient color
-00061a80: 7320 7072 6573 656e 7420 666f 7220 0d0a  s present for ..
-00061a90: 0909 0974 6865 206e 756d 6265 7273 206f  ...the numbers o
-00061aa0: 6620 6c69 6e65 7320 7468 6174 2077 696c  f lines that wil
-00061ab0: 6c20 6265 2070 6c6f 7474 6564 2e20 536f  l be plotted. So
-00061ac0: 2049 2072 6563 6f6d 6d65 6e64 2074 6f20   I recommend to 
-00061ad0: 7072 6f76 6964 6520 6174 206c 6561 7374  provide at least
-00061ae0: 2031 3020 636f 6c6f 7572 7320 0d0a 0909   10 colours ....
-00061af0: 0928 652e 672e 7e79 6f75 7220 756e 6976  .(e.g.~your univ
-00061b00: 6572 7369 7479 2063 6f6c 6f72 7329 2e20  ersity colors). 
-00061b10: 636f 6c6f 7572 7320 6172 6520 616c 7761  colours are alwa
-00061b20: 7973 2067 6976 656e 2061 7320 612c 206c  ys given as a, l
-00061b30: 6973 7420 6f72 2074 7570 6c65 2077 6974  ist or tuple wit
-00061b40: 6820 5247 4120 6f72 2052 4742 410d 0a09  h RGA or RGBA...
-00061b50: 0909 2877 6974 6820 7468 6520 6c61 7374  ..(with the last
-00061b60: 2041 2062 6565 696e 6720 7468 6520 416c   A beeing the Al
-00061b70: 7068 613d 7472 616e 7370 6172 656e 6379  pha=transparency
-00061b80: 2e20 416c 6c20 6e75 6d62 6572 7320 6172  . All numbers ar
-00061b90: 6520 6265 7477 6565 6e20 3020 616e 6420  e between 0 and 
-00061ba0: 312e 200d 0a09 0909 4966 2061 206c 6973  1. .....If a lis
-00061bb0: 742f 7665 6374 6f72 2f44 6174 6146 7261  t/vector/DataFra
-00061bc0: 6d65 2069 7320 6769 7665 6e20 666f 7220  me is given for 
-00061bd0: 7468 6520 636f 6c6f 7572 7320 7468 6579  the colours they
-00061be0: 2077 696c 6c20 6265 2075 7365 6420 696e   will be used in
-00061bf0: 2074 6865 206f 7264 6572 2070 726f 7669   the order provi
-00061c00: 6465 642e 0d0a 0909 0d0a 0909 5363 616c  ded.........Scal
-00061c10: 655f 7479 7065 203a 204e 6f6e 6520 6f72  e_type : None or
-00061c20: 2073 7472 0d0a 0909 0969 7320 6120 6765   str.....is a ge
-00061c30: 6e65 7261 6c20 7365 7474 696e 6720 7468  neral setting th
-00061c40: 6174 2063 616e 2069 6e66 6c75 656e 6365  at can influence
-00061c50: 7320 7768 6174 2074 696d 6520 6178 6973  s what time axis
-00061c60: 2077 696c 6c20 6265 2075 7365 6420 666f   will be used fo
-00061c70: 7220 7468 6520 706c 6f74 732e 200d 0a09  r the plots. ...
-00061c80: 0909 2273 796d 6c6f 6722 2028 6c69 6e65  .."symlog" (line
-00061c90: 6172 2061 726f 756e 6420 7a65 726f 2061  ar around zero a
-00061ca0: 6e64 206c 6f67 6172 6974 686d 6963 206f  nd logarithmic o
-00061cb0: 7468 6572 7769 7365 2920 226c 696e 2220  therwise) "lin" 
-00061cc0: 616e 6420 226c 6f67 2220 6172 6520 7661  and "log" are va
-00061cd0: 6c69 6420 6f70 7469 6f6e 732e 090d 0a09  lid options.....
-00061ce0: 0909 0909 0d0a 0909 4578 616d 706c 6573  ........Examples
-00061cf0: 0d0a 0909 2d2d 2d2d 2d2d 2d2d 0d0a 0909  ....--------....
-00061d00: 0d0a 0909 3e3e 3e20 696d 706f 7274 2070  ....>>> import p
-00061d10: 6c6f 745f 6675 6e63 2061 7320 7066 0d0a  lot_func as pf..
-00061d20: 0909 3e3e 3e20 7461 203d 2070 662e 5441  ..>>> ta = pf.TA
-00061d30: 2827 7465 7374 312e 6864 6635 2729 2023  ('test1.hdf5') #
-00061d40: 6f70 656e 2074 6865 206f 7269 6769 6e61  open the origina
-00061d50: 6c20 7072 6f6a 6563 740d 0a09 090d 0a09  l project.......
-00061d60: 094e 6f77 206f 7065 6e20 6120 6275 6e63  .Now open a bunc
-00061d70: 6820 6f66 206f 7468 6572 2070 726f 6a65  h of other proje
-00061d80: 6374 7320 746f 2063 6f6d 7061 7265 2061  cts to compare a
-00061d90: 6761 696e 7374 0d0a 0909 0d0a 0909 3e3e  gainst........>>
-00061da0: 3e20 6f74 6865 725f 7072 6f6a 6563 7473  > other_projects
-00061db0: 203d 2070 662e 4755 495f 6f70 656e 2870   = pf.GUI_open(p
-00061dc0: 726f 6a65 6374 5f6c 6973 7420 3d20 5b27  roject_list = ['
-00061dd0: 6669 6c65 312e 5349 4127 2c20 2766 696c  file1.SIA', 'fil
-00061de0: 6532 2e53 4941 275d 290d 0a09 090d 0a09  e2.SIA']).......
-00061df0: 0954 7970 6963 616c 2075 7365 3a0d 0a09  .Typical use:...
-00061e00: 0943 6f6d 7061 7265 2074 6865 2072 6177  .Compare the raw
-00061e10: 2064 6174 6120 7769 7468 6f75 7420 6e6f   data without no
-00061e20: 726d 616c 697a 6174 696f 6e20 6174 2034  rmalization at 4
-00061e30: 3030 206e 6d20 616e 6420 3530 3020 6e6d  00 nm and 500 nm
-00061e40: 0d0a 0909 0d0a 0909 3e3e 3e20 7461 2e43  ........>>> ta.C
-00061e50: 6f6d 7061 7265 5f61 745f 7761 7665 2872  ompare_at_wave(r
-00061e60: 656c 5f77 6176 6520 3d20 5b34 3030 2c20  el_wave = [400, 
-00061e70: 3530 305d 2c20 6f74 6865 7273 203d 206f  500], others = o
-00061e80: 7468 6572 5f70 726f 6a65 6374 290d 0a09  ther_project)...
-00061e90: 090d 0a09 0943 6f6d 7061 7265 2074 6865  .....Compare the
-00061ea0: 2071 7561 6c69 7479 206f 6620 7468 6520   quality of the 
-00061eb0: 6669 7420 6461 7461 2077 6974 686f 7574  fit data without
-00061ec0: 206e 6f72 6d61 6c69 7a61 7469 6f6e 2061   normalization a
-00061ed0: 7420 3430 3020 6e6d 2061 6e64 2035 3030  t 400 nm and 500
-00061ee0: 206e 6d0d 0a09 090d 0a09 093e 3e3e 2074   nm........>>> t
-00061ef0: 612e 436f 6d70 6172 655f 6174 5f77 6176  a.Compare_at_wav
-00061f00: 6528 7265 6c5f 7761 7665 203d 205b 3430  e(rel_wave = [40
-00061f10: 302c 2035 3030 5d2c 206f 7468 6572 7320  0, 500], others 
-00061f20: 3d20 6f74 6865 725f 7072 6f6a 6563 742c  = other_project,
-00061f30: 2066 6974 7465 6420 3d20 5472 7565 290d   fitted = True).
-00061f40: 0a09 090d 0a09 0943 6f6d 7061 7265 2077  .......Compare w
-00061f50: 6974 6820 6e6f 726d 616c 697a 6174 696f  ith normalizatio
-00061f60: 6e20 7769 6e64 6f77 2062 6574 7765 656e  n window between
-00061f70: 2031 7073 2061 6e64 2032 7073 2061 6e64   1ps and 2ps and
-00061f80: 2034 3030 6e6d 2061 6e64 2034 3530 6e6d   400nm and 450nm
-00061f90: 0d0a 0909 0d0a 0909 3e3e 3e20 6e6f 726d  ........>>> norm
-00061fa0: 5f77 696e 646f 773d 5b31 2c32 2c34 3030  _window=[1,2,400
-00061fb0: 2c34 3530 5d0d 0a09 093e 3e3e 2074 612e  ,450]....>>> ta.
-00061fc0: 436f 6d70 6172 655f 6174 5f77 6176 6528  Compare_at_wave(
-00061fd0: 7265 6c5f 7761 7665 203d 205b 3430 302c  rel_wave = [400,
-00061fe0: 2035 3030 5d2c 206f 7468 6572 7320 3d20   500], others = 
-00061ff0: 6f74 6865 725f 7072 6f6a 6563 742c 206e  other_project, n
-00062000: 6f72 6d5f 7769 6e64 6f77 203d 206e 6f72  orm_window = nor
-00062010: 6d5f 7769 6e64 6f77 290d 0a09 090d 0a09  m_window).......
-00062020: 0955 7365 2065 7861 6d70 6c65 3a20 4f66  .Use example: Of
-00062030: 7465 6e20 7468 6572 6520 6172 6520 6120  ten there are a 
-00062040: 6c6f 7420 6f66 2064 6966 6665 7265 6e74  lot of different
-00062050: 206d 6561 7375 7265 6d65 6e74 7320 746f   measurements to
-00062060: 200d 0a09 0963 6f6d 7061 7265 2061 7420   ....compare at 
-00062070: 6d75 6c74 6970 6c65 2077 6176 656c 656e  multiple wavelen
-00062080: 6774 682e 2054 6865 206e 6f72 6d6c 697a  gth. The normliz
-00062090: 6174 696f 6e20 6973 2070 6572 666f 726d  ation is perform
-000620a0: 6564 2061 7420 7468 6520 6772 6f75 6e64  ed at the ground
-000620b0: 2073 7461 7465 2062 6c65 6163 680d 0a09   state bleach...
-000620c0: 0934 3630 206e 6d20 616e 6420 6561 726c  .460 nm and earl
-000620d0: 7920 696e 2074 696d 652e 2054 6865 6e20  y in time. Then 
-000620e0: 6974 2069 7320 6265 7474 6572 2074 6f20  it is better to 
-000620f0: 6d61 6b65 2061 206e 6577 2070 6c6f 7420  make a new plot 
-00062100: 666f 7220 6561 6368 200d 0a09 0977 6176  for each ....wav
-00062110: 656c 656e 6774 682e 2054 6865 206e 6f72  elength. The nor
-00062120: 6d61 6c69 7a61 7469 6f6e 2077 696e 646f  malization windo
-00062130: 7720 7374 6179 7320 6669 7865 642e 0d0a  w stays fixed...
-00062140: 0909 0d0a 0909 3e3e 3e20 706c 742e 636c  ......>>> plt.cl
-00062150: 6f73 6528 2761 6c6c 2729 2023 6d61 6b65  ose('all') #make
-00062160: 2073 6f6d 6520 7370 6163 650d 0a09 093e   some space....>
-00062170: 3e3e 206e 6f72 6d5f 7769 6e64 6f77 3d5b  >> norm_window=[
-00062180: 302e 332c 302e 352c 3435 302c 3437 305d  0.3,0.5,450,470]
-00062190: 2023 6465 6669 6e65 2077 696e 646f 7720   #define window 
-000621a0: 696e 2067 726f 756e 6420 7374 6174 6520  in ground state 
-000621b0: 626c 6561 6368 0d0a 0909 3e3e 3e20 666f  bleach....>>> fo
-000621c0: 7220 7761 7665 2069 6e20 5b33 3030 2c34  r wave in [300,4
-000621d0: 3030 2c35 3030 2c36 3030 2c37 3030 5d3a  00,500,600,700]:
-000621e0: 2023 6974 6572 6174 6520 6f76 6572 2074   #iterate over t
-000621f0: 6865 2077 6176 656c 656e 6774 6820 0d0a  he wavelength ..
-00062200: 0909 3e3e 3e20 0974 612e 436f 6d70 6172  ..>>> .ta.Compar
-00062210: 655f 6174 5f77 6176 6528 7265 6c5f 7761  e_at_wave(rel_wa
-00062220: 7665 203d 2077 6176 652c 206f 7468 6572  ve = wave, other
-00062230: 7320 3d20 6f74 6865 725f 7072 6f6a 6563  s = other_projec
-00062240: 742c 206e 6f72 6d5f 7769 6e64 6f77 203d  t, norm_window =
-00062250: 206e 6f72 6d5f 7769 6e64 6f77 290d 0a09   norm_window)...
-00062260: 090d 0a09 0927 2727 090d 0a09 090d 0a09  .....'''........
-00062270: 0969 6620 7365 6c66 2e73 6176 655f 6669  .if self.save_fi
-00062280: 6775 7265 735f 746f 5f66 6f6c 6465 723a  gures_to_folder:
-00062290: 7365 6c66 2e66 6967 7572 655f 7061 7468  self.figure_path
-000622a0: 3d63 6865 636b 5f66 6f6c 6465 7228 7061  =check_folder(pa
-000622b0: 7468 3d27 7265 7375 6c74 5f66 6967 7572  th='result_figur
-000622c0: 6573 272c 6375 7272 656e 745f 7061 7468  es',current_path
-000622d0: 3d73 656c 662e 7061 7468 290d 0a09 0969  =self.path)....i
-000622e0: 6620 7769 6474 6820 6973 204e 6f6e 653a  f width is None:
-000622f0: 7769 6474 683d 7365 6c66 2e77 6176 656c  width=self.wavel
-00062300: 656e 6774 685f 6269 6e0d 0a09 0969 6620  ength_bin....if 
-00062310: 7265 6c5f 7761 7665 2069 7320 4e6f 6e65  rel_wave is None
-00062320: 3a0d 0a09 0909 7265 6c5f 7761 7665 3d73  :.....rel_wave=s
-00062330: 656c 662e 7265 6c5f 7761 7665 0d0a 0909  elf.rel_wave....
-00062340: 6966 206f 7468 6572 2069 7320 6e6f 7420  if other is not 
-00062350: 4e6f 6e65 3a0d 0a09 0909 6966 206e 6f74  None:.....if not
-00062360: 2068 6173 6174 7472 286f 7468 6572 2c27   hasattr(other,'
-00062370: 5f5f 6974 6572 5f5f 2729 3a6f 7468 6572  __iter__'):other
-00062380: 3d5b 6f74 6865 725d 0d0a 0909 6966 206e  =[other]....if n
-00062390: 6f74 2068 6173 6174 7472 2872 656c 5f77  ot hasattr(rel_w
-000623a0: 6176 652c 275f 5f69 7465 725f 5f27 293a  ave,'__iter__'):
-000623b0: 0d0a 0909 0972 656c 5f77 6176 653d 5b72  .....rel_wave=[r
-000623c0: 656c 5f77 6176 655d 0d0a 0909 6966 2063  el_wave]....if c
-000623d0: 6d61 7020 6973 204e 6f6e 653a 636d 6170  map is None:cmap
-000623e0: 3d73 656c 662e 636d 6170 0d0a 0909 6966  =self.cmap....if
-000623f0: 2066 6974 7465 643a 0d0a 0909 0974 7279   fitted:.....try
-00062400: 3a0d 0a09 0909 0972 653d 7365 6c66 2e72  :......re=self.r
-00062410: 650d 0a09 0909 6578 6365 7074 3a0d 0a09  e.....except:...
-00062420: 0909 0970 7269 6e74 2822 4e6f 2066 6974  ...print("No fit
-00062430: 7465 6420 7265 7375 6c74 7320 7072 6573  ted results pres
-00062440: 656e 7422 290d 0a09 0909 0972 6574 7572  ent")......retur
-00062450: 6e20 4661 6c73 650d 0a09 0909 6966 206e  n False.....if n
-00062460: 6f72 6d5f 7769 6e64 6f77 2069 7320 6e6f  orm_window is no
-00062470: 7420 4e6f 6e65 3a0d 0a09 0909 0972 6566  t None:......ref
-00062480: 5f73 6361 6c65 203d 2072 655b 2741 275d  _scale = re['A']
-00062490: 2e6c 6f63 5b6e 6f72 6d5f 7769 6e64 6f77  .loc[norm_window
-000624a0: 5b30 5d3a 6e6f 726d 5f77 696e 646f 775b  [0]:norm_window[
-000624b0: 315d 2c20 6e6f 726d 5f77 696e 646f 775b  1], norm_window[
-000624c0: 325d 3a6e 6f72 6d5f 7769 6e64 6f77 5b33  2]:norm_window[3
-000624d0: 5d5d 2e6d 6561 6e28 292e 6d65 616e 2829  ]].mean().mean()
-000624e0: 0d0a 0909 0966 6967 2c20 6178 203d 2070  .....fig, ax = p
-000624f0: 6c74 2e73 7562 706c 6f74 7328 6669 6773  lt.subplots(figs
-00062500: 697a 6520 3d20 2831 302c 2036 292c 2064  ize = (10, 6), d
-00062510: 7069 203d 2031 3030 290d 0a09 0909 636f  pi = 100).....co
-00062520: 6c6f 7273 203d 2063 6f6c 6d28 636d 6170  lors = colm(cmap
-00062530: 203d 2063 6d61 702c 206b 203d 2072 616e   = cmap, k = ran
-00062540: 6765 286c 656e 2872 656c 5f77 6176 6529  ge(len(rel_wave)
-00062550: 2a28 322b 6c65 6e28 6f74 6865 7229 2929  *(2+len(other)))
-00062560: 290d 0a09 0909 6178 203d 2070 6c6f 7431  ).....ax = plot1
-00062570: 6428 7265 5b27 4127 5d2c 2061 7820 3d20  d(re['A'], ax = 
-00062580: 6178 2c20 7761 7665 6c65 6e67 7468 203d  ax, wavelength =
-00062590: 2072 656c 5f77 6176 652c 2077 6964 7468   rel_wave, width
-000625a0: 203d 2077 6964 7468 2c20 6c69 6e65 735f   = width, lines_
-000625b0: 6172 6520 3d20 2764 6174 6127 2c20 0d0a  are = 'data', ..
-000625c0: 0909 0909 0909 636d 6170 203d 2063 6f6c  ......cmap = col
-000625d0: 6f72 732c 2074 6974 6c65 203d 2027 272c  ors, title = '',
-000625e0: 2070 6c6f 745f 7479 7065 203d 2073 6361   plot_type = sca
-000625f0: 6c65 5f74 7970 652c 206c 696e 6577 6964  le_type, linewid
-00062600: 7468 203d 206c 696e 6577 6964 7468 290d  th = linewidth).
-00062610: 0a09 0909 6178 203d 2070 6c6f 7431 6428  ....ax = plot1d(
-00062620: 7265 5b27 4143 275d 2c20 6178 203d 2061  re['AC'], ax = a
-00062630: 782c 2077 6176 656c 656e 6774 6820 3d20  x, wavelength = 
-00062640: 7265 6c5f 7761 7665 2c20 7769 6474 6820  rel_wave, width 
-00062650: 3d20 7769 6474 682c 206c 696e 6573 5f61  = width, lines_a
-00062660: 7265 203d 2027 6669 7474 6564 272c 200d  re = 'fitted', .
-00062670: 0a09 0909 0909 0963 6d61 7020 3d20 636f  .......cmap = co
-00062680: 6c6f 7273 2c20 7469 746c 6520 3d20 2727  lors, title = ''
-00062690: 2c20 7375 6270 6c6f 7420 3d20 5472 7565  , subplot = True
-000626a0: 2c20 706c 6f74 5f74 7970 6520 3d20 7363  , plot_type = sc
-000626b0: 616c 655f 7479 7065 2c20 6c69 6e65 7769  ale_type, linewi
-000626c0: 6474 6820 3d20 6c69 6e65 7769 6474 6829  dth = linewidth)
-000626d0: 0d0a 0909 0923 6178 203d 2070 6c6f 7431  .....#ax = plot1
-000626e0: 6428 7265 5b27 4143 275d 2c20 6178 203d  d(re['AC'], ax =
-000626f0: 2061 782c 2077 6176 656c 656e 6774 6820   ax, wavelength 
-00062700: 3d20 7265 6c5f 7761 7665 2c20 7769 6474  = rel_wave, widt
-00062710: 6820 3d20 7769 6474 682c 206c 696e 6573  h = width, lines
-00062720: 5f61 7265 203d 2027 6669 7474 6564 272c  _are = 'fitted',
-00062730: 200d 0a09 0909 2309 0909 636d 6170 203d   .....#...cmap =
-00062740: 2063 6f6c 6f72 732c 2063 6f6c 6f72 5f6f   colors, color_o
-00062750: 6666 7365 7420 3d20 6c65 6e28 7265 6c5f  ffset = len(rel_
-00062760: 7761 7665 292c 2074 6974 6c65 203d 2027  wave), title = '
-00062770: 272c 2073 7562 706c 6f74 203d 2054 7275  ', subplot = Tru
-00062780: 652c 2070 6c6f 745f 7479 7065 203d 2073  e, plot_type = s
-00062790: 6361 6c65 5f74 7970 6529 0d0a 0909 0968  cale_type).....h
-000627a0: 616e 642c 2020 6c61 6265 6c73 203d 2061  and,  labels = a
-000627b0: 782e 6765 745f 6c65 6765 6e64 5f68 616e  x.get_legend_han
-000627c0: 646c 6573 5f6c 6162 656c 7328 290d 0a09  dles_labels()...
-000627d0: 0909 6c61 623d 5b27 2567 206e 6d27 2561  ..lab=['%g nm'%a
-000627e0: 202b 2027 5f27 202b 2073 7472 2873 656c   + '_' + str(sel
-000627f0: 662e 6669 6c65 6e61 6d65 2920 666f 7220  f.filename) for 
-00062800: 6120 696e 2072 656c 5f77 6176 655d 0d0a  a in rel_wave]..
-00062810: 0909 0966 6f72 2065 6e74 2069 6e20 7265  ...for ent in re
-00062820: 6c5f 7761 7665 3a0d 0a09 0909 096c 6162  l_wave:......lab
-00062830: 2e61 7070 656e 6428 2725 6720 6e6d 2725  .append('%g nm'%
-00062840: 656e 7420 2b20 275f 2720 2b20 7374 7228  ent + '_' + str(
-00062850: 7365 6c66 2e66 696c 656e 616d 6529 290d  self.filename)).
-00062860: 0a09 0909 0d0a 0909 0969 6620 6f74 6865  .........if othe
-00062870: 7220 6973 206e 6f74 204e 6f6e 653a 0d0a  r is not None:..
-00062880: 0909 0909 666f 7220 692c 6f20 696e 2065  ....for i,o in e
-00062890: 6e75 6d65 7261 7465 286f 7468 6572 293a  numerate(other):
-000628a0: 0d0a 0909 0909 0969 2b3d 310d 0a09 0909  .......i+=1.....
-000628b0: 0909 636f 6c6f 725f 6f66 6673 6574 3d28  ..color_offset=(
-000628c0: 692b 3129 2a6c 656e 2872 656c 5f77 6176  i+1)*len(rel_wav
-000628d0: 6529 0d0a 0909 0909 0974 7279 3a0d 0a09  e).......try:...
-000628e0: 0909 0909 0972 653d 6f2e 7265 0d0a 0909  .....re=o.re....
-000628f0: 0909 0965 7863 6570 743a 0d0a 0909 0909  ...except:......
-00062900: 0909 7072 696e 7428 2725 7320 6861 7320  ..print('%s has 
-00062910: 6e6f 2066 6974 7465 6420 7265 7375 6c74  no fitted result
-00062920: 7327 256f 2e66 696c 656e 616d 6529 0d0a  s'%o.filename)..
-00062930: 0909 0909 0909 636f 6e74 696e 7565 0d0a  ......continue..
-00062940: 0909 0909 0969 6620 6e6f 726d 5f77 696e  .....if norm_win
-00062950: 646f 7720 6973 206e 6f74 204e 6f6e 653a  dow is not None:
-00062960: 0d0a 0909 0909 0909 7265 6c5f 7363 616c  ........rel_scal
-00062970: 653d 7265 5b27 4127 5d2e 6c6f 635b 6e6f  e=re['A'].loc[no
-00062980: 726d 5f77 696e 646f 775b 305d 3a6e 6f72  rm_window[0]:nor
-00062990: 6d5f 7769 6e64 6f77 5b31 5d2c 6e6f 726d  m_window[1],norm
-000629a0: 5f77 696e 646f 775b 325d 3a6e 6f72 6d5f  _window[2]:norm_
-000629b0: 7769 6e64 6f77 5b33 5d5d 2e6d 6561 6e28  window[3]].mean(
-000629c0: 292e 6d65 616e 2829 0d0a 0909 0909 0909  ).mean()........
-000629d0: 0909 0909 0909 0920 0d0a 0909 0909 0909  ....... ........
-000629e0: 7472 793a 0d0a 0909 0909 0909 0973 6361  try:.........sca
-000629f0: 6c69 6e67 3d28 7265 6c5f 7363 616c 6520  ling=(rel_scale 
-00062a00: 2f20 7265 665f 7363 616c 6529 0d0a 0909  / ref_scale)....
-00062a10: 0909 0909 0969 6620 6461 7461 5f61 6e64  .....if data_and
-00062a20: 5f66 6974 3a0d 0a09 0909 0909 0909 0961  _fit:..........a
-00062a30: 7820 3d20 706c 6f74 3164 2872 655b 2741  x = plot1d(re['A
-00062a40: 275d 2f73 6361 6c69 6e67 2c20 636d 6170  ']/scaling, cmap
-00062a50: 203d 2063 6f6c 6f72 732c 2061 7820 3d20   = colors, ax = 
-00062a60: 6178 2c20 7761 7665 6c65 6e67 7468 203d  ax, wavelength =
-00062a70: 2072 656c 5f77 6176 652c 2077 6964 7468   rel_wave, width
-00062a80: 203d 2077 6964 7468 2c0d 0a09 0909 0909   = width,.......
-00062a90: 0909 0909 0909 7469 746c 6520 3d20 2727  ......title = ''
-00062aa0: 2c20 6c69 6e65 735f 6172 6520 3d20 2764  , lines_are = 'd
-00062ab0: 6174 6127 2c20 7375 6270 6c6f 7420 3d20  ata', subplot = 
-00062ac0: 5472 7565 2c20 636f 6c6f 725f 6f66 6673  True, color_offs
-00062ad0: 6574 203d 2063 6f6c 6f72 5f6f 6666 7365  et = color_offse
-00062ae0: 742c 0d0a 0909 0909 0909 0909 0909 0970  t,.............p
-00062af0: 6c6f 745f 7479 7065 203d 2073 6361 6c65  lot_type = scale
-00062b00: 5f74 7970 652c 206c 696e 6577 6964 7468  _type, linewidth
-00062b10: 203d 206c 696e 6577 6964 7468 290d 0a09   = linewidth)...
-00062b20: 0909 0909 0909 6178 203d 2070 6c6f 7431  ......ax = plot1
-00062b30: 6428 7265 5b27 4143 275d 2f73 6361 6c69  d(re['AC']/scali
-00062b40: 6e67 2c20 636d 6170 203d 2063 6f6c 6f72  ng, cmap = color
-00062b50: 732c 2061 7820 3d20 6178 2c20 7761 7665  s, ax = ax, wave
-00062b60: 6c65 6e67 7468 203d 2072 656c 5f77 6176  length = rel_wav
-00062b70: 652c 2077 6964 7468 203d 2077 6964 7468  e, width = width
-00062b80: 2c0d 0a09 0909 0909 0909 0909 0974 6974  ,............tit
-00062b90: 6c65 203d 2027 272c 206c 696e 6573 5f61  le = '', lines_a
-00062ba0: 7265 203d 2027 6669 7474 6564 272c 2073  re = 'fitted', s
-00062bb0: 7562 706c 6f74 203d 2054 7275 652c 2063  ubplot = True, c
-00062bc0: 6f6c 6f72 5f6f 6666 7365 7420 3d20 636f  olor_offset = co
-00062bd0: 6c6f 725f 6f66 6673 6574 2c20 0d0a 0909  lor_offset, ....
-00062be0: 0909 0909 0909 0909 706c 6f74 5f74 7970  ........plot_typ
-00062bf0: 6520 3d20 7363 616c 655f 7479 7065 2c20  e = scale_type, 
-00062c00: 6c69 6e65 7769 6474 6820 3d20 6c69 6e65  linewidth = line
-00062c10: 7769 6474 6829 0d0a 0909 0909 0909 0909  width)..........
-00062c20: 0909 0909 0909 0909 0909 0909 0920 0d0a  ............. ..
-00062c30: 0909 0909 0909 6578 6365 7074 3a0d 0a09  ......except:...
-00062c40: 0909 0909 0909 7072 696e 7428 2773 6361  ......print('sca
-00062c50: 6c69 6e67 2046 6169 6c65 6421 2729 0d0a  ling Failed!')..
-00062c60: 0909 0909 0909 0969 6620 6461 7461 5f61  .......if data_a
-00062c70: 6e64 5f66 6974 3a0d 0a09 0909 0909 0909  nd_fit:.........
-00062c80: 0961 7820 3d20 706c 6f74 3164 2872 655b  .ax = plot1d(re[
-00062c90: 2741 275d 2c20 636d 6170 203d 2063 6f6c  'A'], cmap = col
-00062ca0: 6f72 732c 2061 7820 3d20 6178 2c20 7761  ors, ax = ax, wa
-00062cb0: 7665 6c65 6e67 7468 203d 2072 656c 5f77  velength = rel_w
-00062cc0: 6176 652c 2077 6964 7468 203d 2077 6964  ave, width = wid
-00062cd0: 7468 2c20 0d0a 0909 0909 0909 0909 0909  th, ............
-00062ce0: 0909 7469 746c 6520 3d20 2727 2c20 6c69  ..title = '', li
-00062cf0: 6e65 735f 6172 6520 3d20 2764 6174 6127  nes_are = 'data'
-00062d00: 2c20 7375 6270 6c6f 7420 3d20 5472 7565  , subplot = True
-00062d10: 2c20 636f 6c6f 725f 6f66 6673 6574 203d  , color_offset =
-00062d20: 2063 6f6c 6f72 5f6f 6666 7365 742c 200d   color_offset, .
-00062d30: 0a09 0909 0909 0909 0909 0909 0970 6c6f  .............plo
-00062d40: 745f 7479 7065 203d 2073 6361 6c65 5f74  t_type = scale_t
-00062d50: 7970 652c 206c 696e 6577 6964 7468 203d  ype, linewidth =
-00062d60: 206c 696e 6577 6964 7468 290d 0a09 0909   linewidth).....
-00062d70: 0909 0909 6178 203d 2070 6c6f 7431 6428  ....ax = plot1d(
-00062d80: 7265 5b27 4143 275d 2c20 636d 6170 203d  re['AC'], cmap =
-00062d90: 2063 6f6c 6f72 732c 2061 7820 3d20 6178   colors, ax = ax
-00062da0: 2c20 7761 7665 6c65 6e67 7468 203d 2072  , wavelength = r
-00062db0: 656c 5f77 6176 652c 2077 6964 7468 203d  el_wave, width =
-00062dc0: 2077 6964 7468 2c20 0d0a 0909 0909 0909   width, ........
-00062dd0: 0909 0909 0974 6974 6c65 203d 2027 272c  .....title = '',
-00062de0: 206c 696e 6573 5f61 7265 203d 2027 6669   lines_are = 'fi
-00062df0: 7474 6564 272c 2073 7562 706c 6f74 203d  tted', subplot =
-00062e00: 2054 7275 652c 2063 6f6c 6f72 5f6f 6666   True, color_off
-00062e10: 7365 7420 3d20 636f 6c6f 725f 6f66 6673  set = color_offs
-00062e20: 6574 2c20 0d0a 0909 0909 0909 0909 0909  et, ............
-00062e30: 0970 6c6f 745f 7479 7065 203d 2073 6361  .plot_type = sca
-00062e40: 6c65 5f74 7970 652c 206c 696e 6577 6964  le_type, linewid
-00062e50: 7468 203d 206c 696e 6577 6964 7468 2920  th = linewidth) 
-00062e60: 0d0a 0909 0909 0965 6c73 653a 0d0a 0909  .......else:....
-00062e70: 0909 0909 6966 2064 6174 615f 616e 645f  ....if data_and_
-00062e80: 6669 743a 0d0a 0909 0909 0909 0961 7820  fit:.........ax 
-00062e90: 3d20 706c 6f74 3164 2872 655b 2741 275d  = plot1d(re['A']
-00062ea0: 2c20 636d 6170 203d 2063 6f6c 6f72 732c  , cmap = colors,
-00062eb0: 2061 7820 3d20 6178 2c20 7761 7665 6c65   ax = ax, wavele
-00062ec0: 6e67 7468 203d 2072 656c 5f77 6176 652c  ngth = rel_wave,
-00062ed0: 2077 6964 7468 203d 2077 6964 7468 2c20   width = width, 
-00062ee0: 0d0a 0909 0909 0909 0909 0909 0974 6974  .............tit
-00062ef0: 6c65 203d 2027 272c 206c 696e 6573 5f61  le = '', lines_a
-00062f00: 7265 203d 2027 6461 7461 272c 2073 7562  re = 'data', sub
-00062f10: 706c 6f74 203d 2054 7275 652c 2063 6f6c  plot = True, col
-00062f20: 6f72 5f6f 6666 7365 7420 3d20 636f 6c6f  or_offset = colo
-00062f30: 725f 6f66 6673 6574 2c20 0d0a 0909 0909  r_offset, ......
-00062f40: 0909 0909 0909 0970 6c6f 745f 7479 7065  .......plot_type
-00062f50: 203d 2073 6361 6c65 5f74 7970 652c 206c   = scale_type, l
-00062f60: 696e 6577 6964 7468 203d 206c 696e 6577  inewidth = linew
-00062f70: 6964 7468 290d 0a09 0909 0909 0961 7820  idth)........ax 
-00062f80: 3d20 706c 6f74 3164 2872 655b 2741 4327  = plot1d(re['AC'
-00062f90: 5d2c 2063 6d61 7020 3d20 636f 6c6f 7273  ], cmap = colors
-00062fa0: 2c20 6178 203d 2061 782c 2077 6176 656c  , ax = ax, wavel
-00062fb0: 656e 6774 6820 3d20 7265 6c5f 7761 7665  ength = rel_wave
-00062fc0: 2c20 7769 6474 6820 3d20 7769 6474 682c  , width = width,
-00062fd0: 200d 0a09 0909 0909 0909 0909 0974 6974   ............tit
-00062fe0: 6c65 203d 2027 272c 206c 696e 6573 5f61  le = '', lines_a
-00062ff0: 7265 203d 2027 6669 7474 6564 272c 2073  re = 'fitted', s
-00063000: 7562 706c 6f74 203d 2054 7275 652c 2063  ubplot = True, c
-00063010: 6f6c 6f72 5f6f 6666 7365 7420 3d20 636f  olor_offset = co
-00063020: 6c6f 725f 6f66 6673 6574 2c20 0d0a 0909  lor_offset, ....
-00063030: 0909 0909 0909 0909 706c 6f74 5f74 7970  ........plot_typ
-00063040: 6520 3d20 7363 616c 655f 7479 7065 2c20  e = scale_type, 
-00063050: 6c69 6e65 7769 6474 6820 3d20 6c69 6e65  linewidth = line
-00063060: 7769 6474 6829 0d0a 0909 0909 0966 6f72  width).......for
-00063070: 2065 6e74 2069 6e20 7265 6c5f 7761 7665   ent in rel_wave
-00063080: 3a0d 0a09 0909 0909 0969 6620 6461 7461  :........if data
-00063090: 5f61 6e64 5f66 6974 3a0d 0a09 0909 0909  _and_fit:.......
-000630a0: 0909 6c61 622e 6170 7065 6e64 2827 2567  ..lab.append('%g
-000630b0: 206e 6d27 2565 6e74 202b 2027 5f27 202b   nm'%ent + '_' +
-000630c0: 2073 7472 286f 2e66 696c 656e 616d 6529   str(o.filename)
-000630d0: 290d 0a09 0909 0909 096c 6162 2e61 7070  )........lab.app
-000630e0: 656e 6428 2725 6720 6e6d 2725 656e 7420  end('%g nm'%ent 
-000630f0: 2b20 275f 2720 2b20 7374 7228 6f2e 6669  + '_' + str(o.fi
-00063100: 6c65 6e61 6d65 2929 0d0a 0909 0909 0968  lename)).......h
-00063110: 616e 646c 6573 2c20 6c61 6265 6c73 3d61  andles, labels=a
-00063120: 782e 6765 745f 6c65 6765 6e64 5f68 616e  x.get_legend_han
-00063130: 646c 6573 5f6c 6162 656c 7328 290d 0a09  dles_labels()...
-00063140: 0909 0909 6966 2064 6174 615f 616e 645f  ....if data_and_
-00063150: 6669 743a 0d0a 0909 0909 0909 666f 7220  fit:........for 
-00063160: 6120 696e 2068 616e 646c 6573 5b2d 322a  a in handles[-2*
-00063170: 6c65 6e28 7265 6c5f 7761 7665 293a 5d3a  len(rel_wave):]:
-00063180: 0d0a 0909 0909 0909 0968 616e 642e 6170  .........hand.ap
-00063190: 7065 6e64 2861 290d 0a09 0909 0909 656c  pend(a).......el
-000631a0: 7365 3a0d 0a09 0909 0909 0966 6f72 2061  se:........for a
-000631b0: 2069 6e20 6861 6e64 6c65 735b 2d6c 656e   in handles[-len
-000631c0: 2872 656c 5f77 6176 6529 3a5d 3a0d 0a09  (rel_wave):]:...
-000631d0: 0909 0909 0909 6861 6e64 2e61 7070 656e  ......hand.appen
-000631e0: 6428 6129 0d0a 0909 0969 6620 6e6f 726d  d(a).....if norm
-000631f0: 5f77 696e 646f 7720 6973 206e 6f74 204e  _window is not N
-00063200: 6f6e 653a 0d0a 0909 0909 200d 0a09 0909  one:...... .....
-00063210: 0961 782e 7365 745f 7469 746c 6528 2763  .ax.set_title('c
-00063220: 6f6d 7061 7265 206d 6561 7375 7265 6420  ompare measured 
-00063230: 616e 6420 6669 7474 6564 2064 6174 6120  and fitted data 
-00063240: 6174 2067 6976 656e 2077 6176 656c 656e  at given wavelen
-00063250: 6774 6820 5c6e 2073 6361 6c65 6420 746f  gth \n scaled to
-00063260: 2074 3d25 6720 7073 203a 2025 6720 7073   t=%g ps : %g ps
-00063270: 202c 2077 6c3d 2025 6720 6e6d 3a20 2567   , wl= %g nm: %g
-00063280: 206e 6d27 2528 6e6f 726d 5f77 696e 646f   nm'%(norm_windo
-00063290: 775b 305d 2c6e 6f72 6d5f 7769 6e64 6f77  w[0],norm_window
-000632a0: 5b31 5d2c 6e6f 726d 5f77 696e 646f 775b  [1],norm_window[
-000632b0: 325d 2c6e 6f72 6d5f 7769 6e64 6f77 5b33  2],norm_window[3
-000632c0: 5d29 290d 0a09 0909 656c 7365 3a0d 0a09  ])).....else:...
-000632d0: 0909 0961 782e 7365 745f 7469 746c 6528  ...ax.set_title(
-000632e0: 2763 6f6d 7061 7265 206d 6561 7375 7265  'compare measure
-000632f0: 6420 616e 6420 6669 7474 6564 2064 6174  d and fitted dat
-00063300: 6120 6174 2067 6976 656e 2077 6176 656c  a at given wavel
-00063310: 656e 6774 6827 290d 0a09 0909 6178 2e73  ength').....ax.s
-00063320: 6574 5f78 6c69 6d28 7265 5b27 4127 5d2e  et_xlim(re['A'].
-00063330: 696e 6465 782e 7661 6c75 6573 5b30 5d2c  index.values[0],
-00063340: 7265 5b27 4127 5d2e 696e 6465 782e 7661  re['A'].index.va
-00063350: 6c75 6573 5b2d 315d 290d 0a09 0909 6178  lues[-1]).....ax
-00063360: 2e6c 6567 656e 6428 6861 6e64 2c6c 6162  .legend(hand,lab
-00063370: 290d 0a09 0965 6c73 653a 0d0a 0909 0966  )....else:.....f
-00063380: 6967 2c20 6178 203d 2070 6c74 2e73 7562  ig, ax = plt.sub
-00063390: 706c 6f74 7328 6669 6773 697a 6520 3d20  plots(figsize = 
-000633a0: 2831 302c 2036 292c 2064 7069 203d 2031  (10, 6), dpi = 1
-000633b0: 3030 290d 0a09 0909 636f 6c6f 7273 203d  00).....colors =
-000633c0: 2063 6f6c 6d28 636d 6170 203d 2063 6d61   colm(cmap = cma
-000633d0: 702c 206b 203d 2072 616e 6765 286c 656e  p, k = range(len
-000633e0: 2872 656c 5f77 6176 6529 2a28 322b 6c65  (rel_wave)*(2+le
-000633f0: 6e28 6f74 6865 7229 2929 290d 0a09 0909  n(other)))).....
-00063400: 6966 206e 6f72 6d5f 7769 6e64 6f77 2069  if norm_window i
-00063410: 7320 6e6f 7420 4e6f 6e65 3a0d 0a09 0909  s not None:.....
-00063420: 0972 6566 5f73 6361 6c65 203d 2073 656c  .ref_scale = sel
-00063430: 662e 6473 2e6c 6f63 5b6e 6f72 6d5f 7769  f.ds.loc[norm_wi
-00063440: 6e64 6f77 5b30 5d3a 6e6f 726d 5f77 696e  ndow[0]:norm_win
-00063450: 646f 775b 315d 2c20 6e6f 726d 5f77 696e  dow[1], norm_win
-00063460: 646f 775b 325d 3a6e 6f72 6d5f 7769 6e64  dow[2]:norm_wind
-00063470: 6f77 5b33 5d5d 2e6d 6561 6e28 292e 6d65  ow[3]].mean().me
-00063480: 616e 2829 0d0a 0909 0961 7820 3d20 706c  an().....ax = pl
-00063490: 6f74 3164 2873 656c 662e 6473 2c20 636d  ot1d(self.ds, cm
-000634a0: 6170 203d 2063 6f6c 6f72 732c 2061 7820  ap = colors, ax 
-000634b0: 3d20 6178 2c20 7761 7665 6c65 6e67 7468  = ax, wavelength
-000634c0: 203d 2072 656c 5f77 6176 652c 2077 6964   = rel_wave, wid
-000634d0: 7468 203d 2077 6964 7468 2c20 7469 746c  th = width, titl
-000634e0: 6520 3d20 7365 6c66 2e66 696c 656e 616d  e = self.filenam
-000634f0: 652c 0d0a 0909 0909 0909 6261 7365 756e  e,........baseun
-00063500: 6974 203d 2073 656c 662e 6261 7365 756e  it = self.baseun
-00063510: 6974 2c20 6c69 6e65 735f 6172 6520 3d20  it, lines_are = 
-00063520: 2764 6174 6127 2c20 7363 6174 7465 7263  'data', scatterc
-00063530: 7574 203d 2073 656c 662e 7363 6174 7465  ut = self.scatte
-00063540: 7263 7574 2c20 0d0a 0909 0909 0909 626f  rcut, ........bo
-00063550: 7264 6572 6375 7420 3d20 7365 6c66 2e62  rdercut = self.b
-00063560: 6f72 6465 7263 7574 2c20 7375 6270 6c6f  ordercut, subplo
-00063570: 7420 3d20 4661 6c73 652c 2063 6f6c 6f72  t = False, color
-00063580: 5f6f 6666 7365 7420 3d20 302c 2074 696d  _offset = 0, tim
-00063590: 656c 696d 6974 7320 3d20 7365 6c66 2e74  elimits = self.t
-000635a0: 696d 656c 696d 6974 732c 200d 0a09 0909  imelimits, .....
-000635b0: 0909 0969 6e74 656e 7369 7479 5f72 616e  ...intensity_ran
-000635c0: 6765 203d 2073 656c 662e 696e 7465 6e73  ge = self.intens
-000635d0: 6974 795f 7261 6e67 652c 2070 6c6f 745f  ity_range, plot_
-000635e0: 7479 7065 203d 2073 6361 6c65 5f74 7970  type = scale_typ
-000635f0: 652c 206c 696e 6577 6964 7468 203d 206c  e, linewidth = l
-00063600: 696e 6577 6964 7468 290d 0a09 0909 6178  inewidth).....ax
-00063610: 203d 2070 6c6f 7431 6428 7365 6c66 2e64   = plot1d(self.d
-00063620: 732c 2063 6d61 7020 3d20 636f 6c6f 7273  s, cmap = colors
-00063630: 2c20 6178 203d 2061 782c 2077 6176 656c  , ax = ax, wavel
-00063640: 656e 6774 6820 3d20 7265 6c5f 7761 7665  ength = rel_wave
-00063650: 2c20 7769 6474 6820 3d20 7769 6474 682c  , width = width,
-00063660: 2074 6974 6c65 203d 2073 656c 662e 6669   title = self.fi
-00063670: 6c65 6e61 6d65 2c20 0d0a 0909 0909 0909  lename, ........
-00063680: 6261 7365 756e 6974 203d 2073 656c 662e  baseunit = self.
-00063690: 6261 7365 756e 6974 2c20 6c69 6e65 735f  baseunit, lines_
-000636a0: 6172 6520 3d20 2773 6d6f 6f74 6865 6427  are = 'smoothed'
-000636b0: 2c20 7363 6174 7465 7263 7574 203d 2073  , scattercut = s
-000636c0: 656c 662e 7363 6174 7465 7263 7574 2c20  elf.scattercut, 
-000636d0: 0d0a 0909 0909 0909 626f 7264 6572 6375  ........bordercu
-000636e0: 7420 3d20 7365 6c66 2e62 6f72 6465 7263  t = self.borderc
-000636f0: 7574 2c20 7375 6270 6c6f 7420 3d20 4661  ut, subplot = Fa
-00063700: 6c73 652c 2063 6f6c 6f72 5f6f 6666 7365  lse, color_offse
-00063710: 7420 3d20 302c 2074 696d 656c 696d 6974  t = 0, timelimit
-00063720: 7320 3d20 7365 6c66 2e74 696d 656c 696d  s = self.timelim
-00063730: 6974 732c 200d 0a09 0909 0909 0969 6e74  its, ........int
-00063740: 656e 7369 7479 5f72 616e 6765 203d 2073  ensity_range = s
-00063750: 656c 662e 696e 7465 6e73 6974 795f 7261  elf.intensity_ra
-00063760: 6e67 652c 2070 6c6f 745f 7479 7065 203d  nge, plot_type =
-00063770: 2073 6361 6c65 5f74 7970 652c 206c 696e   scale_type, lin
-00063780: 6577 6964 7468 203d 206c 696e 6577 6964  ewidth = linewid
-00063790: 7468 290d 0a09 0909 6966 2031 3a0d 0a09  th).....if 1:...
-000637a0: 0909 0968 616e 646c 6573 2c20 6c61 6265  ...handles, labe
-000637b0: 6c73 3d61 782e 6765 745f 6c65 6765 6e64  ls=ax.get_legend
-000637c0: 5f68 616e 646c 6573 5f6c 6162 656c 7328  _handles_labels(
-000637d0: 290d 0a09 0909 096c 6162 3d5b 2725 6720  )......lab=['%g 
-000637e0: 6e6d 2725 6120 2b20 275f 2720 2b20 7374  nm'%a + '_' + st
-000637f0: 7228 7365 6c66 2e66 696c 656e 616d 6529  r(self.filename)
-00063800: 2066 6f72 2061 2069 6e20 7265 6c5f 7761   for a in rel_wa
-00063810: 7665 5d0d 0a09 0909 0968 616e 643d 6861  ve]......hand=ha
-00063820: 6e64 6c65 735b 6c65 6e28 7265 6c5f 7761  ndles[len(rel_wa
-00063830: 7665 293a 5d0d 0a09 0909 0969 6620 6f74  ve):]......if ot
-00063840: 6865 7220 6973 206e 6f74 204e 6f6e 653a  her is not None:
-00063850: 0d0a 0909 0909 0966 6f72 2069 2c6f 2069  .......for i,o i
-00063860: 6e20 656e 756d 6572 6174 6528 6f74 6865  n enumerate(othe
-00063870: 7229 3a0d 0a09 0909 0909 0969 2b3d 310d  r):........i+=1.
-00063880: 0a09 0909 0909 0963 6f6c 6f72 5f6f 6666  .......color_off
-00063890: 7365 743d 2869 2b31 292a 6c65 6e28 7265  set=(i+1)*len(re
-000638a0: 6c5f 7761 7665 290d 0a09 0909 0909 0969  l_wave)........i
-000638b0: 6620 6e6f 726d 5f77 696e 646f 7720 6973  f norm_window is
-000638c0: 206e 6f74 204e 6f6e 653a 0d0a 0909 0909   not None:......
-000638d0: 0909 0972 656c 5f73 6361 6c65 3d6f 2e64  ...rel_scale=o.d
-000638e0: 732e 6c6f 635b 6e6f 726d 5f77 696e 646f  s.loc[norm_windo
-000638f0: 775b 305d 3a6e 6f72 6d5f 7769 6e64 6f77  w[0]:norm_window
-00063900: 5b31 5d2c 6e6f 726d 5f77 696e 646f 775b  [1],norm_window[
-00063910: 325d 3a6e 6f72 6d5f 7769 6e64 6f77 5b33  2]:norm_window[3
-00063920: 5d5d 2e6d 6561 6e28 292e 6d65 616e 2829  ]].mean().mean()
-00063930: 0d0a 0909 0909 0909 0974 7279 3a0d 0a09  .........try:...
-00063940: 0909 0909 0909 0973 6361 6c69 6e67 3d28  .......scaling=(
-00063950: 7265 6c5f 7363 616c 652f 7265 665f 7363  rel_scale/ref_sc
-00063960: 616c 6529 0d0a 0909 0909 0909 0909 6178  ale)..........ax
-00063970: 203d 2070 6c6f 7431 6428 6f2e 6473 2f73   = plot1d(o.ds/s
-00063980: 6361 6c69 6e67 2c20 636d 6170 203d 2063  caling, cmap = c
-00063990: 6f6c 6f72 732c 2061 7820 3d20 6178 2c20  olors, ax = ax, 
-000639a0: 7761 7665 6c65 6e67 7468 203d 2072 656c  wavelength = rel
-000639b0: 5f77 6176 652c 2077 6964 7468 203d 2077  _wave, width = w
-000639c0: 6964 7468 2c0d 0a09 0909 0909 0909 0909  idth,...........
-000639d0: 0909 7469 746c 6520 3d20 6f2e 6669 6c65  ..title = o.file
-000639e0: 6e61 6d65 2c20 6261 7365 756e 6974 203d  name, baseunit =
-000639f0: 2073 656c 662e 6261 7365 756e 6974 2c20   self.baseunit, 
-00063a00: 7469 6d65 6c69 6d69 7473 203d 2073 656c  timelimits = sel
-00063a10: 662e 7469 6d65 6c69 6d69 7473 2c0d 0a09  f.timelimits,...
-00063a20: 0909 0909 0909 0909 0909 6c69 6e65 735f  ..........lines_
-00063a30: 6172 6520 3d20 2764 6174 6127 2c20 7363  are = 'data', sc
-00063a40: 6174 7465 7263 7574 203d 2073 656c 662e  attercut = self.
-00063a50: 7363 6174 7465 7263 7574 2c20 626f 7264  scattercut, bord
-00063a60: 6572 6375 7420 3d20 7365 6c66 2e62 6f72  ercut = self.bor
-00063a70: 6465 7263 7574 2c0d 0a09 0909 0909 0909  dercut,.........
-00063a80: 0909 0909 7375 6270 6c6f 7420 3d20 5472  ....subplot = Tr
-00063a90: 7565 2c20 636f 6c6f 725f 6f66 6673 6574  ue, color_offset
-00063aa0: 203d 2063 6f6c 6f72 5f6f 6666 7365 742c   = color_offset,
-00063ab0: 200d 0a09 0909 0909 0909 0909 0909 696e   .............in
-00063ac0: 7465 6e73 6974 795f 7261 6e67 6520 3d20  tensity_range = 
-00063ad0: 7365 6c66 2e69 6e74 656e 7369 7479 5f72  self.intensity_r
-00063ae0: 616e 6765 2c20 706c 6f74 5f74 7970 6520  ange, plot_type 
-00063af0: 3d20 7363 616c 655f 7479 7065 2c20 6c69  = scale_type, li
-00063b00: 6e65 7769 6474 6820 3d20 6c69 6e65 7769  newidth = linewi
-00063b10: 6474 6829 0d0a 0909 0909 0909 0909 6178  dth)..........ax
-00063b20: 203d 2070 6c6f 7431 6428 6f2e 6473 2f73   = plot1d(o.ds/s
-00063b30: 6361 6c69 6e67 2c20 636d 6170 203d 2063  caling, cmap = c
-00063b40: 6f6c 6f72 732c 2061 7820 3d20 6178 2c20  olors, ax = ax, 
-00063b50: 7761 7665 6c65 6e67 7468 203d 2072 656c  wavelength = rel
-00063b60: 5f77 6176 652c 2077 6964 7468 203d 2077  _wave, width = w
-00063b70: 6964 7468 2c0d 0a09 0909 0909 0909 0909  idth,...........
-00063b80: 0909 7469 746c 6520 3d20 6f2e 6669 6c65  ..title = o.file
-00063b90: 6e61 6d65 2c20 6261 7365 756e 6974 203d  name, baseunit =
-00063ba0: 2073 656c 662e 6261 7365 756e 6974 2c20   self.baseunit, 
-00063bb0: 7469 6d65 6c69 6d69 7473 203d 2073 656c  timelimits = sel
-00063bc0: 662e 7469 6d65 6c69 6d69 7473 2c0d 0a09  f.timelimits,...
-00063bd0: 0909 0909 0909 0909 0909 6c69 6e65 735f  ..........lines_
-00063be0: 6172 6520 3d20 2773 6d6f 6f74 6865 6427  are = 'smoothed'
-00063bf0: 2c20 7363 6174 7465 7263 7574 203d 2073  , scattercut = s
-00063c00: 656c 662e 7363 6174 7465 7263 7574 2c20  elf.scattercut, 
-00063c10: 626f 7264 6572 6375 7420 3d20 7365 6c66  bordercut = self
-00063c20: 2e62 6f72 6465 7263 7574 2c0d 0a09 0909  .bordercut,.....
-00063c30: 0909 0909 0909 0909 7375 6270 6c6f 7420  ........subplot 
-00063c40: 3d20 5472 7565 2c20 636f 6c6f 725f 6f66  = True, color_of
-00063c50: 6673 6574 203d 2063 6f6c 6f72 5f6f 6666  fset = color_off
-00063c60: 7365 742c 200d 0a09 0909 0909 0909 0909  set, ...........
-00063c70: 0909 696e 7465 6e73 6974 795f 7261 6e67  ..intensity_rang
-00063c80: 6520 3d20 7365 6c66 2e69 6e74 656e 7369  e = self.intensi
-00063c90: 7479 5f72 616e 6765 2c20 706c 6f74 5f74  ty_range, plot_t
-00063ca0: 7970 6520 3d20 7363 616c 655f 7479 7065  ype = scale_type
-00063cb0: 2c20 6c69 6e65 7769 6474 6820 3d20 6c69  , linewidth = li
-00063cc0: 6e65 7769 6474 6829 0d0a 0909 0909 0909  newidth)........
-00063cd0: 0965 7863 6570 743a 0d0a 0909 0909 0909  .except:........
-00063ce0: 0909 7072 696e 7428 2773 6361 6c69 6e67  ..print('scaling
-00063cf0: 2066 6169 6c65 6427 290d 0a09 0909 0909   failed').......
-00063d00: 0909 0961 7820 3d20 706c 6f74 3164 286f  ...ax = plot1d(o
-00063d10: 2e64 732c 2063 6d61 7020 3d20 636f 6c6f  .ds, cmap = colo
-00063d20: 7273 2c20 6178 203d 2061 782c 2077 6176  rs, ax = ax, wav
-00063d30: 656c 656e 6774 6820 3d20 7265 6c5f 7761  elength = rel_wa
-00063d40: 7665 2c20 7769 6474 6820 3d20 7769 6474  ve, width = widt
-00063d50: 682c 0d0a 0909 0909 0909 0909 0909 0974  h,.............t
-00063d60: 6974 6c65 203d 206f 2e66 696c 656e 616d  itle = o.filenam
-00063d70: 652c 2062 6173 6575 6e69 7420 3d20 7365  e, baseunit = se
-00063d80: 6c66 2e62 6173 6575 6e69 742c 2074 696d  lf.baseunit, tim
-00063d90: 656c 696d 6974 7320 3d20 7365 6c66 2e74  elimits = self.t
-00063da0: 696d 656c 696d 6974 732c 0d0a 0909 0909  imelimits,......
-00063db0: 0909 0909 0909 096c 696e 6573 5f61 7265  .......lines_are
-00063dc0: 203d 2027 6461 7461 272c 2073 6361 7474   = 'data', scatt
-00063dd0: 6572 6375 7420 3d20 7365 6c66 2e73 6361  ercut = self.sca
-00063de0: 7474 6572 6375 742c 2062 6f72 6465 7263  ttercut, borderc
-00063df0: 7574 203d 2073 656c 662e 626f 7264 6572  ut = self.border
-00063e00: 6375 742c 0d0a 0909 0909 0909 0909 0909  cut,............
-00063e10: 0973 7562 706c 6f74 203d 2054 7275 652c  .subplot = True,
-00063e20: 2063 6f6c 6f72 5f6f 6666 7365 7420 3d20   color_offset = 
-00063e30: 636f 6c6f 725f 6f66 6673 6574 2c20 0d0a  color_offset, ..
-00063e40: 0909 0909 0909 0909 0909 0969 6e74 656e  ...........inten
-00063e50: 7369 7479 5f72 616e 6765 203d 2073 656c  sity_range = sel
-00063e60: 662e 696e 7465 6e73 6974 795f 7261 6e67  f.intensity_rang
-00063e70: 652c 2070 6c6f 745f 7479 7065 203d 2073  e, plot_type = s
-00063e80: 6361 6c65 5f74 7970 652c 206c 696e 6577  cale_type, linew
-00063e90: 6964 7468 203d 206c 696e 6577 6964 7468  idth = linewidth
-00063ea0: 290d 0a09 0909 0909 0909 0961 7820 3d20  )..........ax = 
-00063eb0: 706c 6f74 3164 286f 2e64 732c 2063 6d61  plot1d(o.ds, cma
-00063ec0: 7020 3d20 636f 6c6f 7273 2c20 6178 203d  p = colors, ax =
-00063ed0: 2061 782c 2077 6176 656c 656e 6774 6820   ax, wavelength 
-00063ee0: 3d20 7265 6c5f 7761 7665 2c20 7769 6474  = rel_wave, widt
-00063ef0: 6820 3d20 7769 6474 682c 0d0a 0909 0909  h = width,......
-00063f00: 0909 0909 0909 0974 6974 6c65 203d 206f  .......title = o
-00063f10: 2e66 696c 656e 616d 652c 2062 6173 6575  .filename, baseu
-00063f20: 6e69 7420 3d20 7365 6c66 2e62 6173 6575  nit = self.baseu
-00063f30: 6e69 742c 2074 696d 656c 696d 6974 7320  nit, timelimits 
-00063f40: 3d20 7365 6c66 2e74 696d 656c 696d 6974  = self.timelimit
-00063f50: 732c 0d0a 0909 0909 0909 0909 0909 096c  s,.............l
-00063f60: 696e 6573 5f61 7265 203d 2027 736d 6f6f  ines_are = 'smoo
-00063f70: 7468 6564 272c 2073 6361 7474 6572 6375  thed', scattercu
-00063f80: 7420 3d20 7365 6c66 2e73 6361 7474 6572  t = self.scatter
-00063f90: 6375 742c 2062 6f72 6465 7263 7574 203d  cut, bordercut =
-00063fa0: 2073 656c 662e 626f 7264 6572 6375 742c   self.bordercut,
-00063fb0: 0d0a 0909 0909 0909 0909 0909 0973 7562  .............sub
-00063fc0: 706c 6f74 203d 2054 7275 652c 2063 6f6c  plot = True, col
-00063fd0: 6f72 5f6f 6666 7365 7420 3d20 636f 6c6f  or_offset = colo
-00063fe0: 725f 6f66 6673 6574 2c20 0d0a 0909 0909  r_offset, ......
-00063ff0: 0909 0909 0909 0969 6e74 656e 7369 7479  .......intensity
-00064000: 5f72 616e 6765 203d 2073 656c 662e 696e  _range = self.in
-00064010: 7465 6e73 6974 795f 7261 6e67 652c 2070  tensity_range, p
-00064020: 6c6f 745f 7479 7065 203d 2073 6361 6c65  lot_type = scale
-00064030: 5f74 7970 652c 206c 696e 6577 6964 7468  _type, linewidth
-00064040: 203d 206c 696e 6577 6964 7468 290d 0a09   = linewidth)...
-00064050: 0909 0909 0965 6c73 653a 0d0a 0909 0909  .....else:......
-00064060: 0909 0961 7820 3d20 706c 6f74 3164 286f  ...ax = plot1d(o
-00064070: 2e64 732c 2063 6d61 7020 3d20 636f 6c6f  .ds, cmap = colo
-00064080: 7273 2c20 6178 203d 2061 782c 2077 6176  rs, ax = ax, wav
-00064090: 656c 656e 6774 6820 3d20 7265 6c5f 7761  elength = rel_wa
-000640a0: 7665 2c20 7769 6474 6820 3d20 7769 6474  ve, width = widt
-000640b0: 682c 2074 6974 6c65 203d 206f 2e66 696c  h, title = o.fil
-000640c0: 656e 616d 652c 0d0a 0909 0909 0909 0909  ename,..........
-000640d0: 0909 6261 7365 756e 6974 203d 2073 656c  ..baseunit = sel
-000640e0: 662e 6261 7365 756e 6974 2c20 7469 6d65  f.baseunit, time
-000640f0: 6c69 6d69 7473 203d 2073 656c 662e 7469  limits = self.ti
-00064100: 6d65 6c69 6d69 7473 2c20 6c69 6e65 735f  melimits, lines_
-00064110: 6172 6520 3d20 2764 6174 6127 2c0d 0a09  are = 'data',...
-00064120: 0909 0909 0909 0909 0973 6361 7474 6572  .........scatter
-00064130: 6375 7420 3d20 7365 6c66 2e73 6361 7474  cut = self.scatt
-00064140: 6572 6375 742c 2062 6f72 6465 7263 7574  ercut, bordercut
-00064150: 203d 2073 656c 662e 626f 7264 6572 6375   = self.bordercu
-00064160: 742c 2073 7562 706c 6f74 203d 2054 7275  t, subplot = Tru
-00064170: 652c 0d0a 0909 0909 0909 0909 0909 636f  e,............co
-00064180: 6c6f 725f 6f66 6673 6574 203d 2063 6f6c  lor_offset = col
-00064190: 6f72 5f6f 6666 7365 742c 2069 6e74 656e  or_offset, inten
-000641a0: 7369 7479 5f72 616e 6765 203d 2073 656c  sity_range = sel
-000641b0: 662e 696e 7465 6e73 6974 795f 7261 6e67  f.intensity_rang
-000641c0: 652c 200d 0a09 0909 0909 0909 0909 0970  e, ............p
-000641d0: 6c6f 745f 7479 7065 203d 2073 6361 6c65  lot_type = scale
-000641e0: 5f74 7970 652c 206c 696e 6577 6964 7468  _type, linewidth
-000641f0: 203d 206c 696e 6577 6964 7468 290d 0a09   = linewidth)...
-00064200: 0909 0909 0909 6178 203d 2070 6c6f 7431  ......ax = plot1
-00064210: 6428 6f2e 6473 2c20 636d 6170 203d 2063  d(o.ds, cmap = c
-00064220: 6f6c 6f72 732c 2061 7820 3d20 6178 2c20  olors, ax = ax, 
-00064230: 7761 7665 6c65 6e67 7468 203d 2072 656c  wavelength = rel
-00064240: 5f77 6176 652c 2077 6964 7468 203d 2077  _wave, width = w
-00064250: 6964 7468 2c20 7469 746c 6520 3d20 6f2e  idth, title = o.
-00064260: 6669 6c65 6e61 6d65 2c0d 0a09 0909 0909  filename,.......
-00064270: 0909 0909 0962 6173 6575 6e69 7420 3d20  .....baseunit = 
-00064280: 7365 6c66 2e62 6173 6575 6e69 742c 2074  self.baseunit, t
-00064290: 696d 656c 696d 6974 7320 3d20 7365 6c66  imelimits = self
-000642a0: 2e74 696d 656c 696d 6974 732c 206c 696e  .timelimits, lin
-000642b0: 6573 5f61 7265 203d 2027 736d 6f6f 7468  es_are = 'smooth
-000642c0: 6564 272c 0d0a 0909 0909 0909 0909 0909  ed',............
-000642d0: 7363 6174 7465 7263 7574 203d 2073 656c  scattercut = sel
-000642e0: 662e 7363 6174 7465 7263 7574 2c20 626f  f.scattercut, bo
-000642f0: 7264 6572 6375 7420 3d20 7365 6c66 2e62  rdercut = self.b
-00064300: 6f72 6465 7263 7574 2c20 7375 6270 6c6f  ordercut, subplo
-00064310: 7420 3d20 5472 7565 2c0d 0a09 0909 0909  t = True,.......
-00064320: 0909 0909 0963 6f6c 6f72 5f6f 6666 7365  .....color_offse
-00064330: 7420 3d20 636f 6c6f 725f 6f66 6673 6574  t = color_offset
-00064340: 2c20 696e 7465 6e73 6974 795f 7261 6e67  , intensity_rang
-00064350: 6520 3d20 7365 6c66 2e69 6e74 656e 7369  e = self.intensi
-00064360: 7479 5f72 616e 6765 2c20 0d0a 0909 0909  ty_range, ......
-00064370: 0909 0909 0909 706c 6f74 5f74 7970 6520  ......plot_type 
-00064380: 3d20 7363 616c 655f 7479 7065 2c20 6c69  = scale_type, li
-00064390: 6e65 7769 6474 6820 3d20 6c69 6e65 7769  newidth = linewi
-000643a0: 6474 6829 0d0a 0909 0909 0909 666f 7220  dth)........for 
-000643b0: 656e 7420 696e 205b 2725 6720 6e6d 2725  ent in ['%g nm'%
-000643c0: 6120 2b20 275f 2720 2b20 7374 7228 6f2e  a + '_' + str(o.
-000643d0: 6669 6c65 6e61 6d65 2920 666f 7220 6120  filename) for a 
-000643e0: 696e 2072 656c 5f77 6176 655d 3a0d 0a09  in rel_wave]:...
-000643f0: 0909 0909 0909 6c61 622e 6170 7065 6e64  ......lab.append
-00064400: 2865 6e74 290d 0a09 0909 0909 0968 616e  (ent)........han
-00064410: 646c 6573 2c20 6c61 6265 6c73 3d61 782e  dles, labels=ax.
-00064420: 6765 745f 6c65 6765 6e64 5f68 616e 646c  get_legend_handl
-00064430: 6573 5f6c 6162 656c 7328 290d 0a09 0909  es_labels().....
-00064440: 0909 0966 6f72 2068 6120 696e 2068 616e  ...for ha in han
-00064450: 646c 6573 5b2d 6c65 6e28 7265 6c5f 7761  dles[-len(rel_wa
-00064460: 7665 293a 5d3a 0d0a 0909 0909 0909 0968  ve):]:.........h
-00064470: 616e 642e 6170 7065 6e64 2868 6129 0d0a  and.append(ha)..
-00064480: 0909 0909 6178 2e73 6574 5f74 6974 6c65  ....ax.set_title
-00064490: 2827 636f 6d70 6172 6520 6d65 6173 7572  ('compare measur
-000644a0: 6564 2061 6e64 2073 6d6f 6f74 6865 6420  ed and smoothed 
-000644b0: 6461 7461 2061 7420 6769 7665 6e20 7761  data at given wa
-000644c0: 7665 6c65 6e67 7468 2729 0d0a 0909 0909  velength')......
-000644d0: 6966 206e 6f72 6d5f 7769 6e64 6f77 2069  if norm_window i
-000644e0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a09 0909  s not None:.....
-000644f0: 0909 6178 2e73 6574 5f74 6974 6c65 2827  ..ax.set_title('
-00064500: 636f 6d70 6172 6520 6d65 6173 7572 6564  compare measured
-00064510: 2061 6e64 2073 6d6f 6f74 6865 6420 6461   and smoothed da
-00064520: 7461 2061 7420 6769 7665 6e20 7761 7665  ta at given wave
-00064530: 6c65 6e67 7468 205c 6e20 7363 616c 6564  length \n scaled
-00064540: 2074 6f20 743d 2567 2070 7320 3a20 2567   to t=%g ps : %g
-00064550: 2070 7320 2c20 776c 3d20 2567 206e 6d3a   ps , wl= %g nm:
-00064560: 2025 6720 6e6d 2725 286e 6f72 6d5f 7769   %g nm'%(norm_wi
-00064570: 6e64 6f77 5b30 5d2c 6e6f 726d 5f77 696e  ndow[0],norm_win
-00064580: 646f 775b 315d 2c6e 6f72 6d5f 7769 6e64  dow[1],norm_wind
-00064590: 6f77 5b32 5d2c 6e6f 726d 5f77 696e 646f  ow[2],norm_windo
-000645a0: 775b 335d 2929 0d0a 0909 0909 6178 2e6c  w[3]))......ax.l
-000645b0: 6567 656e 6428 6861 6e64 2c6c 6162 290d  egend(hand,lab).
-000645c0: 0a09 0969 6620 7365 6c66 2e73 6176 655f  ...if self.save_
-000645d0: 6669 6775 7265 735f 746f 5f66 6f6c 6465  figures_to_folde
-000645e0: 723a 2020 0d0a 0909 0966 6967 2e73 6176  r:  .....fig.sav
-000645f0: 6566 6967 2863 6865 636b 5f66 6f6c 6465  efig(check_folde
-00064600: 7228 7061 7468 3d73 656c 662e 6669 6775  r(path=self.figu
-00064610: 7265 5f70 6174 682c 6669 6c65 6e61 6d65  re_path,filename
-00064620: 3d27 636f 6d70 6172 655f 6174 5f77 6176  ='compare_at_wav
-00064630: 655f 2573 2e70 6e67 2725 275f 272e 6a6f  e_%s.png'%'_'.jo
-00064640: 696e 285b 2725 6727 2561 2066 6f72 2061  in(['%g'%a for a
-00064650: 2069 6e20 7265 6c5f 7761 7665 5d29 292c   in rel_wave])),
-00064660: 0d0a 0909 0962 626f 785f 696e 6368 6573  .....bbox_inches
-00064670: 3d27 7469 6768 7427 290d 0a09 0909 7265  ='tight').....re
-00064680: 7475 726e 2061 780d 0a0d 0a0d 0a09 6465  turn ax.......de
-00064690: 6620 436f 6d70 6172 655f 4441 4328 7365  f Compare_DAC(se
-000646a0: 6c66 2c20 6f74 6865 7220 3d20 4e6f 6e65  lf, other = None
-000646b0: 2c20 7370 6563 7472 6120 3d20 4e6f 6e65  , spectra = None
-000646c0: 2c20 7365 7061 7261 7465 5f70 6c6f 7473  , separate_plots
-000646d0: 203d 2046 616c 7365 2c20 636d 6170 203d   = False, cmap =
-000646e0: 204e 6f6e 6529 3a0d 0a09 0927 2727 5468   None):....'''Th
-000646f0: 6973 2069 7320 6120 636f 6e76 656e 6965  is is a convenie
-00064700: 6e63 6520 6675 6e63 7469 6f6e 2074 6f20  nce function to 
-00064710: 706c 6f74 206d 756c 7469 706c 6520 6578  plot multiple ex
-00064720: 7472 6163 7465 6420 7370 6563 7472 6120  tracted spectra 
-00064730: 0d0a 0909 2844 4153 206f 7220 7370 6563  ....(DAS or spec
-00064740: 6965 7320 6173 736f 6369 6174 6564 2920  ies associated) 
-00064750: 696e 746f 2074 6865 2073 616d 6520 6669  into the same fi
-00064760: 6775 7265 206f 7220 696e 746f 2061 2073  gure or into a s
-00064770: 6570 6172 6174 6520 6669 6775 7265 0d0a  eparate figure..
-00064780: 0909 6561 6368 2e20 4f74 6865 7220 7368  ..each. Other sh
-00064790: 6f75 6c64 2062 6520 7461 2e70 6c6f 745f  ould be ta.plot_
-000647a0: 6675 6e63 206f 626a 6563 7473 2028 6c6f  func objects (lo
-000647b0: 6164 6564 206f 7220 636f 7069 6564 292e  aded or copied).
-000647c0: 2042 790d 0a09 0973 7461 6e64 6172 6420   By....standard 
-000647d0: 6974 2070 6c6f 7473 2061 6c6c 2069 6e74  it plots all int
-000647e0: 6f20 7468 6520 7361 6d65 2077 696e 646f  o the same windo
-000647f0: 772e 2049 6620 616c 6c20 7072 6f6a 6563  w. If all projec
-00064800: 7420 6861 7665 2074 6865 2073 616d 650d  t have the same.
-00064810: 0a09 096e 756d 6265 7220 6f66 2063 6f6d  ...number of com
-00064820: 706f 6e65 6e74 7320 6f6e 6520 6361 6e20  ponents one can 
-00064830: 6163 7469 7661 7465 2022 7365 7061 7261  activate "separa
-00064840: 7465 5f70 6c6f 7473 2220 616e 6420 6861  te_plots" and ha
-00064850: 7665 2065 6163 680d 0a09 0973 6570 6172  ve each....separ
-00064860: 6174 6564 2028 696e 2074 6865 206f 7264  ated (in the ord
-00064870: 6572 2063 7265 6174 6564 2069 6e20 7468  er created in th
-00064880: 6520 7072 6f6a 6563 7473 292e 0d0a 0d0a  e projects).....
-00064890: 0909 5468 6520 2253 7065 6374 7261 2220  ..The "Spectra" 
-000648a0: 7061 7261 6d65 7465 7220 616c 6c6f 7773  parameter allows
-000648b0: 2061 7320 6265 666f 7265 2074 6865 2069   as before the i
-000648c0: 6e63 6c75 7369 6f6e 206f 6620 616e 2065  nclusion of an e
-000648d0: 7874 6572 6e61 6c0d 0a09 0973 7065 6374  xternal....spect
-000648e0: 7275 6d2e 204f 7468 6572 7320 6973 206f  rum. Others is o
-000648f0: 7074 696f 6e61 6c20 616e 6420 4920 7573  ptional and I us
-00064900: 6520 7468 6973 2066 756e 6374 696f 6e20  e this function 
-00064910: 6f66 7465 6e20 746f 2063 6f6d 7061 7265  often to compare
-00064920: 0d0a 0909 7370 6563 6965 7320 6173 736f  ....species asso
-00064930: 6369 6174 6564 2073 7065 6374 7261 2077  ciated spectra w
-00064940: 6974 6820 6f6e 6520 6f72 206d 756c 7469  ith one or multi
-00064950: 706c 6520 7374 6561 6479 2073 7461 7465  ple steady state
-00064960: 2073 7065 6374 7261 2e0d 0a09 090d 0a09   spectra........
-00064970: 0950 6172 616d 6574 6572 730d 0a09 092d  .Parameters....-
-00064980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a09  -------------...
-00064990: 0909 0d0a 0909 6f74 6865 7220 3a20 5441  ......other : TA
-000649a0: 206f 626a 6563 7420 6f72 206c 6973 7420   object or list 
-000649b0: 6f66 2074 686f 7365 2c20 6f70 7469 6f6e  of those, option
-000649c0: 616c 200d 0a09 0909 7368 6f75 6c64 2062  al .....should b
-000649d0: 6520 7461 2e70 6c6f 745f 6675 6e63 206f  e ta.plot_func o
-000649e0: 626a 6563 7473 2028 6c6f 6164 6564 206f  bjects (loaded o
-000649f0: 7220 636f 7069 6564 2920 616e 6420 6973  r copied) and is
-00064a00: 2077 6861 7420 0d0a 0909 0969 7320 706c   what .....is pl
-00064a10: 6f74 7465 6420 6167 6169 6e73 7420 7468  otted against th
-00064a20: 6520 6461 7461 2075 7365 2061 206c 6973  e data use a lis
-00064a30: 7420 5b74 6131 2c74 6132 2c2e 2e2e 205d  t [ta1,ta2,... ]
-00064a40: 206f 7220 6765 6e65 7261 7465 2074 6869   or generate thi
-00064a50: 730d 0a09 0909 6c69 7374 2075 7369 6e67  s.....list using
-00064a60: 2074 6865 2047 7569 2066 756e 6374 696f   the Gui functio
-00064a70: 6e2e 2053 6565 2073 6563 7469 6f6e 203a  n. See section :
-00064a80: 7265 663a 604f 7065 6e69 6e67 206d 756c  ref:`Opening mul
-00064a90: 7469 706c 6520 6669 6c65 7360 2069 6e20  tiple files` in 
-00064aa0: 0d0a 0909 0974 6865 2064 6f63 756d 656e  .....the documen
-00064ab0: 7461 7469 6f6e 0d0a 0d0a 0909 7370 6563  tation......spec
-00064ac0: 7472 6120 3a20 4e6f 6e65 206f 7220 4461  tra : None or Da
-00064ad0: 7461 4672 616d 652c 206f 7074 696f 6e61  taFrame, optiona
-00064ae0: 6c0d 0a09 0909 4966 2061 6e20 4461 7461  l.....If an Data
-00064af0: 4672 616d 6520 7769 7468 2074 6865 2077  Frame with the w
-00064b00: 6176 656c 656e 6774 6820 6173 2069 6e64  avelength as ind
-00064b10: 6578 2069 7320 7072 6f76 6964 6564 2c20  ex is provided, 
-00064b20: 5468 656e 2074 6865 2073 7065 6374 7261  Then the spectra
-00064b30: 206f 6620 6561 6368 2063 6f6c 756d 6e0d   of each column.
-00064b40: 0a09 0909 6973 2070 6c6f 7474 6564 2069  ....is plotted i
-00064b50: 6e74 6f20 7468 6520 6469 6666 6572 656e  nto the differen
-00064b60: 7469 616c 2073 7065 6374 7261 2031 3a31  tial spectra 1:1
-00064b70: 2061 6e64 2074 6865 2063 6f6c 756d 6e20   and the column 
-00064b80: 6e61 6d65 7320 6172 6520 7573 6564 2069  names are used i
-00064b90: 6e20 7468 6520 6c65 6765 6e64 0d0a 0909  n the legend....
-00064ba0: 0950 7269 6f72 2073 6361 6c69 6e67 2069  .Prior scaling i
-00064bb0: 7320 6869 6768 6c79 2073 7567 6765 7374  s highly suggest
-00064bc0: 6564 2e20 5468 6573 6520 7370 6563 7472  ed. These spectr
-00064bd0: 6120 6172 6520 6e6f 7420 2869 6e20 6765  a are not (in ge
-00064be0: 6e65 7261 6c29 2073 6361 6c65 6420 7769  neral) scaled wi
-00064bf0: 7468 2074 6865 200d 0a09 0909 6e6f 726d  th the .....norm
-00064c00: 2077 696e 646f 772e 2028 7365 6520 6578   window. (see ex
-00064c10: 616d 706c 6573 290d 0a0d 0a09 0973 6570  amples)......sep
-00064c20: 6172 6174 655f 706c 6f74 7320 3a20 626f  arate_plots : bo
-00064c30: 6f6c 2c20 6f70 7469 6f6e 616c 0d0a 0909  ol, optional....
-00064c40: 0954 7275 6520 6f72 2046 616c 7365 2028  .True or False (
-00064c50: 4465 6661 756c 7429 2c20 7365 7061 7261  Default), separa
-00064c60: 7465 2070 6c6f 7473 2069 7320 7468 6520  te plots is the 
-00064c70: 7377 6974 6368 2074 6861 7420 6465 6369  switch that deci
-00064c80: 6465 7320 6966 2061 2061 7869 7320 6f72  des if a axis or
-00064c90: 200d 0a09 0909 6d75 6c74 6970 6c65 2061   .....multiple a
-00064ca0: 7869 7320 6172 6520 7573 6564 2e20 5468  xis are used. Th
-00064cb0: 6973 206f 7074 696f 6e20 7769 6c6c 2072  is option will r
-00064cc0: 6573 756c 7420 696e 2061 2063 7261 7368  esult in a crash
-00064cd0: 2075 6e6c 6573 7320 616c 6c20 6f62 6a65   unless all obje
-00064ce0: 6374 7320 6861 7665 2074 6865 0d0a 0909  cts have the....
-00064cf0: 0973 616d 6520 6e75 6d62 6572 206f 6620  .same number of 
-00064d00: 4441 532f 5341 5320 636f 6d70 6f6e 656e  DAS/SAS componen
-00064d10: 7473 0d0a 0909 0909 0d0a 0909 636d 6170  ts..........cmap
-00064d20: 203a 204e 6f6e 6520 6f72 206d 6174 706c   : None or matpl
-00064d30: 6f74 6c69 6220 636f 6c6f 7220 6d61 702c  otlib color map,
-00064d40: 206f 7074 696f 6e61 6c0d 0a09 0909 6973   optional.....is
-00064d50: 2061 2070 6f77 6572 6675 6c6c 2076 6172   a powerfull var
-00064d60: 6961 626c 6520 7468 6174 2063 686f 6f73  iable that choos
-00064d70: 6573 2074 6865 2063 6f6c 6f75 7220 6d61  es the colour ma
-00064d80: 7020 6170 706c 6965 6420 666f 7220 616c  p applied for al
-00064d90: 6c20 706c 6f74 732e 2049 6620 7365 7420  l plots. If set 
-00064da0: 746f 200d 0a09 0909 4e6f 6e65 2028 4465  to .....None (De
-00064db0: 6661 756c 7429 2074 6865 6e20 7468 6520  fault) then the 
-00064dc0: 7365 6c66 2e63 6d61 7020 6973 2075 7365  self.cmap is use
-00064dd0: 642e 0d0a 0909 0941 7320 7374 616e 6461  d......As standa
-00064de0: 7264 2049 2075 7365 2074 6865 2063 6f6c  rd I use the col
-00064df0: 6f72 206d 6170 2022 6a65 7422 2066 726f  or map "jet" fro
-00064e00: 6d20 6d61 7470 6c6f 746c 6962 2e20 5468  m matplotlib. Th
-00064e10: 6572 6520 6172 6520 6120 7661 7269 6574  ere are a variet
-00064e20: 7920 6f66 2063 6f6c 6f72 6d61 7073 200d  y of colormaps .
-00064e30: 0a09 0909 6176 6169 6c61 626c 6520 7468  ....available th
-00064e40: 6174 2061 7265 2076 6572 7920 7573 6566  at are very usef
-00064e50: 756c 6c2e 2042 6573 6964 6520 226a 6574  ull. Beside "jet
-00064e60: 222c 2022 7669 7269 6469 7322 2069 7320  ", "viridis" is 
-00064e70: 6120 676f 6f64 2063 686f 6963 6520 6173  a good choice as
-00064e80: 2069 7420 6973 2077 656c 6c20 0d0a 0909   it is well ....
-00064e90: 0976 6973 6962 6c65 2075 6e64 6572 2072  .visible under r
-00064ea0: 6564 2d67 7265 656e 2062 6c69 6e64 6e65  ed-green blindne
-00064eb0: 7373 2e20 4f74 6865 7220 7573 6566 756c  ss. Other useful
-00064ec0: 206d 6170 7320 6172 6520 2270 7269 736d   maps are "prism
-00064ed0: 2220 666f 7220 6869 6768 2066 6c75 6374  " for high fluct
-00064ee0: 7561 7469 6f6e 7320 0d0a 0909 096f 7220  uations .....or 
-00064ef0: 6469 7665 7267 696e 6720 636f 6c6f 7220  diverging color 
-00064f00: 6d61 7073 206c 696b 6520 2273 6569 736d  maps like "seism
-00064f10: 6963 222e 200d 0a09 0909 5365 6520 6874  ic". .....See ht
-00064f20: 7470 733a 2f2f 6d61 7470 6c6f 746c 6962  tps://matplotlib
-00064f30: 2e6f 7267 2f33 2e31 2e30 2f74 7574 6f72  .org/3.1.0/tutor
-00064f40: 6961 6c73 2f63 6f6c 6f72 732f 636f 6c6f  ials/colors/colo
-00064f50: 726d 6170 732e 6874 6d6c 2066 6f72 2061  rmaps.html for a
-00064f60: 2063 6f6d 7072 6568 656e 7369 7665 200d   comprehensive .
-00064f70: 0a09 0909 7365 6c65 6374 696f 6e2e 2049  ....selection. I
-00064f80: 6e20 7468 6520 636f 6465 2074 6865 2063  n the code the c
-00064f90: 6f6c 6f72 6d61 7073 2061 7265 2069 6d70  olormaps are imp
-00064fa0: 6f72 7465 6420 736f 2069 6620 706c 6f74  orted so if plot
-00064fb0: 5f66 756e 6320 6973 2069 6d70 6f72 7465  _func is importe
-00064fc0: 6420 6173 2070 6620 7468 656e 200d 0a09  d as pf then ...
-00064fd0: 0909 7365 6c66 2e63 6d61 703d 7066 2e63  ..self.cmap=pf.c
-00064fe0: 6d2e 7669 7269 6469 7320 7365 7473 2076  m.viridis sets v
-00064ff0: 6972 6964 6973 2061 7320 7468 6520 6d61  iridis as the ma
-00065000: 7020 746f 2075 7365 2e20 496e 7465 726e  p to use. Intern
-00065010: 616c 6c79 2074 6865 2063 6f6c 6f72 7320  ally the colors 
-00065020: 6172 6520 6368 6f73 656e 200d 0a09 0909  are chosen .....
-00065030: 7769 7468 2074 6865 2022 636f 6c6d 2220  with the "colm" 
-00065040: 6675 6e63 7469 6f6e 2e20 5468 6520 3264  function. The 2d
-00065050: 2070 6c6f 7473 2072 6571 7569 7265 2061   plots require a
-00065060: 2063 6f6e 7469 6e75 6f75 7320 636f 6c6f   continuous colo
-00065070: 7220 6d61 7020 736f 2069 6620 736f 6d65  r map so if some
-00065080: 7468 696e 6720 0d0a 0909 0965 6c73 6520  thing .....else 
-00065090: 6973 2067 6976 6520 3264 2070 6c6f 7473  is give 2d plots
-000650a0: 2061 7265 2073 686f 776e 2061 7574 6f6d   are shown autom
-000650b0: 6174 6963 616c 6c79 2077 6974 6820 226a  atically with "j
-000650c0: 6574 222e 2046 6f72 2061 6c6c 206f 6620  et". For all of 
-000650d0: 7468 6520 3164 2070 6c6f 7473 2068 6f77  the 1d plots how
-000650e0: 6576 6572 200d 0a09 0909 4920 6669 7273  ever .....I firs
-000650f0: 7420 7365 6c65 6374 2061 206e 756d 6265  t select a numbe
-00065100: 7220 6f66 2063 6f6c 6f72 7320 6265 666f  r of colors befo
-00065110: 7265 2065 6163 6820 706c 6f74 2e20 4966  re each plot. If
-00065120: 2063 6d61 7020 6973 2061 2063 6f6e 7469   cmap is a conti
-00065130: 6e6f 7573 206d 6170 2074 6865 6e20 7468  nous map then th
-00065140: 6573 650d 0a09 0909 6172 6520 7361 6d70  ese.....are samp
-00065150: 6c65 6420 6576 656e 6c79 206f 7665 7220  led evenly over 
-00065160: 7468 6520 636f 6c6f 7572 6d61 702e 204d  the colourmap. M
-00065170: 616e 7561 6c20 6974 6572 6162 6c65 7320  anual iterables 
-00065180: 6f66 2063 6f6c 6f75 7273 200d 0a09 0909  of colours .....
-00065190: 636d 6170 3d5b 2831 2c30 2c30 292c 2830  cmap=[(1,0,0),(0
-000651a0: 2c31 2c30 292c 2830 2c30 2c31 292c 2e2e  ,1,0),(0,0,1),..
-000651b0: 2e5d 2061 7265 2061 6c73 6f20 6163 6365  .] are also acce
-000651c0: 7074 6564 2c20 6173 2061 7265 2076 6563  pted, as are vec
-000651d0: 746f 7273 206f 7220 6461 7461 6672 616d  tors or datafram
-000651e0: 6573 2074 6861 7420 0d0a 0909 0963 6f6e  es that .....con
-000651f0: 7461 696e 2061 7320 726f 7773 2074 6865  tain as rows the
-00065200: 2063 6f6c 6f72 732e 2054 6865 7265 206d   colors. There m
-00065210: 7573 7420 6265 206f 6620 636f 7572 7365  ust be of course
-00065220: 2073 7566 6669 6369 656e 7420 636f 6c6f   sufficient colo
-00065230: 7273 2070 7265 7365 6e74 2066 6f72 200d  rs present for .
-00065240: 0a09 0909 7468 6520 6e75 6d62 6572 7320  ....the numbers 
-00065250: 6f66 206c 696e 6573 2074 6861 7420 7769  of lines that wi
-00065260: 6c6c 2062 6520 706c 6f74 7465 642e 2053  ll be plotted. S
-00065270: 6f20 4920 7265 636f 6d6d 656e 6420 746f  o I recommend to
-00065280: 2070 726f 7669 6465 2061 7420 6c65 6173   provide at leas
-00065290: 7420 3130 2063 6f6c 6f75 7273 200d 0a09  t 10 colours ...
-000652a0: 0909 2865 2e67 2e7e 796f 7572 2075 6e69  ..(e.g.~your uni
-000652b0: 7665 7273 6974 7920 636f 6c6f 7273 292e  versity colors).
-000652c0: 2063 6f6c 6f75 7273 2061 7265 2061 6c77   colours are alw
-000652d0: 6179 7320 6769 7665 6e20 6173 2061 2c20  ays given as a, 
-000652e0: 6c69 7374 206f 7220 7475 706c 6520 7769  list or tuple wi
-000652f0: 7468 2052 4741 206f 7220 5247 4241 0d0a  th RGA or RGBA..
-00065300: 0909 0928 7769 7468 2074 6865 206c 6173  ...(with the las
-00065310: 7420 4120 6265 6569 6e67 2074 6865 2041  t A beeing the A
-00065320: 6c70 6861 3d74 7261 6e73 7061 7265 6e63  lpha=transparenc
-00065330: 792e 2041 6c6c 206e 756d 6265 7273 2061  y. All numbers a
-00065340: 7265 2062 6574 7765 656e 2030 2061 6e64  re between 0 and
-00065350: 2031 2e20 0d0a 0909 0949 6620 6120 6c69   1. .....If a li
-00065360: 7374 2f76 6563 746f 722f 4461 7461 4672  st/vector/DataFr
-00065370: 616d 6520 6973 2067 6976 656e 2066 6f72  ame is given for
-00065380: 2074 6865 2063 6f6c 6f75 7273 2074 6865   the colours the
-00065390: 7920 7769 6c6c 2062 6520 7573 6564 2069  y will be used i
-000653a0: 6e20 7468 6520 6f72 6465 7220 7072 6f76  n the order prov
-000653b0: 6964 6564 2e0d 0a09 090d 0a09 0945 7861  ided.........Exa
-000653c0: 6d70 6c65 730d 0a09 092d 2d2d 2d2d 2d2d  mples....-------
-000653d0: 2d0d 0a09 090d 0a09 093e 3e3e 2069 6d70  -........>>> imp
-000653e0: 6f72 7420 706c 6f74 5f66 756e 6320 6173  ort plot_func as
-000653f0: 2070 660d 0a09 093e 3e3e 2074 6120 3d20   pf....>>> ta = 
-00065400: 7066 2e54 4128 2774 6573 7431 2e68 6466  pf.TA('test1.hdf
-00065410: 3527 2920 236f 7065 6e20 7468 6520 6f72  5') #open the or
-00065420: 6967 696e 616c 2070 726f 6a65 6374 2c20  iginal project, 
-00065430: 0d0a 0909 3e3e 3e20 7468 6973 204d 5553  ....>>> this MUS
-00065440: 5420 636f 6e74 6169 6e20 6120 6669 742c  T contain a fit,
-00065450: 206f 7468 6572 7769 7365 2074 6869 7320   otherwise this 
-00065460: 7769 6c6c 2072 6169 7365 2061 6e20 6572  will raise an er
-00065470: 726f 720d 0a09 090d 0a09 094e 6f77 206f  ror........Now o
-00065480: 7065 6e20 6120 6275 6e63 6820 6f66 206f  pen a bunch of o
-00065490: 7468 6572 2070 726f 6a65 6374 7320 746f  ther projects to
-000654a0: 2063 6f6d 7061 7265 2061 6761 696e 7374   compare against
-000654b0: 2c0d 0a09 090d 0a09 093e 3e3e 2023 636f  ,........>>> #co
-000654c0: 6d70 6172 6520 696e 2061 2073 696e 676c  mpare in a singl
-000654d0: 6520 7769 6e64 6f77 0d0a 0909 3e3e 3e20  e window....>>> 
-000654e0: 6f74 6865 725f 7072 6f6a 6563 7473 203d  other_projects =
-000654f0: 2070 662e 4755 495f 6f70 656e 2870 726f   pf.GUI_open(pro
-00065500: 6a65 6374 5f6c 6973 7420 3d20 5b27 6669  ject_list = ['fi
-00065510: 6c65 312e 6864 6635 272c 2027 6669 6c65  le1.hdf5', 'file
-00065520: 322e 6864 6635 275d 290d 0a09 093e 3e3e  2.hdf5'])....>>>
-00065530: 2074 612e 436f 6d70 6172 655f 4441 4328   ta.Compare_DAC(
-00065540: 6f74 6865 7273 203d 206f 7468 6572 5f70  others = other_p
-00065550: 726f 6a65 6374 290d 0a09 093e 3e3e 2023  roject)....>>> #
-00065560: 636f 6d70 7261 7265 2069 6e20 7365 7061  comprare in sepa
-00065570: 7261 7465 2077 696e 646f 7773 2c20 0d0a  rate windows, ..
-00065580: 0909 3e3e 3e20 2374 6865 206f 7468 6572  ..>>> #the other
-00065590: 2070 726f 6a65 6374 7320 6d75 7374 2068   projects must h
-000655a0: 6176 6520 7468 6520 7361 6d65 206e 756d  ave the same num
-000655b0: 6265 7220 6f66 2063 6f6d 706f 6e65 6e74  ber of component
-000655c0: 730d 0a09 093e 3e3e 2074 612e 436f 6d70  s....>>> ta.Comp
-000655d0: 6172 655f 4441 4328 6f74 6865 7273 203d  are_DAC(others =
-000655e0: 206f 7468 6572 5f70 726f 6a65 6374 2c20   other_project, 
-000655f0: 7365 7061 7261 7465 5f70 6c6f 7473 203d  separate_plots =
-00065600: 2054 7275 6529 0d0a 0909 0d0a 0909 436f   True)........Co
-00065610: 6d70 6172 6520 7468 6520 4441 4320 746f  mpare the DAC to
-00065620: 2061 6e20 6578 7465 726e 616c 2073 7065   an external spe
-00065630: 6374 7275 6d0d 0a09 090d 0a09 093e 3e3e  ctrum........>>>
-00065640: 2065 7874 5f73 7065 6320 3d20 7064 2e72   ext_spec = pd.r
-00065650: 6561 645f 6373 7628 2741 7363 6969 5f73  ead_csv('Ascii_s
-00065660: 7065 6374 7275 6d2e 6461 7427 2c20 7365  pectrum.dat', se
-00065670: 7020 3d20 272c 2729 0d0a 0909 3e3e 3e20  p = ',')....>>> 
-00065680: 7461 2e43 6f6d 7061 7265 5f44 4143 2873  ta.Compare_DAC(s
-00065690: 7065 6374 7261 203d 2065 7874 5f73 7065  pectra = ext_spe
-000656a0: 6329 2023 636f 6d70 6172 6520 6a75 7374  c) #compare just
-000656b0: 2074 6865 2063 7572 7265 6e74 2073 6f6c   the current sol
-000656c0: 7574 696f 6e0d 0a09 093e 3e3e 2074 612e  ution....>>> ta.
-000656d0: 436f 6d70 6172 655f 4441 4328 7370 6563  Compare_DAC(spec
-000656e0: 7472 6120 3d20 6578 745f 7370 6563 2c20  tra = ext_spec, 
-000656f0: 6f74 6865 7273 203d 206f 7468 6572 5f70  others = other_p
-00065700: 726f 6a65 6374 2920 2363 6f6d 7061 7265  roject) #compare
-00065710: 206d 756c 7469 706c 650d 0a09 090d 0a09   multiple.......
-00065720: 0927 2727 0d0a 0909 0d0a 0909 6966 2073  .'''........if s
-00065730: 656c 662e 7361 7665 5f66 6967 7572 6573  elf.save_figures
-00065740: 5f74 6f5f 666f 6c64 6572 3a73 656c 662e  _to_folder:self.
-00065750: 6669 6775 7265 5f70 6174 6820 3d20 6368  figure_path = ch
-00065760: 6563 6b5f 666f 6c64 6572 2870 6174 6820  eck_folder(path 
-00065770: 3d20 2772 6573 756c 745f 6669 6775 7265  = 'result_figure
-00065780: 7327 2c20 6375 7272 656e 745f 7061 7468  s', current_path
-00065790: 203d 2073 656c 662e 7061 7468 290d 0a09   = self.path)...
-000657a0: 0969 6620 6f74 6865 7220 6973 206e 6f74  .if other is not
-000657b0: 204e 6f6e 653a 0d0a 0909 0969 6620 6e6f   None:.....if no
-000657c0: 7420 6861 7361 7474 7228 6f74 6865 722c  t hasattr(other,
-000657d0: 2027 5f5f 6974 6572 5f5f 2729 3a6f 7468   '__iter__'):oth
-000657e0: 6572 203d 205b 6f74 6865 725d 0d0a 0909  er = [other]....
-000657f0: 7472 793a 0d0a 0909 0972 6520 3d20 7365  try:.....re = se
-00065800: 6c66 2e72 652e 636f 7079 2829 0d0a 0909  lf.re.copy()....
-00065810: 6578 6365 7074 3a0d 0a09 0909 7072 696e  except:.....prin
-00065820: 7428 224e 6f20 6669 7474 6564 2072 6573  t("No fitted res
-00065830: 756c 7473 2070 7265 7365 6e74 2229 0d0a  ults present")..
-00065840: 0909 0972 6574 7572 6e20 4661 6c73 650d  ...return False.
-00065850: 0a09 0969 6620 636d 6170 2069 7320 4e6f  ...if cmap is No
-00065860: 6e65 3a63 6d61 7020 3d20 7365 6c66 2e63  ne:cmap = self.c
-00065870: 6d61 700d 0a09 0973 7065 6369 6573 3d72  map....species=r
-00065880: 655b 2744 4143 275d 2e63 6f6c 756d 6e73  e['DAC'].columns
-00065890: 2e76 616c 7565 730d 0a09 0969 6620 6f74  .values....if ot
-000658a0: 6865 7220 6973 204e 6f6e 653a 0d0a 0909  her is None:....
-000658b0: 0963 6f6c 203d 2072 616e 6765 286c 656e  .col = range(len
-000658c0: 2872 655b 2744 4143 275d 2e63 6f6c 756d  (re['DAC'].colum
-000658d0: 6e73 2e76 616c 7565 7329 290d 0a09 0909  ns.values)).....
-000658e0: 636f 6c6f 7273 203d 2063 6f6c 6d28 636d  colors = colm(cm
-000658f0: 6170 203d 2063 6d61 702c 206b 203d 2063  ap = cmap, k = c
-00065900: 6f6c 290d 0a09 0909 0d0a 0909 656c 7365  ol).........else
-00065910: 3a0d 0a09 0909 7265 5b27 4441 4327 5d2e  :.....re['DAC'].
-00065920: 636f 6c75 6d6e 7320 3d20 5b73 656c 662e  columns = [self.
-00065930: 6669 6c65 6e61 6d65 202b 2027 5c6e 2720  filename + '\n' 
-00065940: 2b20 2725 7327 2561 2066 6f72 2061 2069  + '%s'%a for a i
-00065950: 6e20 7265 5b27 4441 4327 5d2e 636f 6c75  n re['DAC'].colu
-00065960: 6d6e 735d 0d0a 0909 0969 6620 7365 7061  mns].....if sepa
-00065970: 7261 7465 5f70 6c6f 7473 3a0d 0a09 0909  rate_plots:.....
-00065980: 0963 6f6c 6f72 7320 3d20 636f 6c6d 2863  .colors = colm(c
-00065990: 6d61 7020 3d20 636d 6170 2c20 6b20 3d20  map = cmap, k = 
-000659a0: 6e70 2e61 7261 6e67 6528 6c65 6e28 6f74  np.arange(len(ot
-000659b0: 6865 7229 2b31 2929 0d0a 0909 0965 6c73  her)+1)).....els
-000659c0: 653a 0d0a 0909 0909 636f 6c6f 7273 203d  e:......colors =
-000659d0: 2063 6f6c 6d28 636d 6170 203d 2063 6d61   colm(cmap = cma
-000659e0: 702c 206b 203d 206e 702e 6172 616e 6765  p, k = np.arange
-000659f0: 2828 6c65 6e28 6f74 6865 7229 2b31 292a  ((len(other)+1)*
-00065a00: 6c65 6e28 7370 6563 6965 7329 2929 0d0a  len(species)))..
-00065a10: 0909 4441 4320 3d20 7265 5b27 4441 4327  ..DAC = re['DAC'
-00065a20: 5d0d 0a09 0968 616e 643d 5b5d 0d0a 0909  ]....hand=[]....
-00065a30: 6966 2073 6570 6172 6174 655f 706c 6f74  if separate_plot
-00065a40: 733a 0d0a 0909 096e 5f63 6f6c 7320 3d20  s:.....n_cols = 
-00065a50: 696e 7428 6e70 2e63 6569 6c28 6c65 6e28  int(np.ceil(len(
-00065a60: 7265 5b27 4441 4327 5d2e 636f 6c75 6d6e  re['DAC'].column
-00065a70: 7329 2f32 2929 0d0a 0909 0963 6f6c 203d  s)/2)).....col =
-00065a80: 205b 636f 6c6f 7273 5b30 5d20 666f 7220   [colors[0] for 
-00065a90: 6120 696e 2072 616e 6765 286c 656e 2872  a in range(len(r
-00065aa0: 655b 2744 4143 275d 2e63 6f6c 756d 6e73  e['DAC'].columns
-00065ab0: 2929 5d0d 0a09 0909 6966 2073 656c 662e  ))].....if self.
-00065ac0: 7363 6174 7465 7263 7574 2069 7320 4e6f  scattercut is No
-00065ad0: 6e65 3a09 0d0a 0909 0909 6178 203d 2044  ne:.......ax = D
-00065ae0: 4143 2e70 6c6f 7428 7375 6270 6c6f 7473  AC.plot(subplots
-00065af0: 203d 2073 6570 6172 6174 655f 706c 6f74   = separate_plot
-00065b00: 732c 2066 6967 7369 7a65 203d 2028 3132  s, figsize = (12
-00065b10: 2c20 3130 292c 206c 6179 6f75 7420 3d20  , 10), layout = 
-00065b20: 286e 5f63 6f6c 732c 2032 292c 200d 0a09  (n_cols, 2), ...
-00065b30: 0909 0909 0909 0909 6c65 6765 6e64 203d  ........legend =
-00065b40: 2046 616c 7365 2c20 636f 6c6f 7220 3d20   False, color = 
-00065b50: 636f 6c2c 2073 6861 7265 7820 3d20 4661  col, sharex = Fa
-00065b60: 6c73 6529 0d0a 0d0a 0909 0909 613d 6178  lse)........a=ax
-00065b70: 2e72 6176 656c 2829 0d0a 0909 0909 6861  .ravel()......ha
-00065b80: 6e64 6c65 732c 6c61 6265 6c73 3d61 5b30  ndles,labels=a[0
-00065b90: 5d2e 6765 745f 6c65 6765 6e64 5f68 616e  ].get_legend_han
-00065ba0: 646c 6573 5f6c 6162 656c 7328 290d 0a09  dles_labels()...
-00065bb0: 0909 0968 616e 642e 6170 7065 6e64 2868  ...hand.append(h
-00065bc0: 616e 646c 6573 5b2d 315d 290d 0a09 0909  andles[-1]).....
-00065bd0: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
-00065be0: 7365 6c66 2e73 6361 7474 6572 6375 745b  self.scattercut[
-00065bf0: 305d 2c20 206e 756d 6265 7273 2e4e 756d  0],  numbers.Num
-00065c00: 6265 7229 3a0d 0a09 0909 0961 7820 3d20  ber):......ax = 
-00065c10: 4441 432e 6c6f 635b 3a73 656c 662e 7363  DAC.loc[:self.sc
-00065c20: 6174 7465 7263 7574 5b30 5d2c 203a 5d2e  attercut[0], :].
-00065c30: 706c 6f74 2873 7562 706c 6f74 7320 3d20  plot(subplots = 
-00065c40: 7365 7061 7261 7465 5f70 6c6f 7473 2c20  separate_plots, 
-00065c50: 6669 6773 697a 6520 3d20 2831 322c 2031  figsize = (12, 1
-00065c60: 3029 2c20 6c61 796f 7574 203d 2028 6e5f  0), layout = (n_
-00065c70: 636f 6c73 2c20 3229 2c20 0d0a 0909 0909  cols, 2), ......
-00065c80: 0909 0909 0909 0909 096c 6567 656e 6420  .........legend 
-00065c90: 3d20 4661 6c73 652c 2063 6f6c 6f72 203d  = False, color =
-00065ca0: 2063 6f6c 2c20 7368 6172 6578 203d 2046   col, sharex = F
-00065cb0: 616c 7365 2909 0909 0909 0909 090d 0a09  alse)...........
-00065cc0: 0909 0961 3d61 782e 7261 7665 6c28 290d  ...a=ax.ravel().
-00065cd0: 0a09 0909 0968 616e 646c 6573 2c6c 6162  .....handles,lab
-00065ce0: 656c 733d 615b 305d 2e67 6574 5f6c 6567  els=a[0].get_leg
-00065cf0: 656e 645f 6861 6e64 6c65 735f 6c61 6265  end_handles_labe
-00065d00: 6c73 2829 0d0a 0909 0909 6861 6e64 2e61  ls()......hand.a
-00065d10: 7070 656e 6428 6861 6e64 6c65 735b 2d31  ppend(handles[-1
-00065d20: 5d29 090d 0a09 0909 0944 4143 5f63 7574  ]).......DAC_cut
-00065d30: 3d44 4143 2e6c 6f63 5b73 656c 662e 7363  =DAC.loc[self.sc
-00065d40: 6174 7465 7263 7574 5b31 5d3a 2c20 3a5d  attercut[1]:, :]
-00065d50: 0d0a 0909 0909 666f 7220 692c 616d 2069  ......for i,am i
-00065d60: 6e20 656e 756d 6572 6174 6528 4441 435f  n enumerate(DAC_
-00065d70: 6375 742e 636f 6c75 6d6e 7329 3a0d 0a09  cut.columns):...
-00065d80: 0909 0909 4441 435f 6375 742e 696c 6f63  ....DAC_cut.iloc
-00065d90: 5b3a 2c69 5d2e 706c 6f74 2861 7820 3d20  [:,i].plot(ax = 
-00065da0: 615b 695d 2c20 6c65 6765 6e64 203d 2046  a[i], legend = F
-00065db0: 616c 7365 2c20 636f 6c6f 7220 3d20 636f  alse, color = co
-00065dc0: 6c29 0d0a 0909 0965 6c73 653a 0d0a 0909  l).....else:....
-00065dd0: 0909 7363 6174 7465 7263 7574 203d 2066  ..scattercut = f
-00065de0: 6c61 7474 656e 2873 656c 662e 7363 6174  latten(self.scat
-00065df0: 7465 7263 7574 290d 0a09 0909 0966 6f72  tercut)......for
-00065e00: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
-00065e10: 7363 6174 7465 7263 7574 292f 322b 3129  scattercut)/2+1)
-00065e20: 3a0d 0a09 0909 0909 6966 2069 203d 3d20  :.......if i == 
-00065e30: 303a 0d0a 0909 0909 0909 6178 203d 2044  0:........ax = D
-00065e40: 4143 2e6c 6f63 5b3a 7363 6174 7465 7263  AC.loc[:scatterc
-00065e50: 7574 5b30 5d2c 203a 5d2e 706c 6f74 2873  ut[0], :].plot(s
-00065e60: 7562 706c 6f74 7320 3d20 7365 7061 7261  ubplots = separa
-00065e70: 7465 5f70 6c6f 7473 2c20 6669 6773 697a  te_plots, figsiz
-00065e80: 6520 3d20 2831 322c 2031 3029 2c20 0d0a  e = (12, 10), ..
-00065e90: 0909 0909 0909 0909 0909 0909 0909 6c61  ..............la
-00065ea0: 796f 7574 203d 2028 6e5f 636f 6c73 2c20  yout = (n_cols, 
-00065eb0: 3229 2c20 6c65 6765 6e64 203d 2046 616c  2), legend = Fal
-00065ec0: 7365 2c20 636f 6c6f 7220 3d20 636f 6c2c  se, color = col,
-00065ed0: 2073 6861 7265 7820 3d20 4661 6c73 6529   sharex = False)
-00065ee0: 0d0a 0909 0909 0909 0d0a 0909 0909 0909  ................
-00065ef0: 613d 6178 2e72 6176 656c 2829 0d0a 0909  a=ax.ravel()....
-00065f00: 0909 0909 6861 6e64 6c65 732c 6c61 6265  ....handles,labe
-00065f10: 6c73 3d61 5b30 5d2e 6765 745f 6c65 6765  ls=a[0].get_lege
-00065f20: 6e64 5f68 616e 646c 6573 5f6c 6162 656c  nd_handles_label
-00065f30: 7328 290d 0a09 0909 0909 0968 616e 642e  s()........hand.
-00065f40: 6170 7065 6e64 2868 616e 646c 6573 5b2d  append(handles[-
-00065f50: 315d 2909 0d0a 0909 0909 0965 6c69 6620  1])........elif 
-00065f60: 693c 286c 656e 2873 6361 7474 6572 6375  i<(len(scattercu
-00065f70: 7429 2f32 293a 0d0a 0909 0909 0909 666f  t)/2):........fo
-00065f80: 7220 6a2c 616d 2069 6e20 656e 756d 6572  r j,am in enumer
-00065f90: 6174 6528 6178 293a 0d0a 0909 0909 0909  ate(ax):........
-00065fa0: 0944 4143 2e6c 6f63 5b73 6361 7474 6572  .DAC.loc[scatter
-00065fb0: 6375 745b 322a 692d 315d 3a73 6361 7474  cut[2*i-1]:scatt
-00065fc0: 6572 6375 745b 322a 695d 2c20 3a5d 2e70  ercut[2*i], :].p
-00065fd0: 6c6f 7428 6178 203d 2061 5b6a 5d2c 206c  lot(ax = a[j], l
-00065fe0: 6567 656e 6420 3d20 4661 6c73 652c 2063  egend = False, c
-00065ff0: 6f6c 6f72 203d 2063 6f6c 2c20 6c61 6265  olor = col, labe
-00066000: 6c20 3d20 275f 6e6f 6c65 6765 6e64 5f27  l = '_nolegend_'
-00066010: 290d 0a09 0909 0909 656c 7365 3a0d 0a09  ).......else:...
-00066020: 0909 0909 0966 6f72 206a 2c61 6d20 696e  .....for j,am in
-00066030: 2065 6e75 6d65 7261 7465 2861 7829 3a0d   enumerate(ax):.
-00066040: 0a09 0909 0909 0909 4441 432e 6c6f 635b  ........DAC.loc[
-00066050: 7363 6174 7465 7263 7574 5b2d 315d 3a2c  scattercut[-1]:,
-00066060: 203a 5d2e 706c 6f74 2861 7820 3d20 615b   :].plot(ax = a[
-00066070: 6a5d 2c20 6c65 6765 6e64 203d 2046 616c  j], legend = Fal
-00066080: 7365 2c20 636f 6c6f 7220 3d20 636f 6c2c  se, color = col,
-00066090: 206c 6162 656c 203d 2027 5f6e 6f6c 6567   label = '_noleg
-000660a0: 656e 645f 2729 0d0a 0909 656c 7365 3a0d  end_')....else:.
-000660b0: 0a09 0909 6966 2073 656c 662e 7363 6174  ....if self.scat
-000660c0: 7465 7263 7574 2069 7320 4e6f 6e65 3a09  tercut is None:.
-000660d0: 0d0a 0909 0909 6178 2020 3d20 2044 4143  ......ax  =  DAC
-000660e0: 2e70 6c6f 7428 7375 6270 6c6f 7473 203d  .plot(subplots =
-000660f0: 2073 6570 6172 6174 655f 706c 6f74 732c   separate_plots,
-00066100: 2066 6967 7369 7a65 203d 2028 3136 2c20   figsize = (16, 
-00066110: 3829 2c20 6c65 6765 6e64 203d 2046 616c  8), legend = Fal
-00066120: 7365 2c20 636f 6c6f 7220 3d20 636f 6c6f  se, color = colo
-00066130: 7273 5b3a 6c65 6e28 7370 6563 6965 7329  rs[:len(species)
-00066140: 5d2c 206c 6162 656c 203d 2027 5f6e 6f6c  ], label = '_nol
-00066150: 6567 656e 645f 2729 0d0a 0909 0965 6c69  egend_').....eli
-00066160: 6620 6973 696e 7374 616e 6365 2873 656c  f isinstance(sel
-00066170: 662e 7363 6174 7465 7263 7574 5b30 5d2c  f.scattercut[0],
-00066180: 206e 756d 6265 7273 2e4e 756d 6265 7229   numbers.Number)
-00066190: 3a0d 0a09 0909 0961 7820 203d 2020 4441  :......ax  =  DA
-000661a0: 432e 6c6f 635b 3a73 656c 662e 7363 6174  C.loc[:self.scat
-000661b0: 7465 7263 7574 5b30 5d2c 203a 5d2e 706c  tercut[0], :].pl
-000661c0: 6f74 2873 7562 706c 6f74 7320 3d20 7365  ot(subplots = se
-000661d0: 7061 7261 7465 5f70 6c6f 7473 2c20 6669  parate_plots, fi
-000661e0: 6773 697a 6520 3d20 2831 362c 2038 292c  gsize = (16, 8),
-000661f0: 206c 6567 656e 6420 3d20 4661 6c73 652c   legend = False,
-00066200: 2063 6f6c 6f72 203d 2063 6f6c 6f72 735b   color = colors[
-00066210: 3a6c 656e 2873 7065 6369 6573 295d 2c20  :len(species)], 
-00066220: 6c61 6265 6c20 3d20 275f 6e6f 6c65 6765  label = '_nolege
-00066230: 6e64 5f27 290d 0a09 0909 0961 7820 203d  nd_')......ax  =
-00066240: 2020 4441 432e 6c6f 635b 7365 6c66 2e73    DAC.loc[self.s
-00066250: 6361 7474 6572 6375 745b 315d 3a2c 2020  cattercut[1]:,  
-00066260: 3a5d 2e70 6c6f 7428 6178 3d61 782c 2073  :].plot(ax=ax, s
-00066270: 7562 706c 6f74 7320 3d20 7365 7061 7261  ubplots = separa
-00066280: 7465 5f70 6c6f 7473 2c20 6669 6773 697a  te_plots, figsiz
-00066290: 6520 3d20 2831 362c 2038 292c 206c 6567  e = (16, 8), leg
-000662a0: 656e 6420 3d20 4661 6c73 652c 2063 6f6c  end = False, col
-000662b0: 6f72 203d 2063 6f6c 6f72 735b 3a6c 656e  or = colors[:len
-000662c0: 2873 7065 6369 6573 295d 2c20 6c61 6265  (species)], labe
-000662d0: 6c20 3d20 275f 6e6f 6c65 6765 6e64 5f27  l = '_nolegend_'
-000662e0: 290d 0a09 0909 656c 7365 3a0d 0a09 0909  ).....else:.....
-000662f0: 0973 6361 7474 6572 6375 7420 203d 2020  .scattercut  =  
-00066300: 666c 6174 7465 6e28 7365 6c66 2e73 6361  flatten(self.sca
-00066310: 7474 6572 6375 7429 0d0a 0909 0909 666f  ttercut)......fo
-00066320: 7220 6920 696e 2072 616e 6765 286c 656e  r i in range(len
-00066330: 2873 6361 7474 6572 6375 7429 2f32 2b31  (scattercut)/2+1
-00066340: 293a 0d0a 0909 0909 0969 6620 6920 203d  ):.......if i  =
-00066350: 3d20 2030 3a0d 0a09 0909 0909 0961 7820  =  0:........ax 
-00066360: 203d 2020 4441 432e 6c6f 635b 3a73 6361   =  DAC.loc[:sca
-00066370: 7474 6572 6375 745b 305d 2c20 203a 5d2e  ttercut[0],  :].
-00066380: 706c 6f74 2873 7562 706c 6f74 7320 3d20  plot(subplots = 
-00066390: 7365 7061 7261 7465 5f70 6c6f 7473 2c20  separate_plots, 
-000663a0: 6669 6773 697a 6520 3d20 2831 362c 2038  figsize = (16, 8
-000663b0: 292c 206c 6567 656e 6420 3d20 4661 6c73  ), legend = Fals
-000663c0: 652c 2063 6f6c 6f72 203d 2063 6f6c 6f72  e, color = color
-000663d0: 735b 3a6c 656e 2873 7065 6369 6573 295d  s[:len(species)]
-000663e0: 2c20 6c61 6265 6c20 3d20 275f 6e6f 6c65  , label = '_nole
-000663f0: 6765 6e64 5f27 290d 0a09 0909 0909 656c  gend_').......el
-00066400: 6966 2069 3c28 6c65 6e28 7363 6174 7465  if i<(len(scatte
-00066410: 7263 7574 292f 3229 3a0d 0a09 0909 0909  rcut)/2):.......
-00066420: 0961 7820 203d 2020 4441 432e 6c6f 635b  .ax  =  DAC.loc[
-00066430: 7363 6174 7465 7263 7574 5b32 2a69 2d31  scattercut[2*i-1
-00066440: 5d3a 7363 6174 7465 7263 7574 5b32 2a69  ]:scattercut[2*i
-00066450: 5d2c 2020 3a5d 2e70 6c6f 7428 6178 3d61  ],  :].plot(ax=a
-00066460: 782c 2073 7562 706c 6f74 7320 3d20 7365  x, subplots = se
-00066470: 7061 7261 7465 5f70 6c6f 7473 2c20 6669  parate_plots, fi
-00066480: 6773 697a 6520 3d20 2831 362c 2038 292c  gsize = (16, 8),
-00066490: 206c 6567 656e 6420 3d20 4661 6c73 652c   legend = False,
-000664a0: 2063 6f6c 6f72 203d 2063 6f6c 6f72 735b   color = colors[
-000664b0: 3a6c 656e 2873 7065 6369 6573 295d 2c20  :len(species)], 
-000664c0: 6c61 6265 6c20 3d20 275f 6e6f 6c65 6765  label = '_nolege
-000664d0: 6e64 5f27 290d 0a09 0909 0909 656c 7365  nd_').......else
-000664e0: 3a0d 0a09 0909 0909 0961 7820 203d 2020  :........ax  =  
-000664f0: 4441 432e 6c6f 635b 7363 6174 7465 7263  DAC.loc[scatterc
-00066500: 7574 5b2d 315d 3a2c 2020 3a5d 2e70 6c6f  ut[-1]:,  :].plo
-00066510: 7428 6178 3d61 782c 2073 7562 706c 6f74  t(ax=ax, subplot
-00066520: 7320 3d20 7365 7061 7261 7465 5f70 6c6f  s = separate_plo
-00066530: 7473 2c20 6669 6773 697a 6520 3d20 2831  ts, figsize = (1
-00066540: 362c 2038 292c 206c 6567 656e 6420 3d20  6, 8), legend = 
-00066550: 4661 6c73 652c 2063 6f6c 6f72 203d 2063  False, color = c
-00066560: 6f6c 6f72 735b 3a6c 656e 2873 7065 6369  olors[:len(speci
-00066570: 6573 295d 2c20 6c61 6265 6c20 3d20 275f  es)], label = '_
-00066580: 6e6f 6c65 6765 6e64 5f27 290d 0a09 0969  nolegend_')....i
-00066590: 6620 6f74 6865 7220 6973 206e 6f74 204e  f other is not N
-000665a0: 6f6e 653a 0d0a 0909 0966 6f72 2069 2c6f  one:.....for i,o
-000665b0: 2069 6e20 656e 756d 6572 6174 6528 6f74   in enumerate(ot
-000665c0: 6865 7229 3a0d 0a09 0909 0974 7279 3a0d  her):......try:.
-000665d0: 0a09 0909 0909 7265 3d6f 2e72 652e 636f  ......re=o.re.co
-000665e0: 7079 2829 0d0a 0909 0909 6578 6365 7074  py()......except
-000665f0: 3a0d 0a09 0909 0909 7072 696e 7428 2725  :.......print('%
-00066600: 7320 6861 7320 6e6f 2066 6974 7465 6420  s has no fitted 
-00066610: 7265 7375 6c74 7327 256f 2e66 696c 656e  results'%o.filen
-00066620: 616d 6529 0d0a 0909 0909 0963 6f6e 7469  ame).......conti
-00066630: 6e75 650d 0a09 0909 0972 655b 2744 4143  nue......re['DAC
-00066640: 275d 2e63 6f6c 756d 6e73 3d5b 6f2e 6669  '].columns=[o.fi
-00066650: 6c65 6e61 6d65 202b 2027 5c6e 2720 2b20  lename + '\n' + 
-00066660: 2725 7327 2561 2066 6f72 2061 2069 6e20  '%s'%a for a in 
-00066670: 7265 5b27 4441 4327 5d2e 636f 6c75 6d6e  re['DAC'].column
-00066680: 735d 0d0a 0909 0909 6966 2073 6570 6172  s]......if separ
-00066690: 6174 655f 706c 6f74 733a 0909 0909 0d0a  ate_plots:......
-000666a0: 0909 0909 0963 6f6c 3d5b 636f 6c6f 7273  .....col=[colors
-000666b0: 5b69 2b31 5d20 666f 7220 6120 696e 2072  [i+1] for a in r
-000666c0: 616e 6765 286c 656e 2872 655b 2744 4143  ange(len(re['DAC
-000666d0: 275d 2e63 6f6c 756d 6e73 2929 5d0d 0a09  '].columns))]...
-000666e0: 0909 0909 666f 7220 6a2c 616d 2069 6e20  ....for j,am in 
-000666f0: 656e 756d 6572 6174 6528 7265 5b27 4441  enumerate(re['DA
-00066700: 4327 5d2e 636f 6c75 6d6e 7329 3a0d 0a09  C'].columns):...
-00066710: 0909 0909 0969 6620 6f2e 7363 6174 7465  .....if o.scatte
-00066720: 7263 7574 2069 7320 4e6f 6e65 3a09 0d0a  rcut is None:...
-00066730: 0909 0909 0909 0972 655b 2744 4143 275d  .......re['DAC']
-00066740: 2e69 6c6f 635b 3a2c 6a5d 2e70 6c6f 7428  .iloc[:,j].plot(
-00066750: 7375 6270 6c6f 7473 3d46 616c 7365 2c61  subplots=False,a
-00066760: 783d 615b 6a5d 2c6c 6567 656e 643d 4661  x=a[j],legend=Fa
-00066770: 6c73 652c 636f 6c6f 723d 636f 6c5b 695d  lse,color=col[i]
-00066780: 290d 0a09 0909 0909 0909 6966 206a 3d3d  ).........if j==
-00066790: 303a 0d0a 0909 0909 0909 0909 6861 6e64  0:..........hand
-000667a0: 6c65 732c 6c61 6265 6c73 3d61 5b30 5d2e  les,labels=a[0].
-000667b0: 6765 745f 6c65 6765 6e64 5f68 616e 646c  get_legend_handl
-000667c0: 6573 5f6c 6162 656c 7328 290d 0a09 0909  es_labels().....
-000667d0: 0909 0909 0968 616e 642e 6170 7065 6e64  .....hand.append
-000667e0: 2868 616e 646c 6573 5b2d 315d 2909 0d0a  (handles[-1])...
-000667f0: 0909 0909 0909 656c 6966 2069 7369 6e73  ......elif isins
-00066800: 7461 6e63 6528 6f2e 7363 6174 7465 7263  tance(o.scatterc
-00066810: 7574 5b30 5d2c 2020 6e75 6d62 6572 732e  ut[0],  numbers.
-00066820: 4e75 6d62 6572 293a 0d0a 0909 0909 0909  Number):........
-00066830: 0972 655b 2744 4143 275d 2e69 6c6f 635b  .re['DAC'].iloc[
-00066840: 3a2c 6a5d 2e6c 6f63 5b3a 6f2e 7363 6174  :,j].loc[:o.scat
-00066850: 7465 7263 7574 5b30 5d5d 2e70 6c6f 7428  tercut[0]].plot(
-00066860: 7375 6270 6c6f 7473 3d46 616c 7365 2c61  subplots=False,a
-00066870: 783d 615b 6a5d 2c6c 6567 656e 643d 4661  x=a[j],legend=Fa
-00066880: 6c73 652c 636f 6c6f 723d 636f 6c5b 695d  lse,color=col[i]
-00066890: 290d 0a09 0909 0909 0909 6966 206a 3d3d  ).........if j==
-000668a0: 303a 0d0a 0909 0909 0909 0909 6861 6e64  0:..........hand
-000668b0: 6c65 732c 6c61 6265 6c73 3d61 5b30 5d2e  les,labels=a[0].
-000668c0: 6765 745f 6c65 6765 6e64 5f68 616e 646c  get_legend_handl
-000668d0: 6573 5f6c 6162 656c 7328 290d 0a09 0909  es_labels().....
-000668e0: 0909 0909 0968 616e 642e 6170 7065 6e64  .....hand.append
-000668f0: 2868 616e 646c 6573 5b2d 315d 2909 0d0a  (handles[-1])...
-00066900: 0909 0909 0909 0972 655b 2744 4143 275d  .......re['DAC']
-00066910: 2e69 6c6f 635b 3a2c 6a5d 2e6c 6f63 5b6f  .iloc[:,j].loc[o
-00066920: 2e73 6361 7474 6572 6375 745b 315d 3a5d  .scattercut[1]:]
-00066930: 2e70 6c6f 7428 7375 6270 6c6f 7473 3d46  .plot(subplots=F
-00066940: 616c 7365 2c61 783d 615b 6a5d 2c6c 6567  alse,ax=a[j],leg
-00066950: 656e 643d 4661 6c73 652c 636f 6c6f 723d  end=False,color=
-00066960: 636f 6c5b 695d 2c6c 6162 656c 203d 2027  col[i],label = '
-00066970: 5f6e 6f6c 6567 656e 645f 2729 0d0a 0909  _nolegend_')....
-00066980: 0909 0909 656c 7365 3a0d 0a09 0909 0909  ....else:.......
-00066990: 0909 7363 6174 7465 7263 7574 203d 2066  ..scattercut = f
-000669a0: 6c61 7474 656e 286f 2e73 6361 7474 6572  latten(o.scatter
-000669b0: 6375 7429 0d0a 0909 0909 0909 0966 6f72  cut).........for
-000669c0: 206d 2069 6e20 7261 6e67 6528 6c65 6e28   m in range(len(
-000669d0: 7363 6174 7465 7263 7574 292f 322b 3129  scattercut)/2+1)
-000669e0: 3a0d 0a09 0909 0909 0909 0969 6620 6d20  :..........if m 
-000669f0: 3d3d 2030 3a0d 0a09 0909 0909 0909 0909  == 0:...........
-00066a00: 7265 5b27 4441 4327 5d2e 696c 6f63 5b3a  re['DAC'].iloc[:
-00066a10: 2c6a 5d2e 6c6f 635b 3a73 6361 7474 6572  ,j].loc[:scatter
-00066a20: 6375 745b 305d 5d2e 706c 6f74 2873 7562  cut[0]].plot(sub
-00066a30: 706c 6f74 733d 4661 6c73 652c 6178 3d61  plots=False,ax=a
-00066a40: 5b6a 5d2c 6c65 6765 6e64 3d46 616c 7365  [j],legend=False
-00066a50: 2c63 6f6c 6f72 3d63 6f6c 5b69 5d29 0d0a  ,color=col[i])..
-00066a60: 0909 0909 0909 0909 0969 6620 6a3d 3d30  .........if j==0
-00066a70: 3a0d 0a09 0909 0909 0909 0909 0968 616e  :............han
-00066a80: 646c 6573 2c6c 6162 656c 733d 615b 6a5d  dles,labels=a[j]
-00066a90: 2e67 6574 5f6c 6567 656e 645f 6861 6e64  .get_legend_hand
-00066aa0: 6c65 735f 6c61 6265 6c73 2829 0d0a 0909  les_labels()....
-00066ab0: 0909 0909 0909 0909 6861 6e64 2e61 7070  ........hand.app
-00066ac0: 656e 6428 6861 6e64 6c65 735b 2d31 5d29  end(handles[-1])
-00066ad0: 090d 0a09 0909 0909 0909 0965 6c69 6620  ...........elif 
-00066ae0: 6d3c 286c 656e 2873 6361 7474 6572 6375  m<(len(scattercu
-00066af0: 7429 2f32 293a 0d0a 0909 0909 0909 0909  t)/2):..........
-00066b00: 0972 655b 2744 4143 275d 2e69 6c6f 635b  .re['DAC'].iloc[
-00066b10: 3a2c 6a5d 2e6c 6f63 5b73 6361 7474 6572  :,j].loc[scatter
-00066b20: 6375 745b 322a 6d2d 315d 3a73 6361 7474  cut[2*m-1]:scatt
-00066b30: 6572 6375 745b 322a 6d5d 5d2e 706c 6f74  ercut[2*m]].plot
-00066b40: 2873 7562 706c 6f74 733d 4661 6c73 652c  (subplots=False,
-00066b50: 6178 3d61 5b6a 5d2c 6c65 6765 6e64 3d46  ax=a[j],legend=F
-00066b60: 616c 7365 2c63 6f6c 6f72 3d63 6f6c 5b69  alse,color=col[i
-00066b70: 5d2c 6c61 6265 6c20 3d20 275f 6e6f 6c65  ],label = '_nole
-00066b80: 6765 6e64 5f27 290d 0a09 0909 0909 0909  gend_').........
-00066b90: 0965 6c73 653a 0d0a 0909 0909 0909 0909  .else:..........
-00066ba0: 0972 655b 2744 4143 275d 2e69 6c6f 635b  .re['DAC'].iloc[
-00066bb0: 3a2c 6a5d 2e6c 6f63 5b73 6361 7474 6572  :,j].loc[scatter
-00066bc0: 6375 745b 2d31 5d3a 5d2e 706c 6f74 2873  cut[-1]:].plot(s
-00066bd0: 7562 706c 6f74 733d 4661 6c73 652c 6178  ubplots=False,ax
-00066be0: 3d61 5b6a 5d2c 6c65 6765 6e64 3d46 616c  =a[j],legend=Fal
-00066bf0: 7365 2c63 6f6c 6f72 3d63 6f6c 5b69 5d2c  se,color=col[i],
-00066c00: 6c61 6265 6c20 3d20 275f 6e6f 6c65 6765  label = '_nolege
-00066c10: 6e64 5f27 290d 0a09 0909 0909 0961 5b6a  nd_')........a[j
-00066c20: 5d2e 7365 745f 786c 6162 656c 2827 5761  ].set_xlabel('Wa
-00066c30: 7665 6c65 6e67 7468 2069 6e20 6e6d 2729  velength in nm')
-00066c40: 0909 0909 0d0a 0909 0909 0909 615b 6a5d  ............a[j]
-00066c50: 2e73 6574 5f79 6c61 6265 6c28 2753 7065  .set_ylabel('Spe
-00066c60: 6374 7261 6c20 7374 7265 6e67 7468 2069  ctral strength i
-00066c70: 6e20 6172 622e 2075 6e69 7473 2729 0d0a  n arb. units')..
-00066c80: 0909 0909 0909 615b 6a5d 2e6c 6567 656e  ......a[j].legen
-00066c90: 6428 666f 6e74 7369 7a65 3d38 2c66 7261  d(fontsize=8,fra
-00066ca0: 6d65 6f6e 3d46 616c 7365 290d 0a09 0909  meon=False).....
-00066cb0: 0d0a 0909 0909 656c 7365 3a0d 0a09 0909  ......else:.....
-00066cc0: 0909 6461 6373 3d6c 656e 2872 655b 2744  ..dacs=len(re['D
-00066cd0: 4143 275d 2e63 6f6c 756d 6e73 290d 0a09  AC'].columns)...
-00066ce0: 0909 0909 636f 6c3d 636f 6c6f 7273 5b28  ....col=colors[(
-00066cf0: 692b 3129 2a64 6163 733a 2869 2b32 292a  i+1)*dacs:(i+2)*
-00066d00: 6461 6373 5d09 0d0a 0909 0909 0944 4143  dacs]........DAC
-00066d10: 3d72 655b 2744 4143 275d 0d0a 0909 0909  =re['DAC']......
-00066d20: 0969 6620 6f2e 7363 6174 7465 7263 7574  .if o.scattercut
-00066d30: 2069 7320 4e6f 6e65 3a09 0d0a 0909 0909   is None:.......
-00066d40: 0909 6178 203d 2044 4143 2e70 6c6f 7428  ..ax = DAC.plot(
-00066d50: 7375 6270 6c6f 7473 3d73 6570 6172 6174  subplots=separat
-00066d60: 655f 706c 6f74 732c 6178 3d61 782c 6c65  e_plots,ax=ax,le
-00066d70: 6765 6e64 3d46 616c 7365 2c63 6f6c 6f72  gend=False,color
-00066d80: 3d63 6f6c 6f72 735b 2869 2b31 292a 6c65  =colors[(i+1)*le
-00066d90: 6e28 7370 6563 6965 7329 3a28 692b 3229  n(species):(i+2)
-00066da0: 2a6c 656e 2873 7065 6369 6573 295d 290d  *len(species)]).
-00066db0: 0a09 0909 0909 656c 6966 2069 7369 6e73  ......elif isins
-00066dc0: 7461 6e63 6528 6f2e 7363 6174 7465 7263  tance(o.scatterc
-00066dd0: 7574 5b30 5d2c 2020 6e75 6d62 6572 732e  ut[0],  numbers.
-00066de0: 4e75 6d62 6572 293a 0d0a 0909 0909 0909  Number):........
-00066df0: 6178 203d 2044 4143 2e6c 6f63 5b3a 6f2e  ax = DAC.loc[:o.
-00066e00: 7363 6174 7465 7263 7574 5b30 5d2c 203a  scattercut[0], :
-00066e10: 5d2e 706c 6f74 2873 7562 706c 6f74 733d  ].plot(subplots=
-00066e20: 7365 7061 7261 7465 5f70 6c6f 7473 2c61  separate_plots,a
-00066e30: 783d 6178 2c6c 6567 656e 643d 4661 6c73  x=ax,legend=Fals
-00066e40: 652c 636f 6c6f 723d 636f 6c6f 7273 5b28  e,color=colors[(
-00066e50: 692b 3129 2a6c 656e 2873 7065 6369 6573  i+1)*len(species
-00066e60: 293a 2869 2b32 292a 6c65 6e28 7370 6563  ):(i+2)*len(spec
-00066e70: 6965 7329 5d29 0d0a 0909 0909 0909 4441  ies)])........DA
-00066e80: 432e 6c6f 635b 6f2e 7363 6174 7465 7263  C.loc[o.scatterc
-00066e90: 7574 5b31 5d3a 2c20 3a5d 2e70 6c6f 7428  ut[1]:, :].plot(
-00066ea0: 7375 6270 6c6f 7473 3d73 6570 6172 6174  subplots=separat
-00066eb0: 655f 706c 6f74 732c 6178 3d61 782c 6c65  e_plots,ax=ax,le
-00066ec0: 6765 6e64 3d46 616c 7365 2c63 6f6c 6f72  gend=False,color
-00066ed0: 3d63 6f6c 6f72 735b 2869 2b31 292a 6c65  =colors[(i+1)*le
-00066ee0: 6e28 7370 6563 6965 7329 3a28 692b 3229  n(species):(i+2)
-00066ef0: 2a6c 656e 2873 7065 6369 6573 295d 290d  *len(species)]).
-00066f00: 0a09 0909 0909 656c 7365 3a0d 0a09 0909  ......else:.....
-00066f10: 0909 0973 6361 7474 6572 6375 7420 3d20  ...scattercut = 
-00066f20: 666c 6174 7465 6e28 6f2e 7363 6174 7465  flatten(o.scatte
-00066f30: 7263 7574 290d 0a09 0909 0909 0966 6f72  rcut)........for
-00066f40: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
-00066f50: 7363 6174 7465 7263 7574 292f 322b 3129  scattercut)/2+1)
-00066f60: 3a0d 0a09 0909 0909 0909 6966 2069 203d  :.........if i =
-00066f70: 3d20 303a 0d0a 0909 0909 0909 0909 6178  = 0:..........ax
-00066f80: 203d 2044 4143 2e6c 6f63 5b3a 7363 6174   = DAC.loc[:scat
-00066f90: 7465 7263 7574 5b30 5d2c 203a 5d2e 706c  tercut[0], :].pl
-00066fa0: 6f74 2873 7562 706c 6f74 733d 7365 7061  ot(subplots=sepa
-00066fb0: 7261 7465 5f70 6c6f 7473 2c61 783d 6178  rate_plots,ax=ax
-00066fc0: 2c6c 6567 656e 643d 4661 6c73 652c 636f  ,legend=False,co
-00066fd0: 6c6f 723d 636f 6c6f 7273 5b28 692b 3129  lor=colors[(i+1)
-00066fe0: 2a6c 656e 2873 7065 6369 6573 293a 2869  *len(species):(i
-00066ff0: 2b32 292a 6c65 6e28 7370 6563 6965 7329  +2)*len(species)
-00067000: 5d29 0d0a 0909 0909 0909 0965 6c69 6620  ]).........elif 
-00067010: 693c 286c 656e 2873 6361 7474 6572 6375  i<(len(scattercu
-00067020: 7429 2f32 293a 0d0a 0909 0909 0909 0909  t)/2):..........
-00067030: 6178 203d 2044 4143 2e6c 6f63 5b73 6361  ax = DAC.loc[sca
-00067040: 7474 6572 6375 745b 322a 692d 315d 3a73  ttercut[2*i-1]:s
-00067050: 6361 7474 6572 6375 745b 322a 695d 2c20  cattercut[2*i], 
-00067060: 3a5d 2e70 6c6f 7428 7375 6270 6c6f 7473  :].plot(subplots
-00067070: 3d73 6570 6172 6174 655f 706c 6f74 732c  =separate_plots,
-00067080: 6178 3d61 782c 6c65 6765 6e64 3d46 616c  ax=ax,legend=Fal
-00067090: 7365 2c63 6f6c 6f72 3d63 6f6c 6f72 735b  se,color=colors[
-000670a0: 2869 2b31 292a 6c65 6e28 7370 6563 6965  (i+1)*len(specie
-000670b0: 7329 3a28 692b 3229 2a6c 656e 2873 7065  s):(i+2)*len(spe
-000670c0: 6369 6573 295d 290d 0a09 0909 0909 0909  cies)]).........
-000670d0: 656c 7365 3a0d 0a09 0909 0909 0909 0961  else:..........a
-000670e0: 7820 3d20 4441 432e 6c6f 635b 7363 6174  x = DAC.loc[scat
-000670f0: 7465 7263 7574 5b2d 315d 3a2c 203a 5d2e  tercut[-1]:, :].
-00067100: 706c 6f74 2873 7562 706c 6f74 733d 7365  plot(subplots=se
-00067110: 7061 7261 7465 5f70 6c6f 7473 2c61 783d  parate_plots,ax=
-00067120: 6178 2c6c 6567 656e 643d 4661 6c73 652c  ax,legend=False,
-00067130: 636f 6c6f 723d 636f 6c6f 7273 5b28 692b  color=colors[(i+
-00067140: 3129 2a6c 656e 2873 7065 6369 6573 293a  1)*len(species):
-00067150: 2869 2b32 292a 6c65 6e28 7370 6563 6965  (i+2)*len(specie
-00067160: 7329 5d29 0d0a 0909 0909 0961 782e 7365  s)]).......ax.se
-00067170: 745f 786c 6162 656c 2827 5761 7665 6c65  t_xlabel('Wavele
-00067180: 6e67 7468 2069 6e20 6e6d 2729 0909 0909  ngth in nm')....
-00067190: 0d0a 0909 0909 0961 782e 7365 745f 796c  .......ax.set_yl
-000671a0: 6162 656c 2827 5370 6563 7472 616c 2073  abel('Spectral s
-000671b0: 7472 656e 6774 6820 696e 2061 7262 2e20  trength in arb. 
-000671c0: 756e 6974 7327 290d 0a09 0909 0909 6178  units').......ax
-000671d0: 2e6c 6567 656e 6428 666f 6e74 7369 7a65  .legend(fontsize
-000671e0: 3d38 2c66 7261 6d65 6f6e 3d46 616c 7365  =8,frameon=False
-000671f0: 290d 0a09 0969 6620 6e6f 7420 6861 7361  )....if not hasa
-00067200: 7474 7228 6178 2c27 5f5f 6974 6572 5f5f  ttr(ax,'__iter__
-00067210: 2729 3a61 783d 6e70 2e61 7272 6179 285b  '):ax=np.array([
-00067220: 6178 5d29 0d0a 0909 6966 2073 7065 6374  ax])....if spect
-00067230: 7261 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ra is not None:.
-00067240: 0a09 0909 666f 7220 6120 696e 2061 783a  ....for a in ax:
-00067250: 0d0a 0909 0909 7370 6563 7472 612e 706c  ......spectra.pl
-00067260: 6f74 2861 783d 612c 7375 6270 6c6f 7473  ot(ax=a,subplots
-00067270: 3d73 6570 6172 6174 655f 706c 6f74 7329  =separate_plots)
-00067280: 0909 0909 0d0a 0909 6669 673d 2861 782e  ........fig=(ax.
-00067290: 7261 7665 6c28 2929 5b30 5d2e 6669 6775  ravel())[0].figu
-000672a0: 7265 0d0a 0909 6966 2073 6570 6172 6174  re....if separat
-000672b0: 655f 706c 6f74 733a 0d0a 0909 0966 6967  e_plots:.....fig
-000672c0: 2e73 6574 5f73 697a 655f 696e 6368 6573  .set_size_inches
-000672d0: 2831 322c 3130 290d 0a09 0909 6178 6573  (12,10).....axes
-000672e0: 5f6e 756d 6265 723d 6669 672e 6765 745f  _number=fig.get_
-000672f0: 6178 6573 2829 0d0a 0909 096e 616d 6573  axes().....names
-00067300: 3d5b 7365 6c66 2e66 696c 656e 616d 655d  =[self.filename]
-00067310: 0d0a 0909 0969 6620 6f74 6865 7220 6973  .....if other is
-00067320: 206e 6f74 204e 6f6e 653a 0d0a 0909 0909   not None:......
-00067330: 666f 7220 6f20 696e 206f 7468 6572 3a0d  for o in other:.
-00067340: 0a09 0909 0909 6e61 6d65 732e 6170 7065  ......names.appe
-00067350: 6e64 286f 2e66 696c 656e 616d 6529 0d0a  nd(o.filename)..
-00067360: 0909 0966 6f72 2069 2c61 7820 696e 2065  ...for i,ax in e
-00067370: 6e75 6d65 7261 7465 2861 7865 735f 6e75  numerate(axes_nu
-00067380: 6d62 6572 293a 0d0a 0909 0909 7472 793a  mber):......try:
-00067390: 0d0a 0909 0909 096e 616d 6574 656d 703d  .......nametemp=
-000673a0: 5b27 2573 2725 7370 6563 6965 735b 695d  ['%s'%species[i]
-000673b0: 202b 2027 202d 2027 202b 2061 2066 6f72   + ' - ' + a for
-000673c0: 2061 2069 6e20 6e61 6d65 735d 0d0a 0909   a in names]....
-000673d0: 0909 0961 782e 6c65 6765 6e64 2868 616e  ...ax.legend(han
-000673e0: 642c 6e61 6d65 7465 6d70 290d 0a09 0909  d,nametemp).....
-000673f0: 0965 7863 6570 743a 0d0a 0909 0909 0970  .except:.......p
-00067400: 6173 730d 0a09 0965 6c73 653a 0d0a 0909  ass....else:....
-00067410: 0961 783d 6669 672e 6765 745f 6178 6573  .ax=fig.get_axes
-00067420: 2829 5b30 5d0d 0a09 0909 6e61 6d65 733d  ()[0].....names=
-00067430: 5b73 656c 662e 6669 6c65 6e61 6d65 5d0d  [self.filename].
-00067440: 0a09 0909 6966 206f 7468 6572 2069 7320  ....if other is 
-00067450: 6e6f 7420 4e6f 6e65 3a0d 0a09 0909 0966  not None:......f
-00067460: 6f72 206f 2069 6e20 6f74 6865 723a 0d0a  or o in other:..
-00067470: 0909 0909 096e 616d 6573 2e61 7070 656e  .....names.appen
-00067480: 6428 6f2e 6669 6c65 6e61 6d65 290d 0a09  d(o.filename)...
-00067490: 0909 6861 6e64 6c65 732c 6c61 6265 6c73  ..handles,labels
-000674a0: 3d61 782e 6765 745f 6c65 6765 6e64 5f68  =ax.get_legend_h
-000674b0: 616e 646c 6573 5f6c 6162 656c 7328 290d  andles_labels().
-000674c0: 0a09 0909 6e61 6d65 7465 6d70 3d5b 5d0d  ....nametemp=[].
-000674d0: 0a09 0909 7472 793a 0d0a 0909 0909 666f  ....try:......fo
-000674e0: 7220 6120 696e 206e 616d 6573 3a0d 0a09  r a in names:...
-000674f0: 0909 0909 666f 7220 6220 696e 2073 7065  ....for b in spe
-00067500: 6369 6573 3a0d 0a09 0909 0909 096e 616d  cies:........nam
-00067510: 6574 656d 702e 6170 7065 6e64 2827 2573  etemp.append('%s
-00067520: 2725 6220 2b20 2720 2d20 2720 2b20 6129  '%b + ' - ' + a)
-00067530: 0d0a 0909 0909 6178 2e6c 6567 656e 6428  ......ax.legend(
-00067540: 6861 6e64 6c65 732c 6e61 6d65 7465 6d70  handles,nametemp
-00067550: 290d 0a09 0909 6578 6365 7074 3a0d 0a09  ).....except:...
-00067560: 0909 0970 6173 730d 0a09 0909 6669 672e  ...pass.....fig.
-00067570: 7365 745f 7369 7a65 5f69 6e63 6865 7328  set_size_inches(
-00067580: 3136 2c38 290d 0a09 0966 6967 2e74 6967  16,8)....fig.tig
-00067590: 6874 5f6c 6179 6f75 7428 290d 0a09 0969  ht_layout()....i
-000675a0: 6620 7365 6c66 2e73 6176 655f 6669 6775  f self.save_figu
-000675b0: 7265 735f 746f 5f66 6f6c 6465 723a 0d0a  res_to_folder:..
-000675c0: 0909 0966 6967 2e73 6176 6566 6967 2863  ...fig.savefig(c
-000675d0: 6865 636b 5f66 6f6c 6465 7228 7061 7468  heck_folder(path
-000675e0: 3d73 656c 662e 6669 6775 7265 5f70 6174  =self.figure_pat
-000675f0: 682c 6669 6c65 6e61 6d65 3d27 636f 6d70  h,filename='comp
-00067600: 6172 655f 4441 432e 706e 6727 292c 6262  are_DAC.png'),bb
-00067610: 6f78 5f69 6e63 6865 733d 2774 6967 6874  ox_inches='tight
-00067620: 2729 0d0a 0d0a 0d0a 0d0a                 ')........
+0005ebc0: 696d 655d 0d0a 0909 0968 616e 3d68 616e  ime].....han=han
+0005ebd0: 646c 6573 5b3a 6c65 6e28 7265 6c5f 7469  dles[:len(rel_ti
+0005ebe0: 6d65 292a 325d 0d0a 0909 0966 6f72 2065  me)*2].....for e
+0005ebf0: 6e74 2069 6e20 7265 6c5f 7469 6d65 3a0d  nt in rel_time:.
+0005ec00: 0a09 0909 096c 6162 2e61 7070 656e 6428  .....lab.append(
+0005ec10: 2725 6720 2573 2066 6974 2725 2865 6e74  '%g %s fit'%(ent
+0005ec20: 2c73 656c 662e 6261 7365 756e 6974 2920  ,self.baseunit) 
+0005ec30: 2b20 275f 2720 2b20 7374 7228 7365 6c66  + '_' + str(self
+0005ec40: 2e66 696c 656e 616d 6529 290d 0a09 0909  .filename)).....
+0005ec50: 6966 206f 7468 6572 2069 7320 6e6f 7420  if other is not 
+0005ec60: 4e6f 6e65 3a0d 0a09 0909 0966 6f72 2069  None:......for i
+0005ec70: 2c6f 2069 6e20 656e 756d 6572 6174 6528  ,o in enumerate(
+0005ec80: 6f74 6865 7229 3a0d 0a09 0909 0909 7472  other):.......tr
+0005ec90: 793a 0d0a 0909 0909 0909 7265 3d6f 2e72  y:........re=o.r
+0005eca0: 650d 0a09 0909 0909 6578 6365 7074 3a0d  e.......except:.
+0005ecb0: 0a09 0909 0909 0970 7269 6e74 2827 2573  .......print('%s
+0005ecc0: 2068 6173 206e 6f20 6669 7474 6564 2072   has no fitted r
+0005ecd0: 6573 756c 7473 2725 6f2e 6669 6c65 6e61  esults'%o.filena
+0005ece0: 6d65 290d 0a09 0909 0909 0963 6f6e 7469  me)........conti
+0005ecf0: 6e75 650d 0a09 0909 0909 6966 206e 6f72  nue.......if nor
+0005ed00: 6d5f 7769 6e64 6f77 2069 7320 6e6f 7420  m_window is not 
+0005ed10: 4e6f 6e65 3a0d 0a09 0909 0909 0972 656c  None:........rel
+0005ed20: 5f73 6361 6c65 3d72 655b 2741 275d 2e6c  _scale=re['A'].l
+0005ed30: 6f63 5b6e 6f72 6d5f 7769 6e64 6f77 5b30  oc[norm_window[0
+0005ed40: 5d3a 6e6f 726d 5f77 696e 646f 775b 315d  ]:norm_window[1]
+0005ed50: 2c6e 6f72 6d5f 7769 6e64 6f77 5b32 5d3a  ,norm_window[2]:
+0005ed60: 6e6f 726d 5f77 696e 646f 775b 335d 5d2e  norm_window[3]].
+0005ed70: 6d65 616e 2829 2e6d 6561 6e28 290d 0a09  mean().mean()...
+0005ed80: 0909 0909 0974 7279 3a0d 0a09 0909 0909  .....try:.......
+0005ed90: 0909 7363 616c 696e 673d 2872 656c 5f73  ..scaling=(rel_s
+0005eda0: 6361 6c65 2f72 6566 5f73 6361 6c65 290d  cale/ref_scale).
+0005edb0: 0a09 0909 0909 0909 6178 3d70 6c6f 745f  ........ax=plot_
+0005edc0: 7469 6d65 2872 655b 2741 4327 5d2f 7363  time(re['AC']/sc
+0005edd0: 616c 696e 672c 2063 6d61 7020 3d20 636f  aling, cmap = co
+0005ede0: 6c6f 7273 2c20 6178 203d 2061 782c 2072  lors, ax = ax, r
+0005edf0: 656c 5f74 696d 6520 3d20 7265 6c5f 7469  el_time = rel_ti
+0005ee00: 6d65 2c20 0d0a 0909 0909 0909 0909 0909  me, ............
+0005ee10: 7469 6d65 5f77 6964 7468 5f70 6572 6365  time_width_perce
+0005ee20: 6e74 203d 2074 696d 655f 7769 6474 685f  nt = time_width_
+0005ee30: 7065 7263 656e 742c 2074 6974 6c65 203d  percent, title =
+0005ee40: 2027 272c 206c 696e 6573 5f61 7265 203d   '', lines_are =
+0005ee50: 2027 6669 7474 6564 272c 200d 0a09 0909   'fitted', .....
+0005ee60: 0909 0909 0909 0973 7562 706c 6f74 203d  .......subplot =
+0005ee70: 2054 7275 652c 2063 6f6c 6f72 5f6f 6666   True, color_off
+0005ee80: 7365 7420 3d20 6c65 6e28 7265 6c5f 7469  set = len(rel_ti
+0005ee90: 6d65 292a 2869 2b31 292c 206c 696e 6577  me)*(i+1), linew
+0005eea0: 6964 7468 203d 206c 696e 6577 6964 7468  idth = linewidth
+0005eeb0: 2c20 7363 6174 7465 7263 7574 203d 206f  , scattercut = o
+0005eec0: 2e73 6361 7474 6572 6375 7429 0d0a 0909  .scattercut)....
+0005eed0: 0909 0909 0968 616e 646c 6573 2c20 6c61  .....handles, la
+0005eee0: 6265 6c73 3d61 782e 6765 745f 6c65 6765  bels=ax.get_lege
+0005eef0: 6e64 5f68 616e 646c 6573 5f6c 6162 656c  nd_handles_label
+0005ef00: 7328 290d 0a09 0909 0909 0909 666f 7220  s().........for 
+0005ef10: 656e 7420 696e 2072 656c 5f74 696d 653a  ent in rel_time:
+0005ef20: 0d0a 0909 0909 0909 0909 6c61 622e 6170  ..........lab.ap
+0005ef30: 7065 6e64 2827 2567 2025 7320 6669 7427  pend('%g %s fit'
+0005ef40: 2528 656e 742c 6f2e 6261 7365 756e 6974  %(ent,o.baseunit
+0005ef50: 2920 2b20 275f 2720 2b20 7374 7228 6f2e  ) + '_' + str(o.
+0005ef60: 6669 6c65 6e61 6d65 2929 0d0a 0909 0909  filename))......
+0005ef70: 0909 0966 6f72 2061 2069 6e20 6861 6e64  ...for a in hand
+0005ef80: 6c65 735b 2d6c 656e 2872 656c 5f74 696d  les[-len(rel_tim
+0005ef90: 6529 3a5d 3a0d 0a09 0909 0909 0909 0968  e):]:..........h
+0005efa0: 616e 2e61 7070 656e 6428 6129 0d0a 0909  an.append(a)....
+0005efb0: 0909 0909 090d 0a09 0909 0909 0909 6966  ..............if
+0005efc0: 2064 6174 615f 616e 645f 6669 743a 0d0a   data_and_fit:..
+0005efd0: 0909 0909 0909 0909 6178 3d70 6c6f 745f  ........ax=plot_
+0005efe0: 7469 6d65 2872 655b 2741 275d 2f73 6361  time(re['A']/sca
+0005eff0: 6c69 6e67 2c20 636d 6170 203d 2073 656c  ling, cmap = sel
+0005f000: 662e 636d 6170 2c20 6178 203d 2061 782c  f.cmap, ax = ax,
+0005f010: 2072 656c 5f74 696d 6520 3d20 7265 6c5f   rel_time = rel_
+0005f020: 7469 6d65 2c20 0d0a 0909 0909 0909 0909  time, ..........
+0005f030: 0909 0974 696d 655f 7769 6474 685f 7065  ...time_width_pe
+0005f040: 7263 656e 7420 3d20 7469 6d65 5f77 6964  rcent = time_wid
+0005f050: 7468 5f70 6572 6365 6e74 2c20 7469 746c  th_percent, titl
+0005f060: 6520 3d20 6f2e 6669 6c65 6e61 6d65 2c20  e = o.filename, 
+0005f070: 0d0a 0909 0909 0909 0909 0909 0962 6173  .............bas
+0005f080: 6575 6e69 7420 3d20 7365 6c66 2e62 6173  eunit = self.bas
+0005f090: 6575 6e69 742c 206c 696e 6573 5f61 7265  eunit, lines_are
+0005f0a0: 203d 2027 6461 7461 272c 2073 7562 706c   = 'data', subpl
+0005f0b0: 6f74 203d 2054 7275 652c 200d 0a09 0909  ot = True, .....
+0005f0c0: 0909 0909 0909 0909 636f 6c6f 725f 6f66  ........color_of
+0005f0d0: 6673 6574 203d 206c 656e 2872 656c 5f74  fset = len(rel_t
+0005f0e0: 696d 6529 2a28 692b 3129 2c20 6c69 6e65  ime)*(i+1), line
+0005f0f0: 7769 6474 6820 3d20 6c69 6e65 7769 6474  width = linewidt
+0005f100: 682c 2073 6361 7474 6572 6375 7420 3d20  h, scattercut = 
+0005f110: 6f2e 7363 6174 7465 7263 7574 290d 0a09  o.scattercut)...
+0005f120: 0909 0909 0909 0968 616e 646c 6573 2c20  .......handles, 
+0005f130: 6c61 6265 6c73 3d61 782e 6765 745f 6c65  labels=ax.get_le
+0005f140: 6765 6e64 5f68 616e 646c 6573 5f6c 6162  gend_handles_lab
+0005f150: 656c 7328 290d 0a09 0909 0909 0909 0966  els()..........f
+0005f160: 6f72 2065 6e74 2069 6e20 7265 6c5f 7469  or ent in rel_ti
+0005f170: 6d65 3a0d 0a09 0909 0909 0909 0909 6c61  me:...........la
+0005f180: 622e 6170 7065 6e64 2827 2567 2025 7327  b.append('%g %s'
+0005f190: 2528 656e 742c 6f2e 6261 7365 756e 6974  %(ent,o.baseunit
+0005f1a0: 2920 2b20 275f 2720 2b20 7374 7228 6f2e  ) + '_' + str(o.
+0005f1b0: 6669 6c65 6e61 6d65 2929 0d0a 0909 0909  filename))......
+0005f1c0: 0909 0909 666f 7220 6120 696e 2068 616e  ....for a in han
+0005f1d0: 646c 6573 5b2d 6c65 6e28 7265 6c5f 7469  dles[-len(rel_ti
+0005f1e0: 6d65 293a 5d3a 0d0a 0909 0909 0909 0909  me):]:..........
+0005f1f0: 0968 616e 2e61 7070 656e 6428 6129 0d0a  .han.append(a)..
+0005f200: 0909 0909 0909 096e 6f72 6d5f 6661 696c  .......norm_fail
+0005f210: 6564 203d 2046 616c 7365 0d0a 0909 0909  ed = False......
+0005f220: 0909 6578 6365 7074 3a0d 0a09 0909 0909  ..except:.......
+0005f230: 0909 7072 696e 7428 2773 6361 6c69 6e67  ..print('scaling
+0005f240: 2046 6169 6c65 6421 2729 0d0a 0909 0909   Failed!')......
+0005f250: 0909 096e 6f72 6d5f 6661 696c 6564 203d  ...norm_failed =
+0005f260: 2054 7275 650d 0a09 0909 0909 656c 7365   True.......else
+0005f270: 3a20 6e6f 726d 5f66 6169 6c65 643d 5472  : norm_failed=Tr
+0005f280: 7565 090d 0a09 0909 0909 6966 206e 6f72  ue........if nor
+0005f290: 6d5f 6661 696c 6564 3a0d 0a09 0909 0909  m_failed:.......
+0005f2a0: 0961 783d 706c 6f74 5f74 696d 6528 7265  .ax=plot_time(re
+0005f2b0: 5b27 4143 275d 2c20 636d 6170 203d 2063  ['AC'], cmap = c
+0005f2c0: 6f6c 6f72 732c 2061 7820 3d20 6178 2c20  olors, ax = ax, 
+0005f2d0: 7265 6c5f 7469 6d65 203d 2072 656c 5f74  rel_time = rel_t
+0005f2e0: 696d 652c 200d 0a09 0909 0909 0909 0909  ime, ...........
+0005f2f0: 0974 696d 655f 7769 6474 685f 7065 7263  .time_width_perc
+0005f300: 656e 7420 3d20 7469 6d65 5f77 6964 7468  ent = time_width
+0005f310: 5f70 6572 6365 6e74 2c20 7469 746c 6520  _percent, title 
+0005f320: 3d20 2727 2c20 6c69 6e65 735f 6172 6520  = '', lines_are 
+0005f330: 3d20 2766 6974 7465 6427 2c20 0d0a 0909  = 'fitted', ....
+0005f340: 0909 0909 0909 0909 7375 6270 6c6f 7420  ........subplot 
+0005f350: 3d20 5472 7565 2c20 636f 6c6f 725f 6f66  = True, color_of
+0005f360: 6673 6574 203d 206c 656e 2872 656c 5f74  fset = len(rel_t
+0005f370: 696d 6529 2a28 692b 3129 2c20 6c69 6e65  ime)*(i+1), line
+0005f380: 7769 6474 6820 3d20 6c69 6e65 7769 6474  width = linewidt
+0005f390: 682c 2073 6361 7474 6572 6375 7420 3d20  h, scattercut = 
+0005f3a0: 6f2e 7363 6174 7465 7263 7574 290d 0a09  o.scattercut)...
+0005f3b0: 0909 0909 0968 616e 646c 6573 2c20 6c61  .....handles, la
+0005f3c0: 6265 6c73 3d61 782e 6765 745f 6c65 6765  bels=ax.get_lege
+0005f3d0: 6e64 5f68 616e 646c 6573 5f6c 6162 656c  nd_handles_label
+0005f3e0: 7328 290d 0a09 0909 0909 0966 6f72 2065  s()........for e
+0005f3f0: 6e74 2069 6e20 7265 6c5f 7469 6d65 3a0d  nt in rel_time:.
+0005f400: 0a09 0909 0909 0909 6c61 622e 6170 7065  ........lab.appe
+0005f410: 6e64 2827 2567 2025 7320 6669 7427 2528  nd('%g %s fit'%(
+0005f420: 656e 742c 6f2e 6261 7365 756e 6974 2920  ent,o.baseunit) 
+0005f430: 2b20 275f 2720 2b20 7374 7228 6f2e 6669  + '_' + str(o.fi
+0005f440: 6c65 6e61 6d65 2929 0d0a 0909 0909 0909  lename))........
+0005f450: 666f 7220 6120 696e 2068 616e 646c 6573  for a in handles
+0005f460: 5b2d 6c65 6e28 7265 6c5f 7469 6d65 293a  [-len(rel_time):
+0005f470: 5d3a 0d0a 0909 0909 0909 0968 616e 2e61  ]:.........han.a
+0005f480: 7070 656e 6428 6129 0d0a 0909 0909 0909  ppend(a)........
+0005f490: 0d0a 0909 0909 0909 6966 2064 6174 615f  ........if data_
+0005f4a0: 616e 645f 6669 743a 0d0a 0909 0909 0909  and_fit:........
+0005f4b0: 0961 783d 706c 6f74 5f74 696d 6528 7265  .ax=plot_time(re
+0005f4c0: 5b27 4127 5d2c 2063 6d61 7020 3d20 7365  ['A'], cmap = se
+0005f4d0: 6c66 2e63 6d61 702c 2061 7820 3d20 6178  lf.cmap, ax = ax
+0005f4e0: 2c20 7265 6c5f 7469 6d65 203d 2072 656c  , rel_time = rel
+0005f4f0: 5f74 696d 652c 200d 0a09 0909 0909 0909  _time, .........
+0005f500: 0909 0974 696d 655f 7769 6474 685f 7065  ...time_width_pe
+0005f510: 7263 656e 7420 3d20 7469 6d65 5f77 6964  rcent = time_wid
+0005f520: 7468 5f70 6572 6365 6e74 2c20 7469 746c  th_percent, titl
+0005f530: 6520 3d20 6f2e 6669 6c65 6e61 6d65 2c20  e = o.filename, 
+0005f540: 0d0a 0909 0909 0909 0909 0909 6261 7365  ............base
+0005f550: 756e 6974 203d 2073 656c 662e 6261 7365  unit = self.base
+0005f560: 756e 6974 2c20 6c69 6e65 735f 6172 6520  unit, lines_are 
+0005f570: 3d20 2764 6174 6127 2c20 7375 6270 6c6f  = 'data', subplo
+0005f580: 7420 3d20 5472 7565 2c20 0d0a 0909 0909  t = True, ......
+0005f590: 0909 0909 0909 636f 6c6f 725f 6f66 6673  ......color_offs
+0005f5a0: 6574 203d 206c 656e 2872 656c 5f74 696d  et = len(rel_tim
+0005f5b0: 6529 2a28 692b 3129 2c20 6c69 6e65 7769  e)*(i+1), linewi
+0005f5c0: 6474 6820 3d20 6c69 6e65 7769 6474 682c  dth = linewidth,
+0005f5d0: 2073 6361 7474 6572 6375 7420 3d20 6f2e   scattercut = o.
+0005f5e0: 7363 6174 7465 7263 7574 290d 0a09 0909  scattercut).....
+0005f5f0: 0909 0909 6861 6e64 6c65 732c 206c 6162  ....handles, lab
+0005f600: 656c 733d 6178 2e67 6574 5f6c 6567 656e  els=ax.get_legen
+0005f610: 645f 6861 6e64 6c65 735f 6c61 6265 6c73  d_handles_labels
+0005f620: 2829 0d0a 0909 0909 0909 0966 6f72 2065  ().........for e
+0005f630: 6e74 2069 6e20 7265 6c5f 7469 6d65 3a0d  nt in rel_time:.
+0005f640: 0a09 0909 0909 0909 096c 6162 2e61 7070  .........lab.app
+0005f650: 656e 6428 2725 6720 2573 2725 2865 6e74  end('%g %s'%(ent
+0005f660: 2c6f 2e62 6173 6575 6e69 7429 202b 2027  ,o.baseunit) + '
+0005f670: 5f27 202b 2073 7472 286f 2e66 696c 656e  _' + str(o.filen
+0005f680: 616d 6529 290d 0a09 0909 0909 0909 666f  ame)).........fo
+0005f690: 7220 6120 696e 2068 616e 646c 6573 5b2d  r a in handles[-
+0005f6a0: 6c65 6e28 7265 6c5f 7469 6d65 293a 5d3a  len(rel_time):]:
+0005f6b0: 0d0a 0909 0909 0909 0909 6861 6e2e 6170  ..........han.ap
+0005f6c0: 7065 6e64 2861 290d 0a09 0909 6966 206e  pend(a).....if n
+0005f6d0: 6f74 206e 6f72 6d5f 6661 696c 6564 3a0d  ot norm_failed:.
+0005f6e0: 0a09 0909 0961 782e 7365 745f 7469 746c  .....ax.set_titl
+0005f6f0: 6528 2763 6f6d 7061 7265 206d 6561 7375  e('compare measu
+0005f700: 7265 6420 616e 6420 6669 7474 6564 2064  red and fitted d
+0005f710: 6174 6120 6174 2067 6976 656e 2074 696d  ata at given tim
+0005f720: 6573 5c6e 2073 6361 6c65 6420 746f 2074  es\n scaled to t
+0005f730: 3d25 6720 7073 203a 2025 6720 7073 202c  =%g ps : %g ps ,
+0005f740: 2077 6c3d 2025 6720 6e6d 3a20 2567 206e   wl= %g nm: %g n
+0005f750: 6d27 2528 6e6f 726d 5f77 696e 646f 775b  m'%(norm_window[
+0005f760: 305d 2c6e 6f72 6d5f 7769 6e64 6f77 5b31  0],norm_window[1
+0005f770: 5d2c 6e6f 726d 5f77 696e 646f 775b 325d  ],norm_window[2]
+0005f780: 2c6e 6f72 6d5f 7769 6e64 6f77 5b33 5d29  ,norm_window[3])
+0005f790: 290d 0a09 0909 656c 7365 3a0d 0a09 0909  ).....else:.....
+0005f7a0: 0961 782e 7365 745f 7469 746c 6528 2763  .ax.set_title('c
+0005f7b0: 6f6d 7061 7265 206d 6561 7375 7265 6420  ompare measured 
+0005f7c0: 616e 6420 6669 7474 6564 2064 6174 6120  and fitted data 
+0005f7d0: 6174 2067 6976 656e 2074 696d 6573 2729  at given times')
+0005f7e0: 0d0a 0909 0961 782e 7365 745f 786c 696d  .....ax.set_xlim
+0005f7f0: 2872 655b 2741 275d 2e63 6f6c 756d 6e73  (re['A'].columns
+0005f800: 2e76 616c 7565 735b 305d 2c72 655b 2741  .values[0],re['A
+0005f810: 275d 2e63 6f6c 756d 6e73 2e76 616c 7565  '].columns.value
+0005f820: 735b 2d31 5d29 0d0a 0909 0961 782e 6c65  s[-1]).....ax.le
+0005f830: 6765 6e64 2868 616e 2c20 6c61 6220 2c6c  gend(han, lab ,l
+0005f840: 6162 656c 7370 6163 696e 6720 3d20 302c  abelspacing = 0,
+0005f850: 206e 636f 6c20 3d20 322c 2063 6f6c 756d   ncol = 2, colum
+0005f860: 6e73 7061 6369 6e67 203d 2031 2c20 6861  nspacing = 1, ha
+0005f870: 6e64 6c65 6c65 6e67 7468 203d 2031 2c20  ndlelength = 1, 
+0005f880: 6672 616d 656f 6e20 3d20 4661 6c73 6529  frameon = False)
+0005f890: 0d0a 0909 656c 7365 3a0d 0a09 0909 6966  ....else:.....if
+0005f8a0: 206e 6f72 6d5f 7769 6e64 6f77 2069 7320   norm_window is 
+0005f8b0: 6e6f 7420 4e6f 6e65 3a0d 0a09 0909 0972  not None:......r
+0005f8c0: 6566 5f73 6361 6c65 3d73 656c 662e 6473  ef_scale=self.ds
+0005f8d0: 2e6c 6f63 5b6e 6f72 6d5f 7769 6e64 6f77  .loc[norm_window
+0005f8e0: 5b30 5d3a 6e6f 726d 5f77 696e 646f 775b  [0]:norm_window[
+0005f8f0: 315d 2c6e 6f72 6d5f 7769 6e64 6f77 5b32  1],norm_window[2
+0005f900: 5d3a 6e6f 726d 5f77 696e 646f 775b 335d  ]:norm_window[3]
+0005f910: 5d2e 6d65 616e 2829 2e6d 6561 6e28 290d  ].mean().mean().
+0005f920: 0a09 0909 6f62 6a65 6374 733d 6c65 6e28  ....objects=len(
+0005f930: 7265 6c5f 7469 6d65 292a 2831 2b6c 656e  rel_time)*(1+len
+0005f940: 286f 7468 6572 2929 0d0a 0909 0963 6f6c  (other)).....col
+0005f950: 6f72 733d 636f 6c6d 2863 6d61 703d 636d  ors=colm(cmap=cm
+0005f960: 6170 2c6b 3d72 616e 6765 286f 626a 6563  ap,k=range(objec
+0005f970: 7473 2929 0d0a 0909 0966 6967 2c61 783d  ts)).....fig,ax=
+0005f980: 706c 742e 7375 6270 6c6f 7473 2866 6967  plt.subplots(fig
+0005f990: 7369 7a65 3d28 3130 2c36 292c 6470 693d  size=(10,6),dpi=
+0005f9a0: 3130 3029 0d0a 0909 095f 3d70 6c6f 745f  100)....._=plot_
+0005f9b0: 7469 6d65 2873 656c 662e 6473 2c20 6178  time(self.ds, ax
+0005f9c0: 203d 2061 782c 2072 656c 5f74 696d 6520   = ax, rel_time 
+0005f9d0: 3d20 7265 6c5f 7469 6d65 2c20 7469 6d65  = rel_time, time
+0005f9e0: 5f77 6964 7468 5f70 6572 6365 6e74 203d  _width_percent =
+0005f9f0: 2074 696d 655f 7769 6474 685f 7065 7263   time_width_perc
+0005fa00: 656e 742c 200d 0a09 0909 0909 0974 6974  ent, ........tit
+0005fa10: 6c65 203d 2074 6974 6c65 2c20 6c69 6e65  le = title, line
+0005fa20: 735f 6172 6520 3d20 2764 6174 6127 2c20  s_are = 'data', 
+0005fa30: 7363 6174 7465 7263 7574 203d 2073 656c  scattercut = sel
+0005fa40: 662e 7363 6174 7465 7263 7574 2c20 626f  f.scattercut, bo
+0005fa50: 7264 6572 6375 7420 3d20 7365 6c66 2e62  rdercut = self.b
+0005fa60: 6f72 6465 7263 7574 2c20 0d0a 0909 0909  ordercut, ......
+0005fa70: 0909 7761 7665 5f6e 6d5f 6269 6e20 3d20  ..wave_nm_bin = 
+0005fa80: 7365 6c66 2e77 6176 655f 6e6d 5f62 696e  self.wave_nm_bin
+0005fa90: 2c20 636d 6170 203d 2063 6f6c 6f72 732c  , cmap = colors,
+0005faa0: 2073 7562 706c 6f74 203d 2054 7275 652c   subplot = True,
+0005fab0: 206c 696e 6577 6964 7468 203d 206c 696e   linewidth = lin
+0005fac0: 6577 6964 7468 2c20 6261 7365 756e 6974  ewidth, baseunit
+0005fad0: 3d73 656c 662e 6261 7365 756e 6974 290d  =self.baseunit).
+0005fae0: 0a09 0909 6966 2031 3a0d 0a09 0909 095f  ....if 1:......_
+0005faf0: 3d70 6c6f 745f 7469 6d65 2873 656c 662e  =plot_time(self.
+0005fb00: 6473 2c20 6178 203d 2061 782c 2072 656c  ds, ax = ax, rel
+0005fb10: 5f74 696d 6520 3d20 7265 6c5f 7469 6d65  _time = rel_time
+0005fb20: 2c20 7469 6d65 5f77 6964 7468 5f70 6572  , time_width_per
+0005fb30: 6365 6e74 203d 2074 696d 655f 7769 6474  cent = time_widt
+0005fb40: 685f 7065 7263 656e 742c 200d 0a09 0909  h_percent, .....
+0005fb50: 0909 0909 7469 746c 6520 3d20 7469 746c  ....title = titl
+0005fb60: 652c 206c 696e 6573 5f61 7265 203d 2027  e, lines_are = '
+0005fb70: 736d 6f6f 7468 6564 272c 2073 6361 7474  smoothed', scatt
+0005fb80: 6572 6375 7420 3d20 7365 6c66 2e73 6361  ercut = self.sca
+0005fb90: 7474 6572 6375 742c 2062 6f72 6465 7263  ttercut, borderc
+0005fba0: 7574 203d 2073 656c 662e 626f 7264 6572  ut = self.border
+0005fbb0: 6375 742c 7761 7665 5f6e 6d5f 6269 6e20  cut,wave_nm_bin 
+0005fbc0: 3d20 7365 6c66 2e77 6176 655f 6e6d 5f62  = self.wave_nm_b
+0005fbd0: 696e 2c20 636d 6170 203d 2063 6f6c 6f72  in, cmap = color
+0005fbe0: 732c 2073 7562 706c 6f74 203d 2046 616c  s, subplot = Fal
+0005fbf0: 7365 2c20 6c69 6e65 7769 6474 6820 3d20  se, linewidth = 
+0005fc00: 6c69 6e65 7769 6474 682c 2062 6173 6575  linewidth, baseu
+0005fc10: 6e69 7420 3d20 7365 6c66 2e62 6173 6575  nit = self.baseu
+0005fc20: 6e69 7429 0d0a 0909 0968 616e 646c 6573  nit).....handles
+0005fc30: 2c20 6c61 6265 6c73 3d61 782e 6765 745f  , labels=ax.get_
+0005fc40: 6c65 6765 6e64 5f68 616e 646c 6573 5f6c  legend_handles_l
+0005fc50: 6162 656c 7328 290d 0a09 0909 6c61 623d  abels().....lab=
+0005fc60: 5b27 2567 2025 7327 2528 656e 742c 7365  ['%g %s'%(ent,se
+0005fc70: 6c66 2e62 6173 6575 6e69 7429 202b 2027  lf.baseunit) + '
+0005fc80: 5f27 202b 2073 7472 2873 656c 662e 6669  _' + str(self.fi
+0005fc90: 6c65 6e61 6d65 2920 666f 7220 656e 7420  lename) for ent 
+0005fca0: 696e 2072 656c 5f74 696d 655d 0d0a 0909  in rel_time]....
+0005fcb0: 0968 616e 3d68 616e 646c 6573 5b3a 6c65  .han=handles[:le
+0005fcc0: 6e28 7265 6c5f 7469 6d65 295d 0d0a 0909  n(rel_time)]....
+0005fcd0: 0969 6620 6f74 6865 7220 6973 206e 6f74  .if other is not
+0005fce0: 204e 6f6e 653a 0d0a 0909 0909 666f 7220   None:......for 
+0005fcf0: 692c 6f20 696e 2065 6e75 6d65 7261 7465  i,o in enumerate
+0005fd00: 286f 7468 6572 293a 0d0a 0909 0909 0969  (other):.......i
+0005fd10: 6620 6e6f 726d 5f77 696e 646f 7720 6973  f norm_window is
+0005fd20: 206e 6f74 204e 6f6e 653a 0d0a 0909 0909   not None:......
+0005fd30: 0909 7265 6c5f 7363 616c 653d 6f2e 6473  ..rel_scale=o.ds
+0005fd40: 2e6c 6f63 5b6e 6f72 6d5f 7769 6e64 6f77  .loc[norm_window
+0005fd50: 5b30 5d3a 6e6f 726d 5f77 696e 646f 775b  [0]:norm_window[
+0005fd60: 315d 2c6e 6f72 6d5f 7769 6e64 6f77 5b32  1],norm_window[2
+0005fd70: 5d3a 6e6f 726d 5f77 696e 646f 775b 335d  ]:norm_window[3]
+0005fd80: 5d2e 6d65 616e 2829 2e6d 6561 6e28 290d  ].mean().mean().
+0005fd90: 0a09 0909 0909 0974 7279 3a0d 0a09 0909  .......try:.....
+0005fda0: 0909 0909 7363 616c 696e 6720 3d20 2872  ....scaling = (r
+0005fdb0: 656c 5f73 6361 6c65 2f72 6566 5f73 6361  el_scale/ref_sca
+0005fdc0: 6c65 290d 0a09 0909 0909 0909 6178 3d70  le).........ax=p
+0005fdd0: 6c6f 745f 7469 6d65 286f 2e64 732f 7363  lot_time(o.ds/sc
+0005fde0: 616c 696e 672c 2063 6d61 7020 3d20 636f  aling, cmap = co
+0005fdf0: 6c6f 7273 2c20 6178 203d 2061 782c 2072  lors, ax = ax, r
+0005fe00: 656c 5f74 696d 6520 3d20 7265 6c5f 7469  el_time = rel_ti
+0005fe10: 6d65 2c20 0d0a 0909 0909 0909 0909 0909  me, ............
+0005fe20: 7469 6d65 5f77 6964 7468 5f70 6572 6365  time_width_perce
+0005fe30: 6e74 203d 2074 696d 655f 7769 6474 685f  nt = time_width_
+0005fe40: 7065 7263 656e 742c 2074 6974 6c65 203d  percent, title =
+0005fe50: 2074 6974 6c65 2c20 6c69 6e65 735f 6172   title, lines_ar
+0005fe60: 6520 3d20 2764 6174 6127 2c20 0d0a 0909  e = 'data', ....
+0005fe70: 0909 0909 0909 0909 7363 6174 7465 7263  ........scatterc
+0005fe80: 7574 203d 206f 2e73 6361 7474 6572 6375  ut = o.scattercu
+0005fe90: 742c 2062 6f72 6465 7263 7574 203d 206f  t, bordercut = o
+0005fea0: 2e62 6f72 6465 7263 7574 2c20 6c69 6e65  .bordercut, line
+0005feb0: 7769 6474 6820 3d20 6c69 6e65 7769 6474  width = linewidt
+0005fec0: 682c 200d 0a09 0909 0909 0909 0909 0977  h, ............w
+0005fed0: 6176 655f 6e6d 5f62 696e 203d 206f 2e77  ave_nm_bin = o.w
+0005fee0: 6176 655f 6e6d 5f62 696e 2c20 7375 6270  ave_nm_bin, subp
+0005fef0: 6c6f 7420 3d20 5472 7565 2c20 636f 6c6f  lot = True, colo
+0005ff00: 725f 6f66 6673 6574 203d 206c 656e 2872  r_offset = len(r
+0005ff10: 656c 5f74 696d 6529 2a28 692b 3129 290d  el_time)*(i+1)).
+0005ff20: 0a09 0909 0909 0909 6861 6e64 6c65 732c  ........handles,
+0005ff30: 206c 6162 656c 733d 6178 2e67 6574 5f6c   labels=ax.get_l
+0005ff40: 6567 656e 645f 6861 6e64 6c65 735f 6c61  egend_handles_la
+0005ff50: 6265 6c73 2829 0d0a 0909 0909 0909 0966  bels().........f
+0005ff60: 6f72 2065 6e74 2069 6e20 7265 6c5f 7469  or ent in rel_ti
+0005ff70: 6d65 3a0d 0a09 0909 0909 0909 096c 6162  me:..........lab
+0005ff80: 2e61 7070 656e 6428 2725 6720 2573 2725  .append('%g %s'%
+0005ff90: 2865 6e74 2c6f 2e62 6173 6575 6e69 7429  (ent,o.baseunit)
+0005ffa0: 202b 2027 5f27 202b 2073 7472 286f 2e66   + '_' + str(o.f
+0005ffb0: 696c 656e 616d 6529 290d 0a09 0909 0909  ilename)).......
+0005ffc0: 0909 666f 7220 6120 696e 2068 616e 646c  ..for a in handl
+0005ffd0: 6573 5b2d 6c65 6e28 7265 6c5f 7469 6d65  es[-len(rel_time
+0005ffe0: 293a 5d3a 0d0a 0909 0909 0909 0909 6861  ):]:..........ha
+0005fff0: 6e2e 6170 7065 6e64 2861 290d 0a0d 0a09  n.append(a).....
+00060000: 0909 0909 0909 6966 2064 6174 615f 616e  ......if data_an
+00060010: 645f 6669 743a 0d0a 0909 0909 0909 0909  d_fit:..........
+00060020: 6178 3d70 6c6f 745f 7469 6d65 286f 2e64  ax=plot_time(o.d
+00060030: 732f 7363 616c 696e 672c 2063 6d61 7020  s/scaling, cmap 
+00060040: 3d20 636f 6c6f 7273 2c20 6178 203d 2061  = colors, ax = a
+00060050: 782c 2072 656c 5f74 696d 6520 3d20 7265  x, rel_time = re
+00060060: 6c5f 7469 6d65 2c20 0d0a 0909 0909 0909  l_time, ........
+00060070: 0909 0909 7469 6d65 5f77 6964 7468 5f70  ....time_width_p
+00060080: 6572 6365 6e74 203d 2074 696d 655f 7769  ercent = time_wi
+00060090: 6474 685f 7065 7263 656e 742c 2074 6974  dth_percent, tit
+000600a0: 6c65 203d 2074 6974 6c65 2c20 6c69 6e65  le = title, line
+000600b0: 735f 6172 6520 3d20 2773 6d6f 6f74 6865  s_are = 'smoothe
+000600c0: 6427 2c20 0d0a 0909 0909 0909 0909 0909  d', ............
+000600d0: 7363 6174 7465 7263 7574 203d 206f 2e73  scattercut = o.s
+000600e0: 6361 7474 6572 6375 742c 2062 6f72 6465  cattercut, borde
+000600f0: 7263 7574 203d 206f 2e62 6f72 6465 7263  rcut = o.borderc
+00060100: 7574 2c20 6c69 6e65 7769 6474 6820 3d20  ut, linewidth = 
+00060110: 6c69 6e65 7769 6474 682c 200d 0a09 0909  linewidth, .....
+00060120: 0909 0909 0909 0977 6176 655f 6e6d 5f62  .......wave_nm_b
+00060130: 696e 203d 206f 2e77 6176 655f 6e6d 5f62  in = o.wave_nm_b
+00060140: 696e 2c20 7375 6270 6c6f 7420 3d20 5472  in, subplot = Tr
+00060150: 7565 2c20 636f 6c6f 725f 6f66 6673 6574  ue, color_offset
+00060160: 203d 206c 656e 2872 656c 5f74 696d 6529   = len(rel_time)
+00060170: 2a28 692b 3129 290d 0a09 0909 0909 0909  *(i+1)).........
+00060180: 7363 616c 696e 675f 6661 696c 6564 3d46  scaling_failed=F
+00060190: 616c 7365 0d0a 0909 0909 0909 6578 6365  alse........exce
+000601a0: 7074 3a0d 0a09 0909 0909 0909 7072 696e  pt:.........prin
+000601b0: 7428 2773 6361 6c69 6e67 2046 6169 6c65  t('scaling Faile
+000601c0: 6421 2729 0d0a 0909 0909 0909 0973 6361  d!').........sca
+000601d0: 6c69 6e67 5f66 6169 6c65 643d 5472 7565  ling_failed=True
+000601e0: 0d0a 0909 0909 0965 6c73 653a 0d0a 0909  .......else:....
+000601f0: 0909 0909 7363 616c 696e 675f 6661 696c  ....scaling_fail
+00060200: 6564 3d54 7275 650d 0a09 0909 0909 6966  ed=True.......if
+00060210: 2073 6361 6c69 6e67 5f66 6169 6c65 643a   scaling_failed:
+00060220: 0d0a 0909 0909 0909 6178 3d70 6c6f 745f  ........ax=plot_
+00060230: 7469 6d65 286f 2e64 732c 2063 6d61 7020  time(o.ds, cmap 
+00060240: 3d20 636f 6c6f 7273 2c20 6178 203d 2061  = colors, ax = a
+00060250: 782c 2072 656c 5f74 696d 6520 3d20 7265  x, rel_time = re
+00060260: 6c5f 7469 6d65 2c20 0d0a 0909 0909 0909  l_time, ........
+00060270: 0909 0974 696d 655f 7769 6474 685f 7065  ...time_width_pe
+00060280: 7263 656e 7420 3d20 7469 6d65 5f77 6964  rcent = time_wid
+00060290: 7468 5f70 6572 6365 6e74 2c20 7469 746c  th_percent, titl
+000602a0: 6520 3d20 7469 746c 652c 206c 696e 6573  e = title, lines
+000602b0: 5f61 7265 203d 2027 6461 7461 272c 200d  _are = 'data', .
+000602c0: 0a09 0909 0909 0909 0909 7363 6174 7465  ..........scatte
+000602d0: 7263 7574 203d 206f 2e73 6361 7474 6572  rcut = o.scatter
+000602e0: 6375 742c 2062 6f72 6465 7263 7574 203d  cut, bordercut =
+000602f0: 206f 2e62 6f72 6465 7263 7574 2c20 6c69   o.bordercut, li
+00060300: 6e65 7769 6474 6820 3d20 6c69 6e65 7769  newidth = linewi
+00060310: 6474 682c 200d 0a09 0909 0909 0909 0909  dth, ...........
+00060320: 7761 7665 5f6e 6d5f 6269 6e20 3d20 6f2e  wave_nm_bin = o.
+00060330: 7761 7665 5f6e 6d5f 6269 6e2c 2073 7562  wave_nm_bin, sub
+00060340: 706c 6f74 203d 2054 7275 652c 2063 6f6c  plot = True, col
+00060350: 6f72 5f6f 6666 7365 7420 3d20 6c65 6e28  or_offset = len(
+00060360: 7265 6c5f 7469 6d65 292a 2869 2b31 2929  rel_time)*(i+1))
+00060370: 0d0a 0909 0909 0909 6861 6e64 6c65 732c  ........handles,
+00060380: 206c 6162 656c 733d 6178 2e67 6574 5f6c   labels=ax.get_l
+00060390: 6567 656e 645f 6861 6e64 6c65 735f 6c61  egend_handles_la
+000603a0: 6265 6c73 2829 0d0a 0909 0909 0909 666f  bels()........fo
+000603b0: 7220 656e 7420 696e 2072 656c 5f74 696d  r ent in rel_tim
+000603c0: 653a 0d0a 0909 0909 0909 096c 6162 2e61  e:.........lab.a
+000603d0: 7070 656e 6428 2725 6720 2573 2725 2865  ppend('%g %s'%(e
+000603e0: 6e74 2c6f 2e62 6173 6575 6e69 7429 202b  nt,o.baseunit) +
+000603f0: 2027 5f27 202b 2073 7472 286f 2e66 696c   '_' + str(o.fil
+00060400: 656e 616d 6529 290d 0a09 0909 0909 0966  ename))........f
+00060410: 6f72 2061 2069 6e20 6861 6e64 6c65 735b  or a in handles[
+00060420: 2d6c 656e 2872 656c 5f74 696d 6529 3a5d  -len(rel_time):]
+00060430: 3a0d 0a09 0909 0909 0909 6861 6e2e 6170  :.........han.ap
+00060440: 7065 6e64 2861 290d 0a09 0909 0909 0969  pend(a)........i
+00060450: 6620 6461 7461 5f61 6e64 5f66 6974 3a0d  f data_and_fit:.
+00060460: 0a09 0909 0909 0909 6178 3d70 6c6f 745f  ........ax=plot_
+00060470: 7469 6d65 286f 2e64 732c 2063 6d61 7020  time(o.ds, cmap 
+00060480: 3d20 636f 6c6f 7273 2c20 6178 203d 2061  = colors, ax = a
+00060490: 782c 2072 656c 5f74 696d 6520 3d20 7265  x, rel_time = re
+000604a0: 6c5f 7469 6d65 2c20 0d0a 0909 0909 0909  l_time, ........
+000604b0: 0909 0974 696d 655f 7769 6474 685f 7065  ...time_width_pe
+000604c0: 7263 656e 7420 3d20 7469 6d65 5f77 6964  rcent = time_wid
+000604d0: 7468 5f70 6572 6365 6e74 2c20 7469 746c  th_percent, titl
+000604e0: 6520 3d20 7469 746c 652c 206c 696e 6573  e = title, lines
+000604f0: 5f61 7265 203d 2027 736d 6f6f 7468 6564  _are = 'smoothed
+00060500: 272c 200d 0a09 0909 0909 0909 0909 7363  ', ...........sc
+00060510: 6174 7465 7263 7574 203d 206f 2e73 6361  attercut = o.sca
+00060520: 7474 6572 6375 742c 2062 6f72 6465 7263  ttercut, borderc
+00060530: 7574 203d 206f 2e62 6f72 6465 7263 7574  ut = o.bordercut
+00060540: 2c20 6c69 6e65 7769 6474 6820 3d20 6c69  , linewidth = li
+00060550: 6e65 7769 6474 682c 200d 0a09 0909 0909  newidth, .......
+00060560: 0909 0909 7761 7665 5f6e 6d5f 6269 6e20  ....wave_nm_bin 
+00060570: 3d20 6f2e 7761 7665 5f6e 6d5f 6269 6e2c  = o.wave_nm_bin,
+00060580: 2073 7562 706c 6f74 203d 2054 7275 652c   subplot = True,
+00060590: 2063 6f6c 6f72 5f6f 6666 7365 7420 3d20   color_offset = 
+000605a0: 6c65 6e28 7265 6c5f 7469 6d65 292a 2869  len(rel_time)*(i
+000605b0: 2b31 2929 0d0a 0909 0909 0909 0909 090d  +1))............
+000605c0: 0a09 0909 6966 206e 6f74 2073 6361 6c69  ....if not scali
+000605d0: 6e67 5f66 6169 6c65 643a 0d0a 0909 0909  ng_failed:......
+000605e0: 6178 2e73 6574 5f74 6974 6c65 2827 636f  ax.set_title('co
+000605f0: 6d70 6172 6520 6d65 6173 7572 6564 2061  mpare measured a
+00060600: 6e64 2073 6d6f 6f74 6865 6420 6461 7461  nd smoothed data
+00060610: 2061 7420 6769 7665 6e20 7469 6d65 735c   at given times\
+00060620: 6e20 7363 616c 6564 2074 6f20 743d 2567  n scaled to t=%g
+00060630: 2070 7320 3a20 2567 2070 7320 2c20 776c   ps : %g ps , wl
+00060640: 3d20 2567 206e 6d3a 2025 6720 6e6d 2725  = %g nm: %g nm'%
+00060650: 286e 6f72 6d5f 7769 6e64 6f77 5b30 5d2c  (norm_window[0],
+00060660: 6e6f 726d 5f77 696e 646f 775b 315d 2c6e  norm_window[1],n
+00060670: 6f72 6d5f 7769 6e64 6f77 5b32 5d2c 6e6f  orm_window[2],no
+00060680: 726d 5f77 696e 646f 775b 335d 2929 0d0a  rm_window[3]))..
+00060690: 0909 0965 6c73 653a 0d0a 0909 0909 6178  ...else:......ax
+000606a0: 2e73 6574 5f74 6974 6c65 2827 636f 6d70  .set_title('comp
+000606b0: 6172 6520 6d65 6173 7572 6564 2061 6e64  are measured and
+000606c0: 2073 6d6f 6f74 6865 6420 6461 7461 2061   smoothed data a
+000606d0: 7420 6769 7665 6e20 7469 6d65 7327 290d  t given times').
+000606e0: 0a09 0909 6178 2e6c 6567 656e 6428 6861  ....ax.legend(ha
+000606f0: 6e2c 206c 6162 2c20 6c61 6265 6c73 7061  n, lab, labelspa
+00060700: 6369 6e67 203d 2030 2c20 6e63 6f6c 203d  cing = 0, ncol =
+00060710: 2032 2c20 636f 6c75 6d6e 7370 6163 696e   2, columnspacin
+00060720: 6720 3d20 312c 2068 616e 646c 656c 656e  g = 1, handlelen
+00060730: 6774 6820 3d20 312c 2066 7261 6d65 6f6e  gth = 1, frameon
+00060740: 203d 2046 616c 7365 290d 0a09 0909 6966   = False).....if
+00060750: 2073 656c 662e 626f 7264 6572 6375 7420   self.bordercut 
+00060760: 6973 204e 6f6e 653a 0d0a 0909 0909 6178  is None:......ax
+00060770: 2e73 6574 5f78 6c69 6d28 7365 6c66 2e64  .set_xlim(self.d
+00060780: 732e 636f 6c75 6d6e 732e 7661 6c75 6573  s.columns.values
+00060790: 5b30 5d2c 7365 6c66 2e64 732e 636f 6c75  [0],self.ds.colu
+000607a0: 6d6e 732e 7661 6c75 6573 5b2d 315d 290d  mns.values[-1]).
+000607b0: 0a09 0909 656c 7365 3a0d 0a09 0909 0961  ....else:......a
+000607c0: 782e 7365 745f 786c 696d 2873 656c 662e  x.set_xlim(self.
+000607d0: 626f 7264 6572 6375 7429 0d0a 0909 6966  bordercut)....if
+000607e0: 2073 7065 6374 7261 2069 7320 6e6f 7420   spectra is not 
+000607f0: 4e6f 6e65 3a0d 0a09 0909 7370 6563 7472  None:.....spectr
+00060800: 612e 706c 6f74 2861 783d 6178 2c6c 6567  a.plot(ax=ax,leg
+00060810: 656e 643d 4661 6c73 6529 0d0a 0909 0968  end=False).....h
+00060820: 616e 646c 6573 2c20 6c61 6265 6c73 3d61  andles, labels=a
+00060830: 782e 6765 745f 6c65 6765 6e64 5f68 616e  x.get_legend_han
+00060840: 646c 6573 5f6c 6162 656c 7328 290d 0a09  dles_labels()...
+00060850: 0909 6861 6e2e 6170 7065 6e64 2868 616e  ..han.append(han
+00060860: 646c 6573 5b2d 315d 290d 0a09 0909 6c61  dles[-1]).....la
+00060870: 622e 6170 7065 6e64 286c 6162 656c 735b  b.append(labels[
+00060880: 2d31 5d29 0d0a 0909 0961 782e 6c65 6765  -1]).....ax.lege
+00060890: 6e64 2868 616e 2c20 6c61 6220 2c6c 6162  nd(han, lab ,lab
+000608a0: 656c 7370 6163 696e 6720 3d20 302c 206e  elspacing = 0, n
+000608b0: 636f 6c20 3d20 322c 2063 6f6c 756d 6e73  col = 2, columns
+000608c0: 7061 6369 6e67 203d 2031 2c20 6861 6e64  pacing = 1, hand
+000608d0: 6c65 6c65 6e67 7468 203d 2031 2c20 6672  lelength = 1, fr
+000608e0: 616d 656f 6e20 3d20 4661 6c73 6529 0d0a  ameon = False)..
+000608f0: 0909 6966 2070 6c6f 745f 7365 636f 6e64  ..if plot_second
+00060900: 5f61 735f 656e 6572 6779 3a0d 0a09 0909  _as_energy:.....
+00060910: 6178 323d 6178 2e74 7769 6e79 2829 0d0a  ax2=ax.twiny()..
+00060920: 0909 0961 7832 2e73 6574 5f78 6c69 6d28  ...ax2.set_xlim(
+00060930: 6178 2e67 6574 5f78 6c69 6d28 2929 0d0a  ax.get_xlim())..
+00060940: 0909 0961 7832 2e73 6574 5f78 7469 636b  ...ax2.set_xtick
+00060950: 7328 6178 2e67 6574 5f78 7469 636b 7328  s(ax.get_xticks(
+00060960: 2929 0d0a 0909 096c 6162 656c 733d 5b27  )).....labels=['
+00060970: 252e 3266 2725 2873 6369 7079 2e63 6f6e  %.2f'%(scipy.con
+00060980: 7374 616e 7473 2e68 2a73 6369 7079 2e63  stants.h*scipy.c
+00060990: 6f6e 7374 616e 7473 2e63 2f28 612a 3165  onstants.c/(a*1e
+000609a0: 2d39 2a73 6369 7079 2e63 6f6e 7374 616e  -9*scipy.constan
+000609b0: 7473 2e65 6c65 6374 726f 6e5f 766f 6c74  ts.electron_volt
+000609c0: 2929 2066 6f72 2061 2069 6e20 6178 322e  )) for a in ax2.
+000609d0: 6765 745f 7874 6963 6b73 2829 5d0d 0a09  get_xticks()]...
+000609e0: 0909 5f3d 6178 322e 7365 745f 7874 6963  .._=ax2.set_xtic
+000609f0: 6b6c 6162 656c 7328 6c61 6265 6c73 290d  klabels(labels).
+00060a00: 0a09 0909 5f3d 6178 322e 7365 745f 786c  ...._=ax2.set_xl
+00060a10: 6162 656c 2827 456e 6572 6779 2069 6e20  abel('Energy in 
+00060a20: 6556 2729 0d0a 0909 0961 782e 7365 745f  eV').....ax.set_
+00060a30: 7a6f 7264 6572 2861 7832 2e67 6574 5f7a  zorder(ax2.get_z
+00060a40: 6f72 6465 7228 292b 3129 0d0a 0909 6669  order()+1)....fi
+00060a50: 673d 706c 742e 6763 6628 290d 0a09 0966  g=plt.gcf()....f
+00060a60: 6967 2e74 6967 6874 5f6c 6179 6f75 7428  ig.tight_layout(
+00060a70: 290d 0a09 0969 6620 7365 6c66 2e73 6176  )....if self.sav
+00060a80: 655f 6669 6775 7265 735f 746f 5f66 6f6c  e_figures_to_fol
+00060a90: 6465 723a 0d0a 0909 0966 6967 2e73 6176  der:.....fig.sav
+00060aa0: 6566 6967 2863 6865 636b 5f66 6f6c 6465  efig(check_folde
+00060ab0: 7228 7061 7468 3d73 656c 662e 6669 6775  r(path=self.figu
+00060ac0: 7265 5f70 6174 682c 6669 6c65 6e61 6d65  re_path,filename
+00060ad0: 3d27 636f 6d70 6172 655f 6174 5f74 696d  ='compare_at_tim
+00060ae0: 655f 2573 2e70 6e67 2725 275f 272e 6a6f  e_%s.png'%'_'.jo
+00060af0: 696e 285b 2725 6727 2561 2066 6f72 2061  in(['%g'%a for a
+00060b00: 2069 6e20 7265 6c5f 7469 6d65 5d29 292c   in rel_time])),
+00060b10: 6262 6f78 5f69 6e63 6865 733d 2774 6967  bbox_inches='tig
+00060b20: 6874 2729 0d0a 0909 0909 0909 2020 0d0a  ht')........  ..
+00060b30: 0d0a 0964 6566 2043 6f6d 7061 7265 5f61  ...def Compare_a
+00060b40: 745f 7761 7665 2873 656c 662c 2072 656c  t_wave(self, rel
+00060b50: 5f77 6176 6520 3d20 4e6f 6e65 2c20 6f74  _wave = None, ot
+00060b60: 6865 7220 3d20 4e6f 6e65 2c20 6669 7474  her = None, fitt
+00060b70: 6564 203d 2046 616c 7365 2c20 6e6f 726d  ed = False, norm
+00060b80: 5f77 696e 646f 7720 3d20 4e6f 6e65 2c0d  _window = None,.
+00060b90: 0a09 0909 0909 0977 6964 7468 203d 204e  .......width = N
+00060ba0: 6f6e 652c 2063 6d61 7020 3d20 4e6f 6e65  one, cmap = None
+00060bb0: 2c20 6461 7461 5f61 6e64 5f66 6974 203d  , data_and_fit =
+00060bc0: 2046 616c 7365 2c20 7363 616c 655f 7479   False, scale_ty
+00060bd0: 7065 203d 2027 7379 6d6c 6f67 272c 206c  pe = 'symlog', l
+00060be0: 696e 6577 6964 7468 203d 2031 293a 0d0a  inewidth = 1):..
+00060bf0: 0909 2727 2754 6869 7320 6675 6e63 7469  ..'''This functi
+00060c00: 6f6e 2070 6c6f 7473 206d 756c 7469 706c  on plots multipl
+00060c10: 6520 6b69 6e65 7469 6373 2069 6e74 6f20  e kinetics into 
+00060c20: 7468 6520 7361 6d65 2066 6967 7572 6520  the same figure 
+00060c30: 6174 206f 6e65 206f 720d 0a09 096d 756c  at one or....mul
+00060c40: 7469 706c 6520 6769 7665 6e20 7761 7665  tiple given wave
+00060c50: 6c65 6e67 7468 2028 7265 6c5f 7761 7665  length (rel_wave
+00060c60: 2920 616e 6420 2061 6c6c 6f77 7320 666f  ) and  allows fo
+00060c70: 7220 0d0a 0909 3a72 6566 3a60 4e6f 726d  r ....:ref:`Norm
+00060c80: 616c 697a 6174 696f 6e20 616e 6420 5363  alization and Sc
+00060c90: 616c 696e 6760 2056 6572 7920 7573 6566  aling` Very usef
+00060ca0: 756c 2074 6f20 636f 6d70 6172 6520 7468  ul to compare th
+00060cb0: 6520 0d0a 0909 6b69 6e65 7469 6373 2066  e ....kinetics f
+00060cc0: 6f72 2064 6966 6665 7265 6e74 2071 7565  or different que
+00060cd0: 6e63 6865 7220 636f 6e63 656e 7472 6174  ncher concentrat
+00060ce0: 696f 6e73 206f 7220 7075 6d70 2070 6f77  ions or pump pow
+00060cf0: 6572 732c 200d 0a09 096f 7220 652e 672e  ers, ....or e.g.
+00060d00: 2064 6966 6665 7265 6e74 2066 6974 732e   different fits.
+00060d10: 2054 6865 2070 6172 616d 6574 6572 2077   The parameter w
+00060d20: 6964 7468 206f 7220 7468 6520 6765 6e65  idth or the gene
+00060d30: 7261 6c20 7365 6c66 2e77 6176 656c 656e  ral self.wavelen
+00060d40: 6774 685f 6269 6e0d 0a09 0977 6869 6368  gth_bin....which
+00060d50: 2069 7320 7573 6564 2069 6620 7769 6474   is used if widt
+00060d60: 6820 6973 204e 6f6e 6520 2844 6566 6175  h is None (Defau
+00060d70: 6c74 2920 6465 6669 6e65 7320 7468 6520  lt) defines the 
+00060d80: 7769 6474 6820 6f66 0d0a 0909 7468 6520  width of....the 
+00060d90: 7370 6563 7472 616c 2077 696e 646f 7720  spectral window 
+00060da0: 7468 6174 2069 7320 696e 7465 6772 6174  that is integrat
+00060db0: 6564 2061 6e64 2073 686f 776e 2e0d 0a0d  ed and shown....
+00060dc0: 0a09 0941 206e 6f72 6d61 6c69 7a61 7469  ...A normalizati
+00060dd0: 6f6e 2077 696e 646f 7720 6361 6e20 6265  on window can be
+00060de0: 2067 6976 656e 2061 7420 7768 6963 6820   given at which 
+00060df0: 616c 6c20 7468 6520 706c 6f74 7465 6420  all the plotted 
+00060e00: 6375 7276 6573 2061 7265 206e 6f72 6d61  curves are norma
+00060e10: 6c69 7a65 6420 746f 2e20 0d0a 0909 5468  lized to. ....Th
+00060e20: 6973 2077 696e 646f 7720 646f 6573 206e  is window does n
+00060e30: 6f74 2068 6176 6520 746f 2062 6520 696e  ot have to be in
+00060e40: 2074 6865 2070 6c6f 7474 6564 2072 6567   the plotted reg
+00060e50: 696f 6e2e 2053 6565 203a 7265 663a 604e  ion. See :ref:`N
+00060e60: 6f72 6d61 6c69 7a61 7469 6f6e 2061 6e64  ormalization and
+00060e70: 2053 6361 6c69 6e67 600d 0a09 090d 0a09   Scaling`.......
+00060e80: 0950 6172 616d 6574 6572 730d 0a09 092d  .Parameters....-
+00060e90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a09  -------------...
+00060ea0: 090d 0a09 0972 656c 5f77 6176 6520 3a20  .....rel_wave : 
+00060eb0: 666c 6f61 7420 6f72 206c 6973 742f 7665  float or list/ve
+00060ec0: 6374 6f72 2028 6f66 2066 6c6f 6174 7329  ctor (of floats)
+00060ed0: 0d0a 0909 0953 7065 6369 6679 2074 6865  .....Specify the
+00060ee0: 2077 6176 656c 656e 6774 6820 7768 6572   wavelength wher
+00060ef0: 6520 746f 2070 6c6f 7420 7468 6520 6b69  e to plot the ki
+00060f00: 6e65 7469 6373 2c20 7369 6e67 6c65 2076  netics, single v
+00060f10: 616c 7565 206f 720d 0a09 0909 6c69 7374  alue or.....list
+00060f20: 2f76 6563 746f 7220 6f66 2076 616c 7565  /vector of value
+00060f30: 7320 286f 6e6c 7920 6d61 6e64 6174 6f72  s (only mandator
+00060f40: 7920 656e 7472 7929 2046 6f72 2065 6163  y entry) For eac
+00060f50: 6820 656e 7472 7920 696e 200d 0a09 0909  h entry in .....
+00060f60: 7265 6c5f 7761 7665 2061 206b 696e 6574  rel_wave a kinet
+00060f70: 6963 2069 7320 706c 6f74 7465 642e 2027  ic is plotted. '
+00060f80: 7265 6c5f 7761 7665 2720 616e 6420 2777  rel_wave' and 'w
+00060f90: 6964 7468 2720 0d0a 0909 0928 696e 2074  idth' .....(in t
+00060fa0: 6865 206f 626a 6563 7420 6361 6c6c 6564  he object called
+00060fb0: 2027 7761 7665 6c65 6e67 7468 5f62 696e   'wavelength_bin
+00060fc0: 2720 776f 726b 2074 6f67 6574 6865 7220  ' work together 
+00060fd0: 666f 7220 7468 6520 6372 6561 7469 6f6e  for the creation
+00060fe0: 200d 0a09 0909 6f66 206b 696e 6574 6963   .....of kinetic
+00060ff0: 2070 6c6f 7473 2e20 4174 2065 6163 6820   plots. At each 
+00061000: 7365 6c65 6374 6564 2077 6176 656c 656e  selected wavelen
+00061010: 6774 6820 7468 6520 6461 7461 2062 6574  gth the data bet
+00061020: 7765 656e 200d 0a09 0909 7761 7665 6c65  ween .....wavele
+00061030: 6e67 7468 2b77 6964 7468 2f32 2061 6e64  ngth+width/2 and
+00061040: 2077 6176 656c 656e 6774 682d 7769 6474   wavelength-widt
+00061050: 682f 3220 6973 2061 7665 7261 6765 6420  h/2 is averaged 
+00061060: 0d0a 0909 0966 6f72 2065 6163 6820 7469  .....for each ti
+00061070: 6d65 706f 696e 740d 0a09 0909 0d0a 0909  mepoint.........
+00061080: 6f74 6865 7220 3a20 5441 206f 626a 6563  other : TA objec
+00061090: 7420 6f72 206c 6973 7420 6f66 2074 686f  t or list of tho
+000610a0: 7365 2c20 6f70 7469 6f6e 616c 200d 0a09  se, optional ...
+000610b0: 0909 7368 6f75 6c64 2062 6520 7461 2e70  ..should be ta.p
+000610c0: 6c6f 745f 6675 6e63 206f 626a 6563 7473  lot_func objects
+000610d0: 2028 6c6f 6164 6564 206f 7220 636f 7069   (loaded or copi
+000610e0: 6564 2920 616e 6420 6973 2077 6861 7420  ed) and is what 
+000610f0: 0d0a 0909 0969 7320 706c 6f74 7465 6420  .....is plotted 
+00061100: 6167 6169 6e73 7420 7468 6520 6461 7461  against the data
+00061110: 2075 7365 2061 206c 6973 7420 5b74 6131   use a list [ta1
+00061120: 2c74 6132 2c2e 2e2e 205d 206f 7220 6765  ,ta2,... ] or ge
+00061130: 6e65 7261 7465 2074 6869 730d 0a09 0909  nerate this.....
+00061140: 6c69 7374 2075 7369 6e67 2074 6865 2047  list using the G
+00061150: 7569 2066 756e 6374 696f 6e2e 2053 6565  ui function. See
+00061160: 2073 6563 7469 6f6e 203a 7265 663a 604f   section :ref:`O
+00061170: 7065 6e69 6e67 206d 756c 7469 706c 6520  pening multiple 
+00061180: 6669 6c65 7360 2069 6e20 0d0a 0909 0974  files` in .....t
+00061190: 6865 2064 6f63 756d 656e 7461 7469 6f6e  he documentation
+000611a0: 0d0a 0d0a 0909 6669 7474 6564 203a 2062  ......fitted : b
+000611b0: 6f6f 6c2c 206f 7074 696f 6e61 6c0d 0a09  ool, optional...
+000611c0: 0909 5472 7565 2f46 616c 7365 2028 4465  ..True/False (De
+000611d0: 6661 756c 7429 202d 2075 7365 2066 6974  fault) - use fit
+000611e0: 7465 6420 6461 7461 2069 6e73 7465 6164  ted data instead
+000611f0: 206f 6620 7261 7720 6461 7461 2e20 0d0a   of raw data. ..
+00061200: 0909 0949 6620 5472 7565 2c20 7468 6520  ...If True, the 
+00061210: 6669 7474 6564 2064 6174 6170 6f69 6e74  fitted datapoint
+00061220: 7320 2877 6974 686f 7574 2069 6e74 6572  s (without inter
+00061230: 706f 6c61 7469 6f6e 2920 6172 6520 7573  polation) are us
+00061240: 6564 2e20 0d0a 0909 0954 6869 7320 6973  ed. .....This is
+00061250: 2069 6e74 656e 6465 6420 666f 7220 636f   intended for co
+00061260: 6d70 6172 696e 6720 652e 672e 2064 6966  mparing e.g. dif
+00061270: 6665 7265 6e74 2066 6974 730d 0a0d 0a09  ferent fits.....
+00061280: 096e 6f72 6d5f 7769 6e64 6f77 203a 204e  .norm_window : N
+00061290: 6f6e 6520 6f72 206c 6973 742f 7665 6374  one or list/vect
+000612a0: 6f72 2028 7769 7468 2034 2066 6c6f 6174  or (with 4 float
+000612b0: 7329 2c20 6f70 7469 6f6e 616c 0d0a 0909  s), optional....
+000612c0: 096e 6f72 6d5f 7769 6e64 6f77 2047 6976  .norm_window Giv
+000612d0: 6520 6120 6c69 7374 2f74 7570 656c 2f76  e a list/tupel/v
+000612e0: 6563 746f 7220 7769 7468 2034 2065 6e74  ector with 4 ent
+000612f0: 7269 6573 2069 6e20 7468 6520 6f72 6465  ries in the orde
+00061300: 7220 0d0a 0909 095b 5374 6172 7420 2d20  r .....[Start - 
+00061310: 7469 6d65 2c20 456e 6420 2d20 7469 6d65  time, End - time
+00061320: 2c20 5374 6172 7420 2d20 7761 7665 6c65  , Start - wavele
+00061330: 6e67 7468 2c20 456e 6420 2d20 5761 7665  ngth, End - Wave
+00061340: 6c65 6e67 7468 5d2c 200d 0a09 0909 7365  length], .....se
+00061350: 6520 7365 6374 696f 6e20 3a72 6566 3a60  e section :ref:`
+00061360: 4e6f 726d 616c 697a 6174 696f 6e20 616e  Normalization an
+00061370: 6420 5363 616c 696e 6760 2069 6e20 7468  d Scaling` in th
+00061380: 6520 646f 6375 6d65 6e74 6174 696f 6e2e  e documentation.
+00061390: 0d0a 0909 0949 6620 4e6f 6e65 2028 4465  .....If None (De
+000613a0: 6661 756c 7429 206e 6f20 6e6f 726d 616c  fault) no normal
+000613b0: 697a 6174 696f 6e20 6973 2064 6f6e 652e  ization is done.
+000613c0: 0d0a 0d0a 0909 7769 6474 680d 0a09 0920  ......width.... 
+000613d0: 2020 5370 6563 6966 7920 7468 6520 7769    Specify the wi
+000613e0: 6474 6820 6162 6f76 6520 616e 6420 6265  dth above and be
+000613f0: 6c6f 7720 7468 6520 6769 7665 6e20 7761  low the given wa
+00061400: 7665 6c65 6e67 7468 2074 6861 7420 6973  velength that is
+00061410: 0d0a 0909 2020 2069 6e74 6567 7261 7465  ....   integrate
+00061420: 6420 6173 2077 696e 646f 772e 2049 6620  d as window. If 
+00061430: 6c65 6674 2074 6f20 2844 6566 6175 6c74  left to (Default
+00061440: 2920 224e 6f6e 6522 2074 6865 2076 616c  ) "None" the val
+00061450: 7565 2066 726f 6d20 7461 2069 730d 0a09  ue from ta is...
+00061460: 0920 2020 7573 6564 2e0d 0a0d 0a09 0964  .   used.......d
+00061470: 6174 615f 616e 645f 6669 7420 3a20 626f  ata_and_fit : bo
+00061480: 6f6c 2c20 6f70 7469 6f6e 616c 0d0a 0909  ol, optional....
+00061490: 0954 7275 6520 6f72 2046 616c 7365 2028  .True or False (
+000614a0: 4465 6661 756c 7429 2c20 6368 6f6f 7365  Default), choose
+000614b0: 2069 6620 666f 7220 7468 6520 4669 7474   if for the Fitt
+000614c0: 6564 2070 6c6f 7420 7468 6520 7261 7720  ed plot the raw 
+000614d0: 6461 7461 206f 6620 7468 6520 0d0a 0909  data of the ....
+000614e0: 096f 7468 6572 2070 726f 6a65 6374 7320  .other projects 
+000614f0: 6973 2074 6f20 6265 2070 6c6f 7474 696e  is to be plottin
+00061500: 6720 696e 2061 6464 6974 696f 6e20 746f  g in addition to
+00061510: 2074 6865 2066 6974 7465 6420 6c69 6e65   the fitted line
+00061520: 2e20 466f 7220 4661 6c73 6520 2844 6566  . For False (Def
+00061530: 6175 6c74 290d 0a09 0909 4f6e 6c79 2074  ault).....Only t
+00061540: 6865 2066 6974 2069 7320 706c 6f74 7465  he fit is plotte
+00061550: 642e 0d0a 0909 090d 0a09 096c 696e 6577  d..........linew
+00061560: 6964 7468 203a 2066 6c6f 6174 2c20 6f70  idth : float, op
+00061570: 7469 6f6e 616c 0d0a 0909 096c 696e 6577  tional.....linew
+00061580: 6964 7468 2074 6f20 6265 2075 7365 6420  idth to be used 
+00061590: 666f 7220 706c 6f74 7469 6e67 0d0a 0909  for plotting....
+000615a0: 0909 0d0a 0909 636d 6170 203a 204e 6f6e  ......cmap : Non
+000615b0: 6520 6f72 206d 6174 706c 6f74 6c69 6220  e or matplotlib 
+000615c0: 636f 6c6f 7220 6d61 702c 206f 7074 696f  color map, optio
+000615d0: 6e61 6c0d 0a09 0909 6973 2061 2070 6f77  nal.....is a pow
+000615e0: 6572 6675 6c6c 2076 6172 6961 626c 6520  erfull variable 
+000615f0: 7468 6174 2063 686f 6f73 6573 2074 6865  that chooses the
+00061600: 2063 6f6c 6f75 7220 6d61 7020 6170 706c   colour map appl
+00061610: 6965 6420 666f 7220 616c 6c20 706c 6f74  ied for all plot
+00061620: 732e 2049 6620 7365 7420 746f 200d 0a09  s. If set to ...
+00061630: 0909 4e6f 6e65 2028 4465 6661 756c 7429  ..None (Default)
+00061640: 2074 6865 6e20 7468 6520 7365 6c66 2e63   then the self.c
+00061650: 6d61 7020 6973 2075 7365 642e 0d0a 0909  map is used.....
+00061660: 0941 7320 7374 616e 6461 7264 2049 2075  .As standard I u
+00061670: 7365 2074 6865 2063 6f6c 6f72 206d 6170  se the color map
+00061680: 2022 6a65 7422 2066 726f 6d20 6d61 7470   "jet" from matp
+00061690: 6c6f 746c 6962 2e20 5468 6572 6520 6172  lotlib. There ar
+000616a0: 6520 6120 7661 7269 6574 7920 6f66 2063  e a variety of c
+000616b0: 6f6c 6f72 6d61 7073 200d 0a09 0909 6176  olormaps .....av
+000616c0: 6169 6c61 626c 6520 7468 6174 2061 7265  ailable that are
+000616d0: 2076 6572 7920 7573 6566 756c 6c2e 2042   very usefull. B
+000616e0: 6573 6964 6520 226a 6574 222c 2022 7669  eside "jet", "vi
+000616f0: 7269 6469 7322 2069 7320 6120 676f 6f64  ridis" is a good
+00061700: 2063 686f 6963 6520 6173 2069 7420 6973   choice as it is
+00061710: 2077 656c 6c20 0d0a 0909 0976 6973 6962   well .....visib
+00061720: 6c65 2075 6e64 6572 2072 6564 2d67 7265  le under red-gre
+00061730: 656e 2062 6c69 6e64 6e65 7373 2e20 4f74  en blindness. Ot
+00061740: 6865 7220 7573 6566 756c 206d 6170 7320  her useful maps 
+00061750: 6172 6520 2270 7269 736d 2220 666f 7220  are "prism" for 
+00061760: 6869 6768 2066 6c75 6374 7561 7469 6f6e  high fluctuation
+00061770: 7320 0d0a 0909 096f 7220 6469 7665 7267  s .....or diverg
+00061780: 696e 6720 636f 6c6f 7220 6d61 7073 206c  ing color maps l
+00061790: 696b 6520 2273 6569 736d 6963 222e 200d  ike "seismic". .
+000617a0: 0a09 0909 5365 6520 6874 7470 733a 2f2f  ....See https://
+000617b0: 6d61 7470 6c6f 746c 6962 2e6f 7267 2f33  matplotlib.org/3
+000617c0: 2e31 2e30 2f74 7574 6f72 6961 6c73 2f63  .1.0/tutorials/c
+000617d0: 6f6c 6f72 732f 636f 6c6f 726d 6170 732e  olors/colormaps.
+000617e0: 6874 6d6c 2066 6f72 2061 2063 6f6d 7072  html for a compr
+000617f0: 6568 656e 7369 7665 200d 0a09 0909 7365  ehensive .....se
+00061800: 6c65 6374 696f 6e2e 2049 6e20 7468 6520  lection. In the 
+00061810: 636f 6465 2074 6865 2063 6f6c 6f72 6d61  code the colorma
+00061820: 7073 2061 7265 2069 6d70 6f72 7465 6420  ps are imported 
+00061830: 736f 2069 6620 706c 6f74 5f66 756e 6320  so if plot_func 
+00061840: 6973 2069 6d70 6f72 7465 6420 6173 2070  is imported as p
+00061850: 6620 7468 656e 200d 0a09 0909 7365 6c66  f then .....self
+00061860: 2e63 6d61 703d 7066 2e63 6d2e 7669 7269  .cmap=pf.cm.viri
+00061870: 6469 7320 7365 7473 2076 6972 6964 6973  dis sets viridis
+00061880: 2061 7320 7468 6520 6d61 7020 746f 2075   as the map to u
+00061890: 7365 2e20 496e 7465 726e 616c 6c79 2074  se. Internally t
+000618a0: 6865 2063 6f6c 6f72 7320 6172 6520 6368  he colors are ch
+000618b0: 6f73 656e 200d 0a09 0909 7769 7468 2074  osen .....with t
+000618c0: 6865 2022 636f 6c6d 2220 6675 6e63 7469  he "colm" functi
+000618d0: 6f6e 2e20 5468 6520 3264 2070 6c6f 7473  on. The 2d plots
+000618e0: 2072 6571 7569 7265 2061 2063 6f6e 7469   require a conti
+000618f0: 6e75 6f75 7320 636f 6c6f 7220 6d61 7020  nuous color map 
+00061900: 736f 2069 6620 736f 6d65 7468 696e 6720  so if something 
+00061910: 0d0a 0909 0965 6c73 6520 6973 2067 6976  .....else is giv
+00061920: 6520 3264 2070 6c6f 7473 2061 7265 2073  e 2d plots are s
+00061930: 686f 776e 2061 7574 6f6d 6174 6963 616c  hown automatical
+00061940: 6c79 2077 6974 6820 226a 6574 222e 2046  ly with "jet". F
+00061950: 6f72 2061 6c6c 206f 6620 7468 6520 3164  or all of the 1d
+00061960: 2070 6c6f 7473 2068 6f77 6576 6572 200d   plots however .
+00061970: 0a09 0909 4920 6669 7273 7420 7365 6c65  ....I first sele
+00061980: 6374 2061 206e 756d 6265 7220 6f66 2063  ct a number of c
+00061990: 6f6c 6f72 7320 6265 666f 7265 2065 6163  olors before eac
+000619a0: 6820 706c 6f74 2e20 4966 2063 6d61 7020  h plot. If cmap 
+000619b0: 6973 2061 2063 6f6e 7469 6e6f 7573 206d  is a continous m
+000619c0: 6170 2074 6865 6e20 7468 6573 650d 0a09  ap then these...
+000619d0: 0909 6172 6520 7361 6d70 6c65 6420 6576  ..are sampled ev
+000619e0: 656e 6c79 206f 7665 7220 7468 6520 636f  enly over the co
+000619f0: 6c6f 7572 6d61 702e 204d 616e 7561 6c20  lourmap. Manual 
+00061a00: 6974 6572 6162 6c65 7320 6f66 2063 6f6c  iterables of col
+00061a10: 6f75 7273 200d 0a09 0909 636d 6170 3d5b  ours .....cmap=[
+00061a20: 2831 2c30 2c30 292c 2830 2c31 2c30 292c  (1,0,0),(0,1,0),
+00061a30: 2830 2c30 2c31 292c 2e2e 2e5d 2061 7265  (0,0,1),...] are
+00061a40: 2061 6c73 6f20 6163 6365 7074 6564 2c20   also accepted, 
+00061a50: 6173 2061 7265 2076 6563 746f 7273 206f  as are vectors o
+00061a60: 7220 6461 7461 6672 616d 6573 2074 6861  r dataframes tha
+00061a70: 7420 0d0a 0909 0963 6f6e 7461 696e 2061  t .....contain a
+00061a80: 7320 726f 7773 2074 6865 2063 6f6c 6f72  s rows the color
+00061a90: 732e 2054 6865 7265 206d 7573 7420 6265  s. There must be
+00061aa0: 206f 6620 636f 7572 7365 2073 7566 6669   of course suffi
+00061ab0: 6369 656e 7420 636f 6c6f 7273 2070 7265  cient colors pre
+00061ac0: 7365 6e74 2066 6f72 200d 0a09 0909 7468  sent for .....th
+00061ad0: 6520 6e75 6d62 6572 7320 6f66 206c 696e  e numbers of lin
+00061ae0: 6573 2074 6861 7420 7769 6c6c 2062 6520  es that will be 
+00061af0: 706c 6f74 7465 642e 2053 6f20 4920 7265  plotted. So I re
+00061b00: 636f 6d6d 656e 6420 746f 2070 726f 7669  commend to provi
+00061b10: 6465 2061 7420 6c65 6173 7420 3130 2063  de at least 10 c
+00061b20: 6f6c 6f75 7273 200d 0a09 0909 2865 2e67  olours .....(e.g
+00061b30: 2e7e 796f 7572 2075 6e69 7665 7273 6974  .~your universit
+00061b40: 7920 636f 6c6f 7273 292e 2063 6f6c 6f75  y colors). colou
+00061b50: 7273 2061 7265 2061 6c77 6179 7320 6769  rs are always gi
+00061b60: 7665 6e20 6173 2061 2c20 6c69 7374 206f  ven as a, list o
+00061b70: 7220 7475 706c 6520 7769 7468 2052 4741  r tuple with RGA
+00061b80: 206f 7220 5247 4241 0d0a 0909 0928 7769   or RGBA.....(wi
+00061b90: 7468 2074 6865 206c 6173 7420 4120 6265  th the last A be
+00061ba0: 6569 6e67 2074 6865 2041 6c70 6861 3d74  eing the Alpha=t
+00061bb0: 7261 6e73 7061 7265 6e63 792e 2041 6c6c  ransparency. All
+00061bc0: 206e 756d 6265 7273 2061 7265 2062 6574   numbers are bet
+00061bd0: 7765 656e 2030 2061 6e64 2031 2e20 0d0a  ween 0 and 1. ..
+00061be0: 0909 0949 6620 6120 6c69 7374 2f76 6563  ...If a list/vec
+00061bf0: 746f 722f 4461 7461 4672 616d 6520 6973  tor/DataFrame is
+00061c00: 2067 6976 656e 2066 6f72 2074 6865 2063   given for the c
+00061c10: 6f6c 6f75 7273 2074 6865 7920 7769 6c6c  olours they will
+00061c20: 2062 6520 7573 6564 2069 6e20 7468 6520   be used in the 
+00061c30: 6f72 6465 7220 7072 6f76 6964 6564 2e0d  order provided..
+00061c40: 0a09 090d 0a09 0953 6361 6c65 5f74 7970  .......Scale_typ
+00061c50: 6520 3a20 4e6f 6e65 206f 7220 7374 720d  e : None or str.
+00061c60: 0a09 0909 6973 2061 2067 656e 6572 616c  ....is a general
+00061c70: 2073 6574 7469 6e67 2074 6861 7420 6361   setting that ca
+00061c80: 6e20 696e 666c 7565 6e63 6573 2077 6861  n influences wha
+00061c90: 7420 7469 6d65 2061 7869 7320 7769 6c6c  t time axis will
+00061ca0: 2062 6520 7573 6564 2066 6f72 2074 6865   be used for the
+00061cb0: 2070 6c6f 7473 2e20 0d0a 0909 0922 7379   plots. ....."sy
+00061cc0: 6d6c 6f67 2220 286c 696e 6561 7220 6172  mlog" (linear ar
+00061cd0: 6f75 6e64 207a 6572 6f20 616e 6420 6c6f  ound zero and lo
+00061ce0: 6761 7269 7468 6d69 6320 6f74 6865 7277  garithmic otherw
+00061cf0: 6973 6529 2022 6c69 6e22 2061 6e64 2022  ise) "lin" and "
+00061d00: 6c6f 6722 2061 7265 2076 616c 6964 206f  log" are valid o
+00061d10: 7074 696f 6e73 2e09 0d0a 0909 0909 090d  ptions..........
+00061d20: 0a09 0945 7861 6d70 6c65 730d 0a09 092d  ...Examples....-
+00061d30: 2d2d 2d2d 2d2d 2d0d 0a09 090d 0a09 093e  -------........>
+00061d40: 3e3e 2069 6d70 6f72 7420 706c 6f74 5f66  >> import plot_f
+00061d50: 756e 6320 6173 2070 660d 0a09 093e 3e3e  unc as pf....>>>
+00061d60: 2074 6120 3d20 7066 2e54 4128 2774 6573   ta = pf.TA('tes
+00061d70: 7431 2e68 6466 3527 2920 236f 7065 6e20  t1.hdf5') #open 
+00061d80: 7468 6520 6f72 6967 696e 616c 2070 726f  the original pro
+00061d90: 6a65 6374 0d0a 0909 0d0a 0909 4e6f 7720  ject........Now 
+00061da0: 6f70 656e 2061 2062 756e 6368 206f 6620  open a bunch of 
+00061db0: 6f74 6865 7220 7072 6f6a 6563 7473 2074  other projects t
+00061dc0: 6f20 636f 6d70 6172 6520 6167 6169 6e73  o compare agains
+00061dd0: 740d 0a09 090d 0a09 093e 3e3e 206f 7468  t........>>> oth
+00061de0: 6572 5f70 726f 6a65 6374 7320 3d20 7066  er_projects = pf
+00061df0: 2e47 5549 5f6f 7065 6e28 7072 6f6a 6563  .GUI_open(projec
+00061e00: 745f 6c69 7374 203d 205b 2766 696c 6531  t_list = ['file1
+00061e10: 2e53 4941 272c 2027 6669 6c65 322e 5349  .SIA', 'file2.SI
+00061e20: 4127 5d29 0d0a 0909 0d0a 0909 5479 7069  A'])........Typi
+00061e30: 6361 6c20 7573 653a 0d0a 0909 436f 6d70  cal use:....Comp
+00061e40: 6172 6520 7468 6520 7261 7720 6461 7461  are the raw data
+00061e50: 2077 6974 686f 7574 206e 6f72 6d61 6c69   without normali
+00061e60: 7a61 7469 6f6e 2061 7420 3430 3020 6e6d  zation at 400 nm
+00061e70: 2061 6e64 2035 3030 206e 6d0d 0a09 090d   and 500 nm.....
+00061e80: 0a09 093e 3e3e 2074 612e 436f 6d70 6172  ...>>> ta.Compar
+00061e90: 655f 6174 5f77 6176 6528 7265 6c5f 7761  e_at_wave(rel_wa
+00061ea0: 7665 203d 205b 3430 302c 2035 3030 5d2c  ve = [400, 500],
+00061eb0: 206f 7468 6572 7320 3d20 6f74 6865 725f   others = other_
+00061ec0: 7072 6f6a 6563 7429 0d0a 0909 0d0a 0909  project)........
+00061ed0: 436f 6d70 6172 6520 7468 6520 7175 616c  Compare the qual
+00061ee0: 6974 7920 6f66 2074 6865 2066 6974 2064  ity of the fit d
+00061ef0: 6174 6120 7769 7468 6f75 7420 6e6f 726d  ata without norm
+00061f00: 616c 697a 6174 696f 6e20 6174 2034 3030  alization at 400
+00061f10: 206e 6d20 616e 6420 3530 3020 6e6d 0d0a   nm and 500 nm..
+00061f20: 0909 0d0a 0909 3e3e 3e20 7461 2e43 6f6d  ......>>> ta.Com
+00061f30: 7061 7265 5f61 745f 7761 7665 2872 656c  pare_at_wave(rel
+00061f40: 5f77 6176 6520 3d20 5b34 3030 2c20 3530  _wave = [400, 50
+00061f50: 305d 2c20 6f74 6865 7273 203d 206f 7468  0], others = oth
+00061f60: 6572 5f70 726f 6a65 6374 2c20 6669 7474  er_project, fitt
+00061f70: 6564 203d 2054 7275 6529 0d0a 0909 0d0a  ed = True)......
+00061f80: 0909 436f 6d70 6172 6520 7769 7468 206e  ..Compare with n
+00061f90: 6f72 6d61 6c69 7a61 7469 6f6e 2077 696e  ormalization win
+00061fa0: 646f 7720 6265 7477 6565 6e20 3170 7320  dow between 1ps 
+00061fb0: 616e 6420 3270 7320 616e 6420 3430 306e  and 2ps and 400n
+00061fc0: 6d20 616e 6420 3435 306e 6d0d 0a09 090d  m and 450nm.....
+00061fd0: 0a09 093e 3e3e 206e 6f72 6d5f 7769 6e64  ...>>> norm_wind
+00061fe0: 6f77 3d5b 312c 322c 3430 302c 3435 305d  ow=[1,2,400,450]
+00061ff0: 0d0a 0909 3e3e 3e20 7461 2e43 6f6d 7061  ....>>> ta.Compa
+00062000: 7265 5f61 745f 7761 7665 2872 656c 5f77  re_at_wave(rel_w
+00062010: 6176 6520 3d20 5b34 3030 2c20 3530 305d  ave = [400, 500]
+00062020: 2c20 6f74 6865 7273 203d 206f 7468 6572  , others = other
+00062030: 5f70 726f 6a65 6374 2c20 6e6f 726d 5f77  _project, norm_w
+00062040: 696e 646f 7720 3d20 6e6f 726d 5f77 696e  indow = norm_win
+00062050: 646f 7729 0d0a 0909 0d0a 0909 5573 6520  dow)........Use 
+00062060: 6578 616d 706c 653a 204f 6674 656e 2074  example: Often t
+00062070: 6865 7265 2061 7265 2061 206c 6f74 206f  here are a lot o
+00062080: 6620 6469 6666 6572 656e 7420 6d65 6173  f different meas
+00062090: 7572 656d 656e 7473 2074 6f20 0d0a 0909  urements to ....
+000620a0: 636f 6d70 6172 6520 6174 206d 756c 7469  compare at multi
+000620b0: 706c 6520 7761 7665 6c65 6e67 7468 2e20  ple wavelength. 
+000620c0: 5468 6520 6e6f 726d 6c69 7a61 7469 6f6e  The normlization
+000620d0: 2069 7320 7065 7266 6f72 6d65 6420 6174   is performed at
+000620e0: 2074 6865 2067 726f 756e 6420 7374 6174   the ground stat
+000620f0: 6520 626c 6561 6368 0d0a 0909 3436 3020  e bleach....460 
+00062100: 6e6d 2061 6e64 2065 6172 6c79 2069 6e20  nm and early in 
+00062110: 7469 6d65 2e20 5468 656e 2069 7420 6973  time. Then it is
+00062120: 2062 6574 7465 7220 746f 206d 616b 6520   better to make 
+00062130: 6120 6e65 7720 706c 6f74 2066 6f72 2065  a new plot for e
+00062140: 6163 6820 0d0a 0909 7761 7665 6c65 6e67  ach ....waveleng
+00062150: 7468 2e20 5468 6520 6e6f 726d 616c 697a  th. The normaliz
+00062160: 6174 696f 6e20 7769 6e64 6f77 2073 7461  ation window sta
+00062170: 7973 2066 6978 6564 2e0d 0a09 090d 0a09  ys fixed........
+00062180: 093e 3e3e 2070 6c74 2e63 6c6f 7365 2827  .>>> plt.close('
+00062190: 616c 6c27 2920 236d 616b 6520 736f 6d65  all') #make some
+000621a0: 2073 7061 6365 0d0a 0909 3e3e 3e20 6e6f   space....>>> no
+000621b0: 726d 5f77 696e 646f 773d 5b30 2e33 2c30  rm_window=[0.3,0
+000621c0: 2e35 2c34 3530 2c34 3730 5d20 2364 6566  .5,450,470] #def
+000621d0: 696e 6520 7769 6e64 6f77 2069 6e20 6772  ine window in gr
+000621e0: 6f75 6e64 2073 7461 7465 2062 6c65 6163  ound state bleac
+000621f0: 680d 0a09 093e 3e3e 2066 6f72 2077 6176  h....>>> for wav
+00062200: 6520 696e 205b 3330 302c 3430 302c 3530  e in [300,400,50
+00062210: 302c 3630 302c 3730 305d 3a20 2369 7465  0,600,700]: #ite
+00062220: 7261 7465 206f 7665 7220 7468 6520 7761  rate over the wa
+00062230: 7665 6c65 6e67 7468 200d 0a09 093e 3e3e  velength ....>>>
+00062240: 2009 7461 2e43 6f6d 7061 7265 5f61 745f   .ta.Compare_at_
+00062250: 7761 7665 2872 656c 5f77 6176 6520 3d20  wave(rel_wave = 
+00062260: 7761 7665 2c20 6f74 6865 7273 203d 206f  wave, others = o
+00062270: 7468 6572 5f70 726f 6a65 6374 2c20 6e6f  ther_project, no
+00062280: 726d 5f77 696e 646f 7720 3d20 6e6f 726d  rm_window = norm
+00062290: 5f77 696e 646f 7729 0d0a 0909 0d0a 0909  _window)........
+000622a0: 2727 2709 0d0a 0909 0d0a 0909 6966 2073  '''.........if s
+000622b0: 656c 662e 7361 7665 5f66 6967 7572 6573  elf.save_figures
+000622c0: 5f74 6f5f 666f 6c64 6572 3a73 656c 662e  _to_folder:self.
+000622d0: 6669 6775 7265 5f70 6174 683d 6368 6563  figure_path=chec
+000622e0: 6b5f 666f 6c64 6572 2870 6174 683d 2772  k_folder(path='r
+000622f0: 6573 756c 745f 6669 6775 7265 7327 2c63  esult_figures',c
+00062300: 7572 7265 6e74 5f70 6174 683d 7365 6c66  urrent_path=self
+00062310: 2e70 6174 6829 0d0a 0909 6966 2077 6964  .path)....if wid
+00062320: 7468 2069 7320 4e6f 6e65 3a77 6964 7468  th is None:width
+00062330: 3d73 656c 662e 7761 7665 6c65 6e67 7468  =self.wavelength
+00062340: 5f62 696e 0d0a 0909 6966 2072 656c 5f77  _bin....if rel_w
+00062350: 6176 6520 6973 204e 6f6e 653a 0d0a 0909  ave is None:....
+00062360: 0972 656c 5f77 6176 653d 7365 6c66 2e72  .rel_wave=self.r
+00062370: 656c 5f77 6176 650d 0a09 0969 6620 6f74  el_wave....if ot
+00062380: 6865 7220 6973 206e 6f74 204e 6f6e 653a  her is not None:
+00062390: 0d0a 0909 0969 6620 6e6f 7420 6861 7361  .....if not hasa
+000623a0: 7474 7228 6f74 6865 722c 275f 5f69 7465  ttr(other,'__ite
+000623b0: 725f 5f27 293a 6f74 6865 723d 5b6f 7468  r__'):other=[oth
+000623c0: 6572 5d0d 0a09 0969 6620 6e6f 7420 6861  er]....if not ha
+000623d0: 7361 7474 7228 7265 6c5f 7761 7665 2c27  sattr(rel_wave,'
+000623e0: 5f5f 6974 6572 5f5f 2729 3a0d 0a09 0909  __iter__'):.....
+000623f0: 7265 6c5f 7761 7665 3d5b 7265 6c5f 7761  rel_wave=[rel_wa
+00062400: 7665 5d0d 0a09 0969 6620 636d 6170 2069  ve]....if cmap i
+00062410: 7320 4e6f 6e65 3a63 6d61 703d 7365 6c66  s None:cmap=self
+00062420: 2e63 6d61 700d 0a09 0969 6620 6669 7474  .cmap....if fitt
+00062430: 6564 3a0d 0a09 0909 7472 793a 0d0a 0909  ed:.....try:....
+00062440: 0909 7265 3d73 656c 662e 7265 0d0a 0909  ..re=self.re....
+00062450: 0965 7863 6570 743a 0d0a 0909 0909 7072  .except:......pr
+00062460: 696e 7428 224e 6f20 6669 7474 6564 2072  int("No fitted r
+00062470: 6573 756c 7473 2070 7265 7365 6e74 2229  esults present")
+00062480: 0d0a 0909 0909 7265 7475 726e 2046 616c  ......return Fal
+00062490: 7365 0d0a 0909 0969 6620 6e6f 726d 5f77  se.....if norm_w
+000624a0: 696e 646f 7720 6973 206e 6f74 204e 6f6e  indow is not Non
+000624b0: 653a 0d0a 0909 0909 7265 665f 7363 616c  e:......ref_scal
+000624c0: 6520 3d20 7265 5b27 4127 5d2e 6c6f 635b  e = re['A'].loc[
+000624d0: 6e6f 726d 5f77 696e 646f 775b 305d 3a6e  norm_window[0]:n
+000624e0: 6f72 6d5f 7769 6e64 6f77 5b31 5d2c 206e  orm_window[1], n
+000624f0: 6f72 6d5f 7769 6e64 6f77 5b32 5d3a 6e6f  orm_window[2]:no
+00062500: 726d 5f77 696e 646f 775b 335d 5d2e 6d65  rm_window[3]].me
+00062510: 616e 2829 2e6d 6561 6e28 290d 0a09 0909  an().mean().....
+00062520: 6669 672c 2061 7820 3d20 706c 742e 7375  fig, ax = plt.su
+00062530: 6270 6c6f 7473 2866 6967 7369 7a65 203d  bplots(figsize =
+00062540: 2028 3130 2c20 3629 2c20 6470 6920 3d20   (10, 6), dpi = 
+00062550: 3130 3029 0d0a 0909 0963 6f6c 6f72 7320  100).....colors 
+00062560: 3d20 636f 6c6d 2863 6d61 7020 3d20 636d  = colm(cmap = cm
+00062570: 6170 2c20 6b20 3d20 7261 6e67 6528 6c65  ap, k = range(le
+00062580: 6e28 7265 6c5f 7761 7665 292a 2832 2b6c  n(rel_wave)*(2+l
+00062590: 656e 286f 7468 6572 2929 2929 0d0a 0909  en(other))))....
+000625a0: 0961 7820 3d20 706c 6f74 3164 2872 655b  .ax = plot1d(re[
+000625b0: 2741 275d 2c20 6178 203d 2061 782c 2077  'A'], ax = ax, w
+000625c0: 6176 656c 656e 6774 6820 3d20 7265 6c5f  avelength = rel_
+000625d0: 7761 7665 2c20 7769 6474 6820 3d20 7769  wave, width = wi
+000625e0: 6474 682c 206c 696e 6573 5f61 7265 203d  dth, lines_are =
+000625f0: 2027 6461 7461 272c 200d 0a09 0909 0909   'data', .......
+00062600: 0963 6d61 7020 3d20 636f 6c6f 7273 2c20  .cmap = colors, 
+00062610: 7469 746c 6520 3d20 2727 2c20 706c 6f74  title = '', plot
+00062620: 5f74 7970 6520 3d20 7363 616c 655f 7479  _type = scale_ty
+00062630: 7065 2c20 6c69 6e65 7769 6474 6820 3d20  pe, linewidth = 
+00062640: 6c69 6e65 7769 6474 6829 0d0a 0909 0961  linewidth).....a
+00062650: 7820 3d20 706c 6f74 3164 2872 655b 2741  x = plot1d(re['A
+00062660: 4327 5d2c 2061 7820 3d20 6178 2c20 7761  C'], ax = ax, wa
+00062670: 7665 6c65 6e67 7468 203d 2072 656c 5f77  velength = rel_w
+00062680: 6176 652c 2077 6964 7468 203d 2077 6964  ave, width = wid
+00062690: 7468 2c20 6c69 6e65 735f 6172 6520 3d20  th, lines_are = 
+000626a0: 2766 6974 7465 6427 2c20 0d0a 0909 0909  'fitted', ......
+000626b0: 0909 636d 6170 203d 2063 6f6c 6f72 732c  ..cmap = colors,
+000626c0: 2074 6974 6c65 203d 2027 272c 2073 7562   title = '', sub
+000626d0: 706c 6f74 203d 2054 7275 652c 2070 6c6f  plot = True, plo
+000626e0: 745f 7479 7065 203d 2073 6361 6c65 5f74  t_type = scale_t
+000626f0: 7970 652c 206c 696e 6577 6964 7468 203d  ype, linewidth =
+00062700: 206c 696e 6577 6964 7468 290d 0a09 0909   linewidth).....
+00062710: 2361 7820 3d20 706c 6f74 3164 2872 655b  #ax = plot1d(re[
+00062720: 2741 4327 5d2c 2061 7820 3d20 6178 2c20  'AC'], ax = ax, 
+00062730: 7761 7665 6c65 6e67 7468 203d 2072 656c  wavelength = rel
+00062740: 5f77 6176 652c 2077 6964 7468 203d 2077  _wave, width = w
+00062750: 6964 7468 2c20 6c69 6e65 735f 6172 6520  idth, lines_are 
+00062760: 3d20 2766 6974 7465 6427 2c20 0d0a 0909  = 'fitted', ....
+00062770: 0923 0909 0963 6d61 7020 3d20 636f 6c6f  .#...cmap = colo
+00062780: 7273 2c20 636f 6c6f 725f 6f66 6673 6574  rs, color_offset
+00062790: 203d 206c 656e 2872 656c 5f77 6176 6529   = len(rel_wave)
+000627a0: 2c20 7469 746c 6520 3d20 2727 2c20 7375  , title = '', su
+000627b0: 6270 6c6f 7420 3d20 5472 7565 2c20 706c  bplot = True, pl
+000627c0: 6f74 5f74 7970 6520 3d20 7363 616c 655f  ot_type = scale_
+000627d0: 7479 7065 290d 0a09 0909 6861 6e64 2c20  type).....hand, 
+000627e0: 206c 6162 656c 7320 3d20 6178 2e67 6574   labels = ax.get
+000627f0: 5f6c 6567 656e 645f 6861 6e64 6c65 735f  _legend_handles_
+00062800: 6c61 6265 6c73 2829 0d0a 0909 096c 6162  labels().....lab
+00062810: 3d5b 2725 6720 6e6d 2725 6120 2b20 275f  =['%g nm'%a + '_
+00062820: 2720 2b20 7374 7228 7365 6c66 2e66 696c  ' + str(self.fil
+00062830: 656e 616d 6529 2066 6f72 2061 2069 6e20  ename) for a in 
+00062840: 7265 6c5f 7761 7665 5d0d 0a09 0909 666f  rel_wave].....fo
+00062850: 7220 656e 7420 696e 2072 656c 5f77 6176  r ent in rel_wav
+00062860: 653a 0d0a 0909 0909 6c61 622e 6170 7065  e:......lab.appe
+00062870: 6e64 2827 2567 206e 6d27 2565 6e74 202b  nd('%g nm'%ent +
+00062880: 2027 5f27 202b 2073 7472 2873 656c 662e   '_' + str(self.
+00062890: 6669 6c65 6e61 6d65 2929 0d0a 0909 090d  filename))......
+000628a0: 0a09 0909 6966 206f 7468 6572 2069 7320  ....if other is 
+000628b0: 6e6f 7420 4e6f 6e65 3a0d 0a09 0909 0966  not None:......f
+000628c0: 6f72 2069 2c6f 2069 6e20 656e 756d 6572  or i,o in enumer
+000628d0: 6174 6528 6f74 6865 7229 3a0d 0a09 0909  ate(other):.....
+000628e0: 0909 692b 3d31 0d0a 0909 0909 0963 6f6c  ..i+=1.......col
+000628f0: 6f72 5f6f 6666 7365 743d 2869 2b31 292a  or_offset=(i+1)*
+00062900: 6c65 6e28 7265 6c5f 7761 7665 290d 0a09  len(rel_wave)...
+00062910: 0909 0909 7472 793a 0d0a 0909 0909 0909  ....try:........
+00062920: 7265 3d6f 2e72 650d 0a09 0909 0909 6578  re=o.re.......ex
+00062930: 6365 7074 3a0d 0a09 0909 0909 0970 7269  cept:........pri
+00062940: 6e74 2827 2573 2068 6173 206e 6f20 6669  nt('%s has no fi
+00062950: 7474 6564 2072 6573 756c 7473 2725 6f2e  tted results'%o.
+00062960: 6669 6c65 6e61 6d65 290d 0a09 0909 0909  filename).......
+00062970: 0963 6f6e 7469 6e75 650d 0a09 0909 0909  .continue.......
+00062980: 6966 206e 6f72 6d5f 7769 6e64 6f77 2069  if norm_window i
+00062990: 7320 6e6f 7420 4e6f 6e65 3a0d 0a09 0909  s not None:.....
+000629a0: 0909 0972 656c 5f73 6361 6c65 3d72 655b  ...rel_scale=re[
+000629b0: 2741 275d 2e6c 6f63 5b6e 6f72 6d5f 7769  'A'].loc[norm_wi
+000629c0: 6e64 6f77 5b30 5d3a 6e6f 726d 5f77 696e  ndow[0]:norm_win
+000629d0: 646f 775b 315d 2c6e 6f72 6d5f 7769 6e64  dow[1],norm_wind
+000629e0: 6f77 5b32 5d3a 6e6f 726d 5f77 696e 646f  ow[2]:norm_windo
+000629f0: 775b 335d 5d2e 6d65 616e 2829 2e6d 6561  w[3]].mean().mea
+00062a00: 6e28 290d 0a09 0909 0909 0909 0909 0909  n().............
+00062a10: 0909 200d 0a09 0909 0909 0974 7279 3a0d  .. ........try:.
+00062a20: 0a09 0909 0909 0909 7363 616c 696e 673d  ........scaling=
+00062a30: 2872 656c 5f73 6361 6c65 202f 2072 6566  (rel_scale / ref
+00062a40: 5f73 6361 6c65 290d 0a09 0909 0909 0909  _scale).........
+00062a50: 6966 2064 6174 615f 616e 645f 6669 743a  if data_and_fit:
+00062a60: 0d0a 0909 0909 0909 0909 6178 203d 2070  ..........ax = p
+00062a70: 6c6f 7431 6428 7265 5b27 4127 5d2f 7363  lot1d(re['A']/sc
+00062a80: 616c 696e 672c 2063 6d61 7020 3d20 636f  aling, cmap = co
+00062a90: 6c6f 7273 2c20 6178 203d 2061 782c 2077  lors, ax = ax, w
+00062aa0: 6176 656c 656e 6774 6820 3d20 7265 6c5f  avelength = rel_
+00062ab0: 7761 7665 2c20 7769 6474 6820 3d20 7769  wave, width = wi
+00062ac0: 6474 682c 0d0a 0909 0909 0909 0909 0909  dth,............
+00062ad0: 0974 6974 6c65 203d 2027 272c 206c 696e  .title = '', lin
+00062ae0: 6573 5f61 7265 203d 2027 6461 7461 272c  es_are = 'data',
+00062af0: 2073 7562 706c 6f74 203d 2054 7275 652c   subplot = True,
+00062b00: 2063 6f6c 6f72 5f6f 6666 7365 7420 3d20   color_offset = 
+00062b10: 636f 6c6f 725f 6f66 6673 6574 2c0d 0a09  color_offset,...
+00062b20: 0909 0909 0909 0909 0909 706c 6f74 5f74  ..........plot_t
+00062b30: 7970 6520 3d20 7363 616c 655f 7479 7065  ype = scale_type
+00062b40: 2c20 6c69 6e65 7769 6474 6820 3d20 6c69  , linewidth = li
+00062b50: 6e65 7769 6474 6829 0d0a 0909 0909 0909  newidth)........
+00062b60: 0961 7820 3d20 706c 6f74 3164 2872 655b  .ax = plot1d(re[
+00062b70: 2741 4327 5d2f 7363 616c 696e 672c 2063  'AC']/scaling, c
+00062b80: 6d61 7020 3d20 636f 6c6f 7273 2c20 6178  map = colors, ax
+00062b90: 203d 2061 782c 2077 6176 656c 656e 6774   = ax, wavelengt
+00062ba0: 6820 3d20 7265 6c5f 7761 7665 2c20 7769  h = rel_wave, wi
+00062bb0: 6474 6820 3d20 7769 6474 682c 0d0a 0909  dth = width,....
+00062bc0: 0909 0909 0909 0909 7469 746c 6520 3d20  ........title = 
+00062bd0: 2727 2c20 6c69 6e65 735f 6172 6520 3d20  '', lines_are = 
+00062be0: 2766 6974 7465 6427 2c20 7375 6270 6c6f  'fitted', subplo
+00062bf0: 7420 3d20 5472 7565 2c20 636f 6c6f 725f  t = True, color_
+00062c00: 6f66 6673 6574 203d 2063 6f6c 6f72 5f6f  offset = color_o
+00062c10: 6666 7365 742c 200d 0a09 0909 0909 0909  ffset, .........
+00062c20: 0909 0970 6c6f 745f 7479 7065 203d 2073  ...plot_type = s
+00062c30: 6361 6c65 5f74 7970 652c 206c 696e 6577  cale_type, linew
+00062c40: 6964 7468 203d 206c 696e 6577 6964 7468  idth = linewidth
+00062c50: 290d 0a09 0909 0909 0909 0909 0909 0909  )...............
+00062c60: 0909 0909 0909 0909 200d 0a09 0909 0909  ........ .......
+00062c70: 0965 7863 6570 743a 0d0a 0909 0909 0909  .except:........
+00062c80: 0970 7269 6e74 2827 7363 616c 696e 6720  .print('scaling 
+00062c90: 4661 696c 6564 2127 290d 0a09 0909 0909  Failed!').......
+00062ca0: 0909 6966 2064 6174 615f 616e 645f 6669  ..if data_and_fi
+00062cb0: 743a 0d0a 0909 0909 0909 0909 6178 203d  t:..........ax =
+00062cc0: 2070 6c6f 7431 6428 7265 5b27 4127 5d2c   plot1d(re['A'],
+00062cd0: 2063 6d61 7020 3d20 636f 6c6f 7273 2c20   cmap = colors, 
+00062ce0: 6178 203d 2061 782c 2077 6176 656c 656e  ax = ax, wavelen
+00062cf0: 6774 6820 3d20 7265 6c5f 7761 7665 2c20  gth = rel_wave, 
+00062d00: 7769 6474 6820 3d20 7769 6474 682c 200d  width = width, .
+00062d10: 0a09 0909 0909 0909 0909 0909 0974 6974  .............tit
+00062d20: 6c65 203d 2027 272c 206c 696e 6573 5f61  le = '', lines_a
+00062d30: 7265 203d 2027 6461 7461 272c 2073 7562  re = 'data', sub
+00062d40: 706c 6f74 203d 2054 7275 652c 2063 6f6c  plot = True, col
+00062d50: 6f72 5f6f 6666 7365 7420 3d20 636f 6c6f  or_offset = colo
+00062d60: 725f 6f66 6673 6574 2c20 0d0a 0909 0909  r_offset, ......
+00062d70: 0909 0909 0909 0909 706c 6f74 5f74 7970  ........plot_typ
+00062d80: 6520 3d20 7363 616c 655f 7479 7065 2c20  e = scale_type, 
+00062d90: 6c69 6e65 7769 6474 6820 3d20 6c69 6e65  linewidth = line
+00062da0: 7769 6474 6829 0d0a 0909 0909 0909 0961  width).........a
+00062db0: 7820 3d20 706c 6f74 3164 2872 655b 2741  x = plot1d(re['A
+00062dc0: 4327 5d2c 2063 6d61 7020 3d20 636f 6c6f  C'], cmap = colo
+00062dd0: 7273 2c20 6178 203d 2061 782c 2077 6176  rs, ax = ax, wav
+00062de0: 656c 656e 6774 6820 3d20 7265 6c5f 7761  elength = rel_wa
+00062df0: 7665 2c20 7769 6474 6820 3d20 7769 6474  ve, width = widt
+00062e00: 682c 200d 0a09 0909 0909 0909 0909 0909  h, .............
+00062e10: 7469 746c 6520 3d20 2727 2c20 6c69 6e65  title = '', line
+00062e20: 735f 6172 6520 3d20 2766 6974 7465 6427  s_are = 'fitted'
+00062e30: 2c20 7375 6270 6c6f 7420 3d20 5472 7565  , subplot = True
+00062e40: 2c20 636f 6c6f 725f 6f66 6673 6574 203d  , color_offset =
+00062e50: 2063 6f6c 6f72 5f6f 6666 7365 742c 200d   color_offset, .
+00062e60: 0a09 0909 0909 0909 0909 0909 706c 6f74  ............plot
+00062e70: 5f74 7970 6520 3d20 7363 616c 655f 7479  _type = scale_ty
+00062e80: 7065 2c20 6c69 6e65 7769 6474 6820 3d20  pe, linewidth = 
+00062e90: 6c69 6e65 7769 6474 6829 200d 0a09 0909  linewidth) .....
+00062ea0: 0909 656c 7365 3a0d 0a09 0909 0909 0969  ..else:........i
+00062eb0: 6620 6461 7461 5f61 6e64 5f66 6974 3a0d  f data_and_fit:.
+00062ec0: 0a09 0909 0909 0909 6178 203d 2070 6c6f  ........ax = plo
+00062ed0: 7431 6428 7265 5b27 4127 5d2c 2063 6d61  t1d(re['A'], cma
+00062ee0: 7020 3d20 636f 6c6f 7273 2c20 6178 203d  p = colors, ax =
+00062ef0: 2061 782c 2077 6176 656c 656e 6774 6820   ax, wavelength 
+00062f00: 3d20 7265 6c5f 7761 7665 2c20 7769 6474  = rel_wave, widt
+00062f10: 6820 3d20 7769 6474 682c 200d 0a09 0909  h = width, .....
+00062f20: 0909 0909 0909 0909 7469 746c 6520 3d20  ........title = 
+00062f30: 2727 2c20 6c69 6e65 735f 6172 6520 3d20  '', lines_are = 
+00062f40: 2764 6174 6127 2c20 7375 6270 6c6f 7420  'data', subplot 
+00062f50: 3d20 5472 7565 2c20 636f 6c6f 725f 6f66  = True, color_of
+00062f60: 6673 6574 203d 2063 6f6c 6f72 5f6f 6666  fset = color_off
+00062f70: 7365 742c 200d 0a09 0909 0909 0909 0909  set, ...........
+00062f80: 0909 706c 6f74 5f74 7970 6520 3d20 7363  ..plot_type = sc
+00062f90: 616c 655f 7479 7065 2c20 6c69 6e65 7769  ale_type, linewi
+00062fa0: 6474 6820 3d20 6c69 6e65 7769 6474 6829  dth = linewidth)
+00062fb0: 0d0a 0909 0909 0909 6178 203d 2070 6c6f  ........ax = plo
+00062fc0: 7431 6428 7265 5b27 4143 275d 2c20 636d  t1d(re['AC'], cm
+00062fd0: 6170 203d 2063 6f6c 6f72 732c 2061 7820  ap = colors, ax 
+00062fe0: 3d20 6178 2c20 7761 7665 6c65 6e67 7468  = ax, wavelength
+00062ff0: 203d 2072 656c 5f77 6176 652c 2077 6964   = rel_wave, wid
+00063000: 7468 203d 2077 6964 7468 2c20 0d0a 0909  th = width, ....
+00063010: 0909 0909 0909 0909 7469 746c 6520 3d20  ........title = 
+00063020: 2727 2c20 6c69 6e65 735f 6172 6520 3d20  '', lines_are = 
+00063030: 2766 6974 7465 6427 2c20 7375 6270 6c6f  'fitted', subplo
+00063040: 7420 3d20 5472 7565 2c20 636f 6c6f 725f  t = True, color_
+00063050: 6f66 6673 6574 203d 2063 6f6c 6f72 5f6f  offset = color_o
+00063060: 6666 7365 742c 200d 0a09 0909 0909 0909  ffset, .........
+00063070: 0909 0970 6c6f 745f 7479 7065 203d 2073  ...plot_type = s
+00063080: 6361 6c65 5f74 7970 652c 206c 696e 6577  cale_type, linew
+00063090: 6964 7468 203d 206c 696e 6577 6964 7468  idth = linewidth
+000630a0: 290d 0a09 0909 0909 666f 7220 656e 7420  ).......for ent 
+000630b0: 696e 2072 656c 5f77 6176 653a 0d0a 0909  in rel_wave:....
+000630c0: 0909 0909 6966 2064 6174 615f 616e 645f  ....if data_and_
+000630d0: 6669 743a 0d0a 0909 0909 0909 096c 6162  fit:.........lab
+000630e0: 2e61 7070 656e 6428 2725 6720 6e6d 2725  .append('%g nm'%
+000630f0: 656e 7420 2b20 275f 2720 2b20 7374 7228  ent + '_' + str(
+00063100: 6f2e 6669 6c65 6e61 6d65 2929 0d0a 0909  o.filename))....
+00063110: 0909 0909 6c61 622e 6170 7065 6e64 2827  ....lab.append('
+00063120: 2567 206e 6d27 2565 6e74 202b 2027 5f27  %g nm'%ent + '_'
+00063130: 202b 2073 7472 286f 2e66 696c 656e 616d   + str(o.filenam
+00063140: 6529 290d 0a09 0909 0909 6861 6e64 6c65  e)).......handle
+00063150: 732c 206c 6162 656c 733d 6178 2e67 6574  s, labels=ax.get
+00063160: 5f6c 6567 656e 645f 6861 6e64 6c65 735f  _legend_handles_
+00063170: 6c61 6265 6c73 2829 0d0a 0909 0909 0969  labels().......i
+00063180: 6620 6461 7461 5f61 6e64 5f66 6974 3a0d  f data_and_fit:.
+00063190: 0a09 0909 0909 0966 6f72 2061 2069 6e20  .......for a in 
+000631a0: 6861 6e64 6c65 735b 2d32 2a6c 656e 2872  handles[-2*len(r
+000631b0: 656c 5f77 6176 6529 3a5d 3a0d 0a09 0909  el_wave):]:.....
+000631c0: 0909 0909 6861 6e64 2e61 7070 656e 6428  ....hand.append(
+000631d0: 6129 0d0a 0909 0909 0965 6c73 653a 0d0a  a).......else:..
+000631e0: 0909 0909 0909 666f 7220 6120 696e 2068  ......for a in h
+000631f0: 616e 646c 6573 5b2d 6c65 6e28 7265 6c5f  andles[-len(rel_
+00063200: 7761 7665 293a 5d3a 0d0a 0909 0909 0909  wave):]:........
+00063210: 0968 616e 642e 6170 7065 6e64 2861 290d  .hand.append(a).
+00063220: 0a09 0909 6966 206e 6f72 6d5f 7769 6e64  ....if norm_wind
+00063230: 6f77 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ow is not None:.
+00063240: 0a09 0909 0920 0d0a 0909 0909 6178 2e73  ..... ......ax.s
+00063250: 6574 5f74 6974 6c65 2827 636f 6d70 6172  et_title('compar
+00063260: 6520 6d65 6173 7572 6564 2061 6e64 2066  e measured and f
+00063270: 6974 7465 6420 6461 7461 2061 7420 6769  itted data at gi
+00063280: 7665 6e20 7761 7665 6c65 6e67 7468 205c  ven wavelength \
+00063290: 6e20 7363 616c 6564 2074 6f20 743d 2567  n scaled to t=%g
+000632a0: 2070 7320 3a20 2567 2070 7320 2c20 776c   ps : %g ps , wl
+000632b0: 3d20 2567 206e 6d3a 2025 6720 6e6d 2725  = %g nm: %g nm'%
+000632c0: 286e 6f72 6d5f 7769 6e64 6f77 5b30 5d2c  (norm_window[0],
+000632d0: 6e6f 726d 5f77 696e 646f 775b 315d 2c6e  norm_window[1],n
+000632e0: 6f72 6d5f 7769 6e64 6f77 5b32 5d2c 6e6f  orm_window[2],no
+000632f0: 726d 5f77 696e 646f 775b 335d 2929 0d0a  rm_window[3]))..
+00063300: 0909 0965 6c73 653a 0d0a 0909 0909 6178  ...else:......ax
+00063310: 2e73 6574 5f74 6974 6c65 2827 636f 6d70  .set_title('comp
+00063320: 6172 6520 6d65 6173 7572 6564 2061 6e64  are measured and
+00063330: 2066 6974 7465 6420 6461 7461 2061 7420   fitted data at 
+00063340: 6769 7665 6e20 7761 7665 6c65 6e67 7468  given wavelength
+00063350: 2729 0d0a 0909 0961 782e 7365 745f 786c  ').....ax.set_xl
+00063360: 696d 2872 655b 2741 275d 2e69 6e64 6578  im(re['A'].index
+00063370: 2e76 616c 7565 735b 305d 2c72 655b 2741  .values[0],re['A
+00063380: 275d 2e69 6e64 6578 2e76 616c 7565 735b  '].index.values[
+00063390: 2d31 5d29 0d0a 0909 0961 782e 6c65 6765  -1]).....ax.lege
+000633a0: 6e64 2868 616e 642c 6c61 6229 0d0a 0909  nd(hand,lab)....
+000633b0: 656c 7365 3a0d 0a09 0909 6669 672c 2061  else:.....fig, a
+000633c0: 7820 3d20 706c 742e 7375 6270 6c6f 7473  x = plt.subplots
+000633d0: 2866 6967 7369 7a65 203d 2028 3130 2c20  (figsize = (10, 
+000633e0: 3629 2c20 6470 6920 3d20 3130 3029 0d0a  6), dpi = 100)..
+000633f0: 0909 0963 6f6c 6f72 7320 3d20 636f 6c6d  ...colors = colm
+00063400: 2863 6d61 7020 3d20 636d 6170 2c20 6b20  (cmap = cmap, k 
+00063410: 3d20 7261 6e67 6528 6c65 6e28 7265 6c5f  = range(len(rel_
+00063420: 7761 7665 292a 2832 2b6c 656e 286f 7468  wave)*(2+len(oth
+00063430: 6572 2929 2929 0d0a 0909 0969 6620 6e6f  er)))).....if no
+00063440: 726d 5f77 696e 646f 7720 6973 206e 6f74  rm_window is not
+00063450: 204e 6f6e 653a 0d0a 0909 0909 7265 665f   None:......ref_
+00063460: 7363 616c 6520 3d20 7365 6c66 2e64 732e  scale = self.ds.
+00063470: 6c6f 635b 6e6f 726d 5f77 696e 646f 775b  loc[norm_window[
+00063480: 305d 3a6e 6f72 6d5f 7769 6e64 6f77 5b31  0]:norm_window[1
+00063490: 5d2c 206e 6f72 6d5f 7769 6e64 6f77 5b32  ], norm_window[2
+000634a0: 5d3a 6e6f 726d 5f77 696e 646f 775b 335d  ]:norm_window[3]
+000634b0: 5d2e 6d65 616e 2829 2e6d 6561 6e28 290d  ].mean().mean().
+000634c0: 0a09 0909 6178 203d 2070 6c6f 7431 6428  ....ax = plot1d(
+000634d0: 7365 6c66 2e64 732c 2063 6d61 7020 3d20  self.ds, cmap = 
+000634e0: 636f 6c6f 7273 2c20 6178 203d 2061 782c  colors, ax = ax,
+000634f0: 2077 6176 656c 656e 6774 6820 3d20 7265   wavelength = re
+00063500: 6c5f 7761 7665 2c20 7769 6474 6820 3d20  l_wave, width = 
+00063510: 7769 6474 682c 2074 6974 6c65 203d 2073  width, title = s
+00063520: 656c 662e 6669 6c65 6e61 6d65 2c0d 0a09  elf.filename,...
+00063530: 0909 0909 0962 6173 6575 6e69 7420 3d20  .....baseunit = 
+00063540: 7365 6c66 2e62 6173 6575 6e69 742c 206c  self.baseunit, l
+00063550: 696e 6573 5f61 7265 203d 2027 6461 7461  ines_are = 'data
+00063560: 272c 2073 6361 7474 6572 6375 7420 3d20  ', scattercut = 
+00063570: 7365 6c66 2e73 6361 7474 6572 6375 742c  self.scattercut,
+00063580: 200d 0a09 0909 0909 0962 6f72 6465 7263   ........borderc
+00063590: 7574 203d 2073 656c 662e 626f 7264 6572  ut = self.border
+000635a0: 6375 742c 2073 7562 706c 6f74 203d 2046  cut, subplot = F
+000635b0: 616c 7365 2c20 636f 6c6f 725f 6f66 6673  alse, color_offs
+000635c0: 6574 203d 2030 2c20 7469 6d65 6c69 6d69  et = 0, timelimi
+000635d0: 7473 203d 2073 656c 662e 7469 6d65 6c69  ts = self.timeli
+000635e0: 6d69 7473 2c20 0d0a 0909 0909 0909 696e  mits, ........in
+000635f0: 7465 6e73 6974 795f 7261 6e67 6520 3d20  tensity_range = 
+00063600: 7365 6c66 2e69 6e74 656e 7369 7479 5f72  self.intensity_r
+00063610: 616e 6765 2c20 706c 6f74 5f74 7970 6520  ange, plot_type 
+00063620: 3d20 7363 616c 655f 7479 7065 2c20 6c69  = scale_type, li
+00063630: 6e65 7769 6474 6820 3d20 6c69 6e65 7769  newidth = linewi
+00063640: 6474 6829 0d0a 0909 0961 7820 3d20 706c  dth).....ax = pl
+00063650: 6f74 3164 2873 656c 662e 6473 2c20 636d  ot1d(self.ds, cm
+00063660: 6170 203d 2063 6f6c 6f72 732c 2061 7820  ap = colors, ax 
+00063670: 3d20 6178 2c20 7761 7665 6c65 6e67 7468  = ax, wavelength
+00063680: 203d 2072 656c 5f77 6176 652c 2077 6964   = rel_wave, wid
+00063690: 7468 203d 2077 6964 7468 2c20 7469 746c  th = width, titl
+000636a0: 6520 3d20 7365 6c66 2e66 696c 656e 616d  e = self.filenam
+000636b0: 652c 200d 0a09 0909 0909 0962 6173 6575  e, ........baseu
+000636c0: 6e69 7420 3d20 7365 6c66 2e62 6173 6575  nit = self.baseu
+000636d0: 6e69 742c 206c 696e 6573 5f61 7265 203d  nit, lines_are =
+000636e0: 2027 736d 6f6f 7468 6564 272c 2073 6361   'smoothed', sca
+000636f0: 7474 6572 6375 7420 3d20 7365 6c66 2e73  ttercut = self.s
+00063700: 6361 7474 6572 6375 742c 200d 0a09 0909  cattercut, .....
+00063710: 0909 0962 6f72 6465 7263 7574 203d 2073  ...bordercut = s
+00063720: 656c 662e 626f 7264 6572 6375 742c 2073  elf.bordercut, s
+00063730: 7562 706c 6f74 203d 2046 616c 7365 2c20  ubplot = False, 
+00063740: 636f 6c6f 725f 6f66 6673 6574 203d 2030  color_offset = 0
+00063750: 2c20 7469 6d65 6c69 6d69 7473 203d 2073  , timelimits = s
+00063760: 656c 662e 7469 6d65 6c69 6d69 7473 2c20  elf.timelimits, 
+00063770: 0d0a 0909 0909 0909 696e 7465 6e73 6974  ........intensit
+00063780: 795f 7261 6e67 6520 3d20 7365 6c66 2e69  y_range = self.i
+00063790: 6e74 656e 7369 7479 5f72 616e 6765 2c20  ntensity_range, 
+000637a0: 706c 6f74 5f74 7970 6520 3d20 7363 616c  plot_type = scal
+000637b0: 655f 7479 7065 2c20 6c69 6e65 7769 6474  e_type, linewidt
+000637c0: 6820 3d20 6c69 6e65 7769 6474 6829 0d0a  h = linewidth)..
+000637d0: 0909 0969 6620 313a 0d0a 0909 0909 6861  ...if 1:......ha
+000637e0: 6e64 6c65 732c 206c 6162 656c 733d 6178  ndles, labels=ax
+000637f0: 2e67 6574 5f6c 6567 656e 645f 6861 6e64  .get_legend_hand
+00063800: 6c65 735f 6c61 6265 6c73 2829 0d0a 0909  les_labels()....
+00063810: 0909 6c61 623d 5b27 2567 206e 6d27 2561  ..lab=['%g nm'%a
+00063820: 202b 2027 5f27 202b 2073 7472 2873 656c   + '_' + str(sel
+00063830: 662e 6669 6c65 6e61 6d65 2920 666f 7220  f.filename) for 
+00063840: 6120 696e 2072 656c 5f77 6176 655d 0d0a  a in rel_wave]..
+00063850: 0909 0909 6861 6e64 3d68 616e 646c 6573  ....hand=handles
+00063860: 5b6c 656e 2872 656c 5f77 6176 6529 3a5d  [len(rel_wave):]
+00063870: 0d0a 0909 0909 6966 206f 7468 6572 2069  ......if other i
+00063880: 7320 6e6f 7420 4e6f 6e65 3a0d 0a09 0909  s not None:.....
+00063890: 0909 666f 7220 692c 6f20 696e 2065 6e75  ..for i,o in enu
+000638a0: 6d65 7261 7465 286f 7468 6572 293a 0d0a  merate(other):..
+000638b0: 0909 0909 0909 692b 3d31 0d0a 0909 0909  ......i+=1......
+000638c0: 0909 636f 6c6f 725f 6f66 6673 6574 3d28  ..color_offset=(
+000638d0: 692b 3129 2a6c 656e 2872 656c 5f77 6176  i+1)*len(rel_wav
+000638e0: 6529 0d0a 0909 0909 0909 6966 206e 6f72  e)........if nor
+000638f0: 6d5f 7769 6e64 6f77 2069 7320 6e6f 7420  m_window is not 
+00063900: 4e6f 6e65 3a0d 0a09 0909 0909 0909 7265  None:.........re
+00063910: 6c5f 7363 616c 653d 6f2e 6473 2e6c 6f63  l_scale=o.ds.loc
+00063920: 5b6e 6f72 6d5f 7769 6e64 6f77 5b30 5d3a  [norm_window[0]:
+00063930: 6e6f 726d 5f77 696e 646f 775b 315d 2c6e  norm_window[1],n
+00063940: 6f72 6d5f 7769 6e64 6f77 5b32 5d3a 6e6f  orm_window[2]:no
+00063950: 726d 5f77 696e 646f 775b 335d 5d2e 6d65  rm_window[3]].me
+00063960: 616e 2829 2e6d 6561 6e28 290d 0a09 0909  an().mean().....
+00063970: 0909 0909 7472 793a 0d0a 0909 0909 0909  ....try:........
+00063980: 0909 7363 616c 696e 673d 2872 656c 5f73  ..scaling=(rel_s
+00063990: 6361 6c65 2f72 6566 5f73 6361 6c65 290d  cale/ref_scale).
+000639a0: 0a09 0909 0909 0909 0961 7820 3d20 706c  .........ax = pl
+000639b0: 6f74 3164 286f 2e64 732f 7363 616c 696e  ot1d(o.ds/scalin
+000639c0: 672c 2063 6d61 7020 3d20 636f 6c6f 7273  g, cmap = colors
+000639d0: 2c20 6178 203d 2061 782c 2077 6176 656c  , ax = ax, wavel
+000639e0: 656e 6774 6820 3d20 7265 6c5f 7761 7665  ength = rel_wave
+000639f0: 2c20 7769 6474 6820 3d20 7769 6474 682c  , width = width,
+00063a00: 0d0a 0909 0909 0909 0909 0909 0974 6974  .............tit
+00063a10: 6c65 203d 206f 2e66 696c 656e 616d 652c  le = o.filename,
+00063a20: 2062 6173 6575 6e69 7420 3d20 7365 6c66   baseunit = self
+00063a30: 2e62 6173 6575 6e69 742c 2074 696d 656c  .baseunit, timel
+00063a40: 696d 6974 7320 3d20 7365 6c66 2e74 696d  imits = self.tim
+00063a50: 656c 696d 6974 732c 0d0a 0909 0909 0909  elimits,........
+00063a60: 0909 0909 096c 696e 6573 5f61 7265 203d  .....lines_are =
+00063a70: 2027 6461 7461 272c 2073 6361 7474 6572   'data', scatter
+00063a80: 6375 7420 3d20 7365 6c66 2e73 6361 7474  cut = self.scatt
+00063a90: 6572 6375 742c 2062 6f72 6465 7263 7574  ercut, bordercut
+00063aa0: 203d 2073 656c 662e 626f 7264 6572 6375   = self.bordercu
+00063ab0: 742c 0d0a 0909 0909 0909 0909 0909 0973  t,.............s
+00063ac0: 7562 706c 6f74 203d 2054 7275 652c 2063  ubplot = True, c
+00063ad0: 6f6c 6f72 5f6f 6666 7365 7420 3d20 636f  olor_offset = co
+00063ae0: 6c6f 725f 6f66 6673 6574 2c20 0d0a 0909  lor_offset, ....
+00063af0: 0909 0909 0909 0909 0969 6e74 656e 7369  .........intensi
+00063b00: 7479 5f72 616e 6765 203d 2073 656c 662e  ty_range = self.
+00063b10: 696e 7465 6e73 6974 795f 7261 6e67 652c  intensity_range,
+00063b20: 2070 6c6f 745f 7479 7065 203d 2073 6361   plot_type = sca
+00063b30: 6c65 5f74 7970 652c 206c 696e 6577 6964  le_type, linewid
+00063b40: 7468 203d 206c 696e 6577 6964 7468 290d  th = linewidth).
+00063b50: 0a09 0909 0909 0909 0961 7820 3d20 706c  .........ax = pl
+00063b60: 6f74 3164 286f 2e64 732f 7363 616c 696e  ot1d(o.ds/scalin
+00063b70: 672c 2063 6d61 7020 3d20 636f 6c6f 7273  g, cmap = colors
+00063b80: 2c20 6178 203d 2061 782c 2077 6176 656c  , ax = ax, wavel
+00063b90: 656e 6774 6820 3d20 7265 6c5f 7761 7665  ength = rel_wave
+00063ba0: 2c20 7769 6474 6820 3d20 7769 6474 682c  , width = width,
+00063bb0: 0d0a 0909 0909 0909 0909 0909 0974 6974  .............tit
+00063bc0: 6c65 203d 206f 2e66 696c 656e 616d 652c  le = o.filename,
+00063bd0: 2062 6173 6575 6e69 7420 3d20 7365 6c66   baseunit = self
+00063be0: 2e62 6173 6575 6e69 742c 2074 696d 656c  .baseunit, timel
+00063bf0: 696d 6974 7320 3d20 7365 6c66 2e74 696d  imits = self.tim
+00063c00: 656c 696d 6974 732c 0d0a 0909 0909 0909  elimits,........
+00063c10: 0909 0909 096c 696e 6573 5f61 7265 203d  .....lines_are =
+00063c20: 2027 736d 6f6f 7468 6564 272c 2073 6361   'smoothed', sca
+00063c30: 7474 6572 6375 7420 3d20 7365 6c66 2e73  ttercut = self.s
+00063c40: 6361 7474 6572 6375 742c 2062 6f72 6465  cattercut, borde
+00063c50: 7263 7574 203d 2073 656c 662e 626f 7264  rcut = self.bord
+00063c60: 6572 6375 742c 0d0a 0909 0909 0909 0909  ercut,..........
+00063c70: 0909 0973 7562 706c 6f74 203d 2054 7275  ...subplot = Tru
+00063c80: 652c 2063 6f6c 6f72 5f6f 6666 7365 7420  e, color_offset 
+00063c90: 3d20 636f 6c6f 725f 6f66 6673 6574 2c20  = color_offset, 
+00063ca0: 0d0a 0909 0909 0909 0909 0909 0969 6e74  .............int
+00063cb0: 656e 7369 7479 5f72 616e 6765 203d 2073  ensity_range = s
+00063cc0: 656c 662e 696e 7465 6e73 6974 795f 7261  elf.intensity_ra
+00063cd0: 6e67 652c 2070 6c6f 745f 7479 7065 203d  nge, plot_type =
+00063ce0: 2073 6361 6c65 5f74 7970 652c 206c 696e   scale_type, lin
+00063cf0: 6577 6964 7468 203d 206c 696e 6577 6964  ewidth = linewid
+00063d00: 7468 290d 0a09 0909 0909 0909 6578 6365  th).........exce
+00063d10: 7074 3a0d 0a09 0909 0909 0909 0970 7269  pt:..........pri
+00063d20: 6e74 2827 7363 616c 696e 6720 6661 696c  nt('scaling fail
+00063d30: 6564 2729 0d0a 0909 0909 0909 0909 6178  ed')..........ax
+00063d40: 203d 2070 6c6f 7431 6428 6f2e 6473 2c20   = plot1d(o.ds, 
+00063d50: 636d 6170 203d 2063 6f6c 6f72 732c 2061  cmap = colors, a
+00063d60: 7820 3d20 6178 2c20 7761 7665 6c65 6e67  x = ax, waveleng
+00063d70: 7468 203d 2072 656c 5f77 6176 652c 2077  th = rel_wave, w
+00063d80: 6964 7468 203d 2077 6964 7468 2c0d 0a09  idth = width,...
+00063d90: 0909 0909 0909 0909 0909 7469 746c 6520  ..........title 
+00063da0: 3d20 6f2e 6669 6c65 6e61 6d65 2c20 6261  = o.filename, ba
+00063db0: 7365 756e 6974 203d 2073 656c 662e 6261  seunit = self.ba
+00063dc0: 7365 756e 6974 2c20 7469 6d65 6c69 6d69  seunit, timelimi
+00063dd0: 7473 203d 2073 656c 662e 7469 6d65 6c69  ts = self.timeli
+00063de0: 6d69 7473 2c0d 0a09 0909 0909 0909 0909  mits,...........
+00063df0: 0909 6c69 6e65 735f 6172 6520 3d20 2764  ..lines_are = 'd
+00063e00: 6174 6127 2c20 7363 6174 7465 7263 7574  ata', scattercut
+00063e10: 203d 2073 656c 662e 7363 6174 7465 7263   = self.scatterc
+00063e20: 7574 2c20 626f 7264 6572 6375 7420 3d20  ut, bordercut = 
+00063e30: 7365 6c66 2e62 6f72 6465 7263 7574 2c0d  self.bordercut,.
+00063e40: 0a09 0909 0909 0909 0909 0909 7375 6270  ............subp
+00063e50: 6c6f 7420 3d20 5472 7565 2c20 636f 6c6f  lot = True, colo
+00063e60: 725f 6f66 6673 6574 203d 2063 6f6c 6f72  r_offset = color
+00063e70: 5f6f 6666 7365 742c 200d 0a09 0909 0909  _offset, .......
+00063e80: 0909 0909 0909 696e 7465 6e73 6974 795f  ......intensity_
+00063e90: 7261 6e67 6520 3d20 7365 6c66 2e69 6e74  range = self.int
+00063ea0: 656e 7369 7479 5f72 616e 6765 2c20 706c  ensity_range, pl
+00063eb0: 6f74 5f74 7970 6520 3d20 7363 616c 655f  ot_type = scale_
+00063ec0: 7479 7065 2c20 6c69 6e65 7769 6474 6820  type, linewidth 
+00063ed0: 3d20 6c69 6e65 7769 6474 6829 0d0a 0909  = linewidth)....
+00063ee0: 0909 0909 0909 6178 203d 2070 6c6f 7431  ......ax = plot1
+00063ef0: 6428 6f2e 6473 2c20 636d 6170 203d 2063  d(o.ds, cmap = c
+00063f00: 6f6c 6f72 732c 2061 7820 3d20 6178 2c20  olors, ax = ax, 
+00063f10: 7761 7665 6c65 6e67 7468 203d 2072 656c  wavelength = rel
+00063f20: 5f77 6176 652c 2077 6964 7468 203d 2077  _wave, width = w
+00063f30: 6964 7468 2c0d 0a09 0909 0909 0909 0909  idth,...........
+00063f40: 0909 7469 746c 6520 3d20 6f2e 6669 6c65  ..title = o.file
+00063f50: 6e61 6d65 2c20 6261 7365 756e 6974 203d  name, baseunit =
+00063f60: 2073 656c 662e 6261 7365 756e 6974 2c20   self.baseunit, 
+00063f70: 7469 6d65 6c69 6d69 7473 203d 2073 656c  timelimits = sel
+00063f80: 662e 7469 6d65 6c69 6d69 7473 2c0d 0a09  f.timelimits,...
+00063f90: 0909 0909 0909 0909 0909 6c69 6e65 735f  ..........lines_
+00063fa0: 6172 6520 3d20 2773 6d6f 6f74 6865 6427  are = 'smoothed'
+00063fb0: 2c20 7363 6174 7465 7263 7574 203d 2073  , scattercut = s
+00063fc0: 656c 662e 7363 6174 7465 7263 7574 2c20  elf.scattercut, 
+00063fd0: 626f 7264 6572 6375 7420 3d20 7365 6c66  bordercut = self
+00063fe0: 2e62 6f72 6465 7263 7574 2c0d 0a09 0909  .bordercut,.....
+00063ff0: 0909 0909 0909 0909 7375 6270 6c6f 7420  ........subplot 
+00064000: 3d20 5472 7565 2c20 636f 6c6f 725f 6f66  = True, color_of
+00064010: 6673 6574 203d 2063 6f6c 6f72 5f6f 6666  fset = color_off
+00064020: 7365 742c 200d 0a09 0909 0909 0909 0909  set, ...........
+00064030: 0909 696e 7465 6e73 6974 795f 7261 6e67  ..intensity_rang
+00064040: 6520 3d20 7365 6c66 2e69 6e74 656e 7369  e = self.intensi
+00064050: 7479 5f72 616e 6765 2c20 706c 6f74 5f74  ty_range, plot_t
+00064060: 7970 6520 3d20 7363 616c 655f 7479 7065  ype = scale_type
+00064070: 2c20 6c69 6e65 7769 6474 6820 3d20 6c69  , linewidth = li
+00064080: 6e65 7769 6474 6829 0d0a 0909 0909 0909  newidth)........
+00064090: 656c 7365 3a0d 0a09 0909 0909 0909 6178  else:.........ax
+000640a0: 203d 2070 6c6f 7431 6428 6f2e 6473 2c20   = plot1d(o.ds, 
+000640b0: 636d 6170 203d 2063 6f6c 6f72 732c 2061  cmap = colors, a
+000640c0: 7820 3d20 6178 2c20 7761 7665 6c65 6e67  x = ax, waveleng
+000640d0: 7468 203d 2072 656c 5f77 6176 652c 2077  th = rel_wave, w
+000640e0: 6964 7468 203d 2077 6964 7468 2c20 7469  idth = width, ti
+000640f0: 746c 6520 3d20 6f2e 6669 6c65 6e61 6d65  tle = o.filename
+00064100: 2c0d 0a09 0909 0909 0909 0909 0962 6173  ,............bas
+00064110: 6575 6e69 7420 3d20 7365 6c66 2e62 6173  eunit = self.bas
+00064120: 6575 6e69 742c 2074 696d 656c 696d 6974  eunit, timelimit
+00064130: 7320 3d20 7365 6c66 2e74 696d 656c 696d  s = self.timelim
+00064140: 6974 732c 206c 696e 6573 5f61 7265 203d  its, lines_are =
+00064150: 2027 6461 7461 272c 0d0a 0909 0909 0909   'data',........
+00064160: 0909 0909 7363 6174 7465 7263 7574 203d  ....scattercut =
+00064170: 2073 656c 662e 7363 6174 7465 7263 7574   self.scattercut
+00064180: 2c20 626f 7264 6572 6375 7420 3d20 7365  , bordercut = se
+00064190: 6c66 2e62 6f72 6465 7263 7574 2c20 7375  lf.bordercut, su
+000641a0: 6270 6c6f 7420 3d20 5472 7565 2c0d 0a09  bplot = True,...
+000641b0: 0909 0909 0909 0909 0963 6f6c 6f72 5f6f  .........color_o
+000641c0: 6666 7365 7420 3d20 636f 6c6f 725f 6f66  ffset = color_of
+000641d0: 6673 6574 2c20 696e 7465 6e73 6974 795f  fset, intensity_
+000641e0: 7261 6e67 6520 3d20 7365 6c66 2e69 6e74  range = self.int
+000641f0: 656e 7369 7479 5f72 616e 6765 2c20 0d0a  ensity_range, ..
+00064200: 0909 0909 0909 0909 0909 706c 6f74 5f74  ..........plot_t
+00064210: 7970 6520 3d20 7363 616c 655f 7479 7065  ype = scale_type
+00064220: 2c20 6c69 6e65 7769 6474 6820 3d20 6c69  , linewidth = li
+00064230: 6e65 7769 6474 6829 0d0a 0909 0909 0909  newidth)........
+00064240: 0961 7820 3d20 706c 6f74 3164 286f 2e64  .ax = plot1d(o.d
+00064250: 732c 2063 6d61 7020 3d20 636f 6c6f 7273  s, cmap = colors
+00064260: 2c20 6178 203d 2061 782c 2077 6176 656c  , ax = ax, wavel
+00064270: 656e 6774 6820 3d20 7265 6c5f 7761 7665  ength = rel_wave
+00064280: 2c20 7769 6474 6820 3d20 7769 6474 682c  , width = width,
+00064290: 2074 6974 6c65 203d 206f 2e66 696c 656e   title = o.filen
+000642a0: 616d 652c 0d0a 0909 0909 0909 0909 0909  ame,............
+000642b0: 6261 7365 756e 6974 203d 2073 656c 662e  baseunit = self.
+000642c0: 6261 7365 756e 6974 2c20 7469 6d65 6c69  baseunit, timeli
+000642d0: 6d69 7473 203d 2073 656c 662e 7469 6d65  mits = self.time
+000642e0: 6c69 6d69 7473 2c20 6c69 6e65 735f 6172  limits, lines_ar
+000642f0: 6520 3d20 2773 6d6f 6f74 6865 6427 2c0d  e = 'smoothed',.
+00064300: 0a09 0909 0909 0909 0909 0973 6361 7474  ...........scatt
+00064310: 6572 6375 7420 3d20 7365 6c66 2e73 6361  ercut = self.sca
+00064320: 7474 6572 6375 742c 2062 6f72 6465 7263  ttercut, borderc
+00064330: 7574 203d 2073 656c 662e 626f 7264 6572  ut = self.border
+00064340: 6375 742c 2073 7562 706c 6f74 203d 2054  cut, subplot = T
+00064350: 7275 652c 0d0a 0909 0909 0909 0909 0909  rue,............
+00064360: 636f 6c6f 725f 6f66 6673 6574 203d 2063  color_offset = c
+00064370: 6f6c 6f72 5f6f 6666 7365 742c 2069 6e74  olor_offset, int
+00064380: 656e 7369 7479 5f72 616e 6765 203d 2073  ensity_range = s
+00064390: 656c 662e 696e 7465 6e73 6974 795f 7261  elf.intensity_ra
+000643a0: 6e67 652c 200d 0a09 0909 0909 0909 0909  nge, ...........
+000643b0: 0970 6c6f 745f 7479 7065 203d 2073 6361  .plot_type = sca
+000643c0: 6c65 5f74 7970 652c 206c 696e 6577 6964  le_type, linewid
+000643d0: 7468 203d 206c 696e 6577 6964 7468 290d  th = linewidth).
+000643e0: 0a09 0909 0909 0966 6f72 2065 6e74 2069  .......for ent i
+000643f0: 6e20 5b27 2567 206e 6d27 2561 202b 2027  n ['%g nm'%a + '
+00064400: 5f27 202b 2073 7472 286f 2e66 696c 656e  _' + str(o.filen
+00064410: 616d 6529 2066 6f72 2061 2069 6e20 7265  ame) for a in re
+00064420: 6c5f 7761 7665 5d3a 0d0a 0909 0909 0909  l_wave]:........
+00064430: 096c 6162 2e61 7070 656e 6428 656e 7429  .lab.append(ent)
+00064440: 0d0a 0909 0909 0909 6861 6e64 6c65 732c  ........handles,
+00064450: 206c 6162 656c 733d 6178 2e67 6574 5f6c   labels=ax.get_l
+00064460: 6567 656e 645f 6861 6e64 6c65 735f 6c61  egend_handles_la
+00064470: 6265 6c73 2829 0d0a 0909 0909 0909 666f  bels()........fo
+00064480: 7220 6861 2069 6e20 6861 6e64 6c65 735b  r ha in handles[
+00064490: 2d6c 656e 2872 656c 5f77 6176 6529 3a5d  -len(rel_wave):]
+000644a0: 3a0d 0a09 0909 0909 0909 6861 6e64 2e61  :.........hand.a
+000644b0: 7070 656e 6428 6861 290d 0a09 0909 0961  ppend(ha)......a
+000644c0: 782e 7365 745f 7469 746c 6528 2763 6f6d  x.set_title('com
+000644d0: 7061 7265 206d 6561 7375 7265 6420 616e  pare measured an
+000644e0: 6420 736d 6f6f 7468 6564 2064 6174 6120  d smoothed data 
+000644f0: 6174 2067 6976 656e 2077 6176 656c 656e  at given wavelen
+00064500: 6774 6827 290d 0a09 0909 0969 6620 6e6f  gth')......if no
+00064510: 726d 5f77 696e 646f 7720 6973 206e 6f74  rm_window is not
+00064520: 204e 6f6e 653a 0d0a 0909 0909 0961 782e   None:.......ax.
+00064530: 7365 745f 7469 746c 6528 2763 6f6d 7061  set_title('compa
+00064540: 7265 206d 6561 7375 7265 6420 616e 6420  re measured and 
+00064550: 736d 6f6f 7468 6564 2064 6174 6120 6174  smoothed data at
+00064560: 2067 6976 656e 2077 6176 656c 656e 6774   given wavelengt
+00064570: 6820 5c6e 2073 6361 6c65 6420 746f 2074  h \n scaled to t
+00064580: 3d25 6720 7073 203a 2025 6720 7073 202c  =%g ps : %g ps ,
+00064590: 2077 6c3d 2025 6720 6e6d 3a20 2567 206e   wl= %g nm: %g n
+000645a0: 6d27 2528 6e6f 726d 5f77 696e 646f 775b  m'%(norm_window[
+000645b0: 305d 2c6e 6f72 6d5f 7769 6e64 6f77 5b31  0],norm_window[1
+000645c0: 5d2c 6e6f 726d 5f77 696e 646f 775b 325d  ],norm_window[2]
+000645d0: 2c6e 6f72 6d5f 7769 6e64 6f77 5b33 5d29  ,norm_window[3])
+000645e0: 290d 0a09 0909 0961 782e 6c65 6765 6e64  )......ax.legend
+000645f0: 2868 616e 642c 6c61 6229 0d0a 0909 6966  (hand,lab)....if
+00064600: 2073 656c 662e 7361 7665 5f66 6967 7572   self.save_figur
+00064610: 6573 5f74 6f5f 666f 6c64 6572 3a20 200d  es_to_folder:  .
+00064620: 0a09 0909 6669 672e 7361 7665 6669 6728  ....fig.savefig(
+00064630: 6368 6563 6b5f 666f 6c64 6572 2870 6174  check_folder(pat
+00064640: 683d 7365 6c66 2e66 6967 7572 655f 7061  h=self.figure_pa
+00064650: 7468 2c66 696c 656e 616d 653d 2763 6f6d  th,filename='com
+00064660: 7061 7265 5f61 745f 7761 7665 5f25 732e  pare_at_wave_%s.
+00064670: 706e 6727 2527 5f27 2e6a 6f69 6e28 5b27  png'%'_'.join(['
+00064680: 2567 2725 6120 666f 7220 6120 696e 2072  %g'%a for a in r
+00064690: 656c 5f77 6176 655d 2929 2c0d 0a09 0909  el_wave])),.....
+000646a0: 6262 6f78 5f69 6e63 6865 733d 2774 6967  bbox_inches='tig
+000646b0: 6874 2729 0d0a 0909 0972 6574 7572 6e20  ht').....return 
+000646c0: 6178 0d0a 0d0a 0d0a 0964 6566 2043 6f6d  ax.......def Com
+000646d0: 7061 7265 5f44 4143 2873 656c 662c 206f  pare_DAC(self, o
+000646e0: 7468 6572 203d 204e 6f6e 652c 2073 7065  ther = None, spe
+000646f0: 6374 7261 203d 204e 6f6e 652c 2073 6570  ctra = None, sep
+00064700: 6172 6174 655f 706c 6f74 7320 3d20 4661  arate_plots = Fa
+00064710: 6c73 652c 2063 6d61 7020 3d20 4e6f 6e65  lse, cmap = None
+00064720: 293a 0d0a 0909 2727 2754 6869 7320 6973  ):....'''This is
+00064730: 2061 2063 6f6e 7665 6e69 656e 6365 2066   a convenience f
+00064740: 756e 6374 696f 6e20 746f 2070 6c6f 7420  unction to plot 
+00064750: 6d75 6c74 6970 6c65 2065 7874 7261 6374  multiple extract
+00064760: 6564 2073 7065 6374 7261 200d 0a09 0928  ed spectra ....(
+00064770: 4441 5320 6f72 2073 7065 6369 6573 2061  DAS or species a
+00064780: 7373 6f63 6961 7465 6429 2069 6e74 6f20  ssociated) into 
+00064790: 7468 6520 7361 6d65 2066 6967 7572 6520  the same figure 
+000647a0: 6f72 2069 6e74 6f20 6120 7365 7061 7261  or into a separa
+000647b0: 7465 2066 6967 7572 650d 0a09 0965 6163  te figure....eac
+000647c0: 682e 204f 7468 6572 2073 686f 756c 6420  h. Other should 
+000647d0: 6265 2074 612e 706c 6f74 5f66 756e 6320  be ta.plot_func 
+000647e0: 6f62 6a65 6374 7320 286c 6f61 6465 6420  objects (loaded 
+000647f0: 6f72 2063 6f70 6965 6429 2e20 4279 0d0a  or copied). By..
+00064800: 0909 7374 616e 6461 7264 2069 7420 706c  ..standard it pl
+00064810: 6f74 7320 616c 6c20 696e 746f 2074 6865  ots all into the
+00064820: 2073 616d 6520 7769 6e64 6f77 2e20 4966   same window. If
+00064830: 2061 6c6c 2070 726f 6a65 6374 2068 6176   all project hav
+00064840: 6520 7468 6520 7361 6d65 0d0a 0909 6e75  e the same....nu
+00064850: 6d62 6572 206f 6620 636f 6d70 6f6e 656e  mber of componen
+00064860: 7473 206f 6e65 2063 616e 2061 6374 6976  ts one can activ
+00064870: 6174 6520 2273 6570 6172 6174 655f 706c  ate "separate_pl
+00064880: 6f74 7322 2061 6e64 2068 6176 6520 6561  ots" and have ea
+00064890: 6368 0d0a 0909 7365 7061 7261 7465 6420  ch....separated 
+000648a0: 2869 6e20 7468 6520 6f72 6465 7220 6372  (in the order cr
+000648b0: 6561 7465 6420 696e 2074 6865 2070 726f  eated in the pro
+000648c0: 6a65 6374 7329 2e0d 0a0d 0a09 0954 6865  jects).......The
+000648d0: 2022 5370 6563 7472 6122 2070 6172 616d   "Spectra" param
+000648e0: 6574 6572 2061 6c6c 6f77 7320 6173 2062  eter allows as b
+000648f0: 6566 6f72 6520 7468 6520 696e 636c 7573  efore the inclus
+00064900: 696f 6e20 6f66 2061 6e20 6578 7465 726e  ion of an extern
+00064910: 616c 0d0a 0909 7370 6563 7472 756d 2e20  al....spectrum. 
+00064920: 4f74 6865 7273 2069 7320 6f70 7469 6f6e  Others is option
+00064930: 616c 2061 6e64 2049 2075 7365 2074 6869  al and I use thi
+00064940: 7320 6675 6e63 7469 6f6e 206f 6674 656e  s function often
+00064950: 2074 6f20 636f 6d70 6172 650d 0a09 0973   to compare....s
+00064960: 7065 6369 6573 2061 7373 6f63 6961 7465  pecies associate
+00064970: 6420 7370 6563 7472 6120 7769 7468 206f  d spectra with o
+00064980: 6e65 206f 7220 6d75 6c74 6970 6c65 2073  ne or multiple s
+00064990: 7465 6164 7920 7374 6174 6520 7370 6563  teady state spec
+000649a0: 7472 612e 0d0a 0909 0d0a 0909 5061 7261  tra.........Para
+000649b0: 6d65 7465 7273 0d0a 0909 2d2d 2d2d 2d2d  meters....------
+000649c0: 2d2d 2d2d 2d2d 2d2d 0d0a 0909 090d 0a09  --------........
+000649d0: 096f 7468 6572 203a 2054 4120 6f62 6a65  .other : TA obje
+000649e0: 6374 206f 7220 6c69 7374 206f 6620 7468  ct or list of th
+000649f0: 6f73 652c 206f 7074 696f 6e61 6c20 0d0a  ose, optional ..
+00064a00: 0909 0973 686f 756c 6420 6265 2074 612e  ...should be ta.
+00064a10: 706c 6f74 5f66 756e 6320 6f62 6a65 6374  plot_func object
+00064a20: 7320 286c 6f61 6465 6420 6f72 2063 6f70  s (loaded or cop
+00064a30: 6965 6429 2061 6e64 2069 7320 7768 6174  ied) and is what
+00064a40: 200d 0a09 0909 6973 2070 6c6f 7474 6564   .....is plotted
+00064a50: 2061 6761 696e 7374 2074 6865 2064 6174   against the dat
+00064a60: 6120 7573 6520 6120 6c69 7374 205b 7461  a use a list [ta
+00064a70: 312c 7461 322c 2e2e 2e20 5d20 6f72 2067  1,ta2,... ] or g
+00064a80: 656e 6572 6174 6520 7468 6973 0d0a 0909  enerate this....
+00064a90: 096c 6973 7420 7573 696e 6720 7468 6520  .list using the 
+00064aa0: 4775 6920 6675 6e63 7469 6f6e 2e20 5365  Gui function. Se
+00064ab0: 6520 7365 6374 696f 6e20 3a72 6566 3a60  e section :ref:`
+00064ac0: 4f70 656e 696e 6720 6d75 6c74 6970 6c65  Opening multiple
+00064ad0: 2066 696c 6573 6020 696e 200d 0a09 0909   files` in .....
+00064ae0: 7468 6520 646f 6375 6d65 6e74 6174 696f  the documentatio
+00064af0: 6e0d 0a0d 0a09 0973 7065 6374 7261 203a  n......spectra :
+00064b00: 204e 6f6e 6520 6f72 2044 6174 6146 7261   None or DataFra
+00064b10: 6d65 2c20 6f70 7469 6f6e 616c 0d0a 0909  me, optional....
+00064b20: 0949 6620 616e 2044 6174 6146 7261 6d65  .If an DataFrame
+00064b30: 2077 6974 6820 7468 6520 7761 7665 6c65   with the wavele
+00064b40: 6e67 7468 2061 7320 696e 6465 7820 6973  ngth as index is
+00064b50: 2070 726f 7669 6465 642c 2054 6865 6e20   provided, Then 
+00064b60: 7468 6520 7370 6563 7472 6120 6f66 2065  the spectra of e
+00064b70: 6163 6820 636f 6c75 6d6e 0d0a 0909 0969  ach column.....i
+00064b80: 7320 706c 6f74 7465 6420 696e 746f 2074  s plotted into t
+00064b90: 6865 2064 6966 6665 7265 6e74 6961 6c20  he differential 
+00064ba0: 7370 6563 7472 6120 313a 3120 616e 6420  spectra 1:1 and 
+00064bb0: 7468 6520 636f 6c75 6d6e 206e 616d 6573  the column names
+00064bc0: 2061 7265 2075 7365 6420 696e 2074 6865   are used in the
+00064bd0: 206c 6567 656e 640d 0a09 0909 5072 696f   legend.....Prio
+00064be0: 7220 7363 616c 696e 6720 6973 2068 6967  r scaling is hig
+00064bf0: 686c 7920 7375 6767 6573 7465 642e 2054  hly suggested. T
+00064c00: 6865 7365 2073 7065 6374 7261 2061 7265  hese spectra are
+00064c10: 206e 6f74 2028 696e 2067 656e 6572 616c   not (in general
+00064c20: 2920 7363 616c 6564 2077 6974 6820 7468  ) scaled with th
+00064c30: 6520 0d0a 0909 096e 6f72 6d20 7769 6e64  e .....norm wind
+00064c40: 6f77 2e20 2873 6565 2065 7861 6d70 6c65  ow. (see example
+00064c50: 7329 0d0a 0d0a 0909 7365 7061 7261 7465  s)......separate
+00064c60: 5f70 6c6f 7473 203a 2062 6f6f 6c2c 206f  _plots : bool, o
+00064c70: 7074 696f 6e61 6c0d 0a09 0909 5472 7565  ptional.....True
+00064c80: 206f 7220 4661 6c73 6520 2844 6566 6175   or False (Defau
+00064c90: 6c74 292c 2073 6570 6172 6174 6520 706c  lt), separate pl
+00064ca0: 6f74 7320 6973 2074 6865 2073 7769 7463  ots is the switc
+00064cb0: 6820 7468 6174 2064 6563 6964 6573 2069  h that decides i
+00064cc0: 6620 6120 6178 6973 206f 7220 0d0a 0909  f a axis or ....
+00064cd0: 096d 756c 7469 706c 6520 6178 6973 2061  .multiple axis a
+00064ce0: 7265 2075 7365 642e 2054 6869 7320 6f70  re used. This op
+00064cf0: 7469 6f6e 2077 696c 6c20 7265 7375 6c74  tion will result
+00064d00: 2069 6e20 6120 6372 6173 6820 756e 6c65   in a crash unle
+00064d10: 7373 2061 6c6c 206f 626a 6563 7473 2068  ss all objects h
+00064d20: 6176 6520 7468 650d 0a09 0909 7361 6d65  ave the.....same
+00064d30: 206e 756d 6265 7220 6f66 2044 4153 2f53   number of DAS/S
+00064d40: 4153 2063 6f6d 706f 6e65 6e74 730d 0a09  AS components...
+00064d50: 0909 090d 0a09 0963 6d61 7020 3a20 4e6f  .......cmap : No
+00064d60: 6e65 206f 7220 6d61 7470 6c6f 746c 6962  ne or matplotlib
+00064d70: 2063 6f6c 6f72 206d 6170 2c20 6f70 7469   color map, opti
+00064d80: 6f6e 616c 0d0a 0909 0969 7320 6120 706f  onal.....is a po
+00064d90: 7765 7266 756c 6c20 7661 7269 6162 6c65  werfull variable
+00064da0: 2074 6861 7420 6368 6f6f 7365 7320 7468   that chooses th
+00064db0: 6520 636f 6c6f 7572 206d 6170 2061 7070  e colour map app
+00064dc0: 6c69 6564 2066 6f72 2061 6c6c 2070 6c6f  lied for all plo
+00064dd0: 7473 2e20 4966 2073 6574 2074 6f20 0d0a  ts. If set to ..
+00064de0: 0909 094e 6f6e 6520 2844 6566 6175 6c74  ...None (Default
+00064df0: 2920 7468 656e 2074 6865 2073 656c 662e  ) then the self.
+00064e00: 636d 6170 2069 7320 7573 6564 2e0d 0a09  cmap is used....
+00064e10: 0909 4173 2073 7461 6e64 6172 6420 4920  ..As standard I 
+00064e20: 7573 6520 7468 6520 636f 6c6f 7220 6d61  use the color ma
+00064e30: 7020 226a 6574 2220 6672 6f6d 206d 6174  p "jet" from mat
+00064e40: 706c 6f74 6c69 622e 2054 6865 7265 2061  plotlib. There a
+00064e50: 7265 2061 2076 6172 6965 7479 206f 6620  re a variety of 
+00064e60: 636f 6c6f 726d 6170 7320 0d0a 0909 0961  colormaps .....a
+00064e70: 7661 696c 6162 6c65 2074 6861 7420 6172  vailable that ar
+00064e80: 6520 7665 7279 2075 7365 6675 6c6c 2e20  e very usefull. 
+00064e90: 4265 7369 6465 2022 6a65 7422 2c20 2276  Beside "jet", "v
+00064ea0: 6972 6964 6973 2220 6973 2061 2067 6f6f  iridis" is a goo
+00064eb0: 6420 6368 6f69 6365 2061 7320 6974 2069  d choice as it i
+00064ec0: 7320 7765 6c6c 200d 0a09 0909 7669 7369  s well .....visi
+00064ed0: 626c 6520 756e 6465 7220 7265 642d 6772  ble under red-gr
+00064ee0: 6565 6e20 626c 696e 646e 6573 732e 204f  een blindness. O
+00064ef0: 7468 6572 2075 7365 6675 6c20 6d61 7073  ther useful maps
+00064f00: 2061 7265 2022 7072 6973 6d22 2066 6f72   are "prism" for
+00064f10: 2068 6967 6820 666c 7563 7475 6174 696f   high fluctuatio
+00064f20: 6e73 200d 0a09 0909 6f72 2064 6976 6572  ns .....or diver
+00064f30: 6769 6e67 2063 6f6c 6f72 206d 6170 7320  ging color maps 
+00064f40: 6c69 6b65 2022 7365 6973 6d69 6322 2e20  like "seismic". 
+00064f50: 0d0a 0909 0953 6565 2068 7474 7073 3a2f  .....See https:/
+00064f60: 2f6d 6174 706c 6f74 6c69 622e 6f72 672f  /matplotlib.org/
+00064f70: 332e 312e 302f 7475 746f 7269 616c 732f  3.1.0/tutorials/
+00064f80: 636f 6c6f 7273 2f63 6f6c 6f72 6d61 7073  colors/colormaps
+00064f90: 2e68 746d 6c20 666f 7220 6120 636f 6d70  .html for a comp
+00064fa0: 7265 6865 6e73 6976 6520 0d0a 0909 0973  rehensive .....s
+00064fb0: 656c 6563 7469 6f6e 2e20 496e 2074 6865  election. In the
+00064fc0: 2063 6f64 6520 7468 6520 636f 6c6f 726d   code the colorm
+00064fd0: 6170 7320 6172 6520 696d 706f 7274 6564  aps are imported
+00064fe0: 2073 6f20 6966 2070 6c6f 745f 6675 6e63   so if plot_func
+00064ff0: 2069 7320 696d 706f 7274 6564 2061 7320   is imported as 
+00065000: 7066 2074 6865 6e20 0d0a 0909 0973 656c  pf then .....sel
+00065010: 662e 636d 6170 3d70 662e 636d 2e76 6972  f.cmap=pf.cm.vir
+00065020: 6964 6973 2073 6574 7320 7669 7269 6469  idis sets viridi
+00065030: 7320 6173 2074 6865 206d 6170 2074 6f20  s as the map to 
+00065040: 7573 652e 2049 6e74 6572 6e61 6c6c 7920  use. Internally 
+00065050: 7468 6520 636f 6c6f 7273 2061 7265 2063  the colors are c
+00065060: 686f 7365 6e20 0d0a 0909 0977 6974 6820  hosen .....with 
+00065070: 7468 6520 2263 6f6c 6d22 2066 756e 6374  the "colm" funct
+00065080: 696f 6e2e 2054 6865 2032 6420 706c 6f74  ion. The 2d plot
+00065090: 7320 7265 7175 6972 6520 6120 636f 6e74  s require a cont
+000650a0: 696e 756f 7573 2063 6f6c 6f72 206d 6170  inuous color map
+000650b0: 2073 6f20 6966 2073 6f6d 6574 6869 6e67   so if something
+000650c0: 200d 0a09 0909 656c 7365 2069 7320 6769   .....else is gi
+000650d0: 7665 2032 6420 706c 6f74 7320 6172 6520  ve 2d plots are 
+000650e0: 7368 6f77 6e20 6175 746f 6d61 7469 6361  shown automatica
+000650f0: 6c6c 7920 7769 7468 2022 6a65 7422 2e20  lly with "jet". 
+00065100: 466f 7220 616c 6c20 6f66 2074 6865 2031  For all of the 1
+00065110: 6420 706c 6f74 7320 686f 7765 7665 7220  d plots however 
+00065120: 0d0a 0909 0949 2066 6972 7374 2073 656c  .....I first sel
+00065130: 6563 7420 6120 6e75 6d62 6572 206f 6620  ect a number of 
+00065140: 636f 6c6f 7273 2062 6566 6f72 6520 6561  colors before ea
+00065150: 6368 2070 6c6f 742e 2049 6620 636d 6170  ch plot. If cmap
+00065160: 2069 7320 6120 636f 6e74 696e 6f75 7320   is a continous 
+00065170: 6d61 7020 7468 656e 2074 6865 7365 0d0a  map then these..
+00065180: 0909 0961 7265 2073 616d 706c 6564 2065  ...are sampled e
+00065190: 7665 6e6c 7920 6f76 6572 2074 6865 2063  venly over the c
+000651a0: 6f6c 6f75 726d 6170 2e20 4d61 6e75 616c  olourmap. Manual
+000651b0: 2069 7465 7261 626c 6573 206f 6620 636f   iterables of co
+000651c0: 6c6f 7572 7320 0d0a 0909 0963 6d61 703d  lours .....cmap=
+000651d0: 5b28 312c 302c 3029 2c28 302c 312c 3029  [(1,0,0),(0,1,0)
+000651e0: 2c28 302c 302c 3129 2c2e 2e2e 5d20 6172  ,(0,0,1),...] ar
+000651f0: 6520 616c 736f 2061 6363 6570 7465 642c  e also accepted,
+00065200: 2061 7320 6172 6520 7665 6374 6f72 7320   as are vectors 
+00065210: 6f72 2064 6174 6166 7261 6d65 7320 7468  or dataframes th
+00065220: 6174 200d 0a09 0909 636f 6e74 6169 6e20  at .....contain 
+00065230: 6173 2072 6f77 7320 7468 6520 636f 6c6f  as rows the colo
+00065240: 7273 2e20 5468 6572 6520 6d75 7374 2062  rs. There must b
+00065250: 6520 6f66 2063 6f75 7273 6520 7375 6666  e of course suff
+00065260: 6963 6965 6e74 2063 6f6c 6f72 7320 7072  icient colors pr
+00065270: 6573 656e 7420 666f 7220 0d0a 0909 0974  esent for .....t
+00065280: 6865 206e 756d 6265 7273 206f 6620 6c69  he numbers of li
+00065290: 6e65 7320 7468 6174 2077 696c 6c20 6265  nes that will be
+000652a0: 2070 6c6f 7474 6564 2e20 536f 2049 2072   plotted. So I r
+000652b0: 6563 6f6d 6d65 6e64 2074 6f20 7072 6f76  ecommend to prov
+000652c0: 6964 6520 6174 206c 6561 7374 2031 3020  ide at least 10 
+000652d0: 636f 6c6f 7572 7320 0d0a 0909 0928 652e  colours .....(e.
+000652e0: 672e 7e79 6f75 7220 756e 6976 6572 7369  g.~your universi
+000652f0: 7479 2063 6f6c 6f72 7329 2e20 636f 6c6f  ty colors). colo
+00065300: 7572 7320 6172 6520 616c 7761 7973 2067  urs are always g
+00065310: 6976 656e 2061 7320 612c 206c 6973 7420  iven as a, list 
+00065320: 6f72 2074 7570 6c65 2077 6974 6820 5247  or tuple with RG
+00065330: 4120 6f72 2052 4742 410d 0a09 0909 2877  A or RGBA.....(w
+00065340: 6974 6820 7468 6520 6c61 7374 2041 2062  ith the last A b
+00065350: 6565 696e 6720 7468 6520 416c 7068 613d  eeing the Alpha=
+00065360: 7472 616e 7370 6172 656e 6379 2e20 416c  transparency. Al
+00065370: 6c20 6e75 6d62 6572 7320 6172 6520 6265  l numbers are be
+00065380: 7477 6565 6e20 3020 616e 6420 312e 200d  tween 0 and 1. .
+00065390: 0a09 0909 4966 2061 206c 6973 742f 7665  ....If a list/ve
+000653a0: 6374 6f72 2f44 6174 6146 7261 6d65 2069  ctor/DataFrame i
+000653b0: 7320 6769 7665 6e20 666f 7220 7468 6520  s given for the 
+000653c0: 636f 6c6f 7572 7320 7468 6579 2077 696c  colours they wil
+000653d0: 6c20 6265 2075 7365 6420 696e 2074 6865  l be used in the
+000653e0: 206f 7264 6572 2070 726f 7669 6465 642e   order provided.
+000653f0: 0d0a 0909 0d0a 0909 4578 616d 706c 6573  ........Examples
+00065400: 0d0a 0909 2d2d 2d2d 2d2d 2d2d 0d0a 0909  ....--------....
+00065410: 0d0a 0909 3e3e 3e20 696d 706f 7274 2070  ....>>> import p
+00065420: 6c6f 745f 6675 6e63 2061 7320 7066 0d0a  lot_func as pf..
+00065430: 0909 3e3e 3e20 7461 203d 2070 662e 5441  ..>>> ta = pf.TA
+00065440: 2827 7465 7374 312e 6864 6635 2729 2023  ('test1.hdf5') #
+00065450: 6f70 656e 2074 6865 206f 7269 6769 6e61  open the origina
+00065460: 6c20 7072 6f6a 6563 742c 200d 0a09 093e  l project, ....>
+00065470: 3e3e 2074 6869 7320 4d55 5354 2063 6f6e  >> this MUST con
+00065480: 7461 696e 2061 2066 6974 2c20 6f74 6865  tain a fit, othe
+00065490: 7277 6973 6520 7468 6973 2077 696c 6c20  rwise this will 
+000654a0: 7261 6973 6520 616e 2065 7272 6f72 0d0a  raise an error..
+000654b0: 0909 0d0a 0909 4e6f 7720 6f70 656e 2061  ......Now open a
+000654c0: 2062 756e 6368 206f 6620 6f74 6865 7220   bunch of other 
+000654d0: 7072 6f6a 6563 7473 2074 6f20 636f 6d70  projects to comp
+000654e0: 6172 6520 6167 6169 6e73 742c 0d0a 0909  are against,....
+000654f0: 0d0a 0909 3e3e 3e20 2363 6f6d 7061 7265  ....>>> #compare
+00065500: 2069 6e20 6120 7369 6e67 6c65 2077 696e   in a single win
+00065510: 646f 770d 0a09 093e 3e3e 206f 7468 6572  dow....>>> other
+00065520: 5f70 726f 6a65 6374 7320 3d20 7066 2e47  _projects = pf.G
+00065530: 5549 5f6f 7065 6e28 7072 6f6a 6563 745f  UI_open(project_
+00065540: 6c69 7374 203d 205b 2766 696c 6531 2e68  list = ['file1.h
+00065550: 6466 3527 2c20 2766 696c 6532 2e68 6466  df5', 'file2.hdf
+00065560: 3527 5d29 0d0a 0909 3e3e 3e20 7461 2e43  5'])....>>> ta.C
+00065570: 6f6d 7061 7265 5f44 4143 286f 7468 6572  ompare_DAC(other
+00065580: 7320 3d20 6f74 6865 725f 7072 6f6a 6563  s = other_projec
+00065590: 7429 0d0a 0909 3e3e 3e20 2363 6f6d 7072  t)....>>> #compr
+000655a0: 6172 6520 696e 2073 6570 6172 6174 6520  are in separate 
+000655b0: 7769 6e64 6f77 732c 200d 0a09 093e 3e3e  windows, ....>>>
+000655c0: 2023 7468 6520 6f74 6865 7220 7072 6f6a   #the other proj
+000655d0: 6563 7473 206d 7573 7420 6861 7665 2074  ects must have t
+000655e0: 6865 2073 616d 6520 6e75 6d62 6572 206f  he same number o
+000655f0: 6620 636f 6d70 6f6e 656e 7473 0d0a 0909  f components....
+00065600: 3e3e 3e20 7461 2e43 6f6d 7061 7265 5f44  >>> ta.Compare_D
+00065610: 4143 286f 7468 6572 7320 3d20 6f74 6865  AC(others = othe
+00065620: 725f 7072 6f6a 6563 742c 2073 6570 6172  r_project, separ
+00065630: 6174 655f 706c 6f74 7320 3d20 5472 7565  ate_plots = True
+00065640: 290d 0a09 090d 0a09 0943 6f6d 7061 7265  )........Compare
+00065650: 2074 6865 2044 4143 2074 6f20 616e 2065   the DAC to an e
+00065660: 7874 6572 6e61 6c20 7370 6563 7472 756d  xternal spectrum
+00065670: 0d0a 0909 0d0a 0909 3e3e 3e20 6578 745f  ........>>> ext_
+00065680: 7370 6563 203d 2070 642e 7265 6164 5f63  spec = pd.read_c
+00065690: 7376 2827 4173 6369 695f 7370 6563 7472  sv('Ascii_spectr
+000656a0: 756d 2e64 6174 272c 2073 6570 203d 2027  um.dat', sep = '
+000656b0: 2c27 290d 0a09 093e 3e3e 2074 612e 436f  ,')....>>> ta.Co
+000656c0: 6d70 6172 655f 4441 4328 7370 6563 7472  mpare_DAC(spectr
+000656d0: 6120 3d20 6578 745f 7370 6563 2920 2363  a = ext_spec) #c
+000656e0: 6f6d 7061 7265 206a 7573 7420 7468 6520  ompare just the 
+000656f0: 6375 7272 656e 7420 736f 6c75 7469 6f6e  current solution
+00065700: 0d0a 0909 3e3e 3e20 7461 2e43 6f6d 7061  ....>>> ta.Compa
+00065710: 7265 5f44 4143 2873 7065 6374 7261 203d  re_DAC(spectra =
+00065720: 2065 7874 5f73 7065 632c 206f 7468 6572   ext_spec, other
+00065730: 7320 3d20 6f74 6865 725f 7072 6f6a 6563  s = other_projec
+00065740: 7429 2023 636f 6d70 6172 6520 6d75 6c74  t) #compare mult
+00065750: 6970 6c65 0d0a 0909 0d0a 0909 2727 270d  iple........'''.
+00065760: 0a09 090d 0a09 0969 6620 7365 6c66 2e73  .......if self.s
+00065770: 6176 655f 6669 6775 7265 735f 746f 5f66  ave_figures_to_f
+00065780: 6f6c 6465 723a 7365 6c66 2e66 6967 7572  older:self.figur
+00065790: 655f 7061 7468 203d 2063 6865 636b 5f66  e_path = check_f
+000657a0: 6f6c 6465 7228 7061 7468 203d 2027 7265  older(path = 're
+000657b0: 7375 6c74 5f66 6967 7572 6573 272c 2063  sult_figures', c
+000657c0: 7572 7265 6e74 5f70 6174 6820 3d20 7365  urrent_path = se
+000657d0: 6c66 2e70 6174 6829 0d0a 0909 6966 206f  lf.path)....if o
+000657e0: 7468 6572 2069 7320 6e6f 7420 4e6f 6e65  ther is not None
+000657f0: 3a0d 0a09 0909 6966 206e 6f74 2068 6173  :.....if not has
+00065800: 6174 7472 286f 7468 6572 2c20 275f 5f69  attr(other, '__i
+00065810: 7465 725f 5f27 293a 6f74 6865 7220 3d20  ter__'):other = 
+00065820: 5b6f 7468 6572 5d0d 0a09 0974 7279 3a0d  [other]....try:.
+00065830: 0a09 0909 7265 203d 2073 656c 662e 7265  ....re = self.re
+00065840: 2e63 6f70 7928 290d 0a09 0965 7863 6570  .copy()....excep
+00065850: 743a 0d0a 0909 0970 7269 6e74 2822 4e6f  t:.....print("No
+00065860: 2066 6974 7465 6420 7265 7375 6c74 7320   fitted results 
+00065870: 7072 6573 656e 7422 290d 0a09 0909 7265  present").....re
+00065880: 7475 726e 2046 616c 7365 0d0a 0909 6966  turn False....if
+00065890: 2063 6d61 7020 6973 204e 6f6e 653a 636d   cmap is None:cm
+000658a0: 6170 203d 2073 656c 662e 636d 6170 0d0a  ap = self.cmap..
+000658b0: 0909 7370 6563 6965 733d 7265 5b27 4441  ..species=re['DA
+000658c0: 4327 5d2e 636f 6c75 6d6e 732e 7661 6c75  C'].columns.valu
+000658d0: 6573 0d0a 0909 6966 206f 7468 6572 2069  es....if other i
+000658e0: 7320 4e6f 6e65 3a0d 0a09 0909 636f 6c20  s None:.....col 
+000658f0: 3d20 7261 6e67 6528 6c65 6e28 7265 5b27  = range(len(re['
+00065900: 4441 4327 5d2e 636f 6c75 6d6e 732e 7661  DAC'].columns.va
+00065910: 6c75 6573 2929 0d0a 0909 0963 6f6c 6f72  lues)).....color
+00065920: 7320 3d20 636f 6c6d 2863 6d61 7020 3d20  s = colm(cmap = 
+00065930: 636d 6170 2c20 6b20 3d20 636f 6c29 0d0a  cmap, k = col)..
+00065940: 0909 090d 0a09 0965 6c73 653a 0d0a 0909  .......else:....
+00065950: 0972 655b 2744 4143 275d 2e63 6f6c 756d  .re['DAC'].colum
+00065960: 6e73 203d 205b 7365 6c66 2e66 696c 656e  ns = [self.filen
+00065970: 616d 6520 2b20 275c 6e27 202b 2027 2573  ame + '\n' + '%s
+00065980: 2725 6120 666f 7220 6120 696e 2072 655b  '%a for a in re[
+00065990: 2744 4143 275d 2e63 6f6c 756d 6e73 5d0d  'DAC'].columns].
+000659a0: 0a09 0909 6966 2073 6570 6172 6174 655f  ....if separate_
+000659b0: 706c 6f74 733a 0d0a 0909 0909 636f 6c6f  plots:......colo
+000659c0: 7273 203d 2063 6f6c 6d28 636d 6170 203d  rs = colm(cmap =
+000659d0: 2063 6d61 702c 206b 203d 206e 702e 6172   cmap, k = np.ar
+000659e0: 616e 6765 286c 656e 286f 7468 6572 292b  ange(len(other)+
+000659f0: 3129 290d 0a09 0909 656c 7365 3a0d 0a09  1)).....else:...
+00065a00: 0909 0963 6f6c 6f72 7320 3d20 636f 6c6d  ...colors = colm
+00065a10: 2863 6d61 7020 3d20 636d 6170 2c20 6b20  (cmap = cmap, k 
+00065a20: 3d20 6e70 2e61 7261 6e67 6528 286c 656e  = np.arange((len
+00065a30: 286f 7468 6572 292b 3129 2a6c 656e 2873  (other)+1)*len(s
+00065a40: 7065 6369 6573 2929 290d 0a09 0944 4143  pecies)))....DAC
+00065a50: 203d 2072 655b 2744 4143 275d 0d0a 0909   = re['DAC']....
+00065a60: 6861 6e64 3d5b 5d0d 0a09 0969 6620 7365  hand=[]....if se
+00065a70: 7061 7261 7465 5f70 6c6f 7473 3a0d 0a09  parate_plots:...
+00065a80: 0909 6e5f 636f 6c73 203d 2069 6e74 286e  ..n_cols = int(n
+00065a90: 702e 6365 696c 286c 656e 2872 655b 2744  p.ceil(len(re['D
+00065aa0: 4143 275d 2e63 6f6c 756d 6e73 292f 3229  AC'].columns)/2)
+00065ab0: 290d 0a09 0909 636f 6c20 3d20 5b63 6f6c  ).....col = [col
+00065ac0: 6f72 735b 305d 2066 6f72 2061 2069 6e20  ors[0] for a in 
+00065ad0: 7261 6e67 6528 6c65 6e28 7265 5b27 4441  range(len(re['DA
+00065ae0: 4327 5d2e 636f 6c75 6d6e 7329 295d 0d0a  C'].columns))]..
+00065af0: 0909 0969 6620 7365 6c66 2e73 6361 7474  ...if self.scatt
+00065b00: 6572 6375 7420 6973 204e 6f6e 653a 090d  ercut is None:..
+00065b10: 0a09 0909 0961 7820 3d20 4441 432e 706c  .....ax = DAC.pl
+00065b20: 6f74 2873 7562 706c 6f74 7320 3d20 7365  ot(subplots = se
+00065b30: 7061 7261 7465 5f70 6c6f 7473 2c20 6669  parate_plots, fi
+00065b40: 6773 697a 6520 3d20 2831 322c 2031 3029  gsize = (12, 10)
+00065b50: 2c20 6c61 796f 7574 203d 2028 6e5f 636f  , layout = (n_co
+00065b60: 6c73 2c20 3229 2c20 0d0a 0909 0909 0909  ls, 2), ........
+00065b70: 0909 096c 6567 656e 6420 3d20 4661 6c73  ...legend = Fals
+00065b80: 652c 2063 6f6c 6f72 203d 2063 6f6c 2c20  e, color = col, 
+00065b90: 7368 6172 6578 203d 2046 616c 7365 290d  sharex = False).
+00065ba0: 0a0d 0a09 0909 0961 3d61 782e 7261 7665  .......a=ax.rave
+00065bb0: 6c28 290d 0a09 0909 0968 616e 646c 6573  l()......handles
+00065bc0: 2c6c 6162 656c 733d 615b 305d 2e67 6574  ,labels=a[0].get
+00065bd0: 5f6c 6567 656e 645f 6861 6e64 6c65 735f  _legend_handles_
+00065be0: 6c61 6265 6c73 2829 0d0a 0909 0909 6861  labels()......ha
+00065bf0: 6e64 2e61 7070 656e 6428 6861 6e64 6c65  nd.append(handle
+00065c00: 735b 2d31 5d29 0d0a 0909 0965 6c69 6620  s[-1]).....elif 
+00065c10: 6973 696e 7374 616e 6365 2873 656c 662e  isinstance(self.
+00065c20: 7363 6174 7465 7263 7574 5b30 5d2c 2020  scattercut[0],  
+00065c30: 6e75 6d62 6572 732e 4e75 6d62 6572 293a  numbers.Number):
+00065c40: 0d0a 0909 0909 6178 203d 2044 4143 2e6c  ......ax = DAC.l
+00065c50: 6f63 5b3a 7365 6c66 2e73 6361 7474 6572  oc[:self.scatter
+00065c60: 6375 745b 305d 2c20 3a5d 2e70 6c6f 7428  cut[0], :].plot(
+00065c70: 7375 6270 6c6f 7473 203d 2073 6570 6172  subplots = separ
+00065c80: 6174 655f 706c 6f74 732c 2066 6967 7369  ate_plots, figsi
+00065c90: 7a65 203d 2028 3132 2c20 3130 292c 206c  ze = (12, 10), l
+00065ca0: 6179 6f75 7420 3d20 286e 5f63 6f6c 732c  ayout = (n_cols,
+00065cb0: 2032 292c 200d 0a09 0909 0909 0909 0909   2), ...........
+00065cc0: 0909 0909 6c65 6765 6e64 203d 2046 616c  ....legend = Fal
+00065cd0: 7365 2c20 636f 6c6f 7220 3d20 636f 6c2c  se, color = col,
+00065ce0: 2073 6861 7265 7820 3d20 4661 6c73 6529   sharex = False)
+00065cf0: 0909 0909 0909 0909 0d0a 0909 0909 613d  ..............a=
+00065d00: 6178 2e72 6176 656c 2829 0d0a 0909 0909  ax.ravel()......
+00065d10: 6861 6e64 6c65 732c 6c61 6265 6c73 3d61  handles,labels=a
+00065d20: 5b30 5d2e 6765 745f 6c65 6765 6e64 5f68  [0].get_legend_h
+00065d30: 616e 646c 6573 5f6c 6162 656c 7328 290d  andles_labels().
+00065d40: 0a09 0909 0968 616e 642e 6170 7065 6e64  .....hand.append
+00065d50: 2868 616e 646c 6573 5b2d 315d 2909 0d0a  (handles[-1])...
+00065d60: 0909 0909 4441 435f 6375 743d 4441 432e  ....DAC_cut=DAC.
+00065d70: 6c6f 635b 7365 6c66 2e73 6361 7474 6572  loc[self.scatter
+00065d80: 6375 745b 315d 3a2c 203a 5d0d 0a09 0909  cut[1]:, :].....
+00065d90: 0966 6f72 2069 2c61 6d20 696e 2065 6e75  .for i,am in enu
+00065da0: 6d65 7261 7465 2844 4143 5f63 7574 2e63  merate(DAC_cut.c
+00065db0: 6f6c 756d 6e73 293a 0d0a 0909 0909 0944  olumns):.......D
+00065dc0: 4143 5f63 7574 2e69 6c6f 635b 3a2c 695d  AC_cut.iloc[:,i]
+00065dd0: 2e70 6c6f 7428 6178 203d 2061 5b69 5d2c  .plot(ax = a[i],
+00065de0: 206c 6567 656e 6420 3d20 4661 6c73 652c   legend = False,
+00065df0: 2063 6f6c 6f72 203d 2063 6f6c 290d 0a09   color = col)...
+00065e00: 0909 656c 7365 3a0d 0a09 0909 0973 6361  ..else:......sca
+00065e10: 7474 6572 6375 7420 3d20 666c 6174 7465  ttercut = flatte
+00065e20: 6e28 7365 6c66 2e73 6361 7474 6572 6375  n(self.scattercu
+00065e30: 7429 0d0a 0909 0909 666f 7220 6920 696e  t)......for i in
+00065e40: 2072 616e 6765 286c 656e 2873 6361 7474   range(len(scatt
+00065e50: 6572 6375 7429 2f32 2b31 293a 0d0a 0909  ercut)/2+1):....
+00065e60: 0909 0969 6620 6920 3d3d 2030 3a0d 0a09  ...if i == 0:...
+00065e70: 0909 0909 0961 7820 3d20 4441 432e 6c6f  .....ax = DAC.lo
+00065e80: 635b 3a73 6361 7474 6572 6375 745b 305d  c[:scattercut[0]
+00065e90: 2c20 3a5d 2e70 6c6f 7428 7375 6270 6c6f  , :].plot(subplo
+00065ea0: 7473 203d 2073 6570 6172 6174 655f 706c  ts = separate_pl
+00065eb0: 6f74 732c 2066 6967 7369 7a65 203d 2028  ots, figsize = (
+00065ec0: 3132 2c20 3130 292c 200d 0a09 0909 0909  12, 10), .......
+00065ed0: 0909 0909 0909 0909 096c 6179 6f75 7420  .........layout 
+00065ee0: 3d20 286e 5f63 6f6c 732c 2032 292c 206c  = (n_cols, 2), l
+00065ef0: 6567 656e 6420 3d20 4661 6c73 652c 2063  egend = False, c
+00065f00: 6f6c 6f72 203d 2063 6f6c 2c20 7368 6172  olor = col, shar
+00065f10: 6578 203d 2046 616c 7365 290d 0a09 0909  ex = False).....
+00065f20: 0909 090d 0a09 0909 0909 0961 3d61 782e  ...........a=ax.
+00065f30: 7261 7665 6c28 290d 0a09 0909 0909 0968  ravel()........h
+00065f40: 616e 646c 6573 2c6c 6162 656c 733d 615b  andles,labels=a[
+00065f50: 305d 2e67 6574 5f6c 6567 656e 645f 6861  0].get_legend_ha
+00065f60: 6e64 6c65 735f 6c61 6265 6c73 2829 0d0a  ndles_labels()..
+00065f70: 0909 0909 0909 6861 6e64 2e61 7070 656e  ......hand.appen
+00065f80: 6428 6861 6e64 6c65 735b 2d31 5d29 090d  d(handles[-1])..
+00065f90: 0a09 0909 0909 656c 6966 2069 3c28 6c65  ......elif i<(le
+00065fa0: 6e28 7363 6174 7465 7263 7574 292f 3229  n(scattercut)/2)
+00065fb0: 3a0d 0a09 0909 0909 0966 6f72 206a 2c61  :........for j,a
+00065fc0: 6d20 696e 2065 6e75 6d65 7261 7465 2861  m in enumerate(a
+00065fd0: 7829 3a0d 0a09 0909 0909 0909 4441 432e  x):.........DAC.
+00065fe0: 6c6f 635b 7363 6174 7465 7263 7574 5b32  loc[scattercut[2
+00065ff0: 2a69 2d31 5d3a 7363 6174 7465 7263 7574  *i-1]:scattercut
+00066000: 5b32 2a69 5d2c 203a 5d2e 706c 6f74 2861  [2*i], :].plot(a
+00066010: 7820 3d20 615b 6a5d 2c20 6c65 6765 6e64  x = a[j], legend
+00066020: 203d 2046 616c 7365 2c20 636f 6c6f 7220   = False, color 
+00066030: 3d20 636f 6c2c 206c 6162 656c 203d 2027  = col, label = '
+00066040: 5f6e 6f6c 6567 656e 645f 2729 0d0a 0909  _nolegend_')....
+00066050: 0909 0965 6c73 653a 0d0a 0909 0909 0909  ...else:........
+00066060: 666f 7220 6a2c 616d 2069 6e20 656e 756d  for j,am in enum
+00066070: 6572 6174 6528 6178 293a 0d0a 0909 0909  erate(ax):......
+00066080: 0909 0944 4143 2e6c 6f63 5b73 6361 7474  ...DAC.loc[scatt
+00066090: 6572 6375 745b 2d31 5d3a 2c20 3a5d 2e70  ercut[-1]:, :].p
+000660a0: 6c6f 7428 6178 203d 2061 5b6a 5d2c 206c  lot(ax = a[j], l
+000660b0: 6567 656e 6420 3d20 4661 6c73 652c 2063  egend = False, c
+000660c0: 6f6c 6f72 203d 2063 6f6c 2c20 6c61 6265  olor = col, labe
+000660d0: 6c20 3d20 275f 6e6f 6c65 6765 6e64 5f27  l = '_nolegend_'
+000660e0: 290d 0a09 0965 6c73 653a 0d0a 0909 0969  )....else:.....i
+000660f0: 6620 7365 6c66 2e73 6361 7474 6572 6375  f self.scattercu
+00066100: 7420 6973 204e 6f6e 653a 090d 0a09 0909  t is None:......
+00066110: 0961 7820 203d 2020 4441 432e 706c 6f74  .ax  =  DAC.plot
+00066120: 2873 7562 706c 6f74 7320 3d20 7365 7061  (subplots = sepa
+00066130: 7261 7465 5f70 6c6f 7473 2c20 6669 6773  rate_plots, figs
+00066140: 697a 6520 3d20 2831 362c 2038 292c 206c  ize = (16, 8), l
+00066150: 6567 656e 6420 3d20 4661 6c73 652c 2063  egend = False, c
+00066160: 6f6c 6f72 203d 2063 6f6c 6f72 735b 3a6c  olor = colors[:l
+00066170: 656e 2873 7065 6369 6573 295d 2c20 6c61  en(species)], la
+00066180: 6265 6c20 3d20 275f 6e6f 6c65 6765 6e64  bel = '_nolegend
+00066190: 5f27 290d 0a09 0909 656c 6966 2069 7369  _').....elif isi
+000661a0: 6e73 7461 6e63 6528 7365 6c66 2e73 6361  nstance(self.sca
+000661b0: 7474 6572 6375 745b 305d 2c20 6e75 6d62  ttercut[0], numb
+000661c0: 6572 732e 4e75 6d62 6572 293a 0d0a 0909  ers.Number):....
+000661d0: 0909 6178 2020 3d20 2044 4143 2e6c 6f63  ..ax  =  DAC.loc
+000661e0: 5b3a 7365 6c66 2e73 6361 7474 6572 6375  [:self.scattercu
+000661f0: 745b 305d 2c20 3a5d 2e70 6c6f 7428 7375  t[0], :].plot(su
+00066200: 6270 6c6f 7473 203d 2073 6570 6172 6174  bplots = separat
+00066210: 655f 706c 6f74 732c 2066 6967 7369 7a65  e_plots, figsize
+00066220: 203d 2028 3136 2c20 3829 2c20 6c65 6765   = (16, 8), lege
+00066230: 6e64 203d 2046 616c 7365 2c20 636f 6c6f  nd = False, colo
+00066240: 7220 3d20 636f 6c6f 7273 5b3a 6c65 6e28  r = colors[:len(
+00066250: 7370 6563 6965 7329 5d2c 206c 6162 656c  species)], label
+00066260: 203d 2027 5f6e 6f6c 6567 656e 645f 2729   = '_nolegend_')
+00066270: 0d0a 0909 0909 6178 2020 3d20 2044 4143  ......ax  =  DAC
+00066280: 2e6c 6f63 5b73 656c 662e 7363 6174 7465  .loc[self.scatte
+00066290: 7263 7574 5b31 5d3a 2c20 203a 5d2e 706c  rcut[1]:,  :].pl
+000662a0: 6f74 2861 783d 6178 2c20 7375 6270 6c6f  ot(ax=ax, subplo
+000662b0: 7473 203d 2073 6570 6172 6174 655f 706c  ts = separate_pl
+000662c0: 6f74 732c 2066 6967 7369 7a65 203d 2028  ots, figsize = (
+000662d0: 3136 2c20 3829 2c20 6c65 6765 6e64 203d  16, 8), legend =
+000662e0: 2046 616c 7365 2c20 636f 6c6f 7220 3d20   False, color = 
+000662f0: 636f 6c6f 7273 5b3a 6c65 6e28 7370 6563  colors[:len(spec
+00066300: 6965 7329 5d2c 206c 6162 656c 203d 2027  ies)], label = '
+00066310: 5f6e 6f6c 6567 656e 645f 2729 0d0a 0909  _nolegend_')....
+00066320: 0965 6c73 653a 0d0a 0909 0909 7363 6174  .else:......scat
+00066330: 7465 7263 7574 2020 3d20 2066 6c61 7474  tercut  =  flatt
+00066340: 656e 2873 656c 662e 7363 6174 7465 7263  en(self.scatterc
+00066350: 7574 290d 0a09 0909 0966 6f72 2069 2069  ut)......for i i
+00066360: 6e20 7261 6e67 6528 6c65 6e28 7363 6174  n range(len(scat
+00066370: 7465 7263 7574 292f 322b 3129 3a0d 0a09  tercut)/2+1):...
+00066380: 0909 0909 6966 2069 2020 3d3d 2020 303a  ....if i  ==  0:
+00066390: 0d0a 0909 0909 0909 6178 2020 3d20 2044  ........ax  =  D
+000663a0: 4143 2e6c 6f63 5b3a 7363 6174 7465 7263  AC.loc[:scatterc
+000663b0: 7574 5b30 5d2c 2020 3a5d 2e70 6c6f 7428  ut[0],  :].plot(
+000663c0: 7375 6270 6c6f 7473 203d 2073 6570 6172  subplots = separ
+000663d0: 6174 655f 706c 6f74 732c 2066 6967 7369  ate_plots, figsi
+000663e0: 7a65 203d 2028 3136 2c20 3829 2c20 6c65  ze = (16, 8), le
+000663f0: 6765 6e64 203d 2046 616c 7365 2c20 636f  gend = False, co
+00066400: 6c6f 7220 3d20 636f 6c6f 7273 5b3a 6c65  lor = colors[:le
+00066410: 6e28 7370 6563 6965 7329 5d2c 206c 6162  n(species)], lab
+00066420: 656c 203d 2027 5f6e 6f6c 6567 656e 645f  el = '_nolegend_
+00066430: 2729 0d0a 0909 0909 0965 6c69 6620 693c  ').......elif i<
+00066440: 286c 656e 2873 6361 7474 6572 6375 7429  (len(scattercut)
+00066450: 2f32 293a 0d0a 0909 0909 0909 6178 2020  /2):........ax  
+00066460: 3d20 2044 4143 2e6c 6f63 5b73 6361 7474  =  DAC.loc[scatt
+00066470: 6572 6375 745b 322a 692d 315d 3a73 6361  ercut[2*i-1]:sca
+00066480: 7474 6572 6375 745b 322a 695d 2c20 203a  ttercut[2*i],  :
+00066490: 5d2e 706c 6f74 2861 783d 6178 2c20 7375  ].plot(ax=ax, su
+000664a0: 6270 6c6f 7473 203d 2073 6570 6172 6174  bplots = separat
+000664b0: 655f 706c 6f74 732c 2066 6967 7369 7a65  e_plots, figsize
+000664c0: 203d 2028 3136 2c20 3829 2c20 6c65 6765   = (16, 8), lege
+000664d0: 6e64 203d 2046 616c 7365 2c20 636f 6c6f  nd = False, colo
+000664e0: 7220 3d20 636f 6c6f 7273 5b3a 6c65 6e28  r = colors[:len(
+000664f0: 7370 6563 6965 7329 5d2c 206c 6162 656c  species)], label
+00066500: 203d 2027 5f6e 6f6c 6567 656e 645f 2729   = '_nolegend_')
+00066510: 0d0a 0909 0909 0965 6c73 653a 0d0a 0909  .......else:....
+00066520: 0909 0909 6178 2020 3d20 2044 4143 2e6c  ....ax  =  DAC.l
+00066530: 6f63 5b73 6361 7474 6572 6375 745b 2d31  oc[scattercut[-1
+00066540: 5d3a 2c20 203a 5d2e 706c 6f74 2861 783d  ]:,  :].plot(ax=
+00066550: 6178 2c20 7375 6270 6c6f 7473 203d 2073  ax, subplots = s
+00066560: 6570 6172 6174 655f 706c 6f74 732c 2066  eparate_plots, f
+00066570: 6967 7369 7a65 203d 2028 3136 2c20 3829  igsize = (16, 8)
+00066580: 2c20 6c65 6765 6e64 203d 2046 616c 7365  , legend = False
+00066590: 2c20 636f 6c6f 7220 3d20 636f 6c6f 7273  , color = colors
+000665a0: 5b3a 6c65 6e28 7370 6563 6965 7329 5d2c  [:len(species)],
+000665b0: 206c 6162 656c 203d 2027 5f6e 6f6c 6567   label = '_noleg
+000665c0: 656e 645f 2729 0d0a 0909 6966 206f 7468  end_')....if oth
+000665d0: 6572 2069 7320 6e6f 7420 4e6f 6e65 3a0d  er is not None:.
+000665e0: 0a09 0909 666f 7220 692c 6f20 696e 2065  ....for i,o in e
+000665f0: 6e75 6d65 7261 7465 286f 7468 6572 293a  numerate(other):
+00066600: 0d0a 0909 0909 7472 793a 0d0a 0909 0909  ......try:......
+00066610: 0972 653d 6f2e 7265 2e63 6f70 7928 290d  .re=o.re.copy().
+00066620: 0a09 0909 0965 7863 6570 743a 0d0a 0909  .....except:....
+00066630: 0909 0970 7269 6e74 2827 2573 2068 6173  ...print('%s has
+00066640: 206e 6f20 6669 7474 6564 2072 6573 756c   no fitted resul
+00066650: 7473 2725 6f2e 6669 6c65 6e61 6d65 290d  ts'%o.filename).
+00066660: 0a09 0909 0909 636f 6e74 696e 7565 0d0a  ......continue..
+00066670: 0909 0909 7265 5b27 4441 4327 5d2e 636f  ....re['DAC'].co
+00066680: 6c75 6d6e 733d 5b6f 2e66 696c 656e 616d  lumns=[o.filenam
+00066690: 6520 2b20 275c 6e27 202b 2027 2573 2725  e + '\n' + '%s'%
+000666a0: 6120 666f 7220 6120 696e 2072 655b 2744  a for a in re['D
+000666b0: 4143 275d 2e63 6f6c 756d 6e73 5d0d 0a09  AC'].columns]...
+000666c0: 0909 0969 6620 7365 7061 7261 7465 5f70  ...if separate_p
+000666d0: 6c6f 7473 3a09 0909 090d 0a09 0909 0909  lots:...........
+000666e0: 636f 6c3d 5b63 6f6c 6f72 735b 692b 315d  col=[colors[i+1]
+000666f0: 2066 6f72 2061 2069 6e20 7261 6e67 6528   for a in range(
+00066700: 6c65 6e28 7265 5b27 4441 4327 5d2e 636f  len(re['DAC'].co
+00066710: 6c75 6d6e 7329 295d 0d0a 0909 0909 0966  lumns))].......f
+00066720: 6f72 206a 2c61 6d20 696e 2065 6e75 6d65  or j,am in enume
+00066730: 7261 7465 2872 655b 2744 4143 275d 2e63  rate(re['DAC'].c
+00066740: 6f6c 756d 6e73 293a 0d0a 0909 0909 0909  olumns):........
+00066750: 6966 206f 2e73 6361 7474 6572 6375 7420  if o.scattercut 
+00066760: 6973 204e 6f6e 653a 090d 0a09 0909 0909  is None:........
+00066770: 0909 7265 5b27 4441 4327 5d2e 696c 6f63  ..re['DAC'].iloc
+00066780: 5b3a 2c6a 5d2e 706c 6f74 2873 7562 706c  [:,j].plot(subpl
+00066790: 6f74 733d 4661 6c73 652c 6178 3d61 5b6a  ots=False,ax=a[j
+000667a0: 5d2c 6c65 6765 6e64 3d46 616c 7365 2c63  ],legend=False,c
+000667b0: 6f6c 6f72 3d63 6f6c 5b69 5d29 0d0a 0909  olor=col[i])....
+000667c0: 0909 0909 0969 6620 6a3d 3d30 3a0d 0a09  .....if j==0:...
+000667d0: 0909 0909 0909 0968 616e 646c 6573 2c6c  .......handles,l
+000667e0: 6162 656c 733d 615b 305d 2e67 6574 5f6c  abels=a[0].get_l
+000667f0: 6567 656e 645f 6861 6e64 6c65 735f 6c61  egend_handles_la
+00066800: 6265 6c73 2829 0d0a 0909 0909 0909 0909  bels()..........
+00066810: 6861 6e64 2e61 7070 656e 6428 6861 6e64  hand.append(hand
+00066820: 6c65 735b 2d31 5d29 090d 0a09 0909 0909  les[-1])........
+00066830: 0965 6c69 6620 6973 696e 7374 616e 6365  .elif isinstance
+00066840: 286f 2e73 6361 7474 6572 6375 745b 305d  (o.scattercut[0]
+00066850: 2c20 206e 756d 6265 7273 2e4e 756d 6265  ,  numbers.Numbe
+00066860: 7229 3a0d 0a09 0909 0909 0909 7265 5b27  r):.........re['
+00066870: 4441 4327 5d2e 696c 6f63 5b3a 2c6a 5d2e  DAC'].iloc[:,j].
+00066880: 6c6f 635b 3a6f 2e73 6361 7474 6572 6375  loc[:o.scattercu
+00066890: 745b 305d 5d2e 706c 6f74 2873 7562 706c  t[0]].plot(subpl
+000668a0: 6f74 733d 4661 6c73 652c 6178 3d61 5b6a  ots=False,ax=a[j
+000668b0: 5d2c 6c65 6765 6e64 3d46 616c 7365 2c63  ],legend=False,c
+000668c0: 6f6c 6f72 3d63 6f6c 5b69 5d29 0d0a 0909  olor=col[i])....
+000668d0: 0909 0909 0969 6620 6a3d 3d30 3a0d 0a09  .....if j==0:...
+000668e0: 0909 0909 0909 0968 616e 646c 6573 2c6c  .......handles,l
+000668f0: 6162 656c 733d 615b 305d 2e67 6574 5f6c  abels=a[0].get_l
+00066900: 6567 656e 645f 6861 6e64 6c65 735f 6c61  egend_handles_la
+00066910: 6265 6c73 2829 0d0a 0909 0909 0909 0909  bels()..........
+00066920: 6861 6e64 2e61 7070 656e 6428 6861 6e64  hand.append(hand
+00066930: 6c65 735b 2d31 5d29 090d 0a09 0909 0909  les[-1])........
+00066940: 0909 7265 5b27 4441 4327 5d2e 696c 6f63  ..re['DAC'].iloc
+00066950: 5b3a 2c6a 5d2e 6c6f 635b 6f2e 7363 6174  [:,j].loc[o.scat
+00066960: 7465 7263 7574 5b31 5d3a 5d2e 706c 6f74  tercut[1]:].plot
+00066970: 2873 7562 706c 6f74 733d 4661 6c73 652c  (subplots=False,
+00066980: 6178 3d61 5b6a 5d2c 6c65 6765 6e64 3d46  ax=a[j],legend=F
+00066990: 616c 7365 2c63 6f6c 6f72 3d63 6f6c 5b69  alse,color=col[i
+000669a0: 5d2c 6c61 6265 6c20 3d20 275f 6e6f 6c65  ],label = '_nole
+000669b0: 6765 6e64 5f27 290d 0a09 0909 0909 0965  gend_')........e
+000669c0: 6c73 653a 0d0a 0909 0909 0909 0973 6361  lse:.........sca
+000669d0: 7474 6572 6375 7420 3d20 666c 6174 7465  ttercut = flatte
+000669e0: 6e28 6f2e 7363 6174 7465 7263 7574 290d  n(o.scattercut).
+000669f0: 0a09 0909 0909 0909 666f 7220 6d20 696e  ........for m in
+00066a00: 2072 616e 6765 286c 656e 2873 6361 7474   range(len(scatt
+00066a10: 6572 6375 7429 2f32 2b31 293a 0d0a 0909  ercut)/2+1):....
+00066a20: 0909 0909 0909 6966 206d 203d 3d20 303a  ......if m == 0:
+00066a30: 0d0a 0909 0909 0909 0909 0972 655b 2744  ...........re['D
+00066a40: 4143 275d 2e69 6c6f 635b 3a2c 6a5d 2e6c  AC'].iloc[:,j].l
+00066a50: 6f63 5b3a 7363 6174 7465 7263 7574 5b30  oc[:scattercut[0
+00066a60: 5d5d 2e70 6c6f 7428 7375 6270 6c6f 7473  ]].plot(subplots
+00066a70: 3d46 616c 7365 2c61 783d 615b 6a5d 2c6c  =False,ax=a[j],l
+00066a80: 6567 656e 643d 4661 6c73 652c 636f 6c6f  egend=False,colo
+00066a90: 723d 636f 6c5b 695d 290d 0a09 0909 0909  r=col[i]).......
+00066aa0: 0909 0909 6966 206a 3d3d 303a 0d0a 0909  ....if j==0:....
+00066ab0: 0909 0909 0909 0909 6861 6e64 6c65 732c  ........handles,
+00066ac0: 6c61 6265 6c73 3d61 5b6a 5d2e 6765 745f  labels=a[j].get_
+00066ad0: 6c65 6765 6e64 5f68 616e 646c 6573 5f6c  legend_handles_l
+00066ae0: 6162 656c 7328 290d 0a09 0909 0909 0909  abels().........
+00066af0: 0909 0968 616e 642e 6170 7065 6e64 2868  ...hand.append(h
+00066b00: 616e 646c 6573 5b2d 315d 2909 0d0a 0909  andles[-1]).....
+00066b10: 0909 0909 0909 656c 6966 206d 3c28 6c65  ......elif m<(le
+00066b20: 6e28 7363 6174 7465 7263 7574 292f 3229  n(scattercut)/2)
+00066b30: 3a0d 0a09 0909 0909 0909 0909 7265 5b27  :...........re['
+00066b40: 4441 4327 5d2e 696c 6f63 5b3a 2c6a 5d2e  DAC'].iloc[:,j].
+00066b50: 6c6f 635b 7363 6174 7465 7263 7574 5b32  loc[scattercut[2
+00066b60: 2a6d 2d31 5d3a 7363 6174 7465 7263 7574  *m-1]:scattercut
+00066b70: 5b32 2a6d 5d5d 2e70 6c6f 7428 7375 6270  [2*m]].plot(subp
+00066b80: 6c6f 7473 3d46 616c 7365 2c61 783d 615b  lots=False,ax=a[
+00066b90: 6a5d 2c6c 6567 656e 643d 4661 6c73 652c  j],legend=False,
+00066ba0: 636f 6c6f 723d 636f 6c5b 695d 2c6c 6162  color=col[i],lab
+00066bb0: 656c 203d 2027 5f6e 6f6c 6567 656e 645f  el = '_nolegend_
+00066bc0: 2729 0d0a 0909 0909 0909 0909 656c 7365  ')..........else
+00066bd0: 3a0d 0a09 0909 0909 0909 0909 7265 5b27  :...........re['
+00066be0: 4441 4327 5d2e 696c 6f63 5b3a 2c6a 5d2e  DAC'].iloc[:,j].
+00066bf0: 6c6f 635b 7363 6174 7465 7263 7574 5b2d  loc[scattercut[-
+00066c00: 315d 3a5d 2e70 6c6f 7428 7375 6270 6c6f  1]:].plot(subplo
+00066c10: 7473 3d46 616c 7365 2c61 783d 615b 6a5d  ts=False,ax=a[j]
+00066c20: 2c6c 6567 656e 643d 4661 6c73 652c 636f  ,legend=False,co
+00066c30: 6c6f 723d 636f 6c5b 695d 2c6c 6162 656c  lor=col[i],label
+00066c40: 203d 2027 5f6e 6f6c 6567 656e 645f 2729   = '_nolegend_')
+00066c50: 0d0a 0909 0909 0909 615b 6a5d 2e73 6574  ........a[j].set
+00066c60: 5f78 6c61 6265 6c28 2757 6176 656c 656e  _xlabel('Wavelen
+00066c70: 6774 6820 696e 206e 6d27 2909 0909 090d  gth in nm').....
+00066c80: 0a09 0909 0909 0961 5b6a 5d2e 7365 745f  .......a[j].set_
+00066c90: 796c 6162 656c 2827 5370 6563 7472 616c  ylabel('Spectral
+00066ca0: 2073 7472 656e 6774 6820 696e 2061 7262   strength in arb
+00066cb0: 2e20 756e 6974 7327 290d 0a09 0909 0909  . units').......
+00066cc0: 0961 5b6a 5d2e 6c65 6765 6e64 2866 6f6e  .a[j].legend(fon
+00066cd0: 7473 697a 653d 382c 6672 616d 656f 6e3d  tsize=8,frameon=
+00066ce0: 4661 6c73 6529 0d0a 0909 090d 0a09 0909  False)..........
+00066cf0: 0965 6c73 653a 0d0a 0909 0909 0964 6163  .else:.......dac
+00066d00: 733d 6c65 6e28 7265 5b27 4441 4327 5d2e  s=len(re['DAC'].
+00066d10: 636f 6c75 6d6e 7329 0d0a 0909 0909 0963  columns).......c
+00066d20: 6f6c 3d63 6f6c 6f72 735b 2869 2b31 292a  ol=colors[(i+1)*
+00066d30: 6461 6373 3a28 692b 3229 2a64 6163 735d  dacs:(i+2)*dacs]
+00066d40: 090d 0a09 0909 0909 4441 433d 7265 5b27  ........DAC=re['
+00066d50: 4441 4327 5d0d 0a09 0909 0909 6966 206f  DAC'].......if o
+00066d60: 2e73 6361 7474 6572 6375 7420 6973 204e  .scattercut is N
+00066d70: 6f6e 653a 090d 0a09 0909 0909 0961 7820  one:.........ax 
+00066d80: 3d20 4441 432e 706c 6f74 2873 7562 706c  = DAC.plot(subpl
+00066d90: 6f74 733d 7365 7061 7261 7465 5f70 6c6f  ots=separate_plo
+00066da0: 7473 2c61 783d 6178 2c6c 6567 656e 643d  ts,ax=ax,legend=
+00066db0: 4661 6c73 652c 636f 6c6f 723d 636f 6c6f  False,color=colo
+00066dc0: 7273 5b28 692b 3129 2a6c 656e 2873 7065  rs[(i+1)*len(spe
+00066dd0: 6369 6573 293a 2869 2b32 292a 6c65 6e28  cies):(i+2)*len(
+00066de0: 7370 6563 6965 7329 5d29 0d0a 0909 0909  species)])......
+00066df0: 0965 6c69 6620 6973 696e 7374 616e 6365  .elif isinstance
+00066e00: 286f 2e73 6361 7474 6572 6375 745b 305d  (o.scattercut[0]
+00066e10: 2c20 206e 756d 6265 7273 2e4e 756d 6265  ,  numbers.Numbe
+00066e20: 7229 3a0d 0a09 0909 0909 0961 7820 3d20  r):........ax = 
+00066e30: 4441 432e 6c6f 635b 3a6f 2e73 6361 7474  DAC.loc[:o.scatt
+00066e40: 6572 6375 745b 305d 2c20 3a5d 2e70 6c6f  ercut[0], :].plo
+00066e50: 7428 7375 6270 6c6f 7473 3d73 6570 6172  t(subplots=separ
+00066e60: 6174 655f 706c 6f74 732c 6178 3d61 782c  ate_plots,ax=ax,
+00066e70: 6c65 6765 6e64 3d46 616c 7365 2c63 6f6c  legend=False,col
+00066e80: 6f72 3d63 6f6c 6f72 735b 2869 2b31 292a  or=colors[(i+1)*
+00066e90: 6c65 6e28 7370 6563 6965 7329 3a28 692b  len(species):(i+
+00066ea0: 3229 2a6c 656e 2873 7065 6369 6573 295d  2)*len(species)]
+00066eb0: 290d 0a09 0909 0909 0944 4143 2e6c 6f63  )........DAC.loc
+00066ec0: 5b6f 2e73 6361 7474 6572 6375 745b 315d  [o.scattercut[1]
+00066ed0: 3a2c 203a 5d2e 706c 6f74 2873 7562 706c  :, :].plot(subpl
+00066ee0: 6f74 733d 7365 7061 7261 7465 5f70 6c6f  ots=separate_plo
+00066ef0: 7473 2c61 783d 6178 2c6c 6567 656e 643d  ts,ax=ax,legend=
+00066f00: 4661 6c73 652c 636f 6c6f 723d 636f 6c6f  False,color=colo
+00066f10: 7273 5b28 692b 3129 2a6c 656e 2873 7065  rs[(i+1)*len(spe
+00066f20: 6369 6573 293a 2869 2b32 292a 6c65 6e28  cies):(i+2)*len(
+00066f30: 7370 6563 6965 7329 5d29 0d0a 0909 0909  species)])......
+00066f40: 0965 6c73 653a 0d0a 0909 0909 0909 7363  .else:........sc
+00066f50: 6174 7465 7263 7574 203d 2066 6c61 7474  attercut = flatt
+00066f60: 656e 286f 2e73 6361 7474 6572 6375 7429  en(o.scattercut)
+00066f70: 0d0a 0909 0909 0909 666f 7220 6920 696e  ........for i in
+00066f80: 2072 616e 6765 286c 656e 2873 6361 7474   range(len(scatt
+00066f90: 6572 6375 7429 2f32 2b31 293a 0d0a 0909  ercut)/2+1):....
+00066fa0: 0909 0909 0969 6620 6920 3d3d 2030 3a0d  .....if i == 0:.
+00066fb0: 0a09 0909 0909 0909 0961 7820 3d20 4441  .........ax = DA
+00066fc0: 432e 6c6f 635b 3a73 6361 7474 6572 6375  C.loc[:scattercu
+00066fd0: 745b 305d 2c20 3a5d 2e70 6c6f 7428 7375  t[0], :].plot(su
+00066fe0: 6270 6c6f 7473 3d73 6570 6172 6174 655f  bplots=separate_
+00066ff0: 706c 6f74 732c 6178 3d61 782c 6c65 6765  plots,ax=ax,lege
+00067000: 6e64 3d46 616c 7365 2c63 6f6c 6f72 3d63  nd=False,color=c
+00067010: 6f6c 6f72 735b 2869 2b31 292a 6c65 6e28  olors[(i+1)*len(
+00067020: 7370 6563 6965 7329 3a28 692b 3229 2a6c  species):(i+2)*l
+00067030: 656e 2873 7065 6369 6573 295d 290d 0a09  en(species)])...
+00067040: 0909 0909 0909 656c 6966 2069 3c28 6c65  ......elif i<(le
+00067050: 6e28 7363 6174 7465 7263 7574 292f 3229  n(scattercut)/2)
+00067060: 3a0d 0a09 0909 0909 0909 0961 7820 3d20  :..........ax = 
+00067070: 4441 432e 6c6f 635b 7363 6174 7465 7263  DAC.loc[scatterc
+00067080: 7574 5b32 2a69 2d31 5d3a 7363 6174 7465  ut[2*i-1]:scatte
+00067090: 7263 7574 5b32 2a69 5d2c 203a 5d2e 706c  rcut[2*i], :].pl
+000670a0: 6f74 2873 7562 706c 6f74 733d 7365 7061  ot(subplots=sepa
+000670b0: 7261 7465 5f70 6c6f 7473 2c61 783d 6178  rate_plots,ax=ax
+000670c0: 2c6c 6567 656e 643d 4661 6c73 652c 636f  ,legend=False,co
+000670d0: 6c6f 723d 636f 6c6f 7273 5b28 692b 3129  lor=colors[(i+1)
+000670e0: 2a6c 656e 2873 7065 6369 6573 293a 2869  *len(species):(i
+000670f0: 2b32 292a 6c65 6e28 7370 6563 6965 7329  +2)*len(species)
+00067100: 5d29 0d0a 0909 0909 0909 0965 6c73 653a  ]).........else:
+00067110: 0d0a 0909 0909 0909 0909 6178 203d 2044  ..........ax = D
+00067120: 4143 2e6c 6f63 5b73 6361 7474 6572 6375  AC.loc[scattercu
+00067130: 745b 2d31 5d3a 2c20 3a5d 2e70 6c6f 7428  t[-1]:, :].plot(
+00067140: 7375 6270 6c6f 7473 3d73 6570 6172 6174  subplots=separat
+00067150: 655f 706c 6f74 732c 6178 3d61 782c 6c65  e_plots,ax=ax,le
+00067160: 6765 6e64 3d46 616c 7365 2c63 6f6c 6f72  gend=False,color
+00067170: 3d63 6f6c 6f72 735b 2869 2b31 292a 6c65  =colors[(i+1)*le
+00067180: 6e28 7370 6563 6965 7329 3a28 692b 3229  n(species):(i+2)
+00067190: 2a6c 656e 2873 7065 6369 6573 295d 290d  *len(species)]).
+000671a0: 0a09 0909 0909 6178 2e73 6574 5f78 6c61  ......ax.set_xla
+000671b0: 6265 6c28 2757 6176 656c 656e 6774 6820  bel('Wavelength 
+000671c0: 696e 206e 6d27 2909 0909 090d 0a09 0909  in nm').........
+000671d0: 0909 6178 2e73 6574 5f79 6c61 6265 6c28  ..ax.set_ylabel(
+000671e0: 2753 7065 6374 7261 6c20 7374 7265 6e67  'Spectral streng
+000671f0: 7468 2069 6e20 6172 622e 2075 6e69 7473  th in arb. units
+00067200: 2729 0d0a 0909 0909 0961 782e 6c65 6765  ').......ax.lege
+00067210: 6e64 2866 6f6e 7473 697a 653d 382c 6672  nd(fontsize=8,fr
+00067220: 616d 656f 6e3d 4661 6c73 6529 0d0a 0909  ameon=False)....
+00067230: 6966 206e 6f74 2068 6173 6174 7472 2861  if not hasattr(a
+00067240: 782c 275f 5f69 7465 725f 5f27 293a 6178  x,'__iter__'):ax
+00067250: 3d6e 702e 6172 7261 7928 5b61 785d 290d  =np.array([ax]).
+00067260: 0a09 0969 6620 7370 6563 7472 6120 6973  ...if spectra is
+00067270: 206e 6f74 204e 6f6e 653a 0d0a 0909 0966   not None:.....f
+00067280: 6f72 2061 2069 6e20 6178 3a0d 0a09 0909  or a in ax:.....
+00067290: 0973 7065 6374 7261 2e70 6c6f 7428 6178  .spectra.plot(ax
+000672a0: 3d61 2c73 7562 706c 6f74 733d 7365 7061  =a,subplots=sepa
+000672b0: 7261 7465 5f70 6c6f 7473 2909 0909 090d  rate_plots).....
+000672c0: 0a09 0966 6967 3d28 6178 2e72 6176 656c  ...fig=(ax.ravel
+000672d0: 2829 295b 305d 2e66 6967 7572 650d 0a09  ())[0].figure...
+000672e0: 0969 6620 7365 7061 7261 7465 5f70 6c6f  .if separate_plo
+000672f0: 7473 3a0d 0a09 0909 6669 672e 7365 745f  ts:.....fig.set_
+00067300: 7369 7a65 5f69 6e63 6865 7328 3132 2c31  size_inches(12,1
+00067310: 3029 0d0a 0909 0961 7865 735f 6e75 6d62  0).....axes_numb
+00067320: 6572 3d66 6967 2e67 6574 5f61 7865 7328  er=fig.get_axes(
+00067330: 290d 0a09 0909 6e61 6d65 733d 5b73 656c  ).....names=[sel
+00067340: 662e 6669 6c65 6e61 6d65 5d0d 0a09 0909  f.filename].....
+00067350: 6966 206f 7468 6572 2069 7320 6e6f 7420  if other is not 
+00067360: 4e6f 6e65 3a0d 0a09 0909 0966 6f72 206f  None:......for o
+00067370: 2069 6e20 6f74 6865 723a 0d0a 0909 0909   in other:......
+00067380: 096e 616d 6573 2e61 7070 656e 6428 6f2e  .names.append(o.
+00067390: 6669 6c65 6e61 6d65 290d 0a09 0909 666f  filename).....fo
+000673a0: 7220 692c 6178 2069 6e20 656e 756d 6572  r i,ax in enumer
+000673b0: 6174 6528 6178 6573 5f6e 756d 6265 7229  ate(axes_number)
+000673c0: 3a0d 0a09 0909 0974 7279 3a0d 0a09 0909  :......try:.....
+000673d0: 0909 6e61 6d65 7465 6d70 3d5b 2725 7327  ..nametemp=['%s'
+000673e0: 2573 7065 6369 6573 5b69 5d20 2b20 2720  %species[i] + ' 
+000673f0: 2d20 2720 2b20 6120 666f 7220 6120 696e  - ' + a for a in
+00067400: 206e 616d 6573 5d0d 0a09 0909 0909 6178   names].......ax
+00067410: 2e6c 6567 656e 6428 6861 6e64 2c6e 616d  .legend(hand,nam
+00067420: 6574 656d 7029 0d0a 0909 0909 6578 6365  etemp)......exce
+00067430: 7074 3a0d 0a09 0909 0909 7061 7373 0d0a  pt:.......pass..
+00067440: 0909 656c 7365 3a0d 0a09 0909 6178 3d66  ..else:.....ax=f
+00067450: 6967 2e67 6574 5f61 7865 7328 295b 305d  ig.get_axes()[0]
+00067460: 0d0a 0909 096e 616d 6573 3d5b 7365 6c66  .....names=[self
+00067470: 2e66 696c 656e 616d 655d 0d0a 0909 0969  .filename].....i
+00067480: 6620 6f74 6865 7220 6973 206e 6f74 204e  f other is not N
+00067490: 6f6e 653a 0d0a 0909 0909 666f 7220 6f20  one:......for o 
+000674a0: 696e 206f 7468 6572 3a0d 0a09 0909 0909  in other:.......
+000674b0: 6e61 6d65 732e 6170 7065 6e64 286f 2e66  names.append(o.f
+000674c0: 696c 656e 616d 6529 0d0a 0909 0968 616e  ilename).....han
+000674d0: 646c 6573 2c6c 6162 656c 733d 6178 2e67  dles,labels=ax.g
+000674e0: 6574 5f6c 6567 656e 645f 6861 6e64 6c65  et_legend_handle
+000674f0: 735f 6c61 6265 6c73 2829 0d0a 0909 096e  s_labels().....n
+00067500: 616d 6574 656d 703d 5b5d 0d0a 0909 0974  ametemp=[].....t
+00067510: 7279 3a0d 0a09 0909 0966 6f72 2061 2069  ry:......for a i
+00067520: 6e20 6e61 6d65 733a 0d0a 0909 0909 0966  n names:.......f
+00067530: 6f72 2062 2069 6e20 7370 6563 6965 733a  or b in species:
+00067540: 0d0a 0909 0909 0909 6e61 6d65 7465 6d70  ........nametemp
+00067550: 2e61 7070 656e 6428 2725 7327 2562 202b  .append('%s'%b +
+00067560: 2027 202d 2027 202b 2061 290d 0a09 0909   ' - ' + a).....
+00067570: 0961 782e 6c65 6765 6e64 2868 616e 646c  .ax.legend(handl
+00067580: 6573 2c6e 616d 6574 656d 7029 0d0a 0909  es,nametemp)....
+00067590: 0965 7863 6570 743a 0d0a 0909 0909 7061  .except:......pa
+000675a0: 7373 0d0a 0909 0966 6967 2e73 6574 5f73  ss.....fig.set_s
+000675b0: 697a 655f 696e 6368 6573 2831 362c 3829  ize_inches(16,8)
+000675c0: 0d0a 0909 6669 672e 7469 6768 745f 6c61  ....fig.tight_la
+000675d0: 796f 7574 2829 0d0a 0909 6966 2073 656c  yout()....if sel
+000675e0: 662e 7361 7665 5f66 6967 7572 6573 5f74  f.save_figures_t
+000675f0: 6f5f 666f 6c64 6572 3a0d 0a09 0909 6669  o_folder:.....fi
+00067600: 672e 7361 7665 6669 6728 6368 6563 6b5f  g.savefig(check_
+00067610: 666f 6c64 6572 2870 6174 683d 7365 6c66  folder(path=self
+00067620: 2e66 6967 7572 655f 7061 7468 2c66 696c  .figure_path,fil
+00067630: 656e 616d 653d 2763 6f6d 7061 7265 5f44  ename='compare_D
+00067640: 4143 2e70 6e67 2729 2c62 626f 785f 696e  AC.png'),bbox_in
+00067650: 6368 6573 3d27 7469 6768 7427 290d 0a0d  ches='tight')...
+00067660: 0a0d 0a0d 0a                             .....
```

### Comparing `KiMoPack-7.0.1/src/KiMoPack.egg-info/PKG-INFO` & `KiMoPack-7.0.2/src/KiMoPack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KiMoPack
-Version: 7.0.1
+Version: 7.0.2
 Summary: A comprehensive package for the analysis of kinetic data.
 Home-page: https://github.com/erdzeichen/KiMoPack
 Author: Jens Uhlig
 Author-email: jens.uhlig@chemphys.lu.se
 Project-URL: Bug Tracker, https://github.com/erdzeichen/KiMoPack/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `KiMoPack-7.0.1/src/KiMoPack.egg-info/SOURCES.txt` & `KiMoPack-7.0.2/src/KiMoPack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

