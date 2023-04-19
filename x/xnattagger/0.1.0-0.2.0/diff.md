# Comparing `tmp/xnattagger-0.1.0-py2.py3-none-any.whl.zip` & `tmp/xnattagger-0.2.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5511 bytes, number of entries: 8
--rw-r--r--  2.0 unx    10267 b- defN 23-Apr-13 19:31 xnattagger/__init__.py
--rw-r--r--  2.0 unx      220 b- defN 23-Apr-13 19:31 xnattagger/__version__.py
--rwxr-xr-x  2.0 unx     2177 b- defN 23-Apr-13 19:37 xnattagger-0.1.0.data/scripts/xnat_tagger.py
--rw-r--r--  2.0 unx     1541 b- defN 23-Apr-13 19:37 xnattagger-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      289 b- defN 23-Apr-13 19:37 xnattagger-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-13 19:37 xnattagger-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-13 19:37 xnattagger-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      663 b- defN 23-Apr-13 19:37 xnattagger-0.1.0.dist-info/RECORD
-8 files, 15278 bytes uncompressed, 4351 bytes compressed:  71.5%
+Zip file size: 5606 bytes, number of entries: 8
+-rw-r--r--  2.0 unx    12507 b- defN 23-Apr-19 19:55 xnattagger/__init__.py
+-rw-r--r--  2.0 unx      220 b- defN 23-Apr-19 19:55 xnattagger/__version__.py
+-rwxr-xr-x  2.0 unx     2185 b- defN 23-Apr-19 23:39 xnattagger-0.2.0.data/scripts/xnat_tagger.py
+-rw-r--r--  2.0 unx     1541 b- defN 23-Apr-19 23:39 xnattagger-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      289 b- defN 23-Apr-19 23:39 xnattagger-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-19 23:39 xnattagger-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-19 23:39 xnattagger-0.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      663 b- defN 23-Apr-19 23:39 xnattagger-0.2.0.dist-info/RECORD
+8 files, 17526 bytes uncompressed, 4446 bytes compressed:  74.6%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: xnattagger/__init__.py
 Comment: 
 
 Filename: xnattagger/__version__.py
 Comment: 
 
-Filename: xnattagger-0.1.0.data/scripts/xnat_tagger.py
+Filename: xnattagger-0.2.0.data/scripts/xnat_tagger.py
 Comment: 
 
-Filename: xnattagger-0.1.0.dist-info/LICENSE
+Filename: xnattagger-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: xnattagger-0.1.0.dist-info/METADATA
+Filename: xnattagger-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: xnattagger-0.1.0.dist-info/WHEEL
+Filename: xnattagger-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: xnattagger-0.1.0.dist-info/top_level.txt
+Filename: xnattagger-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: xnattagger-0.1.0.dist-info/RECORD
+Filename: xnattagger-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xnattagger/__init__.py

```diff
@@ -32,15 +32,21 @@
                 't1w': self.t1w(self.scans),  # Generate updates for T1w scan(s)
                 't1w_move': self.t1w_move(self.scans)  # Generate updates for T1w_MOVE scan(s)
             })
         elif self.target == 't2':
             self.updates.update({
                 't2w': self.t2w(self.scans),  # Generate updates for T2w scan(s)
                 't2w_move': self.t2w_move(self.scans)  # Generate updates for T2w_MOVE scan(s)
-            })  
+            })
+        elif self.target == 'bold':
+            self.updates.update({
+                'bold': self.bold(self.scans),
+                'bold_PA': self.bold_PA(self.scans),
+                'bold_AP': self.bold_AP(self.scans)
+                })
         elif self.target == 'all':
             self.updates.update({
                 't1w': self.t1w(self.scans),  # Generate updates for T1w scan(s)
                 't1w_move': self.t1w_move(self.scans),  # Generate updates for T1w_MOVE scan(s)
                 't2w': self.t2w(self.scans),  # Generate updates for T2w scan(s)
                 't2w_move': self.t2w_move(self.scans),  # Generate updates for T2w_MOVE scan(s)
                 'dwi': self.dwi(self.scans), # Generate updates for main DWI scan(s)
@@ -207,14 +213,71 @@
                 'scan': sid,
                 'series_description': series,
                 'note': note,
                 'tag': tag
                 })
         return updates
 
+    def bold(self, scans):
+        updates = list()
+        scans = self.filter('bold')
+        for i, scan in enumerate(scans, start=1):
+            sid = scan['id']
+            session = scan['session_label']
+            series = scan['series_description'].strip()
+            note = scan['note'].strip()
+            tag = f'#BOLD_{i:03}'
+            updates.append({
+                'project': scan['session_project'],
+                'subject': scan['subject_label'],
+                'session': session, 
+                'scan': sid,
+                'series_description': series,
+                'note': note,
+                'tag': tag
+                })
+
+    def bold_PA(self, scans):
+        updates = list()
+        scans = self.filter('bold_PA')
+        for i, scan in enumerate(scans, start=1):
+            sid = scan['id']
+            session = scan['session_label']
+            series = scan['series_description'].strip()
+            note = scan['note'].strip()
+            tag = f'#BOLD_PA_{i:03}'
+            updates.append({
+                'project': scan['session_project'],
+                'subject': scan['subject_label'],
+                'session': session, 
+                'scan': sid,
+                'series_description': series,
+                'note': note,
+                'tag': tag
+                })
+
+    def bold_AP(self, scans):
+        updates = list()
+        scans = self.filter('bold_AP')
+        for i, scan in enumerate(scans, start=1):
+            sid = scan['id']
+            session = scan['session_label']
+            series = scan['series_description'].strip()
+            note = scan['note'].strip()
+            tag = f'#BOLD_AP_{i:03}'
+            updates.append({
+                'project': scan['session_project'],
+                'subject': scan['subject_label'],
+                'session': session, 
+                'scan': sid,
+                'series_description': series,
+                'note': note,
+                'tag': tag
+                })
+
     def upsert(self, confirm=True):
         updates = list(self._squeeze(self.updates))
         for scan in self.scans:
             sid = scan['id']
             note = scan['note']
             update = [x for x in updates if x['scan'] == sid]
             if not update:
```

