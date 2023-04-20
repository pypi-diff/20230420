# Comparing `tmp/dckit-0.9.0.tar.gz` & `tmp/dckit-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dckit-0.9.0.tar", last modified: Mon May 25 16:30:23 2020, max compression
+gzip compressed data, was "dist/dckit-0.9.1.tar", last modified: Fri Jun  5 09:10:28 2020, max compression
```

## Comparing `dckit-0.9.0.tar` & `dckit-0.9.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-25 16:30:23.000000 dckit-0.9.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)      153 2020-05-25 16:29:15.000000 dckit-0.9.0/MANIFEST.in
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-25 16:30:23.000000 dckit-0.9.0/dckit.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2710 2020-05-25 16:30:23.000000 dckit-0.9.0/dckit.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-05-25 16:30:23.000000 dckit-0.9.0/dckit.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2020-05-25 16:30:23.000000 dckit-0.9.0/dckit.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      671 2020-05-25 16:30:23.000000 dckit-0.9.0/dckit.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       76 2020-05-25 16:30:23.000000 dckit-0.9.0/dckit.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       43 2020-05-25 16:30:23.000000 dckit-0.9.0/dckit.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2710 2020-05-25 16:30:23.000000 dckit-0.9.0/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-25 16:30:23.000000 dckit-0.9.0/dckit/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7137 2020-05-25 16:29:15.000000 dckit-0.9.0/dckit/main.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     1796 2020-05-25 16:29:15.000000 dckit-0.9.0/dckit/dlg_log.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     5349 2020-05-25 16:29:15.000000 dckit-0.9.0/dckit/meta_tool.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7095 2020-05-25 16:29:15.000000 dckit-0.9.0/dckit/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2182 2020-05-25 16:29:15.000000 dckit-0.9.0/dckit/history.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-25 16:30:23.000000 dckit-0.9.0/dckit/img/
--rw-rw-r--   0 travis    (2000) travis    (2000)    42784 2020-05-25 16:29:15.000000 dckit-0.9.0/dckit/img/splash.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     3293 2020-05-25 16:29:15.000000 dckit-0.9.0/dckit/img/icon.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     2666 2020-05-25 16:29:15.000000 dckit-0.9.0/dckit/dlg_join.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     1115 2020-05-25 16:29:15.000000 dckit-0.9.0/dckit/__main__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2991 2020-05-25 16:29:15.000000 dckit-0.9.0/dckit/dlg_repack.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     7693 2020-05-25 16:29:15.000000 dckit-0.9.0/dckit/dlg_icheck.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     3064 2020-05-25 16:29:15.000000 dckit-0.9.0/dckit/update.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27807 2020-05-25 16:29:15.000000 dckit-0.9.0/dckit/main.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       59 2020-05-25 16:29:15.000000 dckit-0.9.0/dckit/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       82 2020-05-25 16:29:19.000000 dckit-0.9.0/dckit/_version_save.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8443 2020-05-25 16:29:15.000000 dckit-0.9.0/dckit/dlg_icheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       98 2020-05-25 16:30:23.000000 dckit-0.9.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2855 2020-05-25 16:29:15.000000 dckit-0.9.0/CHANGELOG
--rw-rw-r--   0 travis    (2000) travis    (2000)    35149 2020-05-25 16:29:15.000000 dckit-0.9.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     1817 2020-05-25 16:29:15.000000 dckit-0.9.0/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1446 2020-05-25 16:29:15.000000 dckit-0.9.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-25 16:30:23.000000 dckit-0.9.0/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3576 2020-05-25 16:29:15.000000 dckit-0.9.0/tests/test_gui_basic.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2988 2020-05-25 16:29:15.000000 dckit-0.9.0/tests/helper_methods.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-25 16:30:23.000000 dckit-0.9.0/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)    40059 2020-05-25 16:29:15.000000 dckit-0.9.0/tests/data/rtdc_data_traces_video.zip
--rw-rw-r--   0 travis    (2000) travis    (2000)    98573 2020-05-25 16:29:15.000000 dckit-0.9.0/tests/data/rtdc_data_hdf5_rtfdc.zip
--rw-rw-r--   0 travis    (2000) travis    (2000)     1538 2020-05-25 16:29:15.000000 dckit-0.9.0/tests/test_history.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-05 09:10:28.000000 dckit-0.9.1/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      153 2020-06-05 09:09:18.000000 dckit-0.9.1/MANIFEST.in
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-05 09:10:28.000000 dckit-0.9.1/dckit.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2710 2020-06-05 09:10:28.000000 dckit-0.9.1/dckit.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-06-05 09:10:28.000000 dckit-0.9.1/dckit.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        6 2020-06-05 09:10:28.000000 dckit-0.9.1/dckit.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      671 2020-06-05 09:10:28.000000 dckit-0.9.1/dckit.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       76 2020-06-05 09:10:28.000000 dckit-0.9.1/dckit.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       43 2020-06-05 09:10:28.000000 dckit-0.9.1/dckit.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2710 2020-06-05 09:10:28.000000 dckit-0.9.1/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-05 09:10:28.000000 dckit-0.9.1/dckit/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7137 2020-06-05 09:09:18.000000 dckit-0.9.1/dckit/main.ui
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1796 2020-06-05 09:09:18.000000 dckit-0.9.1/dckit/dlg_log.ui
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5349 2020-06-05 09:09:18.000000 dckit-0.9.1/dckit/meta_tool.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7095 2020-06-05 09:09:18.000000 dckit-0.9.1/dckit/_version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2182 2020-06-05 09:09:18.000000 dckit-0.9.1/dckit/history.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-05 09:10:28.000000 dckit-0.9.1/dckit/img/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42784 2020-06-05 09:09:18.000000 dckit-0.9.1/dckit/img/splash.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3293 2020-06-05 09:09:18.000000 dckit-0.9.1/dckit/img/icon.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2666 2020-06-05 09:09:18.000000 dckit-0.9.1/dckit/dlg_join.ui
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1115 2020-06-05 09:09:18.000000 dckit-0.9.1/dckit/__main__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2991 2020-06-05 09:09:18.000000 dckit-0.9.1/dckit/dlg_repack.ui
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7693 2020-06-05 09:09:18.000000 dckit-0.9.1/dckit/dlg_icheck.ui
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3064 2020-06-05 09:09:18.000000 dckit-0.9.1/dckit/update.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28089 2020-06-05 09:09:18.000000 dckit-0.9.1/dckit/main.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       59 2020-06-05 09:09:18.000000 dckit-0.9.1/dckit/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       82 2020-06-05 09:09:29.000000 dckit-0.9.1/dckit/_version_save.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8443 2020-06-05 09:09:18.000000 dckit-0.9.1/dckit/dlg_icheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       98 2020-06-05 09:10:28.000000 dckit-0.9.1/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3010 2020-06-05 09:09:18.000000 dckit-0.9.1/CHANGELOG
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35149 2020-06-05 09:09:18.000000 dckit-0.9.1/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1817 2020-06-05 09:09:18.000000 dckit-0.9.1/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1446 2020-06-05 09:09:18.000000 dckit-0.9.1/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-05 09:10:28.000000 dckit-0.9.1/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3576 2020-06-05 09:09:18.000000 dckit-0.9.1/tests/test_gui_basic.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2988 2020-06-05 09:09:18.000000 dckit-0.9.1/tests/helper_methods.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-05 09:10:28.000000 dckit-0.9.1/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40059 2020-06-05 09:09:18.000000 dckit-0.9.1/tests/data/rtdc_data_traces_video.zip
+-rw-rw-r--   0 travis    (2000) travis    (2000)    98573 2020-06-05 09:09:18.000000 dckit-0.9.1/tests/data/rtdc_data_hdf5_rtfdc.zip
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1538 2020-06-05 09:09:18.000000 dckit-0.9.1/tests/test_history.py
```

### Comparing `dckit-0.9.0/dckit.egg-info/PKG-INFO` & `dckit-0.9.1/dckit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dckit
-Version: 0.9.0
+Version: 0.9.1
 Summary: Graphical toolkit for RT-DC data management
 Home-page: https://github.com/ZELLMECHANIK-DRESDEN/DCKit
 Author: Paul Müller
 Author-email: dev@craban.de
 License: GPL v3
 Description: |DCKit|
         =======
