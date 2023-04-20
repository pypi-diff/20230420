# Comparing `tmp/rots-py-1.0.0.tar.gz` & `tmp/rots-py-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rots-py-1.0.0.tar", last modified: Tue Apr 18 14:34:41 2023, max compression
+gzip compressed data, was "rots-py-1.0.2.tar", last modified: Thu Apr 20 14:13:00 2023, max compression
```

## Comparing `rots-py-1.0.0.tar` & `rots-py-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 14:34:41.647170 rots-py-1.0.0/
--rw-rw-rw-   0        0        0     1097 2023-04-18 12:29:22.000000 rots-py-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2070 2023-04-18 14:34:41.646175 rots-py-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-04-18 14:24:25.000000 rots-py-1.0.0/README.md
--rw-rw-rw-   0        0        0      724 2023-04-18 14:34:08.000000 rots-py-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-18 14:34:41.647170 rots-py-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-18 14:34:41.611267 rots-py-1.0.0/src/
--rw-rw-rw-   0        0        0        0 2023-04-18 12:38:29.000000 rots-py-1.0.0/src/__init__.py
--rw-rw-rw-   0        0        0      164 2023-04-18 12:48:35.000000 rots-py-1.0.0/src/__main__.py
--rw-rw-rw-   0        0        0     3138 2023-04-18 11:13:23.000000 rots-py-1.0.0/src/calculateOverlaps1.py
--rw-rw-rw-   0        0        0     2723 2023-04-18 08:56:42.000000 rots-py-1.0.0/src/calculateOverlaps2.py
--rw-rw-rw-   0        0        0     8324 2023-04-18 10:37:22.000000 rots-py-1.0.0/src/helpers.py
--rw-rw-rw-   0        0        0    11251 2023-04-18 12:05:13.000000 rots-py-1.0.0/src/rots.py
-drwxrwxrwx   0        0        0        0 2023-04-18 14:34:41.641185 rots-py-1.0.0/src/rots_py.egg-info/
--rw-rw-rw-   0        0        0     2070 2023-04-18 14:34:41.000000 rots-py-1.0.0/src/rots_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2023-04-18 14:34:41.000000 rots-py-1.0.0/src/rots_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 14:34:41.000000 rots-py-1.0.0/src/rots_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-04-18 14:34:41.000000 rots-py-1.0.0/src/rots_py.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2023-04-18 14:34:41.000000 rots-py-1.0.0/src/rots_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       69 2023-04-18 14:34:41.000000 rots-py-1.0.0/src/rots_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 14:13:00.338101 rots-py-1.0.2/
+-rw-rw-rw-   0        0        0     1097 2023-04-18 12:29:22.000000 rots-py-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2070 2023-04-20 14:13:00.338101 rots-py-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-04-18 14:24:25.000000 rots-py-1.0.2/README.md
+-rw-rw-rw-   0        0        0      724 2023-04-20 14:10:58.000000 rots-py-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-20 14:13:00.338101 rots-py-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-20 14:13:00.291235 rots-py-1.0.2/src/
+-rw-rw-rw-   0        0        0        0 2023-04-18 12:38:29.000000 rots-py-1.0.2/src/__init__.py
+-rw-rw-rw-   0        0        0      164 2023-04-18 12:48:35.000000 rots-py-1.0.2/src/__main__.py
+-rw-rw-rw-   0        0        0     3017 2023-04-19 21:46:21.000000 rots-py-1.0.2/src/calculateOverlaps1.py
+-rw-rw-rw-   0        0        0     2732 2023-04-19 22:23:51.000000 rots-py-1.0.2/src/calculateOverlaps2.py
+-rw-rw-rw-   0        0        0     8324 2023-04-19 22:04:50.000000 rots-py-1.0.2/src/helpers.py
+-rw-rw-rw-   0        0        0    11266 2023-04-19 22:18:42.000000 rots-py-1.0.2/src/rots.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:13:00.338101 rots-py-1.0.2/src/rots_py.egg-info/
+-rw-rw-rw-   0        0        0     2070 2023-04-20 14:13:00.000000 rots-py-1.0.2/src/rots_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2023-04-20 14:13:00.000000 rots-py-1.0.2/src/rots_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 14:13:00.000000 rots-py-1.0.2/src/rots_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-04-20 14:13:00.000000 rots-py-1.0.2/src/rots_py.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2023-04-20 14:13:00.000000 rots-py-1.0.2/src/rots_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       69 2023-04-20 14:13:00.000000 rots-py-1.0.2/src/rots_py.egg-info/top_level.txt
```

### Comparing `rots-py-1.0.0/LICENSE` & `rots-py-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rots-py-1.0.0/PKG-INFO` & `rots-py-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rots-py
-Version: 1.0.0
+Version: 1.0.2
 Summary: ROTS gene ranking implementation in Python
 Author-email: "F.Mamadbekov, M.Shakya, A.Montoya, I.Ul-Haq" <fmamadbe@abo.fi>
 License: MIT License
         
         Copyright (c) 2023 EDISS-intake2-team4
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rots-py-1.0.0/pyproject.toml` & `rots-py-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pyproject.toml
 
 [project]
 name = "rots-py"
