# Comparing `tmp/JupyterPiDAQ-0.7.9.tar.gz` & `tmp/JupyterPiDAQ-0.8.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JupyterPiDAQ-0.7.9.tar", last modified: Thu Mar  9 20:50:11 2023, max compression
+gzip compressed data, was "JupyterPiDAQ-0.8.0.dev0.tar", last modified: Wed Apr 19 22:07:45 2023, max compression
```

## Comparing `JupyterPiDAQ-0.7.9.tar` & `JupyterPiDAQ-0.8.0.dev0.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-03-09 20:50:11.326069 JupyterPiDAQ-0.7.9/
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-03-09 20:50:11.322383 JupyterPiDAQ-0.7.9/JupyterPiDAQ.egg-info/
--rw-r--r--   0 gutow    (60685682) staff       (20)     4153 2023-03-09 20:50:11.000000 JupyterPiDAQ-0.7.9/JupyterPiDAQ.egg-info/PKG-INFO
--rw-r--r--   0 gutow    (60685682) staff       (20)      776 2023-03-09 20:50:11.000000 JupyterPiDAQ-0.7.9/JupyterPiDAQ.egg-info/SOURCES.txt
--rw-r--r--   0 gutow    (60685682) staff       (20)        1 2023-03-09 20:50:11.000000 JupyterPiDAQ-0.7.9/JupyterPiDAQ.egg-info/dependency_links.txt
--rw-r--r--   0 gutow    (60685682) staff       (20)      337 2023-03-09 20:50:11.000000 JupyterPiDAQ-0.7.9/JupyterPiDAQ.egg-info/requires.txt
--rw-r--r--   0 gutow    (60685682) staff       (20)       19 2023-03-09 20:50:11.000000 JupyterPiDAQ-0.7.9/JupyterPiDAQ.egg-info/top_level.txt
--rw-r--r--   0 gutow    (60685682) staff       (20)     4153 2023-03-09 20:50:11.325926 JupyterPiDAQ-0.7.9/PKG-INFO
--rw-r--r--   0 gutow    (60685682) staff       (20)     3451 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.7.9/README.md
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-03-09 20:50:11.322643 JupyterPiDAQ-0.7.9/Tests/
--rw-r--r--   0 gutow    (60685682) staff       (20)        0 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.7.9/Tests/__init__.py
--rw-r--r--   0 gutow    (60685682) staff       (20)     4894 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.7.9/Tests/test_boards.py
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-03-09 20:50:11.323708 JupyterPiDAQ-0.7.9/jupyterpidaq/
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-03-09 20:50:11.324004 JupyterPiDAQ-0.7.9/jupyterpidaq/Boards/
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-03-09 20:50:11.324574 JupyterPiDAQ-0.7.9/jupyterpidaq/Boards/PiGPIO/
--rw-r--r--   0 gutow    (60685682) staff       (20)     8820 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.7.9/jupyterpidaq/Boards/PiGPIO/ADS1115.py
--rw-r--r--   0 gutow    (60685682) staff       (20)     8053 2023-03-09 20:46:10.000000 JupyterPiDAQ-0.7.9/jupyterpidaq/Boards/PiGPIO/DAQC2.py
--rw-r--r--   0 gutow    (60685682) staff       (20)       69 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.7.9/jupyterpidaq/Boards/PiGPIO/__init__.py
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-03-09 20:50:11.325169 JupyterPiDAQ-0.7.9/jupyterpidaq/Boards/Simulated/
--rw-r--r--   0 gutow    (60685682) staff       (20)     7977 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.7.9/jupyterpidaq/Boards/Simulated/ADCsim.py
--rw-r--r--   0 gutow    (60685682) staff       (20)     9380 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.7.9/jupyterpidaq/Boards/Simulated/ADCsim_line.py
--rw-r--r--   0 gutow    (60685682) staff       (20)       55 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.7.9/jupyterpidaq/Boards/Simulated/__init__.py
--rw-r--r--   0 gutow    (60685682) staff       (20)      131 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.7.9/jupyterpidaq/Boards/__init__.py
--rw-r--r--   0 gutow    (60685682) staff       (20)     7559 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.7.9/jupyterpidaq/Boards/boards.py
--rw-r--r--   0 gutow    (60685682) staff       (20)     9279 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.7.9/jupyterpidaq/ChannelSettings.py
--rw-r--r--   0 gutow    (60685682) staff       (20)     4140 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.7.9/jupyterpidaq/DAQProc.py
--rw-r--r--   0 gutow    (60685682) staff       (20)    33293 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.7.9/jupyterpidaq/DAQinstance.py
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-03-09 20:50:11.325472 JupyterPiDAQ-0.7.9/jupyterpidaq/Sensors/
--rw-r--r--   0 gutow    (60685682) staff       (20)       91 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.7.9/jupyterpidaq/Sensors/__init__.py
--rw-r--r--   0 gutow    (60685682) staff       (20)    27233 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.7.9/jupyterpidaq/Sensors/sensors.py
--rw-r--r--   0 gutow    (60685682) staff       (20)      243 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.7.9/jupyterpidaq/__init__.py
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-03-09 20:50:11.325698 JupyterPiDAQ-0.7.9/jupyterpidaq/javascript/
--rw-r--r--   0 gutow    (60685682) staff       (20)     4770 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.7.9/jupyterpidaq/javascript/JupyterPiDAQmnu.js
--rw-r--r--   0 gutow    (60685682) staff       (20)       38 2023-03-09 20:50:11.326105 JupyterPiDAQ-0.7.9/setup.cfg
--rw-r--r--   0 gutow    (60685682) staff       (20)     1768 2023-03-09 20:30:44.000000 JupyterPiDAQ-0.7.9/setup.py
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-19 22:07:45.440769 JupyterPiDAQ-0.8.0.dev0/
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-19 22:07:45.435094 JupyterPiDAQ-0.8.0.dev0/JupyterPiDAQ.egg-info/
+-rw-r--r--   0 gutow    (60685682) staff       (20)     4679 2023-04-19 22:07:45.000000 JupyterPiDAQ-0.8.0.dev0/JupyterPiDAQ.egg-info/PKG-INFO
+-rw-r--r--   0 gutow    (60685682) staff       (20)      856 2023-04-19 22:07:45.000000 JupyterPiDAQ-0.8.0.dev0/JupyterPiDAQ.egg-info/SOURCES.txt
+-rw-r--r--   0 gutow    (60685682) staff       (20)        1 2023-04-19 22:07:45.000000 JupyterPiDAQ-0.8.0.dev0/JupyterPiDAQ.egg-info/dependency_links.txt
+-rw-r--r--   0 gutow    (60685682) staff       (20)      371 2023-04-19 22:07:45.000000 JupyterPiDAQ-0.8.0.dev0/JupyterPiDAQ.egg-info/requires.txt
+-rw-r--r--   0 gutow    (60685682) staff       (20)       19 2023-04-19 22:07:45.000000 JupyterPiDAQ-0.8.0.dev0/JupyterPiDAQ.egg-info/top_level.txt
+-rw-r--r--   0 gutow    (60685682) staff       (20)     4679 2023-04-19 22:07:45.440631 JupyterPiDAQ-0.8.0.dev0/PKG-INFO
+-rw-r--r--   0 gutow    (60685682) staff       (20)     3972 2023-04-19 19:23:05.000000 JupyterPiDAQ-0.8.0.dev0/README.md
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-19 22:07:45.435363 JupyterPiDAQ-0.8.0.dev0/Tests/
+-rw-r--r--   0 gutow    (60685682) staff       (20)        0 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0.dev0/Tests/__init__.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)     4894 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0.dev0/Tests/test_boards.py
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-19 22:07:45.437545 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-19 22:07:45.438108 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-19 22:07:45.438762 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/PiGPIO/
+-rw-r--r--   0 gutow    (60685682) staff       (20)     8820 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/PiGPIO/ADS1115.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)     8053 2023-03-09 20:46:10.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/PiGPIO/DAQC2.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)       69 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/PiGPIO/__init__.py
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-19 22:07:45.439214 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/Simulated/
+-rw-r--r--   0 gutow    (60685682) staff       (20)     7977 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/Simulated/ADCsim.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)     9380 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/Simulated/ADCsim_line.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)       55 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/Simulated/__init__.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)      131 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/__init__.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)     7617 2023-04-08 16:27:02.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/boards.py
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-19 22:07:45.439644 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/vernier/
+-rw-r--r--   0 gutow    (60685682) staff       (20)       62 2023-04-08 16:27:02.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/vernier/__init__.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)    11240 2023-04-14 15:10:40.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/vernier/labquest.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)     9279 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/ChannelSettings.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)     4794 2023-04-14 15:10:40.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/DAQProc.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)    34634 2023-04-18 17:52:45.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/DAQinstance.py
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-19 22:07:45.440114 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Sensors/
+-rw-r--r--   0 gutow    (60685682) staff       (20)       91 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Sensors/__init__.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)    27233 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Sensors/sensors.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)      243 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/__init__.py
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-19 22:07:45.440301 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/javascript/
+-rw-r--r--   0 gutow    (60685682) staff       (20)     4901 2023-04-03 16:01:44.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/javascript/JupyterPiDAQmnu.js
+-rw-r--r--   0 gutow    (60685682) staff       (20)       38 2023-04-19 22:07:45.440826 JupyterPiDAQ-0.8.0.dev0/setup.cfg
+-rw-r--r--   0 gutow    (60685682) staff       (20)     1827 2023-04-18 21:52:39.000000 JupyterPiDAQ-0.8.0.dev0/setup.py
```

### Comparing `JupyterPiDAQ-0.7.9/JupyterPiDAQ.egg-info/PKG-INFO` & `JupyterPiDAQ-0.8.0.dev0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,29 @@
-Metadata-Version: 2.1
-Name: JupyterPiDAQ
-Version: 0.7.9
-Summary: Data Acquisition in Jupyter notebook on Raspberry Pi
-Home-page: https://github.com/JupyterPhysSciLab/JupyterPiDAQ
-Author: Jonathan Gutow
-Author-email: gutow@uwosh.edu
-License: GPL-3.0+
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: JavaScript
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-
 ## JupyterPiDAQ
 [Introduction](#introduction) | [License](#license)
 
 ### [Website/Documentation](https://jupyterphysscilab.github.io/JupyterPiDAQ/)
 
 ### Introduction:
 This software allows realtime collection and plotting of 
-digitized data in  a Jupyter notebook. The package was initially developed
+digitized data inside  a Jupyter notebook. The package was initially developed
 to provide an inexpensive laboratory system for teaching based on
-the Raspberry Pi.  However, as the development has progressed the data
-acquisition board drivers have been separated out of the user interface,
-so that the software has potential to work on other computers running Jupyter
-with A-to-D board specific connector code. Presently the compatible A-to-Ds are
-for Raspberry Pis: 
+the Raspberry Pi.  __However, it now also works on other hardware__. 
+Presently the working combinations are:
+
+__on Raspberry Pis__ 
 * Adafruit compliant ADS1115 boards 
 ([example](https://www.amazon.com/KNACRO-4-Channel-Raspberry-ADS1115-Channel/dp/B07149WH7P),
 also available from other vendors);
-* The [&pi;-Plates DAQC2 plate](https://pi-plates.com/daqc2r1/). 
+* The [&pi;-Plates DAQC2 plate](https://pi-plates.com/daqc2r1/).
+
+__on Macs (and probably Windows)__
+* [Vernier](https://www.vernier.com) LabQuest USB A-to-Ds.
+
+__demo mode on anything Jupyter runs on__
 * A demo mode will run on any computer with a Jupyter notebook install and
 Python 3.6+. You can try the demo mode without installing on your own 
   computer by launching an instance on the MyBinder servers:
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JupyterPhysSciLab/JupyterPiDAQ.git/HEAD?urlpath=/tree/usage_examples)
   
 The goal is for the user interface to be as close to self-explanatory as
  possible. However, documentation is being developed along with some example
@@ -52,32 +38,44 @@
 code may provide additional sensors not listed here:
 * __ADS1115 compatible__ (board can provide 3.3 V of power/reference to
  sensors):
   * voltage reading (V, mV) from any sensor that puts out a voltage in the
    range +/-3.3 V.
   * built-in thermistor (V, mV, K, C, F).
   * Vernier SS temperature probe (V, mV, K, C, F).
+  
 * __DAQC2 compatible__ (board can provide 5.0 V of power/reference to sensors):
   * voltage reading (V, mV) from any sensor that puts out a voltage in the
    range +/- 12 V.
   * Vernier SS temperature probe (V, mV, K, C, F).
   * Vernier old and new pressure sensors (V, Pa, kPa, Bar, Torr, mmHg, atm)  
   * Vernier standard pH probe (V, mV, pH).
   * Vernier flat (tris compatible) pH probe (V, mV, pH).
   * Compatible with standard Vernier analog probes. Default calibrations
   being added as time and sensors become available.
-
-You can also hook up your own sensors and manually convert the raw voltage
-readings or write and submit a new sensor definition to the project.
+  
+* __LabQuest compatible__ (board provides 5.0 V of power/reference to sensors):
+  * voltage reading (V, mV) from any sensor that puts out a voltage in the
+   range +/- 10 V.
+  * Vernier SS temperature probe (V, mV, K, C, F).
+  * Vernier old and new pressure sensors (V, Pa, kPa, Bar, Torr, mmHg, atm)  
+  * Vernier standard pH probe (V, mV, pH).
+  * Vernier flat (tris compatible) pH probe (V, mV, pH).
+  * Compatible with standard Vernier analog probes. Default calibrations
+  being added as time and sensors become available.
+  
+With any of these interfaces, you can hook up your own sensors and 
+manually convert the raw voltage readings or write and submit a new sensor 
+definition to the project.
 
 ### License:
 [This software is distributed under the GNU V3 license](https://gnu.org/licenses).
 This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
     This program is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
-Copyright - Jonathan Gutow, 2021, 2022.
+Copyright - Jonathan Gutow, 2021, 2022, 2023.
```

### Comparing `JupyterPiDAQ-0.7.9/JupyterPiDAQ.egg-info/SOURCES.txt` & `JupyterPiDAQ-0.8.0.dev0/JupyterPiDAQ.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -15,11 +15,13 @@
 jupyterpidaq/Boards/boards.py
 jupyterpidaq/Boards/PiGPIO/ADS1115.py
 jupyterpidaq/Boards/PiGPIO/DAQC2.py
 jupyterpidaq/Boards/PiGPIO/__init__.py
 jupyterpidaq/Boards/Simulated/ADCsim.py
 jupyterpidaq/Boards/Simulated/ADCsim_line.py
 jupyterpidaq/Boards/Simulated/__init__.py
+jupyterpidaq/Boards/vernier/__init__.py
+jupyterpidaq/Boards/vernier/labquest.py
 jupyterpidaq/Sensors/__init__.py
 jupyterpidaq/Sensors/sensors.py
 jupyterpidaq/javascript/JupyterPiDAQmnu.js
 tests/test_boards.py
```

### Comparing `JupyterPiDAQ-0.7.9/PKG-INFO` & `JupyterPiDAQ-0.8.0.dev0/JupyterPiDAQ.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JupyterPiDAQ
-Version: 0.7.9
+Version: 0.8.0.dev0
 Summary: Data Acquisition in Jupyter notebook on Raspberry Pi
 Home-page: https://github.com/JupyterPhysSciLab/JupyterPiDAQ
 Author: Jonathan Gutow
 Author-email: gutow@uwosh.edu
 License: GPL-3.0+
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -19,25 +19,29 @@
 ## JupyterPiDAQ
 [Introduction](#introduction) | [License](#license)
 
 ### [Website/Documentation](https://jupyterphysscilab.github.io/JupyterPiDAQ/)
 
 ### Introduction:
 This software allows realtime collection and plotting of 
-digitized data in  a Jupyter notebook. The package was initially developed
+digitized data inside  a Jupyter notebook. The package was initially developed
 to provide an inexpensive laboratory system for teaching based on
-the Raspberry Pi.  However, as the development has progressed the data
-acquisition board drivers have been separated out of the user interface,
-so that the software has potential to work on other computers running Jupyter
-with A-to-D board specific connector code. Presently the compatible A-to-Ds are
-for Raspberry Pis: 
+the Raspberry Pi.  __However, it now also works on other hardware__. 
+Presently the working combinations are:
+
+__on Raspberry Pis__ 
 * Adafruit compliant ADS1115 boards 
 ([example](https://www.amazon.com/KNACRO-4-Channel-Raspberry-ADS1115-Channel/dp/B07149WH7P),
 also available from other vendors);
-* The [&pi;-Plates DAQC2 plate](https://pi-plates.com/daqc2r1/). 
+* The [&pi;-Plates DAQC2 plate](https://pi-plates.com/daqc2r1/).
+
+__on Macs (and probably Windows)__
+* [Vernier](https://www.vernier.com) LabQuest USB A-to-Ds.
+
+__demo mode on anything Jupyter runs on__
 * A demo mode will run on any computer with a Jupyter notebook install and
 Python 3.6+. You can try the demo mode without installing on your own 
   computer by launching an instance on the MyBinder servers:
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JupyterPhysSciLab/JupyterPiDAQ.git/HEAD?urlpath=/tree/usage_examples)
   
 The goal is for the user interface to be as close to self-explanatory as
  possible. However, documentation is being developed along with some example
@@ -52,32 +56,44 @@
 code may provide additional sensors not listed here:
 * __ADS1115 compatible__ (board can provide 3.3 V of power/reference to
  sensors):
   * voltage reading (V, mV) from any sensor that puts out a voltage in the
    range +/-3.3 V.
   * built-in thermistor (V, mV, K, C, F).
   * Vernier SS temperature probe (V, mV, K, C, F).
+  
 * __DAQC2 compatible__ (board can provide 5.0 V of power/reference to sensors):
   * voltage reading (V, mV) from any sensor that puts out a voltage in the
    range +/- 12 V.
   * Vernier SS temperature probe (V, mV, K, C, F).
   * Vernier old and new pressure sensors (V, Pa, kPa, Bar, Torr, mmHg, atm)  
   * Vernier standard pH probe (V, mV, pH).
   * Vernier flat (tris compatible) pH probe (V, mV, pH).
   * Compatible with standard Vernier analog probes. Default calibrations
   being added as time and sensors become available.
-
-You can also hook up your own sensors and manually convert the raw voltage
-readings or write and submit a new sensor definition to the project.
+  
+* __LabQuest compatible__ (board provides 5.0 V of power/reference to sensors):
+  * voltage reading (V, mV) from any sensor that puts out a voltage in the
+   range +/- 10 V.
+  * Vernier SS temperature probe (V, mV, K, C, F).
+  * Vernier old and new pressure sensors (V, Pa, kPa, Bar, Torr, mmHg, atm)  
+  * Vernier standard pH probe (V, mV, pH).
+  * Vernier flat (tris compatible) pH probe (V, mV, pH).
+  * Compatible with standard Vernier analog probes. Default calibrations
+  being added as time and sensors become available.
+  
+With any of these interfaces, you can hook up your own sensors and 
+manually convert the raw voltage readings or write and submit a new sensor 
+definition to the project.
 
 ### License:
 [This software is distributed under the GNU V3 license](https://gnu.org/licenses).
 This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
     This program is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
-Copyright - Jonathan Gutow, 2021, 2022.
+Copyright - Jonathan Gutow, 2021, 2022, 2023.
```

### Comparing `JupyterPiDAQ-0.7.9/README.md` & `JupyterPiDAQ-0.8.0.dev0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,47 @@
+Metadata-Version: 2.1
+Name: JupyterPiDAQ
+Version: 0.8.0.dev0
+Summary: Data Acquisition in Jupyter notebook on Raspberry Pi
+Home-page: https://github.com/JupyterPhysSciLab/JupyterPiDAQ
+Author: Jonathan Gutow
+Author-email: gutow@uwosh.edu
+License: GPL-3.0+
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: JavaScript
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+
 ## JupyterPiDAQ
 [Introduction](#introduction) | [License](#license)
 
 ### [Website/Documentation](https://jupyterphysscilab.github.io/JupyterPiDAQ/)
 
 ### Introduction:
 This software allows realtime collection and plotting of 
-digitized data in  a Jupyter notebook. The package was initially developed
+digitized data inside  a Jupyter notebook. The package was initially developed
 to provide an inexpensive laboratory system for teaching based on
-the Raspberry Pi.  However, as the development has progressed the data
-acquisition board drivers have been separated out of the user interface,
-so that the software has potential to work on other computers running Jupyter
-with A-to-D board specific connector code. Presently the compatible A-to-Ds are
-for Raspberry Pis: 
+the Raspberry Pi.  __However, it now also works on other hardware__. 
+Presently the working combinations are:
+
+__on Raspberry Pis__ 
 * Adafruit compliant ADS1115 boards 
 ([example](https://www.amazon.com/KNACRO-4-Channel-Raspberry-ADS1115-Channel/dp/B07149WH7P),
 also available from other vendors);
-* The [&pi;-Plates DAQC2 plate](https://pi-plates.com/daqc2r1/). 
+* The [&pi;-Plates DAQC2 plate](https://pi-plates.com/daqc2r1/).
+
+__on Macs (and probably Windows)__
+* [Vernier](https://www.vernier.com) LabQuest USB A-to-Ds.
+
+__demo mode on anything Jupyter runs on__
 * A demo mode will run on any computer with a Jupyter notebook install and
 Python 3.6+. You can try the demo mode without installing on your own 
   computer by launching an instance on the MyBinder servers:
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JupyterPhysSciLab/JupyterPiDAQ.git/HEAD?urlpath=/tree/usage_examples)
   
 The goal is for the user interface to be as close to self-explanatory as
  possible. However, documentation is being developed along with some example
@@ -34,32 +56,44 @@
 code may provide additional sensors not listed here:
 * __ADS1115 compatible__ (board can provide 3.3 V of power/reference to
  sensors):
   * voltage reading (V, mV) from any sensor that puts out a voltage in the
    range +/-3.3 V.
   * built-in thermistor (V, mV, K, C, F).
   * Vernier SS temperature probe (V, mV, K, C, F).
+  
 * __DAQC2 compatible__ (board can provide 5.0 V of power/reference to sensors):
   * voltage reading (V, mV) from any sensor that puts out a voltage in the
    range +/- 12 V.
   * Vernier SS temperature probe (V, mV, K, C, F).
   * Vernier old and new pressure sensors (V, Pa, kPa, Bar, Torr, mmHg, atm)  
   * Vernier standard pH probe (V, mV, pH).
   * Vernier flat (tris compatible) pH probe (V, mV, pH).
   * Compatible with standard Vernier analog probes. Default calibrations
   being added as time and sensors become available.
-
-You can also hook up your own sensors and manually convert the raw voltage
-readings or write and submit a new sensor definition to the project.
+  
+* __LabQuest compatible__ (board provides 5.0 V of power/reference to sensors):
+  * voltage reading (V, mV) from any sensor that puts out a voltage in the
+   range +/- 10 V.
+  * Vernier SS temperature probe (V, mV, K, C, F).
+  * Vernier old and new pressure sensors (V, Pa, kPa, Bar, Torr, mmHg, atm)  
+  * Vernier standard pH probe (V, mV, pH).
+  * Vernier flat (tris compatible) pH probe (V, mV, pH).
+  * Compatible with standard Vernier analog probes. Default calibrations
+  being added as time and sensors become available.
+  
+With any of these interfaces, you can hook up your own sensors and 
+manually convert the raw voltage readings or write and submit a new sensor 
+definition to the project.
 
 ### License:
 [This software is distributed under the GNU V3 license](https://gnu.org/licenses).
 This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
     This program is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
-Copyright - Jonathan Gutow, 2021, 2022.
+Copyright - Jonathan Gutow, 2021, 2022, 2023.
```

### Comparing `JupyterPiDAQ-0.7.9/Tests/test_boards.py` & `JupyterPiDAQ-0.8.0.dev0/Tests/test_boards.py`

 * *Files identical despite different names*

### Comparing `JupyterPiDAQ-0.7.9/jupyterpidaq/Boards/PiGPIO/ADS1115.py` & `JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/PiGPIO/ADS1115.py`

 * *Files identical despite different names*

### Comparing `JupyterPiDAQ-0.7.9/jupyterpidaq/Boards/PiGPIO/DAQC2.py` & `JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/PiGPIO/DAQC2.py`

 * *Files identical despite different names*

### Comparing `JupyterPiDAQ-0.7.9/jupyterpidaq/Boards/Simulated/ADCsim.py` & `JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/Simulated/ADCsim.py`

 * *Files identical despite different names*

### Comparing `JupyterPiDAQ-0.7.9/jupyterpidaq/Boards/Simulated/ADCsim_line.py` & `JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/Simulated/ADCsim_line.py`

 * *Files identical despite different names*

### Comparing `JupyterPiDAQ-0.7.9/jupyterpidaq/Boards/boards.py` & `JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/boards.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 logger = logging.getLogger(__name__)
 
 # TODO: Update this list of available board options as they are created.
 # Name format is `.package.boardname` where `boardname` is the name of the
 # python file defining the required board operations.
 
 knownboardpkgs = ('jupyterpidaq.Boards.PiGPIO.ADS1115',
-                  'jupyterpidaq.Boards.PiGPIO.DAQC2')
+                  'jupyterpidaq.Boards.PiGPIO.DAQC2',
+                  'jupyterpidaq.Boards.vernier.labquest')
 knownsimulators = ('jupyterpidaq.Boards.Simulated.ADCsim',
                    'jupyterpidaq.Boards.Simulated.ADCsim_line')
 
 
 def load_boards():
     """
     Uses the list of known board packages to search for available boards.
```

### Comparing `JupyterPiDAQ-0.7.9/jupyterpidaq/ChannelSettings.py` & `JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/ChannelSettings.py`

 * *Files identical despite different names*

### Comparing `JupyterPiDAQ-0.7.9/jupyterpidaq/DAQProc.py` & `JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/DAQProc.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # the drawing process gets bogged down.
 # J. Gutow <gutow@uwosh.edu> May 19, 2019
 # license GPL V3 or greater.
 
 # utilities for timing and queues
 from collections import deque
 import time
+from jupyterpidaq.Boards.vernier.labquest import Board_LQ
 
 def DAQProc(whichchn, gains, avgtime, timedelta, DAQconn, DAQCTL):
     """
     This function is to be run in a separate thread to asynchronously
     communicate with the ADC board.
 
     :param list whichchn: a list of dictionaries. Each dictionary is of the
@@ -28,15 +29,15 @@
 
     :param pipe DAQCTL: the control pipe
 
     :return: Data is returned via the pipes.
         On the DAQCTL pipe this only returns 'done'
         On the DAQconn pipe a list of lists with data is returned.
     """
-    # f=open('daq.log','w')
+    #f=open('daq.log','w')
     databuf = deque()
     collect = True
     transmit = False
     chncnt = 0
     for i in range(len(whichchn)):
         if (whichchn[i]):
             chncnt += 1
@@ -48,63 +49,75 @@
         stdevs = []
         avg_stdevs = []
         avg_vdds = []
         calltime = time.time()
         for i in range(len(whichchn)):
             if (whichchn[i]):
                 time.sleep(0.001)
-                # f.write('Calling adc...')
-                v_avg, v_std, avg_std, meastime, vdd_avg = \
+                #f.write('Calling adc...')
+                if isinstance(whichchn[i]["board"],Board_LQ):
+                    v_avg, v_std, avg_std, meastime, vdd_avg = \
+                    whichchn[i]['board'].V_oversampchan_stats(whichchn[i][
+                                                                  'chnl'],
+                                                              gains[i],
+                                                              timedelta)
+                else:
+                    v_avg, v_std, avg_std, meastime, vdd_avg = \
                     whichchn[i]['board'].V_oversampchan_stats(whichchn[i][
                                                                    'chnl'],
                                                               gains[i],
                                                            avgtime)
-                # f.write('Successful return from call to adc.\n')
+                #f.write('Successful return from call to adc.\n')
                 times.append(meastime - starttime)
                 values.append(v_avg)
                 stdevs.append(v_std)
                 avg_stdevs.append(avg_std)
                 avg_vdds.append(vdd_avg)
         pkg.append(times)
         pkg.append(values)
         pkg.append(stdevs)
         pkg.append(avg_stdevs)
         pkg.append(avg_vdds)
         databuf.append(pkg)
-        # f.write('Buffer length: '+str(len(databuf))+'\n')
+        #f.write('Buffer length: '+str(len(databuf))+'\n')
+        #f.write('Buffer[0]: ' + str(databuf) + '\n')
         if DAQCTL.poll():
             CTLmsg = DAQCTL.recv()
             if (CTLmsg == 'Send' or CTLmsg == 'send'):
                 transmit = True
             if (CTLmsg == 'Stop' or CTLmsg == 'stop'):
                 collect = False
-        #   f.write('Received msg: '+str(CTLmsg)+'\n')
+            #f.write('Received msg: '+str(CTLmsg)+'\n')
         if transmit:  # the other end is ready
             navail = len(databuf)
             nsend = 60
             if (navail <= 60):
                 nsend = navail
             for i in range(nsend):
                 DAQconn.send(databuf.popleft())
-            #  f.write('Sent '+str(nsend)+' buffer chunks.\n')
+                #f.write('Sent '+str(nsend)+' buffer chunks.\n')
             transmit = False  # we've done our burst of sending.
         elapsedtime = time.time() - calltime
         if elapsedtime < timedelta:
             time.sleep(timedelta -elapsedtime- 0.002)
     # We should now send anything left...
-    # f.write('Left in buffer: '+str(len(databuf))+'\n')
+    #f.write('Left in buffer: '+str(len(databuf))+'\n')
     while len(databuf) > 1:
         if DAQCTL.poll():
             CTLmsg = DAQCTL.recv()
             if (CTLmsg == 'Send' or CTLmsg == 'send'):
                 transmit = True
         if transmit:  # the other end is ready
             navail = len(databuf)
             nsend = 60
             if (navail <= 60):
                 nsend = navail
             for i in range(nsend):
                 DAQconn.send(databuf.popleft())
             transmit = False  # we've done our burst of sending.
     DAQCTL.send('done')
-    # f.write('Cleared buffer. Quitting.\n\n')
-    # f.close()
+    # Wait a while to terminate so that the Pipe is up for the other end to
+    # collect the data.
+    #f.flush()
+    #f.close()
+    time.sleep(5)
+    return
```

### Comparing `JupyterPiDAQ-0.7.9/jupyterpidaq/DAQinstance.py` & `JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/DAQinstance.py`

 * *Files 8% similar despite different names*

```diff
@@ -119,45 +119,46 @@
     if os.stat(logname).st_size == 0:
         os.remove(logname)
 except FileNotFoundError:
     pass
 
 # Data Aquistion Instance (a run).
 class DAQinstance():
-    def __init__(self, idno, livefig, title='None', ntraces=4, **kwargs):
+    def __init__(self, idno, title='None', ntraces=4, **kwargs):
         """
         Data Aquistion Instance (a run).
 
         :param idno : id number you wish to use to keep track
-        :param livefig: plotly FigureWidget to use for live display
         :param title: optional name
         :param ntraces: number of traces (default = 4) more than 4 easily
             overwhelms a pi4.
         :param kwargs:
             :ignore_skew: bool (default: True) if True only a single average
             collection time will be recorded for each time in a multichannel
             data collection. If False a separate set of time will be
             recorded for each channel.
         """
+        from plotly import graph_objects as go
         self.ignore_skew = kwargs.pop('ignore_skew',True)
         self.idno = idno
-        self.livefig = livefig
+        self.livefig = go.FigureWidget(layout_template='simple_white')
         self.title = str(title)
-        self.svname = ''
+        self.svname = title + '.jpidaq.html'
         self.averaging_time = 0.1  # seconds adjusted based on collection rate
         self.gain = [1] * ntraces
         self.data = []
         self.timestamp = []
         self.stdev = []
         self.pandadf = None
         self.ntraces = ntraces
         self.separate_plots = True
         self.traces = []
         # index map from returned data to trace,
         self.tracemap = []
+        self.tracefrdatachn = []
         self.tracelbls = []
         self.units = []
         for i in range(self.ntraces):
             self.traces.append(ChannelSettings(i, availboards))
         self.ratemax = 20.0  # Hz
         self.rate = 1.0  # Hz
         self.deltamin = 1 / self.ratemax
@@ -210,15 +211,15 @@
             placeholder='',
             description='')
         self.setup_layout_bottom = widgets.HBox(
             [self.rateinp, self.timelbl, self.setupbtn])
         self.setup_layout = widgets.VBox([self.separate_traces_checkbox,
                                           self.setup_layout_bottom])
         self.collect_layout = widgets.HBox([self.collectbtn, self.collecttxt])
-        
+        self.output = widgets.Output()
     def _make_defaultparamtxt(self):
         """
         Uses AdvancedHTMLParser (mimics javascript) to generate valid HTML for
         the default parameter text.
         :return: valid html string for the default parameter text.
         """
         from AdvancedHTMLParser import AdvancedTag as domel
@@ -413,85 +414,109 @@
         self.delta = 1 / self.rate
         self.separate_plots = copy(self.separate_traces_checkbox.value)
         self.defaultparamtxt = self._make_defaultparamtxt()
         self.runtitle.close()
         del self.runtitle
         self.setup_layout.close()
         del self.setup_layout
-        JPSLUtils.new_cell_immediately_below()
-        cmdstr = 'doRun(runs[' + str(self.idno - 1) + '])'
-        cmdstr += '\\nruns[' + str(self.idno - 1) + '].livefig'
-        JPSLUtils.insert_text_into_next_cell(cmdstr)
-        JPSLUtils.select_containing_cell("RunSetUp")
-        JPSLUtils.select_cell_immediately_below()
-        JPSLUtils.OTJS('Jupyter.notebook.get_selected_cell().execute()')
+        self.output.clear_output()
+        doRun(runs[self.idno-1])
+        with self.output:
+            display(runs[self.idno - 1].livefig)
         pass
 
     def setup(self):
-        display(HTML("<h3 id ='RunSetUp' "
-                     "style='text-align:center;'>Set Run Parameters</h3>"))
-        self.setupbtn.on_click(self.setupclick)
-        display(self.runtitle)
-        for i in range(self.ntraces):
-            self.traces[i].setup()
-        display(self.setup_layout)
+        with self.output:
+            display(HTML("<h3 id ='RunSetUp' "
+                         "style='text-align:center;'>Set Run Parameters</h3>"))
+            self.setupbtn.on_click(self.setupclick)
+            display(self.runtitle)
+            for i in range(self.ntraces):
+                self.traces[i].setup()
+            display(self.setup_layout)
+        display(self.output)
         pass
 
     def collectclick(self, btn):
         if (btn.description == 'Start Collecting'):
             btn.description = 'Stop Collecting'
             btn.button_style = 'danger'
             btn.tooltip = 'Stop the data collection'
             # do not allow parameters to be reset after starting run.
             self.setupbtn.disabled = True
             self.setupbtn.tooltip = 'Parameters locked. The run has started.'
             self.rateinp.disabled = True
             self.timelbl.disabled = True
-            thread = threading.Thread(target=self.updatingplot, args=())
+            PLTconn, DAQconn = Pipe()
+            DAQCTL, PLTCTL = Pipe()
+            nactive = 0
+            for k in self.traces:
+                if k.isactive:
+                    nactive += 1
+            whichchn = []
+            gains =[]
+            for i in range(self.ntraces):
+                if (self.traces[i].isactive):
+                    brd = self.traces[i].board
+                    chn = self.traces[i].channel
+                    newchn = True
+                    if len(whichchn) > 0:
+                        for k in range(len(whichchn)):
+                            if whichchn[k]['board'] == brd \
+                                and whichchn[k]['chnl'] == chn:
+                                self.tracefrdatachn.append(k)
+                                newchn = False
+                    if newchn:
+                        whichchn.append({'board': brd,
+                                         'chnl': chn})
+                        gains.append(self.traces[i].toselectedgain)
+                        self.tracefrdatachn.append(len(whichchn)-1)
+            # Use up to 30% of the time for averaging if channels were spaced
+            # evenly between data collection times (with DACQ2 they appear
+            # more synchronous than that).
+            self.averaging_time = self.delta / nactive / 3
+            DAQ = Process(target=DAQProc,
+                          args=(
+                              whichchn, gains, self.averaging_time, self.delta,
+                              DAQconn, DAQCTL))
+            DAQ.start()
+            thread = threading.Thread(target=self.updatingplot, args=(
+                                        PLTconn, PLTCTL))
             thread.start()
             # self.updatingplot() hangs up user interface
         else:
             btn.description = 'Done'
             btn.button_style = ''
             btn.tooltip = ''
             time.sleep(3)  # wait a few seconds for end of data collection
             self.data = data
             self.timestamp = timestamp
             self.stdev = stdev
             self.fillpandadf()
             # save data to html file so it is human readable and can be loaded
             # elsewhere.
-            self.svname = self.title + '_' + time.strftime('%y-%m-%d_%H%M%S',
-                                        time.localtime()) + '.html'
+            #self.svname = self.title + '_' + time.strftime('%y-%m-%d_%H%M%S',
+                                       # time.localtime()) + '.html'
             svhtml = '<!DOCTYPE html>' \
                      '<html><body>'+ self.defaultparamtxt + \
                      '<table id="file_info" border="1"><tr><th>Saved as ' \
                      '</th></tr><tr><td>' +  \
                      self.svname+'</td></tr></table>' \
                      '<h2>DATA</h2>'+ \
                      self.pandadf.to_html() + '</body></html>'
             f = open(self.svname,'w')
             f.write(svhtml)
             f.close()
             self.collectbtn.close()
             del self.collectbtn
-            #display(self.collecttxt)
-            display(HTML(
-                '<span style="color:blue;font-weight:bold;">DATA SAVED TO:' +
-                self.svname + '</span>'))
-            JPSLUtils.select_containing_cell('LiveRun_'+str(self.idno))
-            JPSLUtils.new_cell_immediately_below()
-            cmdstr = 'from jupyterpidaq.DAQinstance import * ' \
-                    '# Does nothing if already imported.\n' \
-                    'displayRun(' + str(self.idno)+', \"' \
-                    + self.svname + '\") # display the data'
-            JPSLUtils.insert_text_into_next_cell(cmdstr)
-            JPSLUtils.select_containing_cell('LiveRun_'+str(self.idno))
-            JPSLUtils.select_cell_immediately_below()
-            JPSLUtils.OTJS('Jupyter.notebook.get_selected_cell().execute()')
+            with self.output:
+                display(HTML(
+                    '<span style="color:blue;font-weight:bold;">DATA SAVED TO:' +
+                    self.svname + '</span>'))
+        return
 
     def fillpandadf(self):
         datacolumns = []
         temptimes = np.transpose(self.timestamp)
         tempdata = np.transpose(self.data)
         tempstdev = np.transpose(self.stdev)
         chncnt = 0
@@ -523,37 +548,80 @@
                         i].units.value + ')')
                 titles.append(
                     self.traces[i].tracelbl.value + '_' + 'stdev')
         #print(str(titles))
         #print(str(datacolumns))
         self.pandadf = pd.DataFrame(np.transpose(datacolumns), columns=titles)
 
-    def updatingplot(self):
+    def updatingplot(self, PLTconn, PLTCTL):
         """
         Runs until a check of self.collectbtn.description does not return
         'Stop Collecting'. This would probably be more efficient if set a
         boolean.
+        Parameters
+        ----------
+        PLTconn: Pipe
+            connection plotter end
+        DAQconn: Pipe
+            connection DAQ end
+        PLTCTL: Pipe
+            control pipe plotter end
+        DAQCTL: Pipe
+            control pipe DAQ end
         """
         starttime = time.time()
         global data
         data = []
         global timestamp
         timestamp = []
         global stdev
         stdev = []
         datalegend = []
         timelegend = []
         stdevlegend = []
-        PLTconn, DAQconn = Pipe()
-        DAQCTL, PLTCTL = Pipe()
         whichchn = []
         gains = []
         toplotx = []
         toploty = []
         nactive = 0
+        def convert_pkg():
+            plttime = 0
+            if self.ignore_skew:
+                plttime = sum(pkg[0]) / len(pkg[0])
+            traceidx = 0
+            tmptime = []
+            tmpavg = []
+            tmpstd = []
+            tmpavg_std = []
+            for i, k in zip(self.tracemap, self.tracefrdatachn):
+
+                avg = pkg[1][k]
+                std = pkg[2][k]
+                avg_std = pkg[3][k]
+                avg_vdd = pkg[4][k]
+                avg, std, avg_std = self.traces[i].toselectedunits(avg,
+                                                                   std, avg_std,
+                                                                   avg_vdd)
+                avg, std, avg_std = sensors. \
+                    to_reasonable_significant_figures_fast(avg, std, avg_std)
+                tmptime.append(pkg[0][k])
+                tmpavg.append(avg)
+                tmpstd.append(std)
+                tmpavg_std.append(avg_std)
+                if self.ignore_skew:
+                    toplotx[traceidx].append(plttime)
+                else:
+                    toplotx[traceidx].append(pkg[0][k])
+                toploty[traceidx].append(avg)
+                traceidx += 1
+            timestamp.append(tmptime)
+            data.append(tmpavg)
+            stdev.append(tmpavg_std)
+            return
+
         for k in self.traces:
             if k.isactive:
                 nactive += 1
         if self.separate_plots:
             self.livefig.set_subplots(rows = nactive, cols = 1,
                                       shared_xaxes= True)
             self.livefig.update_xaxes(title = self.timelbl.value,
@@ -561,17 +629,14 @@
         else:
             self.livefig.update_yaxes(title = "Values")
             self.livefig.update_xaxes(title = self.timelbl.value)
         active_count = 0
         for i in range(self.ntraces):
             if (self.traces[i].isactive):
                 active_count += 1
-                whichchn.append({'board':self.traces[i].board,
-                                'chnl':self.traces[i].channel})
-                gains.append(self.traces[i].toselectedgain)
                 tempstr = self.traces[i].tracelbl.value + '(' + \
                           self.traces[i].units.value + ')'
                 timelegend.append('time_' + tempstr)
                 datalegend.append(tempstr)
                 stdevlegend.append('stdev_' + tempstr)
                 if self.separate_plots:
                     scat = go.Scatter(y=[],x=[], name=tempstr)
@@ -579,61 +644,27 @@
                                            col = 1)
                     self.livefig.update_yaxes(title = self.traces[
                         i].units.value, row = active_count, col = 1)
                 else:
                     self.livefig.add_scatter(y=[],x=[], name=tempstr)
                 toplotx.append([])
                 toploty.append([])
-                
-        #print('whichchn: '+str(whichchn))
-        #print('gains: '+str(gains))
-        # Use up to 30% of the time for averaging if channels were spaced
-        # evenly between data collection times (with DACQ2 they appear
-        # more synchronous than that).
-        self.averaging_time = self.delta/nactive/3
-        DAQ = Process(target=DAQProc,
-                      args=(
-                      whichchn, gains, self.averaging_time, self.delta,
-                      DAQconn, DAQCTL))
-        DAQ.start()
         lastupdatetime = time.time()
 
         pts = 0
         oldpts = 0
         #print('about to enter while loop',end='')
         while (self.collectbtn.description == 'Stop Collecting'):
             #print('.',end='')
             while PLTconn.poll():
                 pkg = PLTconn.recv()
                 self.lastpkgstr = str(pkg)
                 #print(self.lastpkgstr)
                 # convert voltage to requested units.
-                tmptime = 0
-                if self.ignore_skew:
-                    tmptime = sum(pkg[0]) / len(pkg[0])
-                for i in range(len(pkg[0])):
-                    avg = pkg[1][i]
-                    std = pkg[2][i]
-                    avg_std = pkg[3][i]
-                    avg_vdd = pkg[4][i]
-                    avg, std, avg_std = self.traces[
-                        self.tracemap[i]].toselectedunits(avg, std, avg_std, avg_vdd)
-                    avg, std, avg_std = sensors.to_reasonable_significant_figures_fast(
-                        avg, std, avg_std)
-                    pkg[1][i] = avg
-                    pkg[2][i] = std
-                    pkg[3][i] = avg_std
-                    if self.ignore_skew:
-                        toplotx[i].append(tmptime)
-                    else:
-                        toplotx[i].append(pkg[0][i])
-                    toploty[i].append(avg)
-                timestamp.append(pkg[0])
-                data.append(pkg[1])
-                stdev.append(pkg[3])
+                convert_pkg()
             currenttime = time.time()
             mindelay = 1.0
             if self.separate_traces_checkbox.value:
                 mindelay = nactive*1.0
             else:
                 mindelay = nactive*0.5
             if (currenttime - lastupdatetime)>(mindelay+len(toplotx[0])*len(
@@ -653,131 +684,139 @@
         time.sleep(0.5)
         msg = ''
         while (msg != 'done'):
             while PLTconn.poll():
                 pkg = PLTconn.recv()
                 # print(str(pkg))
                 # convert voltage to requested units.
-                for i in range(len(pkg[0])):
-                    avg = pkg[1][i]
-                    std = pkg[2][i]
-                    avg_std = pkg[3][i]
-                    avg_vdd = pkg[4][i]
-                    avg, std, avg_std = self.traces[
-                        self.tracemap[i]].toselectedunits(avg, std, avg_std, avg_vdd)
-                    avg, std, avg_std = sensors.to_reasonable_significant_figures_fast(
-                        avg, std, avg_std)
-                    pkg[1][i] = avg
-                    pkg[2][i] = std
-                    pkg[3][i] = avg_std
-                    if self.ignore_skew:
-                        tmptime = sum(pkg[0])/len(pkg[0])
-                        toplotx[i].append(tmptime)
-                    else:
-                        toplotx[i].append(pkg[0][i])
-                    toploty[i].append(avg)
-                    #print(pkg[0][i])
-                    #print(avg)
-                timestamp.append(pkg[0])
-                data.append(pkg[1])
-                stdev.append(pkg[3])
+                convert_pkg()
             PLTCTL.send('send')
             time.sleep(0.2)
             if PLTCTL.poll():
                 msg = PLTCTL.recv()
                 # print (str(msg))
                 if (msg != 'done'):
                     print('Received unexpected message: ' + str(msg))
         for k in range(len(self.livefig.data)):
             self.livefig.data[k].x = toplotx[k]
             self.livefig.data[k].y = toploty[k]
-        DAQ.join()  # make sure garbage collection occurs when it stops.
-        DAQconn.close()
-        PLTconn.close()
-        DAQCTL.close()
-        PLTCTL.close()
-
 
-def newRun(livefig):
-    """
-    Set up a new data collection run and add it to the list of runs.
-    """
-    nrun = len(runs) + 1
-    runs.append(DAQinstance(nrun, livefig, title='Run-' + str(nrun)))
-    runs[nrun - 1].setup()
-    pass
-
-def doRun(whichrun):
-    display(HTML('<span id="LiveRun_'+str(whichrun.idno)+'"></span>'))
-    display(HTML(whichrun.defaultparamtxt))
-    if hasattr(whichrun, "collectbtn"):
-        # only show if hasn't already collected data
-        whichrun.collectbtn.on_click(whichrun.collectclick)
-        display(whichrun.collectbtn)
-    display(HTML(whichrun.defaultcollecttxt))
-    JPSLUtils.select_containing_cell("RunSetUp")
-    JPSLUtils.delete_selected_cell()
-    pass
-
-def displayRun(runidx,file):
-    """
-    Displays a run. It can fall back to loading from a file if the outputarea
-    is accidentally cleared.
-    :param runidx: index+1 for the run in the runs array. Thus, the run id #.
-    :param file: name of the file the run is saved to
-    :return: A string warning if things are not initialized properly.
+# TODO delete newRun once sure not needed.
+# def newRun(livefig):
+#     """
+#     Set up a new data collection run and add it to the list of runs.
+#     """
+#     nrun = len(runs) + 1
+#     runs.append(DAQinstance(nrun, livefig, title='Run-' + str(nrun)))
+#     runs[nrun - 1].setup()
+#     pass
+
+def Run(name):
+    """Load a run from stored data or start a new run if the local file for
+    the run does not exist.
+    Parameters
+    ----------
+    name: str
+        String name for the run. The data will be stored in a file of this
+        name with the extension of `.jpidaq.html`.
     """
+    from pathlib import Path
     from IPython import get_ipython
-    from JPSLUtils import find_pandas_dataframe_names, find_figure_names
-    idxnum = runidx - 1
-    run_id_table = pd.read_html(file, attrs={'id': 'run_id'})[0]
-    run_title = run_id_table['Title'][0]
-    run_id = run_id_table['Id #'][0]
-    svname = pd.read_html(file, attrs={'id': 'file_info'})[0]['Saved as'][0]
+    from IPython.display import display
     global_dict = get_ipython().user_ns
     runs = None
     if 'runs' in global_dict and 'DAQinstance' in global_dict:
         runs = global_dict['runs']
     else:
         return ('Initialization of JupyterPiDAQ required')
-    exists = None
-    if len(runs)>=runidx:
-        if isinstance(runs[idxnum].livefig,go.FigureWidget) and runs[
-            idxnum].idno == run_id and runs[idxnum].svname ==svname:
-            exists = True
-        else:
-            exists = False
-    if exists:
-        display(HTML(runs[idxnum].defaultparamtxt))
-        display(HTML('<h3>Saved as: '+runs[idxnum].svname+'</h3>'))
-        runs[idxnum].livefig.show()
-        display(HTML(runs[idxnum].defaultcollecttxt))
-        JPSLUtils.select_containing_cell("LiveRun_"+str(runidx))
-        JPSLUtils.delete_selected_cell()
-    else:
-        # Fall back on loading the data from the default save file.
-        # Note: the file must be available.
-        nrunfigs = 0
-        for k in find_figure_names():
-            if k.startswith('run_fig'):
-                nrunfigs+=1
-        runfigname = 'run_fig'+str(nrunfigs+1)
-        global_dict[runfigname] = go.FigureWidget()
-        fig = global_dict[runfigname]
-        runs.append(DAQinstance(run_id, fig, title=run_title))
-        idxnum = len(runs)-1
-        runs[idxnum]._load_from_html(file)
-        display(HTML(runs[idxnum].defaultparamtxt))
-        display(HTML('<h3>Saved as: ' + runs[idxnum].svname + '</h3>'))
-        runs[idxnum].livefig.show()
-        display(HTML(runs[idxnum].defaultcollecttxt))
-    # protect the cell
-    JPSLUtils.OTJS('protect_selected_cells();')
+    # Check if run completed, if so reload data, display and exit
+    datafilepath = Path.cwd() / Path(str(name) + '.jpidaq.html')
+    if datafilepath.exists():
+        # display the data as a live plotly plot.
+        svname = name + '.jpidaq.html'
+        runs.append(DAQinstance(len(runs)+1, title = name))
+        runs[-1]._load_from_html(svname)
+        display(HTML(runs[-1].defaultparamtxt))
+        display(HTML('<h3>Saved as: '+runs[-1].svname+'</h3>'))
+        display(runs[-1].livefig)
+        display(HTML(runs[-1].defaultcollecttxt))
+        return
+    nrun = len(runs) + 1
+    runs.append(DAQinstance(nrun, title=name))
+    runs[-1].setup()
+    return
+
+def doRun(whichrun):
+    with whichrun.output:
+        display(HTML('<span id="LiveRun_'+str(whichrun.idno)+'"></span>'))
+        display(HTML(whichrun.defaultparamtxt))
+        if hasattr(whichrun, "collectbtn"):
+            # only show if hasn't already collected data
+            whichrun.collectbtn.on_click(whichrun.collectclick)
+            display(whichrun.collectbtn)
+        display(HTML(whichrun.defaultcollecttxt))
     pass
 
+# TODO delete displayRun once not needed.
+# def displayRun(runidx,file):
+#     """
+#     Displays a run. It can fall back to loading from a file if the outputarea
+#     is accidentally cleared.
+#     :param runidx: index+1 for the run in the runs array. Thus, the run id #.
+#     :param file: name of the file the run is saved to
+#     :return: A string warning if things are not initialized properly.
+#     """
+#     from IPython import get_ipython
+#     from JPSLUtils import find_pandas_dataframe_names, find_figure_names
+#     idxnum = runidx - 1
+#     run_id_table = pd.read_html(file, attrs={'id': 'run_id'})[0]
+#     run_title = run_id_table['Title'][0]
+#     run_id = run_id_table['Id #'][0]
+#     svname = pd.read_html(file, attrs={'id': 'file_info'})[0]['Saved as'][0]
+#     global_dict = get_ipython().user_ns
+#     runs = None
+#     if 'runs' in global_dict and 'DAQinstance' in global_dict:
+#         runs = global_dict['runs']
+#     else:
+#         return ('Initialization of JupyterPiDAQ required')
+#     exists = None
+#     if len(runs)>=runidx:
+#         if isinstance(runs[idxnum].livefig,go.FigureWidget) and runs[
+#             idxnum].idno == run_id and runs[idxnum].svname ==svname:
+#             exists = True
+#         else:
+#             exists = False
+#     if exists:
+#         display(HTML(runs[idxnum].defaultparamtxt))
+#         display(HTML('<h3>Saved as: '+runs[idxnum].svname+'</h3>'))
+#         runs[idxnum].livefig.show()
+#         display(HTML(runs[idxnum].defaultcollecttxt))
+#         JPSLUtils.select_containing_cell("LiveRun_"+str(runidx))
+#         JPSLUtils.delete_selected_cell()
+#     else:
+#         # Fall back on loading the data from the default save file.
+#         # Note: the file must be available.
+#         nrunfigs = 0
+#         for k in find_figure_names():
+#             if k.startswith('run_fig'):
+#                 nrunfigs+=1
+#         runfigname = 'run_fig'+str(nrunfigs+1)
+#         global_dict[runfigname] = go.FigureWidget()
+#         fig = global_dict[runfigname]
+#         runs.append(DAQinstance(run_id, fig, title=run_title))
+#         idxnum = len(runs)-1
+#         runs[idxnum]._load_from_html(file)
+#         display(HTML(runs[idxnum].defaultparamtxt))
+#         display(HTML('<h3>Saved as: ' + runs[idxnum].svname + '</h3>'))
+#         runs[idxnum].livefig.show()
+#         display(HTML(runs[idxnum].defaultcollecttxt))
+#     # protect the cell
+#     JPSLUtils.OTJS('protect_selected_cells();')
+#     pass
+
 def update_runsdrp():
     # get list of runs
     runlst = [('Choose Run', -1)]
     for i in range(len(runs)):
         runlst.append((str(i + 1) + ': ' + runs[i].title, i))
     # buid selection menu
     global runsdrp
@@ -787,32 +826,41 @@
         description='Select Run #:',
         disabled=False,
     )
     pass
 
 def showSelectedRunTable(change):
     global runsdrp
+    global last_run_table_out
     whichrun = runsdrp.value
     runsdrp.close()
+    last_run_table_out.clear_output()
     tbldiv = '<div style="height:10em;">' + str(runs[whichrun].title)
     tbldiv += str(runs[whichrun].pandadf.to_html()) + '</div>'
-    display(HTML(tbldiv))
+    with last_run_table_out:
+        display(HTML(tbldiv))
+    return
 
 def showDataTable():
     """
     Provides a menu to select which run. Then displays the run in a
     10 em high scrolling table. Selection menu is removed after choice
     is made.
     """
+    from ipywidgets import Output
+    global last_run_table_out
+    last_run_table_out = Output()
     update_runsdrp()
     global runsdrp
     runsdrp.observe(showSelectedRunTable, names='value')
-    display(runsdrp)
+    with last_run_table_out:
+        display(runsdrp)
+    display(last_run_table_out)
     # will display selected run and delete menu upon selection.
-
+    return
 def newCalculatedColumn():
     """
     Uses jupyter-pandas-GUI.new_pandas_column_GUI to provide a GUI expression
     composer. This method finds the datasets and launches the GUI.
     """
     df_info = []
     for i in range(len(runs)):
```

### Comparing `JupyterPiDAQ-0.7.9/jupyterpidaq/Sensors/sensors.py` & `JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Sensors/sensors.py`

 * *Files identical despite different names*

### Comparing `JupyterPiDAQ-0.7.9/jupyterpidaq/javascript/JupyterPiDAQmnu.js` & `JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/javascript/JupyterPiDAQmnu.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,45 +1,48 @@
 // TODO: isolate under a name such as juputerPiDAQ.
 var insertruncount = 0
-var newrunstr = 'run_fig$ = go.FigureWidget() # Create figure to show data.\n'
-newrunstr += 'newRun(run_fig$) # Initiate run setup.'
-//newrunstr += 'fig$ # Display the live figure.'
+var newrunstr = '# EDIT THE COMMAND BELOW BY PROVIDING A RUN NAME.\n'
+newrunstr += '# The name should be surrounded by double quotes ("run_name").\n'
+newrunstr += '# using _ instead of spaces will avoid problems, especially on '
+newrunstr += 'Windows machines.\n'
+newrunstr += 'Run("REPLACE_ME_WITH_NAME_FOR_RUN") # Initiate run or load a '
+newrunstr += 'completed run.'
 
 function insertnewRun() {
     //Insert a cell below the current selection
     Jupyter.notebook.insert_cell_below();
     Jupyter.notebook.select_next(true);
     Jupyter.notebook.focus_cell();
     var currentcell = Jupyter.notebook.get_selected_cell();
     insertruncount += 1
-    var cmdstr = newrunstr.replaceAll('$', insertruncount)
+    var cmdstr = newrunstr
     currentcell.set_text(cmdstr);
-    currentcell.execute();
+    //currentcell.execute();
 }
 
 function addnewRun() {
     //find the last cell in notebook
     var lastcellidx = Jupyter.notebook.ncells() - 1;
     var lastcell = Jupyter.notebook.get_cell(lastcellidx);
     Jupyter.notebook.select(lastcellidx);
     //If the cell is empty put command in it. Otherwise
     //add another cell at the end of the worksheet. Then
     //put the command in the new lastcell.
     insertruncount += 1
-    var cmdstr = newrunstr.replaceAll('$', insertruncount)
+    var cmdstr = newrunstr
     if (lastcell.get_text() == '') {
         lastcell.set_text(cmdstr);
     } else {
         Jupyter.notebook.insert_cell_below();
         Jupyter.notebook.select_next(true);
         Jupyter.notebook.focus_cell();
         lastcell = Jupyter.notebook.get_cell(lastcellidx + 1);
         lastcell.set_text(cmdstr);
     }
-    lastcell.execute();
+    //lastcell.execute();
 }
 
 function showDataTable() {
     //find the currently active cell
     var currentcell = Jupyter.notebook.get_selected_cell();
     //Because we could destroy date created by having run
     //this cell previously do not use this cell if it contains
```

### Comparing `JupyterPiDAQ-0.7.9/setup.py` & `JupyterPiDAQ-0.8.0.dev0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="JupyterPiDAQ",
     url = "https://github.com/JupyterPhysSciLab/JupyterPiDAQ",
-    version="0.7.9",
+    version="0.8.0dev",
     description="Data Acquisition in Jupyter notebook on Raspberry Pi",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Jonathan Gutow",
     author_email="gutow@uwosh.edu",
     license="GPL-3.0+",
     packages=setuptools.find_packages(exclude=("dist","build","dev_testing",)),
@@ -25,14 +25,16 @@
         'Adafruit-PureIO>=1.1.9',
         'Adafruit-ADS1x15>=1.0.2',
         'Adafruit-GPIO>=1.0.3',
         'pi-plates>=7.21',
         'numpy>=1.21',
         'plotly>=5.8.2',
         'jupyter>=1.0.0',
+        'jupyterlab>=3.6.2',
+        'labquest>=1.0.0',
         'notebook>=6.4.12', # security fixes
         'jupyter-contrib-nbextensions>=0.5.1',
         'pandas>=1.4.2',
         'jupyter-pandas-GUI>=0.7.0',
         'JPSLMenus>=0.5.0',
         'JPSLUtils>=0.7.0',
         'AdvancedHTMLParser>=9.0.1'
```

