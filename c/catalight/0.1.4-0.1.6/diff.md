# Comparing `tmp/catalight-0.1.4.tar.gz` & `tmp/catalight-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catalight-0.1.4.tar", last modified: Sat Mar  4 01:53:42 2023, max compression
+gzip compressed data, was "catalight-0.1.6.tar", last modified: Thu Apr 20 18:37:55 2023, max compression
```

## Comparing `catalight-0.1.4.tar` & `catalight-0.1.6.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-03-04 01:53:42.833459 catalight-0.1.4/
--rw-rw-rw-   0        0        0     1092 2023-01-17 01:38:58.000000 catalight-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     2274 2023-03-04 01:53:42.834456 catalight-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1678 2023-03-04 01:25:58.000000 catalight-0.1.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-04 01:53:42.244466 catalight-0.1.4/catalight/
--rw-rw-rw-   0        0        0       80 2023-03-03 02:17:34.000000 catalight-0.1.4/catalight/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-04 01:53:42.327056 catalight-0.1.4/catalight/analysis/
--rw-rw-rw-   0        0        0      380 2023-02-28 19:42:43.000000 catalight-0.1.4/catalight/analysis/__init__.py
--rw-rw-rw-   0        0        0     7351 2023-03-03 01:34:26.000000 catalight-0.1.4/catalight/analysis/chromatogram_scanner_gui.py
--rw-rw-rw-   0        0        0    14270 2023-03-03 02:21:45.000000 catalight-0.1.4/catalight/analysis/gcdata.py
--rw-rw-rw-   0        0        0     2489 2023-03-03 01:36:00.000000 catalight-0.1.4/catalight/analysis/make_empty_cal_expt.py
--rw-rw-rw-   0        0        0    16927 2023-03-03 02:43:01.000000 catalight-0.1.4/catalight/analysis/plotting.py
--rw-rw-rw-   0        0        0     3995 2023-03-03 02:45:07.000000 catalight-0.1.4/catalight/analysis/run_calibration.py
--rw-rw-rw-   0        0        0     5068 2023-03-03 02:46:39.000000 catalight-0.1.4/catalight/analysis/run_change_xdata.py
--rw-rw-rw-   0        0        0     6227 2023-03-03 01:39:59.000000 catalight-0.1.4/catalight/analysis/run_initial_analysis.py
--rw-rw-rw-   0        0        0     3752 2023-03-03 01:40:08.000000 catalight-0.1.4/catalight/analysis/run_plot_chromatograms_stacked.py
--rw-rw-rw-   0        0        0     4746 2023-03-03 23:24:19.000000 catalight-0.1.4/catalight/analysis/run_plot_comparison.py
--rw-rw-rw-   0        0        0    26565 2023-03-03 02:33:23.000000 catalight-0.1.4/catalight/analysis/tools.py
--rw-rw-rw-   0        0        0    20647 2023-03-03 01:44:09.000000 catalight-0.1.4/catalight/analysis/user_inputs.py
--rw-rw-rw-   0        0        0    46801 2023-03-01 22:42:41.000000 catalight-0.1.4/catalight/catalight_GUI.py
-drwxrwxrwx   0        0        0        0 2023-03-04 01:53:42.333040 catalight-0.1.4/catalight/equipment/
--rw-rw-rw-   0        0        0       81 2023-03-03 02:16:55.000000 catalight-0.1.4/catalight/equipment/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-04 01:53:42.378246 catalight-0.1.4/catalight/equipment/alicat_MFC/
--rw-rw-rw-   0        0        0      214 2023-03-03 02:15:51.000000 catalight-0.1.4/catalight/equipment/alicat_MFC/__init__.py
--rw-rw-rw-   0        0        0     1548 2023-03-03 02:03:42.000000 catalight-0.1.4/catalight/equipment/alicat_MFC/connection_tester.py
--rw-rw-rw-   0        0        0    13241 2023-03-03 01:52:54.000000 catalight-0.1.4/catalight/equipment/alicat_MFC/gas_control.py
-drwxrwxrwx   0        0        0        0 2023-03-04 01:53:42.381239 catalight-0.1.4/catalight/equipment/diode_laser/
--rw-rw-rw-   0        0        0      215 2023-03-03 02:13:39.000000 catalight-0.1.4/catalight/equipment/diode_laser/__init__.py
--rw-rw-rw-   0        0        0    16628 2023-03-03 01:52:00.000000 catalight-0.1.4/catalight/equipment/diode_laser/diode_control.py
--rw-rw-rw-   0        0        0    38102 2023-03-03 23:24:19.000000 catalight-0.1.4/catalight/equipment/experiment_control.py
--rw-rw-rw-   0        0        0     4399 2023-03-02 21:52:12.000000 catalight-0.1.4/catalight/equipment/gc_delay_tester.py
-drwxrwxrwx   0        0        0        0 2023-03-04 01:53:42.391219 catalight-0.1.4/catalight/equipment/harrick_watlow/
--rw-rw-rw-   0        0        0      210 2023-03-03 02:12:49.000000 catalight-0.1.4/catalight/equipment/harrick_watlow/__init__.py
--rw-rw-rw-   0        0        0     8798 2023-03-03 01:50:42.000000 catalight-0.1.4/catalight/equipment/harrick_watlow/heater_control.py
-drwxrwxrwx   0        0        0        0 2023-03-04 01:53:42.393207 catalight-0.1.4/catalight/equipment/nkt_laser/
--rw-rw-rw-   0        0        0       90 2023-01-17 00:29:35.000000 catalight-0.1.4/catalight/equipment/nkt_laser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-04 01:53:42.780602 catalight-0.1.4/catalight/equipment/power_meter/
--rw-rw-rw-   0        0        0      215 2023-03-03 02:14:21.000000 catalight-0.1.4/catalight/equipment/power_meter/__init__.py
--rw-rw-rw-   0        0        0     2079 2023-01-31 00:37:57.000000 catalight-0.1.4/catalight/equipment/power_meter/demo.py
--rw-rw-rw-   0        0        0     2950 2023-03-03 01:50:11.000000 catalight-0.1.4/catalight/equipment/power_meter/power_meter_ctrl.py
--rw-rw-rw-   0        0        0     4112 2023-03-03 01:45:42.000000 catalight-0.1.4/catalight/equipment/run_diode_calibration.py
-drwxrwxrwx   0        0        0        0 2023-03-04 01:53:42.830295 catalight-0.1.4/catalight/equipment/sri_gc/
--rw-rw-rw-   0        0        0      267 2023-03-03 02:15:11.000000 catalight-0.1.4/catalight/equipment/sri_gc/__init__.py
--rw-rw-rw-   0        0        0    12071 2023-03-03 01:49:31.000000 catalight-0.1.4/catalight/equipment/sri_gc/gc_control.py
--rw-rw-rw-   0        0        0      979 2023-01-31 00:30:40.000000 catalight-0.1.4/catalight/equipment/sri_gc/peaksimple_control_demo.py
-drwxrwxrwx   0        0        0        0 2023-03-04 01:53:42.259348 catalight-0.1.4/catalight.egg-info/
--rw-rw-rw-   0        0        0     2274 2023-03-04 01:53:42.000000 catalight-0.1.4/catalight.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1526 2023-03-04 01:53:42.000000 catalight-0.1.4/catalight.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-04 01:53:42.000000 catalight-0.1.4/catalight.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      301 2023-03-04 01:53:42.000000 catalight-0.1.4/catalight.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-04 01:53:42.000000 catalight-0.1.4/catalight.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      805 2023-03-04 01:51:33.000000 catalight-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0      452 2023-03-04 01:53:42.835453 catalight-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1187 2023-01-31 05:23:17.000000 catalight-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 18:37:55.221634 catalight-0.1.6/
+-rw-rw-rw-   0        0        0     1092 2023-01-17 01:38:58.000000 catalight-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     2276 2023-04-20 18:37:55.222671 catalight-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1680 2023-04-04 02:45:53.000000 catalight-0.1.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-20 18:37:55.095066 catalight-0.1.6/catalight/
+-rw-rw-rw-   0        0        0       80 2023-03-03 02:17:34.000000 catalight-0.1.6/catalight/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 18:37:55.176777 catalight-0.1.6/catalight/analysis/
+-rw-rw-rw-   0        0        0      380 2023-02-28 19:42:43.000000 catalight-0.1.6/catalight/analysis/__init__.py
+-rw-rw-rw-   0        0        0     8813 2023-04-20 18:35:36.000000 catalight-0.1.6/catalight/analysis/chromatogram_scanner_gui.py
+-rw-rw-rw-   0        0        0    14326 2023-04-20 18:35:36.000000 catalight-0.1.6/catalight/analysis/gcdata.py
+-rw-rw-rw-   0        0        0     2489 2023-03-03 01:36:00.000000 catalight-0.1.6/catalight/analysis/make_empty_cal_expt.py
+-rw-rw-rw-   0        0        0    16927 2023-03-03 02:43:01.000000 catalight-0.1.6/catalight/analysis/plotting.py
+-rw-rw-rw-   0        0        0     3995 2023-03-03 02:45:07.000000 catalight-0.1.6/catalight/analysis/run_calibration.py
+-rw-rw-rw-   0        0        0     5068 2023-03-03 02:46:39.000000 catalight-0.1.6/catalight/analysis/run_change_xdata.py
+-rw-rw-rw-   0        0        0     6227 2023-03-03 01:39:59.000000 catalight-0.1.6/catalight/analysis/run_initial_analysis.py
+-rw-rw-rw-   0        0        0     3752 2023-03-03 01:40:08.000000 catalight-0.1.6/catalight/analysis/run_plot_chromatograms_stacked.py
+-rw-rw-rw-   0        0        0     4746 2023-03-03 23:24:19.000000 catalight-0.1.6/catalight/analysis/run_plot_comparison.py
+-rw-rw-rw-   0        0        0    26803 2023-04-20 18:35:36.000000 catalight-0.1.6/catalight/analysis/tools.py
+-rw-rw-rw-   0        0        0    20598 2023-04-20 18:35:36.000000 catalight-0.1.6/catalight/analysis/user_inputs.py
+-rw-rw-rw-   0        0        0    46788 2023-04-20 18:35:36.000000 catalight-0.1.6/catalight/catalight_GUI.py
+drwxrwxrwx   0        0        0        0 2023-04-20 18:37:55.184755 catalight-0.1.6/catalight/equipment/
+-rw-rw-rw-   0        0        0       81 2023-03-03 02:16:55.000000 catalight-0.1.6/catalight/equipment/__init__.py
+-rw-rw-rw-   0        0        0     1548 2023-04-20 18:35:36.000000 catalight-0.1.6/catalight/equipment/alicat_connection_tester.py
+-rw-rw-rw-   0        0        0    38064 2023-04-20 18:35:36.000000 catalight-0.1.6/catalight/equipment/experiment_control.py
+drwxrwxrwx   0        0        0        0 2023-04-20 18:37:55.193732 catalight-0.1.6/catalight/equipment/gas_control/
+-rw-rw-rw-   0        0        0      214 2023-04-20 18:35:36.000000 catalight-0.1.6/catalight/equipment/gas_control/__init__.py
+-rw-rw-rw-   0        0        0    13246 2023-04-20 18:35:36.000000 catalight-0.1.6/catalight/equipment/gas_control/alicat.py
+-rw-rw-rw-   0        0        0    12495 2023-04-20 18:35:36.000000 catalight-0.1.6/catalight/equipment/gas_control/template.py
+drwxrwxrwx   0        0        0        0 2023-04-20 18:37:55.205726 catalight-0.1.6/catalight/equipment/gc_control/
+-rw-rw-rw-   0        0        0      267 2023-04-20 18:35:36.000000 catalight-0.1.6/catalight/equipment/gc_control/__init__.py
+-rw-rw-rw-   0        0        0      979 2023-04-20 18:35:36.000000 catalight-0.1.6/catalight/equipment/gc_control/peaksimple_control_demo.py
+-rw-rw-rw-   0        0        0    12525 2023-04-20 18:35:36.000000 catalight-0.1.6/catalight/equipment/gc_control/sri_gc.py
+-rw-rw-rw-   0        0        0     5370 2023-04-20 18:35:36.000000 catalight-0.1.6/catalight/equipment/gc_control/template.py
+-rw-rw-rw-   0        0        0     4380 2023-04-20 18:35:36.000000 catalight-0.1.6/catalight/equipment/gc_delay_tester.py
+drwxrwxrwx   0        0        0        0 2023-04-20 18:37:55.212057 catalight-0.1.6/catalight/equipment/heating/
+-rw-rw-rw-   0        0        0      210 2023-04-20 18:35:36.000000 catalight-0.1.6/catalight/equipment/heating/__init__.py
+-rw-rw-rw-   0        0        0     9998 2023-04-20 18:35:36.000000 catalight-0.1.6/catalight/equipment/heating/template.py
+-rw-rw-rw-   0        0        0     8788 2023-04-20 18:35:36.000000 catalight-0.1.6/catalight/equipment/heating/watlow.py
+drwxrwxrwx   0        0        0        0 2023-04-20 18:37:55.216665 catalight-0.1.6/catalight/equipment/light_sources/
+-rw-rw-rw-   0        0        0      215 2023-04-20 18:35:36.000000 catalight-0.1.6/catalight/equipment/light_sources/__init__.py
+-rw-rw-rw-   0        0        0    16628 2023-04-20 18:35:36.000000 catalight-0.1.6/catalight/equipment/light_sources/diode_control.py
+-rw-rw-rw-   0        0        0    10225 2023-04-20 18:35:36.000000 catalight-0.1.6/catalight/equipment/light_sources/template.py
+drwxrwxrwx   0        0        0        0 2023-04-20 18:37:55.220636 catalight-0.1.6/catalight/equipment/power_meter/
+-rw-rw-rw-   0        0        0      215 2023-03-03 02:14:21.000000 catalight-0.1.6/catalight/equipment/power_meter/__init__.py
+-rw-rw-rw-   0        0        0     2950 2023-04-20 18:35:36.000000 catalight-0.1.6/catalight/equipment/power_meter/newport.py
+-rw-rw-rw-   0        0        0     4105 2023-04-20 18:35:36.000000 catalight-0.1.6/catalight/equipment/run_diode_calibration.py
+drwxrwxrwx   0        0        0        0 2023-04-20 18:37:55.157006 catalight-0.1.6/catalight.egg-info/
+-rw-rw-rw-   0        0        0     2276 2023-04-20 18:37:55.000000 catalight-0.1.6/catalight.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1591 2023-04-20 18:37:55.000000 catalight-0.1.6/catalight.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 18:37:55.000000 catalight-0.1.6/catalight.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      301 2023-04-20 18:37:55.000000 catalight-0.1.6/catalight.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-20 18:37:55.000000 catalight-0.1.6/catalight.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      805 2023-04-20 18:36:54.000000 catalight-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0      452 2023-04-20 18:37:55.229660 catalight-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1187 2023-01-31 05:23:17.000000 catalight-0.1.6/setup.py
```

### Comparing `catalight-0.1.4/LICENSE` & `catalight-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `catalight-0.1.4/PKG-INFO` & `catalight-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catalight
-Version: 0.1.4
+Version: 0.1.6
 Summary: Photoreactor system automation, data handling, and analysis.
 Author-email: Briley Bourgeois <bbourge6@stanford.edu>, Claire Carlin <cccarlin@stanford.edu>
 Project-URL: Homepage, https://github.com/Dionne-Lab/catalight
 Project-URL: Bug Tracker, https://github.com/Dionne-Lab/catalight/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 Welcome to Catalight!
 =======================
 .. figure:: https://raw.githubusercontent.com/Dionne-Lab/catalight/main/docs/source/_static/images/catalight_header_g.png
     :width: 800
 
 Introduction
 ------------
-Catalight is tool set developed by scientists at Stanford to help automate photocatalysis experiments. catalight is capable of connecting to hardware, coordinating instruments to run a variety of different experimental procedures, and organizing and analyzing data collected by the system. The project is designed in a modular format to enable users to bring their own unique hardware while still utilizing the core features of experiment management and data handling. The program functions in both a scripted version and a GUI to aid users in planning experimental procedures and manually controlling hardware.
+Catalight is a tool set developed by scientists at Stanford to help automate photocatalysis experiments. Catalight is capable of connecting to hardware, coordinating instruments to run a variety of different experimental procedures, and organizing and analyzing data collected by the system. The project is designed in a modular format to enable users to bring their own unique hardware while still utilizing the core features of experiment management and data handling. The program functions in both a scripted version and a GUI to aid users in planning experimental procedures and manually controlling hardware.
 
 To date, catalight is compatible with Alicat mass flow controllers, heater systems controlled by Watlow components, Measurement Computing data acquisition boards (used for communication with (ThorLabs laser diode drivers), NewPort 843-R power meter, and SRI gas chromatographs. Support for additional hardware is planned for the future, including FTIR data collection and analysis and NKT Photonics lasers. We strongly encourage interested users to consider contributing to the project by adding new device support and helping expand the catalight functionality.
 
 **ReadtheDocs Page:**
 https://catalight.readthedocs.io/en/latest/
 
 **PyPI Page:**
```

