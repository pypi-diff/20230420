# Comparing `tmp/wasscli-0.1.3.tar.gz` & `tmp/wasscli-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/fibe/projects/wass_1.6/cli/dist/tmp_gwsdv2g/wasscli-0.1.3.tar", last modified: Tue Oct  4 13:22:59 2022, max compression
+gzip compressed data, was "/home/fibe/projects/wass/cli/dist/.tmp-fb06om6g/wasscli-0.1.4.tar", last modified: Thu Apr 20 12:57:56 2023, max compression
```

## Comparing `wasscli-0.1.3.tar` & `wasscli-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2022-10-04 13:22:59.135635 wasscli-0.1.3/
--rw-rw-r--   0 fibe      (1000) fibe      (1000)      811 2022-10-04 13:22:59.135635 wasscli-0.1.3/PKG-INFO
--rw-rw-r--   0 fibe      (1000) fibe      (1000)      317 2022-09-20 14:37:47.000000 wasscli-0.1.3/README.md
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     1075 2022-10-04 12:36:51.000000 wasscli-0.1.3/pyproject.toml
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       38 2022-10-04 13:22:59.135635 wasscli-0.1.3/setup.cfg
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2022-10-04 13:22:59.135635 wasscli-0.1.3/wasscli/
--rw-rw-r--   0 fibe      (1000) fibe      (1000)      710 2022-09-20 14:37:47.000000 wasscli-0.1.3/wasscli/__init__.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)      748 2022-09-20 14:37:47.000000 wasscli-0.1.3/wasscli/__main__.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)    15478 2022-10-04 13:09:33.000000 wasscli-0.1.3/wasscli/wasscli.py
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2022-10-04 13:22:59.135635 wasscli-0.1.3/wasscli.egg-info/
--rw-rw-r--   0 fibe      (1000) fibe      (1000)      811 2022-10-04 13:22:58.000000 wasscli-0.1.3/wasscli.egg-info/PKG-INFO
--rw-rw-r--   0 fibe      (1000) fibe      (1000)      271 2022-10-04 13:22:59.000000 wasscli-0.1.3/wasscli.egg-info/SOURCES.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)        1 2022-10-04 13:22:58.000000 wasscli-0.1.3/wasscli.egg-info/dependency_links.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       49 2022-10-04 13:22:58.000000 wasscli-0.1.3/wasscli.egg-info/entry_points.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       39 2022-10-04 13:22:58.000000 wasscli-0.1.3/wasscli.egg-info/requires.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)        8 2022-10-04 13:22:58.000000 wasscli-0.1.3/wasscli.egg-info/top_level.txt
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2023-04-20 12:57:56.500147 wasscli-0.1.4/
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)      811 2023-04-20 12:57:56.500147 wasscli-0.1.4/PKG-INFO
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)      317 2023-01-12 09:58:42.000000 wasscli-0.1.4/README.md
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     1075 2023-01-12 09:58:42.000000 wasscli-0.1.4/pyproject.toml
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       38 2023-04-20 12:57:56.500147 wasscli-0.1.4/setup.cfg
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2023-04-20 12:57:56.500147 wasscli-0.1.4/wasscli/
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)      710 2023-01-12 09:58:42.000000 wasscli-0.1.4/wasscli/__init__.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)      748 2023-01-12 09:58:42.000000 wasscli-0.1.4/wasscli/__main__.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)    15721 2023-04-20 12:56:19.000000 wasscli-0.1.4/wasscli/wasscli.py
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2023-04-20 12:57:56.500147 wasscli-0.1.4/wasscli.egg-info/
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)      811 2023-04-20 12:57:56.000000 wasscli-0.1.4/wasscli.egg-info/PKG-INFO
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)      271 2023-04-20 12:57:56.000000 wasscli-0.1.4/wasscli.egg-info/SOURCES.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)        1 2023-04-20 12:57:56.000000 wasscli-0.1.4/wasscli.egg-info/dependency_links.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       49 2023-04-20 12:57:56.000000 wasscli-0.1.4/wasscli.egg-info/entry_points.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       39 2023-04-20 12:57:56.000000 wasscli-0.1.4/wasscli.egg-info/requires.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)        8 2023-04-20 12:57:56.000000 wasscli-0.1.4/wasscli.egg-info/top_level.txt
```

### Comparing `wasscli-0.1.3/PKG-INFO` & `wasscli-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wasscli
-Version: 0.1.3
+Version: 0.1.4
 Summary: WASS command line interface
 Author: Filippo Bergamasco
 Author-email: filippo.bergamasco@unive.it
 License: GPL3
 Project-URL: homepage, https://sites.google.com/unive.it/wass
 Project-URL: repository, https://github.com/fbergama/wass/tree/master/cli
 Keywords: WASS,3D,Interpolation
```

### Comparing `wasscli-0.1.3/pyproject.toml` & `wasscli-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wasscli-0.1.3/wasscli/__init__.py` & `wasscli-0.1.4/wasscli/__init__.py`

 * *Files identical despite different names*

### Comparing `wasscli-0.1.3/wasscli/__main__.py` & `wasscli-0.1.4/wasscli/__main__.py`

 * *Files identical despite different names*

### Comparing `wasscli-0.1.3/wasscli/wasscli.py` & `wasscli-0.1.4/wasscli/wasscli.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,21 +20,23 @@
 import colorama
 import subprocess
 import os
 import sys
 import numpy as np
 import glob
 import tqdm
+from time import sleep
+from random import randint
 from tqdm.contrib.concurrent import thread_map
 from PyInquirer import prompt, Separator, Validator, ValidationError
 #from wassgridsurface import wassgridsurface_main
 
 colorama.init()
 
-VERSION = "0.1.3"
+VERSION = "0.1.4"
 
 
 WASS_PIPELINE = {
     "wass_prepare": None,
     "wass_match": None,
     "wass_autocalibrate": None,
     "wass_stereo": None
@@ -287,15 +289,21 @@
     answers = prompt(questions)
 
     with open("output/planes.txt", "w") as fplanes:
 
         while( True ):
             print("Running wass_stereo... please be patient")
 
+
             def _stereo_task( t ):
+                if t<NUM_PARALLEL_PROCESSES:
+                    nsec = t*2
+                    print("Waiting %d secs. to optimize the disk access..."%nsec )
+                    sleep(nsec)
+
                 wdirname = "output/%06d_wd"%t
                 ret = subprocess.run( [WASS_PIPELINE["wass_stereo"],"config/stereo_config.txt", wdirname ], capture_output=True )
                 if ret.returncode != 0:
                     print( colorama.Fore.RED+("ERROR while running wass_stereo on frame %06d ****************"%t)+colorama.Style.RESET_ALL)
                     print(ret.stdout.decode("ascii"))
                     print( colorama.Fore.RED+("*********************************************************************")+colorama.Style.RESET_ALL)
                     return False
```

### Comparing `wasscli-0.1.3/wasscli.egg-info/PKG-INFO` & `wasscli-0.1.4/wasscli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wasscli
-Version: 0.1.3
+Version: 0.1.4
 Summary: WASS command line interface
 Author: Filippo Bergamasco
 Author-email: filippo.bergamasco@unive.it
 License: GPL3
 Project-URL: homepage, https://sites.google.com/unive.it/wass
 Project-URL: repository, https://github.com/fbergama/wass/tree/master/cli
 Keywords: WASS,3D,Interpolation
```

