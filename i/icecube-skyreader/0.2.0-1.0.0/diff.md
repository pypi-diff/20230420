# Comparing `tmp/icecube-skyreader-0.2.0.tar.gz` & `tmp/icecube-skyreader-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icecube-skyreader-0.2.0.tar", last modified: Thu Apr 20 19:07:30 2023, max compression
+gzip compressed data, was "icecube-skyreader-1.0.0.tar", last modified: Thu Apr 20 20:21:36 2023, max compression
```

## Comparing `icecube-skyreader-0.2.0.tar` & `icecube-skyreader-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 19:07:30.168347 icecube-skyreader-0.2.0/
--rw-r--r--   0 root         (0) root         (0)     1085 2023-04-20 19:07:26.000000 icecube-skyreader-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1974 2023-04-20 19:07:30.168347 icecube-skyreader-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1025 2023-04-20 19:07:26.000000 icecube-skyreader-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 19:07:30.164347 icecube-skyreader-0.2.0/icecube_skyreader.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1974 2023-04-20 19:07:30.000000 icecube-skyreader-0.2.0/icecube_skyreader.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      389 2023-04-20 19:07:30.000000 icecube-skyreader-0.2.0/icecube_skyreader.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 19:07:30.000000 icecube-skyreader-0.2.0/icecube_skyreader.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      120 2023-04-20 19:07:30.000000 icecube-skyreader-0.2.0/icecube_skyreader.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-20 19:07:30.000000 icecube-skyreader-0.2.0/icecube_skyreader.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1749 2023-04-20 19:07:30.168347 icecube-skyreader-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       76 2023-04-20 19:07:26.000000 icecube-skyreader-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 19:07:30.168347 icecube-skyreader-0.2.0/skyreader/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-20 19:07:27.000000 icecube-skyreader-0.2.0/skyreader/__init__.py
--rw-r--r--   0 root         (0) root         (0)      915 2023-04-20 19:07:26.000000 icecube-skyreader-0.2.0/skyreader/event_metadata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 19:07:30.168347 icecube-skyreader-0.2.0/skyreader/plot/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 19:07:26.000000 icecube-skyreader-0.2.0/skyreader/plot/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9066 2023-04-20 19:07:26.000000 icecube-skyreader-0.2.0/skyreader/plot/plotting_tools.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 19:07:26.000000 icecube-skyreader-0.2.0/skyreader/py.typed
--rw-r--r--   0 root         (0) root         (0)    46927 2023-04-20 19:07:26.000000 icecube-skyreader-0.2.0/skyreader/result.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:21:36.744133 icecube-skyreader-1.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-04-20 20:21:33.000000 icecube-skyreader-1.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1974 2023-04-20 20:21:36.744133 icecube-skyreader-1.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-04-20 20:21:33.000000 icecube-skyreader-1.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:21:36.744133 icecube-skyreader-1.0.0/icecube_skyreader.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1974 2023-04-20 20:21:36.000000 icecube-skyreader-1.0.0/icecube_skyreader.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      389 2023-04-20 20:21:36.000000 icecube-skyreader-1.0.0/icecube_skyreader.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 20:21:36.000000 icecube-skyreader-1.0.0/icecube_skyreader.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      120 2023-04-20 20:21:36.000000 icecube-skyreader-1.0.0/icecube_skyreader.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-20 20:21:36.000000 icecube-skyreader-1.0.0/icecube_skyreader.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1749 2023-04-20 20:21:36.744133 icecube-skyreader-1.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       76 2023-04-20 20:21:33.000000 icecube-skyreader-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:21:36.744133 icecube-skyreader-1.0.0/skyreader/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-20 20:21:34.000000 icecube-skyreader-1.0.0/skyreader/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      915 2023-04-20 20:21:33.000000 icecube-skyreader-1.0.0/skyreader/event_metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:21:36.744133 icecube-skyreader-1.0.0/skyreader/plot/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:21:33.000000 icecube-skyreader-1.0.0/skyreader/plot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9057 2023-04-20 20:21:33.000000 icecube-skyreader-1.0.0/skyreader/plot/plotting_tools.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:21:33.000000 icecube-skyreader-1.0.0/skyreader/py.typed
+-rw-r--r--   0 root         (0) root         (0)    47095 2023-04-20 20:21:33.000000 icecube-skyreader-1.0.0/skyreader/result.py
```

### Comparing `icecube-skyreader-0.2.0/LICENSE` & `icecube-skyreader-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-0.2.0/PKG-INFO` & `icecube-skyreader-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icecube-skyreader
-Version: 0.2.0
+Version: 1.0.0
 Summary: An API for Results Produced by SkyDriver & the Skymap Scanner
 Home-page: https://github.com/icecube/skyreader
 Download-URL: https://pypi.org/project/icecube-skyreader/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/icecube/skyreader/issues