### Comparing `catalight-0.1.4/README.rst` & `catalight-0.1.6/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Welcome to Catalight!
 =======================
 .. figure:: https://raw.githubusercontent.com/Dionne-Lab/catalight/main/docs/source/_static/images/catalight_header_g.png
     :width: 800
 
 Introduction
 ------------
-Catalight is tool set developed by scientists at Stanford to help automate photocatalysis experiments. catalight is capable of connecting to hardware, coordinating instruments to run a variety of different experimental procedures, and organizing and analyzing data collected by the system. The project is designed in a modular format to enable users to bring their own unique hardware while still utilizing the core features of experiment management and data handling. The program functions in both a scripted version and a GUI to aid users in planning experimental procedures and manually controlling hardware.
+Catalight is a tool set developed by scientists at Stanford to help automate photocatalysis experiments. Catalight is capable of connecting to hardware, coordinating instruments to run a variety of different experimental procedures, and organizing and analyzing data collected by the system. The project is designed in a modular format to enable users to bring their own unique hardware while still utilizing the core features of experiment management and data handling. The program functions in both a scripted version and a GUI to aid users in planning experimental procedures and manually controlling hardware.
 
 To date, catalight is compatible with Alicat mass flow controllers, heater systems controlled by Watlow components, Measurement Computing data acquisition boards (used for communication with (ThorLabs laser diode drivers), NewPort 843-R power meter, and SRI gas chromatographs. Support for additional hardware is planned for the future, including FTIR data collection and analysis and NKT Photonics lasers. We strongly encourage interested users to consider contributing to the project by adding new device support and helping expand the catalight functionality.
 
 **ReadtheDocs Page:**
 https://catalight.readthedocs.io/en/latest/
 
 **PyPI Page:**
```

### Comparing `catalight-0.1.4/catalight/analysis/chromatogram_scanner_gui.py` & `catalight-0.1.6/catalight/analysis/chromatogram_scanner_gui.py`

 * *Files 21% similar despite different names*

```diff
@@ -88,23 +88,28 @@
     def init_plot(self):
         """Pull first data file and add to plot."""
         # Make the first file in the list appear as the plot upon opening
         # Get data from filepath
         path = self.listWidget.item(0).text()
         data = GCData(path, basecorrect=False)
         datacorr = GCData(path, basecorrect=True)
-
         # Plot pulled data
         self.data_line = self.graphWidget.plot(data.time, data.signal,
                                                pen=self.pen1, name="raw")
         self.data_line_corr = self.graphWidget.plot(datacorr.time,
                                                     datacorr.signal,
                                                     pen=self.pen2,
                                                     name="corrected")
-        self.data_line_corr.clear()
+        self.data_line_left = self.graphWidget.plot([0],[0],pen=None, symbol='o', name="left indices")
+        self.data_line_right = self.graphWidget.plot([0],[0],pen=None, symbol='o', name="right indices")
+        self.data_line_apex = self.graphWidget.plot([0],[0],pen=None, symbol='o', name="apex indices")
+        self.graphWidget.removeItem(self.data_line_corr)
+        self.graphWidget.removeItem(self.data_line_left)
+        self.graphWidget.removeItem(self.data_line_right)
+        self.graphWidget.removeItem(self.data_line_apex)
         self.graphWidget.setTitle('Run 0:', color="k", size="18pt")
 
     def set_graph_style(self):
         """Update graph appearance."""
         # graph styling things
         self.graphWidget.addLegend(labelTextColor="k", labelTextSize="14pt")
         self.graphWidget.setBackground('w')
@@ -123,17 +128,15 @@
         self.pen1 = pg.mkPen(color=(0, 102, 255), width=2)
         self.pen2 = pg.mkPen(color=(0, 153, 51), width=1)
 
     def update_plot(self):
         """Update plot with current listWidget item, if present."""
         if not self.listWidget.currentItem():
             print('No Items')
-            self.data_line.clear()
-            self.data_line_corr.clear()
-            self.graphWidget.setTitle('')
+            self.graphWidget.clear()
             return
 
         path = self.listWidget.currentItem().text()
         data = GCData(path, basecorrect=False)
         datacorr = GCData(path, basecorrect=True)
         num = self.filelist.index(path)
 
@@ -141,31 +144,50 @@
         self.graphWidget.setTitle("run " + str(num) + ":",
                                   color="k", size="18pt")
 
         # Update data, check if baseline correction is needed
         self.data_line.setData(data.time, data.signal,
                                pen=self.pen1, name="raw")
         if self.int_box.isChecked():
-            data.integration_inds()
-            [left_idx, right_idx] = (np.rint(data.lind).astype('int'),
-                                     np.rint(data.rind).astype('int'))
-            self.graphWidget.plot(data.time[data.apex_ind],
-                                  data.signal[data.apex_ind],
-                                  'bo', label='apex')
-            self.graphWidget.plot(data.time[left_idx],
-                                  data.signal[left_idx],
-                                  'go', label='left')
-            self.graphWidget.plot(data.time[right_idx],
-                                  data.signal[right_idx],
-                                  'ro', label='right')
+            if self.bc_box.isChecked():
+                data_ind = datacorr
+            else:
+                data_ind = data
+            if self.data_line_left not in self.graphWidget.listDataItems():
+                self.graphWidget.addItem(self.data_line_left)
+                self.graphWidget.addItem(self.data_line_right)
+                self.graphWidget.addItem(self.data_line_apex)
+
+            [left_idx, right_idx] = (np.rint(data_ind.lind).astype('int'), np.rint(data_ind.rind).astype('int'))
+            apex_idx = data.apex_ind
+            self.data_line_left.setData(data_ind.time[left_idx], data_ind.signal[left_idx],
+                                        pen=None,symbolBrush=(216,27,96),
+                                        symbol='o',symbolSize = 6,
+                                        name="left indices")
+            self.data_line_right.setData(data_ind.time[right_idx], data_ind.signal[right_idx],
+                                        pen=None,symbolBrush=(42,164,56),
+                                        symbol='o',symbolSize = 6)
+            self.data_line_apex.setData(data_ind.time[apex_idx], data_ind.signal[apex_idx],
+                                        pen=None,symbolBrush=(76,206,241),
+                                        symbol='o',symbolSize = 6)
+
+        else:
+            self.graphWidget.removeItem(self.data_line_left)
+            self.graphWidget.removeItem(self.data_line_right)
+            self.graphWidget.removeItem(self.data_line_apex)
+
         if self.bc_box.isChecked():
+            if self.data_line_corr not in self.graphWidget.listDataItems() :
+                self.graphWidget.addItem(self.data_line_corr)
+
             self.data_line_corr.setData(datacorr.time, datacorr.signal,
                                         pen=self.pen2, name="corrected")
         else:
-            self.data_line_corr.clear()
+            #self.data_line_corr.clear()
+            self.graphWidget.removeItem(self.data_line_corr)
 
 
 if __name__ == "__main__":
 
     app = QApplication(sys.argv)
     window = MainWindow()
     window.show()
```

### Comparing `catalight-0.1.4/catalight/analysis/gcdata.py` & `catalight-0.1.6/catalight/analysis/gcdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         Use scipy.signal.find_peaks to find peaks in signal.
 
         Returns
         -------
         numpy.ndarray
             All peak locations (as integer indices NOT times)
         """
-        apex_ind, _ = scisig.find_peaks(self.signal, prominence=4)
+        apex_ind, _ = scisig.find_peaks(self.signal, prominence=0.2)
         return apex_ind
 
     def integration_inds(self):
         """
         Find bounds of integration for apexes.
 
         Edge values determined by self._half_index_search.
@@ -182,15 +182,15 @@
             rhs = self.signal[apex - 1:]
             rind[k] = apex + self._half_index_search(rhs)
             k += 1
 
         return lind.astype(int), rind.astype(int)
 
     @staticmethod
-    def _half_index_search(dat, tol=0.5):
+    def _half_index_search(dat, tol=0.1):
         """
         Support function for integration_inds to search for integration bounds.
 
         Determined where:
         1. the change in signal is less than 0.5%
             of the previous signal point (with averaging); or
         2. the added intensity starts increasing
@@ -240,24 +240,24 @@
         Find the area under the peak using a trapezoidal method.
 
         Calculate for each peak identified using bounds from integration_inds.
         Integrates peak trapezoidal in units of seconds*signal intensity.
 
         Returns
         -------
-        numpy.int32
-            counts rounded using np.around()
+        numpy.ndarray
+            counts for all peaks, rounded to three decimal places using np.around()
         """
         counts = np.zeros(self.numpeaks)
         for i in range(0, self.numpeaks):
             counts[i] = np.trapz(self.signal[self.lind[i]:self.rind[i]],
                                  x=60 * self.time[self.lind[i]:self.rind[i]])
             if counts[i] == 0:
                 counts[i] = 1
-        return np.around(counts)
+        return np.around(counts,decimals=3)
 
     def get_concentrations(self, calDF):
         """
         Return a Pandas series of chemical concentrations.
 
         Output has the same order as the calibration file chem IDs.
         Prints warning if zero molecules are detected or if peaks are found
@@ -274,15 +274,15 @@
             Concentrations for each peak in apex_ind, given in ppm
         Notes
         -----
             Unknown peaks could be added to calibration dataframe for reference
         """
         # TODO Unknown peaks could be added
         # to calibration dataframe for reference
-        self.integration_inds()
+        #self.integration_inds()
         # Creates empty series where index are ChemIDs from Cal file
         conc = pd.Series(0.0, index=['timestamp', *calDF.index.to_list()])
         conc['timestamp'] = self.timestamp
         counts = self.integrate_peak()
         UnknownPeaks = 0
         for i in range(len(self.apex_ind)):
             # Determine peak time based on index
@@ -323,15 +323,15 @@
         # with data_analysis module.
         plt.rcParams.update({'font.size': 14})
         plt.rcParams['axes.linewidth'] = 2
         plt.gca().tick_params(which='both', width=1.5, length=6)
         plt.gca().tick_params(which='minor', width=1.5, length=3)
 
         plt.figure
-        self.integration_inds()
+        #self.integration_inds()
         [left_idx, right_idx] = (np.rint(self.lind).astype('int'),
                                  np.rint(self.rind).astype('int'))
         # Plot signal
         plt.plot(self.time, self.signal, linewidth=2.5)
         # Plot Derivative
         # plt.plot(time, 10*np.gradient(signal))
         # Plot peak and bounds
```

### Comparing `catalight-0.1.4/catalight/analysis/make_empty_cal_expt.py` & `catalight-0.1.6/catalight/analysis/make_empty_cal_expt.py`

 * *Files identical despite different names*

### Comparing `catalight-0.1.4/catalight/analysis/plotting.py` & `catalight-0.1.6/catalight/analysis/plotting.py`

 * *Files identical despite different names*

### Comparing `catalight-0.1.4/catalight/analysis/run_calibration.py` & `catalight-0.1.6/catalight/analysis/run_calibration.py`

 * *Files identical despite different names*

### Comparing `catalight-0.1.4/catalight/analysis/run_change_xdata.py` & `catalight-0.1.6/catalight/analysis/run_change_xdata.py`

 * *Files identical despite different names*

### Comparing `catalight-0.1.4/catalight/analysis/run_initial_analysis.py` & `catalight-0.1.6/catalight/analysis/run_initial_analysis.py`

 * *Files identical despite different names*

### Comparing `catalight-0.1.4/catalight/analysis/run_plot_chromatograms_stacked.py` & `catalight-0.1.6/catalight/analysis/run_plot_chromatograms_stacked.py`

 * *Files identical despite different names*

### Comparing `catalight-0.1.4/catalight/analysis/run_plot_comparison.py` & `catalight-0.1.6/catalight/analysis/run_plot_comparison.py`

 * *Files identical despite different names*

### Comparing `catalight-0.1.4/catalight/analysis/tools.py` & `catalight-0.1.6/catalight/analysis/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     for root in main_dirs:
         for dirpath, dirnames, filenames in os.walk(root):
             for filename in filenames:
                 if (filename.lower().endswith(suffix.lower())
                         & (target.lower() in filename.lower())):
                     filepath = os.path.join(dirpath, filename)
                     filepath_list.append(filepath)
+    # TODO sort filepath_list?
     return filepath_list
 
 
 def list_expt_obj(file_paths):
     """
     Get list of experiments.
 
@@ -353,20 +354,21 @@
         ax_calibration.ticklabel_format(axis='both', style='sci',
                                         scilimits=[-2, 2])
 
         # Fit w/ counts as 'y' and 'y_err'
         if force_zero:  # Add point (0, 0) w/ infinitesimal error
             x_data = np.append(0, expected_ppm)
             y_data = np.append(0, avg[chemical].to_numpy())
-            y_err = np.append(1e-19, std[chemical].to_numpy())
+            y_err = np.append(1, std[chemical].to_numpy())
         else:
             x_data = expected_ppm
             y_data = avg[chemical].to_numpy()
             y_err = std[chemical].to_numpy()
         try:
+            y_err[y_err == 0] = 1  # Set "zero" error to small number.
             p, V = np.polyfit(x_data, y_data, 1, cov=True, w=1 / y_err)
             m, b, err_m, err_b = (*p, np.sqrt(V[0][0]), np.sqrt(V[1][1]))
 
             # Convert linear fit of ppm vs counts
             # to linear fit of counts vs ppm (flip axes)
             m = 1 / m
             err_m = err_m
@@ -389,14 +391,19 @@
                                 horizontalalignment='right',
                                 transform=ax_calibration.transAxes, fontsize=8)
         except (np.linalg.LinAlgError):
             label = chemical + '\nBad Fit'
             ax_calibration.text(.02, .75, label,
                                 horizontalalignment='left',
                                 transform=ax_calibration.transAxes, fontsize=8)
+            # If fit fails, set all values to zero
+            m = 0
+            b = 0
+            err_m = 0
+            err_b = 0
         new_calibration.loc[chemical, 'slope':'err_intercept'] = [m, err_m,
                                                                   b, err_b]
 
     ax_run_num = fig_run_num.add_subplot(111, frameon=False)
     # hide tick and tick label of the big axis
     ax_run_num.tick_params(labelcolor='none', which='both',
                            top=False, bottom=False, left=False, right=False)
@@ -555,15 +562,15 @@
     if units == 'frac':  # Change label style to stacked compositions.
         condition = condition.str.replace('_', '\n')
         condition = condition.str.replace('frac', '')
 
     elif expt.expt_type == 'stability_test':
         pass  # Already Float
 
-    else:  # Convert filenames to float w/o units.
+    else:  # Convert folder name to float w/o units.
         condition = condition.str.replace(r'\D', '', regex=True).astype(float)
 
     # Results
     ###########################################################################
     avg = pd.DataFrame(avg_dat, columns=calchemIDs, index=condition)
     # TODO add err_concentration values to std
     std = pd.DataFrame(std_dat, columns=calchemIDs, index=condition)
```

### Comparing `catalight-0.1.4/catalight/analysis/user_inputs.py` & `catalight-0.1.6/catalight/analysis/user_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,21 +5,20 @@
 calibration files, data paths, and enter function parameters.
 Created on Thu Jun 23 22:42:55 2022
 @author: Briley Bourgeois
 
 References
 ----------
 # noqa
-(1) https://github.com/napari/magicgui/issues/9
-(2) https://stackoverflow.com/questions/28544425/pyqt-qfiledialog-multiple-directory-selection
-(3) https://stackoverflow.com/questions/38746002/pyqt-qfiledialog-directly-browse-to-a-folder
-(4) https://stackoverflow.com/questions/4286036/how-to-have-a-directory-dialog
-(5) https://stackoverflow.com/questions/38609516/hide-empty-parent-folders-qtreeview-qfilesystemmodel
-(6) https://www.youtube.com/watch?v=dqg0L7Qw3ko
-(7) https://stackoverflow.com/questions/52592977/how-to-return-variables-from-pyqt5-ui-to-main-function-python
+(1) https://stackoverflow.com/questions/28544425/pyqt-qfiledialog-multiple-directory-selection
+(2) https://stackoverflow.com/questions/38746002/pyqt-qfiledialog-directly-browse-to-a-folder
+(3) https://stackoverflow.com/questions/4286036/how-to-have-a-directory-dialog
+(4) https://stackoverflow.com/questions/38609516/hide-empty-parent-folders-qtreeview-qfilesystemmodel
+(5) https://www.youtube.com/watch?v=dqg0L7Qw3ko
+(6) https://stackoverflow.com/questions/52592977/how-to-return-variables-from-pyqt5-ui-to-main-function-python
 """
 from __future__ import annotations
 import os
 import sys
 from ast import literal_eval
 from dataclasses import dataclass, fields, is_dataclass
```

### Comparing `catalight-0.1.4/catalight/catalight_GUI.py` & `catalight-0.1.6/catalight/catalight_GUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 import time
 
 import matplotlib
 import numpy as np
 import pandas as pd
 import psutil
 from alicat import FlowController
-from catalight.equipment.alicat_MFC.gas_control import Gas_System
-from catalight.equipment.diode_laser.diode_control import Diode_Laser
-from catalight.equipment.harrick_watlow.heater_control import Heater
-from catalight.equipment.sri_gc.gc_control import GC_Connector
+from catalight.equipment.gas_control.alicat import Gas_System
+from catalight.equipment.light_sources.diode_control import Diode_Laser
+from catalight.equipment.heating.watlow import Heater
+from catalight.equipment.gc_control.sri_gc import GC_Connector
 from catalight.equipment.experiment_control import Experiment
 
 import matplotlib.pyplot as plt
 from matplotlib.backends.backend_qt5agg import \
     NavigationToolbar2QT as NavigationToolbar
 from PyQt5.QtCore import (QObject, QRunnable, Qt, QThreadPool, QTimer,
                           pyqtSignal, pyqtSlot)
@@ -163,15 +163,15 @@
         calDF = pd.read_csv(filePath, delimiter=',', index_col='Chem ID')
         if self.gas_Status.isChecked():
             attribute_list = vars(self.gas_controller)
             for key in attribute_list:
                 attr = attribute_list[key]
                 if isinstance(attr, FlowController):
                     self.gas_controller.set_calibration_gas(attr, calDF,
-                                                             fill_gas='Ar')
+                                                            fill_gas='Ar')
 
             self.setGasAType.insertItem(0, 'CalGas')
             self.setGasBType.insertItem(0, 'CalGas')
             self.setGasCType.insertItem(0, 'CalGas')
             self.setGasDType.insertItem(0, 'CalGas')
             self.manualGasAType.insertItem(0, 'CalGas')
             self.manualGasBType.insertItem(0, 'CalGas')
