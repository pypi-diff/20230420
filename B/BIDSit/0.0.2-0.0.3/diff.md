# Comparing `tmp/BIDSit-0.0.2.tar.gz` & `tmp/BIDSit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BIDSit-0.0.2.tar", last modified: Mon Apr 17 23:29:04 2023, max compression
+gzip compressed data, was "BIDSit-0.0.3.tar", last modified: Wed Apr 19 23:01:18 2023, max compression
```

## Comparing `BIDSit-0.0.2.tar` & `BIDSit-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-17 23:29:04.957500 BIDSit-0.0.2/
--rw-r--r--   0 labmanager   (501) staff       (20)     1115 2023-04-17 23:29:04.957118 BIDSit-0.0.2/PKG-INFO
--rw-r--r--   0 labmanager   (501) staff       (20)      664 2023-04-17 23:17:11.000000 BIDSit-0.0.2/README.rst
--rw-r--r--   0 labmanager   (501) staff       (20)       38 2023-04-17 23:29:04.957625 BIDSit-0.0.2/setup.cfg
--rw-r--r--   0 labmanager   (501) staff       (20)     2421 2023-04-17 23:21:54.000000 BIDSit-0.0.2/setup.py
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-17 23:29:04.951182 BIDSit-0.0.2/src/
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-17 23:29:04.954551 BIDSit-0.0.2/src/BIDSit/
--rw-r--r--   0 labmanager   (501) staff       (20)    49238 2023-04-17 23:14:31.000000 BIDSit-0.0.2/src/BIDSit/BIDSit.py
--rw-r--r--   0 labmanager   (501) staff       (20)    21664 2023-04-17 22:02:10.000000 BIDSit-0.0.2/src/BIDSit/Test_script.py
--rw-r--r--   0 labmanager   (501) staff       (20)        1 2023-03-23 19:34:37.000000 BIDSit-0.0.2/src/BIDSit/__init__.py
--rw-r--r--   0 labmanager   (501) staff       (20)      576 2023-04-17 23:27:35.000000 BIDSit-0.0.2/src/BIDSit/version.py
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-17 23:29:04.956516 BIDSit-0.0.2/src/BIDSit.egg-info/
--rw-r--r--   0 labmanager   (501) staff       (20)     1115 2023-04-17 23:29:04.000000 BIDSit-0.0.2/src/BIDSit.egg-info/PKG-INFO
--rw-r--r--   0 labmanager   (501) staff       (20)      280 2023-04-17 23:29:04.000000 BIDSit-0.0.2/src/BIDSit.egg-info/SOURCES.txt
--rw-r--r--   0 labmanager   (501) staff       (20)        1 2023-04-17 23:29:04.000000 BIDSit-0.0.2/src/BIDSit.egg-info/dependency_links.txt
--rw-r--r--   0 labmanager   (501) staff       (20)       39 2023-04-17 23:29:04.000000 BIDSit-0.0.2/src/BIDSit.egg-info/requires.txt
--rw-r--r--   0 labmanager   (501) staff       (20)        7 2023-04-17 23:29:04.000000 BIDSit-0.0.2/src/BIDSit.egg-info/top_level.txt
+drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-19 23:01:18.844223 BIDSit-0.0.3/
+-rw-r--r--   0 labmanager   (501) staff       (20)     1213 2023-04-19 23:01:18.843960 BIDSit-0.0.3/PKG-INFO
+-rw-r--r--   0 labmanager   (501) staff       (20)      762 2023-04-19 23:00:43.000000 BIDSit-0.0.3/README.rst
+-rw-r--r--   0 labmanager   (501) staff       (20)       38 2023-04-19 23:01:18.844320 BIDSit-0.0.3/setup.cfg
+-rw-r--r--   0 labmanager   (501) staff       (20)     2421 2023-04-18 00:01:02.000000 BIDSit-0.0.3/setup.py
+drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-19 23:01:18.838538 BIDSit-0.0.3/src/
+drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-19 23:01:18.841817 BIDSit-0.0.3/src/BIDSit/
+-rw-r--r--   0 labmanager   (501) staff       (20)    21664 2023-04-17 22:02:10.000000 BIDSit-0.0.3/src/BIDSit/Test_script.py
+-rw-r--r--   0 labmanager   (501) staff       (20)        1 2023-03-23 19:34:37.000000 BIDSit-0.0.3/src/BIDSit/__init__.py
+-rw-r--r--   0 labmanager   (501) staff       (20)    49255 2023-04-18 00:00:52.000000 BIDSit-0.0.3/src/BIDSit/go.py
+-rw-r--r--   0 labmanager   (501) staff       (20)      576 2023-04-18 00:01:08.000000 BIDSit-0.0.3/src/BIDSit/version.py
+drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-19 23:01:18.843551 BIDSit-0.0.3/src/BIDSit.egg-info/
+-rw-r--r--   0 labmanager   (501) staff       (20)     1213 2023-04-19 23:01:18.000000 BIDSit-0.0.3/src/BIDSit.egg-info/PKG-INFO
+-rw-r--r--   0 labmanager   (501) staff       (20)      276 2023-04-19 23:01:18.000000 BIDSit-0.0.3/src/BIDSit.egg-info/SOURCES.txt
+-rw-r--r--   0 labmanager   (501) staff       (20)        1 2023-04-19 23:01:18.000000 BIDSit-0.0.3/src/BIDSit.egg-info/dependency_links.txt
+-rw-r--r--   0 labmanager   (501) staff       (20)       39 2023-04-19 23:01:18.000000 BIDSit-0.0.3/src/BIDSit.egg-info/requires.txt
+-rw-r--r--   0 labmanager   (501) staff       (20)        7 2023-04-19 23:01:18.000000 BIDSit-0.0.3/src/BIDSit.egg-info/top_level.txt
```

### Comparing `BIDSit-0.0.2/PKG-INFO` & `BIDSit-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BIDSit
-Version: 0.0.2
+Version: 0.0.3
 Summary: A BIDS conversion tool for fMRI data
 Home-page: https://github.com/jenburrell/BIDSit
 Author: Jen Burrell
 Author-email: jenbur@psych.ubc.ca
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -33,11 +33,8 @@
 	Python3 setup.py install
 	
 
 Dependencies
 ------------
 All of the core dependencies of ``BIDSit`` will be installed by ``pip``.
 