```

### Comparing `dckit-0.9.0/dckit.egg-info/SOURCES.txt` & `dckit-0.9.1/dckit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dckit-0.9.0/PKG-INFO` & `dckit-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dckit
-Version: 0.9.0
+Version: 0.9.1
 Summary: Graphical toolkit for RT-DC data management
 Home-page: https://github.com/ZELLMECHANIK-DRESDEN/DCKit
 Author: Paul Müller
 Author-email: dev@craban.de
 License: GPL v3
 Description: |DCKit|
         =======
```

### Comparing `dckit-0.9.0/dckit/main.ui` & `dckit-0.9.1/dckit/main.ui`

 * *Files identical despite different names*

### Comparing `dckit-0.9.0/dckit/dlg_log.ui` & `dckit-0.9.1/dckit/dlg_log.ui`

 * *Files identical despite different names*

### Comparing `dckit-0.9.0/dckit/meta_tool.py` & `dckit-0.9.1/dckit/meta_tool.py`

 * *Files identical despite different names*

### Comparing `dckit-0.9.0/dckit/_version.py` & `dckit-0.9.1/dckit/_version.py`

 * *Files identical despite different names*

### Comparing `dckit-0.9.0/dckit/history.py` & `dckit-0.9.1/dckit/history.py`

 * *Files identical despite different names*

### Comparing `dckit-0.9.0/dckit/img/splash.png` & `dckit-0.9.1/dckit/img/splash.png`

 * *Files identical despite different names*

### Comparing `dckit-0.9.0/dckit/img/icon.png` & `dckit-0.9.1/dckit/img/icon.png`

 * *Files identical despite different names*

### Comparing `dckit-0.9.0/dckit/dlg_join.ui` & `dckit-0.9.1/dckit/dlg_join.ui`

 * *Files identical despite different names*

### Comparing `dckit-0.9.0/dckit/__main__.py` & `dckit-0.9.1/dckit/__main__.py`

 * *Files identical despite different names*

### Comparing `dckit-0.9.0/dckit/dlg_repack.ui` & `dckit-0.9.1/dckit/dlg_repack.ui`

 * *Files identical despite different names*

### Comparing `dckit-0.9.0/dckit/dlg_icheck.ui` & `dckit-0.9.1/dckit/dlg_icheck.ui`

 * *Files identical despite different names*

### Comparing `dckit-0.9.0/dckit/update.py` & `dckit-0.9.1/dckit/update.py`

 * *Files identical despite different names*

### Comparing `dckit-0.9.0/dckit/main.py` & `dckit-0.9.1/dckit/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,20 @@
         # Help menu
         self.actionSoftware.triggered.connect(self.on_action_software)
         self.actionAbout.triggered.connect(self.on_action_about)
         #: contains all imported paths (index is DCKit-id)
         self.pathlist = []
         # contains all integrity buttons (keys are DCKit-ids)
         self.integrity_buttons = {}
