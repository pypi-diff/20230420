# Comparing `tmp/ltool-1.7.3.tar.gz` & `tmp/ltool-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ltool-1.7.3.tar", last modified: Tue Jan 24 12:48:09 2023, max compression
+gzip compressed data, was "dist/ltool-1.7.4.tar", last modified: Thu Apr 20 08:15:35 2023, max compression
```

## Comparing `ltool-1.7.3.tar` & `ltool-1.7.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 nsiomos   (1022) scc       (1000)        0 2023-01-24 12:48:09.000000 ltool-1.7.3/
--rw-r--r--   0 nsiomos   (1022) scc       (1000)      420 2023-01-24 12:48:09.000000 ltool-1.7.3/PKG-INFO
--rwxr-xr-x   0 nsiomos   (1022) scc       (1000)     1070 2022-01-18 11:00:42.000000 ltool-1.7.3/README.md
-drwxr-xr-x   0 nsiomos   (1022) scc       (1000)        0 2023-01-24 12:48:09.000000 ltool-1.7.3/ltool/
--rwxr-xr-x   0 nsiomos   (1022) scc       (1000)       58 2022-01-18 11:00:42.000000 ltool-1.7.3/ltool/__init__.py
--rwxr-xr-x   0 nsiomos   (1022) scc       (1000)     8770 2022-05-11 14:55:12.000000 ltool-1.7.3/ltool/__main__.py
-drwxr-xr-x   0 nsiomos   (1022) scc       (1000)        0 2023-01-24 12:48:09.000000 ltool-1.7.3/ltool/debug/
--rwxr-xr-x   0 nsiomos   (1022) scc       (1000)       23 2022-01-18 11:00:42.000000 ltool-1.7.3/ltool/debug/__init__.py
--rwxr-xr-x   0 nsiomos   (1022) scc       (1000)     1883 2022-01-18 11:00:42.000000 ltool-1.7.3/ltool/debug/log_pack.py
--rwxr-xr-x   0 nsiomos   (1022) scc       (1000)     3324 2022-01-18 11:00:42.000000 ltool-1.7.3/ltool/debug/plot.py
-drwxr-xr-x   0 nsiomos   (1022) scc       (1000)        0 2023-01-24 12:48:09.000000 ltool-1.7.3/ltool/export/
--rw-r--r--   0 nsiomos   (1022) scc       (1000)       41 2022-01-18 11:00:42.000000 ltool-1.7.3/ltool/export/__init__.py
--rwxr-xr-x   0 nsiomos   (1022) scc       (1000)     5787 2022-02-15 09:34:04.000000 ltool-1.7.3/ltool/export/export_nc.py
--rwxr-xr-x   0 nsiomos   (1022) scc       (1000)     2039 2022-01-18 11:00:42.000000 ltool-1.7.3/ltool/export/update_scc_db.py
-drwxr-xr-x   0 nsiomos   (1022) scc       (1000)        0 2023-01-24 12:48:09.000000 ltool-1.7.3/ltool/readers/
--rw-r--r--   0 nsiomos   (1022) scc       (1000)       68 2022-01-18 11:00:42.000000 ltool-1.7.3/ltool/readers/__init__.py
--rwxr-xr-x   0 nsiomos   (1022) scc       (1000)     2050 2022-01-18 11:00:42.000000 ltool-1.7.3/ltool/readers/get_files.py
--rwxr-xr-x   0 nsiomos   (1022) scc       (1000)      727 2022-01-18 11:00:42.000000 ltool-1.7.3/ltool/readers/parse_config.py
--rwxr-xr-x   0 nsiomos   (1022) scc       (1000)     1533 2022-01-18 11:00:42.000000 ltool-1.7.3/ltool/readers/read_config.py
--rwxr-xr-x   0 nsiomos   (1022) scc       (1000)     2872 2022-05-11 11:25:27.000000 ltool-1.7.3/ltool/readers/read_scc_db.py
-drwxr-xr-x   0 nsiomos   (1022) scc       (1000)        0 2023-01-24 12:48:09.000000 ltool-1.7.3/ltool/tools/
--rw-r--r--   0 nsiomos   (1022) scc       (1000)       34 2022-01-18 11:00:42.000000 ltool-1.7.3/ltool/tools/__init__.py
--rwxr-xr-x   0 nsiomos   (1022) scc       (1000)    12414 2022-05-11 14:55:25.000000 ltool-1.7.3/ltool/tools/geom_dtf.py
--rwxr-xr-x   0 nsiomos   (1022) scc       (1000)     1032 2022-01-18 11:00:42.000000 ltool-1.7.3/ltool/tools/wavelet.py
--rwxr-xr-x   0 nsiomos   (1022) scc       (1000)       22 2023-01-24 12:36:19.000000 ltool-1.7.3/ltool/version.py
-drwxr-xr-x   0 nsiomos   (1022) scc       (1000)        0 2023-01-24 12:48:09.000000 ltool-1.7.3/ltool.egg-info/
--rw-r--r--   0 nsiomos   (1022) scc       (1000)      420 2023-01-24 12:48:08.000000 ltool-1.7.3/ltool.egg-info/PKG-INFO
--rw-r--r--   0 nsiomos   (1022) scc       (1000)      608 2023-01-24 12:48:09.000000 ltool-1.7.3/ltool.egg-info/SOURCES.txt
--rw-r--r--   0 nsiomos   (1022) scc       (1000)        1 2023-01-24 12:48:08.000000 ltool-1.7.3/ltool.egg-info/dependency_links.txt
--rw-r--r--   0 nsiomos   (1022) scc       (1000)       47 2023-01-24 12:48:08.000000 ltool-1.7.3/ltool.egg-info/entry_points.txt
--rw-r--r--   0 nsiomos   (1022) scc       (1000)       37 2023-01-24 12:48:08.000000 ltool-1.7.3/ltool.egg-info/requires.txt
--rw-r--r--   0 nsiomos   (1022) scc       (1000)        6 2023-01-24 12:48:08.000000 ltool-1.7.3/ltool.egg-info/top_level.txt
--rw-r--r--   0 nsiomos   (1022) scc       (1000)       38 2023-01-24 12:48:09.000000 ltool-1.7.3/setup.cfg
--rwxr-xr-x   0 nsiomos   (1022) scc       (1000)     1249 2022-01-18 11:00:42.000000 ltool-1.7.3/setup.py
+drwxr-xr-x   0 nsiomos   (1022) scc       (1000)        0 2023-04-20 08:15:35.000000 ltool-1.7.4/
+-rw-r--r--   0 nsiomos   (1022) scc       (1000)      420 2023-04-20 08:15:35.000000 ltool-1.7.4/PKG-INFO
+-rwxr-xr-x   0 nsiomos   (1022) scc       (1000)     1070 2022-01-18 11:00:42.000000 ltool-1.7.4/README.md
+drwxr-xr-x   0 nsiomos   (1022) scc       (1000)        0 2023-04-20 08:15:35.000000 ltool-1.7.4/ltool/
+-rwxr-xr-x   0 nsiomos   (1022) scc       (1000)       58 2022-01-18 11:00:42.000000 ltool-1.7.4/ltool/__init__.py
+-rwxr-xr-x   0 nsiomos   (1022) scc       (1000)    11071 2023-01-27 09:59:23.000000 ltool-1.7.4/ltool/__main__.py
+drwxr-xr-x   0 nsiomos   (1022) scc       (1000)        0 2023-04-20 08:15:35.000000 ltool-1.7.4/ltool/debug/
+-rwxr-xr-x   0 nsiomos   (1022) scc       (1000)       23 2022-01-18 11:00:42.000000 ltool-1.7.4/ltool/debug/__init__.py
+-rwxr-xr-x   0 nsiomos   (1022) scc       (1000)     1883 2022-01-18 11:00:42.000000 ltool-1.7.4/ltool/debug/log_pack.py
+-rwxr-xr-x   0 nsiomos   (1022) scc       (1000)     3324 2022-01-18 11:00:42.000000 ltool-1.7.4/ltool/debug/plot.py
+drwxr-xr-x   0 nsiomos   (1022) scc       (1000)        0 2023-04-20 08:15:35.000000 ltool-1.7.4/ltool/export/
+-rw-r--r--   0 nsiomos   (1022) scc       (1000)       41 2022-01-18 11:00:42.000000 ltool-1.7.4/ltool/export/__init__.py
+-rwxr-xr-x   0 nsiomos   (1022) scc       (1000)     5787 2022-02-15 09:34:04.000000 ltool-1.7.4/ltool/export/export_nc.py
+-rwxr-xr-x   0 nsiomos   (1022) scc       (1000)     3238 2023-01-26 10:45:40.000000 ltool-1.7.4/ltool/export/update_scc_db.py
+drwxr-xr-x   0 nsiomos   (1022) scc       (1000)        0 2023-04-20 08:15:35.000000 ltool-1.7.4/ltool/readers/
+-rw-r--r--   0 nsiomos   (1022) scc       (1000)       68 2022-01-18 11:00:42.000000 ltool-1.7.4/ltool/readers/__init__.py
+-rwxr-xr-x   0 nsiomos   (1022) scc       (1000)     2056 2023-01-26 10:18:38.000000 ltool-1.7.4/ltool/readers/get_files.py
+-rwxr-xr-x   0 nsiomos   (1022) scc       (1000)      727 2022-01-18 11:00:42.000000 ltool-1.7.4/ltool/readers/parse_config.py
+-rwxr-xr-x   0 nsiomos   (1022) scc       (1000)     1778 2023-01-26 09:28:25.000000 ltool-1.7.4/ltool/readers/read_config.py
+-rwxr-xr-x   0 nsiomos   (1022) scc       (1000)     2452 2023-01-26 10:34:45.000000 ltool-1.7.4/ltool/readers/read_scc_db.py
+drwxr-xr-x   0 nsiomos   (1022) scc       (1000)        0 2023-04-20 08:15:35.000000 ltool-1.7.4/ltool/tools/
+-rw-r--r--   0 nsiomos   (1022) scc       (1000)       34 2022-01-18 11:00:42.000000 ltool-1.7.4/ltool/tools/__init__.py
+-rwxr-xr-x   0 nsiomos   (1022) scc       (1000)    12414 2022-05-11 14:55:25.000000 ltool-1.7.4/ltool/tools/geom_dtf.py
+-rwxr-xr-x   0 nsiomos   (1022) scc       (1000)     1032 2022-01-18 11:00:42.000000 ltool-1.7.4/ltool/tools/wavelet.py
+-rwxr-xr-x   0 nsiomos   (1022) scc       (1000)       22 2023-04-20 08:05:56.000000 ltool-1.7.4/ltool/version.py
+drwxr-xr-x   0 nsiomos   (1022) scc       (1000)        0 2023-04-20 08:15:35.000000 ltool-1.7.4/ltool.egg-info/
+-rw-r--r--   0 nsiomos   (1022) scc       (1000)      420 2023-04-20 08:15:35.000000 ltool-1.7.4/ltool.egg-info/PKG-INFO
+-rw-r--r--   0 nsiomos   (1022) scc       (1000)      608 2023-04-20 08:15:35.000000 ltool-1.7.4/ltool.egg-info/SOURCES.txt
+-rw-r--r--   0 nsiomos   (1022) scc       (1000)        1 2023-04-20 08:15:35.000000 ltool-1.7.4/ltool.egg-info/dependency_links.txt
+-rw-r--r--   0 nsiomos   (1022) scc       (1000)       47 2023-04-20 08:15:35.000000 ltool-1.7.4/ltool.egg-info/entry_points.txt
+-rw-r--r--   0 nsiomos   (1022) scc       (1000)       37 2023-04-20 08:15:35.000000 ltool-1.7.4/ltool.egg-info/requires.txt
+-rw-r--r--   0 nsiomos   (1022) scc       (1000)        6 2023-04-20 08:15:35.000000 ltool-1.7.4/ltool.egg-info/top_level.txt
+-rw-r--r--   0 nsiomos   (1022) scc       (1000)       38 2023-04-20 08:15:35.000000 ltool-1.7.4/setup.cfg
+-rwxr-xr-x   0 nsiomos   (1022) scc       (1000)     1249 2022-01-18 11:00:42.000000 ltool-1.7.4/setup.py
```

### Comparing `ltool-1.7.3/README.md` & `ltool-1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `ltool-1.7.3/ltool/debug/log_pack.py` & `ltool-1.7.4/ltool/debug/log_pack.py`

 * *Files identical despite different names*

