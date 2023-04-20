# Comparing `tmp/flashcam-1.4.1.tar.gz` & `tmp/flashcam-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flashcam-1.4.1.tar", last modified: Thu Apr 20 12:20:31 2023, max compression
+gzip compressed data, was "flashcam-1.4.2.tar", last modified: Thu Apr 20 12:49:38 2023, max compression
```

## Comparing `flashcam-1.4.1.tar` & `flashcam-1.4.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-20 12:20:31.694709 flashcam-1.4.1/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      830 2023-04-20 12:20:31.694709 flashcam-1.4.1/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      569 2023-04-17 13:40:53.000000 flashcam-1.4.1/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-20 12:20:31.690709 flashcam-1.4.1/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    24826 2023-04-20 12:20:29.000000 flashcam-1.4.1/bin/flashcam
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2023-04-06 11:29:38.000000 flashcam-1.4.1/bin/flashcam_join
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      311 2023-04-06 11:29:38.000000 flashcam-1.4.1/bin/flashcam_rep
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      551 2023-04-06 11:48:21.000000 flashcam-1.4.1/bin/flashcamg
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-20 12:20:31.690709 flashcam-1.4.1/flashcam/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2023-04-06 11:29:38.000000 flashcam-1.4.1/flashcam/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5255 2023-04-06 11:29:38.000000 flashcam-1.4.1/flashcam/base_camera2.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8079 2023-04-17 13:40:53.000000 flashcam-1.4.1/flashcam/config.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-20 12:20:31.694709 flashcam-1.4.1/flashcam/data/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2023-04-06 11:29:38.000000 flashcam-1.4.1/flashcam/data/BEAM_OFF.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2023-04-06 11:29:38.000000 flashcam-1.4.1/flashcam/data/BEAM_ON_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2023-04-06 11:29:38.000000 flashcam-1.4.1/flashcam/data/DET_NRDY.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2023-04-06 11:29:38.000000 flashcam-1.4.1/flashcam/data/DET_RDY_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-04-06 11:29:38.000000 flashcam-1.4.1/flashcam/data/digital-7.mono.ttf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2023-04-06 11:29:38.000000 flashcam-1.4.1/flashcam/data/monoskop.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    59930 2023-04-20 08:33:53.000000 flashcam-1.4.1/flashcam/data/win_rain.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    91079 2023-04-20 08:33:53.000000 flashcam-1.4.1/flashcam/data/win_skull.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    76270 2023-04-20 08:33:53.000000 flashcam-1.4.1/flashcam/data/win_storm.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    61604 2023-04-20 08:33:53.000000 flashcam-1.4.1/flashcam/data/win_winter.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-04-20 08:33:53.000000 flashcam-1.4.1/flashcam/data/windows.jpg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2023-04-06 11:29:38.000000 flashcam-1.4.1/flashcam/direct.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-04-06 11:29:38.000000 flashcam-1.4.1/flashcam/izmq_receiver.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4178 2023-04-06 11:29:38.000000 flashcam-1.4.1/flashcam/mmapwr.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    44831 2023-04-20 11:58:02.000000 flashcam-1.4.1/flashcam/real_camera.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    35953 2023-04-20 12:14:15.000000 flashcam-1.4.1/flashcam/stream_enhancer.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)   100516 2023-04-06 11:29:38.000000 flashcam-1.4.1/flashcam/uniwrec.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11302 2023-04-06 11:51:33.000000 flashcam-1.4.1/flashcam/usbcheck.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    27417 2023-04-06 11:29:38.000000 flashcam-1.4.1/flashcam/v4lc.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-04-20 12:20:31.000000 flashcam-1.4.1/flashcam/version.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    30138 2023-04-20 08:32:51.000000 flashcam-1.4.1/flashcam/web.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-20 12:20:31.694709 flashcam-1.4.1/flashcam.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      830 2023-04-20 12:20:31.000000 flashcam-1.4.1/flashcam.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      820 2023-04-20 12:20:31.000000 flashcam-1.4.1/flashcam.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-04-20 12:20:31.000000 flashcam-1.4.1/flashcam.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      157 2023-04-20 12:20:31.000000 flashcam-1.4.1/flashcam.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2023-04-20 12:20:31.000000 flashcam-1.4.1/flashcam.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-04-20 12:20:31.694709 flashcam-1.4.1/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2008 2023-04-18 08:31:29.000000 flashcam-1.4.1/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-20 12:49:38.909970 flashcam-1.4.2/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      830 2023-04-20 12:49:38.909970 flashcam-1.4.2/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      569 2023-04-17 13:40:53.000000 flashcam-1.4.2/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-20 12:49:38.905970 flashcam-1.4.2/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    24826 2023-04-20 12:20:29.000000 flashcam-1.4.2/bin/flashcam
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2023-04-06 11:29:38.000000 flashcam-1.4.2/bin/flashcam_join
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      311 2023-04-06 11:29:38.000000 flashcam-1.4.2/bin/flashcam_rep
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      551 2023-04-06 11:48:21.000000 flashcam-1.4.2/bin/flashcamg
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-20 12:49:38.905970 flashcam-1.4.2/flashcam/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2023-04-06 11:29:38.000000 flashcam-1.4.2/flashcam/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5255 2023-04-06 11:29:38.000000 flashcam-1.4.2/flashcam/base_camera2.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8079 2023-04-17 13:40:53.000000 flashcam-1.4.2/flashcam/config.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-20 12:49:38.909970 flashcam-1.4.2/flashcam/data/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2023-04-06 11:29:38.000000 flashcam-1.4.2/flashcam/data/BEAM_OFF.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2023-04-06 11:29:38.000000 flashcam-1.4.2/flashcam/data/BEAM_ON_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2023-04-06 11:29:38.000000 flashcam-1.4.2/flashcam/data/DET_NRDY.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2023-04-06 11:29:38.000000 flashcam-1.4.2/flashcam/data/DET_RDY_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-04-06 11:29:38.000000 flashcam-1.4.2/flashcam/data/digital-7.mono.ttf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2023-04-06 11:29:38.000000 flashcam-1.4.2/flashcam/data/monoskop.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    59930 2023-04-20 08:33:53.000000 flashcam-1.4.2/flashcam/data/win_rain.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    91079 2023-04-20 08:33:53.000000 flashcam-1.4.2/flashcam/data/win_skull.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    76270 2023-04-20 08:33:53.000000 flashcam-1.4.2/flashcam/data/win_storm.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    61604 2023-04-20 08:33:53.000000 flashcam-1.4.2/flashcam/data/win_winter.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-04-20 08:33:53.000000 flashcam-1.4.2/flashcam/data/windows.jpg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2023-04-06 11:29:38.000000 flashcam-1.4.2/flashcam/direct.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-04-06 11:29:38.000000 flashcam-1.4.2/flashcam/izmq_receiver.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4178 2023-04-06 11:29:38.000000 flashcam-1.4.2/flashcam/mmapwr.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    44831 2023-04-20 12:48:48.000000 flashcam-1.4.2/flashcam/real_camera.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    35953 2023-04-20 12:14:15.000000 flashcam-1.4.2/flashcam/stream_enhancer.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)   100516 2023-04-06 11:29:38.000000 flashcam-1.4.2/flashcam/uniwrec.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11302 2023-04-06 11:51:33.000000 flashcam-1.4.2/flashcam/usbcheck.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    27417 2023-04-06 11:29:38.000000 flashcam-1.4.2/flashcam/v4lc.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-04-20 12:49:38.000000 flashcam-1.4.2/flashcam/version.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    30138 2023-04-20 12:48:25.000000 flashcam-1.4.2/flashcam/web.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-20 12:49:38.909970 flashcam-1.4.2/flashcam.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      830 2023-04-20 12:49:38.000000 flashcam-1.4.2/flashcam.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      820 2023-04-20 12:49:38.000000 flashcam-1.4.2/flashcam.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-04-20 12:49:38.000000 flashcam-1.4.2/flashcam.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      157 2023-04-20 12:49:38.000000 flashcam-1.4.2/flashcam.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2023-04-20 12:49:38.000000 flashcam-1.4.2/flashcam.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-04-20 12:49:38.909970 flashcam-1.4.2/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2008 2023-04-18 08:31:29.000000 flashcam-1.4.2/setup.py
```

### Comparing `flashcam-1.4.1/PKG-INFO` & `flashcam-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashcam
-Version: 1.4.1
+Version: 1.4.2
 Summary: Composition of scripts to control a web camera
 Home-page: https://gitlab.com/jaromrax/flashcam
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
```

### Comparing `flashcam-1.4.1/README.md` & `flashcam-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.1/bin/flashcam` & `flashcam-1.4.2/bin/flashcam`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.1/bin/flashcamg` & `flashcam-1.4.2/bin/flashcamg`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.1/flashcam/base_camera2.py` & `flashcam-1.4.2/flashcam/base_camera2.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.1/flashcam/config.py` & `flashcam-1.4.2/flashcam/config.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.1/flashcam/data/BEAM_OFF.jpg` & `flashcam-1.4.2/flashcam/data/BEAM_OFF.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.1/flashcam/data/BEAM_ON_.jpg` & `flashcam-1.4.2/flashcam/data/BEAM_ON_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.1/flashcam/data/DET_NRDY.jpg` & `flashcam-1.4.2/flashcam/data/DET_NRDY.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.1/flashcam/data/DET_RDY_.jpg` & `flashcam-1.4.2/flashcam/data/DET_RDY_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.1/flashcam/data/digital-7.mono.ttf` & `flashcam-1.4.2/flashcam/data/digital-7.mono.ttf`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.1/flashcam/data/monoskop.jpg` & `flashcam-1.4.2/flashcam/data/monoskop.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.1/flashcam/data/win_rain.jpg` & `flashcam-1.4.2/flashcam/data/win_rain.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.1/flashcam/data/win_skull.jpg` & `flashcam-1.4.2/flashcam/data/win_skull.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.1/flashcam/data/win_storm.jpg` & `flashcam-1.4.2/flashcam/data/win_storm.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.1/flashcam/data/win_winter.jpg` & `flashcam-1.4.2/flashcam/data/win_winter.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.1/flashcam/data/windows.jpg` & `flashcam-1.4.2/flashcam/data/windows.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.1/flashcam/direct.py` & `flashcam-1.4.2/flashcam/direct.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.1/flashcam/izmq_receiver.py` & `flashcam-1.4.2/flashcam/izmq_receiver.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.1/flashcam/mmapwr.py` & `flashcam-1.4.2/flashcam/mmapwr.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.1/flashcam/real_camera.py` & `flashcam-1.4.2/flashcam/real_camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,15 +306,15 @@
         #print(config.CONFIG)
         #print( "AVERAGE I AM HAVING ",config.CONFIG['average'] )
         framekind    = config.CONFIG['framekind']
         average      = int(config.CONFIG['average'])
         threshold    = int(config.CONFIG['threshold'])
         blur         = int(config.CONFIG['blur'])
         timelaps     = int(config.CONFIG['laps'])
-        histogram    = config.CONFIG['histogram']
+        histogram    = config.CONFIG['Histogram']
         res          = config.CONFIG['resolution']
         speedx       = float(config.CONFIG['x'])
         speedy       = float(config.CONFIG['y'])
         rotate180    = int(config.CONFIG['otate'])
         zoom         = int(config.CONFIG['zoom'])
 
         MODE_DMbase = "MODE DM"
@@ -442,16 +442,16 @@
 
         # *********  video works,  get capacities and go with EXPO GAIN
         if not( (vidnum is None) or (vidnum == -1) ):
 
             cc = v4lc.V4L2_CTL("/dev/video"+str(vidnum))
             capa = cc.get_capbilities()
 
-            if (config.CONFIG["histogram"]!=None) or \
-               (config.CONFIG["histogram"]==True):
+            if (config.CONFIG["Histogram"]!=None) or \
+               (config.CONFIG["Histogram"]==True):
                     print("i... HISTOGRAM ON ===> MANUAL EGM")
                     set_gem(cc, "def","auto","def") # exp 'def' is different from auto
             else:
                 # I CALL SET_GAM from
                 set_gem(cc, config.CONFIG['gain'],
                         config.CONFIG['expo'],
                         config.CONFIG['mmaga'])
```

