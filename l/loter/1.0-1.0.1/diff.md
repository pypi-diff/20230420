# Comparing `tmp/loter-1.0.tar.gz` & `tmp/loter-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loter-1.0.tar", last modified: Fri Oct  8 09:25:11 2021, max compression
+gzip compressed data, was "loter-1.0.1.tar", last modified: Thu Apr 20 13:33:02 2023, max compression
```

## Comparing `loter-1.0.tar` & `loter-1.0.1.tar`

### file list

```diff
@@ -1,46 +1,45 @@
-drwxrwxr-x   0 drg       (1000) drg       (1000)        0 2021-10-08 09:25:11.940369 loter-1.0/
--rw-rw-r--   0 drg       (1000) drg       (1000)     1055 2021-10-06 13:34:31.000000 loter-1.0/LICENSE.txt
--rw-rw-r--   0 drg       (1000) drg       (1000)       37 2021-10-06 13:56:08.000000 loter-1.0/MANIFEST.in
--rw-rw-r--   0 drg       (1000) drg       (1000)      234 2021-10-08 09:25:11.940369 loter-1.0/PKG-INFO
--rw-rw-r--   0 drg       (1000) drg       (1000)     6786 2021-10-08 08:42:21.000000 loter-1.0/README.md
-drwxrwxr-x   0 drg       (1000) drg       (1000)        0 2021-10-08 09:25:11.936369 loter-1.0/loter/
--rw-rw-r--   0 drg       (1000) drg       (1000)        0 2019-02-18 15:06:38.000000 loter-1.0/loter/__init__.py
--rw-rw-r--   0 drg       (1000) drg       (1000)     6363 2021-09-16 13:44:57.000000 loter-1.0/loter/cli.py
-drwxrwxr-x   0 drg       (1000) drg       (1000)        0 2021-10-08 09:25:11.940369 loter-1.0/loter/datastruct/
--rw-rw-r--   0 drg       (1000) drg       (1000)        0 2019-02-18 15:06:38.000000 loter-1.0/loter/datastruct/__init__.py
--rw-rw-r--   0 drg       (1000) drg       (1000)     4596 2019-02-18 15:06:38.000000 loter-1.0/loter/datastruct/parameter.py
--rw-rw-r--   0 drg       (1000) drg       (1000)      185 2019-02-18 15:06:38.000000 loter-1.0/loter/errorhandler.py
--rw-rw-r--   0 drg       (1000) drg       (1000)     7032 2021-02-19 10:14:59.000000 loter-1.0/loter/estimatea.py
--rw-rw-r--   0 drg       (1000) drg       (1000)     8403 2019-02-18 15:06:38.000000 loter-1.0/loter/estimateh.py
--rw-rw-r--   0 drg       (1000) drg       (1000)     1136 2019-02-18 15:06:38.000000 loter-1.0/loter/find_lib.py
--rw-rw-r--   0 drg       (1000) drg       (1000)    10175 2020-02-11 09:17:20.000000 loter-1.0/loter/graph.py
--rw-rw-r--   0 drg       (1000) drg       (1000)     5439 2019-02-18 17:24:33.000000 loter-1.0/loter/initdata.py
--rw-rw-r--   0 drg       (1000) drg       (1000)      428 2019-02-18 15:06:38.000000 loter-1.0/loter/initparam.py
-drwxrwxr-x   0 drg       (1000) drg       (1000)        0 2021-10-08 09:25:11.940369 loter-1.0/loter/locanc/
--rw-rw-r--   0 drg       (1000) drg       (1000)        0 2019-02-18 15:06:38.000000 loter-1.0/loter/locanc/__init__.py
--rw-rw-r--   0 drg       (1000) drg       (1000)    23753 2019-02-26 12:42:39.000000 loter-1.0/loter/locanc/local_ancestry.bak.py
--rw-rw-r--   0 drg       (1000) drg       (1000)    11654 2020-02-11 09:17:20.000000 loter-1.0/loter/locanc/local_ancestry.py
--rw-rw-r--   0 drg       (1000) drg       (1000)     1654 2019-02-18 15:06:38.000000 loter-1.0/loter/metrics.py
--rw-rw-r--   0 drg       (1000) drg       (1000)     5469 2019-02-18 15:06:38.000000 loter-1.0/loter/opti.py
--rw-rw-r--   0 drg       (1000) drg       (1000)     6814 2019-02-18 15:06:38.000000 loter-1.0/loter/pipeline.py
--rw-rw-r--   0 drg       (1000) drg       (1000)     2643 2019-02-18 15:06:38.000000 loter-1.0/loter/predcombine.py
--rw-rw-r--   0 drg       (1000) drg       (1000)      299 2019-02-18 15:06:38.000000 loter-1.0/loter/toolsfunc.py
--rw-rw-r--   0 drg       (1000) drg       (1000)     3353 2019-02-18 15:06:38.000000 loter-1.0/loter/tree.py
--rw-rw-r--   0 drg       (1000) drg       (1000)      723 2019-02-18 15:06:38.000000 loter-1.0/loter/utils.py
--rw-rw-r--   0 drg       (1000) drg       (1000)     5332 2019-02-18 15:06:38.000000 loter-1.0/loter/wrapper_cpp.py
-drwxrwxr-x   0 drg       (1000) drg       (1000)        0 2021-10-08 09:25:11.936369 loter-1.0/loter.egg-info/
--rw-rw-r--   0 drg       (1000) drg       (1000)      234 2021-10-08 09:25:11.000000 loter-1.0/loter.egg-info/PKG-INFO
--rw-rw-r--   0 drg       (1000) drg       (1000)     2173 2021-10-08 09:25:11.000000 loter-1.0/loter.egg-info/SOURCES.txt
--rw-rw-r--   0 drg       (1000) drg       (1000)        1 2021-10-08 09:25:11.000000 loter-1.0/loter.egg-info/dependency_links.txt
--rw-rw-r--   0 drg       (1000) drg       (1000)       46 2021-10-08 09:25:11.000000 loter-1.0/loter.egg-info/entry_points.txt
--rw-rw-r--   0 drg       (1000) drg       (1000)        1 2019-02-18 15:28:06.000000 loter-1.0/loter.egg-info/not-zip-safe
--rw-rw-r--   0 drg       (1000) drg       (1000)       32 2021-10-08 09:25:11.000000 loter-1.0/loter.egg-info/requires.txt
--rw-rw-r--   0 drg       (1000) drg       (1000)       12 2021-10-08 09:25:11.000000 loter-1.0/loter.egg-info/top_level.txt
--rw-rw-r--   0 drg       (1000) drg       (1000)       54 2021-10-08 09:25:11.940369 loter-1.0/setup.cfg
--rw-rw-r--   0 drg       (1000) drg       (1000)     1823 2021-10-06 13:59:10.000000 loter-1.0/setup.py
-drwxrwxr-x   0 drg       (1000) drg       (1000)        0 2021-10-08 09:25:11.940369 loter-1.0/tests/
--rw-rw-r--   0 drg       (1000) drg       (1000)        0 2019-02-18 15:06:38.000000 loter-1.0/tests/__init__.py
--rw-rw-r--   0 drg       (1000) drg       (1000)      866 2019-02-18 15:06:38.000000 loter-1.0/tests/generate_input.py
--rw-rw-r--   0 drg       (1000) drg       (1000)      928 2019-02-18 15:06:38.000000 loter-1.0/tests/test_estimatea.py
--rw-rw-r--   0 drg       (1000) drg       (1000)     1496 2019-02-18 15:06:38.000000 loter-1.0/tests/test_estimateh.py
--rw-rw-r--   0 drg       (1000) drg       (1000)     4013 2019-02-18 15:06:38.000000 loter-1.0/tests/test_estimates.py
+drwxr-xr-x   0 gdurif    (1002) gdurif    (1002)        0 2023-04-20 13:33:02.205659 loter-1.0.1/
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)     1055 2021-10-08 07:48:18.000000 loter-1.0.1/LICENSE.txt
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)       37 2021-10-08 07:48:18.000000 loter-1.0.1/MANIFEST.in
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)     7232 2023-04-20 13:33:02.205659 loter-1.0.1/PKG-INFO
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)     6958 2023-04-20 10:26:55.000000 loter-1.0.1/README.md
+drwxr-xr-x   0 gdurif    (1002) gdurif    (1002)        0 2023-04-20 13:33:02.202326 loter-1.0.1/loter/
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)        0 2021-10-06 09:55:12.000000 loter-1.0.1/loter/__init__.py
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)     6363 2021-10-06 09:55:12.000000 loter-1.0.1/loter/cli.py
+drwxr-xr-x   0 gdurif    (1002) gdurif    (1002)        0 2023-04-20 13:33:02.205659 loter-1.0.1/loter/datastruct/
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)        0 2021-10-06 09:55:12.000000 loter-1.0.1/loter/datastruct/__init__.py
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)     4596 2021-10-06 09:55:12.000000 loter-1.0.1/loter/datastruct/parameter.py
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)      185 2021-10-06 09:55:12.000000 loter-1.0.1/loter/errorhandler.py
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)     7032 2021-10-06 09:55:12.000000 loter-1.0.1/loter/estimatea.py
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)     8403 2021-10-06 09:55:12.000000 loter-1.0.1/loter/estimateh.py
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)     1136 2021-10-06 09:55:12.000000 loter-1.0.1/loter/find_lib.py
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)    10175 2021-10-06 09:55:12.000000 loter-1.0.1/loter/graph.py
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)     5446 2023-04-20 10:26:55.000000 loter-1.0.1/loter/initdata.py
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)      428 2021-10-06 09:55:12.000000 loter-1.0.1/loter/initparam.py
+drwxr-xr-x   0 gdurif    (1002) gdurif    (1002)        0 2023-04-20 13:33:02.205659 loter-1.0.1/loter/locanc/
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)        0 2021-10-06 09:55:12.000000 loter-1.0.1/loter/locanc/__init__.py
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)    11654 2021-10-06 09:55:12.000000 loter-1.0.1/loter/locanc/local_ancestry.py
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)     1654 2021-10-06 09:55:12.000000 loter-1.0.1/loter/metrics.py
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)     5469 2021-10-06 09:55:12.000000 loter-1.0.1/loter/opti.py
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)     6814 2021-10-06 09:55:12.000000 loter-1.0.1/loter/pipeline.py
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)     2645 2023-04-20 10:26:55.000000 loter-1.0.1/loter/predcombine.py
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)      299 2021-10-06 09:55:12.000000 loter-1.0.1/loter/toolsfunc.py
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)     3353 2021-10-06 09:55:12.000000 loter-1.0.1/loter/tree.py
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)      723 2021-10-06 09:55:12.000000 loter-1.0.1/loter/utils.py
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)     5332 2021-10-06 09:55:12.000000 loter-1.0.1/loter/wrapper_cpp.py
+drwxr-xr-x   0 gdurif    (1002) gdurif    (1002)        0 2023-04-20 13:33:02.205659 loter-1.0.1/loter.egg-info/
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)     7232 2023-04-20 13:33:02.000000 loter-1.0.1/loter.egg-info/PKG-INFO
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)     1843 2023-04-20 13:33:02.000000 loter-1.0.1/loter.egg-info/SOURCES.txt
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)        1 2023-04-20 13:33:02.000000 loter-1.0.1/loter.egg-info/dependency_links.txt
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)       45 2023-04-20 13:33:02.000000 loter-1.0.1/loter.egg-info/entry_points.txt
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)        1 2023-04-20 10:39:59.000000 loter-1.0.1/loter.egg-info/not-zip-safe
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)       32 2023-04-20 13:33:02.000000 loter-1.0.1/loter.egg-info/requires.txt
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)       12 2023-04-20 13:33:02.000000 loter-1.0.1/loter.egg-info/top_level.txt
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)       38 2023-04-20 13:33:02.205659 loter-1.0.1/setup.cfg
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)     2101 2023-04-20 10:26:55.000000 loter-1.0.1/setup.py
+drwxr-xr-x   0 gdurif    (1002) gdurif    (1002)        0 2023-04-20 13:33:02.205659 loter-1.0.1/tests/
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)        0 2021-10-06 09:55:12.000000 loter-1.0.1/tests/__init__.py
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)      866 2021-10-06 09:55:12.000000 loter-1.0.1/tests/generate_input.py
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)      928 2021-10-06 09:55:12.000000 loter-1.0.1/tests/test_estimatea.py
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)     1496 2021-10-06 09:55:12.000000 loter-1.0.1/tests/test_estimateh.py
+-rw-r--r--   0 gdurif    (1002) gdurif    (1002)     4013 2021-10-06 09:55:12.000000 loter-1.0.1/tests/test_estimates.py
```

### Comparing `loter-1.0/LICENSE.txt` & `loter-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `loter-1.0/README.md` & `loter-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: loter
+Version: 1.0.1
+Summary: Optimization Package to phase haplotypes and infer local ancestry
+Home-page: https://github.com/bcm-uga/Loter
+Author: Thomas Dias-Alves
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # Loter Python package
 
 Loter can be used for haplotype phasing and local ancestry inference.
 
 Loter is available under the MIT license. Copyright 2017 - Inria, UGA, CNRS.
 
 If you encounter any problem or if you have questions regarding Loter,
@@ -10,14 +20,16 @@
 
 ---
 
 ## Requirements
 
 The package requires BLAS/LAPACK libraries, OpenMP (optional but recommended for parallel computing), a C++ compiler (tested with g++) and Python 3 (for the Python package). In addition, a version for R is under development.
 
+:information_source: When using Python precompiled package for Linux 64bits, only Python 3 is required (other required libraries are included in the precompiled package).
+
 ---
 
 ## Installation
 
 ### Python package
 
 #### From PyPI
```

