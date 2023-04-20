# Comparing `tmp/vmapper-0.1.0.dev202304120903-py3-none-any.whl.zip` & `tmp/vmapper-0.1.0.dev202304200502-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 9932 bytes, number of entries: 7
+Zip file size: 9942 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 vmapper/__init__.py
 -rw-r--r--  2.0 unx     7759 b- defN 80-Jan-01 00:00 vmapper/color.py
 -rw-r--r--  2.0 unx     3395 b- defN 80-Jan-01 00:00 vmapper/meta_func.py
 -rw-r--r--  2.0 unx    29669 b- defN 80-Jan-01 00:00 vmapper/vmapper.py
--rw-r--r--  2.0 unx     1809 b- defN 80-Jan-01 00:00 vmapper-0.1.0.dev202304120903.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 vmapper-0.1.0.dev202304120903.dist-info/WHEEL
-?rw-r--r--  2.0 unx      554 b- defN 16-Jan-01 00:00 vmapper-0.1.0.dev202304120903.dist-info/RECORD
-7 files, 43326 bytes uncompressed, 8954 bytes compressed:  79.3%
+-rw-r--r--  2.0 unx     1962 b- defN 80-Jan-01 00:00 vmapper-0.1.0.dev202304200502.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 vmapper-0.1.0.dev202304200502.dist-info/WHEEL
+?rw-r--r--  2.0 unx      554 b- defN 16-Jan-01 00:00 vmapper-0.1.0.dev202304200502.dist-info/RECORD
+7 files, 43479 bytes uncompressed, 8964 bytes compressed:  79.4%
```

## zipnote {}

```diff
@@ -6,17 +6,17 @@
 
 Filename: vmapper/meta_func.py
 Comment: 
 
 Filename: vmapper/vmapper.py
 Comment: 
 
-Filename: vmapper-0.1.0.dev202304120903.dist-info/METADATA
+Filename: vmapper-0.1.0.dev202304200502.dist-info/METADATA
 Comment: 
 
-Filename: vmapper-0.1.0.dev202304120903.dist-info/WHEEL
+Filename: vmapper-0.1.0.dev202304200502.dist-info/WHEEL
 Comment: 
 
-Filename: vmapper-0.1.0.dev202304120903.dist-info/RECORD
+Filename: vmapper-0.1.0.dev202304200502.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `vmapper-0.1.0.dev202304120903.dist-info/METADATA` & `vmapper-0.1.0.dev202304200502.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmapper
-Version: 0.1.0.dev202304120903
+Version: 0.1.0.dev202304200502
 Summary: V-Mapper
 Home-page: https://github.com/yusuke-imoto-lab/V-Mapper
 Author: Yusuke Imoto
 Requires-Python: >=3.7,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -16,20 +16,21 @@
 Requires-Dist: scikit-learn (>=0.24)
 Project-URL: Documentation, https://yusuke-imoto-lab.github.io/V-Mapper/
 Project-URL: Repository, https://github.com/yusuke-imoto-lab/V-Mapper
 Description-Content-Type: text/markdown
 
 # V-Mapper - Velocity Mapper
 
+<div style="text-align:left"><img style="width:50%; height: auto" src="https://github.com/yusuke-imoto-lab/V-Mapper/blob/main/images/Logo_VMapper.png"/></div>
 <div style="text-align:left"><img style="width:60%; height: auto" src="https://github.com/yusuke-imoto-lab/V-Mapper/blob/main/images/VMapper_Top.jpg"/></div>
 
 V-Mapper (velocity Mapper) is an extension of Mapper, which is a well-known topological data analysis (TDA)  method for extracting high-dimensional topological structures as a graph \[[Singh et al., 2007](https://doi.org/10.2312/SPBG/SPBG07/091-100)\].
 V-Mapper is for high-dimensional data with position and velocity and describes a topological structure and flows on it simultaneously as a weighted directed graph (V-Mapper graph) by embedding given velocity data in the edges of the Mapper graph.
 
-[Y. Imoto and Y. Hiraoka. V-Mapper: topological data analysis for high-dimensional data with velocity, 2023, Nonlinear Theory and Its Applications, IEICE](https://dx.doi.org/10.26508/lsa.202201591). 
+[Y. Imoto and Y. Hiraoka. V-Mapper: topological data analysis for high-dimensional data with velocity, 2023, Nonlinear Theory and Its Applications, IEICE](https://doi.org/10.1587/nolta.14.92). 
 
 
 ## Installation
 To install V-Mapper package, use `pip` as follows:
 
 ```
 $ pip install vmapper
```

