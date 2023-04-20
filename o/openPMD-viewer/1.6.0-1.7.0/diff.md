# Comparing `tmp/openPMD-viewer-1.6.0.tar.gz` & `tmp/openPMD-viewer-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openPMD-viewer-1.6.0.tar", last modified: Thu Feb  9 07:08:13 2023, max compression
+gzip compressed data, was "openPMD-viewer-1.7.0.tar", last modified: Thu Apr 20 15:36:38 2023, max compression
```

## Comparing `openPMD-viewer-1.6.0.tar` & `openPMD-viewer-1.7.0.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2023-02-09 07:08:13.095713 openPMD-viewer-1.6.0/
--rw-r--r--   0 rlehe      (501) staff       (20)     2442 2020-02-07 13:04:53.000000 openPMD-viewer-1.6.0/LICENSE.txt
--rw-r--r--   0 rlehe      (501) staff       (20)      164 2020-03-09 15:30:32.000000 openPMD-viewer-1.6.0/MANIFEST.in
--rw-r--r--   0 rlehe      (501) staff       (20)     5007 2023-02-09 07:08:13.095188 openPMD-viewer-1.6.0/PKG-INFO
--rw-r--r--   0 rlehe      (501) staff       (20)     3899 2022-04-14 17:51:46.000000 openPMD-viewer-1.6.0/README.md
-drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2023-02-09 07:08:13.063922 openPMD-viewer-1.6.0/openPMD_viewer.egg-info/
--rw-r--r--   0 rlehe      (501) staff       (20)     5007 2023-02-09 07:08:12.000000 openPMD-viewer-1.6.0/openPMD_viewer.egg-info/PKG-INFO
--rw-r--r--   0 rlehe      (501) staff       (20)     1780 2023-02-09 07:08:12.000000 openPMD-viewer-1.6.0/openPMD_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 rlehe      (501) staff       (20)        1 2023-02-09 07:08:12.000000 openPMD-viewer-1.6.0/openPMD_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 rlehe      (501) staff       (20)      254 2023-02-09 07:08:12.000000 openPMD-viewer-1.6.0/openPMD_viewer.egg-info/requires.txt
--rw-r--r--   0 rlehe      (501) staff       (20)       27 2023-02-09 07:08:12.000000 openPMD-viewer-1.6.0/openPMD_viewer.egg-info/top_level.txt
-drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2023-02-09 07:08:13.065321 openPMD-viewer-1.6.0/openpmd_viewer/
--rw-r--r--   0 rlehe      (501) staff       (20)      433 2021-01-06 04:52:04.000000 openPMD-viewer-1.6.0/openpmd_viewer/__init__.py
--rw-r--r--   0 rlehe      (501) staff       (20)       22 2023-02-09 07:07:58.000000 openPMD-viewer-1.6.0/openpmd_viewer/__version__.py
-drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2023-02-09 07:08:13.066039 openPMD-viewer-1.6.0/openpmd_viewer/addons/
--rw-r--r--   0 rlehe      (501) staff       (20)       61 2020-03-09 15:30:33.000000 openPMD-viewer-1.6.0/openpmd_viewer/addons/__init__.py
-drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2023-02-09 07:08:13.068698 openPMD-viewer-1.6.0/openpmd_viewer/addons/pic/
--rw-r--r--   0 rlehe      (501) staff       (20)       73 2020-03-09 15:30:33.000000 openPMD-viewer-1.6.0/openpmd_viewer/addons/pic/__init__.py
--rw-r--r--   0 rlehe      (501) staff       (20)    47200 2023-02-09 07:07:58.000000 openPMD-viewer-1.6.0/openpmd_viewer/addons/pic/lpa_diagnostics.py
-drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2023-02-09 07:08:13.071015 openPMD-viewer-1.6.0/openpmd_viewer/notebook_starter/
--rw-r--r--   0 rlehe      (501) staff       (20)     1537 2022-03-04 23:18:06.000000 openPMD-viewer-1.6.0/openpmd_viewer/notebook_starter/Template_notebook.ipynb
--rwxr-xr-x   0 rlehe      (501) staff       (20)      853 2020-03-09 15:30:33.000000 openPMD-viewer-1.6.0/openpmd_viewer/notebook_starter/openPMD_notebook
-drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2023-02-09 07:08:13.079203 openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/
--rw-r--r--   0 rlehe      (501) staff       (20)      244 2022-03-04 23:18:06.000000 openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/__init__.py
-drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2023-02-09 07:08:13.081007 openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/data_reader/
--rw-r--r--   0 rlehe      (501) staff       (20)      103 2022-03-04 23:18:06.000000 openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/data_reader/__init__.py
--rw-r--r--   0 rlehe      (501) staff       (20)    12684 2023-02-06 20:20:32.000000 openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/data_reader/data_reader.py
-drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2023-02-09 07:08:13.086588 openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/data_reader/h5py_reader/
--rw-r--r--   0 rlehe      (501) staff       (20)      359 2022-03-04 23:18:06.000000 openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/data_reader/h5py_reader/__init__.py
--rw-r--r--   0 rlehe      (501) staff       (20)    17177 2023-02-06 20:20:32.000000 openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/data_reader/h5py_reader/field_reader.py
--rw-r--r--   0 rlehe      (501) staff       (20)     9072 2022-03-04 23:18:06.000000 openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/data_reader/h5py_reader/params_reader.py
--rw-r--r--   0 rlehe      (501) staff       (20)     3187 2022-03-04 23:18:06.000000 openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/data_reader/h5py_reader/particle_reader.py
--rw-r--r--   0 rlehe      (501) staff       (20)     6148 2023-02-09 07:07:58.000000 openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/data_reader/h5py_reader/utilities.py
-drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2023-02-09 07:08:13.092543 openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/data_reader/io_reader/
--rw-r--r--   0 rlehe      (501) staff       (20)      318 2022-03-04 23:18:06.000000 openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/data_reader/io_reader/__init__.py
--rw-r--r--   0 rlehe      (501) staff       (20)    16025 2023-02-06 20:20:32.000000 openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/data_reader/io_reader/field_reader.py
--rw-r--r--   0 rlehe      (501) staff       (20)     7816 2022-03-04 23:18:06.000000 openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/data_reader/io_reader/params_reader.py
--rw-r--r--   0 rlehe      (501) staff       (20)     3397 2022-03-04 23:18:06.000000 openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/data_reader/io_reader/particle_reader.py
--rw-r--r--   0 rlehe      (501) staff       (20)     6036 2023-02-09 07:07:58.000000 openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/data_reader/io_reader/utilities.py
--rw-r--r--   0 rlehe      (501) staff       (20)     6846 2022-04-14 17:51:46.000000 openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/field_metainfo.py
--rw-r--r--   0 rlehe      (501) staff       (20)    36934 2021-02-09 16:41:14.000000 openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/interactive.py
--rw-r--r--   0 rlehe      (501) staff       (20)    28276 2023-02-09 07:03:49.000000 openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/main.py
--rw-r--r--   0 rlehe      (501) staff       (20)      881 2020-03-09 15:30:32.000000 openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/numba_wrapper.py
--rw-r--r--   0 rlehe      (501) staff       (20)    11111 2022-08-05 19:55:33.000000 openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/particle_tracker.py
--rw-r--r--   0 rlehe      (501) staff       (20)    15484 2023-02-09 07:07:58.000000 openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/plotter.py
--rw-r--r--   0 rlehe      (501) staff       (20)    12721 2022-04-14 17:51:46.000000 openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/utilities.py
-drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2023-02-09 07:08:13.093672 openPMD-viewer-1.6.0/opmd_viewer/
--rw-r--r--   0 rlehe      (501) staff       (20)     1117 2020-03-09 15:30:32.000000 openPMD-viewer-1.6.0/opmd_viewer/__init__.py
--rw-r--r--   0 rlehe      (501) staff       (20)       36 2022-03-04 23:18:06.000000 openPMD-viewer-1.6.0/requirements.txt
--rw-r--r--   0 rlehe      (501) staff       (20)       38 2023-02-09 07:08:13.095911 openPMD-viewer-1.6.0/setup.cfg
--rw-r--r--   0 rlehe      (501) staff       (20)     2635 2022-04-14 17:51:46.000000 openPMD-viewer-1.6.0/setup.py
+drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2023-04-20 15:36:38.427964 openPMD-viewer-1.7.0/
+-rw-r--r--   0 rlehe      (501) staff       (20)     2442 2020-02-07 13:04:53.000000 openPMD-viewer-1.7.0/LICENSE.txt
+-rw-r--r--   0 rlehe      (501) staff       (20)      164 2020-03-09 15:30:32.000000 openPMD-viewer-1.7.0/MANIFEST.in
+-rw-r--r--   0 rlehe      (501) staff       (20)     5008 2023-04-20 15:36:38.427638 openPMD-viewer-1.7.0/PKG-INFO
+-rw-r--r--   0 rlehe      (501) staff       (20)     3899 2022-04-14 17:51:46.000000 openPMD-viewer-1.7.0/README.md
+drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2023-04-20 15:36:38.403585 openPMD-viewer-1.7.0/openPMD_viewer.egg-info/
+-rw-r--r--   0 rlehe      (501) staff       (20)     5008 2023-04-20 15:36:38.000000 openPMD-viewer-1.7.0/openPMD_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 rlehe      (501) staff       (20)     1828 2023-04-20 15:36:38.000000 openPMD-viewer-1.7.0/openPMD_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 rlehe      (501) staff       (20)        1 2023-04-20 15:36:38.000000 openPMD-viewer-1.7.0/openPMD_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 rlehe      (501) staff       (20)      254 2023-04-20 15:36:38.000000 openPMD-viewer-1.7.0/openPMD_viewer.egg-info/requires.txt
+-rw-r--r--   0 rlehe      (501) staff       (20)       27 2023-04-20 15:36:38.000000 openPMD-viewer-1.7.0/openPMD_viewer.egg-info/top_level.txt
+drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2023-04-20 15:36:38.404967 openPMD-viewer-1.7.0/openpmd_viewer/
+-rw-r--r--   0 rlehe      (501) staff       (20)      433 2021-01-06 04:52:04.000000 openPMD-viewer-1.7.0/openpmd_viewer/__init__.py
+-rw-r--r--   0 rlehe      (501) staff       (20)       22 2023-04-20 15:34:54.000000 openPMD-viewer-1.7.0/openpmd_viewer/__version__.py
+drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2023-04-20 15:36:38.405435 openPMD-viewer-1.7.0/openpmd_viewer/addons/
+-rw-r--r--   0 rlehe      (501) staff       (20)       61 2020-03-09 15:30:33.000000 openPMD-viewer-1.7.0/openpmd_viewer/addons/__init__.py
+drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2023-04-20 15:36:38.406720 openPMD-viewer-1.7.0/openpmd_viewer/addons/pic/
+-rw-r--r--   0 rlehe      (501) staff       (20)       73 2020-03-09 15:30:33.000000 openPMD-viewer-1.7.0/openpmd_viewer/addons/pic/__init__.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    47681 2023-04-20 15:34:54.000000 openPMD-viewer-1.7.0/openpmd_viewer/addons/pic/lpa_diagnostics.py
+drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2023-04-20 15:36:38.408577 openPMD-viewer-1.7.0/openpmd_viewer/notebook_starter/
+-rw-r--r--   0 rlehe      (501) staff       (20)     1537 2022-03-04 23:18:06.000000 openPMD-viewer-1.7.0/openpmd_viewer/notebook_starter/Template_notebook.ipynb
+-rwxr-xr-x   0 rlehe      (501) staff       (20)      853 2020-03-09 15:30:33.000000 openPMD-viewer-1.7.0/openpmd_viewer/notebook_starter/openPMD_notebook
+drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2023-04-20 15:36:38.416158 openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/
+-rw-r--r--   0 rlehe      (501) staff       (20)      244 2022-03-04 23:18:06.000000 openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/__init__.py
+-rw-r--r--   0 rlehe      (501) staff       (20)      616 2023-04-20 15:34:54.000000 openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/data_order.py
+drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2023-04-20 15:36:38.417559 openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/data_reader/
+-rw-r--r--   0 rlehe      (501) staff       (20)      103 2022-03-04 23:18:06.000000 openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/data_reader/__init__.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    12684 2023-04-10 16:36:05.000000 openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/data_reader/data_reader.py
+drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2023-04-20 15:36:38.422420 openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/data_reader/h5py_reader/
+-rw-r--r--   0 rlehe      (501) staff       (20)      359 2022-03-04 23:18:06.000000 openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/data_reader/h5py_reader/__init__.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    18033 2023-04-20 15:34:54.000000 openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/data_reader/h5py_reader/field_reader.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     9072 2022-03-04 23:18:06.000000 openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/data_reader/h5py_reader/params_reader.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     3187 2022-03-04 23:18:06.000000 openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/data_reader/h5py_reader/particle_reader.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     6148 2023-04-18 14:41:03.000000 openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/data_reader/h5py_reader/utilities.py
+drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2023-04-20 15:36:38.426182 openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/data_reader/io_reader/
+-rw-r--r--   0 rlehe      (501) staff       (20)      318 2022-03-04 23:18:06.000000 openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/data_reader/io_reader/__init__.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    17005 2023-04-20 15:34:54.000000 openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/data_reader/io_reader/field_reader.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     7816 2022-03-04 23:18:06.000000 openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/data_reader/io_reader/params_reader.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     3397 2022-03-04 23:18:06.000000 openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/data_reader/io_reader/particle_reader.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     6105 2023-04-20 15:34:54.000000 openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/data_reader/io_reader/utilities.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     6846 2022-04-14 17:51:46.000000 openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/field_metainfo.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    36934 2021-02-09 16:41:14.000000 openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/interactive.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    28276 2023-04-18 14:41:03.000000 openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/main.py
+-rw-r--r--   0 rlehe      (501) staff       (20)      881 2020-03-09 15:30:32.000000 openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/numba_wrapper.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    11111 2023-04-18 14:41:03.000000 openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/particle_tracker.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    15484 2023-04-18 14:41:03.000000 openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/plotter.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    12994 2023-04-20 15:34:54.000000 openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/utilities.py
+drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2023-04-20 15:36:38.426870 openPMD-viewer-1.7.0/opmd_viewer/
+-rw-r--r--   0 rlehe      (501) staff       (20)     1117 2020-03-09 15:30:32.000000 openPMD-viewer-1.7.0/opmd_viewer/__init__.py
+-rw-r--r--   0 rlehe      (501) staff       (20)       36 2022-03-04 23:18:06.000000 openPMD-viewer-1.7.0/requirements.txt
+-rw-r--r--   0 rlehe      (501) staff       (20)       38 2023-04-20 15:36:38.428106 openPMD-viewer-1.7.0/setup.cfg
+-rw-r--r--   0 rlehe      (501) staff       (20)     2636 2023-04-20 15:34:54.000000 openPMD-viewer-1.7.0/setup.py
```

### Comparing `openPMD-viewer-1.6.0/LICENSE.txt` & `openPMD-viewer-1.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openPMD-viewer-1.6.0/PKG-INFO` & `openPMD-viewer-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openPMD-viewer
-Version: 1.6.0
+Version: 1.7.0
 Summary: Visualization tools for openPMD files
 Home-page: https://github.com/openPMD/openPMD-viewer.git
 Maintainer: Remi Lehe
 Maintainer-email: remi.lehe@lbl.gov
 License: BSD-3-Clause-LBNL
 Platform: any
 Classifier: Programming Language :: Python
