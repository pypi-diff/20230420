# Comparing `tmp/MatAn-0.1.5.2-py3-none-any.whl.zip` & `tmp/MatAn-0.1.5.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 19075 bytes, number of entries: 8
--rw-r--r--  2.0 unx    17024 b- defN 23-Apr-20 06:16 matan/__init__.py
+Zip file size: 19807 bytes, number of entries: 8
+-rw-r--r--  2.0 unx    17003 b- defN 23-Apr-20 21:22 matan/__init__.py
 -rw-r--r--  2.0 unx      107 b- defN 23-Apr-18 08:30 misc/__init__.py
--rw-r--r--  2.0 unx     2363 b- defN 23-Apr-18 08:30 properties/__init__.py
--rw-r--r--  2.0 unx    34670 b- defN 23-Apr-20 21:01 MatAn-0.1.5.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     2187 b- defN 23-Apr-20 21:01 MatAn-0.1.5.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-20 21:01 MatAn-0.1.5.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       22 b- defN 23-Apr-20 21:01 MatAn-0.1.5.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      613 b- defN 23-Apr-20 21:01 MatAn-0.1.5.2.dist-info/RECORD
-8 files, 57078 bytes uncompressed, 18017 bytes compressed:  68.4%
+-rw-r--r--  2.0 unx     2491 b- defN 23-Apr-20 21:21 properties/__init__.py
+-rw-r--r--  2.0 unx    34670 b- defN 23-Apr-20 21:28 MatAn-0.1.5.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3931 b- defN 23-Apr-20 21:28 MatAn-0.1.5.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-20 21:28 MatAn-0.1.5.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       22 b- defN 23-Apr-20 21:28 MatAn-0.1.5.2.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      623 b- defN 23-Apr-20 21:28 MatAn-0.1.5.2.1.dist-info/RECORD
+8 files, 58939 bytes uncompressed, 18729 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: misc/__init__.py
 Comment: 
 
 Filename: properties/__init__.py
 Comment: 
 
-Filename: MatAn-0.1.5.2.dist-info/LICENSE
+Filename: MatAn-0.1.5.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: MatAn-0.1.5.2.dist-info/METADATA
+Filename: MatAn-0.1.5.2.1.dist-info/METADATA
 Comment: 
 
-Filename: MatAn-0.1.5.2.dist-info/WHEEL
+Filename: MatAn-0.1.5.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: MatAn-0.1.5.2.dist-info/top_level.txt
+Filename: MatAn-0.1.5.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: MatAn-0.1.5.2.dist-info/RECORD
+Filename: MatAn-0.1.5.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## matan/__init__.py

```diff
@@ -7,23 +7,24 @@
 import glob
 from typing import Union
 import properties
 # from sklearn.linear_model import LinearRegression
 
 
 """
+TODO:
+Create  abstract class for properties like tensile strength, tensile modulus, etc, with pass, so using diffrent norms and materials will be easier
+Move calculation of real values into method of engineering values
+Add decorators
 
-1. move real and eng values to other files
-2. create instance in sample
-3. inherit logic to both eng and real values from another class
 SOURCES:
 
 https://professorkazarinoff.github.io/Engineering-Materials-Programming/07-Mechanical-Properties/mechanical-properties-from-stress-strain-curves.html
 
-According to ISO 527-1: https://cdn.standards.iteh.ai/samples/75824/61c480ef4bf0494aa6966bd4c2244c2e/ISO-527-1-2019.pdf
+
 """
 
 """c
     class to menage files
     methods are types of techniques used to manufacture material
     """
```

## properties/__init__.py

```diff
@@ -1,10 +1,13 @@
 import numpy as np
 import misc
 
+"""
+According to ISO 527-1: https://cdn.standards.iteh.ai/samples/75824/61c480ef4bf0494aa6966bd4c2244c2e/ISO-527-1-2019.pdf
+"""
 class tensile_modulus:
     def __init__(self,
                  stress,
                  strain,
                  percent_strain=False,
                  lower_limit=0.05,
                  upper_limit=0.25
```

## Comparing `MatAn-0.1.5.2.dist-info/LICENSE` & `MatAn-0.1.5.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

