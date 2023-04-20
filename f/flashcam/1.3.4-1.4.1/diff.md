# Comparing `tmp/flashcam-1.3.4.tar.gz` & `tmp/flashcam-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flashcam-1.3.4.tar", last modified: Wed Mar  1 18:44:42 2023, max compression
+gzip compressed data, was "flashcam-1.4.1.tar", last modified: Thu Apr 20 12:20:31 2023, max compression
```

## Comparing `flashcam-1.3.4.tar` & `flashcam-1.4.1.tar`

### file list

```diff
@@ -1,44 +1,42 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-03-01 18:44:42.243785 flashcam-1.3.4/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    10122 2023-03-01 18:44:42.243785 flashcam-1.3.4/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     7670 2023-03-01 18:44:38.000000 flashcam-1.3.4/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-03-01 18:44:42.239785 flashcam-1.3.4/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    26096 2023-02-15 18:20:42.000000 flashcam-1.3.4/bin/flashcam
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2021-11-06 15:40:40.000000 flashcam-1.3.4/bin/flashcam_join
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      311 2022-01-21 21:23:45.000000 flashcam-1.3.4/bin/flashcam_rep
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      447 2022-06-10 13:50:42.000000 flashcam-1.3.4/bin/flashcamg
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-03-01 18:44:42.239785 flashcam-1.3.4/flashcam/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2021-10-01 16:29:02.000000 flashcam-1.3.4/flashcam/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5255 2022-01-28 21:15:30.000000 flashcam-1.3.4/flashcam/base_camera2.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8079 2023-02-01 13:41:33.000000 flashcam-1.3.4/flashcam/config.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-03-01 18:44:42.243785 flashcam-1.3.4/flashcam/data/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2022-11-16 13:28:21.000000 flashcam-1.3.4/flashcam/data/BEAM_OFF.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2022-11-16 13:28:21.000000 flashcam-1.3.4/flashcam/data/BEAM_ON_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2022-11-16 13:28:21.000000 flashcam-1.3.4/flashcam/data/DET_NRDY.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2022-11-16 13:28:21.000000 flashcam-1.3.4/flashcam/data/DET_RDY_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    88835 2022-11-16 13:28:21.000000 flashcam-1.3.4/flashcam/data/c120.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)   533468 2022-11-16 13:28:21.000000 flashcam-1.3.4/flashcam/data/c270_orig.png
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1697 2022-11-16 13:28:21.000000 flashcam-1.3.4/flashcam/data/cameras.org
--rw-rw-r--   0 ojr       (1000) ojr       (1000)  1024874 2022-11-16 13:28:21.000000 flashcam-1.3.4/flashcam/data/cameras.pdf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1975 2022-11-16 13:28:21.000000 flashcam-1.3.4/flashcam/data/cameras.tex
--rw-rw-r--   0 ojr       (1000) ojr       (1000)   115345 2022-11-16 13:28:21.000000 flashcam-1.3.4/flashcam/data/f100.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    30371 2022-11-16 13:28:21.000000 flashcam-1.3.4/flashcam/data/f100_orig.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2022-11-16 13:28:21.000000 flashcam-1.3.4/flashcam/data/monoskop.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    82499 2022-11-16 13:28:21.000000 flashcam-1.3.4/flashcam/data/vf0770.jpg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2022-04-20 12:50:34.000000 flashcam-1.3.4/flashcam/direct.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-02-06 11:14:13.000000 flashcam-1.3.4/flashcam/izmq_receiver.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4176 2023-03-01 15:27:12.000000 flashcam-1.3.4/flashcam/mmapwr.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    45014 2023-03-01 15:27:12.000000 flashcam-1.3.4/flashcam/real_camera.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    35197 2023-02-14 15:48:37.000000 flashcam-1.3.4/flashcam/stream_enhancer.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    97755 2023-03-01 18:42:49.000000 flashcam-1.3.4/flashcam/uniwrec.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11293 2022-11-16 13:28:21.000000 flashcam-1.3.4/flashcam/usbcheck.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    27417 2022-11-16 13:28:21.000000 flashcam-1.3.4/flashcam/v4lc.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-03-01 18:44:41.000000 flashcam-1.3.4/flashcam/version.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    29797 2023-02-15 17:29:21.000000 flashcam-1.3.4/flashcam/web.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-03-01 18:44:42.239785 flashcam-1.3.4/flashcam.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    10122 2023-03-01 18:44:42.000000 flashcam-1.3.4/flashcam.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      854 2023-03-01 18:44:42.000000 flashcam-1.3.4/flashcam.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-03-01 18:44:42.000000 flashcam-1.3.4/flashcam.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      157 2023-03-01 18:44:42.000000 flashcam-1.3.4/flashcam.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2023-03-01 18:44:42.000000 flashcam-1.3.4/flashcam.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-03-01 18:44:42.243785 flashcam-1.3.4/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1687 2023-03-01 15:27:12.000000 flashcam-1.3.4/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-20 12:20:31.694709 flashcam-1.4.1/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      830 2023-04-20 12:20:31.694709 flashcam-1.4.1/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      569 2023-04-17 13:40:53.000000 flashcam-1.4.1/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-20 12:20:31.690709 flashcam-1.4.1/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    24826 2023-04-20 12:20:29.000000 flashcam-1.4.1/bin/flashcam
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2023-04-06 11:29:38.000000 flashcam-1.4.1/bin/flashcam_join
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      311 2023-04-06 11:29:38.000000 flashcam-1.4.1/bin/flashcam_rep
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      551 2023-04-06 11:48:21.000000 flashcam-1.4.1/bin/flashcamg
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-20 12:20:31.690709 flashcam-1.4.1/flashcam/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2023-04-06 11:29:38.000000 flashcam-1.4.1/flashcam/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5255 2023-04-06 11:29:38.000000 flashcam-1.4.1/flashcam/base_camera2.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8079 2023-04-17 13:40:53.000000 flashcam-1.4.1/flashcam/config.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-20 12:20:31.694709 flashcam-1.4.1/flashcam/data/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2023-04-06 11:29:38.000000 flashcam-1.4.1/flashcam/data/BEAM_OFF.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2023-04-06 11:29:38.000000 flashcam-1.4.1/flashcam/data/BEAM_ON_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2023-04-06 11:29:38.000000 flashcam-1.4.1/flashcam/data/DET_NRDY.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2023-04-06 11:29:38.000000 flashcam-1.4.1/flashcam/data/DET_RDY_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-04-06 11:29:38.000000 flashcam-1.4.1/flashcam/data/digital-7.mono.ttf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2023-04-06 11:29:38.000000 flashcam-1.4.1/flashcam/data/monoskop.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    59930 2023-04-20 08:33:53.000000 flashcam-1.4.1/flashcam/data/win_rain.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    91079 2023-04-20 08:33:53.000000 flashcam-1.4.1/flashcam/data/win_skull.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    76270 2023-04-20 08:33:53.000000 flashcam-1.4.1/flashcam/data/win_storm.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    61604 2023-04-20 08:33:53.000000 flashcam-1.4.1/flashcam/data/win_winter.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-04-20 08:33:53.000000 flashcam-1.4.1/flashcam/data/windows.jpg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2023-04-06 11:29:38.000000 flashcam-1.4.1/flashcam/direct.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-04-06 11:29:38.000000 flashcam-1.4.1/flashcam/izmq_receiver.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4178 2023-04-06 11:29:38.000000 flashcam-1.4.1/flashcam/mmapwr.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    44831 2023-04-20 11:58:02.000000 flashcam-1.4.1/flashcam/real_camera.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    35953 2023-04-20 12:14:15.000000 flashcam-1.4.1/flashcam/stream_enhancer.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)   100516 2023-04-06 11:29:38.000000 flashcam-1.4.1/flashcam/uniwrec.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11302 2023-04-06 11:51:33.000000 flashcam-1.4.1/flashcam/usbcheck.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    27417 2023-04-06 11:29:38.000000 flashcam-1.4.1/flashcam/v4lc.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-04-20 12:20:31.000000 flashcam-1.4.1/flashcam/version.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    30138 2023-04-20 08:32:51.000000 flashcam-1.4.1/flashcam/web.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-20 12:20:31.694709 flashcam-1.4.1/flashcam.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      830 2023-04-20 12:20:31.000000 flashcam-1.4.1/flashcam.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      820 2023-04-20 12:20:31.000000 flashcam-1.4.1/flashcam.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-04-20 12:20:31.000000 flashcam-1.4.1/flashcam.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      157 2023-04-20 12:20:31.000000 flashcam-1.4.1/flashcam.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2023-04-20 12:20:31.000000 flashcam-1.4.1/flashcam.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-04-20 12:20:31.694709 flashcam-1.4.1/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2008 2023-04-18 08:31:29.000000 flashcam-1.4.1/setup.py
```

### Comparing `flashcam-1.3.4/bin/flashcam` & `flashcam-1.4.1/bin/flashcam`

 * *Files 12% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
 import flashcam.config as config
 
 try:
     import flashcam.uniwrec as uniwrec
 except:
     print("X... cannot import uniwrec ... ?problem with pynput and Xserver")
+    print(" ... i go on... anyway")
 
 import os #  for exit
 
 import numpy as np
 
 import datetime as dt
 
@@ -186,14 +187,18 @@
         print("i... cfg path is ok")
 
         xapp_path = get_data_path( "x" )
 
         for i in ["BEAM_OFF.jpg","BEAM_ON_.jpg","DET_NRDY.jpg",
                   "DET_RDY_.jpg","monoskop.jpg",
                   "windows.jpg",
+                  "win_rain.jpg",
+                  "win_skull.jpg",
+                  "win_storm.jpg",
+                  "win_winter.jpg",
                   "digital-7.mono.ttf"]:
             fuln = path+"/"+i
             if not os.path.exists( fuln ):
 
                 app_path = get_data_path( i )
 
                 print(f"i...  copying ... from {app_path} to {fuln}")
@@ -219,39 +224,41 @@
          average = None,
          blur = None,
          laps = None,
          web5000 = None,
          expo = None,
          gain = None,
          mmaga = None,
-         histogram = None,
+         Histogram = None,
          imagezmq = None,
          jtelegram = None,
          kompress = None,
          save = None,
          qpassfile = None,
          otate = None,
          x = None,
          y = None,
          debug = None,
          vof = None, # framekind already taken
          zoom = None,
-         XY = "1x1"
+         XY = "1x1",
+         help = None
 ):
 
-    ''' Main function of the project, alphabetical order
+
+    helptext = """ Main function of the project, alphabetical order
 |    |                                           |    |
 | -a | average  averaging                        |  6 |
 | -b | blur                                      |  7 |
 | -c | command                                   |  2 |
 | -d | debug                                     |  1 |
 | -e | expo ( in v4l )                           | 11 |
 | -f | framekind  target_frame                   |  5 |
 | -g | gain                                      | 12 |
-| -h | histogram (show mean in image)            | 14 |
+| -H | Histogram (show mean in image)            | 14 |
 | -i | imagezmq                                  |    |
 | -j | telegram (no letter free)                 |    |
 | -k | compression of the stream                 | 95 |
 | -l | laps                                      |  9 |
 | -m | gamma                                     | 13 |
 |    |                                           |    |
 | -o | rOtate                                    | 19 |
@@ -264,16 +271,20 @@
 | -v | FOV field of View in degrees              |101 |
 | -w | web5000 ... view flask                    | 10 |
 | -x | speed of translation for astrophotography | 17 |
 | -y | speed of translation for astrophotography | 18 |
 | -z | zoom                                      | 20 |
 |    |       n   u                               |    |
 | -X | XY                                        |    |
-    '''
+| -h | help                                      |    |
+    """
 
+    if help is not None:
+        print(helptext)
+        sys.exit(0)
     print("i... python path",os.path.realpath(sys.executable))
 
     if getattr(sys, 'frozen', False):
         application_path = os.path.dirname(sys.executable)
     elif __file__:
         application_path = os.path.dirname(__file__)
     print("i... application path",application_path)
@@ -305,15 +316,15 @@
     main_defaults["average"] = 0
     main_defaults["blur"] = 0
     main_defaults["laps"] = -1
     main_defaults["web5000"] = False
     main_defaults["expo"] = "auto"
     main_defaults["gain"] = -1
     main_defaults["mmaga"] = -1
-    main_defaults["histogram"] = False
+    main_defaults["Histogram"] = False
     main_defaults["imagezmq"] = None
     main_defaults["jtelegram"] = False
     main_defaults["kompress"] = 95
     main_defaults["save"] = False,  # for UNI
     main_defaults["qpassfile"] = "~/.pycamfw_userpass"
     main_defaults["otate"] = False # for UNI, also for CONFIG, also for show
     main_defaults["x"] = 0
@@ -333,15 +344,15 @@
     main_actual["average"] = average
     main_actual["blur"] = blur
     main_actual["laps"] = laps
     main_actual["web5000"] = web5000
     main_actual["expo"] = expo
     main_actual["gain"] = gain
     main_actual["mmaga"] = mmaga
-    main_actual["histogram"] = histogram
+    main_actual["Histogram"] = Histogram
     main_actual["imagezmq"] = imagezmq
     main_actual["jtelegram"] = jtelegram
     main_actual["kompress"] = kompress
     main_actual["save"] = save  # for UNI
     main_actual["qpassfile"] = qpassfile
     main_actual["otate"] = otate # for UNI, also for CONFIG, also for show
     main_actual["x"] = x
@@ -351,15 +362,15 @@
     main_actual["zoom"]=zoom
 
     main_actual["XY"]=XY
 
     #----- check -- invalids --------------------------------------
     #      except  bool types:  True/False ------------------------
     for k,v in main_actual.items():
-        if ( type(v) == bool) and not(k in ['web5000','histogram','save','otate','debug','jtelegram']):
+        if ( type(v) == bool) and not(k in ['web5000','Histogram','save','otate','debug','jtelegram']):
             print(f"!... missing a value for parameter {k}: ... incorrect suggested value is: {v}")
             sys.exit(1)
 
 
 
     # ----- print nicely AND UPDATE config ---------------------
     for k,v in main_actual.items():
@@ -406,55 +417,14 @@
     if not (cmd in all_commands):
         print(f"X... unknown command {cmd} !! ... ",  all_commands)
         sys.exit(1)
 
 
 
 
-#=====================================================CONFIG UPDATE
-    # saveme = False
-    # # print( "i... USER  bin_fla:", config.CONFIG['user'] )
-    # # if main_defaults["framekind"] is None:
-
-    # if config.CONFIG['target_frame'] != framekind:
-    #     config.CONFIG['target_frame'] = framekind
-    #     saveme = True
-    # if config.CONFIG['threshold']    != threshold:
-    #     config.CONFIG['threshold']    = threshold
-    #     saveme = True
-    # if config.CONFIG['average']      != average:
-    #     config.CONFIG['average']      = average
-    #     saveme = True
-    # if config.CONFIG['blur']         != blur:
-    #     config.CONFIG['blur']         = blur
-    #     saveme = True
-    # if config.CONFIG['timelaps']         != laps:
-    #     config.CONFIG['timelaps']         = laps
-    #     saveme = True
-    # if config.CONFIG['histogram']         != histogram:
-    #     config.CONFIG['histogram']         = histogram
-    #     saveme = True
-    # if config.CONFIG['resolution']         != res:
-    #     config.CONFIG['resolution']         = res
-    #     saveme = True
-    # if config.CONFIG['x']         != x:
-    #     config.CONFIG['x']         = x
-    #     saveme = True
-    # if config.CONFIG['y']         != y:
-    #     config.CONFIG['y']         = y
-    #     saveme = True
-
-    # if config.CONFIG['rotate180']         != otate:
-    #     config.CONFIG['rotate180'] = otate
-    #     saveme = True
-
-    # if product != "":
-    #     config.CONFIG['recommended'] = product
-    #     saveme = True
-#====================== I update the values from CONFIG for now ========
 
 
 
     if cmd == "usage":
         print(''' ... usage:
     flashcam command [options]
 _____________________________________________________
@@ -473,15 +443,15 @@
         -p ... product/ IDPath / jpg   | -p 14.0-usb-0:2:1.0
                                        | -p screenshot.jpg
         -r ... resolution (see getres) | -r 320x240
         -a ... accumulation* : n frames| -a 10
         -b ... blur* : blur the frame  | -b 3
         -t ... threshold for motiondet | -t 100
         -f ... frame kind (direct,delta*,detect*,histo)
-        -h ... show a mean histo value | -h
+        -H ... show a mean histo value | -H
         -l ... save timelaps [seconds] | -l 3600
         -w ... open web (for flask5000)| -w
         -e ... exposure (0-1;auto)     | -e 0.02
         -g ... gain     (0-1; default) | -g 0.1
         -m ... gamma    (0-1;default)  | -m 0.1
         -q ... passfile for UNI        | -q ~/.pycamfw_userpass
         -x ... move image in x ( -y)   | -x 0.01
```