@@ -13,20 +13,20 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: GUI
 Provides-Extra: plot
 Provides-Extra: tutorials
 Provides-Extra: numba
 Provides-Extra: openpmd-api
```

### Comparing `openPMD-viewer-1.6.0/README.md` & `openPMD-viewer-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `openPMD-viewer-1.6.0/openPMD_viewer.egg-info/PKG-INFO` & `openPMD-viewer-1.7.0/openPMD_viewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openPMD-viewer
-Version: 1.6.0
+Version: 1.7.0
 Summary: Visualization tools for openPMD files
 Home-page: https://github.com/openPMD/openPMD-viewer.git
 Maintainer: Remi Lehe
 Maintainer-email: remi.lehe@lbl.gov
 License: BSD-3-Clause-LBNL
 Platform: any
 Classifier: Programming Language :: Python
@@ -13,20 +13,20 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: GUI
 Provides-Extra: plot
 Provides-Extra: tutorials
 Provides-Extra: numba
 Provides-Extra: openpmd-api
```

### Comparing `openPMD-viewer-1.6.0/openPMD_viewer.egg-info/SOURCES.txt` & `openPMD-viewer-1.7.0/openPMD_viewer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 openpmd_viewer/__version__.py
 openpmd_viewer/addons/__init__.py
 openpmd_viewer/addons/pic/__init__.py
 openpmd_viewer/addons/pic/lpa_diagnostics.py
 openpmd_viewer/notebook_starter/Template_notebook.ipynb
 openpmd_viewer/notebook_starter/openPMD_notebook
 openpmd_viewer/openpmd_timeseries/__init__.py
