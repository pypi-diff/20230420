# Comparing `tmp/periodogram-0.0.1.tar.gz` & `tmp/periodogram-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "periodogram-0.0.1.tar", last modified: Wed Apr 19 22:55:52 2023, max compression
+gzip compressed data, was "periodogram-0.0.11.tar", last modified: Thu Apr 20 00:38:03 2023, max compression
```

## Comparing `periodogram-0.0.1.tar` & `periodogram-0.0.11.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-19 22:55:52.251331 periodogram-0.0.1/
--rw-r--r--   0 daniel     (501) staff       (20)      399 2023-04-19 22:55:52.251194 periodogram-0.0.1/PKG-INFO
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-19 22:55:52.250418 periodogram-0.0.1/periodogram/
--rw-r--r--   0 daniel     (501) staff       (20)       27 2023-04-19 22:31:37.000000 periodogram-0.0.1/periodogram/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)     2650 2023-04-19 22:30:49.000000 periodogram-0.0.1/periodogram/estimator.py
--rw-r--r--   0 daniel     (501) staff       (20)     3124 2023-04-19 22:40:56.000000 periodogram-0.0.1/periodogram/periodogram.py
--rw-r--r--   0 daniel     (501) staff       (20)      519 2023-04-19 22:39:05.000000 periodogram-0.0.1/periodogram/utils.py
--rw-r--r--   0 daniel     (501) staff       (20)     3215 2023-04-19 22:23:07.000000 periodogram-0.0.1/periodogram/window.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-19 22:55:52.251029 periodogram-0.0.1/periodogram.egg-info/
--rw-r--r--   0 daniel     (501) staff       (20)      399 2023-04-19 22:55:52.000000 periodogram-0.0.1/periodogram.egg-info/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)      267 2023-04-19 22:55:52.000000 periodogram-0.0.1/periodogram.egg-info/SOURCES.txt
--rw-r--r--   0 daniel     (501) staff       (20)        1 2023-04-19 22:55:52.000000 periodogram-0.0.1/periodogram.egg-info/dependency_links.txt
--rw-r--r--   0 daniel     (501) staff       (20)       12 2023-04-19 22:55:52.000000 periodogram-0.0.1/periodogram.egg-info/top_level.txt
--rw-r--r--   0 daniel     (501) staff       (20)       38 2023-04-19 22:55:52.251367 periodogram-0.0.1/setup.cfg
--rw-r--r--   0 daniel     (501) staff       (20)      528 2023-04-19 22:31:50.000000 periodogram-0.0.1/setup.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-20 00:38:03.316663 periodogram-0.0.11/
+-rw-r--r--   0 daniel     (501) staff       (20)     1378 2023-04-20 00:38:03.316532 periodogram-0.0.11/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)      977 2023-04-20 00:36:08.000000 periodogram-0.0.11/README.md
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-20 00:38:03.315600 periodogram-0.0.11/periodogram/
+-rw-r--r--   0 daniel     (501) staff       (20)       56 2023-04-20 00:36:08.000000 periodogram-0.0.11/periodogram/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2650 2023-04-19 22:30:49.000000 periodogram-0.0.11/periodogram/estimator.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3079 2023-04-20 00:36:08.000000 periodogram-0.0.11/periodogram/normalization.py
+-rw-r--r--   0 daniel     (501) staff       (20)     4669 2023-04-20 00:36:08.000000 periodogram-0.0.11/periodogram/periodogram.py
+-rw-r--r--   0 daniel     (501) staff       (20)      519 2023-04-19 22:39:05.000000 periodogram-0.0.11/periodogram/utils.py
+-rw-r--r--   0 daniel     (501) staff       (20)       23 2023-04-19 23:05:55.000000 periodogram-0.0.11/periodogram/version.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3215 2023-04-19 22:23:07.000000 periodogram-0.0.11/periodogram/window.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-20 00:38:03.316372 periodogram-0.0.11/periodogram.egg-info/
+-rw-r--r--   0 daniel     (501) staff       (20)     1378 2023-04-20 00:38:03.000000 periodogram-0.0.11/periodogram.egg-info/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)      363 2023-04-20 00:38:03.000000 periodogram-0.0.11/periodogram.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        1 2023-04-20 00:38:03.000000 periodogram-0.0.11/periodogram.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       25 2023-04-20 00:38:03.000000 periodogram-0.0.11/periodogram.egg-info/requires.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       12 2023-04-20 00:38:03.000000 periodogram-0.0.11/periodogram.egg-info/top_level.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       38 2023-04-20 00:38:03.316700 periodogram-0.0.11/setup.cfg
+-rw-r--r--   0 daniel     (501) staff       (20)      836 2023-04-19 23:04:31.000000 periodogram-0.0.11/setup.py
```

### Comparing `periodogram-0.0.1/periodogram/estimator.py` & `periodogram-0.0.11/periodogram/estimator.py`

 * *Files identical despite different names*

### Comparing `periodogram-0.0.1/periodogram/periodogram.py` & `periodogram-0.0.11/periodogram/normalization.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import division, print_function
-
 import numpy as np
 from astropy.timeseries import LombScargle
 
 
 def amplitude_spectrum(
     t: np.array,
     y: np.array,
@@ -98,13 +96,13 @@
     Returns:
         tuple: Frequency and power
     """
     freq, amp = amplitude_spectrum(*args, **kwargs)
     return freq, amp**2
 
 
-def psd_muHz(*args, **kwargs) -> tuple:
-    freq, p = psd(*args, **kwargs)
+def psd_muHz(t, y, **kwargs) -> tuple:
+    freq, p = psd(t, y * 1e6, **kwargs)
 
     freq = freq / (24 * 3600) * 1e6  # c/d to muHz
     p = p * (24 * 3600) * 1e-6  #  # ppm^2/(c/d) to ppm^2/muHz
     return freq, p
```

### Comparing `periodogram-0.0.1/periodogram/utils.py` & `periodogram-0.0.11/periodogram/utils.py`

 * *Files identical despite different names*

### Comparing `periodogram-0.0.1/periodogram/window.py` & `periodogram-0.0.11/periodogram/window.py`

 * *Files identical despite different names*

