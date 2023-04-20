# Comparing `tmp/determined_deploy-0.21.2rc0-py3-none-any.whl.zip` & `tmp/determined_deploy-0.21.2rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
 Zip file size: 1815 bytes, number of entries: 6
--rw-r--r--  2.0 unx      235 b- defN 23-Apr-19 15:01 determined_deploy/__init__.py
--rw-r--r--  2.0 unx       27 b- defN 23-Apr-19 15:01 determined_deploy/__version__.py
--rw-r--r--  2.0 unx      417 b- defN 23-Apr-19 15:01 determined_deploy-0.21.2rc0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 15:01 determined_deploy-0.21.2rc0.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-Apr-19 15:01 determined_deploy-0.21.2rc0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      525 b- defN 23-Apr-19 15:01 determined_deploy-0.21.2rc0.dist-info/RECORD
+-rw-r--r--  2.0 unx      235 b- defN 23-Apr-20 16:40 determined_deploy/__init__.py
+-rw-r--r--  2.0 unx       27 b- defN 23-Apr-20 16:40 determined_deploy/__version__.py
+-rw-r--r--  2.0 unx      417 b- defN 23-Apr-20 16:40 determined_deploy-0.21.2rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-20 16:40 determined_deploy-0.21.2rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-Apr-20 16:40 determined_deploy-0.21.2rc1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      525 b- defN 23-Apr-20 16:40 determined_deploy-0.21.2rc1.dist-info/RECORD
 6 files, 1314 bytes uncompressed, 847 bytes compressed:  35.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: determined_deploy/__init__.py
 Comment: 
 
 Filename: determined_deploy/__version__.py
 Comment: 
 
-Filename: determined_deploy-0.21.2rc0.dist-info/METADATA
+Filename: determined_deploy-0.21.2rc1.dist-info/METADATA
 Comment: 
 
-Filename: determined_deploy-0.21.2rc0.dist-info/WHEEL
+Filename: determined_deploy-0.21.2rc1.dist-info/WHEEL
 Comment: 
 
-Filename: determined_deploy-0.21.2rc0.dist-info/top_level.txt
+Filename: determined_deploy-0.21.2rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: determined_deploy-0.21.2rc0.dist-info/RECORD
+Filename: determined_deploy-0.21.2rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## determined_deploy/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.21.2-rc0"
+__version__ = "0.21.2-rc1"
```

## Comparing `determined_deploy-0.21.2rc0.dist-info/RECORD` & `determined_deploy-0.21.2rc1.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 determined_deploy/__init__.py,sha256=e4caLmyNqYzmNjIyNmPBCVCCmZ0BPYY6K_M279HBLeA,235
-determined_deploy/__version__.py,sha256=UHXTN33vnqwFsI22yOFoomuPOMawuPv1zgbFL0cRCPs,27
-determined_deploy-0.21.2rc0.dist-info/METADATA,sha256=FuQdey3mU5_wg8RvbnhCAbglhEBRkjpnxKALGAz41zM,417
-determined_deploy-0.21.2rc0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-determined_deploy-0.21.2rc0.dist-info/top_level.txt,sha256=cP5FE7UPh3f1fj49mbwhot5Rs5UcGIZpFFy-tZeaPhg,18
-determined_deploy-0.21.2rc0.dist-info/RECORD,,
+determined_deploy/__version__.py,sha256=v8errfpJ1jIFbo5yuHdWwU0hD-X0S1Q-G8Ut3xcPq2k,27
+determined_deploy-0.21.2rc1.dist-info/METADATA,sha256=NIFdWZJA3FwV8wYvHKH4LYfqYHrw4XB3qkXgZtq1mbQ,417
+determined_deploy-0.21.2rc1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+determined_deploy-0.21.2rc1.dist-info/top_level.txt,sha256=cP5FE7UPh3f1fj49mbwhot5Rs5UcGIZpFFy-tZeaPhg,18
+determined_deploy-0.21.2rc1.dist-info/RECORD,,
```

