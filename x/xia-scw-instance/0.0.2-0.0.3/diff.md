# Comparing `tmp/xia_scw_instance-0.0.2-cp39-none-win_amd64.whl.zip` & `tmp/xia_scw_instance-0.0.3-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 100938 bytes, number of entries: 7
--rw-r--r--  2.0 unx      107 b- defN 23-Apr-17 18:32 xia_scw_instance/__init__.py
--rw-r--r--  2.0 unx   239104 b- defN 23-Apr-17 18:40 xia_scw_instance/instance.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-17 18:40 xia_scw_instance-0.0.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      672 b- defN 23-Apr-17 18:40 xia_scw_instance-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-17 18:40 xia_scw_instance-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Apr-17 18:40 xia_scw_instance-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      620 b- defN 23-Apr-17 18:40 xia_scw_instance-0.0.2.dist-info/RECORD
-7 files, 240771 bytes uncompressed, 99824 bytes compressed:  58.5%
+Zip file size: 101435 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      107 b- defN 23-Apr-20 14:09 xia_scw_instance/__init__.py
+-rw-r--r--  2.0 unx   240640 b- defN 23-Apr-20 14:14 xia_scw_instance/instance.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-20 14:14 xia_scw_instance-0.0.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      672 b- defN 23-Apr-20 14:14 xia_scw_instance-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-20 14:14 xia_scw_instance-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Apr-20 14:14 xia_scw_instance-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      620 b- defN 23-Apr-20 14:14 xia_scw_instance-0.0.3.dist-info/RECORD
+7 files, 242307 bytes uncompressed, 100321 bytes compressed:  58.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_scw_instance/__init__.py
 Comment: 
 
 Filename: xia_scw_instance/instance.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_scw_instance-0.0.2.dist-info/LICENSE.txt
+Filename: xia_scw_instance-0.0.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_scw_instance-0.0.2.dist-info/METADATA
+Filename: xia_scw_instance-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: xia_scw_instance-0.0.2.dist-info/WHEEL
+Filename: xia_scw_instance-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: xia_scw_instance-0.0.2.dist-info/top_level.txt
+Filename: xia_scw_instance-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_scw_instance-0.0.2.dist-info/RECORD
+Filename: xia_scw_instance-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_scw_instance/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_scw_instance.instance import ScwInstance
 
 
 __all__ = [
     "ScwInstance"
 ]
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
```

## Comparing `xia_scw_instance-0.0.2.dist-info/METADATA` & `xia_scw_instance-0.0.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-scw-instance
-Version: 0.0.2
+Version: 0.0.3
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-scw-instance/0.0.2/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-scw-instance/0.0.3/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_scw_instance-0.0.2.dist-info/RECORD` & `xia_scw_instance-0.0.3.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_scw_instance/__init__.py,sha256=vbUt2EttdesmQIAHKkwPl1qElAXT7nT4zDRSGEgN8wM,107
-xia_scw_instance/instance.cp39-win_amd64.pyd,sha256=P5rBOx9FRFEii4Dkgs6hpYkzVH6JnR8SiJ37FJ2RcnQ,239104
-xia_scw_instance-0.0.2.dist-info/LICENSE.txt,sha256=shnIQsYEvU4d6D0nUxqrQjhHb0U9ulEMxyt2I58AdZ4,152
-xia_scw_instance-0.0.2.dist-info/METADATA,sha256=3kNLxZ5Y9KPEUbqMFKLi7iS_FsHESnLJxohk-6MWAR0,672
-xia_scw_instance-0.0.2.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_scw_instance-0.0.2.dist-info/top_level.txt,sha256=ffd5mxc0r47bbdzdm8uAtew5JL-56N5Dvcrqvp9tri0,17
-xia_scw_instance-0.0.2.dist-info/RECORD,,
+xia_scw_instance/__init__.py,sha256=QN2C2gAbLj2knZrfhMrkR86fc1pXYReHuNDX62_Eidk,107
+xia_scw_instance/instance.cp39-win_amd64.pyd,sha256=Tse7s3ziMabnmt4cTe16UGSyANPHT_BWRdF-yZ-oqos,240640
+xia_scw_instance-0.0.3.dist-info/LICENSE.txt,sha256=shnIQsYEvU4d6D0nUxqrQjhHb0U9ulEMxyt2I58AdZ4,152
+xia_scw_instance-0.0.3.dist-info/METADATA,sha256=ioOFGr8kStGACF5MBPNmarTTX163ct235iGyKrdUBMU,672
+xia_scw_instance-0.0.3.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_scw_instance-0.0.3.dist-info/top_level.txt,sha256=ffd5mxc0r47bbdzdm8uAtew5JL-56N5Dvcrqvp9tri0,17
+xia_scw_instance-0.0.3.dist-info/RECORD,,
```

