# Comparing `tmp/cnd_scaffold-2.2.2-py3-none-any.whl.zip` & `tmp/cnd_scaffold-2.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4540 bytes, number of entries: 8
--rw-rw-rw-  2.0 unx        5 b- defN 23-Feb-28 15:27 cnd_scaffold/VERSION
--rw-r--r--  2.0 unx      129 b- defN 23-Feb-28 15:27 cnd_scaffold/__init__.py
--rw-r--r--  2.0 unx      121 b- defN 23-Feb-28 15:27 cnd_scaffold/__version__.py
--rw-r--r--  2.0 unx     6661 b- defN 23-Feb-28 15:27 cnd_scaffold/cnd_scaffold.py
--rw-r--r--  2.0 unx     2517 b- defN 23-Feb-28 15:27 cnd_scaffold-2.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-28 15:27 cnd_scaffold-2.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Feb-28 15:27 cnd_scaffold-2.2.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      640 b- defN 23-Feb-28 15:27 cnd_scaffold-2.2.2.dist-info/RECORD
-8 files, 10178 bytes uncompressed, 3416 bytes compressed:  66.4%
+Zip file size: 4562 bytes, number of entries: 8
+-rw-rw-rw-  2.0 unx        5 b- defN 23-Apr-19 23:20 cnd_scaffold/VERSION
+-rw-r--r--  2.0 unx      129 b- defN 23-Apr-19 23:20 cnd_scaffold/__init__.py
+-rw-r--r--  2.0 unx      121 b- defN 23-Apr-19 23:20 cnd_scaffold/__version__.py
+-rw-r--r--  2.0 unx     6764 b- defN 23-Apr-19 23:20 cnd_scaffold/cnd_scaffold.py
+-rw-r--r--  2.0 unx     2517 b- defN 23-Apr-19 23:20 cnd_scaffold-2.2.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 23:20 cnd_scaffold-2.2.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Apr-19 23:20 cnd_scaffold-2.2.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      640 b- defN 23-Apr-19 23:20 cnd_scaffold-2.2.4.dist-info/RECORD
+8 files, 10281 bytes uncompressed, 3438 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: cnd_scaffold/__version__.py
 Comment: 
 
 Filename: cnd_scaffold/cnd_scaffold.py
 Comment: 
 
-Filename: cnd_scaffold-2.2.2.dist-info/METADATA
+Filename: cnd_scaffold-2.2.4.dist-info/METADATA
 Comment: 
 
-Filename: cnd_scaffold-2.2.2.dist-info/WHEEL
+Filename: cnd_scaffold-2.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: cnd_scaffold-2.2.2.dist-info/top_level.txt
+Filename: cnd_scaffold-2.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: cnd_scaffold-2.2.2.dist-info/RECORD
+Filename: cnd_scaffold-2.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cnd_scaffold/VERSION

```diff
@@ -1 +1 @@
-2.2.2
+2.2.4
```

## cnd_scaffold/cnd_scaffold.py

```diff
@@ -59,15 +59,18 @@
 
     def _replace_default(self, item, target, content):
         files = []
         repeat = {'values': [''], 'key': ''}
         if 'repeat' in item:
             repeat = {'key': item['repeat'], 'values': self._data_to_replace[item['repeat']]}
         for value in repeat['values']:
-            global_vars = {repeat['key']: value}
+            if  value == '':
+                global_vars = self._data_to_replace
+            else:
+                global_vars = {repeat['key']: value}
             for item in self._data_to_replace:
                 if isinstance(self._data_to_replace[item], list) or isinstance(self._data_to_replace[item], dict):
                     continue
                 global_vars[item] = self._data_to_replace[item]
             file_name = self._replace_content(target, global_vars)
             file_content = self._replace_content(content, global_vars)
             if file_name.split('.')[-1] == 'yml':
```

## Comparing `cnd_scaffold-2.2.2.dist-info/METADATA` & `cnd_scaffold-2.2.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnd-scaffold
-Version: 2.2.2
+Version: 2.2.4
 Summary: Tools initiate a new project in git lab, based on a existing definition
 Home-page: https://gitlab.com/changendevops/gitopstoolkit/cnd-scaffold.git
 Author: Denis FABIEN
 Author-email: denis.fabien@changendevops.com
 License: MIT/X11
 Project-URL: Documentation, https://changendevops.com
 Project-URL: Source, https://gitlab.com/changendevops/gitopstoolkit/cnd-scaffold.git
```

## Comparing `cnd_scaffold-2.2.2.dist-info/RECORD` & `cnd_scaffold-2.2.4.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-cnd_scaffold/VERSION,sha256=SF6vF6vdEEOdWs-1Mw0SF-_AV0mJc7F8j78B1YSTd98,5
+cnd_scaffold/VERSION,sha256=IsKHmRjI0cnMOiHMCFHqQLqtYd2RRkcCylDO0IObSCQ,5
 cnd_scaffold/__init__.py,sha256=lrHENo1vmuBxM5rDVLod1IRy4vj1VkmANGW4TJxjEzA,129
 cnd_scaffold/__version__.py,sha256=H3kvuz6COTEsEmLiRYVrEExrhU4b1hgM4hWI9_yQx0g,121
-cnd_scaffold/cnd_scaffold.py,sha256=h0_gseMbw3Yy1uOT6dXKbnALxJ4sx8mGcnYqMHvLwLE,6661
-cnd_scaffold-2.2.2.dist-info/METADATA,sha256=L_VHzN5CSTD5SwbdRp0VAiOzbEA9N0rKhmb23FCQcZw,2517
-cnd_scaffold-2.2.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-cnd_scaffold-2.2.2.dist-info/top_level.txt,sha256=SSg5zF4f5c15HCseVrjsgR1pKy0NSF--6NYV7M2Q37k,13
-cnd_scaffold-2.2.2.dist-info/RECORD,,
+cnd_scaffold/cnd_scaffold.py,sha256=IQdNgFkEY_IXdTQ5avRveWsw9reb1I_z2EVWftK9_GQ,6764
+cnd_scaffold-2.2.4.dist-info/METADATA,sha256=gxcQhtroyzoWUp8OuULuNY9crG4tgFZE_eq4BdwmA1g,2517
+cnd_scaffold-2.2.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+cnd_scaffold-2.2.4.dist-info/top_level.txt,sha256=SSg5zF4f5c15HCseVrjsgR1pKy0NSF--6NYV7M2Q37k,13
+cnd_scaffold-2.2.4.dist-info/RECORD,,
```

