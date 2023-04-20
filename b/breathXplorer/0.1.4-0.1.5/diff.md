# Comparing `tmp/breathXplorer-0.1.4.tar.gz` & `tmp/breathXplorer-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breathXplorer-0.1.4.tar", last modified: Thu Apr 20 00:29:27 2023, max compression
+gzip compressed data, was "breathXplorer-0.1.5.tar", last modified: Thu Apr 20 21:16:09 2023, max compression
```

## Comparing `breathXplorer-0.1.4.tar` & `breathXplorer-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-04-20 00:29:27.089240 breathXplorer-0.1.4/
--rw-r--r--   0 wangyk     (501) staff       (20)     1067 2023-04-12 00:06:18.000000 breathXplorer-0.1.4/LICENSE
--rw-r--r--   0 wangyk     (501) staff       (20)     1867 2023-04-20 00:29:27.089050 breathXplorer-0.1.4/PKG-INFO
--rw-r--r--   0 wangyk     (501) staff       (20)     1185 2023-04-19 23:51:39.000000 breathXplorer-0.1.4/README.md
-drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-04-20 00:29:27.087123 breathXplorer-0.1.4/breathXplorer/
--rw-r--r--   0 wangyk     (501) staff       (20)       60 2023-04-19 22:11:13.000000 breathXplorer-0.1.4/breathXplorer/__init__.py
--rw-r--r--   0 wangyk     (501) staff       (20)     2972 2023-04-12 17:21:22.000000 breathXplorer-0.1.4/breathXplorer/cluster.py
--rw-r--r--   0 wangyk     (501) staff       (20)     1858 2023-04-19 23:07:11.000000 breathXplorer-0.1.4/breathXplorer/extract.py
--rw-r--r--   0 wangyk     (501) staff       (20)     5045 2023-04-19 22:06:06.000000 breathXplorer-0.1.4/breathXplorer/file_io.py
--rw-r--r--   0 wangyk     (501) staff       (20)     6018 2023-04-12 17:21:22.000000 breathXplorer-0.1.4/breathXplorer/find_peak.py
--rw-r--r--   0 wangyk     (501) staff       (20)     2331 2023-04-20 00:26:00.000000 breathXplorer-0.1.4/breathXplorer/utils.py
-drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-04-20 00:29:27.088431 breathXplorer-0.1.4/breathXplorer.egg-info/
--rw-r--r--   0 wangyk     (501) staff       (20)     1867 2023-04-20 00:29:27.000000 breathXplorer-0.1.4/breathXplorer.egg-info/PKG-INFO
--rw-r--r--   0 wangyk     (501) staff       (20)      383 2023-04-20 00:29:27.000000 breathXplorer-0.1.4/breathXplorer.egg-info/SOURCES.txt
--rw-r--r--   0 wangyk     (501) staff       (20)        1 2023-04-20 00:29:27.000000 breathXplorer-0.1.4/breathXplorer.egg-info/dependency_links.txt
--rw-r--r--   0 wangyk     (501) staff       (20)       53 2023-04-20 00:29:27.000000 breathXplorer-0.1.4/breathXplorer.egg-info/requires.txt
--rw-r--r--   0 wangyk     (501) staff       (20)       14 2023-04-20 00:29:27.000000 breathXplorer-0.1.4/breathXplorer.egg-info/top_level.txt
--rw-r--r--   0 wangyk     (501) staff       (20)       38 2023-04-20 00:29:27.089303 breathXplorer-0.1.4/setup.cfg
--rw-r--r--   0 wangyk     (501) staff       (20)      957 2023-04-20 00:18:56.000000 breathXplorer-0.1.4/setup.py
-drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-04-20 00:29:27.088638 breathXplorer-0.1.4/tests/
--rw-r--r--   0 wangyk     (501) staff       (20)      935 2023-04-20 00:27:30.000000 breathXplorer-0.1.4/tests/test_extract.py
+drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-04-20 21:16:09.893903 breathXplorer-0.1.5/
+-rw-r--r--   0 wangyk     (501) staff       (20)     1067 2023-04-12 00:06:18.000000 breathXplorer-0.1.5/LICENSE
+-rw-r--r--   0 wangyk     (501) staff       (20)     1867 2023-04-20 21:16:09.893738 breathXplorer-0.1.5/PKG-INFO
+-rw-r--r--   0 wangyk     (501) staff       (20)     1185 2023-04-19 23:51:39.000000 breathXplorer-0.1.5/README.md
+drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-04-20 21:16:09.892137 breathXplorer-0.1.5/breathXplorer/
+-rw-r--r--   0 wangyk     (501) staff       (20)       60 2023-04-19 22:11:13.000000 breathXplorer-0.1.5/breathXplorer/__init__.py
+-rw-r--r--   0 wangyk     (501) staff       (20)     2972 2023-04-12 17:21:22.000000 breathXplorer-0.1.5/breathXplorer/cluster.py
+-rw-r--r--   0 wangyk     (501) staff       (20)     1858 2023-04-19 23:07:11.000000 breathXplorer-0.1.5/breathXplorer/extract.py
+-rw-r--r--   0 wangyk     (501) staff       (20)     5045 2023-04-19 22:06:06.000000 breathXplorer-0.1.5/breathXplorer/file_io.py
+-rw-r--r--   0 wangyk     (501) staff       (20)     6018 2023-04-12 17:21:22.000000 breathXplorer-0.1.5/breathXplorer/find_peak.py
+-rw-r--r--   0 wangyk     (501) staff       (20)     2392 2023-04-20 20:29:08.000000 breathXplorer-0.1.5/breathXplorer/utils.py
+drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-04-20 21:16:09.893170 breathXplorer-0.1.5/breathXplorer.egg-info/
+-rw-r--r--   0 wangyk     (501) staff       (20)     1867 2023-04-20 21:16:09.000000 breathXplorer-0.1.5/breathXplorer.egg-info/PKG-INFO
+-rw-r--r--   0 wangyk     (501) staff       (20)      383 2023-04-20 21:16:09.000000 breathXplorer-0.1.5/breathXplorer.egg-info/SOURCES.txt
+-rw-r--r--   0 wangyk     (501) staff       (20)        1 2023-04-20 21:16:09.000000 breathXplorer-0.1.5/breathXplorer.egg-info/dependency_links.txt
+-rw-r--r--   0 wangyk     (501) staff       (20)       53 2023-04-20 21:16:09.000000 breathXplorer-0.1.5/breathXplorer.egg-info/requires.txt
+-rw-r--r--   0 wangyk     (501) staff       (20)       14 2023-04-20 21:16:09.000000 breathXplorer-0.1.5/breathXplorer.egg-info/top_level.txt
+-rw-r--r--   0 wangyk     (501) staff       (20)       38 2023-04-20 21:16:09.893961 breathXplorer-0.1.5/setup.cfg
+-rw-r--r--   0 wangyk     (501) staff       (20)      957 2023-04-20 20:24:13.000000 breathXplorer-0.1.5/setup.py
+drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-04-20 21:16:09.893351 breathXplorer-0.1.5/tests/
+-rw-r--r--   0 wangyk     (501) staff       (20)      985 2023-04-20 20:29:28.000000 breathXplorer-0.1.5/tests/test_extract.py
```

### Comparing `breathXplorer-0.1.4/LICENSE` & `breathXplorer-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `breathXplorer-0.1.4/PKG-INFO` & `breathXplorer-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breathXplorer
-Version: 0.1.4
+Version: 0.1.5
 Summary: A toolkit for breath metabolomics analysis
 Home-page: https://github.com/wykswr/breathXplorer
 Author: wykswr
 Author-email: bifocal.above.0y@icloud.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `breathXplorer-0.1.4/README.md` & `breathXplorer-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `breathXplorer-0.1.4/breathXplorer/cluster.py` & `breathXplorer-0.1.5/breathXplorer/cluster.py`

 * *Files identical despite different names*