+openpmd_viewer/openpmd_timeseries/data_order.py
 openpmd_viewer/openpmd_timeseries/field_metainfo.py
 openpmd_viewer/openpmd_timeseries/interactive.py
 openpmd_viewer/openpmd_timeseries/main.py
 openpmd_viewer/openpmd_timeseries/numba_wrapper.py
 openpmd_viewer/openpmd_timeseries/particle_tracker.py
 openpmd_viewer/openpmd_timeseries/plotter.py
 openpmd_viewer/openpmd_timeseries/utilities.py
```

### Comparing `openPMD-viewer-1.6.0/openpmd_viewer/addons/pic/lpa_diagnostics.py` & `openPMD-viewer-1.7.0/openpmd_viewer/addons/pic/lpa_diagnostics.py`

 * *Files 1% similar despite different names*

```diff
@@ -882,15 +882,15 @@
                                    E, p0=[ z0, E0, ctau ])
             return( params[2] )
 
         else:
             raise ValueError('Unknown method: {:s}'.format(method))
 
     def get_laser_waist( self, t=None, iteration=None, pol=None, theta=0,
-                         method='fit' ):
+                         laser_propagation='z', method='fit' ):
         """
         Calculate the waist of a (gaussian) laser pulse. ( sqrt(2) * sigma_r)
 
         In 3D, this function takes a slice across `y`, and thus computes the
         waist in the `x-z` plane.
 
         Parameters
@@ -907,14 +907,18 @@
         pol : string
             Polarization of the field. Options are 'x', 'y'
 
         theta : float, optional
            Only used for thetaMode geometry
            The angle of the plane of observation, with respect to the x axis
 
+        laser_propagation : string, optional
+            Coordinate along which laser field propagates.
+            Default is 'z'.
+
         method : str, optional
            The method which is used to compute the waist
            'fit': Gaussian fit of the transverse profile
            'rms': RMS radius, weighted by the transverse profile
            ('rms' tends to give more weight to the "wings" of the pulse)
 
         Returns
@@ -926,34 +930,39 @@
         if geometry == '3dcartesian':
             slice_across = 'y'
         else:
             slice_across = None
 
         # Get the field envelope (as 2D array)
         field, info = self.get_laser_envelope(t=t, iteration=iteration,
-                         pol=pol, slice_across=slice_across, theta=theta)
+                         pol=pol, laser_propagation=laser_propagation,
+                         slice_across=slice_across, theta=theta)
         assert field.ndim == 2
-        # Find the indices of the maximum field, and
-        # pick the corresponding transverse slice
-        itrans_max, iz_max = np.unravel_index(
-            np.argmax( field ), field.shape )
-        trans_slice = field[ :, iz_max ]
-        # Get transverse positons
-        trans_pos = getattr(info, info.axes[0])
+
+        # Detect direction of laser propagation
+        inverted_axes_dict = {info.axes[key]: key for key in info.axes.keys()}
+        slicing_index = inverted_axes_dict[laser_propagation]
+        # Find the indices of the maximum field
+        i_max = np.unravel_index( np.argmax( field ), field.shape )
+        # Pick the corresponding transverse slice
+        # (Transverse to laser propagation)
+        trans_slice = np.take( field, [i_max[slicing_index]], axis=slicing_index ).flatten()
+        # Get transverse positions
+        trans_pos = getattr(info, info.axes[(slicing_index+1)%2])
 
         # Compute waist with RMS value
         # (serves as initial guess when method=='fit')
         w0 = np.sqrt(2) * w_std(trans_pos, trans_slice)
         if method == 'rms':
             return( w0 )
 
         # Compute waist with Gaussian fit
         elif method == 'fit':
             # Get initial guess for the amplitude
-            E0 = field[ itrans_max, iz_max ]
+            E0 = trans_pos.max()
             # Assume that the pulse is centered
             x0 = 0
             # Perform the fit
             params, _ = curve_fit( gaussian_profile, trans_pos,
                                    trans_slice, p0=[x0, E0, w0 ])
             return( params[2] )
```

### Comparing `openPMD-viewer-1.6.0/openpmd_viewer/notebook_starter/Template_notebook.ipynb` & `openPMD-viewer-1.7.0/openpmd_viewer/notebook_starter/Template_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `openPMD-viewer-1.6.0/openpmd_viewer/notebook_starter/openPMD_notebook` & `openPMD-viewer-1.7.0/openpmd_viewer/notebook_starter/openPMD_notebook`

 * *Files identical despite different names*

### Comparing `openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/data_reader/data_reader.py` & `openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/data_reader/data_reader.py`

 * *Files identical despite different names*

### Comparing `openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/data_reader/h5py_reader/field_reader.py` & `openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/data_reader/h5py_reader/field_reader.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 Author: Remi Lehe
 License: 3-Clause-BSD-LBNL
 """
 
 import h5py
 import numpy as np
 from .utilities import get_shape, get_data, join_infile_path