### Comparing `flashcam-1.3.4/flashcam/base_camera2.py` & `flashcam-1.4.1/flashcam/base_camera2.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.3.4/flashcam/config.py` & `flashcam-1.4.1/flashcam/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
           'average':0,
           'blur':0,
           'laps':0,
           'web5000':False,
           'expo':'auto',
           'gain':'def',
           'mmaga':'def',
-          'histogram':False,
+          'Histogram':False,
           'imagezmq':None,
           'jtelegram':False,
           'kompress':98,
           'save':False,
 
           'qpassfile':"~/.pycamfw_userpass",
```

### Comparing `flashcam-1.3.4/flashcam/data/BEAM_OFF.jpg` & `flashcam-1.4.1/flashcam/data/BEAM_OFF.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.3.4/flashcam/data/BEAM_ON_.jpg` & `flashcam-1.4.1/flashcam/data/BEAM_ON_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.3.4/flashcam/data/DET_NRDY.jpg` & `flashcam-1.4.1/flashcam/data/DET_NRDY.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.3.4/flashcam/data/DET_RDY_.jpg` & `flashcam-1.4.1/flashcam/data/DET_RDY_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.3.4/flashcam/data/monoskop.jpg` & `flashcam-1.4.1/flashcam/data/monoskop.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.3.4/flashcam/direct.py` & `flashcam-1.4.1/flashcam/direct.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.3.4/flashcam/izmq_receiver.py` & `flashcam-1.4.1/flashcam/izmq_receiver.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.3.4/flashcam/mmapwr.py` & `flashcam-1.4.1/flashcam/mmapwr.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 
 
 def mmread_n_clear(  filename = MMAPFILE ):
     """
     read and clear  filename
     """