### Comparing `breathXplorer-0.1.4/breathXplorer/extract.py` & `breathXplorer-0.1.5/breathXplorer/extract.py`

 * *Files identical despite different names*

### Comparing `breathXplorer-0.1.4/breathXplorer/file_io.py` & `breathXplorer-0.1.5/breathXplorer/file_io.py`

 * *Files identical despite different names*

### Comparing `breathXplorer-0.1.4/breathXplorer/find_peak.py` & `breathXplorer-0.1.5/breathXplorer/find_peak.py`

 * *Files identical despite different names*

### Comparing `breathXplorer-0.1.4/breathXplorer/utils.py` & `breathXplorer-0.1.5/breathXplorer/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from functools import reduce
 from typing import Sequence
+
 import numpy as np
 import pandas as pd
-from scipy.interpolate import interp1d
 from numba import njit
+from scipy.interpolate import interp1d
 
 
 def cal_auc(x: np.ndarray, y: np.ndarray) -> float:
     """
     Calculate the area under the curve.
     :param x: x values.
     :param y: y values.
@@ -31,19 +32,21 @@
     return dict(zip(mzs, [cal_auc(times, v) / factor for v in scanned['intensities'].values()]))
 
 
 # make negative in  np.ndarray 0
 @njit
 def __make_zero(x: np.ndarray) -> np.ndarray:
     """
