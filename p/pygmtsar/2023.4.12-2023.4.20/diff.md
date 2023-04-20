# Comparing `tmp/pygmtsar-2023.4.12.tar.gz` & `tmp/pygmtsar-2023.4.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmtsar-2023.4.12.tar", last modified: Thu Apr 13 09:44:23 2023, max compression
+gzip compressed data, was "pygmtsar-2023.4.20.tar", last modified: Thu Apr 20 09:01:06 2023, max compression
```

## Comparing `pygmtsar-2023.4.12.tar` & `pygmtsar-2023.4.20.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2023-04-13 09:44:23.660218 pygmtsar-2023.4.12/
--rw-r--r--   0 mbg        (501) staff       (20)     1563 2023-04-01 05:11:16.000000 pygmtsar-2023.4.12/LICENSE.txt
--rw-r--r--   0 mbg        (501) staff       (20)    10038 2023-04-13 09:44:23.659787 pygmtsar-2023.4.12/PKG-INFO
--rw-r--r--   0 mbg        (501) staff       (20)     9313 2023-03-12 07:12:55.000000 pygmtsar-2023.4.12/README.md
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2023-04-13 09:44:23.656524 pygmtsar-2023.4.12/pygmtsar/
--rwxr-xr-x   0 mbg        (501) staff       (20)    25116 2023-04-09 08:43:45.000000 pygmtsar-2023.4.12/pygmtsar/PRM.py
--rw-r--r--   0 mbg        (501) staff       (20)    21884 2023-03-07 05:42:58.000000 pygmtsar-2023.4.12/pygmtsar/PRM_gmtsar.py
--rwxr-xr-x   0 mbg        (501) staff       (20)    11684 2023-03-30 13:07:17.000000 pygmtsar-2023.4.12/pygmtsar/SBAS.py
--rw-r--r--   0 mbg        (501) staff       (20)    17137 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_base.py
--rw-r--r--   0 mbg        (501) staff       (20)     2161 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_dem.py
--rw-r--r--   0 mbg        (501) staff       (20)     7320 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_dem_gmt_gdal.py
--rw-r--r--   0 mbg        (501) staff       (20)     8780 2023-04-05 05:10:27.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_detrend.py
--rw-r--r--   0 mbg        (501) staff       (20)    12220 2023-04-12 18:26:43.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_geocode.py
--rw-r--r--   0 mbg        (501) staff       (20)     4791 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_incidence.py
--rw-r--r--   0 mbg        (501) staff       (20)     2693 2023-04-12 07:30:31.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_intf.py
--rw-r--r--   0 mbg        (501) staff       (20)     1488 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_landmask.py
--rw-r--r--   0 mbg        (501) staff       (20)     1799 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_landmask_gmt.py
--rw-r--r--   0 mbg        (501) staff       (20)     4993 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_merge.py
--rw-r--r--   0 mbg        (501) staff       (20)      927 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_merge_gmtsar.py
--rw-r--r--   0 mbg        (501) staff       (20)      821 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_orbits.py
--rw-r--r--   0 mbg        (501) staff       (20)     9743 2023-03-07 05:42:58.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_reframe.py
--rw-r--r--   0 mbg        (501) staff       (20)     5518 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_reframe_gmtsar.py
--rw-r--r--   0 mbg        (501) staff       (20)    13303 2023-04-09 14:02:35.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_sbas.py
--rw-r--r--   0 mbg        (501) staff       (20)     5448 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_sbas_gmtsar.py
--rw-r--r--   0 mbg        (501) staff       (20)    10429 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_stack.py
--rw-r--r--   0 mbg        (501) staff       (20)     5630 2023-04-11 17:42:45.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_topo_ra.py
--rw-r--r--   0 mbg        (501) staff       (20)     8644 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_trans.py
--rw-r--r--   0 mbg        (501) staff       (20)     1219 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_unwrap.py
--rw-r--r--   0 mbg        (501) staff       (20)     5856 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_unwrap_snaphu.py
--rw-r--r--   0 mbg        (501) staff       (20)      257 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/__init__.py
--rw-r--r--   0 mbg        (501) staff       (20)    10812 2023-03-31 15:15:54.000000 pygmtsar-2023.4.12/pygmtsar/datagrid.py
--rw-r--r--   0 mbg        (501) staff       (20)     1820 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/tqdm_dask.py
--rw-r--r--   0 mbg        (501) staff       (20)      992 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/tqdm_joblib.py
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2023-04-13 09:44:23.659052 pygmtsar-2023.4.12/pygmtsar.egg-info/
--rw-r--r--   0 mbg        (501) staff       (20)    10038 2023-04-13 09:44:23.000000 pygmtsar-2023.4.12/pygmtsar.egg-info/PKG-INFO
--rw-r--r--   0 mbg        (501) staff       (20)      872 2023-04-13 09:44:23.000000 pygmtsar-2023.4.12/pygmtsar.egg-info/SOURCES.txt
--rw-r--r--   0 mbg        (501) staff       (20)        1 2023-04-13 09:44:23.000000 pygmtsar-2023.4.12/pygmtsar.egg-info/dependency_links.txt
--rw-r--r--   0 mbg        (501) staff       (20)      259 2023-04-13 09:44:23.000000 pygmtsar-2023.4.12/pygmtsar.egg-info/requires.txt
--rw-r--r--   0 mbg        (501) staff       (20)        9 2023-04-13 09:44:23.000000 pygmtsar-2023.4.12/pygmtsar.egg-info/top_level.txt
--rw-r--r--   0 mbg        (501) staff       (20)       38 2023-04-13 09:44:23.660270 pygmtsar-2023.4.12/setup.cfg
--rw-r--r--   0 mbg        (501) staff       (20)     1900 2023-04-12 15:02:17.000000 pygmtsar-2023.4.12/setup.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2023-04-20 09:01:06.898529 pygmtsar-2023.4.20/
+-rw-r--r--   0 mbg        (501) staff       (20)     1563 2023-04-01 05:11:16.000000 pygmtsar-2023.4.20/LICENSE.txt
+-rw-r--r--   0 mbg        (501) staff       (20)    10038 2023-04-20 09:01:06.898343 pygmtsar-2023.4.20/PKG-INFO
+-rw-r--r--   0 mbg        (501) staff       (20)     9313 2023-03-12 07:12:55.000000 pygmtsar-2023.4.20/README.md
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2023-04-20 09:01:06.897275 pygmtsar-2023.4.20/pygmtsar/
+-rwxr-xr-x   0 mbg        (501) staff       (20)    25099 2023-04-16 07:24:33.000000 pygmtsar-2023.4.20/pygmtsar/PRM.py
+-rw-r--r--   0 mbg        (501) staff       (20)    21884 2023-03-07 05:42:58.000000 pygmtsar-2023.4.20/pygmtsar/PRM_gmtsar.py
+-rwxr-xr-x   0 mbg        (501) staff       (20)    11684 2023-03-30 13:07:17.000000 pygmtsar-2023.4.20/pygmtsar/SBAS.py
+-rw-r--r--   0 mbg        (501) staff       (20)    17137 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_base.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2161 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_dem.py
+-rw-r--r--   0 mbg        (501) staff       (20)     7320 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_dem_gmt_gdal.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8780 2023-04-05 05:10:27.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_detrend.py
+-rw-r--r--   0 mbg        (501) staff       (20)    12220 2023-04-12 18:26:43.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_geocode.py
+-rw-r--r--   0 mbg        (501) staff       (20)     4791 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_incidence.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2693 2023-04-12 07:30:31.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_intf.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1488 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_landmask.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1799 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_landmask_gmt.py
+-rw-r--r--   0 mbg        (501) staff       (20)     4993 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_merge.py
+-rw-r--r--   0 mbg        (501) staff       (20)      927 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_merge_gmtsar.py
+-rw-r--r--   0 mbg        (501) staff       (20)      821 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_orbits.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9743 2023-03-07 05:42:58.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_reframe.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5518 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_reframe_gmtsar.py
+-rw-r--r--   0 mbg        (501) staff       (20)    13303 2023-04-09 14:02:35.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_sbas.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5448 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_sbas_gmtsar.py
+-rw-r--r--   0 mbg        (501) staff       (20)    10429 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_stack.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5630 2023-04-11 17:42:45.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_topo_ra.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8644 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_trans.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1824 2023-04-20 05:34:55.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_unwrap.py
+-rw-r--r--   0 mbg        (501) staff       (20)     6045 2023-04-20 05:36:07.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_unwrap_snaphu.py
+-rw-r--r--   0 mbg        (501) staff       (20)      257 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/__init__.py
+-rw-r--r--   0 mbg        (501) staff       (20)    10812 2023-03-31 15:15:54.000000 pygmtsar-2023.4.20/pygmtsar/datagrid.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1820 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/tqdm_dask.py
+-rw-r--r--   0 mbg        (501) staff       (20)      992 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/tqdm_joblib.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2023-04-20 09:01:06.898115 pygmtsar-2023.4.20/pygmtsar.egg-info/
+-rw-r--r--   0 mbg        (501) staff       (20)    10038 2023-04-20 09:01:06.000000 pygmtsar-2023.4.20/pygmtsar.egg-info/PKG-INFO
+-rw-r--r--   0 mbg        (501) staff       (20)      872 2023-04-20 09:01:06.000000 pygmtsar-2023.4.20/pygmtsar.egg-info/SOURCES.txt
+-rw-r--r--   0 mbg        (501) staff       (20)        1 2023-04-20 09:01:06.000000 pygmtsar-2023.4.20/pygmtsar.egg-info/dependency_links.txt
+-rw-r--r--   0 mbg        (501) staff       (20)      259 2023-04-20 09:01:06.000000 pygmtsar-2023.4.20/pygmtsar.egg-info/requires.txt
+-rw-r--r--   0 mbg        (501) staff       (20)        9 2023-04-20 09:01:06.000000 pygmtsar-2023.4.20/pygmtsar.egg-info/top_level.txt
+-rw-r--r--   0 mbg        (501) staff       (20)       38 2023-04-20 09:01:06.898573 pygmtsar-2023.4.20/setup.cfg
+-rw-r--r--   0 mbg        (501) staff       (20)     1900 2023-04-20 09:00:51.000000 pygmtsar-2023.4.20/setup.py
```

### Comparing `pygmtsar-2023.4.12/LICENSE.txt` & `pygmtsar-2023.4.20/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.12/PKG-INFO` & `pygmtsar-2023.4.20/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtsar
-Version: 2023.4.12
+Version: 2023.4.20
 Summary: PyGMTSAR (Python GMTSAR) - Easy and Fast Satellite Interferometry For Everyone
 Home-page: https://github.com/mobigroup/gmtsar
 Author: Alexey Pechnikov
 Author-email: pechnikov@mobigroup.ru
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pygmtsar-2023.4.12/README.md` & `pygmtsar-2023.4.20/README.md`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.12/pygmtsar/PRM.py` & `pygmtsar-2023.4.20/pygmtsar/PRM.py`

 * *Files 1% similar despite different names*