-    print("D... MMRC")
+    # print("D... MMRC")
     if os.path.exists(filename):
         file_size = os.path.getsize( MMAPFILE )
         if int(file_size) != int(MMAPSIZE):
             print(f"! File Size == {file_size}, should be {MMAPSIZE}")
             print(f"! File Size == {file_size}, should be {MMAPSIZE}")
             print(f"! File Size == {file_size}, should be {MMAPSIZE}")
             print(f"! File Size == {file_size}, should be {MMAPSIZE}")
```

### Comparing `flashcam-1.3.4/flashcam/real_camera.py` & `flashcam-1.4.1/flashcam/real_camera.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 
 # -----------------------------------------------------------------
 
 class Camera(BaseCamera):
 
     video_source = 0
     histomean = 50
+    #nfrm = 0 # number frame.... nonono
     capdevice = None # global
 
     @staticmethod
     def init_cam(  ):
         """
         should return videocapture device
         but also sould set Camerare.video_source
@@ -134,18 +135,18 @@
             ret = False
         else:
             print(f"i... frame {BaseCamera.nframes:8d}   ", end="\r" )
             try: #----this catches errors of libjpeg with cv2.CAP_V4L2
                 ret, frame = cap.read()
                 BaseCamera.nframes+=1
                 #wname = f"res {frame.shape[1]}x{frame.shape[0]}"
-                nfrm+=1
+                # nfrm+=1
                 #print(f"D... got frame (frames iter)   ret={ret}  {frame.shape}")
             except Exception as ex:
-                print("D... SOME OTHER EXCEPTION ON RECV...", ex)
+                print("D... SOME OTHER EXCEPTION ON RECV (realc)...", ex)
                 config.CONFIG["camera_on"] = False
        # --- camera probably works ret True
         if not ret:
             time.sleep(0.5)
             config.CONFIG["camera_on"] = False
             print("i... ??? cap didnt go ok, graying... trying to acquire new cap")
             cap = Camera.init_cam( ) # WHAT IS THIS? the same?<= static?
@@ -193,15 +194,15 @@
                 scale_percent = 50
                 width = int(image.shape[1] * scale_percent / 100)
                 height = int(image.shape[0] * scale_percent / 100)
                 # dsize
                 dsize = (width, height)
                 # resize image
                 frame = cv2.resize(image, dsize)
-                time.sleep(0.1) # from 85%cpu to 20% ??????
+                time.sleep(0.3) # from 85%cpu to 20% ??????
                 return "image", frame, cap # repeat cap==image
 
             elif cap.find("clock.jpg")==0:
                 height, width = 480, 640
                 blank_image = np.zeros((height,width,3), np.uint8)
                 blank_image[:,0:width//2] = (20,20,20)      # (B, G, R)
                 blank_image[:,width//2:width] = (25,25,25)
@@ -215,15 +216,15 @@
                 draw = ImageDraw.Draw(img_pil)
                 drtext = dt.datetime.now().strftime("%H:%M:%S.%f")[:-5]
 
                 #draw.text( position,  "国庆节/中秋节 快乐!", font = font, fill = (b, g, r, a))
                 b,g,r,a = 0,255,0,200
                 draw.text( position,  drtext, font = font, fill = (b, g, r, a))
                 frame = np.array(img_pil)
-                time.sleep(0.1) # from 85%cpu to 20%
+                time.sleep(0.3) # from 85%cpu to 20% with 0.1;
                 # cv2.putText(
                 #     blank_image, #numpy array on which text is written
                 #     drtext, #text
                 #     position, #position at which writing has to start
                 #     #cv2.FONT_HERSHEY_SIMPLEX, #font family
                 #     font,
                 #     4, #font size
@@ -236,15 +237,15 @@
                 #print("i... static image mode")
                 capfull = os.path.expanduser( f"~/.config/flashcam/{cap}" )
                 if  os.path.exists(capfull):
                     fullpath_fixed_image =  capfull
                 else:
                     print("X... image doesnt exist", cap, "using monoskop")
 
-                time.sleep(0.1) # from 85%cpu to 20%
+                time.sleep(0.3) # from 85%cpu to 20% with 0.1
                 return "image", cv2.imread( fullpath_fixed_image), cap # repeat cap==image
         else:
             #print("i...  camera mode")
             if cap is None and vidnum is None:
                 print("X... camera not accessible")
                 time.sleep(0.2)
                 return "image",  cv2.imread( fullpath_fixed_image), cap # repeat cap==image
@@ -673,15 +674,15 @@
                     # ------------- COMMANDS COMMING FROM WEB.PY----------------
                     #  expressions
                     # ------------- commands comming from web.py----------------
                     #           -------------- or from seread (fixed_image ...)
                     expression,value = mmread_n_clear( )
 
                     if expression[:5] != "xxxxx":
-                        print(f"i...  *  EXPR: {expression} == {value}")
+                        #print(f"i...  *  EXPR: {expression} == {value}")
                         print(f"i...  *  EXPR: {expression} == {value}")
                         print(f"i...  *  EXPR: {expression} == {value}")
 
                         # -------------------- conversions without eval inf float bool, string
                         if is_int(value):
                             print("i... ",value, 'can be safely converted to an integer.')
                             value = int(float(value)) # 1.0 => int crashes
@@ -703,32 +704,25 @@
                             # eval makes float float and int int
                             #print("o... evaluating")
                             globals()[expression] = value  #was  eval(value)
                             print("i... evaluated")
                         except:
                             print("X... globals expression FAIL",expression,value)
 
+                        # I need a crosscheck here on terminal screen
+                        if expression=="pausedMOTION":
+                            if value is True:
+                                print("===================== DM RUNNING ====================")
+                            if value is False:
+                                print("--------------------- DM on standby -----------------")
+
+                        if expression=="telegram":
+                            print("i... telegram test******************************* value=",value)
+                            senh.telegram_send_image(blocking= False) # it has an internal block (300sec)
 
-                    # THIs - I think - Is for send telegram via web interface
-                    # it is rather DEBUG tool than a real use
-                    # NOT TESTED
-                    #senh.telegram_send_image()
-
-                    # telegramnow = dt.datetime.now()
-                    # if not (send_telegram is None):
-                    #     # telegram
-                    #     if os.path.exists(os.path.expanduser("~/.telegram.token")):
-                    #         if (telegramnow-telegramlast).total_seconds()>10:
-                    #             y = threading.Thread(target=telegram.bot_send, args=("ALERT", f"{send_telegram} {telegramnow.strftime('%a %H:%M:%S')}",frame) )
-                    #             y.start()
-
-                    #             telegramlast=telegramnow
-                    #             send_telegram = None
-                    #     else:
-                    #         print("X... telegram requested, token not found")
 
 
                     if save_background:
                         print("D... HERE I SAVE save_background of mask")
                         print("D... HERE I SAVE save_background of mask")
                         print("D... HERE I SAVE save_background of mask")
                         senh.save_background()
@@ -949,17 +943,17 @@
 
 
 
                     # delayed telegram - preset in DM ========================
 
                     if not(type(senh.telegramtrigger))==bool:
                         if dt.datetime.now()>senh.telegramtrigger:
-                            print("i... telegram time tripped...", senh.telegramtrigger.strftime("%H:%M:%S"), "NOW=",dt.datetime.now().strftime("%H:%M:%S") )
+                            print("i... telegram time tripped the  2s wire:", senh.telegramtrigger.strftime("%H:%M:%S"), "NOW=",dt.datetime.now().strftime("%H:%M:%S") )
                             senh.telegramtrigger = False
-                            senh.telegram_send_image()
+                            senh.telegram_send_image() # it has an internal block (300sec)
 
 
                     # ----  for DetMo ---- work with detect motion----------------
                     #   telegram and imagezmq are active only here
                     if (threshold>0) :
                         # here there was MODE DM.
                         # but with imageZMQ and Telegram ALERT....
```

### Comparing `flashcam-1.3.4/flashcam/stream_enhancer.py` & `flashcam-1.4.1/flashcam/stream_enhancer.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,16 +98,16 @@
 
     zmqrpi_name = socket.gethostname()
     zmqtarget = None #IP is operated from real_camera
     zmqsender = None # object
     zmqlast = dt.datetime.now()
 
     jtelegram = False # connector from real_camera
+    telegram_tripwire = 2 # send 2 sec later after the triger...
     telegramlast = dt.datetime.now()
-    telegramdelay = 2 #  send 2 sec later after the triger...
     telegramtrigger = False ## either BOOL or DATETIME
 
 
     def RC_COLOR(self,row,col):
         if not self.frame_ok: return  # B  G R
         if (row,col) == self.TIME: return (200,0,0)
         if (row,col) == self.MODE: return (0,0,255)
@@ -179,33 +179,39 @@
 
 
 #---------------------------  INSERT FRAME TO THIS OBJECT ----
     def add_frame(self, image):
         # print("D... adding fframe")
         try:
             h,w = image.shape[0],image.shape[1]
+            # I found that monoskop.jpg crashed - was not 640x480
+            if image.shape[0]!=self.resolution[0] or image.shape[1]!=self.resolution[1]:
+                self.frame = cv2.resize(image, (self.resolution[0], self.resolution[1]), interpolation=cv2.INTER_NEAREST)
+
+            else:
+                self.frame = image
             self.frame_ok = True
         except Exception as e:
             print("D... in add frame bad frame")
             self.frame_ok = False
             return False
-        self.frame = image
         self.maxcol=5 # NORMALLY 4
         # self.maxcol=7 # with x y
         self.maxrow=14
         # #if fontScale == 0.5
         #if w==320:
         #    self.maxcol=2
         #    self.maxrow=5
         # #if fontScale is W/640 *0.5
         if w==320:
         #    self.maxcol=2
             self.maxrow=13
 
         if self.first_frame:
+            print( "D... 1st frame len=",len(self.frame) )
             self.averageValue1 = np.float32(self.frame)
             self.first_frame = False
 
 
         return True
 
 
@@ -539,14 +545,15 @@
         # NOT HERE; this is a timelock - only a new seq self.motion_detected = False #  Here the flag is risen
         motion = False
         self.detect_frame = self.frame.copy()
         self.frame_number+= 1
 
         #print( self.delta_frame)
         if not (self.delta_frame is None):
+            # ------------- THIS IS TUNABLE FROM COMMANDLINE/CONFIG
             thresh = cv2.threshold(self.delta_frame, threshold, 255,
                                 cv2.THRESH_BINARY)[1]
             # print(thresh)
             ok = False
             try:
                 noz = cv2.countNonZero(thresh)
                 ok = True
@@ -577,30 +584,32 @@
                     largesta = dearea
                     largest = [c] # cheap trick, one instead of all
 
             # for c in cnts:
             largesta = int(largesta/frame_area*1000)/10 # recode for late
 
             motion = False
-            # -----one in the list  for now.
-            for c in largest:
+            # -----one in the list  for now.... if larger than 0.7 ==> i dont care...
+            for c in largest: # THE LIST OF ONE ELEMENT - TRICK
                 area = cv2.contourArea(c)
                 # print("Largest: {}/{}  ... {:.2f}%".format(area, frame_area, area/frame_area*100) )
                 # rectangl 1% IS FINE. I pUSH to 0.1%
-                if (area/frame_area < 0.001) or (area/frame_area > 0.7): #minarea 0.5%
+                AREA_THR_MIN = 0.001
+                AREA_THR_MAX = 0.7
+                if (area/frame_area < AREA_THR_MIN) or (area/frame_area > AREA_THR_MAX): #minarea 0.5%
                     # go away for any smaller
                     continue
                 (x, y, w, h) = cv2.boundingRect(c)
-                # print(  x, y, w, h , self.text_height)
-
                 cv2.rectangle(self.detect_frame, (x,y),(x+w,y+h),(0,0,255),2)  # BGR
+
                 motion = True
-                area=w*h
+                area=w*h # of the largest box
 
 
+                #  DM conditions in orange :  area/frame % / noz/frame % / cnts
                 dtext = "{:.1f}%/{:.1f}%/{}".format(
                     area/frame_area*100, noz*100/frame_area, len(cnts) )
                 # --- all with detection is done here.... detect and delta frames must exist then
                 self.setbox( f"{dtext}", self.dm ,  target = self.detect_frame )
                 self.setbox( f"{dtext}", self.dm ,  target = self.delta_frame )
                 self.setbox( f"{dtext}", self.dm    )
                 if "self.histo_frame" in locals():
@@ -809,33 +818,33 @@
             print(f"i... zmq was sent to {self.zmqtarget}")
         except:
             print(f"i... zmq NOT sent to {self.zmqtarget}")
             self.zmqsender = None
         return
 
 
-    def telegram_send_image(self):
+    def telegram_send_image(self, blocking = True):
         """
         send telegram from here... be sure:no flooding
         """
         # telegram
         TELEGRAMBLOCK = 300 # seconds
         if self.jtelegram and (os.path.exists(os.path.expanduser("~/.telegram.token"))):
             telegramnow = dt.datetime.now()
             # 5 minutes
             # protection against flooding
-            if (telegramnow-self.telegramlast).total_seconds()>TELEGRAMBLOCK:
+            if blocking==False or  (telegramnow-self.telegramlast).total_seconds()>TELEGRAMBLOCK:
                 print(f"fCAMERA {self.zmqrpi_name} ")
                 print(f"fCAMERA {self.zmqrpi_name} {telegramnow.strftime('%a %H:%M:%S')}")
                 y = threading.Thread(target=telegram.bot_send, args=("ALERT", f"CAMERA {self.zmqrpi_name} {telegramnow.strftime('%a %H:%M:%S')}", self.frame))
                 y.start()
                 print("i.. telegram SENT============")
                 self.telegramlast=telegramnow
             else:
-                print("i.. telegram not allowed due time", (telegramnow-self.telegramlast).total_seconds())
+                print(f"i.. telegram not allowed due to block-time ({TELEGRAMBLOCK} s); now=", (telegramnow-self.telegramlast).total_seconds())
         #else:
         #    print(f"X...  jtele=={self.jtelegram}, token")
         return
 
 
 
 # --------------------------------------------------------save avi ------------
@@ -883,15 +892,15 @@
                 self.aviout = cv2.VideoWriter( filename , fourcc , 25.0, (640,480))
 
             self.aviout.write(self.frame)
             # plan telegram send to future
             # bool means it is not set....
             #
             if self.jtelegram and type(self.telegramtrigger)==bool:
-                self.telegramtrigger = dt.datetime.now()+dt.timedelta(seconds=2)
+                self.telegramtrigger = dt.datetime.now()+dt.timedelta(seconds=self.telegram_tripwire) # TRIPWIRE 2 seconds
                 print("i... telegramtrigger preset to +2 sec.",self.telegramtrigger.strftime("%H:%M:%S"))
             # MOMENT WHEN AVI IS SAVED===========> imagezmq, telegram...
 
 
 
 
             #print(self.zmqsender,self.zmqtarget)
```

### Comparing `flashcam-1.3.4/flashcam/uniwrec.py` & `flashcam-1.4.1/flashcam/uniwrec.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,14 +118,16 @@
        * with remote flashcam server """
 
 
 
 
 
 def rotate_image(image, angle):