@@ -618,15 +618,15 @@
                 # This block determines if sensible values are in ind_var
                 start = widget_grid[ind_var_row][3].value()
                 stop = widget_grid[ind_var_row][4].value() + 1
                 step = widget_grid[ind_var_row][5].value()
                 if (stop > start) and (step > 0):
                     ind_var = np.arange(start, stop, step)
                 else:
-                    return(False)
+                    return False
 
                 ind_var = ind_var / 100  # convert from % to frac
                 comp_list[ind_var_row - 1] = ind_var.tolist()
 
                 # fill_vals = np.ones(len(ind_var)) # Fill values = 1 (100%)
                 fill_vals = 1 - ind_var
 
@@ -969,14 +969,15 @@
         # self.threadpool.clear()
         # self.threadpool.cancel()
         self.threadpool.cancel(self.run_study_thread)
         self.threadpool.cancel(self.manual_ctrl_thread)
         # self.threadpool.disconnect()
         self.shut_down()
 
+
 class EmittingStream():
     """
     Capture console print statements and broadcast within the GUI.
 
     Redefine sys.stdout, which typically handles all print statements.
     We rewrite the write method to also write to a given Qtextedit.
 
@@ -999,18 +1000,20 @@
         self.textbox.setTextCursor(cursor)
         self.textbox.ensureCursorVisible()
 
     def flush(self):
         """Force print to terminal without buffering"""
         self.terminal.flush()
 
+
 class WorkerSignal(QObject):
     """Provide signals for interacting w/ worker threads."""
     finished = pyqtSignal()
 
+
 class Worker(QRunnable):
     """
     Worker thread.
 
     Inherits from QRunnable to handle
     worker thread setup, signals and wrap-up.
