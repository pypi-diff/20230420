# Comparing `tmp/icecube-skyreader-0.1.1.tar.gz` & `tmp/icecube-skyreader-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icecube-skyreader-0.1.1.tar", last modified: Tue Apr 18 19:48:50 2023, max compression
+gzip compressed data, was "icecube-skyreader-0.2.0.tar", last modified: Thu Apr 20 19:07:30 2023, max compression
```

## Comparing `icecube-skyreader-0.1.1.tar` & `icecube-skyreader-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 19:48:50.556802 icecube-skyreader-0.1.1/
--rw-r--r--   0 root         (0) root         (0)     1085 2023-04-18 19:48:47.000000 icecube-skyreader-0.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1974 2023-04-18 19:48:50.556802 icecube-skyreader-0.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1025 2023-04-18 19:48:47.000000 icecube-skyreader-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 19:48:50.552802 icecube-skyreader-0.1.1/icecube_skyreader.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1974 2023-04-18 19:48:50.000000 icecube-skyreader-0.1.1/icecube_skyreader.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      389 2023-04-18 19:48:50.000000 icecube-skyreader-0.1.1/icecube_skyreader.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 19:48:50.000000 icecube-skyreader-0.1.1/icecube_skyreader.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      120 2023-04-18 19:48:50.000000 icecube-skyreader-0.1.1/icecube_skyreader.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-18 19:48:50.000000 icecube-skyreader-0.1.1/icecube_skyreader.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1749 2023-04-18 19:48:50.556802 icecube-skyreader-0.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       76 2023-04-18 19:48:47.000000 icecube-skyreader-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 19:48:50.552802 icecube-skyreader-0.1.1/skyreader/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-18 19:48:48.000000 icecube-skyreader-0.1.1/skyreader/__init__.py
--rw-r--r--   0 root         (0) root         (0)      915 2023-04-18 19:48:47.000000 icecube-skyreader-0.1.1/skyreader/event_metadata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 19:48:50.556802 icecube-skyreader-0.1.1/skyreader/plot/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 19:48:47.000000 icecube-skyreader-0.1.1/skyreader/plot/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9066 2023-04-18 19:48:47.000000 icecube-skyreader-0.1.1/skyreader/plot/plotting_tools.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 19:48:47.000000 icecube-skyreader-0.1.1/skyreader/py.typed
--rw-r--r--   0 root         (0) root         (0)    47132 2023-04-18 19:48:47.000000 icecube-skyreader-0.1.1/skyreader/result.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 19:07:30.168347 icecube-skyreader-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-04-20 19:07:26.000000 icecube-skyreader-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1974 2023-04-20 19:07:30.168347 icecube-skyreader-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-04-20 19:07:26.000000 icecube-skyreader-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 19:07:30.164347 icecube-skyreader-0.2.0/icecube_skyreader.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1974 2023-04-20 19:07:30.000000 icecube-skyreader-0.2.0/icecube_skyreader.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      389 2023-04-20 19:07:30.000000 icecube-skyreader-0.2.0/icecube_skyreader.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 19:07:30.000000 icecube-skyreader-0.2.0/icecube_skyreader.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      120 2023-04-20 19:07:30.000000 icecube-skyreader-0.2.0/icecube_skyreader.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-20 19:07:30.000000 icecube-skyreader-0.2.0/icecube_skyreader.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1749 2023-04-20 19:07:30.168347 icecube-skyreader-0.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       76 2023-04-20 19:07:26.000000 icecube-skyreader-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 19:07:30.168347 icecube-skyreader-0.2.0/skyreader/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-20 19:07:27.000000 icecube-skyreader-0.2.0/skyreader/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      915 2023-04-20 19:07:26.000000 icecube-skyreader-0.2.0/skyreader/event_metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 19:07:30.168347 icecube-skyreader-0.2.0/skyreader/plot/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 19:07:26.000000 icecube-skyreader-0.2.0/skyreader/plot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9066 2023-04-20 19:07:26.000000 icecube-skyreader-0.2.0/skyreader/plot/plotting_tools.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 19:07:26.000000 icecube-skyreader-0.2.0/skyreader/py.typed
+-rw-r--r--   0 root         (0) root         (0)    46927 2023-04-20 19:07:26.000000 icecube-skyreader-0.2.0/skyreader/result.py
```

### Comparing `icecube-skyreader-0.1.1/LICENSE` & `icecube-skyreader-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-0.1.1/PKG-INFO` & `icecube-skyreader-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icecube-skyreader
-Version: 0.1.1
+Version: 0.2.0
 Summary: An API for Results Produced by SkyDriver & the Skymap Scanner
 Home-page: https://github.com/icecube/skyreader
 Download-URL: https://pypi.org/project/icecube-skyreader/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/icecube/skyreader/issues