### Comparing `ltool-1.7.3/ltool/debug/plot.py` & `ltool-1.7.4/ltool/debug/plot.py`

 * *Files identical despite different names*

### Comparing `ltool-1.7.3/ltool/export/export_nc.py` & `ltool-1.7.4/ltool/export/export_nc.py`

 * *Files identical despite different names*

### Comparing `ltool-1.7.3/ltool/readers/get_files.py` & `ltool-1.7.4/ltool/readers/get_files.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,9 +54,9 @@
 
     wct_peak_margin[wct_peak_margin == None] = 1.
     
     ids = np.array([x[0] for x in query], dtype = str)
     typ = np.array([x[1] for x in query], dtype = str)
     
     mydb.close()
-        
-    return(files, rpath, alphas,snr_factor, wct_peak_margin, typ, ids)
+            
+    return(files, rpath, alphas, snr_factor, wct_peak_margin, typ, ids)
```

### Comparing `ltool-1.7.3/ltool/readers/parse_config.py` & `ltool-1.7.4/ltool/readers/parse_config.py`

 * *Files identical despite different names*

### Comparing `ltool-1.7.3/ltool/readers/read_config.py` & `ltool-1.7.4/ltool/readers/read_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 @author: P. Paschou
 """
 import configparser
-import re
+import re, os
 import numpy as np
 
 class config():
     """
     Holds all the configurable variables
     
     Fields
