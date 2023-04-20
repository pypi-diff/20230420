# Comparing `tmp/pylovelace.kernel-2023.1.4-cp312-none-any.whl.zip` & `tmp/pylovelace.kernel-2023.1.5-cp312-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 187105 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat      213 b- defN 23-Apr-20 01:43 pylovelace/kernel/__init__.py
--rw-rw-rw-  2.0 fat   449536 b- defN 23-Apr-20 01:25 pylovelace/kernel/lovelace.pyd
--rw-rw-rw-  2.0 fat      145 b- defN 23-Apr-20 01:50 pylovelace.kernel-2023.1.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       94 b- defN 23-Apr-20 01:50 pylovelace.kernel-2023.1.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-20 01:50 pylovelace.kernel-2023.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      523 b- defN 23-Apr-20 01:50 pylovelace.kernel-2023.1.4.dist-info/RECORD
-6 files, 450522 bytes uncompressed, 186149 bytes compressed:  58.7%
+Zip file size: 187417 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat      270 b- defN 23-Apr-20 02:11 pylovelace/kernel/__init__.py
+-rw-rw-rw-  2.0 fat   450048 b- defN 23-Apr-20 02:15 pylovelace/kernel/lovelace.pyd
+-rw-rw-rw-  2.0 fat      145 b- defN 23-Apr-20 02:15 pylovelace.kernel-2023.1.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       94 b- defN 23-Apr-20 02:15 pylovelace.kernel-2023.1.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-20 02:15 pylovelace.kernel-2023.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      523 b- defN 23-Apr-20 02:15 pylovelace.kernel-2023.1.5.dist-info/RECORD
+6 files, 451091 bytes uncompressed, 186461 bytes compressed:  58.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: pylovelace/kernel/__init__.py
 Comment: 
 
 Filename: pylovelace/kernel/lovelace.pyd
 Comment: 
 
-Filename: pylovelace.kernel-2023.1.4.dist-info/METADATA
+Filename: pylovelace.kernel-2023.1.5.dist-info/METADATA
 Comment: 
 
-Filename: pylovelace.kernel-2023.1.4.dist-info/WHEEL
+Filename: pylovelace.kernel-2023.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: pylovelace.kernel-2023.1.4.dist-info/top_level.txt
+Filename: pylovelace.kernel-2023.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: pylovelace.kernel-2023.1.4.dist-info/RECORD
+Filename: pylovelace.kernel-2023.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pylovelace/kernel/__init__.py

```diff
@@ -3,10 +3,12 @@
 PyLovelace Kernel
 Copyright (c) 2023 PyLovelace
 All rights reserved.
 
 @Author: nshout
 @File: __init__.py
 """
-
-__version__ = '2023.1.4'
-__description__ = 'PyLovelace Kernel'
+from .lovelace import (
+    PyLovelace, get_runtime_module,
+    protect_code, compile_module,
+    finalize, validate
+)
```

## Comparing `pylovelace.kernel-2023.1.4.dist-info/RECORD` & `pylovelace.kernel-2023.1.5.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-pylovelace/kernel/__init__.py,sha256=puxZh76eJXvCHHa7AJT6QvIvJvQQUCt7oAkhdnPt7rs,213
-pylovelace/kernel/lovelace.pyd,sha256=alJe6JhUxlKnoTX4DiuWaZtzrmQsUSnjLNcBFXF7qRk,449536
-pylovelace.kernel-2023.1.4.dist-info/METADATA,sha256=yLY4Hj_KgcramctJYWIK__NqY-vvcBvZEqRbSEjVlEE,145
-pylovelace.kernel-2023.1.4.dist-info/WHEEL,sha256=y3qbVa0h6Xc5sDMG8DpM6VuvsiM-PVvRy__oVQHkDzw,94
-pylovelace.kernel-2023.1.4.dist-info/top_level.txt,sha256=J7DsoNzAcCKQQcB_uVPOh9mNcQSDemGF9xpSWgkWUDs,11
-pylovelace.kernel-2023.1.4.dist-info/RECORD,,
+pylovelace/kernel/__init__.py,sha256=zu1dF8ySBb18iUiJSnCrjl-oaani1T0aJPl_qI2YkHw,270
+pylovelace/kernel/lovelace.pyd,sha256=1_wl2LBeOuG64sxLFomz-5iwsuzoGJpVcmB5gIGPzZM,450048
+pylovelace.kernel-2023.1.5.dist-info/METADATA,sha256=Z7Etkue8QpzpXXvELhWVIiGp_EBe3Gsxa5jvHKRTBMo,145
+pylovelace.kernel-2023.1.5.dist-info/WHEEL,sha256=y3qbVa0h6Xc5sDMG8DpM6VuvsiM-PVvRy__oVQHkDzw,94
+pylovelace.kernel-2023.1.5.dist-info/top_level.txt,sha256=J7DsoNzAcCKQQcB_uVPOh9mNcQSDemGF9xpSWgkWUDs,11
+pylovelace.kernel-2023.1.5.dist-info/RECORD,,
```