```diff
@@ -389,19 +389,19 @@
             #print ('basename', basename)
 
         # make full file name
         fullname = lambda name: os.path.join(basedir, basename + name)
         gmtsar_sharedir = self.gmtsar_sharedir()
 
         filename_fill_3x3  = os.path.join(gmtsar_sharedir, 'filters', 'fill.3x3')
-        filename_boxcar3x5 = os.path.join(gmtsar_sharedir, 'filters', 'boxcar.3x5')
         filename_gauss5x5  = os.path.join(gmtsar_sharedir, 'filters', 'gauss5x5')
         
         #!conv 1 1 /usr/local/GMTSAR/share/gmtsar/filters/fill.3x3 raw/tmp2.nc raw/corr.nc
         fill_3x3 = np.genfromtxt(filename_fill_3x3, skip_header=1)
+        gauss5x5 = np.genfromtxt(filename_gauss5x5, skip_header=1)
         # gauss_dec inconsistent, see https://github.com/gmtsar/gmtsar/issues/706
         gauss_dec, gauss_string = self.make_gaussian_filter(2, 1, wavelength=wavelength)
         #print (gauss_matrix_astext)
 
         # prepare PRMs for the calculation below
         other.set(self.SAT_baseline(other, tail=9))
         self.set(self.SAT_baseline(self).sel('SC_height','SC_height_start','SC_height_end'))
```

