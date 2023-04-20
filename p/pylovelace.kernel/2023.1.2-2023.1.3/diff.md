# Comparing `tmp/pylovelace.kernel-2023.1.2-py3-none-any.whl.zip` & `tmp/pylovelace.kernel-2023.1.3-cp312-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 196362 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat      317 b- defN 23-Apr-19 08:38 pylovelace/kernel/__init__.py
--rw-rw-rw-  2.0 fat   469504 b- defN 23-Apr-19 08:38 pylovelace/kernel/lovelace.pyd
--rw-rw-rw-  2.0 fat      113 b- defN 23-Apr-19 08:38 pylovelace.kernel-2023.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-19 08:38 pylovelace.kernel-2023.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-19 08:38 pylovelace.kernel-2023.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      523 b- defN 23-Apr-19 08:38 pylovelace.kernel-2023.1.2.dist-info/RECORD
-6 files, 470560 bytes uncompressed, 195406 bytes compressed:  58.5%
+Zip file size: 187102 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat      213 b- defN 23-Apr-20 00:49 pylovelace/kernel/__init__.py
+-rw-rw-rw-  2.0 fat   449536 b- defN 23-Apr-20 01:25 pylovelace/kernel/lovelace.pyd
+-rw-rw-rw-  2.0 fat      145 b- defN 23-Apr-20 01:25 pylovelace.kernel-2023.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       94 b- defN 23-Apr-20 01:25 pylovelace.kernel-2023.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-20 01:25 pylovelace.kernel-2023.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      523 b- defN 23-Apr-20 01:25 pylovelace.kernel-2023.1.3.dist-info/RECORD
+6 files, 450522 bytes uncompressed, 186146 bytes compressed:  58.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: pylovelace/kernel/__init__.py
 Comment: 
 
 Filename: pylovelace/kernel/lovelace.pyd
 Comment: 
 
-Filename: pylovelace.kernel-2023.1.2.dist-info/METADATA
+Filename: pylovelace.kernel-2023.1.3.dist-info/METADATA
 Comment: 
 
-Filename: pylovelace.kernel-2023.1.2.dist-info/WHEEL
+Filename: pylovelace.kernel-2023.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: pylovelace.kernel-2023.1.2.dist-info/top_level.txt
+Filename: pylovelace.kernel-2023.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pylovelace.kernel-2023.1.2.dist-info/RECORD
+Filename: pylovelace.kernel-2023.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pylovelace/kernel/__init__.py

```diff
@@ -3,11 +3,10 @@
 PyLovelace Kernel
 Copyright (c) 2023 PyLovelace
 All rights reserved.
 
 @Author: nshout
 @File: __init__.py
 """
-from .lovelace import PyLovelace, get_runtime_module, protect_code, compile_module, finalize, validate
 
-__version__ = '2023.1.2'
+__version__ = '2023.1.3'
 __description__ = 'PyLovelace Kernel'
```