### Comparing `loter-1.0/loter/cli.py` & `loter-1.0.1/loter/cli.py`

 * *Files identical despite different names*

### Comparing `loter-1.0/loter/datastruct/parameter.py` & `loter-1.0.1/loter/datastruct/parameter.py`

 * *Files identical despite different names*

### Comparing `loter-1.0/loter/estimatea.py` & `loter-1.0.1/loter/estimatea.py`

 * *Files identical despite different names*

### Comparing `loter-1.0/loter/estimateh.py` & `loter-1.0.1/loter/estimateh.py`

 * *Files identical despite different names*

### Comparing `loter-1.0/loter/find_lib.py` & `loter-1.0.1/loter/find_lib.py`

 * *Files identical despite different names*

### Comparing `loter-1.0/loter/graph.py` & `loter-1.0.1/loter/graph.py`

 * *Files identical despite different names*

### Comparing `loter-1.0/loter/initdata.py` & `loter-1.0.1/loter/initdata.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from sklearn.cluster import KMeans
 
 def init_data(data, inita, inith):
     data["A"] = inita(data["A"], data["G"]).astype(np.float32)
     data["H"] = inith(data["H"], data["G"])
     return data
 
-def init_a_rand(A, G, randomstate=None,dtype=np.int):
+def init_a_rand(A, G, randomstate=None,dtype=np.int_):
     """Initialize the clusters randomly.
 
     Initialize an already allocated matrix A (ancestry,cluster,...)
     that is an numpy array with random values between 0 and 1.
 
     :param A:           Array to initialize
     :type A:            np array
@@ -24,48 +24,48 @@
     :returns:           np.array -- Initialized A
     """
 
     if randomstate == None:
         randomstate = np.random.RandomState()
 
     (k,m) = A.shape
