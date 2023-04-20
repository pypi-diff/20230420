# Comparing `tmp/unravel-python-1.2.0.tar.gz` & `tmp/unravel-python-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unravel-python-1.2.0.tar", last modified: Tue Apr 11 16:23:29 2023, max compression
+gzip compressed data, was "unravel-python-1.2.1.tar", last modified: Thu Apr 20 08:12:29 2023, max compression
```

## Comparing `unravel-python-1.2.0.tar` & `unravel-python-1.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 16:23:29.570000 unravel-python-1.2.0/
--rw-rw-rw-   0        0        0    35823 2023-03-09 15:58:46.000000 unravel-python-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     3897 2023-04-11 16:23:30.000000 unravel-python-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3439 2023-04-05 09:30:36.000000 unravel-python-1.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-11 16:23:30.000000 unravel-python-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1057 2023-03-10 13:34:14.000000 unravel-python-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 16:23:29.570000 unravel-python-1.2.0/unravel/
--rw-rw-rw-   0        0        0      358 2023-04-11 16:23:06.000000 unravel-python-1.2.0/unravel/__init__.py
--rw-rw-rw-   0        0        0    48173 2023-04-05 16:32:30.000000 unravel-python-1.2.0/unravel/core.py
--rw-rw-rw-   0        0        0     4558 2023-04-05 16:37:44.000000 unravel-python-1.2.0/unravel/example.py
--rw-rw-rw-   0        0        0    14119 2023-04-09 12:47:56.000000 unravel-python-1.2.0/unravel/utils.py
--rw-rw-rw-   0        0        0     3746 2023-04-08 18:50:14.000000 unravel-python-1.2.0/unravel/viz.py
-drwxrwxrwx   0        0        0        0 2023-04-11 16:23:29.580000 unravel-python-1.2.0/unravel_python.egg-info/
--rw-rw-rw-   0        0        0     3897 2023-04-11 16:23:30.000000 unravel-python-1.2.0/unravel_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-04-11 16:23:30.000000 unravel-python-1.2.0/unravel_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 16:23:30.000000 unravel-python-1.2.0/unravel_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-04-11 16:23:30.000000 unravel-python-1.2.0/unravel_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-11 16:23:30.000000 unravel-python-1.2.0/unravel_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 08:12:29.850000 unravel-python-1.2.1/
+-rw-rw-rw-   0        0        0    35823 2023-03-09 15:58:46.000000 unravel-python-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     3897 2023-04-20 08:12:30.000000 unravel-python-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3439 2023-04-05 09:30:36.000000 unravel-python-1.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-20 08:12:30.000000 unravel-python-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1057 2023-03-10 13:34:14.000000 unravel-python-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 08:12:29.850000 unravel-python-1.2.1/unravel/
+-rw-rw-rw-   0        0        0      358 2023-04-20 08:12:00.000000 unravel-python-1.2.1/unravel/__init__.py
+-rw-rw-rw-   0        0        0    48173 2023-04-05 16:32:30.000000 unravel-python-1.2.1/unravel/core.py
+-rw-rw-rw-   0        0        0     4558 2023-04-05 16:37:44.000000 unravel-python-1.2.1/unravel/example.py
+-rw-rw-rw-   0        0        0    14119 2023-04-20 08:05:44.000000 unravel-python-1.2.1/unravel/utils.py
+-rw-rw-rw-   0        0        0     3746 2023-04-20 07:59:10.000000 unravel-python-1.2.1/unravel/viz.py
+drwxrwxrwx   0        0        0        0 2023-04-20 08:12:29.860000 unravel-python-1.2.1/unravel_python.egg-info/
+-rw-rw-rw-   0        0        0     3897 2023-04-20 08:12:30.000000 unravel-python-1.2.1/unravel_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-04-20 08:12:30.000000 unravel-python-1.2.1/unravel_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 08:12:30.000000 unravel-python-1.2.1/unravel_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-04-20 08:12:30.000000 unravel-python-1.2.1/unravel_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-20 08:12:30.000000 unravel-python-1.2.1/unravel_python.egg-info/top_level.txt
```

### Comparing `unravel-python-1.2.0/LICENSE` & `unravel-python-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.0/PKG-INFO` & `unravel-python-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unravel-python
-Version: 1.2.0
+Version: 1.2.1
 Summary: Implementation of UNRAVEL
 Home-page: https://github.com/DelinteNicolas/UNRAVEL
 Author: Nicolas Delinte
 Author-email: nicolas.delinte@uclouvain.be
 License: GNU General Public License v3.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
```

### Comparing `unravel-python-1.2.0/README.md` & `unravel-python-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.0/setup.py` & `unravel-python-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.0/unravel/core.py` & `unravel-python-1.2.1/unravel/core.py`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.0/unravel/example.py` & `unravel-python-1.2.1/unravel/example.py`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.0/unravel/utils.py` & `unravel-python-1.2.1/unravel/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,17 +337,17 @@
     density : 3-D array of shape (x,y,z)
         Array containing the streamline density in each voxel.
     '''
 
     from TIME.core import tract_to_streamlines, compute_subsegments
     from tqdm import tqdm
 
-    density = np.zeros(trk._dimensions*resolution_increase, dtype=np.float16)
+    density = np.zeros(trk._dimensions*resolution_increase, dtype=np.float32)
     rgb = np.zeros(tuple(trk._dimensions*resolution_increase)+(3,),
-                   dtype=np.float16)
+                   dtype=np.float32)
 
     sList = tract_to_streamlines(trk)
 
     for streamline in tqdm(sList):
 
         previous_point = streamline[0, :]*resolution_increase
```

### Comparing `unravel-python-1.2.0/unravel/viz.py` & `unravel-python-1.2.1/unravel/viz.py`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.0/unravel_python.egg-info/PKG-INFO` & `unravel-python-1.2.1/unravel_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unravel-python
-Version: 1.2.0
+Version: 1.2.1
 Summary: Implementation of UNRAVEL
 Home-page: https://github.com/DelinteNicolas/UNRAVEL
 Author: Nicolas Delinte
 Author-email: nicolas.delinte@uclouvain.be
 License: GNU General Public License v3.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
```

