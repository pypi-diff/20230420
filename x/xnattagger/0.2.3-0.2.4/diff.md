# Comparing `tmp/xnattagger-0.2.3-py2.py3-none-any.whl.zip` & `tmp/xnattagger-0.2.4-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5621 bytes, number of entries: 8
--rw-r--r--  2.0 unx    12527 b- defN 23-Apr-20 00:58 xnattagger/__init__.py
--rw-r--r--  2.0 unx      220 b- defN 23-Apr-20 00:58 xnattagger/__version__.py
--rwxr-xr-x  2.0 unx     2185 b- defN 23-Apr-20 00:58 xnattagger-0.2.3.data/scripts/xnat_tagger.py
--rw-r--r--  2.0 unx     1541 b- defN 23-Apr-20 00:58 xnattagger-0.2.3.dist-info/LICENSE
--rw-r--r--  2.0 unx      289 b- defN 23-Apr-20 00:58 xnattagger-0.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-20 00:58 xnattagger-0.2.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-20 00:58 xnattagger-0.2.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      663 b- defN 23-Apr-20 00:58 xnattagger-0.2.3.dist-info/RECORD
-8 files, 17546 bytes uncompressed, 4461 bytes compressed:  74.6%
+Zip file size: 5617 bytes, number of entries: 8
+-rw-r--r--  2.0 unx    12590 b- defN 23-Apr-20 16:27 xnattagger/__init__.py
+-rw-r--r--  2.0 unx      220 b- defN 23-Apr-20 16:28 xnattagger/__version__.py
+-rwxr-xr-x  2.0 unx     2178 b- defN 23-Apr-20 16:28 xnattagger-0.2.4.data/scripts/xnat_tagger.py
+-rw-r--r--  2.0 unx     1541 b- defN 23-Apr-20 16:28 xnattagger-0.2.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx      289 b- defN 23-Apr-20 16:28 xnattagger-0.2.4.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-20 16:28 xnattagger-0.2.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-20 16:28 xnattagger-0.2.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      663 b- defN 23-Apr-20 16:28 xnattagger-0.2.4.dist-info/RECORD
+8 files, 17602 bytes uncompressed, 4457 bytes compressed:  74.7%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: xnattagger/__init__.py
 Comment: 
 
 Filename: xnattagger/__version__.py
 Comment: 
 
-Filename: xnattagger-0.2.3.data/scripts/xnat_tagger.py
+Filename: xnattagger-0.2.4.data/scripts/xnat_tagger.py
 Comment: 
 
-Filename: xnattagger-0.2.3.dist-info/LICENSE
+Filename: xnattagger-0.2.4.dist-info/LICENSE
 Comment: 
 
-Filename: xnattagger-0.2.3.dist-info/METADATA
+Filename: xnattagger-0.2.4.dist-info/METADATA
 Comment: 
 
-Filename: xnattagger-0.2.3.dist-info/WHEEL
+Filename: xnattagger-0.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: xnattagger-0.2.3.dist-info/top_level.txt
+Filename: xnattagger-0.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: xnattagger-0.2.3.dist-info/RECORD
+Filename: xnattagger-0.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xnattagger/__init__.py

```diff
@@ -231,14 +231,15 @@
                 'subject': scan['subject_label'],
                 'session': session, 
                 'scan': sid,
                 'series_description': series,
                 'note': note,
                 'tag': tag
                 })
+        return updates
 
     def bold_PA(self, scans):
         updates = list()
         scans = self.filter('bold_PA')
         for i, scan in enumerate(scans, start=1):
             sid = scan['id']
             session = scan['session_label']
@@ -250,14 +251,15 @@
                 'subject': scan['subject_label'],
                 'session': session, 
                 'scan': sid,
                 'series_description': series,
                 'note': note,
                 'tag': tag
                 })
+        return updates
 
     def bold_AP(self, scans):
         updates = list()
         scans = self.filter('bold_AP')
         for i, scan in enumerate(scans, start=1):
             sid = scan['id']
             session = scan['session_label']
@@ -269,14 +271,15 @@
                 'subject': scan['subject_label'],
                 'session': session, 
                 'scan': sid,
                 'series_description': series,
                 'note': note,
                 'tag': tag
                 })
+        return updates
 
     def upsert(self, confirm=True):
         updates = list(self._squeeze(self.updates))
         for scan in self.scans:
             sid = scan['id']
             note = scan['note']
             update = [x for x in updates if x['scan'] == sid]
@@ -340,8 +343,8 @@
                     fo.write(json.dumps(self.scans, indent=2))
         else:
             logger.info(f'cache hit {cachefile}')
             with open(cachefile) as fo:
                 self.scans = json.loads(fo.read())
 
 class BadArgumentError(Exception):
-    pass(yaxil)
+    pass
```

## xnattagger/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'xnattagger'
 __description__ = 'XNAT Tagger'
 __url__ = 'https://github.com/harvard-nrg/xnattagger'
-__version__ = '0.2.3'
+__version__ = '0.2.4'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## Comparing `xnattagger-0.2.3.data/scripts/xnat_tagger.py` & `xnattagger-0.2.4.data/scripts/xnat_tagger.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     parser.add_argument('-o', '--output-file',
         help='Output summary of updates')  # Provide help text for output-file argument
     parser.add_argument('--dry-run', action='store_true',
         help='Do not execute updates')  # Provide help text for dry-run argument
     parser.add_argument('--confirm', action='store_true',
         help='Prompt user to confirm every update')  # Provide help text for confirm argument
     parser.add_argument('--filters', required=True,
-        help='Filters configuration output_file') 
+        help='Filters configuration file') 
     parser.add_argument('--target', choices=['t1', 't2', 'dwi', 'bold', 'all'], required=True, type=str.lower) # Require --target argument
     parser.add_argument('session')  # Require session argument
     args = parser.parse_args()
 
     with open(args.filters) as fo:
         filters = yaml.load(fo, Loader=yaml.SafeLoader)
```

## Comparing `xnattagger-0.2.3.dist-info/LICENSE` & `xnattagger-0.2.4.dist-info/LICENSE`

 * *Files identical despite different names*