```

### Comparing `icecube-skyreader-0.2.0/README.md` & `icecube-skyreader-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-0.2.0/icecube_skyreader.egg-info/PKG-INFO` & `icecube-skyreader-1.0.0/icecube_skyreader.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icecube-skyreader
-Version: 0.2.0
+Version: 1.0.0
 Summary: An API for Results Produced by SkyDriver & the Skymap Scanner
 Home-page: https://github.com/icecube/skyreader
 Download-URL: https://pypi.org/project/icecube-skyreader/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/icecube/skyreader/issues
```

### Comparing `icecube-skyreader-0.2.0/setup.cfg` & `icecube-skyreader-1.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-0.2.0/skyreader/__init__.py` & `icecube-skyreader-1.0.0/skyreader/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "0.2.0"
+__version__ = "1.0.0"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `icecube-skyreader-0.2.0/skyreader/event_metadata.py` & `icecube-skyreader-1.0.0/skyreader/event_metadata.py`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-0.2.0/skyreader/plot/plotting_tools.py` & `icecube-skyreader-1.0.0/skyreader/plot/plotting_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 def format_fits_header(event_id_tuple, mjd, ra, dec, uncertainty):
     """Prepare some of the relevant event information for a fits file
     header."""
     run_id, event_id, event_type = event_id_tuple
 
     header = [
-        ('RUNID', run_id), 
+        ('RUNID', run_id),
         ('EVENTID', event_id),
         ('SENDER', 'IceCube Collaboration'),
         ('EventMJD', mjd),
         ('I3TYPE', '%s'%event_type,'Alert Type'),
         ('RA', np.round(ra,2),'Degree'),
         ('DEC', np.round(dec,2),'Degree'),
         ('RA_ERR_PLUS', np.round(uncertainty[0][1],2),
@@ -60,15 +60,15 @@
         # location of other, fixed coordinate
         lon_offset = rot[0]+lonra[0] - 0.025*(lonra[1]-lonra[0])
         lat_offset = rot[1]+latra[0] - 0.05*(latra[1]-latra[0])
         # lonlat coordinates for labels
         min_lon = np.round(lon_offset/2.)*2. - 2
         max_lon = lon_offset+lonra[1]-lonra[0] + 2
         lons = np.arange(min_lon, max_lon, 2)
-        
+
         min_lat = np.round(lat_offset/2.)*2. - 2
         max_lat = lat_offset+latra[1]-latra[0] + 2
         lats = np.arange(min_lat, max_lat, 2)
 
         lon_set = []
         for lon in lons:
             if lon > lower_lon and lon < upper_lon:
```

### Comparing `icecube-skyreader-0.2.0/skyreader/result.py` & `icecube-skyreader-1.0.0/skyreader/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-"""For encapsulating the result of an event scan in a single instance."""
+"""For encapsulating the results of an event scan in a single instance."""
 
 # fmt: off
 # pylint: skip-file
 # mypy: ignore-errors
 # flake8: noqa
 
+
 import io
 import itertools as it
 import json
 import logging
 import pickle
 from functools import cached_property
 from pathlib import Path
@@ -46,18 +47,20 @@
     """Raised when a pixel-value is illegal."""
 
 
 ###############################################################################
 # MAIN CLASS
 
 class SkyScanResult:
-    """This class parses stores the relevant numeric result of the scan.
-    Ideally it should serve as the basic data structure for plotting /
-    processing / transmission of the scan result.
+    """This class parses a nsides_dict and stores the relevant numeric result
+    of the scan. Ideally it should serve as the basic data structure for
+    plotting / processing / transmission of the scan result.
 
+    nsides_dict is a dictionary keyed by 'nside' values for which a scan
+    result is available (e.g. 8, 64, 512), see `pixel_classes.NSidesDict`.
     The scan result is a dictionary:
     - i (pixel index, integer) ->
         'frame', 'llh', 'recoLossesInside', 'recoLossesTotal'
 
     The numeric values of interest are 'llh', 'recoLossesInside',
     'recoLossesTotal'. The pixel indices in the input dictionary are in
     general unsorted (python dict are unsorted by design) and are
```

