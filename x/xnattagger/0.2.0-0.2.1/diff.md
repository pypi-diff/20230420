# Comparing `tmp/xnattagger-0.2.0-py2.py3-none-any.whl.zip` & `tmp/xnattagger-0.2.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5606 bytes, number of entries: 8
--rw-r--r--  2.0 unx    12507 b- defN 23-Apr-19 19:55 xnattagger/__init__.py
--rw-r--r--  2.0 unx      220 b- defN 23-Apr-19 19:55 xnattagger/__version__.py
--rwxr-xr-x  2.0 unx     2185 b- defN 23-Apr-19 23:39 xnattagger-0.2.0.data/scripts/xnat_tagger.py
--rw-r--r--  2.0 unx     1541 b- defN 23-Apr-19 23:39 xnattagger-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      289 b- defN 23-Apr-19 23:39 xnattagger-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-19 23:39 xnattagger-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-19 23:39 xnattagger-0.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      663 b- defN 23-Apr-19 23:39 xnattagger-0.2.0.dist-info/RECORD
-8 files, 17526 bytes uncompressed, 4446 bytes compressed:  74.6%
+Zip file size: 5614 bytes, number of entries: 8
+-rw-r--r--  2.0 unx    12520 b- defN 23-Apr-20 00:40 xnattagger/__init__.py
+-rw-r--r--  2.0 unx      220 b- defN 23-Apr-20 00:40 xnattagger/__version__.py
+-rwxr-xr-x  2.0 unx     2185 b- defN 23-Apr-20 00:40 xnattagger-0.2.1.data/scripts/xnat_tagger.py
+-rw-r--r--  2.0 unx     1541 b- defN 23-Apr-20 00:40 xnattagger-0.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      289 b- defN 23-Apr-20 00:40 xnattagger-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-20 00:40 xnattagger-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-20 00:40 xnattagger-0.2.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      663 b- defN 23-Apr-20 00:40 xnattagger-0.2.1.dist-info/RECORD
+8 files, 17539 bytes uncompressed, 4454 bytes compressed:  74.6%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: xnattagger/__init__.py
 Comment: 
 
 Filename: xnattagger/__version__.py
 Comment: 
 
-Filename: xnattagger-0.2.0.data/scripts/xnat_tagger.py
+Filename: xnattagger-0.2.1.data/scripts/xnat_tagger.py
 Comment: 
 
-Filename: xnattagger-0.2.0.dist-info/LICENSE
+Filename: xnattagger-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: xnattagger-0.2.0.dist-info/METADATA
+Filename: xnattagger-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: xnattagger-0.2.0.dist-info/WHEEL
+Filename: xnattagger-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: xnattagger-0.2.0.dist-info/top_level.txt
+Filename: xnattagger-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: xnattagger-0.2.0.dist-info/RECORD
+Filename: xnattagger-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xnattagger/__init__.py

```diff
@@ -7,15 +7,15 @@
 import requests
 from yaxil.exceptions import NoExperimentsError
 
 logger = logging.getLogger()
 
 class Tagger:
     def __init__(self, auth, filters, target, session, project=None, cache=None):
-        self.auth = auth
+        self.auth = yaxil.auth(alias)
         self.filters = filters
         self.project = project
         self.cache = cache
         self.target = target 
         self.session = session
         self.updates = dict()
```

## xnattagger/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'xnattagger'
 __description__ = 'XNAT Tagger'
 __url__ = 'https://github.com/harvard-nrg/xnattagger'
-__version__ = '0.2.0'
+__version__ = '0.2.1'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## Comparing `xnattagger-0.2.0.data/scripts/xnat_tagger.py` & `xnattagger-0.2.1.data/scripts/xnat_tagger.py`

 * *Files identical despite different names*

## Comparing `xnattagger-0.2.0.dist-info/LICENSE` & `xnattagger-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `xnattagger-0.2.0.dist-info/RECORD` & `xnattagger-0.2.1.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-xnattagger/__init__.py,sha256=EQBc2YshobcGvo56V6--sUNCP7Ze2473cfWqyKzqKzQ,12507
-xnattagger/__version__.py,sha256=SoZbn4rPmikZzvVkgSS98LGZxEWNvAunL27H412fhC4,220
-xnattagger-0.2.0.data/scripts/xnat_tagger.py,sha256=T9jbTR77lAg3KEFqAGYableE1K9XNIdEky9s3Nk0qpc,2185
-xnattagger-0.2.0.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
-xnattagger-0.2.0.dist-info/METADATA,sha256=9rjUnjlz5rja0SaxjRBfciVK4yQ3rTzUlD1b9O3GRvA,289
-xnattagger-0.2.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-xnattagger-0.2.0.dist-info/top_level.txt,sha256=LdHhj5smL9uEh9HAguIPB8FH7EgYimhI-AODf4fl6tE,11
-xnattagger-0.2.0.dist-info/RECORD,,
+xnattagger/__init__.py,sha256=Tj9HvD7niq6PtPfNu2dOzK0a5Y7GK6xd1HNguRUMVhQ,12520
+xnattagger/__version__.py,sha256=sh_rE03oyl8iKBOvg-Au5x40W2VJxVFUM9HxQjsLVkU,220
+xnattagger-0.2.1.data/scripts/xnat_tagger.py,sha256=T9jbTR77lAg3KEFqAGYableE1K9XNIdEky9s3Nk0qpc,2185
+xnattagger-0.2.1.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
+xnattagger-0.2.1.dist-info/METADATA,sha256=wc6hiNCplUM-8y5KF4bJk7tdGK2MTCbUFeoj3ULUO4E,289
+xnattagger-0.2.1.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+xnattagger-0.2.1.dist-info/top_level.txt,sha256=LdHhj5smL9uEh9HAguIPB8FH7EgYimhI-AODf4fl6tE,11
+xnattagger-0.2.1.dist-info/RECORD,,
```