### Comparing `flashcam-1.4.1/flashcam/stream_enhancer.py` & `flashcam-1.4.2/flashcam/stream_enhancer.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.1/flashcam/uniwrec.py` & `flashcam-1.4.2/flashcam/uniwrec.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.1/flashcam/usbcheck.py` & `flashcam-1.4.2/flashcam/usbcheck.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.1/flashcam/v4lc.py` & `flashcam-1.4.2/flashcam/v4lc.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.1/flashcam/web.py` & `flashcam-1.4.2/flashcam/web.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     print("XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXx")
     print("XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXx")
     print("XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXx")
     print("XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXx")
     sys.exit(1)
 print("---------------------------------------- LOADED IN WEBPY")
 print(config.CONFIG)
-print(config.CONFIG["histogram"], "==histo in web")
+print(config.CONFIG["Histogram"], "==histo in web")
 # print("------------JUST LOADED---------------")
 
 
 
 
 
 from importlib import import_module
```

### Comparing `flashcam-1.4.1/flashcam.egg-info/PKG-INFO` & `flashcam-1.4.2/flashcam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashcam
-Version: 1.4.1
+Version: 1.4.2
 Summary: Composition of scripts to control a web camera
 Home-page: https://gitlab.com/jaromrax/flashcam
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
```

### Comparing `flashcam-1.4.1/flashcam.egg-info/SOURCES.txt` & `flashcam-1.4.2/flashcam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.1/setup.py` & `flashcam-1.4.2/setup.py`

 * *Files identical despite different names*