+    if angle is None:     return image
+    if abs(angle)<0.1:     return image
     image_center = tuple(np.array(image.shape[1::-1]) / 2)
     # print( "rotate", image_center, angle )
     rot_mat = cv2.getRotationMatrix2D(image_center, angle, 1.0)
     #print(rot_mat)
     result = cv2.warpAffine(image, rot_mat, image.shape[1::-1], flags=cv2.INTER_LINEAR)
     #print("rotated by ", angle)
     return result
@@ -1241,28 +1243,38 @@
                             else:
                                 row.append(wide)
                         # -----
                         # -----
                         row.append(order)
                         row = sorted(row)
                         row = row[::-1]  # revert - we want Big to small
-                        if len(row) <= 4:
+                        # print( "TICKS... max:", row[0]  )
+
+                        base = 10**math.floor( math.log10( row[0]) )
+                        if row[0]/base<4:
+                            base = 10**math.floor( math.log10( row[0]/4) )
+
+                        minors = np.arange( base, row[0], base)
+                        minors = minors[::-1]
+                        #print(minors)
+                        if len(row) <= 2:
                             in0 = row[0] / 2
-                            in1 =  row[0] / 4
-                            in2 = row[0] / 4 *3
-                            in3 = row[0] / 5
-                            #in2 = row[-1]/10
                             row.append(in0)