-    if dtype is np.int:
+    if dtype is np.int_:
         A = randomstate.randint(0,2,size=(k,m))
     else:
-        A = randomstate.random_sample(size=(k,m), dtype=np.float)
+        A = randomstate.random_sample(size=(k,m), dtype=np.float_)
 
     return A
 
-def init_a_selection_g(A, G, randomstate=None, dtype=np.int):
+def init_a_selection_g(A, G, randomstate=None, dtype=np.int_):
 
     (k,m) = A.shape
     (n,_) = G.shape
 
     if randomstate == None:
         randomstate = np.random.RandomState()
 
     def snp_to_a(snp, dtype):
         if snp == 0:
             return 0
         elif snp == 2:
             return 1
         else:
-            if dtype is np.int:
+            if dtype is np.int_:
                 return randomstate.randint(0,2)
             else:
                 return randomstate.uniform()
 
     for j in range(m):
         selected_snps = randomstate.choice(n,k,replace=False)
         for i, pos_snps in enumerate(selected_snps):
             A[i,j] = snp_to_a(G[pos_snps,j], dtype)
 
     return A
 
-def init_a_tree(A, G, randomstate=None, dtype=np.int):
+def init_a_tree(A, G, randomstate=None, dtype=np.int_):
     k, m = A.shape
     n, _ = G.shape
 
     if randomstate == None:
         randomstate = np.random.RandomState()
 
     rd_split = randomstate.randint(1, m-1)
