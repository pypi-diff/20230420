# Comparing `tmp/flarespy-0.7.2.tar.gz` & `tmp/flarespy-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flarespy-0.7.2.tar", max compression
+gzip compressed data, was "flarespy-0.7.3.tar", max compression
```

## Comparing `flarespy-0.7.2.tar` & `flarespy-0.7.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.7.2/LICENSE
--rw-r--r--   0        0        0      428 2023-04-18 05:56:19.591443 flarespy-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.7.2/src/flarespy/Flare_model.py
--rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.7.2/src/flarespy/__init__.py
--rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.7.2/src/flarespy/data/model.dat
--rw-r--r--   0        0        0    26162 2023-04-18 05:56:03.763611 flarespy-0.7.2/src/flarespy/flarefinder.py
--rw-r--r--   0        0        0     4572 2023-04-16 09:27:59.194030 flarespy-0.7.2/src/flarespy/utils.py
--rw-r--r--   0        0        0       22 2023-04-18 05:56:19.589313 flarespy-0.7.2/src/flarespy/version.py
--rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 flarespy-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.7.3/LICENSE
+-rw-r--r--   0        0        0      428 2023-04-20 02:34:27.679255 flarespy-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.7.3/src/flarespy/Flare_model.py
+-rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.7.3/src/flarespy/__init__.py
+-rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.7.3/src/flarespy/data/model.dat
+-rw-r--r--   0        0        0    26176 2023-04-20 02:13:28.425091 flarespy-0.7.3/src/flarespy/flarefinder.py
+-rw-r--r--   0        0        0     4572 2023-04-16 09:27:59.194030 flarespy-0.7.3/src/flarespy/utils.py
+-rw-r--r--   0        0        0       22 2023-04-20 02:34:27.680752 flarespy-0.7.3/src/flarespy/version.py
+-rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 flarespy-0.7.3/PKG-INFO
```

### Comparing `flarespy-0.7.2/LICENSE` & `flarespy-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flarespy-0.7.2/src/flarespy/Flare_model.py` & `flarespy-0.7.3/src/flarespy/Flare_model.py`

 * *Files identical despite different names*

### Comparing `flarespy-0.7.2/src/flarespy/data/model.dat` & `flarespy-0.7.3/src/flarespy/data/model.dat`

 * *Files identical despite different names*

### Comparing `flarespy-0.7.2/src/flarespy/flarefinder.py` & `flarespy-0.7.3/src/flarespy/flarefinder.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,15 +304,15 @@
 
         before = np.nonzero((time > t_start - window) & (time < t_start))[0]
         after = np.nonzero((time > t_stop) & (time < t_stop + window))[0]
 
         return False if (before.size and after.size) else True
 
     def query_stellar_parameters(self):
-        self.stellar_parameters = pd.Series(index=STELLAR_PARAMETER_COLUMNS)
+        self.stellar_parameters = pd.Series(index=STELLAR_PARAMETER_COLUMNS, dtype=object)
         self.stellar_parameters.obs_duration = np.round(
             self.meta["TIMEDEL"] * np.nonzero(~np.isnan(self.flux.value))[0].size, 4
         )
 
         # Query parallax from Gaia DR3
         coord = SkyCoord(self.ra, self.dec, unit="deg", frame="icrs", equinox="J2000")
         radius = u.Quantity(1, u.arcmin)
```

### Comparing `flarespy-0.7.2/src/flarespy/utils.py` & `flarespy-0.7.3/src/flarespy/utils.py`

 * *Files identical despite different names*

### Comparing `flarespy-0.7.2/PKG-INFO` & `flarespy-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flarespy
-Version: 0.7.2
+Version: 0.7.3
 Summary: Find flares in TESS light curves
 Home-page: https://github.com/keyuxing/flarespy
 License: MIT
 Author: Keyu Xing
 Author-email: kyxing@mail.bnu.edu.cn
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