-    Make negative values in a numpy array 0.
+    Make negative float values in a numpy array 0.
     :param x: A numpy array.
     :return: A numpy array with negative values 0.
     """
-    x[x < 0] = 0
+    for i in range(len(x)):
+        if x[i] < 0:
+            x[i] = 0
     return x
 
 
 def interpolate_time(tb: pd.DataFrame, time: np.ndarray) -> pd.DataFrame:
     """
     Interpolate the intensities at given time points.
     :param tb: Extracted DataFrame from one sample.
@@ -52,15 +55,15 @@
     """
     intensity = tb.intensity
     tb = tb.iloc[:, 1:]
     mz = tb.index
     original_time = tb.columns.values.astype(float)
     mat = [
         __make_zero(
-            interp1d(original_time, original_int, kind='cubic', bounds_error=False, fill_value='extrapolate')(time))
+            interp1d(original_time, original_int, kind='linear', bounds_error=False, fill_value='extrapolate')(time))
         for original_int in tb.values]
     tb = pd.DataFrame(mat, index=mz, columns=time)
     tb['intensity'] = intensity
     # make intensity the first column
     cols = tb.columns.tolist()
     cols = cols[-1:] + cols[:-1]
     tb = tb[cols]
```

### Comparing `breathXplorer-0.1.4/breathXplorer.egg-info/PKG-INFO` & `breathXplorer-0.1.5/breathXplorer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breathXplorer
-Version: 0.1.4
+Version: 0.1.5
 Summary: A toolkit for breath metabolomics analysis
 Home-page: https://github.com/wykswr/breathXplorer
 Author: wykswr
 Author-email: bifocal.above.0y@icloud.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `breathXplorer-0.1.4/setup.py` & `breathXplorer-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirement.txt") as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="breathXplorer",
-    version="0.1.4",
+    version="0.1.5",
     packages=find_packages(),
     install_requires=required_packages,
     author="wykswr",
     author_email="bifocal.above.0y@icloud.com",
     description="A toolkit for breath metabolomics analysis",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

### Comparing `breathXplorer-0.1.4/tests/test_extract.py` & `breathXplorer-0.1.5/tests/test_extract.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,7 +20,8 @@
     tb = find_feature(sample, False, .2, "Topological", 6)
     tb2 = tb.copy()
     tb2.columns = ["intensity"] + list(tb.columns[1:].values + 0.001)
     tb3 = tb.copy()
     tb3.columns = ["intensity"] + list(tb.columns[1:].values - 0.002)
     tbs = time_align([tb, tb2, tb3])
     assert (tbs[0].columns[1:].values - tbs[1].columns[1:].values).sum() < 0.001
+    assert (tbs[0].iloc[:, 1:].values >= 0).any()
```

