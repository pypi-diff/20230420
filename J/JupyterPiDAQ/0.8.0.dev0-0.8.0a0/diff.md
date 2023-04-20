# Comparing `tmp/JupyterPiDAQ-0.8.0.dev0.tar.gz` & `tmp/JupyterPiDAQ-0.8.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JupyterPiDAQ-0.8.0.dev0.tar", last modified: Wed Apr 19 22:07:45 2023, max compression
+gzip compressed data, was "JupyterPiDAQ-0.8.0a0.tar", last modified: Thu Apr 20 13:35:46 2023, max compression
```

## Comparing `JupyterPiDAQ-0.8.0.dev0.tar` & `JupyterPiDAQ-0.8.0a0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-19 22:07:45.440769 JupyterPiDAQ-0.8.0.dev0/
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-19 22:07:45.435094 JupyterPiDAQ-0.8.0.dev0/JupyterPiDAQ.egg-info/
--rw-r--r--   0 gutow    (60685682) staff       (20)     4679 2023-04-19 22:07:45.000000 JupyterPiDAQ-0.8.0.dev0/JupyterPiDAQ.egg-info/PKG-INFO
--rw-r--r--   0 gutow    (60685682) staff       (20)      856 2023-04-19 22:07:45.000000 JupyterPiDAQ-0.8.0.dev0/JupyterPiDAQ.egg-info/SOURCES.txt
--rw-r--r--   0 gutow    (60685682) staff       (20)        1 2023-04-19 22:07:45.000000 JupyterPiDAQ-0.8.0.dev0/JupyterPiDAQ.egg-info/dependency_links.txt
--rw-r--r--   0 gutow    (60685682) staff       (20)      371 2023-04-19 22:07:45.000000 JupyterPiDAQ-0.8.0.dev0/JupyterPiDAQ.egg-info/requires.txt
--rw-r--r--   0 gutow    (60685682) staff       (20)       19 2023-04-19 22:07:45.000000 JupyterPiDAQ-0.8.0.dev0/JupyterPiDAQ.egg-info/top_level.txt
--rw-r--r--   0 gutow    (60685682) staff       (20)     4679 2023-04-19 22:07:45.440631 JupyterPiDAQ-0.8.0.dev0/PKG-INFO
--rw-r--r--   0 gutow    (60685682) staff       (20)     3972 2023-04-19 19:23:05.000000 JupyterPiDAQ-0.8.0.dev0/README.md
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-19 22:07:45.435363 JupyterPiDAQ-0.8.0.dev0/Tests/
--rw-r--r--   0 gutow    (60685682) staff       (20)        0 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0.dev0/Tests/__init__.py
--rw-r--r--   0 gutow    (60685682) staff       (20)     4894 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0.dev0/Tests/test_boards.py
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-19 22:07:45.437545 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-19 22:07:45.438108 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-19 22:07:45.438762 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/PiGPIO/
--rw-r--r--   0 gutow    (60685682) staff       (20)     8820 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/PiGPIO/ADS1115.py
--rw-r--r--   0 gutow    (60685682) staff       (20)     8053 2023-03-09 20:46:10.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/PiGPIO/DAQC2.py
--rw-r--r--   0 gutow    (60685682) staff       (20)       69 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/PiGPIO/__init__.py
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-19 22:07:45.439214 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/Simulated/
--rw-r--r--   0 gutow    (60685682) staff       (20)     7977 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/Simulated/ADCsim.py
--rw-r--r--   0 gutow    (60685682) staff       (20)     9380 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/Simulated/ADCsim_line.py
--rw-r--r--   0 gutow    (60685682) staff       (20)       55 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/Simulated/__init__.py
--rw-r--r--   0 gutow    (60685682) staff       (20)      131 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/__init__.py
--rw-r--r--   0 gutow    (60685682) staff       (20)     7617 2023-04-08 16:27:02.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/boards.py
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-19 22:07:45.439644 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/vernier/
--rw-r--r--   0 gutow    (60685682) staff       (20)       62 2023-04-08 16:27:02.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/vernier/__init__.py
--rw-r--r--   0 gutow    (60685682) staff       (20)    11240 2023-04-14 15:10:40.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/vernier/labquest.py
--rw-r--r--   0 gutow    (60685682) staff       (20)     9279 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/ChannelSettings.py
--rw-r--r--   0 gutow    (60685682) staff       (20)     4794 2023-04-14 15:10:40.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/DAQProc.py
--rw-r--r--   0 gutow    (60685682) staff       (20)    34634 2023-04-18 17:52:45.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/DAQinstance.py
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-19 22:07:45.440114 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Sensors/
--rw-r--r--   0 gutow    (60685682) staff       (20)       91 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Sensors/__init__.py
--rw-r--r--   0 gutow    (60685682) staff       (20)    27233 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Sensors/sensors.py
--rw-r--r--   0 gutow    (60685682) staff       (20)      243 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/__init__.py
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-19 22:07:45.440301 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/javascript/
--rw-r--r--   0 gutow    (60685682) staff       (20)     4901 2023-04-03 16:01:44.000000 JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/javascript/JupyterPiDAQmnu.js
--rw-r--r--   0 gutow    (60685682) staff       (20)       38 2023-04-19 22:07:45.440826 JupyterPiDAQ-0.8.0.dev0/setup.cfg
--rw-r--r--   0 gutow    (60685682) staff       (20)     1827 2023-04-18 21:52:39.000000 JupyterPiDAQ-0.8.0.dev0/setup.py
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-20 13:35:46.704400 JupyterPiDAQ-0.8.0a0/
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-20 13:35:46.699470 JupyterPiDAQ-0.8.0a0/JupyterPiDAQ.egg-info/
+-rw-r--r--   0 gutow    (60685682) staff       (20)     4666 2023-04-20 13:35:46.000000 JupyterPiDAQ-0.8.0a0/JupyterPiDAQ.egg-info/PKG-INFO
+-rw-r--r--   0 gutow    (60685682) staff       (20)      856 2023-04-20 13:35:46.000000 JupyterPiDAQ-0.8.0a0/JupyterPiDAQ.egg-info/SOURCES.txt
+-rw-r--r--   0 gutow    (60685682) staff       (20)        1 2023-04-20 13:35:46.000000 JupyterPiDAQ-0.8.0a0/JupyterPiDAQ.egg-info/dependency_links.txt
+-rw-r--r--   0 gutow    (60685682) staff       (20)      371 2023-04-20 13:35:46.000000 JupyterPiDAQ-0.8.0a0/JupyterPiDAQ.egg-info/requires.txt
+-rw-r--r--   0 gutow    (60685682) staff       (20)       19 2023-04-20 13:35:46.000000 JupyterPiDAQ-0.8.0a0/JupyterPiDAQ.egg-info/top_level.txt
+-rw-r--r--   0 gutow    (60685682) staff       (20)     4666 2023-04-20 13:35:46.704219 JupyterPiDAQ-0.8.0a0/PKG-INFO
+-rw-r--r--   0 gutow    (60685682) staff       (20)     3972 2023-04-19 19:23:05.000000 JupyterPiDAQ-0.8.0a0/README.md
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-20 13:35:46.699727 JupyterPiDAQ-0.8.0a0/Tests/
+-rw-r--r--   0 gutow    (60685682) staff       (20)        0 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0a0/Tests/__init__.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)     4894 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0a0/Tests/test_boards.py
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-20 13:35:46.701069 JupyterPiDAQ-0.8.0a0/jupyterpidaq/
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-20 13:35:46.701603 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-20 13:35:46.702293 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/PiGPIO/
+-rw-r--r--   0 gutow    (60685682) staff       (20)     8820 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/PiGPIO/ADS1115.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)     8063 2023-04-20 01:16:08.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/PiGPIO/DAQC2.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)       69 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/PiGPIO/__init__.py
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-20 13:35:46.702822 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/Simulated/
+-rw-r--r--   0 gutow    (60685682) staff       (20)     7977 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/Simulated/ADCsim.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)     9380 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/Simulated/ADCsim_line.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)       55 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/Simulated/__init__.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)      131 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/__init__.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)     7617 2023-04-08 16:27:02.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/boards.py
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-20 13:35:46.703185 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/vernier/
+-rw-r--r--   0 gutow    (60685682) staff       (20)       62 2023-04-08 16:27:02.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/vernier/__init__.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)    11392 2023-04-20 01:25:10.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/vernier/labquest.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)     9279 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/ChannelSettings.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)     4794 2023-04-14 15:10:40.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/DAQProc.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)    34634 2023-04-20 01:10:28.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/DAQinstance.py
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-20 13:35:46.703583 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Sensors/
+-rw-r--r--   0 gutow    (60685682) staff       (20)       91 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Sensors/__init__.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)    27233 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Sensors/sensors.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)      243 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/__init__.py
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-20 13:35:46.703790 JupyterPiDAQ-0.8.0a0/jupyterpidaq/javascript/
+-rw-r--r--   0 gutow    (60685682) staff       (20)     4901 2023-04-03 16:01:44.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/javascript/JupyterPiDAQmnu.js
+-rw-r--r--   0 gutow    (60685682) staff       (20)       38 2023-04-20 13:35:46.704443 JupyterPiDAQ-0.8.0a0/setup.cfg
+-rw-r--r--   0 gutow    (60685682) staff       (20)     1815 2023-04-20 13:35:37.000000 JupyterPiDAQ-0.8.0a0/setup.py
```

### Comparing `JupyterPiDAQ-0.8.0.dev0/JupyterPiDAQ.egg-info/PKG-INFO` & `JupyterPiDAQ-0.8.0a0/JupyterPiDAQ.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: JupyterPiDAQ
-Version: 0.8.0.dev0
-Summary: Data Acquisition in Jupyter notebook on Raspberry Pi
+Version: 0.8.0a0
+Summary: Live Data Acquisition in Jupyter notebooks
 Home-page: https://github.com/JupyterPhysSciLab/JupyterPiDAQ
 Author: Jonathan Gutow
 Author-email: gutow@uwosh.edu
 License: GPL-3.0+
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `JupyterPiDAQ-0.8.0.dev0/JupyterPiDAQ.egg-info/SOURCES.txt` & `JupyterPiDAQ-0.8.0a0/JupyterPiDAQ.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JupyterPiDAQ-0.8.0.dev0/PKG-INFO` & `JupyterPiDAQ-0.8.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: JupyterPiDAQ
-Version: 0.8.0.dev0
-Summary: Data Acquisition in Jupyter notebook on Raspberry Pi
+Version: 0.8.0a0
+Summary: Live Data Acquisition in Jupyter notebooks
 Home-page: https://github.com/JupyterPhysSciLab/JupyterPiDAQ
 Author: Jonathan Gutow
 Author-email: gutow@uwosh.edu
 License: GPL-3.0+
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `JupyterPiDAQ-0.8.0.dev0/README.md` & `JupyterPiDAQ-0.8.0a0/README.md`

 * *Files identical despite different names*

### Comparing `JupyterPiDAQ-0.8.0.dev0/Tests/test_boards.py` & `JupyterPiDAQ-0.8.0a0/Tests/test_boards.py`

 * *Files identical despite different names*

### Comparing `JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/PiGPIO/ADS1115.py` & `JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/PiGPIO/ADS1115.py`

 * *Files identical despite different names*

### Comparing `JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/PiGPIO/DAQC2.py` & `JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/PiGPIO/DAQC2.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import numpy as np
 
 import logging
 
 try:
     from piplates import DAQC2plate
 except Exception as e:
-    print("DAQC2plate: "+str(e))
+    print("\nDAQC2plate: "+str(e), end='')
     DAQC2plate = None
 
 from jupyterpidaq.Boards import Board
 
 logger = logging.getLogger(__name__)
 
 # Optimized for Pi 3B+ for an installed ADS1115 ADC PiHAT. This is
```

### Comparing `JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/Simulated/ADCsim.py` & `JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/Simulated/ADCsim.py`

 * *Files identical despite different names*

### Comparing `JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/Simulated/ADCsim_line.py` & `JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/Simulated/ADCsim_line.py`

 * *Files identical despite different names*

### Comparing `JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/boards.py` & `JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/boards.py`

 * *Files identical despite different names*

### Comparing `JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Boards/vernier/labquest.py` & `JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/vernier/labquest.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     import labquest
     labquestdrvs = True
     starttime = Value('d',time.time())
     samples = []
     for k in range(3):
         samples.append(Value('i',0))
 except Exception as e:
-    print("LabQuest: "+str(e))
+    print("\nLabQuest: "+str(e))
     labquestdrvs = False
 
 from jupyterpidaq.Boards import Board
 
 logger = logging.getLogger(__name__)
 
 # Optimized for Pi 3B+ for an installed ADS1115 ADC PiHAT. This is