+from ...data_order import RZorder, order_error_msg
 from openpmd_viewer.openpmd_timeseries.field_metainfo import FieldMetaInformation
 from openpmd_viewer.openpmd_timeseries.utilities import construct_3d_from_circ
 
 
 def read_field_cartesian( filename, iteration, field, coord, axis_labels,
                           slice_relative_position, slice_across ):
     """
@@ -183,22 +184,26 @@
     else:
         field_path = join_infile_path( field, coord )
     group, dset = find_dataset( dfile, iteration, field_path )
 
     # Extract the metainformation
     coord_labels = {ii: coord.decode() for (ii,coord) in
                                 enumerate(group.attrs['axisLabels'])}
-    if coord_labels[0] == 'r':
-        rz_switch = False  # fastest varying index is z
+    coord_label_str = ''.join(coord_labels.values())
+    coord_label_str = 'm' + coord_label_str
+    coord_order = RZorder[coord_label_str]
+
+    if coord_order == RZorder.mrz:
         Nm, Nr, Nz = get_shape( dset )
         N_pair = (Nr, Nz)
-    else:
-        rz_switch = True  # fastest varying index is r
+    elif coord_order == RZorder.mzr:
         Nm, Nz, Nr = get_shape( dset )
         N_pair = (Nz, Nr)
+    else:
+        raise Exception(order_error_msg)
     info = FieldMetaInformation( coord_labels, N_pair,
         group.attrs['gridSpacing'], group.attrs['gridGlobalOffset'],
         group.attrs['gridUnitSI'], dset.attrs['position'], thetaMode=True )
 
     # Convert to a 3D Cartesian array if theta is None
     if theta is None:
 
@@ -216,100 +221,115 @@
         # If necessary, reduce resolution of 3D reconstruction
         if max_resolution_3d is not None:
             max_res_lon, max_res_transv = max_resolution_3d
             if Nz > max_res_lon:
                 # Calculate excess of elements along z
                 excess_z = int(np.round(Nz/max_res_lon))
                 # Preserve only one every excess_z elements
-                if not rz_switch:
+                if coord_order is RZorder.mrz:
                     Fcirc = Fcirc[:, :, ::excess_z]
-                else:
+                elif coord_order is RZorder.mzr:
                     Fcirc = Fcirc[:, ::excess_z, :]
+                else:
+                    raise Exception(order_error_msg)
+
                 # Update info accordingly
                 info.z = info.z[::excess_z]
                 info.dz = info.z[1] - info.z[0]
             if Nr > max_res_transv/2:
                 # Calculate excess of elements along r
                 excess_r = int(np.round(Nr/(max_res_transv/2)))
                 # Preserve only one every excess_r elements
-                if not rz_switch:
+                if coord_order is RZorder.mrz:
                     Fcirc = Fcirc[:, ::excess_r, :]
-                else:
+                elif coord_order is RZorder.mzr:
                     Fcirc = Fcirc[:, :, ::excess_r]
+                else:
+                    raise Exception(order_error_msg)
+
                 # Update info and necessary parameters accordingly
                 info.r = info.r[::excess_r]
                 info.dr = info.r[1] - info.r[0]
                 inv_dr = 1./info.dr
                 # Update Nr after reducing radial resolution.
-                if not rz_switch:
+                if coord_order is RZorder.mrz:
                     Nr = Fcirc.shape[1]
-                else:
+                elif coord_order is RZorder.mzr:
                     Nr = Fcirc.shape[2]
+                else:
+                    raise Exception(order_error_msg)
+
 
         # Convert cylindrical data to Cartesian data
         info._convert_cylindrical_to_3Dcartesian()
         nx, ny, nz = len(info.x), len(info.y), len(info.z)
         F_total = np.zeros( (nx, ny, nz) )
         construct_3d_from_circ( F_total, Fcirc, info.x, info.y, modes,
-            nx, ny, nz, Nr, nmodes, inv_dr, rmax, rz_switch=rz_switch )
+            nx, ny, nz, Nr, nmodes, inv_dr, rmax, coord_order )
 
     else:
 
         # Extract the modes and recombine them properly
-        if not rz_switch:
+        if coord_order is RZorder.mrz:
             F_total = np.zeros( (2 * Nr, Nz ) )
-        else:
+        elif coord_order is RZorder.mzr:
             F_total = np.zeros( (Nz, 2 * Nr ) )
+        else:
+            raise Exception(order_error_msg)
         if m == 'all':
             # Sum of all the modes
             # - Prepare the multiplier arrays
             mult_above_axis = [1]
             mult_below_axis = [1]
             for mode in range(1, int(Nm / 2) + 1):
                 cos = np.cos( mode * theta )
                 sin = np.sin( mode * theta )
                 mult_above_axis += [cos, sin]
                 mult_below_axis += [ (-1) ** mode * cos, (-1) ** mode * sin ]
             mult_above_axis = np.array( mult_above_axis )
             mult_below_axis = np.array( mult_below_axis )
             # - Sum the modes
             F = get_data( dset )  # (Extracts all modes)
-            if not rz_switch:
+            if coord_order is RZorder.mrz:
                 F_total[Nr:, :] = np.tensordot( mult_above_axis,
                                                 F, axes=(0, 0) )[:, :]
                 F_total[:Nr, :] = np.tensordot( mult_below_axis,
                                                 F, axes=(0, 0) )[::-1, :]
-            else:
+            elif coord_order is RZorder.mzr:
                 F_total[:, Nr:] = np.tensordot( mult_above_axis,
                                                 F, axes=(0, 0) )[:, :]
                 F_total[:, :Nr] = np.tensordot( mult_below_axis,
                                                 F, axes=(0, 0) )[:, ::-1]
         elif m == 0:
             # Extract mode 0
             F = get_data( dset, 0, 0 )
-            if not rz_switch:
+            if coord_order is RZorder.mrz:
                 F_total[Nr:, :] = F[:, :]
                 F_total[:Nr, :] = F[::-1, :]
-            else:
+            elif coord_order is RZorder.mzr:
                 F_total[:, Nr:] = F[:, :]
                 F_total[:, :Nr] = F[:, ::-1]
+            else:
+                raise Exception(order_error_msg)
 
         else:
             # Extract higher mode
             cos = np.cos( m * theta )
             sin = np.sin( m * theta )
             F_cos = get_data( dset, 2 * m - 1, 0 )
             F_sin = get_data( dset, 2 * m, 0 )
             F = cos * F_cos + sin * F_sin
-            if not rz_switch:
+            if coord_order is RZorder.mrz:
                 F_total[Nr:, :] = F[:, :]
                 F_total[:Nr, :] = (-1) ** m * F[::-1, :]
-            else:
+            elif coord_order is RZorder.mzr:
                 F_total[:, Nr:] = F[:, :]
                 F_total[:, :Nr] = (-1) ** m * F[:, ::-1]
+            else:
+                raise Exception(order_error_msg)
 
     # Perform slicing if needed
     if slice_across is not None:
         # Slice field and clear metadata
         inverted_axes_dict = {info.axes[key]: key for key in info.axes.keys()}
         for count, slice_across_item in enumerate(slice_across):
             slicing_index = inverted_axes_dict[slice_across_item]
```

### Comparing `openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/data_reader/h5py_reader/params_reader.py` & `openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/data_reader/h5py_reader/params_reader.py`

 * *Files identical despite different names*

### Comparing `openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/data_reader/h5py_reader/particle_reader.py` & `openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/data_reader/h5py_reader/particle_reader.py`

 * *Files identical despite different names*

### Comparing `openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/data_reader/h5py_reader/utilities.py` & `openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/data_reader/h5py_reader/utilities.py`

 * *Files identical despite different names*

### Comparing `openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/data_reader/io_reader/field_reader.py` & `openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/data_reader/io_reader/field_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 
 Copyright 2020, openPMD-viewer contributors
 Author: Axel Huebl
 License: 3-Clause-BSD-LBNL
 """
 
 import numpy as np