+                            in1 =  row[0] / 4
                             row.append(in1)
-                            row.append(in2)
-                            # row.append( in2 )
+                        #     in2 = row[0] / 4 *3
+                        #     in3 = row[0] / 5
+                        #     #in2 = row[-1]/10
+                        #     row.append(in2)
+                        #     # row.append( in2 )
                             # print("   > ",row)
-                        return row  # Big to small
+                        return row,minors  # Big to small
+
 
-                    def one_mark(dist=1.7, wide=[1, 2], speed=0):
+                    def one_mark(dist=1.7, wide=[1, 2], speed=0, dispnumb = True):
                         #  wide ...  # Big to small
                         # h,w = frame.shape[0], frame.shape[1]
                         # pixel distance of halfwidth
 
                         # alpha = pixwid * radians_per_pixel2
                         # dist = wide/math.tan( alpha)
                         # I need to calculate 1m
@@ -1289,58 +1301,79 @@
 
                             mY = mY + level * step
 
                             yA, yB = mY, mY
 
                             xA = mX
                             xB = mX + int(pixwid)
+
+                            yC = mY - int(pixwid) # up
+
                             color = (0, 255, 0)  # BGR
                             color = (55, 0, 255)  # BGR same as the red cross
                             colos = (255, 0, 55)  # BGR same as the red cross
                             if level == 0:
-                                # line
+                                # line - horiznotal
                                 cv2.line(
                                     frame,
                                     (int(xA), int(yA)),
                                     (int(xB), int(yB)),
                                     color,
                                     1,
                                 )
-                                cv2.line(
+                                cv2.line( # left
                                     frame,
                                     (int(xA), int(yA)),
                                     (int(2*xA-xB), int(yB)),
-                                    colos,
+                                    color,
                                     1,
                                 )
 
-                                cv2.line( # probably 1st mark
+
+                                cv2.line( # probably central  mark
                                     frame,
                                     (int(xA), int(yA + 8)),
                                     (int(xA), int(yA - 8)),
                                     color,
                                     1,
                                 )
 
-                            # vert bars -
-                            cv2.line(
+                            # vert bars on horiz axis
+                            cv2.line(  # ticks right
                                 frame,
-                                (int(xB), int(yB + 2)),
-                                (int(xB), int(yB - 2)),
+                                (int(xB), int(yB + 3)),
+                                (int(xB), int(yB - 3)),
                                 color,
                                 1,
                             )
-                            cv2.line(
+                            cv2.line( # ticks left
                                 frame,
-                                (int(2*xA-xB), int(yB + 2)),
-                                (int(2*xA-xB), int(yB - 2)),
-                                colos,
+                                (int(2*xA-xB), int(yB + 3)),
+                                (int(2*xA-xB), int(yB - 3)),
+                                color,
                                 1,
                             )
 
+                            if yC>0:
+                                # horz bars on vertic axis
+                                cv2.line( # up
+                                    frame,
+                                    (int(xA), int(yA)),
+                                    (int(xA), int(yC)),
+                                    color,
+                                    1,
+                                )
+                                cv2.line(
+                                    frame,
+                                    (int(xA-3), int(yC )),
+                                    (int(xA+3), int(yC )),
+                                    color,
+                                    1,
+                                )
+
                             unit = "m"
                             # --- check the biggest to set the unit [0] is biggest
                             if wide[0] <= 0.001:
                                 iwide = round(iwide * 1000 * 1000) / 1000
                                 unit = "mm"
                             elif wide[0] <= 0.01:
                                 iwide = round(iwide * 100 * 1000) / 1000
@@ -1370,35 +1403,61 @@
                             if level > 0:
                                 unit = ""  # no unit during the scale
                             unit2 = "m"
 
                             if str(iwide)[:2] == "0.":
                                 iwide = str(iwide)[1:]
 
-                            # width on scale - scale values
-                            cv2.putText(
-                                frame,
-                                f"{iwide}{unit}",
-                                (int(xB - 10), int(mY - 7)),  # little rightx a bit up y
-                                cv2.FONT_HERSHEY_SIMPLEX,
-                                0.35,
-                                color,
-                                1,
-                            )
-                            cv2.putText(
-                                frame,
-                                f"{iwide}{unit}",
-                                (int(2*xA-xB - 10), int(mY - 7)),  # little rightx a bit up y
-                                cv2.FONT_HERSHEY_SIMPLEX,
-                                0.35,
-                                colos,
-                                1,
-                            )
+                            if dispnumb:
+                                # width on scale - scale values
+                                cv2.putText(
+                                    frame,
+                                    f"{iwide}",
+                                    (int(xB - 10), int(mY - 7)),  # little rightx a bit up y
+                                    cv2.FONT_HERSHEY_SIMPLEX,
+                                    0.35,
+                                    color,
+                                    1,
+                                )
+                                cv2.putText(
+                                    frame,
+                                    f"{iwide}",
+                                    (int(2*xA-xB - 10), int(mY - 7)),  # little rightx a bit up y
+                                    cv2.FONT_HERSHEY_SIMPLEX,
+                                    0.35,
+                                    color,
+                                    1,
+                                )
+
+                                cv2.putText(  # up
+                                    frame,
+                                    f"{iwide}{unit}",
+                                    (int(xA + 10), int(yC)),  # little rightx a bit up y
+                                    cv2.FONT_HERSHEY_SIMPLEX,
+                                    0.35,
+                                    color,
+                                    1,
+                                )
+
 
 
+                                if level==0 and unit!="":
+                                    cv2.putText(
+                                        frame,
+                                        f"  unit ... {unit}",
+                                        (
+                                            int(xA - 130),
+                                            int(mY - 5 -40),
+                                        ),  # little rightx a bit up y
+                                        cv2.FONT_HERSHEY_SIMPLEX,
+                                        0.35,
+                                        color,
+                                        1,
+                                    )
+
 
                             if level >= 0:
                                 # distance - only at first mark
                                 cv2.putText(
                                     frame,
                                     f"  at {dist} {unit2}",
                                     (
@@ -1435,15 +1494,18 @@
                                         0.35,
                                         color,
                                         1,
                                     )
                             level += 1
 
                     # main part of the ruler making---------------
-                    order = get_order(dist=measure)
+
+                    order,minorticks = get_order(dist=measure)
+                    # print(minorticks)
+
                     # speed computation
                     if not (tracker1 is None) and len(tracker_list) > 2:
                         b = tracker_list[-1]
                         try:
                             v_from = -2
                             a = tracker_list[v_from]
                             while True:
@@ -1460,14 +1522,15 @@
                         c = ((b[0] - a[0]) ** 2 + (b[1] - a[1]) ** 2) ** 0.5
                         v = c / dt * radians_per_pixel2
                         v = round(100 * math.tan(v) * measure) / 100
                         # print(f"i... speed = {v} m/s  {dt:.2}==dt " )
                     else:
                         v = 0
                     # plot ruler
+                    one_mark(dist=measure, wide=minorticks, speed=v, dispnumb = False)
                     one_mark(dist=measure, wide=order, speed=v)
 
                     # ----------- THERE IS A MISTAKE countdown_s not known here
                 #                 if "countdown" in locals() and len(countdown) > 0:
                 #                     now = datetime.datetime.now()
                 #                     delta = now - datetime.datetime(1970, 1, 1)
                 #                     if delta < countdown_s:
@@ -1760,15 +1823,15 @@
                     (measure > 0)
                     and (frame is not None)
                     and (rpi_name != "")
                     and (key == ord("N"))
                 ):
                     print("N PRESSED! - measure distance - far")
                     measure_prev_tmp = measure
-                    measure = round(10 * measure / 1.15) / 10
+                    measure = round(10 * measure / 1.2) / 10
                     if measure_prev_tmp == measure:
                         measure = measure/2
                     if measure < 0.1:
                         measure = 0.1
 
                 if (
                     (measure > 0)
```

### Comparing `flashcam-1.3.4/flashcam/usbcheck.py` & `flashcam-1.4.1/flashcam/usbcheck.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
                 #wname = f"res {frame.shape[1]}x{frame.shape[0]}"
                 nfrm+=1
                 print("D... got frame",nfrm, "ret=", ret)
     #        except TimeoutError:
     #            timeoutok = True
     #            nfrm = 0
             except Exception as ex:
-                print("D... SOME OTHER EXCEPTION ON RECV...", ex)
+                print("D... SOME OTHER EXCEPTION ON RECV (usbchk)...", ex)
 
 #        if  timeoutok:
 #            print("X... timout")
 
         if not ret:
             time.sleep(0.5)
             print("D... trying to recommend")
```

### Comparing `flashcam-1.3.4/flashcam/v4lc.py` & `flashcam-1.4.1/flashcam/v4lc.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.3.4/flashcam/web.py` & `flashcam-1.4.1/flashcam/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -503,23 +503,23 @@
             if request.form.get('left2') == 'LEFT2':
                 print("<-")
                 if (pantilthat.get_pan()+8)<=90:
                     pantilthat.pan( pantilthat.get_pan()+8 )
 
         if  request.form.get('external_signal') is not None:
             excommand = str( request.form.get('external_signal') )
-            print(f"**** external signal == {excommand} *****")
-            print(f"**** external signal == {excommand} *****")
-            print(f"**** external signal == {excommand} *****")
+            #print(f"**** external signal == {excommand} *****")
+            #print(f"**** external signal == {excommand} *****")
+            #print(f"**** external signal == {excommand} *****")
             print(f"**** external signal == {excommand} *****")
             if excommand == "pausedmON":
-                print("i... unpause   - Detect Motion")
+                print("i... unpause   - Detect Motion         unpause   - Detect Motion ")
                 mmwrite(f"pausedMOTION False" )
             if excommand == "pausedmOF":
-                print("i... pause - NO Detect Motion NOW")
+                print("i... pause - NO Detect Motion              pause - NO Detect Motion")
                 mmwrite(f"pausedMOTION True" )
 
 
         if  request.form.get('crosson') == 'CROSSON':
             print("green cross ON")
             cross_on = True
         elif  request.form.get('crossoff') == 'CROSSOFF':
@@ -546,20 +546,25 @@
 
         #---------------- I am blindly adding functionality ... compression now
         if  request.form.get('kompress') == 'KOMPRESS':
             print("kompress asked  ....... ")
             #kompressvalue = request.form.get('kompressvalue')
             if config.CONFIG['kompress']>90:
                 config.CONFIG['kompress'] = 9
-                print("KOMPRESS", config.CONFIG['kompress'] )
+                print("i... KOMPRESS", config.CONFIG['kompress'] )
             else:
                 config.CONFIG['kompress'] = 99
-                print("KOMPRESS", config.CONFIG['kompress'] )
+                print("i... KOMPRESS", config.CONFIG['kompress'] )
                 #mmwrite(f"zoom 2" ) # not here...
 
+        #---------------- TELEGRAM TEST
+        if  request.form.get('telegram') == 'TELEGRAM':
+            print("i...  telegram asked  ....... ")
+            mmwrite(f"telegram TELEGRAM" )
+
 
         # .... save cross x and y inside a file at ~/.config/flashcam/
         with open(crocfg,"w") as f:
             f.write(f"{cross_dx} {cross_dy}")
 
     remote_ip=request.environ.get('HTTP_X_REAL_IP', request.remote_addr)
     logthis( " / remote      = "+request.remote_addr )
@@ -569,16 +574,21 @@
     url_fg = url_for('foreground')
     #time.sleep(0.5)
     return render_template_string(index_page, url=url, url_bg  = url_bg, url_fg  = url_fg)
 
 
 
 
+
+
+
 @auth.verify_password
 def verify_password(username, password):
+    global remote_ip
+    remote_ip=request.environ.get('HTTP_X_REAL_IP', request.remote_addr)
 #    user = User.query.filter_by(username = username).first()
 #    if not user or not user.verify_password(password):
 #        return False
 #    g.user = user
     # config.load_config() # IMPLIES THAT ALL changes in 'bin flask500' are lost
     # config.show_config()
     u = config.CONFIG["user"]
@@ -589,20 +599,19 @@
     #     with open( os.path.expanduser("~/.pycamfw_pass") ) as f:
     #         print("YES---> FILE  ","~/.pycamfw_pass")
     #         p=f.readlines()[0].strip()
     # except:
     #     print("NO FILE  ","~/.pycamfw_pass")
 
     if (username==u) and (password==p):
-        logthis( "   TRUE  checking userpass (client)"+username+"/"+password+"/")
-        logthis( "   TRUE  checking userpass (real  )"+u+"/"+p+"/")
+        # logthis( "   TRUE  checking userpass (client)"+username+"/"+password+"/")
+        logthis( f" TRUE  PASS {request.remote_addr:15s} {remote_ip:15s}: /{u}/{p}/")
         return True
     else:
-        logthis( "   FALSE checking userpass (client)"+username+"/"+password+"/")
-        logthis( "   FALSE checking userpass (real  )"+u+"/"+p+"/")
+        logthis( f" FALSE PASS {request.remote_addr:15s} {remote_ip:15s}: /{username}/{password}/")
         return False
 
 
 
 
 @app.route('/')
 @auth.login_required
```

### Comparing `flashcam-1.3.4/flashcam.egg-info/SOURCES.txt` & `flashcam-1.4.1/flashcam.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -22,16 +22,14 @@
 flashcam.egg-info/dependency_links.txt
 flashcam.egg-info/requires.txt
 flashcam.egg-info/top_level.txt
 flashcam/data/BEAM_OFF.jpg
 flashcam/data/BEAM_ON_.jpg
 flashcam/data/DET_NRDY.jpg
 flashcam/data/DET_RDY_.jpg
-flashcam/data/c120.jpg
-flashcam/data/c270_orig.png
-flashcam/data/cameras.org
-flashcam/data/cameras.pdf
-flashcam/data/cameras.tex
-flashcam/data/f100.jpg
-flashcam/data/f100_orig.jpg
+flashcam/data/digital-7.mono.ttf
 flashcam/data/monoskop.jpg
-flashcam/data/vf0770.jpg
+flashcam/data/win_rain.jpg
+flashcam/data/win_skull.jpg
+flashcam/data/win_storm.jpg
+flashcam/data/win_winter.jpg
+flashcam/data/windows.jpg
```