@@ -35,34 +35,37 @@
     :return: list of LabQuests (Types too?)
     """
     boards = []
     # The following is a hack to get around the fact that the whole module
     # needs to be reinstantiated on the new thread. I think the best option
     # is to upon discovery spawn a process and then just communicate with it.
     if labquestdrvs:
-        LabQuests = labquest.LabQuest()
-        if LabQuests.open() == 0:
-            # Count number of boards
-            nboards = len(labquest.config.hDevice)
-            # Close things
-            LabQuests.close()
-            # launch a process to talk to, need Pipes to communicate.
-            from multiprocessing import Process, Pipe
-            cmdsend, cmdrcv = Pipe()
-            datasend, datarcv = Pipe()
-            LQ = Process(target = LQProc,
-                         args = (cmdrcv, datasend, starttime, samples))
-            LQ.start()
-            # append an object for each board that knows how to talk to the
-            # process and get information from that particular device
-            addr = 0
-            for addr in range(nboards):
-                # TODO what to pass to each Board_LQ
-                boards.append(Board_LQ(addr, cmdsend, datarcv))
-                addr+=1
+        try:
+            LabQuests = labquest.LabQuest()
+            if LabQuests.open() == 0:
+                # Count number of boards
+                nboards = len(labquest.config.hDevice)
+                # Close things
+                LabQuests.close()
+                # launch a process to talk to, need Pipes to communicate.
+                from multiprocessing import Process, Pipe
+                cmdsend, cmdrcv = Pipe()
+                datasend, datarcv = Pipe()
+                LQ = Process(target = LQProc,
+                             args = (cmdrcv, datasend, starttime, samples))
+                LQ.start()
+                # append an object for each board that knows how to talk to the
+                # process and get information from that particular device
+                addr = 0
+                for addr in range(nboards):
+                    boards.append(Board_LQ(addr, cmdsend, datarcv))
+                    addr+=1
+        except Exception as e:
+            print ("\nLabQuest(s) not found.", end='')
+            logger.debug(e)
     return boards
 
 class Board_LQ(Board):
     """
     Class defining the properties of the analog-to-digital block of the
     LabQuests. Key characteristics:
```

### Comparing `JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/ChannelSettings.py` & `JupyterPiDAQ-0.8.0a0/jupyterpidaq/ChannelSettings.py`

 * *Files identical despite different names*

### Comparing `JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/DAQProc.py` & `JupyterPiDAQ-0.8.0a0/jupyterpidaq/DAQProc.py`

 * *Files identical despite different names*

### Comparing `JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/DAQinstance.py` & `JupyterPiDAQ-0.8.0a0/jupyterpidaq/DAQinstance.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import logging
 
 # Start Logging
 import JPSLUtils
 
 logname = 'DAQinstance_' + time.strftime('%y-%m-%d_%H%M%S',
                                          time.localtime()) + '.log'
-logging.basicConfig(filename=logname, level=logging.INFO)
+logging.basicConfig(filename=logname, level=logging.WARN)
 
 # below is equivalent to %matplotlib notebook in a Jupyter cell
 from IPython import get_ipython
 
 ipython = get_ipython()
 print('Importing drivers and searching for available data acquisition '
       'hardware.',end='')
```

### Comparing `JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/Sensors/sensors.py` & `JupyterPiDAQ-0.8.0a0/jupyterpidaq/Sensors/sensors.py`

 * *Files identical despite different names*

### Comparing `JupyterPiDAQ-0.8.0.dev0/jupyterpidaq/javascript/JupyterPiDAQmnu.js` & `JupyterPiDAQ-0.8.0a0/jupyterpidaq/javascript/JupyterPiDAQmnu.js`

 * *Files identical despite different names*

### Comparing `JupyterPiDAQ-0.8.0.dev0/setup.py` & `JupyterPiDAQ-0.8.0a0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="JupyterPiDAQ",
     url = "https://github.com/JupyterPhysSciLab/JupyterPiDAQ",
-    version="0.8.0dev",
-    description="Data Acquisition in Jupyter notebook on Raspberry Pi",
+    version="0.8.0a",
+    description="Live Data Acquisition in Jupyter notebooks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Jonathan Gutow",
     author_email="gutow@uwosh.edu",
     license="GPL-3.0+",
     packages=setuptools.find_packages(exclude=("dist","build","dev_testing",)),
     #package_data={'javascript': ['javascript/*.js']},
```