### Comparing `pygmtsar-2023.4.12/pygmtsar/PRM_gmtsar.py` & `pygmtsar-2023.4.20/pygmtsar/PRM_gmtsar.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.12/pygmtsar/SBAS.py` & `pygmtsar-2023.4.20/pygmtsar/SBAS.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.12/pygmtsar/SBAS_base.py` & `pygmtsar-2023.4.20/pygmtsar/SBAS_base.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.12/pygmtsar/SBAS_dem.py` & `pygmtsar-2023.4.20/pygmtsar/SBAS_dem.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.12/pygmtsar/SBAS_dem_gmt_gdal.py` & `pygmtsar-2023.4.20/pygmtsar/SBAS_dem_gmt_gdal.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.12/pygmtsar/SBAS_detrend.py` & `pygmtsar-2023.4.20/pygmtsar/SBAS_detrend.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.12/pygmtsar/SBAS_geocode.py` & `pygmtsar-2023.4.20/pygmtsar/SBAS_geocode.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.12/pygmtsar/SBAS_incidence.py` & `pygmtsar-2023.4.20/pygmtsar/SBAS_incidence.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.12/pygmtsar/SBAS_intf.py` & `pygmtsar-2023.4.20/pygmtsar/SBAS_intf.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.12/pygmtsar/SBAS_landmask.py` & `pygmtsar-2023.4.20/pygmtsar/SBAS_landmask.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.12/pygmtsar/SBAS_landmask_gmt.py` & `pygmtsar-2023.4.20/pygmtsar/SBAS_landmask_gmt.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.12/pygmtsar/SBAS_merge.py` & `pygmtsar-2023.4.20/pygmtsar/SBAS_merge.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.12/pygmtsar/SBAS_merge_gmtsar.py` & `pygmtsar-2023.4.20/pygmtsar/SBAS_merge_gmtsar.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.12/pygmtsar/SBAS_orbits.py` & `pygmtsar-2023.4.20/pygmtsar/SBAS_orbits.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.12/pygmtsar/SBAS_reframe.py` & `pygmtsar-2023.4.20/pygmtsar/SBAS_reframe.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.12/pygmtsar/SBAS_reframe_gmtsar.py` & `pygmtsar-2023.4.20/pygmtsar/SBAS_reframe_gmtsar.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.12/pygmtsar/SBAS_sbas.py` & `pygmtsar-2023.4.20/pygmtsar/SBAS_sbas.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.12/pygmtsar/SBAS_sbas_gmtsar.py` & `pygmtsar-2023.4.20/pygmtsar/SBAS_sbas_gmtsar.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.12/pygmtsar/SBAS_stack.py` & `pygmtsar-2023.4.20/pygmtsar/SBAS_stack.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.12/pygmtsar/SBAS_topo_ra.py` & `pygmtsar-2023.4.20/pygmtsar/SBAS_topo_ra.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.12/pygmtsar/SBAS_trans.py` & `pygmtsar-2023.4.20/pygmtsar/SBAS_trans.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.12/pygmtsar/SBAS_unwrap.py` & `pygmtsar-2023.4.20/pygmtsar/SBAS_unwrap.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,43 @@
 #!/usr/bin/env python3
 # Alexey Pechnikov, Oct, 2022, https://github.com/mobigroup/gmtsar
 from .SBAS_unwrap_snaphu import SBAS_unwrap_snaphu
 
 class SBAS_unwrap(SBAS_unwrap_snaphu):
 