```

### Comparing `catalight-0.1.4/catalight/equipment/alicat_MFC/connection_tester.py` & `catalight-0.1.6/catalight/equipment/alicat_connection_tester.py`

 * *Files identical despite different names*

### Comparing `catalight-0.1.4/catalight/equipment/alicat_MFC/gas_control.py` & `catalight-0.1.6/catalight/equipment/gas_control/alicat.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,19 +133,19 @@
             else:
                 gas_list.append(gas_name)
         # convert to percents, make dict, drop zero values
         percents = np.array(comp_list, dtype=float) * 100
         gas_series = pd.Series(percents, gas_list)
         gas_series = gas_series.groupby(level=0).sum()  # sums duplicates
         gas_dict = gas_series.to_dict()
-        gas_dict = {x:y for x,y in gas_dict.items() if y != 0}
+        gas_dict = {x: y for x, y in gas_dict.items() if y != 0}
 
         # Uses create_mix method to write to gas slot 236,
         # first custom gas slot on MFC
-        if len(gas_dict)>1: # if more than 1 gas, creates mix
+        if len(gas_dict) > 1:  # if more than 1 gas, creates mix
             self.mfc_E.create_mix(mix_no=236, name='output',
                                   gases=gas_dict)
             self.mfc_E.set_gas(236)
         else:  # If only one gas, sets that as output
             self.mfc_E.set_gas(list(gas_dict)[0])
         self.is_busy = False