```

### Comparing `icecube-skyreader-0.1.1/README.md` & `icecube-skyreader-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-0.1.1/icecube_skyreader.egg-info/PKG-INFO` & `icecube-skyreader-0.2.0/icecube_skyreader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icecube-skyreader
-Version: 0.1.1
+Version: 0.2.0
 Summary: An API for Results Produced by SkyDriver & the Skymap Scanner
 Home-page: https://github.com/icecube/skyreader
 Download-URL: https://pypi.org/project/icecube-skyreader/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/icecube/skyreader/issues
```

### Comparing `icecube-skyreader-0.1.1/setup.cfg` & `icecube-skyreader-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-0.1.1/skyreader/__init__.py` & `icecube-skyreader-0.2.0/skyreader/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "0.1.1"
+__version__ = "0.2.0"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `icecube-skyreader-0.1.1/skyreader/event_metadata.py` & `icecube-skyreader-0.2.0/skyreader/event_metadata.py`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-0.1.1/skyreader/plot/plotting_tools.py` & `icecube-skyreader-0.2.0/skyreader/plot/plotting_tools.py`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-0.1.1/skyreader/result.py` & `icecube-skyreader-0.2.0/skyreader/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""For encapsulating an event scan result (via Skymap Scanner) in an object."""
-
+"""For encapsulating the result of an event scan in a single instance."""
 
 # fmt: off
 # pylint: skip-file
 # mypy: ignore-errors
 # flake8: noqa
 
 import io
@@ -25,16 +24,14 @@
 from matplotlib import text
 
 from .event_metadata import EventMetadata
 
 ###############################################################################
 # DATA TYPES
 
-PixelTuple = Tuple[int, float, float, float]
-
 
 class PyDictNSidePixels(TypedDict):
     columns: List[str]
     metadata: Dict[str, Any]
     data: List[List[Union[int, float]]]
 
 
@@ -49,20 +46,18 @@
     """Raised when a pixel-value is illegal."""
 
 
 ###############################################################################
 # MAIN CLASS
 
 class SkyScanResult:
-    """This class parses a nsides_dict and stores the relevant numeric result
-    of the scan. Ideally it should serve as the basic data structure for
-    plotting / processing / transmission of the scan result.
+    """This class parses stores the relevant numeric result of the scan.
+    Ideally it should serve as the basic data structure for plotting /
+    processing / transmission of the scan result.
 
-    nsides_dict is a dictionary keyed by 'nside' values for which a scan
-    result is available (e.g. 8, 64, 512), see `pixel_classes.NSidesDict`.
     The scan result is a dictionary:
     - i (pixel index, integer) ->
         'frame', 'llh', 'recoLossesInside', 'recoLossesTotal'
 
     The numeric values of interest are 'llh', 'recoLossesInside',
     'recoLossesTotal'. The pixel indices in the input dictionary are in
     general unsorted (python dict are unsorted by design) and are
@@ -1157,38 +1152,38 @@
                     Phi[j] = RA
                 Theta[bins] = Theta[0]
                 Phi[bins] = Phi[0]
                 return Theta, Phi
 
             # dist = angular_distance(minRA, minDec, extra_ra * np.pi/180., extra_dec * np.pi/180.)
             # print("Millipede best fit is", dist /(np.pi * extra_radius/(1.177 * 180.)), "sigma from reported best fit")
-
+        
 
             extra_ra_rad = np.radians(extra_ra)
             extra_dec_rad = np.radians(extra_dec)
             extra_radius_rad = np.radians(extra_radius)
             extra_lon = extra_ra_rad
             extra_lat = extra_dec_rad
 
             healpy.projscatter(np.degrees(extra_lon), np.degrees(extra_lat),
                 lonlat=True, c='m', marker='x', s=20, label=r'Reported online (50%, 90%)')
-            for cont_lev, cont_scale, cont_col, cont_sty in zip(['50', '90.'],
+            for cont_lev, cont_scale, cont_col, cont_sty in zip(['50', '90.'], 
                     [1., 2.1459/1.177], ['m', 'm'], ['-', '--']):
                 spline_contour = circular_contour(extra_ra_rad, extra_dec_rad,
                     extra_radius_rad*cont_scale, healpy.get_nside(equatorial_map))
                 spline_lon = spline_contour[1]
                 spline_lat = np.pi/2. - spline_contour[0]
-                healpy.projplot(np.degrees(spline_lon), np.degrees(spline_lat),
-                    lonlat=True, linewidth=2., color=cont_col,
+                healpy.projplot(np.degrees(spline_lon), np.degrees(spline_lat), 
+                    lonlat=True, linewidth=2., color=cont_col, 
                     linestyle=cont_sty)
 
         plt.legend(fontsize=6, loc="lower left")
 
         # For vertical events, calculate the area with the number of pixels
-        # In the healpy map
+        # In the healpy map   
         for lev in contour_levels[1:2]:
             area_per_pix = healpy.nside2pixarea(healpy.get_nside(equatorial_map))
             num_pixs = np.count_nonzero(equatorial_map[~np.isnan(equatorial_map)] < lev)
             healpy_area = num_pixs * area_per_pix * (180./np.pi)**2.
         print("Contour Area (90%):", contour_areas[1], "degrees (cartesian)",
             healpy_area, "degrees (scaled)")
```