-    def unwrap_parallel(self, pairs=None, n_jobs=-1, **kwargs):
+    def unwrap_parallel(self, pairs=None, mask=None, n_jobs=-1, **kwargs):
+        import xarray as xr
         import pandas as pd
         from tqdm.auto import tqdm
         import joblib
         import os
 
         # for now (Python 3.10.10 on MacOS) joblib loads the code from disk instead of copying it
         kwargs['chunksize'] = self.chunksize
 
-        def unwrap(pair, **kwargs):
+        def unwrap_tiledir(pair, **kwargs):
             # define unique tiledir name for parallel processing
             if 'conf' in kwargs:
                 dirpath = self.get_filenames(None, [pair], 'snaphu_tiledir')[0][:-4]
                 kwargs['conf'] += f'    TILEDIR {dirpath}'
             return self.unwrap(pair, **kwargs)
 
         if pairs is None:
             pairs = self.find_pairs()
         elif isinstance(pairs, pd.DataFrame):
             pairs = pairs.values
 
+        # materialize lazy mask
+        if mask is not None and isinstance(mask, xr.DataArray):
+            mask_filename = self.get_filenames(None, None, 'unwrapmask')
+            if os.path.exists(mask_filename):
+                os.remove(mask_filename)
+            # workaround to save NetCDF file correct
+            mask.rename('mask').rename({'y':'a','x':'r'}).\
+                to_netcdf(mask_filename, encoding={'mask': self.compression(chunksize=self.chunksize)}, engine=self.engine)
+            kwargs['mask'] = 'unwrapmask'
+
+        # save results to NetCDF files
+        kwargs['interactive'] = False
+
         with self.tqdm_joblib(tqdm(desc='Unwrapping', total=len(pairs))) as progress_bar:
-            joblib.Parallel(n_jobs=n_jobs)(joblib.delayed(unwrap)(pair, interactive=False, **kwargs) \
-                                           for pair in pairs)
+            joblib.Parallel(n_jobs=n_jobs)(joblib.delayed(unwrap_tiledir)(pair, **kwargs) for pair in pairs)
```

### Comparing `pygmtsar-2023.4.12/pygmtsar/SBAS_unwrap_snaphu.py` & `pygmtsar-2023.4.20/pygmtsar/SBAS_unwrap_snaphu.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,45 +3,48 @@
 from .SBAS_landmask import SBAS_landmask
 
 class SBAS_unwrap_snaphu(SBAS_landmask):
 
     # -s for SMOOTH mode and -d for DEFO mode when DEFOMAX_CYCLE should be defined in the configuration
     # DEFO mode (-d) and DEFOMAX_CYCLE=0 is equal to SMOOTH mode (-s)
     # https://web.stanford.edu/group/radar/softwareandlinks/sw/snaphu/snaphu_man1.html
-    def unwrap(self, pair, threshold=None, conf=None, func=None, mask=None, conncomp=False,
+    def unwrap(self, pair, threshold=1e-3, conf=None, func=None, mask=None, conncomp=False,
                phase='phasefilt', corr='corr', interactive=True, chunksize=None, debug=False):
         import xarray as xr
         import numpy as np
         import os
         import subprocess
 
         # define lost class variables due to joblib
         if chunksize is None:
             chunksize = self.chunksize
 
-        if threshold is None:
-            # set to very low value but still exclude 0 (masked areas)
-            threshold = 1e-6
-
-        # convert user-defined mask to binary mask (NaN values converted to 0)
-        if mask is not None:
-            assert self.is_ra(mask), 'ERROR: mask should be defined in radar coordinates'
-            # crop mask to minimum extent
-            binmask = self.cropna(xr.where(mask>0, 1, np.nan)).fillna(0).astype(bool)
-        else:
-            binmask = 1
-
         if conf is None:
             conf = self.PRM().snaphu_config()
-
+    
         # open input data grids if needed
         if isinstance(phase, str):
             phase = self.open_grids([pair], phase, chunksize=chunksize, interactive=False)[0]
         if isinstance(corr, str):
             corr = self.open_grids([pair], corr, chunksize=chunksize, interactive=False)[0]
+        if mask is not None and isinstance(mask, str):
+            mask = self.open_grids(None, mask, chunksize=chunksize, interactive=False)
+        
+        # convert user-defined mask to boolean mask (NaN values converted to 0)
+        if mask is not None:
+            assert self.is_ra(mask), 'ERROR: mask should be defined in radar coordinates'
+            # define mask on the same grid as phase and convert to boolean
+            binmask = xr.where(mask>0, 1, 0).astype(bool)
+            # unify grids to maybe smallest mask
+            phase = phase.reindex_like(mask)
+            corr = corr.reindex_like(mask)
+        else:
+            binmask = 1
+        # add threshold mask
+        binmask = binmask & (corr>=threshold)
 
         # extract dates from pair
         date1, date2 = pair
 
         basename = self.get_filenames(None, [pair], '')[0][:-4]
         #print ('basename', basename)
 
@@ -51,35 +54,30 @@
         # SNAPHU input files
         phase_in = basename + 'unwrap.phase'
         corr_in = basename + 'unwrap.corr'
         # SNAPHU output files
         unwrap_out = basename + 'unwrap.out'
         conncomp_out = basename + 'conncomp.out'
 
-        if mask is not None:
-            phase = phase.reindex_like(binmask)
-            corr = corr.reindex_like(binmask)
-
         # cleanup from previous runs
         for tmp_file in [phase_in, corr_in, unwrap_out, conncomp_out] \
                       + [conncomp_filename, unwrap_filename] if not interactive else []:
             #print ('tmp_file', tmp_file)
             if os.path.exists(tmp_file):
                 if debug:
                     print ('DEBUG: remove', tmp_file)
                 os.remove(tmp_file)
 
         # prepare SNAPHU input files
         # NaN values are not allowed for SNAPHU phase input file
-        phasemasked = phase.where(binmask)
-        phasemasked.fillna(0).astype(np.float32).values.tofile(phase_in)
-        # apply threshold and binary mask
-        corrmasked = corr.where(binmask & (corr>=threshold))
+        # interpolate when exist valid values around and fill zero pixels far away from valid ones
+        self.nearest_grid(phase.where(binmask)).fillna(0).astype(np.float32).values.tofile(phase_in)
         # NaN values are not allowed for SNAPHU correlation input file
-        corrmasked.fillna(0).astype(np.float32).values.tofile(corr_in)
+        # just fill NaNs by zeroes because the main trick is phase filling
+        corr.where(binmask).fillna(0).astype(np.float32).values.tofile(corr_in)
 
         # launch SNAPHU binary (NaNs are not allowed for input but returned in output)
         argv = ['snaphu', phase_in, str(phase.shape[1]), '-c', corr_in,
                 '-f', '/dev/stdin', '-o', unwrap_out, '-d']
         if conncomp:
             argv.append('-g')
             argv.append(conncomp_out)
@@ -103,18 +101,18 @@
         # convert to grid unwrapped phase from SNAPHU output applying postprocessing
         values = np.fromfile(unwrap_out, dtype=np.float32).reshape(phase.shape)
         #values = np.frombuffer(stdout_data, dtype=np.float32).reshape(phase.shape)
         unwrap = xr.DataArray(values, phase.coords).chunk(chunksize)
         # apply user-defined function for post-processing
         if func is not None:
             # the both grids should have the right chunksize
-            unwrap = func(corrmasked, unwrap)
+            unwrap = func(corr.where(binmask), unwrap)
         # apply binary mask after the post-processing to completely exclude masked regions
         # NaN values allowed in the output grid, assign userfriendly name for the output grid
-        unwrap = unwrap.where(binmask>0).rename('phase')
+        unwrap = unwrap.where(binmask).rename('phase')
 
         # the output files required for interactive output
         for tmp_file in [phase_in, corr_in] + [unwrap_out, conncomp_out] if not interactive else []:
             if os.path.exists(tmp_file):
                 if debug:
                     print ('DEBUG: remove', tmp_file)
                 os.remove(tmp_file)
```

### Comparing `pygmtsar-2023.4.12/pygmtsar/datagrid.py` & `pygmtsar-2023.4.20/pygmtsar/datagrid.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.12/pygmtsar/tqdm_dask.py` & `pygmtsar-2023.4.20/pygmtsar/tqdm_dask.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.12/pygmtsar/tqdm_joblib.py` & `pygmtsar-2023.4.20/pygmtsar/tqdm_joblib.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.12/pygmtsar.egg-info/PKG-INFO` & `pygmtsar-2023.4.20/pygmtsar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtsar
-Version: 2023.4.12
+Version: 2023.4.20
 Summary: PyGMTSAR (Python GMTSAR) - Easy and Fast Satellite Interferometry For Everyone
 Home-page: https://github.com/mobigroup/gmtsar
 Author: Alexey Pechnikov
 Author-email: pechnikov@mobigroup.ru
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pygmtsar-2023.4.12/pygmtsar.egg-info/SOURCES.txt` & `pygmtsar-2023.4.20/pygmtsar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.12/setup.py` & `pygmtsar-2023.4.20/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='pygmtsar',
-    version='2023.4.12',
+    version='2023.4.20',
     description='PyGMTSAR (Python GMTSAR) - Easy and Fast Satellite Interferometry For Everyone',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/mobigroup/gmtsar',
     author='Alexey Pechnikov',
     author_email='pechnikov@mobigroup.ru',
     license='BSD-3-Clause',
```