+
 from .utilities import get_data
+from ...data_order import RZorder, order_error_msg
 from openpmd_viewer.openpmd_timeseries.field_metainfo import FieldMetaInformation
 from openpmd_viewer.openpmd_timeseries.utilities import construct_3d_from_circ
 
 
 def read_field_cartesian( series, iteration, field_name, component_name,
                           axis_labels, slice_relative_position, slice_across ):
     """
@@ -186,22 +188,25 @@
         component = field[component_name]
 
     # Extract the metainformation
     #   FIXME here and in h5py reader, we need to invert the order on 'F' for
     #         grid spacing/offset/position
 
     coord_labels = {ii: coord for (ii, coord) in enumerate(field.axis_labels)}
-    if coord_labels[0] == 'r':
-        rz_switch = False
+    coord_label_str = ''.join(coord_labels.values())
+    coord_label_str = 'm' + coord_label_str
+    coord_order = RZorder[coord_label_str]
+    if coord_order is RZorder.mrz:
         Nm, Nr, Nz = component.shape
         N_pair = (Nr, Nz)
-    else:
-        rz_switch = True
+    elif coord_order is RZorder.mzr:
         Nm, Nz, Nr = component.shape
         N_pair = (Nz, Nr)
+    else:
+        raise Exception(order_error_msg)
 
     # Nm, Nr, Nz = component.shape
     info = FieldMetaInformation( coord_labels, N_pair,
         field.grid_spacing, field.grid_global_offset,
         field.grid_unit_SI, component.position, thetaMode=True )
 
     # Convert to a 3D Cartesian array if theta is None
@@ -221,99 +226,113 @@
         # If necessary, reduce resolution of 3D reconstruction
         if max_resolution_3d is not None:
             max_res_lon, max_res_transv = max_resolution_3d
             if Nz > max_res_lon:
                 # Calculate excess of elements along z
                 excess_z = int(np.round(Nz/max_res_lon))
                 # Preserve only one every excess_z elements
-                if not rz_switch:
+                if coord_order is RZorder.mrz:
                     Fcirc = Fcirc[:, :, ::excess_z]
-                else:
+                elif coord_order is RZorder.mzr:
                     Fcirc = Fcirc[:, ::excess_z, :]
+                else:
+                    raise Exception(order_error_msg)
                 # Update info accordingly
                 info.z = info.z[::excess_z]
                 info.dz = info.z[1] - info.z[0]
             if Nr > max_res_transv/2:
                 # Calculate excess of elements along r
                 excess_r = int(np.round(Nr/(max_res_transv/2)))
                 # Preserve only one every excess_r elements
-                if not rz_switch:
+                if coord_order is RZorder.mrz:
                     Fcirc = Fcirc[:, ::excess_r, :]
-                else:
+                elif coord_order is RZorder.mzr:
                     Fcirc = Fcirc[:, :, ::excess_r]
+                else:
+                    raise Exception(order_error_msg)
                 # Update info and necessary parameters accordingly
                 info.r = info.r[::excess_r]
                 info.dr = info.r[1] - info.r[0]
                 inv_dr = 1./info.dr
                 # Update Nr after reducing radial resolution.
-                if not rz_switch:
+                if coord_order is RZorder.mrz:
                     Nr = Fcirc.shape[1]
-                else:
+                elif coord_order is RZorder.mzr:
                     Nr = Fcirc.shape[2]
+                else:
+                    raise Exception(order_error_msg)
 
         # Convert cylindrical data to Cartesian data
         info._convert_cylindrical_to_3Dcartesian()
         nx, ny, nz = len(info.x), len(info.y), len(info.z)
         F_total = np.zeros( (nx, ny, nz) )
         construct_3d_from_circ( F_total, Fcirc, info.x, info.y, modes,
-            nx, ny, nz, Nr, nmodes, inv_dr, rmax, rz_switch=rz_switch)
+            nx, ny, nz, Nr, nmodes, inv_dr, rmax, coord_order)
 
     else:
 
         # Extract the modes and recombine them properly
-        if not rz_switch:
+        if coord_order is RZorder.mrz:
             F_total = np.zeros( (2 * Nr, Nz ) )
-        else:
+        elif coord_order is RZorder.mzr:
             F_total = np.zeros( (Nz, 2 * Nr ) )
+        else:
+            raise Exception(order_error_msg)
         if m == 'all':
             # Sum of all the modes
             # - Prepare the multiplier arrays
             mult_above_axis = [1]
             mult_below_axis = [1]
             for mode in range(1, int(Nm / 2) + 1):
                 cos = np.cos( mode * theta )
                 sin = np.sin( mode * theta )
                 mult_above_axis += [cos, sin]
                 mult_below_axis += [ (-1) ** mode * cos, (-1) ** mode * sin ]
             mult_above_axis = np.array( mult_above_axis )
             mult_below_axis = np.array( mult_below_axis )
             # - Sum the modes
             F = get_data( series, component )  # (Extracts all modes)
-            if not rz_switch:
+            if coord_order is RZorder.mrz:
                 F_total[Nr:, :] = np.tensordot( mult_above_axis,
                                                 F, axes=(0, 0) )[:, :]
                 F_total[:Nr, :] = np.tensordot( mult_below_axis,
                                                 F, axes=(0, 0) )[::-1, :]
-            else:
+            elif coord_order is RZorder.mzr:
                 F_total[:, Nr:] = np.tensordot( mult_above_axis,
                                                 F, axes=(0, 0) )[:, :]
                 F_total[:, :Nr] = np.tensordot( mult_below_axis,
                                                 F, axes=(0, 0) )[:, ::-1]
+            else:
+                raise Exception(order_error_msg)
         elif m == 0:
             # Extract mode 0
             F = get_data( series, component, 0, 0 )
-            if not rz_switch:
+            if coord_order is RZorder.mrz:
                 F_total[Nr:, :] = F[:, :]
                 F_total[:Nr, :] = F[::-1, :]
-            else:
+            elif coord_order is RZorder.mzr:
                 F_total[:, Nr:] = F[:, :]
                 F_total[:, :Nr] = F[:, ::-1]
+            else:
+                raise Exception(order_error_msg)
         else:
             # Extract higher mode
             cos = np.cos( m * theta )
             sin = np.sin( m * theta )
             F_cos = get_data( series, component, 2 * m - 1, 0 )
             F_sin = get_data( series, component, 2 * m, 0 )
             F = cos * F_cos + sin * F_sin
-            if not rz_switch:
+            if coord_order is RZorder.mrz:
                 F_total[Nr:, :] = F[:, :]
                 F_total[:Nr, :] = (-1) ** m * F[::-1, :]
-            else:
+            elif coord_order is RZorder.mzr:
                 F_total[:, Nr:] = F[:, :]
                 F_total[:, :Nr] = (-1) ** m * F[:, ::-1]
+            else:
+                raise Exception(order_error_msg)
 
     # Perform slicing if needed
     if slice_across is not None:
         # Slice field and clear metadata
         inverted_axes_dict = {info.axes[key]: key for key in info.axes.keys()}
         for count, slice_across_item in enumerate(slice_across):
             slicing_index = inverted_axes_dict[slice_across_item]
```

### Comparing `openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/data_reader/io_reader/params_reader.py` & `openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/data_reader/io_reader/params_reader.py`

 * *Files identical despite different names*

### Comparing `openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/data_reader/io_reader/particle_reader.py` & `openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/data_reader/io_reader/particle_reader.py`

 * *Files identical despite different names*

### Comparing `openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/data_reader/io_reader/utilities.py` & `openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/data_reader/io_reader/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,18 +142,20 @@
                 series.flush()
                 data[s_target] = x
 
     # Convert to the right type
     if (output_type is not None) and (data.dtype != output_type):
         data = data.astype( output_type )
     # Scale by the conversion factor
-    if np.issubdtype(data.dtype, np.floating) or \
-        np.issubdtype(data.dtype, np.complexfloating):
-        if record_component.unit_SI != 1.0:
+    if record_component.unit_SI != 1.0:
+        if np.issubdtype(data.dtype, np.floating) or \
+            np.issubdtype(data.dtype, np.complexfloating):
             data *= record_component.unit_SI
+        else:
+            data = data * record_component.unit_SI
 
     return data
 
 
 def join_infile_path(*paths):
     """
     Join path components using '/' as separator.
