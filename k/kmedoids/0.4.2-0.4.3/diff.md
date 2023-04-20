# Comparing `tmp/kmedoids-0.4.2-cp39-none-win_amd64.whl.zip` & `tmp/kmedoids-0.4.3-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 364100 bytes, number of entries: 6
--rw-r--r--  4.6 unx     7212 b- defN 23-Mar-07 11:48 kmedoids-0.4.2.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-Mar-07 11:48 kmedoids-0.4.2.dist-info/WHEEL
--rw-r--r--  4.6 unx    35823 b- defN 23-Mar-07 11:48 kmedoids-0.4.2.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx    35644 b- defN 23-Mar-07 11:48 kmedoids/__init__.py
--rwxr-xr-x  4.6 unx   994816 b- defN 23-Mar-07 11:48 kmedoids/kmedoids.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      486 b- defN 23-Mar-07 11:48 kmedoids-0.4.2.dist-info/RECORD
-6 files, 1074077 bytes uncompressed, 363230 bytes compressed:  66.2%
+Zip file size: 360938 bytes, number of entries: 6
+-rw-r--r--  4.6 unx     7212 b- defN 23-Apr-20 20:51 kmedoids-0.4.3.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- defN 23-Apr-20 20:51 kmedoids-0.4.3.dist-info/WHEEL
+-rw-r--r--  4.6 unx    35823 b- defN 23-Apr-20 20:51 kmedoids-0.4.3.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx    35547 b- defN 23-Apr-20 20:51 kmedoids/__init__.py
+-rwxr-xr-x  4.6 unx   991744 b- defN 23-Apr-20 20:51 kmedoids/kmedoids.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      486 b- defN 23-Apr-20 20:51 kmedoids-0.4.3.dist-info/RECORD
+6 files, 1070908 bytes uncompressed, 360068 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: kmedoids-0.4.2.dist-info/METADATA
+Filename: kmedoids-0.4.3.dist-info/METADATA
 Comment: 
 
-Filename: kmedoids-0.4.2.dist-info/WHEEL
+Filename: kmedoids-0.4.3.dist-info/WHEEL
 Comment: 
 
-Filename: kmedoids-0.4.2.dist-info/license_files/LICENSE
+Filename: kmedoids-0.4.3.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: kmedoids/__init__.py
 Comment: 
 
 Filename: kmedoids/kmedoids.cp39-win_amd64.pyd
 Comment: 
 
-Filename: kmedoids-0.4.2.dist-info/RECORD
+Filename: kmedoids-0.4.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kmedoids/__init__.py

```diff
@@ -613,39 +613,38 @@
 	"""
 	import numpy as np, os
 	from .kmedoids import _silhouette_i32, _silhouette_f32, _silhouette_f64
 	from .kmedoids import _par_silhouette_i32, _par_silhouette_f32, _par_silhouette_f64
 
 	if not isinstance(diss, np.ndarray):
 		diss = np.array(diss)
-	if not isinstance(labels, np.ndarray):
-		labels = np.array(labels, dtype=np.uint64)
+	labels = np.unique(labels, return_inverse=True)[1].astype(np.uint64) # ensure labels are 0..k-1
 
 	if isinstance(diss, np.ndarray):
 		dtype = diss.dtype
 		if n_cpu == -1 and samples: n_cpu = 1
 		if n_cpu == -1: n_cpu = os.cpu_count() or 1
 		assert n_cpu > 0
 		if n_cpu > 1:
 			assert not samples, "samples=true currently may only be used with n_cpu=1"
 			if dtype == np.float32:
-				return (_par_silhouette_f32(diss, labels.astype(np.uint64), n_cpu), [])
+				return (_par_silhouette_f32(diss, labels, n_cpu), [])
 			elif dtype == np.float64:
-				return (_par_silhouette_f64(diss, labels.astype(np.uint64), n_cpu), [])
+				return (_par_silhouette_f64(diss, labels, n_cpu), [])
 			elif dtype == np.int32:
-				return (_par_silhouette_i32(diss, labels.astype(np.uint64), n_cpu), [])
+				return (_par_silhouette_i32(diss, labels, n_cpu), [])
 			elif dtype == np.int64:
 				raise ValueError("Input of int64 is currently not supported, as it could overflow the float64 used internally when computing Silhouette. Use diss.astype(numpy.float64) if that is acceptable and you have the necessary memory for this copy.")
 		else:
 			if dtype == np.float32:
-				return _silhouette_f32(diss, labels.astype(np.uint64), samples)
+				return _silhouette_f32(diss, labels, samples)
 			elif dtype == np.float64:
-				return _silhouette_f64(diss, labels.astype(np.uint64), samples)
+				return _silhouette_f64(diss, labels, samples)
 			elif dtype == np.int32:
-				return _silhouette_i32(diss, labels.astype(np.uint64), samples)
+				return _silhouette_i32(diss, labels, samples)
 			elif dtype == np.int64:
 				raise ValueError("Input of int64 is currently not supported, as it could overflow the float64 used internally when computing Silhouette. Use diss.astype(numpy.float64) if that is acceptable and you have the necessary memory for this copy.")
 	raise ValueError("Input data not supported. Use a numpy array of floats.")
 
 def medoid_silhouette(diss, meds, samples=False):
 	"""Medoid Silhouette index for cluster evaluation.
```

## Comparing `kmedoids-0.4.2.dist-info/METADATA` & `kmedoids-0.4.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmedoids
-Version: 0.4.2
+Version: 0.4.3
 License-File: LICENSE
 Summary: k-Medoids Clustering in Python with FasterPAM
 Home-Page: https://github.com/kno10/python-kmedoids
 Author: Erich Schubert <erich.schubert@tu-dortmund.de>, Lars Lenssen <lars.lenssen@tu-dortmund.de>
 Author-email: Erich Schubert <erich.schubert@tu-dortmund.de>, Lars Lenssen <lars.lenssen@tu-dortmund.de>
 License: GPL-3.0-or-later
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

## Comparing `kmedoids-0.4.2.dist-info/license_files/LICENSE` & `kmedoids-0.4.3.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