```

### Comparing `catalight-0.1.4/catalight/equipment/diode_laser/diode_control.py` & `catalight-0.1.6/catalight/equipment/light_sources/diode_control.py`

 * *Files identical despite different names*

### Comparing `catalight-0.1.4/catalight/equipment/experiment_control.py` & `catalight-0.1.6/catalight/equipment/experiment_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,18 +30,18 @@
 
     Parameters
     ----------
     eqpt_list: list of objects, optional
         List of equipment objects. Calls :py:meth:`update_eqpt_list`,
         if provided.
         Order of list should be:
-        (:py:class:`~catalight.equipment.sri_gc.gc_control.GC_Connector`,
-        :class:`~catalight.equipment.diode_laser.diode_control.Diode_Laser`,
-        :class:`~catalight.equipment.alicat_MFC.gas_control.Gas_System`,
-        :class:`~catalight.equipment.harrick_watlow.heater_control.Heater`)
+        (:py:class:`~catalight.equipment.gc_control.sri_gc.GC_Connector`,
+        :class:`~catalight.equipment.light_sources.diode_control.Diode_Laser`,
+        :class:`~catalight.equipment.gas_control.alicat.Gas_System`,
+        :class:`~catalight.equipment.heating.watlow.Heater`)
     """
 
     def __init__(self, eqpt_list=False):
         """Init experiment object."""
         # This class attribute defines the possible experiments. This is an
         # important part of the class and should be altered with caution
         # noqa to suppress extra spaces PEP violation. Done for clarity.
@@ -50,15 +50,15 @@
         # careful bug checking needs to be performed everywhere expt.ind_var
         # is used.
         self._expt_list = pd.DataFrame(
             [['temp_sweep',      'temp', False,    'K'],  # noqa
              ['power_sweep',    'power', False,   'mW'],  # noqa
              ['comp_sweep',  'gas_comp', False, 'frac'],  # noqa
              ['flow_sweep',  'tot_flow', False, 'sccm'],  # noqa
-             ['calibration', 'gas_comp', False,  'ppm'],  # noqa
+             ['calibration', 'gas_comp', False, 'frac'],  # noqa
              ['stability_test',  'temp', False,  'min']], # noqa
             columns=['Expt Name',
                      'Independent Variable',
                      'Active Status',
                      'Units'])
 
         # Set default values of properties
@@ -434,15 +434,15 @@
                     self._expt_name = data
                 elif re.search('Sample Name =', line):
                     self.sample_name = data
                 elif re.search('Temperature', line):
                     self.temp = literal_eval(data)
                 elif re.search('Power', line):
                     self.power = literal_eval(data)
-                elif re.search('Gas \d+ type', line):  # \d+ is 1 or more digit
+                elif re.search(r'Gas \d+ type', line):  # \d+ is 1+ digits
                     # Get left side of '=' sign
                     gas_str = line.split('=')[0].strip(' \n')
                     # Pull number from left side
                     for string in gas_str.split():
                         if string.isdigit():
                             num = int(string)
                     # If the gas_type list is shorter than this entry number,
@@ -715,18 +715,18 @@
         and assigns each component to experiment object
         updates sample rate by given value in gc_control and updates heater
         ramp rate by the rate specified in experiment object
 
         Parameters
         ----------
         eqpt_list: list[object]
-            (:py:class:`~catalight.equipment.sri_gc.gc_control.GC_Connector`,
-            :class:`~catalight.equipment.diode_laser.diode_control.Diode_Laser`,
-            :class:`~catalight.equipment.alicat_MFC.gas_control.Gas_System`,
-            :class:`~catalight.equipment.harrick_watlow.heater_control.Heater`)
+            (:py:class:`~catalight.equipment.gc_control.sri_gc.GC_Connector`,
+            :class:`~catalight.equipment.light_sources.diode_control.Diode_Laser`,
+            :class:`~catalight.equipment.gas_control.alicat.Gas_System`,
+            :class:`~catalight.equipment.heating.watlow.Heater`)
         """
         # eqpt_list needs to be tuple
         self._gc_control = eqpt_list[0]
         self._laser_control = eqpt_list[1]
         self._gas_control = eqpt_list[2]
         self._heater = eqpt_list[3]
 
