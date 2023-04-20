# Comparing `tmp/pylovelace.kernel-2023.1.3-cp312-none-any.whl.zip` & `tmp/pylovelace.kernel-2023.1.4-cp312-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 187102 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat      213 b- defN 23-Apr-20 00:49 pylovelace/kernel/__init__.py
+Zip file size: 187105 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat      213 b- defN 23-Apr-20 01:43 pylovelace/kernel/__init__.py
 -rw-rw-rw-  2.0 fat   449536 b- defN 23-Apr-20 01:25 pylovelace/kernel/lovelace.pyd
--rw-rw-rw-  2.0 fat      145 b- defN 23-Apr-20 01:25 pylovelace.kernel-2023.1.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       94 b- defN 23-Apr-20 01:25 pylovelace.kernel-2023.1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-20 01:25 pylovelace.kernel-2023.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      523 b- defN 23-Apr-20 01:25 pylovelace.kernel-2023.1.3.dist-info/RECORD
-6 files, 450522 bytes uncompressed, 186146 bytes compressed:  58.7%
+-rw-rw-rw-  2.0 fat      145 b- defN 23-Apr-20 01:50 pylovelace.kernel-2023.1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       94 b- defN 23-Apr-20 01:50 pylovelace.kernel-2023.1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-20 01:50 pylovelace.kernel-2023.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      523 b- defN 23-Apr-20 01:50 pylovelace.kernel-2023.1.4.dist-info/RECORD
+6 files, 450522 bytes uncompressed, 186149 bytes compressed:  58.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: pylovelace/kernel/__init__.py
 Comment: 
 
 Filename: pylovelace/kernel/lovelace.pyd
 Comment: 
 
-Filename: pylovelace.kernel-2023.1.3.dist-info/METADATA
+Filename: pylovelace.kernel-2023.1.4.dist-info/METADATA
 Comment: 
 
-Filename: pylovelace.kernel-2023.1.3.dist-info/WHEEL
+Filename: pylovelace.kernel-2023.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: pylovelace.kernel-2023.1.3.dist-info/top_level.txt
+Filename: pylovelace.kernel-2023.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: pylovelace.kernel-2023.1.3.dist-info/RECORD
+Filename: pylovelace.kernel-2023.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pylovelace/kernel/__init__.py

```diff
@@ -4,9 +4,9 @@
 Copyright (c) 2023 PyLovelace
 All rights reserved.
 
 @Author: nshout
 @File: __init__.py
 """
 
-__version__ = '2023.1.3'
+__version__ = '2023.1.4'
 __description__ = 'PyLovelace Kernel'
```

## Comparing `pylovelace.kernel-2023.1.3.dist-info/RECORD` & `pylovelace.kernel-2023.1.4.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-pylovelace/kernel/__init__.py,sha256=99Dz5VN61tcVUsEWQtNdp7z2BCzA3Kr2eiB1qjhVmno,213
+pylovelace/kernel/__init__.py,sha256=puxZh76eJXvCHHa7AJT6QvIvJvQQUCt7oAkhdnPt7rs,213
 pylovelace/kernel/lovelace.pyd,sha256=alJe6JhUxlKnoTX4DiuWaZtzrmQsUSnjLNcBFXF7qRk,449536
-pylovelace.kernel-2023.1.3.dist-info/METADATA,sha256=1YCfF3HpGurEoBVcUAKjkTGzURuA7C_qfbJmU6_u_1g,145
-pylovelace.kernel-2023.1.3.dist-info/WHEEL,sha256=y3qbVa0h6Xc5sDMG8DpM6VuvsiM-PVvRy__oVQHkDzw,94
-pylovelace.kernel-2023.1.3.dist-info/top_level.txt,sha256=J7DsoNzAcCKQQcB_uVPOh9mNcQSDemGF9xpSWgkWUDs,11
-pylovelace.kernel-2023.1.3.dist-info/RECORD,,
+pylovelace.kernel-2023.1.4.dist-info/METADATA,sha256=yLY4Hj_KgcramctJYWIK__NqY-vvcBvZEqRbSEjVlEE,145
+pylovelace.kernel-2023.1.4.dist-info/WHEEL,sha256=y3qbVa0h6Xc5sDMG8DpM6VuvsiM-PVvRy__oVQHkDzw,94
+pylovelace.kernel-2023.1.4.dist-info/top_level.txt,sha256=J7DsoNzAcCKQQcB_uVPOh9mNcQSDemGF9xpSWgkWUDs,11
+pylovelace.kernel-2023.1.4.dist-info/RECORD,,
```