```

### Comparing `openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/field_metainfo.py` & `openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/field_metainfo.py`

 * *Files identical despite different names*

### Comparing `openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/interactive.py` & `openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/interactive.py`

 * *Files identical despite different names*

### Comparing `openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/main.py` & `openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/main.py`

 * *Files identical despite different names*

### Comparing `openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/numba_wrapper.py` & `openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/numba_wrapper.py`

 * *Files identical despite different names*

### Comparing `openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/particle_tracker.py` & `openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/particle_tracker.py`

 * *Files identical despite different names*

### Comparing `openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/plotter.py` & `openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/plotter.py`

 * *Files identical despite different names*

### Comparing `openPMD-viewer-1.6.0/openpmd_viewer/openpmd_timeseries/utilities.py` & `openPMD-viewer-1.7.0/openpmd_viewer/openpmd_timeseries/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 License: 3-Clause-BSD-LBNL
 """
 
 import copy
 import math
 import numpy as np
 from .numba_wrapper import jit
+from .data_order import RZorder, order_error_msg
 
 def sanitize_slicing(slice_across, slice_relative_position):
     """
     Return standardized format for `slice_across` and `slice_relative_position`:
     - either `slice_across` and `slice_relative_position` are both `None` (no slicing)
     - or `slice_across` and `slice_relative_position` are both lists,
     with the same number of elements
