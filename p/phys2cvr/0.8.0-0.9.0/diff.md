# Comparing `tmp/phys2cvr-0.8.0.tar.gz` & `tmp/phys2cvr-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/phys2cvr-0.8.0.tar", last modified: Wed Feb 23 20:56:18 2022, max compression
+gzip compressed data, was "dist/phys2cvr-0.9.0.tar", last modified: Wed Feb 23 20:59:09 2022, max compression
```

## Comparing `phys2cvr-0.8.0.tar` & `phys2cvr-0.9.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-23 20:56:18.000000 phys2cvr-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (116)      113 2022-02-23 20:56:06.000000 phys2cvr-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)    68611 2022-02-23 20:56:06.000000 phys2cvr-0.8.0/versioneer.py
--rw-r--r--   0 runner    (1001) docker     (116)      375 2022-02-23 20:56:06.000000 phys2cvr-0.8.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)     1479 2022-02-23 20:56:06.000000 phys2cvr-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-23 20:56:18.000000 phys2cvr-0.8.0/phys2cvr/
--rw-r--r--   0 runner    (1001) docker     (116)     4275 2022-02-23 20:56:06.000000 phys2cvr-0.8.0/phys2cvr/signal.py
--rw-r--r--   0 runner    (1001) docker     (116)      370 2022-02-23 20:56:06.000000 phys2cvr-0.8.0/phys2cvr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-23 20:56:18.000000 phys2cvr-0.8.0/phys2cvr/cli/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-23 20:56:06.000000 phys2cvr-0.8.0/phys2cvr/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    24774 2022-02-23 20:56:06.000000 phys2cvr-0.8.0/phys2cvr/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (116)      497 2022-02-23 20:56:18.000000 phys2cvr-0.8.0/phys2cvr/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-23 20:56:18.000000 phys2cvr-0.8.0/phys2cvr/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-23 20:56:06.000000 phys2cvr-0.8.0/phys2cvr/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7456 2022-02-23 20:56:06.000000 phys2cvr-0.8.0/phys2cvr/io.py
--rw-r--r--   0 runner    (1001) docker     (116)    15319 2022-02-23 20:56:06.000000 phys2cvr-0.8.0/phys2cvr/stats.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    25729 2022-02-23 20:56:06.000000 phys2cvr-0.8.0/phys2cvr/phys2cvr.py
--rw-r--r--   0 runner    (1001) docker     (116)     1662 2022-02-23 20:56:18.000000 phys2cvr-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)       52 2022-02-23 20:56:06.000000 phys2cvr-0.8.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-23 20:56:18.000000 phys2cvr-0.8.0/phys2cvr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)       54 2022-02-23 20:56:18.000000 phys2cvr-0.8.0/phys2cvr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-02-23 20:56:18.000000 phys2cvr-0.8.0/phys2cvr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-02-23 20:56:18.000000 phys2cvr-0.8.0/phys2cvr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      491 2022-02-23 20:56:18.000000 phys2cvr-0.8.0/phys2cvr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)     2749 2022-02-23 20:56:18.000000 phys2cvr-0.8.0/phys2cvr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      220 2022-02-23 20:56:18.000000 phys2cvr-0.8.0/phys2cvr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2022-02-23 20:56:18.000000 phys2cvr-0.8.0/phys2cvr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)    11357 2022-02-23 20:56:06.000000 phys2cvr-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     2749 2022-02-23 20:56:18.000000 phys2cvr-0.8.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-23 20:59:09.000000 phys2cvr-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (116)      113 2022-02-23 20:58:57.000000 phys2cvr-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)    68611 2022-02-23 20:58:57.000000 phys2cvr-0.9.0/versioneer.py
+-rw-r--r--   0 runner    (1001) docker     (116)      375 2022-02-23 20:58:57.000000 phys2cvr-0.9.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1479 2022-02-23 20:58:57.000000 phys2cvr-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-23 20:59:09.000000 phys2cvr-0.9.0/phys2cvr/
+-rw-r--r--   0 runner    (1001) docker     (116)     4275 2022-02-23 20:58:57.000000 phys2cvr-0.9.0/phys2cvr/signal.py
+-rw-r--r--   0 runner    (1001) docker     (116)      370 2022-02-23 20:58:57.000000 phys2cvr-0.9.0/phys2cvr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-23 20:59:09.000000 phys2cvr-0.9.0/phys2cvr/cli/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-23 20:58:57.000000 phys2cvr-0.9.0/phys2cvr/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    24774 2022-02-23 20:58:57.000000 phys2cvr-0.9.0/phys2cvr/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (116)      497 2022-02-23 20:59:09.000000 phys2cvr-0.9.0/phys2cvr/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-23 20:59:09.000000 phys2cvr-0.9.0/phys2cvr/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-23 20:58:57.000000 phys2cvr-0.9.0/phys2cvr/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7456 2022-02-23 20:58:57.000000 phys2cvr-0.9.0/phys2cvr/io.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14785 2022-02-23 20:58:57.000000 phys2cvr-0.9.0/phys2cvr/stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    25729 2022-02-23 20:58:57.000000 phys2cvr-0.9.0/phys2cvr/phys2cvr.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1662 2022-02-23 20:59:09.000000 phys2cvr-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)       52 2022-02-23 20:58:57.000000 phys2cvr-0.9.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-23 20:59:09.000000 phys2cvr-0.9.0/phys2cvr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)       54 2022-02-23 20:59:08.000000 phys2cvr-0.9.0/phys2cvr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-02-23 20:59:08.000000 phys2cvr-0.9.0/phys2cvr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-02-23 20:59:08.000000 phys2cvr-0.9.0/phys2cvr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)      491 2022-02-23 20:59:08.000000 phys2cvr-0.9.0/phys2cvr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     2749 2022-02-23 20:59:08.000000 phys2cvr-0.9.0/phys2cvr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      220 2022-02-23 20:59:08.000000 phys2cvr-0.9.0/phys2cvr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        9 2022-02-23 20:59:08.000000 phys2cvr-0.9.0/phys2cvr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)    11357 2022-02-23 20:58:57.000000 phys2cvr-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)     2749 2022-02-23 20:59:09.000000 phys2cvr-0.9.0/PKG-INFO
```

### Comparing `phys2cvr-0.8.0/versioneer.py` & `phys2cvr-0.9.0/versioneer.py`

 * *Files identical despite different names*

### Comparing `phys2cvr-0.8.0/README.md` & `phys2cvr-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `phys2cvr-0.8.0/phys2cvr/signal.py` & `phys2cvr-0.9.0/phys2cvr/signal.py`

 * *Files identical despite different names*