## xnattagger/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'xnattagger'
 __description__ = 'XNAT Tagger'
 __url__ = 'https://github.com/harvard-nrg/xnattagger'
-__version__ = '0.1.0'
+__version__ = '0.2.0'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## Comparing `xnattagger-0.1.0.data/scripts/xnat_tagger.py` & `xnattagger-0.2.0.data/scripts/xnat_tagger.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         help='Output summary of updates')  # Provide help text for output-file argument
     parser.add_argument('--dry-run', action='store_true',
         help='Do not execute updates')  # Provide help text for dry-run argument
     parser.add_argument('--confirm', action='store_true',
         help='Prompt user to confirm every update')  # Provide help text for confirm argument
     parser.add_argument('--filters', required=True,
         help='Filters configuration output_file') 
-    parser.add_argument('--target', choices=['t1', 't2', 'dwi', 'all'], required=True, type=str.lower) # Require --target argument
+    parser.add_argument('--target', choices=['t1', 't2', 'dwi', 'bold', 'all'], required=True, type=str.lower) # Require --target argument
     parser.add_argument('session')  # Require session argument
     args = parser.parse_args()
 
     with open(args.filters) as fo:
         filters = yaml.load(fo, Loader=yaml.SafeLoader)
 
     tagger = Tagger(args.alias, filters, args.target, args.session)
```

## Comparing `xnattagger-0.1.0.dist-info/LICENSE` & `xnattagger-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `xnattagger-0.1.0.dist-info/RECORD` & `xnattagger-0.2.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-xnattagger/__init__.py,sha256=1qfC0Ah3E9jsjThUozYljIyIqO8rEoDfIQxzYnmTHrs,10267
-xnattagger/__version__.py,sha256=rERC_LALV36jZR7rK7pqxDfiqt9LKqgodkJDo8QHD_U,220
-xnattagger-0.1.0.data/scripts/xnat_tagger.py,sha256=myknt1647R_jVVGRRXXhA8IjjNlVUpy0OVeDLQ4elp0,2177
-xnattagger-0.1.0.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
-xnattagger-0.1.0.dist-info/METADATA,sha256=qLGCPjEHZpITsTvgJGQySYhctJwdxrwi_g162TQGSL0,289
-xnattagger-0.1.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-xnattagger-0.1.0.dist-info/top_level.txt,sha256=LdHhj5smL9uEh9HAguIPB8FH7EgYimhI-AODf4fl6tE,11
-xnattagger-0.1.0.dist-info/RECORD,,
+xnattagger/__init__.py,sha256=EQBc2YshobcGvo56V6--sUNCP7Ze2473cfWqyKzqKzQ,12507
+xnattagger/__version__.py,sha256=SoZbn4rPmikZzvVkgSS98LGZxEWNvAunL27H412fhC4,220
+xnattagger-0.2.0.data/scripts/xnat_tagger.py,sha256=T9jbTR77lAg3KEFqAGYableE1K9XNIdEky9s3Nk0qpc,2185
+xnattagger-0.2.0.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
+xnattagger-0.2.0.dist-info/METADATA,sha256=9rjUnjlz5rja0SaxjRBfciVK4yQ3rTzUlD1b9O3GRvA,289
+xnattagger-0.2.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+xnattagger-0.2.0.dist-info/top_level.txt,sha256=LdHhj5smL9uEh9HAguIPB8FH7EgYimhI-AODf4fl6tE,11
+xnattagger-0.2.0.dist-info/RECORD,,
```

