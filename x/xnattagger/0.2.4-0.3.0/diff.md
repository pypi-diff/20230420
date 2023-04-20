# Comparing `tmp/xnattagger-0.2.4-py2.py3-none-any.whl.zip` & `tmp/xnattagger-0.3.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5617 bytes, number of entries: 8
--rw-r--r--  2.0 unx    12590 b- defN 23-Apr-20 16:27 xnattagger/__init__.py
--rw-r--r--  2.0 unx      220 b- defN 23-Apr-20 16:28 xnattagger/__version__.py
--rwxr-xr-x  2.0 unx     2178 b- defN 23-Apr-20 16:28 xnattagger-0.2.4.data/scripts/xnat_tagger.py
--rw-r--r--  2.0 unx     1541 b- defN 23-Apr-20 16:28 xnattagger-0.2.4.dist-info/LICENSE
--rw-r--r--  2.0 unx      289 b- defN 23-Apr-20 16:28 xnattagger-0.2.4.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-20 16:28 xnattagger-0.2.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-20 16:28 xnattagger-0.2.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      663 b- defN 23-Apr-20 16:28 xnattagger-0.2.4.dist-info/RECORD
-8 files, 17602 bytes uncompressed, 4457 bytes compressed:  74.7%
+Zip file size: 5630 bytes, number of entries: 8
+-rw-r--r--  2.0 unx    12743 b- defN 23-Apr-20 16:35 xnattagger/__init__.py
+-rw-r--r--  2.0 unx      220 b- defN 23-Apr-20 16:36 xnattagger/__version__.py
+-rwxr-xr-x  2.0 unx     2178 b- defN 23-Apr-20 16:36 xnattagger-0.3.0.data/scripts/xnat_tagger.py
+-rw-r--r--  2.0 unx     1541 b- defN 23-Apr-20 16:36 xnattagger-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      289 b- defN 23-Apr-20 16:36 xnattagger-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-20 16:36 xnattagger-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-20 16:36 xnattagger-0.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      663 b- defN 23-Apr-20 16:36 xnattagger-0.3.0.dist-info/RECORD
+8 files, 17755 bytes uncompressed, 4470 bytes compressed:  74.8%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: xnattagger/__init__.py
 Comment: 
 
 Filename: xnattagger/__version__.py
 Comment: 
 
-Filename: xnattagger-0.2.4.data/scripts/xnat_tagger.py
+Filename: xnattagger-0.3.0.data/scripts/xnat_tagger.py
 Comment: 
 
-Filename: xnattagger-0.2.4.dist-info/LICENSE
+Filename: xnattagger-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: xnattagger-0.2.4.dist-info/METADATA
+Filename: xnattagger-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: xnattagger-0.2.4.dist-info/WHEEL
+Filename: xnattagger-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: xnattagger-0.2.4.dist-info/top_level.txt
+Filename: xnattagger-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: xnattagger-0.2.4.dist-info/RECORD
+Filename: xnattagger-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xnattagger/__init__.py

```diff
@@ -47,15 +47,18 @@
             self.updates.update({
                 't1w': self.t1w(self.scans),  # Generate updates for T1w scan(s)
                 't1w_move': self.t1w_move(self.scans),  # Generate updates for T1w_MOVE scan(s)
                 't2w': self.t2w(self.scans),  # Generate updates for T2w scan(s)
                 't2w_move': self.t2w_move(self.scans),  # Generate updates for T2w_MOVE scan(s)
                 'dwi': self.dwi(self.scans), # Generate updates for main DWI scan(s)
                 'dwi_PA': self.dwi_PA(self.scans), # Generate updates for PA fieldmap(s)
-                'dwi_AP': self.dwi_AP(self.scans) # Generate updates for AP fieldmap(s)
+                'dwi_AP': self.dwi_AP(self.scans), # Generate updates for AP fieldmap(s)
+                'bold': self.bold(self.scans),
+                'bold_PA': self.bold_PA(self.scans),
+                'bold_AP': self.bold_AP(self.scans)
             })
 
     def apply_updates(self):
         self.upsert()
 
     def filter(self, modality):
         matches = []
```

## xnattagger/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'xnattagger'
 __description__ = 'XNAT Tagger'
 __url__ = 'https://github.com/harvard-nrg/xnattagger'
-__version__ = '0.2.4'
+__version__ = '0.3.0'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## Comparing `xnattagger-0.2.4.data/scripts/xnat_tagger.py` & `xnattagger-0.3.0.data/scripts/xnat_tagger.py`

 * *Files identical despite different names*

## Comparing `xnattagger-0.2.4.dist-info/LICENSE` & `xnattagger-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