-To install ``BIDSit``, along with all the tools you need to develop
-and run tests run the following in your virtualenv ::
-
-	pip install -e .[dev] 
+``BIDSit`` requires ``dcm2niiX`` to convert the DICOM and PAR/REC files to NIfTI files. ``dcm2niiX`` can be downloaded from as part of MRIcroGL’s graphical interface from https://www.nitrc.org/plugins/mwiki/index.php/dcm2nii:MainPage#Download
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `BIDSit-0.0.2/setup.py` & `BIDSit-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `BIDSit-0.0.2/src/BIDSit/BIDSit.py` & `BIDSit-0.0.3/src/BIDSit/go.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,18 @@
 #    print(user_info)
     
     # - define variables in use - #
     in_dir = user_info['in_dir'] # in_dir is where the input files are
     out_dir = user_info['out_dir'] # out_dir is where the output files will go
     WDIR = in_dir # WDIR is wherever we are working at the time
     user_info['WDIR'] = WDIR
+        
+    if user_info['bids_it']:
+        bids_info = BIDSit_gui(user_info)
+        user_info = {**user_info, **bids_info}
     
     ### --- convert files to NIFTIs --- ###
     if user_info['dcm2niix']:
         WDIR = out_dir
         sub_folders = glob.glob(f"{in_dir}/*/")
         ses_folders = []
         for sub in sub_folders:
@@ -59,18 +63,15 @@
         WDIR = user_info['WDIR']
         
     ### --- sourcedata folder --- ###
     if user_info['copy'] == "Yes":
         copy_it(WDIR, out_dir + "/sourcedata")
     
     ### --- BIDSit --- ###
-    print(user_info)
     if user_info['bids_it']:
-        bids_info = BIDSit_gui(user_info)
-        user_info = {**user_info, **bids_info}
         sub_list = listdir(WDIR)
         for entry in sub_list:
             if user_info['ses'] =='Yes':
                 for file in listdir(os.path.join(WDIR,entry)):
                     if os.path.isdir(os.path.join(WDIR,entry,file)):
                         if entry in sub_list:
                             sub_list = [entry.replace(entry,os.path.join(entry,file))]
```

### Comparing `BIDSit-0.0.2/src/BIDSit/Test_script.py` & `BIDSit-0.0.3/src/BIDSit/Test_script.py`

 * *Files identical despite different names*

### Comparing `BIDSit-0.0.2/src/BIDSit/version.py` & `BIDSit-0.0.3/src/BIDSit/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 # Script Name: version.py                                                    #
 #                                                                            #
 # Description: specifies version for BIDSit                                  #
 #                                                                            #
 # Author:      Jen Burrell (April 17th, 2023)                                #
 #============================================================================#
 
-__version__ = '0.0.2'
+__version__ = '0.0.3'
```

### Comparing `BIDSit-0.0.2/src/BIDSit.egg-info/PKG-INFO` & `BIDSit-0.0.3/src/BIDSit.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BIDSit
-Version: 0.0.2
+Version: 0.0.3
 Summary: A BIDS conversion tool for fMRI data
 Home-page: https://github.com/jenburrell/BIDSit
 Author: Jen Burrell
 Author-email: jenbur@psych.ubc.ca
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -33,11 +33,8 @@
 	Python3 setup.py install
 	
 
 Dependencies
 ------------
 All of the core dependencies of ``BIDSit`` will be installed by ``pip``.
 
-To install ``BIDSit``, along with all the tools you need to develop
-and run tests run the following in your virtualenv ::
-
-	pip install -e .[dev] 
+``BIDSit`` requires ``dcm2niiX`` to convert the DICOM and PAR/REC files to NIfTI files. ``dcm2niiX`` can be downloaded from as part of MRIcroGL’s graphical interface from https://www.nitrc.org/plugins/mwiki/index.php/dcm2nii:MainPage#Download
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