### Comparing `phys2cvr-0.8.0/phys2cvr/cli/run.py` & `phys2cvr-0.9.0/phys2cvr/cli/run.py`

 * *Files identical despite different names*

### Comparing `phys2cvr-0.8.0/phys2cvr/io.py` & `phys2cvr-0.9.0/phys2cvr/io.py`

 * *Files identical despite different names*

### Comparing `phys2cvr-0.8.0/phys2cvr/stats.py` & `phys2cvr-0.9.0/phys2cvr/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,25 +156,14 @@
     petco2hrf_cut = petco2hrf[first_tp:]
 
     nrep = len(petco2hrf_cut) - len(func_cut)
 
     _, optshift, xcorr = x_corr(func_cut, petco2hrf, nrep)
     LGR.info(f'First cross correlation estimated bulk shift at {optshift/freq} seconds')
 
-    if trial_len and n_trials and n_trials > 2:
-        LGR.info('Running second bulk shift estimation')
-        if len(func_upsampled) + nrep > len(petco2hrf):
-            pad = len(func_upsampled) + nrep - len(petco2hrf)
-            petco2hrf_padded = np.pad(petco2hrf, pad, mode='mean')
-        else:
-            petco2hrf_padded = petco2hrf
-
-        _, optshift, xcorr = x_corr(func_upsampled, petco2hrf_padded, nrep, -nrep, optshift)
-        LGR.info(f'Second cross correlation estimated bulk shift at {optshift/freq} seconds')
-
     # Export estimated optimal shift in seconds
     with open(f'{outname}_optshift.1D', 'w') as f:
         print(f'{(optshift/freq):.4f}', file=f)
 
     petco2hrf_shift = petco2hrf[optshift:optshift+len_upd]
 
     # preparing for and exporting figures of shift
```

### Comparing `phys2cvr-0.8.0/phys2cvr/phys2cvr.py` & `phys2cvr-0.9.0/phys2cvr/phys2cvr.py`

 * *Files identical despite different names*

### Comparing `phys2cvr-0.8.0/setup.cfg` & `phys2cvr-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `phys2cvr-0.8.0/phys2cvr.egg-info/PKG-INFO` & `phys2cvr-0.9.0/phys2cvr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phys2cvr
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python library to generate regressors for and compute Cerebrovascular Reactivity and lag maps.
 Home-page: https://github.com/smoia/phys2cvr
 Author: Stefano Moia
 Maintainer: Stefano Moia
 Maintainer-email: s.moia@bcbl.eu
 License: Apache-2.0
 Download-URL: https://github.com/smoia/phys2cvr
@@ -59,11 +59,11 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides: phys2cvr
 Requires-Python: >=3.6.1
 Description-Content-Type: text/markdown; charset=UTF-8
+Provides-Extra: style
 Provides-Extra: all
 Provides-Extra: test
-Provides-Extra: style
 Provides-Extra: doc
```

### Comparing `phys2cvr-0.8.0/LICENSE` & `phys2cvr-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phys2cvr-0.8.0/PKG-INFO` & `phys2cvr-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phys2cvr
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python library to generate regressors for and compute Cerebrovascular Reactivity and lag maps.
 Home-page: https://github.com/smoia/phys2cvr
 Author: Stefano Moia
 Maintainer: Stefano Moia
 Maintainer-email: s.moia@bcbl.eu
 License: Apache-2.0
 Download-URL: https://github.com/smoia/phys2cvr
@@ -59,11 +59,11 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides: phys2cvr
 Requires-Python: >=3.6.1
 Description-Content-Type: text/markdown; charset=UTF-8
+Provides-Extra: style
 Provides-Extra: all
 Provides-Extra: test
-Provides-Extra: style
 Provides-Extra: doc
```