@@ -295,15 +296,15 @@
                 hist_data[ i1_low_bin+1, i2_low_bin+1 ] += w[i]*(1.-S1_low)*(1.-S2_low)
 
     return( hist_data )
 
 
 @jit
 def construct_3d_from_circ( F3d, Fcirc, x_array, y_array, modes,
-    nx, ny, nz, nr, nmodes, inv_dr, rmax, rz_switch = False ):
+    nx, ny, nz, nr, nmodes, inv_dr, rmax, coord_order): 
     """
     Reconstruct the field from a quasi-cylindrical simulation (`Fcirc`), as
     a 3D cartesian array (`F3d`).
     """
     for ix in range(nx):
         x = x_array[ix]
         for iy in range(ny):
@@ -317,23 +318,27 @@
             if ir >= nr:
                 ir = nr-1
 
             # Calculate linear projection from ir and ir-1
             if ir>0:
                 s0 = ir + 0.5 - r* inv_dr
                 s1 = 1. - s0
-                if not rz_switch:
+                if coord_order is RZorder.mrz:
                     Fcirc_proj = s1*Fcirc[:, ir, :] + s0*Fcirc[:, ir-1, :]
-                else:
+                elif coord_order is RZorder.mzr:
                     Fcirc_proj = s1*Fcirc[:, :, ir] + s0*Fcirc[:, :, ir-1]
