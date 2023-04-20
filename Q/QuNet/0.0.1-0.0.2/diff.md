# Comparing `tmp/QuNet-0.0.1-py3-none-any.whl.zip` & `tmp/QuNet-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,14 @@
-Zip file size: 19116 bytes, number of entries: 11
+Zip file size: 24524 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat        3 b- defN 23-Apr-17 09:46 qunet/__init__.py
 -rw-rw-rw-  2.0 fat     4089 b- defN 23-Apr-19 07:30 qunet/data.py
 -rw-rw-rw-  2.0 fat    21896 b- defN 23-Apr-17 09:00 qunet/models.py
+-rw-rw-rw-  2.0 fat    19126 b- defN 23-Apr-20 12:05 qunet/nnet_v1.py
 -rw-rw-rw-  2.0 fat     5344 b- defN 23-Apr-17 11:35 qunet/optim.py
 -rw-rw-rw-  2.0 fat     7781 b- defN 23-Apr-19 13:39 qunet/plotter.py
 -rw-rw-rw-  2.0 fat    21632 b- defN 23-Apr-19 13:40 qunet/trainer.py
--rw-rw-rw-  2.0 fat     1066 b- defN 23-Apr-20 10:41 QuNet-0.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      454 b- defN 23-Apr-20 10:41 QuNet-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-20 10:41 QuNet-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-20 10:41 QuNet-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      806 b- defN 23-Apr-20 10:41 QuNet-0.0.1.dist-info/RECORD
-11 files, 63169 bytes uncompressed, 17778 bytes compressed:  71.9%
+-rw-rw-rw-  2.0 fat     1066 b- defN 23-Apr-20 12:36 QuNet-0.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      453 b- defN 23-Apr-20 12:36 QuNet-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-20 12:36 QuNet-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-20 12:36 QuNet-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      880 b- defN 23-Apr-20 12:36 QuNet-0.0.2.dist-info/RECORD
+12 files, 82368 bytes uncompressed, 23078 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -3,32 +3,35 @@
 
 Filename: qunet/data.py
 Comment: 
 
 Filename: qunet/models.py
 Comment: 
 
+Filename: qunet/nnet_v1.py
+Comment: 
+
 Filename: qunet/optim.py
 Comment: 
 
 Filename: qunet/plotter.py
 Comment: 
 
 Filename: qunet/trainer.py
 Comment: 
 
-Filename: QuNet-0.0.1.dist-info/LICENSE
+Filename: QuNet-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: QuNet-0.0.1.dist-info/METADATA
+Filename: QuNet-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: QuNet-0.0.1.dist-info/WHEEL
+Filename: QuNet-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: QuNet-0.0.1.dist-info/top_level.txt
+Filename: QuNet-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: QuNet-0.0.1.dist-info/RECORD
+Filename: QuNet-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `QuNet-0.0.1.dist-info/LICENSE` & `QuNet-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `QuNet-0.0.1.dist-info/RECORD` & `QuNet-0.0.2.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 qunet/__init__.py,sha256=8ZRc1sGeVrPBx4lD717BgRaQekyh78QKV9SKsdt638U,3
 qunet/data.py,sha256=bDtDaNEOgX1krqJxGDVq5RdNaFstoIa40VI6TmLReHw,4089
 qunet/models.py,sha256=iWn9WbaR6ZB5T36jtmOinmNO_Y8eGIg16g64tDC5j5w,21896
+qunet/nnet_v1.py,sha256=zP4ev1XC7VJiGaDie0HsxubTd7PmKzdDiVvd3lKNZoo,19126
 qunet/optim.py,sha256=Q_OMgrRJKvB7kRUZni1gbjwskVclFrI5L7Hn-LiR0Ac,5344
 qunet/plotter.py,sha256=M6M94dkmeIIyk4AFq69ZeeOg2iQ2_keBM1WExqOGrsI,7781
 qunet/trainer.py,sha256=eyHpxJUx0XKb0_JbsAFUXRsyBQ0dORjOXyqgnT8qA-Y,21632
-QuNet-0.0.1.dist-info/LICENSE,sha256=x3PjoTukGVa8zbtGhLogDcamZ27C895jJMSz6dVG_Mc,1066
-QuNet-0.0.1.dist-info/METADATA,sha256=oiVbZgjPLtOW8ughfzLCZ5Me8_igxzgnZ5u8YWUEqS4,454
-QuNet-0.0.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-QuNet-0.0.1.dist-info/top_level.txt,sha256=fZTlCNIA7T6KO6-qMX35d8uK01uhYTGRKO117oubma8,6
-QuNet-0.0.1.dist-info/RECORD,,
+QuNet-0.0.2.dist-info/LICENSE,sha256=x3PjoTukGVa8zbtGhLogDcamZ27C895jJMSz6dVG_Mc,1066
+QuNet-0.0.2.dist-info/METADATA,sha256=rEOiv6lg3m_gLpe3hhDjm745Jv8ebZeL8S4q2mFWM3Q,453
+QuNet-0.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+QuNet-0.0.2.dist-info/top_level.txt,sha256=fZTlCNIA7T6KO6-qMX35d8uK01uhYTGRKO117oubma8,6
+QuNet-0.0.2.dist-info/RECORD,,
```

