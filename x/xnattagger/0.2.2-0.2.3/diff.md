# Comparing `tmp/xnattagger-0.2.2-py2.py3-none-any.whl.zip` & `tmp/xnattagger-0.2.3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5619 bytes, number of entries: 8
--rw-r--r--  2.0 unx    12521 b- defN 23-Apr-20 00:45 xnattagger/__init__.py
--rw-r--r--  2.0 unx      220 b- defN 23-Apr-20 00:48 xnattagger/__version__.py
--rwxr-xr-x  2.0 unx     2185 b- defN 23-Apr-20 00:48 xnattagger-0.2.2.data/scripts/xnat_tagger.py
--rw-r--r--  2.0 unx     1541 b- defN 23-Apr-20 00:48 xnattagger-0.2.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      289 b- defN 23-Apr-20 00:48 xnattagger-0.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-20 00:48 xnattagger-0.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-20 00:48 xnattagger-0.2.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      663 b- defN 23-Apr-20 00:48 xnattagger-0.2.2.dist-info/RECORD
-8 files, 17540 bytes uncompressed, 4459 bytes compressed:  74.6%
+Zip file size: 5621 bytes, number of entries: 8
+-rw-r--r--  2.0 unx    12527 b- defN 23-Apr-20 00:58 xnattagger/__init__.py
+-rw-r--r--  2.0 unx      220 b- defN 23-Apr-20 00:58 xnattagger/__version__.py
+-rwxr-xr-x  2.0 unx     2185 b- defN 23-Apr-20 00:58 xnattagger-0.2.3.data/scripts/xnat_tagger.py
+-rw-r--r--  2.0 unx     1541 b- defN 23-Apr-20 00:58 xnattagger-0.2.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      289 b- defN 23-Apr-20 00:58 xnattagger-0.2.3.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-20 00:58 xnattagger-0.2.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-20 00:58 xnattagger-0.2.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      663 b- defN 23-Apr-20 00:58 xnattagger-0.2.3.dist-info/RECORD
+8 files, 17546 bytes uncompressed, 4461 bytes compressed:  74.6%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: xnattagger/__init__.py
 Comment: 
 
 Filename: xnattagger/__version__.py
 Comment: 
 
-Filename: xnattagger-0.2.2.data/scripts/xnat_tagger.py
+Filename: xnattagger-0.2.3.data/scripts/xnat_tagger.py
 Comment: 
 
-Filename: xnattagger-0.2.2.dist-info/LICENSE
+Filename: xnattagger-0.2.3.dist-info/LICENSE
 Comment: 
 
-Filename: xnattagger-0.2.2.dist-info/METADATA
+Filename: xnattagger-0.2.3.dist-info/METADATA
 Comment: 
 
-Filename: xnattagger-0.2.2.dist-info/WHEEL
+Filename: xnattagger-0.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: xnattagger-0.2.2.dist-info/top_level.txt
+Filename: xnattagger-0.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: xnattagger-0.2.2.dist-info/RECORD
+Filename: xnattagger-0.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xnattagger/__init__.py

```diff
@@ -340,8 +340,8 @@
                     fo.write(json.dumps(self.scans, indent=2))
         else:
             logger.info(f'cache hit {cachefile}')
             with open(cachefile) as fo:
                 self.scans = json.loads(fo.read())
 
 class BadArgumentError(Exception):
-    pass
+    pass(yaxil)
```

## xnattagger/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'xnattagger'
 __description__ = 'XNAT Tagger'
 __url__ = 'https://github.com/harvard-nrg/xnattagger'
-__version__ = '0.2.2'
+__version__ = '0.2.3'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## Comparing `xnattagger-0.2.2.data/scripts/xnat_tagger.py` & `xnattagger-0.2.3.data/scripts/xnat_tagger.py`

 * *Files identical despite different names*

## Comparing `xnattagger-0.2.2.dist-info/LICENSE` & `xnattagger-0.2.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `xnattagger-0.2.2.dist-info/RECORD` & `xnattagger-0.2.3.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-xnattagger/__init__.py,sha256=3aZUnVNuUwgPuPfaomNSd3GwciOzPkpKKJO2Gw8CbJ4,12521
-xnattagger/__version__.py,sha256=i8jHRmMOHYgScCyYS9QVOKM5SBOs26aUrZZrClhbcnc,220
-xnattagger-0.2.2.data/scripts/xnat_tagger.py,sha256=T9jbTR77lAg3KEFqAGYableE1K9XNIdEky9s3Nk0qpc,2185
-xnattagger-0.2.2.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
-xnattagger-0.2.2.dist-info/METADATA,sha256=0uAcgB4V_Nzeyz1Dsj-PZ8ey-KZLH-EByRLpunCB0WY,289
-xnattagger-0.2.2.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-xnattagger-0.2.2.dist-info/top_level.txt,sha256=LdHhj5smL9uEh9HAguIPB8FH7EgYimhI-AODf4fl6tE,11
-xnattagger-0.2.2.dist-info/RECORD,,
+xnattagger/__init__.py,sha256=Q6kzl0PfYMLplliWDB9M6G1FupbPNDk2QDghftdEmlY,12527
+xnattagger/__version__.py,sha256=kF4tmZn-fBYG4ds7V4oE7kXsPtzTj80VT3Wlx0yOyuI,220
+xnattagger-0.2.3.data/scripts/xnat_tagger.py,sha256=T9jbTR77lAg3KEFqAGYableE1K9XNIdEky9s3Nk0qpc,2185
+xnattagger-0.2.3.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
+xnattagger-0.2.3.dist-info/METADATA,sha256=USWlvnxuetW0-YSI_1-hcLmS-U-QVhNwHjSGE01uIIM,289
+xnattagger-0.2.3.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+xnattagger-0.2.3.dist-info/top_level.txt,sha256=LdHhj5smL9uEh9HAguIPB8FH7EgYimhI-AODf4fl6tE,11
+xnattagger-0.2.3.dist-info/RECORD,,
```