+        # if "--version" was specified, print the version and exit
+        if "--version" in sys.argv:
+            print(__version__)
+            QtWidgets.QApplication.processEvents()
+            sys.exit(0)
+        # check update after version printing (QThread: Destroyed error)
         if check_update:
             # Update Check
             self.on_action_check_update(True)
 
     def append_paths(self, pathlist):
         """Append selected paths to table"""
         QtWidgets.QApplication.setOverrideCursor(QtCore.Qt.WaitCursor)
```

### Comparing `dckit-0.9.0/dckit/dlg_icheck.py` & `dckit-0.9.1/dckit/dlg_icheck.py`

 * *Files identical despite different names*

### Comparing `dckit-0.9.0/CHANGELOG` & `dckit-0.9.1/CHANGELOG`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+0.9.1
+ - enh: allow keyword argument --version (print version and exit)
+ - build: pin PyQt5 to 5.14.2 on Linux/macOS
+ - build: macOS build was not working
 0.9.0
  - fix: export file names were allowed to have invalid characters
  - fix: ignore ResourceWarning
  - enh: improved preview speed for .tdms data
  - setup: bump dclab from 0.25.0 to 0.27.5 (support ML features)
  - setup: bump imageio to >=2.8.0
  - setup: bump nptdms to >=0.27.0
```

### Comparing `dckit-0.9.0/LICENSE` & `dckit-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dckit-0.9.0/README.rst` & `dckit-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `dckit-0.9.0/setup.py` & `dckit-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `dckit-0.9.0/tests/test_gui_basic.py` & `dckit-0.9.1/tests/test_gui_basic.py`

 * *Files identical despite different names*

### Comparing `dckit-0.9.0/tests/helper_methods.py` & `dckit-0.9.1/tests/helper_methods.py`

 * *Files identical despite different names*

### Comparing `dckit-0.9.0/tests/data/rtdc_data_traces_video.zip` & `dckit-0.9.1/tests/data/rtdc_data_traces_video.zip`

 * *Files identical despite different names*

### Comparing `dckit-0.9.0/tests/data/rtdc_data_hdf5_rtfdc.zip` & `dckit-0.9.1/tests/data/rtdc_data_hdf5_rtfdc.zip`

 * *Files identical despite different names*

### Comparing `dckit-0.9.0/tests/test_history.py` & `dckit-0.9.1/tests/test_history.py`

 * *Files identical despite different names*