-version = "1.0.0"
+version = "1.0.2"
 description = "ROTS gene ranking implementation in Python"
 readme = "README.md"
 authors = [{ name = "F.Mamadbekov, M.Shakya, A.Montoya, I.Ul-Haq", email = "fmamadbe@abo.fi" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `rots-py-1.0.0/src/calculateOverlaps2.py` & `rots-py-1.0.2/src/calculateOverlaps2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,92 +1,89 @@
 import numpy as np
-from numba import njit
 import pandas as pd
+from numba import jit, prange
+from numba.typed import List
 
 
 def calculateOverlaps2(D, pD, D_len, N, N_len, B, overlaps, overlaps_P):
   D_ovlp = D.ravel()  
   pD_ovlp = pD.ravel()
   overlaps_ovlp = overlaps.ravel()
   overlaps_P_ovlp = overlaps_P.ravel()
 
-  res1 = np.zeros((D_len,1))
-  res2 = np.zeros((D_len,1))
-  pres1 = np.zeros((D_len,1))
-  pres2 = np.zeros((D_len,1))
+  res1 = np.zeros(D_len)
+  res2 = np.zeros(D_len)
+  pres1 = np.zeros(D_len)
+  pres2 = np.zeros(D_len)
   for b in range(1, B):
-    for i in range(D_len):
-      #ipdb.set_trace(context=6)   ## BREAKPOINT
-      res1[i] = np.abs( D_ovlp[(b-1) * D_len + i] )
-      res2[i] = np.abs( D_ovlp[(b + B - 1) * D_len + i] )
-      pres1[i] = np.abs( pD_ovlp[(b-1) * D_len + i] )
-      pres2[i] = np.abs( pD_ovlp[(b + B - 1) * D_len + i] )
-
-    ##### CalculateOverlap_2: overlaps ####  overlaps_ovlp = calculateOverlap_2(res1, res2, D_len, N, N_len, b, B, overlaps)
-    # Copy r2 and sort the copy.
-    r3 = sorted(res2, reverse=True)    
-    # Sort r2 by r1
-    r1, r2 = sort2_2(res1, res2, D_len)    
-    #Calculate the overlap
-    for k in range(N_len):
-      sum = 0
-      for j in range(N[k]):
-        sum += (r2[j] >= r3[N[k] - 1])
-      overlaps_ovlp[ (b-1) + k*B ] = sum / N[k]
-    del r3
-    #########################
-    
-    ##### CalculateOverlap_2: overlaps_P_ovlp ####  overlaps_P_ovlp = calculateOverlap_2(pres1, pres2, D_len, N, N_len, b, B, overlaps_P)
-    # Copy r2 and sort the copy.
-    pr3 = sorted(pres2, reverse=True)    
-    # Sort r2 by r1
-    pr1, pr2 = sort2_2(pres1, pres2, D_len)    
-    #Calculate the overlap
-    for k in range(N_len):
-      sum = 0
-      for j in range(N[k]):
-        sum += (pr2[j] >= pr3[N[k] - 1])
-      overlaps_P_ovlp[ (b-1) + k*B ] = sum / N[k]
-    del pr3    
-    #########################
+    res1, res2, pres1, pres2 = fast_make_res(res1, res2, pres1, pres2, D_ovlp, pD_ovlp, D_len, b, B)
+
+    overlaps_ovlp = calculateOverlap_2(res1, res2, D_len, N, N_len, b, B, overlaps_ovlp)      
+    overlaps_P_ovlp = calculateOverlap_2(pres1, pres2, D_len, N, N_len, b, B, overlaps_P_ovlp)    
 
   return {'overlaps': overlaps_ovlp.reshape(overlaps.shape), 'overlaps_P': overlaps_P_ovlp.reshape(overlaps_P.shape)}
 
+@jit(nopython=True)
+def fast_make_res(res1, res2, pres1, pres2, D_ovlp, pD_ovlp, D_len, b, B):
+  for i in range(D_len):      
+    res1[i] = np.abs( D_ovlp[(b-1) * D_len + i] )
+    res2[i] = np.abs( D_ovlp[(b + B - 1) * D_len + i] )
+    pres1[i] = np.abs( pD_ovlp[(b-1) * D_len + i] )
+    pres2[i] = np.abs( pD_ovlp[(b + B - 1) * D_len + i] )
+
+  return res1, res2, pres1, pres2 
 
-# Calculate the overlap
 
+# Calculate the overlap
 def calculateOverlap_2(r1, r2, r_len, N, N_len, b, B, overlaps):
   # Copy r2 and sort the copy.
   r3 = sorted(r2, reverse=True)
   
   # Sort r2 by r1
   r1, r2 = sort2_2(r1, r2, r_len)
   
+  typed_r3 = List()
+  [typed_r3.append(x) for x in r3]
+  #Calculate the overlap
+  overlaps = fast_ovlp(r2, typed_r3, N_len, N, B, b, overlaps)
+
+  return overlaps
+
+@jit(nopython=True)
+def fast_ovlp(r2, r3, N_len, N, B, b, overlaps):
   #Calculate the overlap
   for i in range(N_len):
     sum = 0
     for j in range(N[i]):
       sum += (r2[j] >= r3[N[i] - 1])
     overlaps[ (b-1) + i*B ] = sum / N[i]
-
-  del r3
-
   return overlaps
 
 # Sort array b based on the array a (decreasingly)
-
 def sort2_2(a, b, n):
-  pairs = [] #np.zeros([n, 2], dtype=float, order='C')
-  for i in range(n):
-    pairs.append((a[i], b[i]))
+  pairs = make_pairs(a, b, n)
   
-  # Sort the pairs (inc)
-  pairs = sorted(pairs)
+  # Sort the pairs (inc). By default pairs are sorted by the first value and
+  # in the case of a tie, the second values are used.
+  pairs = pairs[np.lexsort((pairs[:, 0], pairs[:, 1]))]
+
+  # Split the pairs back into the original vectors (dec).
+  a, b = split_pairs(pairs, n)
 
+  return (a, b)
+
+@jit(nopython=True, parallel=True)
+def make_pairs(a, b, n):
+  pairs = np.empty((n, 2))
+  for i in prange(n):
+    pairs[i] = [a[i], b[i]]
+  return pairs
+
+@jit(nopython=True, parallel=True)
+def split_pairs(pairs, n):
   # Split the pairs back into the original vectors (dec).
-  for i in range(n):
+  a = np.empty(n)
+  b = np.empty(n)
+  for i in prange(n):
     a[n-1-i] = pairs[i][0]
     b[n-1-i] = pairs[i][1]
-  
-  del pairs
-
   return (a, b)
```

### Comparing `rots-py-1.0.0/src/helpers.py` & `rots-py-1.0.2/src/helpers.py`

 * *Files identical despite different names*

### Comparing `rots-py-1.0.0/src/rots.py` & `rots-py-1.0.2/src/rots.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,16 +115,16 @@
     if progress: 
       pb.update()
     
   if progress: 
     pb.close()
 
   ## Free up memory
-  del samples
-  del pSamples
+  ##del samples
+  ##del pSamples
     
   ## ---------------------------------------------------------------------------
 
   if  a1==None or a2==None:
     ## Optimize the parameters
     if verbose:
       print("Optimizing parameters")
@@ -196,43 +196,43 @@
 
     ## Call the custom c++-loop 2.
     cResults = calculateOverlaps2(D, pD, len(D), N.astype(int), len(N),
                     int(B), overlaps, overlaps_P)
 
     ## Free up memory
     #rm(D, S)
-    del D
-    del S
+    #del D
+    #del S
 
     #ipdb.set_trace(context=6)   ## BREAKPOINT
     reprotable.iloc[i] = np.mean(cResults["overlaps"], axis=0) #colMeans(cResults[["overlaps"]])
     reprotable_P.iloc[i] = np.mean(cResults["overlaps_P"], axis=0) #colMeans(cResults[["overlaps_P"]])
     ## Standard deviation for each column
     #sqrt(rowSums((t(cResults[["overlaps"]]) - reprotable[i,])^2) / (nrow(cResults[["overlaps"]]) - 1))
     #reprotable_sd.iloc[i] = np.std(cResults["overlaps"])
     reprotable_sd.iloc[i] = np.sqrt(np.sum((cResults["overlaps"].T - reprotable.iloc[i].values[0])**2, axis=1) / 
                                       (cResults["overlaps"].shape[0] - 1))[0]
 
     ## Free up memory
-    del overlaps
-    del overlaps_P
-    del cResults
+    ##del overlaps
+    #del overlaps_P
+    #del cResults
 
     ## -------------------------------------------------------------------------
 
     ## Calculate the Z-statistic and find the top list size and the
     ## (a1,a2)-combination giving the maximal Z-value
     ztable = (reprotable - reprotable_P) / reprotable_sd
     ## Rownames of ztable are c(ssq, "slr") and colnames are N
 
     ztable = ztable.infer_objects()
 
     ## Free up memory
-    del reprotable_P
-    del reprotable_sd
+    #del reprotable_P
+    #del reprotable_sd
     
     sel = np.unravel_index(np.argmax(ztable[np.isfinite(ztable)]), ztable.shape) #np.where(ztable == max(ztable[is.finite(ztable)]), arr.ind=TRUE)
     ## Sel is a matrix containing the location(s) of the largest value (row,
     ## col). If the location of the largest value is not unique then nrow(sel)
     ## > 2 (length(sel) > 2)
 
     #ipdb.set_trace(context=6)   ## BREAKPOINT
@@ -248,37 +248,37 @@
       a2 = 0
     
     k = int(reprotable.columns[sel[1]])
     R = reprotable.iloc[sel[0],sel[1]]
     Z = ztable.iloc[sel[0],sel[1]]
     
     ## Free up memory
-    del reprotable
+    #del reprotable
     
     #ipdb.set_trace(context=6)   ## BREAKPOINT
     ## Calculate the reproducibility-optimized test statistic based on the
     ## reproducibility-maximizing a1, a2 and k values and the corresponding FDR      
     #fit = testStatistic(paired, lapply(split(1:len(cl), cl), function(x) data[:,x]))
     fit = testStatistic(paired, np.split(data.to_numpy(), np.where(np.diff(cl) != 0)[0] + 1, axis=1))
     d = fit['d'] / (a1 + a2 * fit['s'])
     pD = pD/(a1 + a2 * pS)
     
     ## Free up memory
-    del pS
+    #del pS
     
     if verbose: 
       print("Calculating p-values")
     p = calculateP(d, pD)
     
     if verbose:
       print("Calculating FDR")
     FDR = calculateFDR(d, pD, progress)
     
     ## Free up memory
-    del pD
+    #del pD
 
     ROTS_output = {
       "data": data,
       "B": B,
       "d": d,
       "logfc": logfc,
       "p": p,
```

### Comparing `rots-py-1.0.0/src/rots_py.egg-info/PKG-INFO` & `rots-py-1.0.2/src/rots_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rots-py
-Version: 1.0.0
+Version: 1.0.2
 Summary: ROTS gene ranking implementation in Python
 Author-email: "F.Mamadbekov, M.Shakya, A.Montoya, I.Ul-Haq" <fmamadbe@abo.fi>
 License: MIT License
         
         Copyright (c) 2023 EDISS-intake2-team4
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