@@ -189,15 +189,15 @@
 def create_data(G, param):
     n, m = G.shape
     k = param["nbclust"]
     data = {}
     data["G"] = G
     data["H"] = np.ascontiguousarray(np.zeros((2*n,m), dtype=np.uint8))
     data["S"] = np.ascontiguousarray(np.zeros((2*n,m), dtype=np.uint8))
-    data["A"] = np.ascontiguousarray(np.zeros((k,m), dtype=np.float))
+    data["A"] = np.ascontiguousarray(np.zeros((k,m), dtype=np.float_))
 
     return data
 
 data_initializers = {
     "rand": init_rand,
     "deter": init_deter,
     "a with g, h rand": init_awithg_hrand,
```

### Comparing `loter-1.0/loter/locanc/local_ancestry.py` & `loter-1.0.1/loter/locanc/local_ancestry.py`

 * *Files identical despite different names*

### Comparing `loter-1.0/loter/metrics.py` & `loter-1.0.1/loter/metrics.py`

 * *Files identical despite different names*

### Comparing `loter-1.0/loter/opti.py` & `loter-1.0.1/loter/opti.py`

 * *Files identical despite different names*

### Comparing `loter-1.0/loter/pipeline.py` & `loter-1.0.1/loter/pipeline.py`

 * *Files identical despite different names*

### Comparing `loter-1.0/loter/predcombine.py` & `loter-1.0.1/loter/predcombine.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import operator
 import loter.utils as utils
 
 def unpack_data_from_input(l_input):
     return [data for data, param in l_input]
 
 def compress_H(H):
-    H1, H2 = np.copy(H[::2]).astype(np.int), np.copy(H[1::2]).astype(np.int)
+    H1, H2 = np.copy(H[::2]).astype(np.int_), np.copy(H[1::2]).astype(np.int_)
     H1[H1 == 1] = 4
     H2[H2 == 1] = 5
     return H1 + H2
 
 def build_H1(H):
     r = np.copy(H)
     r[r == 4] = 1
```

### Comparing `loter-1.0/loter/tree.py` & `loter-1.0.1/loter/tree.py`

 * *Files identical despite different names*

### Comparing `loter-1.0/loter/utils.py` & `loter-1.0.1/loter/utils.py`

 * *Files identical despite different names*

### Comparing `loter-1.0/loter/wrapper_cpp.py` & `loter-1.0.1/loter/wrapper_cpp.py`

 * *Files identical despite different names*

### Comparing `loter-1.0/setup.py` & `loter-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,20 +50,27 @@
     library_dirs = libdirs,
     libraries = libs,
     extra_link_args = link_flags,
     language = 'c++',
     depends = dep,
 )
 
+# long description from the README file
+with open(os.path.join(curr_path, "README.md"), encoding="utf-8") as f:
+    long_description = f.read()
 
+
+# package setup
 setup(
     name='loter',
-    version='1.0',
-    description="Optimization Package to phase haplotypes",
+    version='1.0.1',
+    description="Optimization Package to phase haplotypes and infer local ancestry",
     author="Thomas Dias-Alves",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     url = 'https://github.com/bcm-uga/Loter',
     license = "MIT",
     license_files = ('LICENSE.txt',),
     setup_requires=['numpy'],
     install_requires=[
         "numpy",
         "pandas",
```

### Comparing `loter-1.0/tests/generate_input.py` & `loter-1.0.1/tests/generate_input.py`

 * *Files identical despite different names*

### Comparing `loter-1.0/tests/test_estimatea.py` & `loter-1.0.1/tests/test_estimatea.py`

 * *Files identical despite different names*

### Comparing `loter-1.0/tests/test_estimateh.py` & `loter-1.0.1/tests/test_estimateh.py`

 * *Files identical despite different names*

### Comparing `loter-1.0/tests/test_estimates.py` & `loter-1.0.1/tests/test_estimates.py`

 * *Files identical despite different names*