@@ -17,33 +17,35 @@
     """
     
     def __init__(self, path):
         """Reads the config file at the given path"""
         
         parser = configparser.ConfigParser()
         parser.read(path)
+        if os.path.exists(path) == False:
+            raise AssertionError(' The configuration file does not exist')
 
 #Database   
         if parser.has_section('database'):
             self.dtb = parser._sections['database']
             for key in self.dtb.keys():
                 self.dtb[key] = read_var(self.dtb[key], str)
             
         else:
-            self.dtb = []
+            raise AssertionError(' The configuration file is missing a database section')
 
 # SCC 
         
         if parser.has_section('scc'):
             self.scc = parser._sections['scc']
             for key in self.scc.keys():
                 self.scc[key] = read_var(self.scc[key], str)
             
         else:
-            self.scc = []
+            raise AssertionError(' The configuration file is missing an scc section')
         
 
 # -------- END OF CLASS
 
 def read_dictionary_with_dtype(d, keys, func):
     return {
         key: func(value)
```

### Comparing `ltool-1.7.3/ltool/readers/read_scc_db.py` & `ltool-1.7.4/ltool/readers/read_scc_db.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,70 +10,69 @@
 import logging
 from dateutil.parser import parse 
 from datetime import datetime
 from netCDF4 import Dataset
 
 logger = logging.getLogger(__name__)
 
-def read_scc_db(fpath, end_fill):
+def read_scc_db(path):
 
-    prod_arr = []
-    prod_err_arr = []
-    alt_arr = []
-    alt_b_arr = []
-    dt_start_arr = []
-    metadata = []
-    wave = []
-    for i in range(len(fpath)):
-        path = fpath[i]
-
-        base = os.path.basename(path)
-        
-        logger.info(f"       Reading file: {base} ")
-        
-        fh = Dataset(path, mode='r')
-        temp_meta = fh.__dict__
-        temp_meta['title'] = 'Geometrical properties of aerosol layers'
+    base = os.path.basename(path)
+    
+    logger.info(f"       Reading file: {base} ")
+    
+    fh = Dataset(path, mode='r')
+    metadata = fh.__dict__
+    metadata['title'] = 'Geometrical properties of aerosol layers'
+    metadata['input_file'] = base
+    
+    # Dates
+    start_m = parse(fh.measurement_start_datetime)
+    dt_start = datetime(start_m.year, start_m.month, start_m.day, 
+                        start_m.hour, start_m.minute, start_m.second)
+    
+    # Profiles
+    alt = np.round(fh.variables['altitude'][:].data/1000., decimals = 5)
+    prod = fh.variables['backscatter'][0, 0, :].data
+    rh = (fh.variables['backscatter_calibration_range'][0,1] + fh.variables['backscatter_calibration_range'][0,0])/2.
+    prod_err = fh.variables['error_backscatter'][0, 0, :].data
+    
+    # Wavelength
+    wave = str(int(fh.variables['wavelength'][0].data))
+
+    return(dt_start, alt, prod, prod_err, metadata, wave, rh)
+
+def check_arrays(alt, prod, prod_err):
+    
+    if (len(prod[prod == prod]) <= 10) or (len(alt[prod > 0.]) <= 10) \
+        or (len(alt[prod_err > 0.]) <= 10):
+        
+        raise Exception()
+    
+    return()
+
+def trim_arrays(alt, prod, prod_err, rh):
+
+    step = np.round(np.nanmin(alt[1:] - alt[:-1]), decimals = 5)
+        
+    # Nans above the reference height and where prod =  9.96920997e+36              
+    mask = (alt < rh) & (prod >= 0.) & (prod < 1)
+    
+    prod = prod[mask]
+    prod_err = prod_err[mask]
+    alt = alt[mask]  
+
+    alt_b = alt[0]
+
+    return(alt, prod, prod_err, alt_b, step)
+
+def interp_arrays(alt, prod, prod_err, step, end_fill):
+                  
+    # Interpolate intermediate nans and also keep nan above half wavelet step above end
+    alt_n = np.round(np.arange(alt[0] - end_fill, alt[-1] + end_fill, step), decimals = 5)
+    prod_n = np.interp(alt_n, np.hstack((alt[0] - end_fill, alt, alt[-1] + end_fill)),
+                       np.hstack((prod[0], prod, prod[-1])))
+    prod_err_n = np.interp(alt_n, np.hstack((alt[0] - end_fill, alt, alt[-1] + end_fill)),
+                           np.hstack((prod_err[0], prod_err, prod_err[-1])))  
         
-        # Dates
-        start_m = parse(fh.measurement_start_datetime)
-        dt_start = datetime(start_m.year, start_m.month, start_m.day, 
-                            start_m.hour, start_m.minute, start_m.second)
-        
-        # Profiles
-        alt = np.round(fh.variables['altitude'][:].data/1000., decimals = 5)
-        prod = fh.variables['backscatter'][0, 0, :].data
-        rh = (fh.variables['backscatter_calibration_range'][0,1] + fh.variables['backscatter_calibration_range'][0,0])/2.
-        prod_err = fh.variables['error_backscatter'][0, 0, :].data
-
+    return(alt_n, prod_n, prod_err_n)
         
-        # Nans above the reference height and where prod =  9.96920997e+36              
-        step = np.round(alt[1] - alt[0], decimals = 5)
-        mask = (alt < rh) & (prod >= 0.) & (prod < 1)
-        
-        # Wavelength
-        wave.append(str(int(fh.variables['wavelength'][0].data)))
-        
-        prod = prod[mask]
-        prod_err = prod_err[mask]
-        alt = alt[mask]                
-        
-        if (len(alt) > 0) & (len(prod) > 0):
-            # Interpolate intermediate nans and also keep nan above half wavelet step above end
-            alt_b = alt[0]
-            alt_n = np.round(np.arange(alt[0] - end_fill[i], alt[-1] + end_fill[i], step), decimals = 5)
-            prod_n = np.interp(alt_n, np.hstack((alt[0] - end_fill[i], alt, alt[-1] + end_fill[i])),
-                               np.hstack((prod[0], prod, prod[-1])))
-            prod_err_n = np.interp(alt_n, np.hstack((alt[0] - end_fill[i], alt, alt[-1] + end_fill[i])),
-                                   np.hstack((prod_err[0], prod_err, prod_err[-1])))  
-            
-            # Append to lists
-            if (len(prod[prod == prod]) > 10) & (len(alt[prod > 0.]) > 10):
-                dt_start_arr.append(dt_start)
-                alt_b_arr.append(alt_b)
-                alt_arr.append(alt_n)
-                prod_arr.append(prod_n)
-                prod_err_arr.append(prod_err_n)
-                temp_meta['input_file'] = base
-                metadata.append(temp_meta)
-
-    return(dt_start_arr, alt_b_arr, alt_arr, prod_arr, prod_err_arr, metadata, wave)
```

### Comparing `ltool-1.7.3/ltool/tools/geom_dtf.py` & `ltool-1.7.4/ltool/tools/geom_dtf.py`

 * *Files identical despite different names*

### Comparing `ltool-1.7.3/ltool/tools/wavelet.py` & `ltool-1.7.4/ltool/tools/wavelet.py`

 * *Files identical despite different names*

### Comparing `ltool-1.7.3/ltool.egg-info/SOURCES.txt` & `ltool-1.7.4/ltool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ltool-1.7.3/setup.py` & `ltool-1.7.4/setup.py`

 * *Files identical despite different names*

