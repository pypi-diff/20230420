# Comparing `tmp/pylovelace-2023.1.4-py3-none-any.whl.zip` & `tmp/pylovelace-2023.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 18007 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat      228 b- defN 23-Apr-20 01:30 pylovelace/__init__.py
+Zip file size: 18008 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat      228 b- defN 23-Apr-20 02:18 pylovelace/__init__.py
 -rw-rw-rw-  2.0 fat     8086 b- defN 23-Apr-19 05:09 pylovelace/__main__.py
 -rw-rw-rw-  2.0 fat     4383 b- defN 23-Apr-19 05:09 pylovelace/protect.py
--rw-rw-rw-  2.0 fat    35149 b- defN 23-Apr-20 01:30 pylovelace-2023.1.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1743 b- defN 23-Apr-20 01:30 pylovelace-2023.1.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-20 01:30 pylovelace-2023.1.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       56 b- defN 23-Apr-20 01:30 pylovelace-2023.1.4.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-20 01:30 pylovelace-2023.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      753 b- defN 23-Apr-20 01:30 pylovelace-2023.1.4.dist-info/RECORD
-9 files, 50501 bytes uncompressed, 16701 bytes compressed:  66.9%
+-rw-rw-rw-  2.0 fat    35149 b- defN 23-Apr-20 02:19 pylovelace-2023.1.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1743 b- defN 23-Apr-20 02:19 pylovelace-2023.1.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-20 02:19 pylovelace-2023.1.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       56 b- defN 23-Apr-20 02:19 pylovelace-2023.1.5.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-20 02:19 pylovelace-2023.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      753 b- defN 23-Apr-20 02:19 pylovelace-2023.1.5.dist-info/RECORD
+9 files, 50501 bytes uncompressed, 16702 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: pylovelace/__main__.py
 Comment: 
 
 Filename: pylovelace/protect.py
 Comment: 
 
-Filename: pylovelace-2023.1.4.dist-info/LICENSE
+Filename: pylovelace-2023.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: pylovelace-2023.1.4.dist-info/METADATA
+Filename: pylovelace-2023.1.5.dist-info/METADATA
 Comment: 
 
-Filename: pylovelace-2023.1.4.dist-info/WHEEL
+Filename: pylovelace-2023.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: pylovelace-2023.1.4.dist-info/entry_points.txt
+Filename: pylovelace-2023.1.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: pylovelace-2023.1.4.dist-info/top_level.txt
+Filename: pylovelace-2023.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: pylovelace-2023.1.4.dist-info/RECORD
+Filename: pylovelace-2023.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pylovelace/__init__.py

```diff
@@ -4,9 +4,9 @@
 Copyright (c) 2023 PyLovelace
 All rights reserved.
 
 @Author: nshout
 @File: __init__.py
 """
 
-__version__ = "2023.1.4"
+__version__ = "2023.1.5"
 __description__ = "Python code protection/obfuscation tool"
```

## Comparing `pylovelace-2023.1.4.dist-info/LICENSE` & `pylovelace-2023.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pylovelace-2023.1.4.dist-info/METADATA` & `pylovelace-2023.1.5.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylovelace
-Version: 2023.1.4
+Version: 2023.1.5
 Summary: Python code protection/obfuscation tool
 Home-page: https://github.com/pylovelace/pylovelace
 Author: nshout
 Keywords: obfuscate obfuscation distribute production tool
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Requires-Python: >=3.10, <3.13
 License-File: LICENSE
-Requires-Dist: pylovelace.kernel (>2023.1.2)
+Requires-Dist: pylovelace.kernel (>2023.1.4)
 
 PyLovelace Python protection tool.
 ===================================
 
 PyLovelace is a Python protection tool that can be used to protect
 Python source code from being reverse engineered.
```