+                else:
+                    raise Exception(order_error_msg)
             else:
-                if not rz_switch:
+                if coord_order is RZorder.mrz:
                     Fcirc_proj = Fcirc[:, ir, :]
-                else:
+                elif coord_order is RZorder.mzr:
                     Fcirc_proj = Fcirc[:, :, ir]
+                else:
+                    raise Exception(order_error_msg)
 
             # Loop over all modes and recontruct data
             if r == 0:
                 expItheta = 1. + 0.j
             else:
                 expItheta = (x+1.j*y)/r
```

### Comparing `openPMD-viewer-1.6.0/opmd_viewer/__init__.py` & `openPMD-viewer-1.7.0/opmd_viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `openPMD-viewer-1.6.0/setup.py` & `openPMD-viewer-1.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,25 +43,25 @@
         'plot': ["matplotlib"],
         'tutorials': ["ipywidgets", "ipympl", "matplotlib", "wget"],
         'numba': ["numba"],
         'openpmd-api': ["openpmd-api~=0.14.0"]
         },
       cmdclass={'test': PyTest},
       platforms='any',
-      python_requires='>=3.6',
+      python_requires='>=3.7',
       classifiers=[
           'Programming Language :: Python',
           'Development Status :: 4 - Beta',
           'Natural Language :: English',
           'Environment :: Console',
           'Intended Audience :: Science/Research',
           'Operating System :: OS Independent',
           'Topic :: Scientific/Engineering :: Physics',
           'Topic :: Scientific/Engineering :: Visualization',
           'Topic :: Database :: Front-Ends',
           'Programming Language :: Python :: 3',
-          'Programming Language :: Python :: 3.6',
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
-          'Programming Language :: Python :: 3.10'],
+          'Programming Language :: Python :: 3.10',
+          'Programming Language :: Python :: 3.11'],
       )
```