@@ -844,24 +844,25 @@
             # This segment times when to start GC and prints status
             # -----------------------------------------------------
             print('Waiting for steady state: '
                   + time.strftime("%H:%M:%S", time.localtime()))
             t1 = time.time()
             while self._gc_control.is_running():
                 time.sleep(10)  # Don't update ctrl file while running
-            self._gc_control.update_ctrl_file(path)
+            self._gc_control.update_gc_settings(path)
             t2 = time.time()
             t_passed = round(t2 - t1)  # GC can take a while to respond
             for i in range(int(self.t_steady_state * 60 - t_passed)):
-                time.sleep(1)  # Break sleep in bits so keyboard interrupt works
+                time.sleep(1)
+                # Break sleep in bits so keyboard interrupt works
 
             print('Starting Collection: '
                   + time.strftime("%H:%M:%S", time.localtime()))
             print('Starting Temp = ', self._heater.read_temp(), ' C')
-            self._gc_control.peaksimple.SetRunning(1, True)
+            self._gc_control.set_running()
             # t_collect ends on last gc pull
             t_collect = self.sample_rate * (self.sample_set_size - 1) * 60
 
             for i in range(int(t_collect)):
                 time.sleep(1)
 
             print('Finished Collecting: '
```

### Comparing `catalight-0.1.4/catalight/equipment/gc_delay_tester.py` & `catalight-0.1.6/catalight/equipment/gc_delay_tester.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 @author: Briley Bourgeois
 """
 import os
 import time
 from datetime import date
 
-from catalight.equipment.alicat_MFC.gas_control import Gas_System
-from catalight.equipment.sri_gc.gc_control import GC_Connector
+from catalight.equipment.gas_control.alicat import Gas_System
+from catalight.equipment.gc_control.sri_gc import GC_Connector
 
 
 def main(main_dir, delay_times, flows, gas_list, comp_list_on, comp_list_off,
          ctrl_file=None, flush_flowrate=50):
     """
     Test the response time of the GC by collecting samples in controlled way.
 
@@ -72,22 +72,22 @@
 
     for tot_flow in flows:
         flow_dir = os.path.join(expt_dir, (str(tot_flow) + '_sccm'))
         for delay in delay_times:
             filename = (str(delay) + '_min_delay')
             filepath = os.path.join(flow_dir, filename)
             os.makedirs(filepath, exist_ok=True)
-            gc.update_ctrl_file(filepath)  # Changes save path
+            gc.update_gc_settings(filepath)  # Changes save path
             gas_control.set_flows(comp_list_on, tot_flow)  # Flow Target Gas
 
             for second in range(int(delay * 60)):
                 time.sleep(1)  # 1 second at a time so script can be stopped
 
             # Turn on gc and pause a minute to be safe
-            gc.peaksimple.SetRunning(1, True)
+            gc.set_running()
             time.sleep(60)
             # Clear out gas line
             gas_control.set_flows(comp_list_off, flush_flowrate)
 
             # Wait until gc collection is done
             for second in range(int((gc.sample_rate - 1) * 60)):
                 time.sleep(1)  # 1 second at a time so script can be stopped
```

### Comparing `catalight-0.1.4/catalight/equipment/harrick_watlow/heater_control.py` & `catalight-0.1.6/catalight/equipment/heating/watlow.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,24 +227,24 @@
             (deg C) Starting setpoint to use for testing. The default is 30.
 
         Returns
         -------
         None.
 
         """
-        heater.ramp(20)  # Start from 'off'
+        self.ramp(20)  # Start from 'off'
         time.sleep(300)  # Allow steady state for 5 min
         for rate in rates:
             # Set new rate, ramp, turn off
-            heater.ramp_rate = rate
-            read_out, fig, ax = heater.ramp(T_max, T_min, record=True)
-            heater.shut_down()
+            self.ramp_rate = rate
+            read_out, fig, ax = self.ramp(T_max, T_min, record=True)
+            self.shut_down()
 
             # Allow temperature to return to < 30 C
-            while heater.read_temp() > 30:
+            while self.read_temp() > 30:
                 time.sleep(60)
 
             # Save results
             read_out.to_csv(os.path.join(savepath,
                                          str(rate) + '_heater_read_out.csv'))
             fig.savefig(os.path.join(savepath, str(rate) + '_heater_test.svg'),
                         format="svg")
```

### Comparing `catalight-0.1.4/catalight/equipment/power_meter/power_meter_ctrl.py` & `catalight-0.1.6/catalight/equipment/power_meter/newport.py`

 * *Files identical despite different names*

### Comparing `catalight-0.1.4/catalight/equipment/run_diode_calibration.py` & `catalight-0.1.6/catalight/equipment/run_diode_calibration.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 diode laser being used. Works for Newport power meter and Thorlabs diode driver
 powered by MCC DAQ.
 Created on Tue Feb 22 23:15:23 2022
 @author: Briley Bourgeois
 """
 import numpy as np
 import pandas as pd
-from catalight.equipment.diode_laser.diode_control import Diode_Laser
-from catalight.equipment.power_meter.power_meter_ctrl import NewportMeter
+from catalight.equipment.light_sources.diode_control import Diode_Laser
+from catalight.equipment.power_meter.newport import NewportMeter
 
 
 def main(current_range=(150, 800, 35), wavelength=450, tolerance=10):
     """
     Runs a calibration on the connected Diode_Laser.
 
     The current is varied based on the supplied current_range and the power
```

### Comparing `catalight-0.1.4/catalight/equipment/sri_gc/gc_control.py` & `catalight-0.1.6/catalight/equipment/gc_control/sri_gc.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 clr.AddReference(assemblydir)  # Add the assembly to python.NET
 # Now that the Assembly has been added to python.NET,
 # it can be imported like a normal module, though the name is different.
 import Peaksimple  # Need add assembly before import. # noqa # type: ignore
 
 # TODO some control file needs to be placed within package to work w/ any user.
 # the default won't run from the repo for some reason
-default_ctrl_file = ("C:\\Peak489Win10\\CONTROL_FILE\\"
-                     "HayN_C2H2_Hydrogenation\\C2H2_Hydro_HayN_TCD_off.CON")
+default_ctrl_file = os.path.join(dir_path, 'DEFAULT.CON')
 
 
 class GC_Connector():
     """
     Interface with SRI GC through Peaksimple interface via .dll file.
 
     If the assembly can't be found, find the .dll file, right click,
@@ -49,35 +48,36 @@
         :ref:`sri_gc_doc` for more info on methods."""
 
         self.ctrl_file = ctrl_file
         """str: Full path to control file to use."""
 
         self.sample_set_size = 4
         """
-        int:  Number of GC collection for each time peaksimple.setRunning()
+        int:  Number of GC collection for each time set_running()
         is called. Can be changed per experiment by editing
         :attr:`Experiment.sample_set_size
         <catalight.equipment.experiment_control.Experiment.sample_set_size>`
         """
 
         # Init Procedure:
         # ---------------
         self.connect()
         self._sample_rate = 0  # Dummy value, reset when ctrl file loaded
+        self._min_sample_rate = 0  # Dummy value, reset when ctrl file loaded
         # Sends ctrl file to GC, updates self w/ new data
         print('Loading', ctrl_file)
         self.load_ctrl_file()
 
     # Properties
     # ----------
     # Makes min_sample_rate read only
     min_sample_rate = property(lambda self: self._min_sample_rate)
     """float, read-only: (min) Minimum setpoint for sample_rate.
     Sum of Channel 1 Time and Channel 1 Posttime from GC control file.
-    Value automatically updates when :meth:`read_ctrl_file` is called."""
+    Value automatically updates when :meth:`read_gc_settings` is called."""
 
     # Setting sample rate changes when connected to GC
     @property
     def sample_rate(self):
         """
         Time between setting collections in minutes.
 
@@ -94,23 +94,23 @@
         else:
             print('Minimum Sample Rate = %5.2f' % self.min_sample_rate)
             print('Sample rate set to minimum')
             self._sample_rate = self.min_sample_rate
 
     # Methods:
     # --------
-    def update_ctrl_file(self, data_file_path):
+    def update_gc_settings(self, data_file_path):
         """
         Write over the currently loaded ctrl file to update settings.
 
-        Goes line by line through the control file defined by ctrl_file attr
-        and rewrites the line to set appropriate options. Ensures postrun cycle
-        & repeat, autoincrement, and save image, data, & results are all
-        turned on. Updates data file path to that provided. Sets postrun repeat
-        to sample_set_size.
+        Updates data file path to that provided. Sets postrun repeat
+        to sample_set_size. Goes line by line through the control file defined
+        by ctrl_file attr and rewrites the line to set appropriate options.
+        Ensures postrun cycle & repeat, autoincrement, and save image, data,
+        & results are all turned on.
 
         Parameters
         ----------
         data_file_path : str
             Full path to the directory in which you'd like to save data files.
         """
         with open(self.ctrl_file, 'r+') as ctrl_file:
@@ -182,17 +182,17 @@
                 print('Write error. Retrying...')
                 time.sleep(1)
                 continue
             except Peaksimple.NoConnectionException:
                 print('Write Error: GC Not Connected')
                 break
         time.sleep(5)  # I think peaksimple is cranky when rushed
-        self.read_ctrl_file()
+        self.read_gc_settings()
 
-    def read_ctrl_file(self):
+    def read_gc_settings(self):
         """
         Read loaded control file and updates object with values from file.
 
         Currently updates min_sample_rate property by pulling run time postrun
         cycle time from control file. Updates sample_rate if it is faster than
         the new min_sample_rate
 
@@ -211,14 +211,24 @@
                     post_time = int(line.split('=')[-1].strip(' \n'))
 
             self._min_sample_rate = (run_time + post_time) / 1000
 
             if self.sample_rate < self.min_sample_rate:
                 self.sample_rate = self.min_sample_rate
 
+    def set_running(self):
+        """
+        Start data collection. Make sure correct GC settings are loaded first.
+
+        Wraps over peaksimple set running function. Will set channel 1 running
+        by default. This could be made flexible in the future if ever needed.
+        I think most SRI GC interactions are controlled by channel 1 though.
+        """
+        self.peaksimple.SetRunning(1, True)
+
     def is_running(self, max_tries=3):
         """
         Request status of GC collection (running or not).
 
         Parameters
         ----------
         max_tries : int, optional
@@ -312,15 +322,16 @@
 
 
 if __name__ == "__main__":
     print(dir_path)
     gc1 = GC_Connector()
     data_path = 'C:\\Peak489Win10\\GCDATA\\20221117_CodeTest'
     gc1.sample_set_size = 2
-    gc1.update_ctrl_file(data_path)
-    gc1.peaksimple.SetRunning(1, True)
-    time.sleep(10)
-    for n in range(0, 31):
-        print(time.ctime(), '---', gc1.peaksimple.IsRunning(1))
-        # IsRunning returns false inbetween runs. Returns True during run
-        time.sleep(60)
-    print('Finished')
+    gc1.update_gc_settings(data_path)
+    gc1.peaksimple.IsConnected()
+    # gc1.set_running()
+    # time.sleep(10)
+    # for n in range(0, 31):
+    #     print(time.ctime(), '---', gc1.peaksimple.IsRunning(1))
+    #     # IsRunning returns false inbetween runs. Returns True during run
+    #     time.sleep(60)
+    # print('Finished')
```

### Comparing `catalight-0.1.4/catalight/equipment/sri_gc/peaksimple_control_demo.py` & `catalight-0.1.6/catalight/equipment/gc_control/peaksimple_control_demo.py`

 * *Files identical despite different names*

### Comparing `catalight-0.1.4/catalight.egg-info/PKG-INFO` & `catalight-0.1.6/catalight.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catalight
-Version: 0.1.4
+Version: 0.1.6
 Summary: Photoreactor system automation, data handling, and analysis.
 Author-email: Briley Bourgeois <bbourge6@stanford.edu>, Claire Carlin <cccarlin@stanford.edu>
 Project-URL: Homepage, https://github.com/Dionne-Lab/catalight
 Project-URL: Bug Tracker, https://github.com/Dionne-Lab/catalight/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 Welcome to Catalight!
 =======================
 .. figure:: https://raw.githubusercontent.com/Dionne-Lab/catalight/main/docs/source/_static/images/catalight_header_g.png
     :width: 800
 
 Introduction
 ------------
-Catalight is tool set developed by scientists at Stanford to help automate photocatalysis experiments. catalight is capable of connecting to hardware, coordinating instruments to run a variety of different experimental procedures, and organizing and analyzing data collected by the system. The project is designed in a modular format to enable users to bring their own unique hardware while still utilizing the core features of experiment management and data handling. The program functions in both a scripted version and a GUI to aid users in planning experimental procedures and manually controlling hardware.
+Catalight is a tool set developed by scientists at Stanford to help automate photocatalysis experiments. Catalight is capable of connecting to hardware, coordinating instruments to run a variety of different experimental procedures, and organizing and analyzing data collected by the system. The project is designed in a modular format to enable users to bring their own unique hardware while still utilizing the core features of experiment management and data handling. The program functions in both a scripted version and a GUI to aid users in planning experimental procedures and manually controlling hardware.
 
 To date, catalight is compatible with Alicat mass flow controllers, heater systems controlled by Watlow components, Measurement Computing data acquisition boards (used for communication with (ThorLabs laser diode drivers), NewPort 843-R power meter, and SRI gas chromatographs. Support for additional hardware is planned for the future, including FTIR data collection and analysis and NKT Photonics lasers. We strongly encourage interested users to consider contributing to the project by adding new device support and helping expand the catalight functionality.
 
 **ReadtheDocs Page:**
 https://catalight.readthedocs.io/en/latest/
 
 **PyPI Page:**
```

### Comparing `catalight-0.1.4/catalight.egg-info/SOURCES.txt` & `catalight-0.1.6/catalight.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -19,24 +19,26 @@
 catalight/analysis/run_change_xdata.py
 catalight/analysis/run_initial_analysis.py
 catalight/analysis/run_plot_chromatograms_stacked.py
 catalight/analysis/run_plot_comparison.py
 catalight/analysis/tools.py
 catalight/analysis/user_inputs.py
 catalight/equipment/__init__.py
+catalight/equipment/alicat_connection_tester.py
 catalight/equipment/experiment_control.py
 catalight/equipment/gc_delay_tester.py
 catalight/equipment/run_diode_calibration.py
-catalight/equipment/alicat_MFC/__init__.py
-catalight/equipment/alicat_MFC/connection_tester.py
-catalight/equipment/alicat_MFC/gas_control.py
-catalight/equipment/diode_laser/__init__.py
-catalight/equipment/diode_laser/diode_control.py
-catalight/equipment/harrick_watlow/__init__.py
-catalight/equipment/harrick_watlow/heater_control.py
-catalight/equipment/nkt_laser/__init__.py
+catalight/equipment/gas_control/__init__.py
+catalight/equipment/gas_control/alicat.py
+catalight/equipment/gas_control/template.py
+catalight/equipment/gc_control/__init__.py
+catalight/equipment/gc_control/peaksimple_control_demo.py
+catalight/equipment/gc_control/sri_gc.py
+catalight/equipment/gc_control/template.py
+catalight/equipment/heating/__init__.py
+catalight/equipment/heating/template.py
+catalight/equipment/heating/watlow.py
+catalight/equipment/light_sources/__init__.py
+catalight/equipment/light_sources/diode_control.py
+catalight/equipment/light_sources/template.py
 catalight/equipment/power_meter/__init__.py
-catalight/equipment/power_meter/demo.py
-catalight/equipment/power_meter/power_meter_ctrl.py
-catalight/equipment/sri_gc/__init__.py
-catalight/equipment/sri_gc/gc_control.py
-catalight/equipment/sri_gc/peaksimple_control_demo.py
+catalight/equipment/power_meter/newport.py
```

### Comparing `catalight-0.1.4/pyproject.toml` & `catalight-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "catalight"
-version = "0.1.4"
+version = "0.1.6"
 authors = [
   { name="Briley Bourgeois", email="bbourge6@stanford.edu" },
   { name="Claire Carlin", email="cccarlin@stanford.edu" }
 ]
 description = "Photoreactor system automation, data handling, and analysis."
 readme = "README.rst"
 requires-python = ">=3.7"
```

### Comparing `catalight-0.1.4/setup.py` & `catalight-0.1.6/setup.py`

 * *Files identical despite different names*

