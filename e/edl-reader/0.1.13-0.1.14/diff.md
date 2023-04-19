# Comparing `tmp/edl_reader-0.1.13-py2.py3-none-any.whl.zip` & `tmp/edl_reader-0.1.14-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7526 bytes, number of entries: 7
+Zip file size: 7527 bytes, number of entries: 7
 -rwxrwxrwx  2.0 unx    16200 b- defN 23-Apr-19 16:08 edl/__init__.py
--rwxrwxrwx  2.0 unx       23 b- defN 23-Apr-19 21:58 edl/__version__.py
--rwxrwxrwx  2.0 unx     1094 b- defN 23-Apr-19 22:08 edl_reader-0.1.13.dist-info/LICENSE
--rwxrwxrwx  2.0 unx     3623 b- defN 23-Apr-19 22:08 edl_reader-0.1.13.dist-info/METADATA
--rwxrwxrwx  2.0 unx      110 b- defN 23-Apr-19 22:08 edl_reader-0.1.13.dist-info/WHEEL
--rwxrwxrwx  2.0 unx        4 b- defN 23-Apr-19 22:08 edl_reader-0.1.13.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      552 b- defN 23-Apr-19 22:08 edl_reader-0.1.13.dist-info/RECORD
-7 files, 21606 bytes uncompressed, 6548 bytes compressed:  69.7%
+-rwxrwxrwx  2.0 unx       23 b- defN 23-Apr-19 22:13 edl/__version__.py
+-rwxrwxrwx  2.0 unx     1094 b- defN 23-Apr-19 22:14 edl_reader-0.1.14.dist-info/LICENSE
+-rwxrwxrwx  2.0 unx     3623 b- defN 23-Apr-19 22:14 edl_reader-0.1.14.dist-info/METADATA
+-rwxrwxrwx  2.0 unx      110 b- defN 23-Apr-19 22:14 edl_reader-0.1.14.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx        4 b- defN 23-Apr-19 22:14 edl_reader-0.1.14.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      552 b- defN 23-Apr-19 22:14 edl_reader-0.1.14.dist-info/RECORD
+7 files, 21606 bytes uncompressed, 6549 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: edl/__init__.py
 Comment: 
 
 Filename: edl/__version__.py
 Comment: 
 
-Filename: edl_reader-0.1.13.dist-info/LICENSE
+Filename: edl_reader-0.1.14.dist-info/LICENSE
 Comment: 
 
-Filename: edl_reader-0.1.13.dist-info/METADATA
+Filename: edl_reader-0.1.14.dist-info/METADATA
 Comment: 
 
-Filename: edl_reader-0.1.13.dist-info/WHEEL
+Filename: edl_reader-0.1.14.dist-info/WHEEL
 Comment: 
 
-Filename: edl_reader-0.1.13.dist-info/top_level.txt
+Filename: edl_reader-0.1.14.dist-info/top_level.txt
 Comment: 
 
-Filename: edl_reader-0.1.13.dist-info/RECORD
+Filename: edl_reader-0.1.14.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## edl/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.13"
+__version__ = "0.1.14"
```

## Comparing `edl_reader-0.1.13.dist-info/LICENSE` & `edl_reader-0.1.14.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `edl_reader-0.1.13.dist-info/METADATA` & `edl_reader-0.1.14.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edl-reader
-Version: 0.1.13
+Version: 0.1.14
 Summary: Simple EDL reading library.
 Home-page: http://www.simon-hargreaves.com/python-edl
 Author: Simon Hargreaves,
 Author-email: simon@simon-hargreaves.com,
 Maintainer: CG Wire,
 Maintainer-email: evan@cg-wire.com,
 License: MIT
@@ -36,22 +36,22 @@
 Provides-Extra: lint
 Requires-Dist: black (==23.3.0) ; extra == 'lint'
 Requires-Dist: pre-commit (==3.2.2) ; extra == 'lint'
 Provides-Extra: test
 Requires-Dist: pytest ; extra == 'test'
 Requires-Dist: pytest-cov ; extra == 'test'
 
-edl-parser
+edl-reader
 ==========
 
 A python EDL (Edit Decision List) parsing library, based on the ruby EDL
 library by Julik Tarkhanov http://guerilla-di.org/edl/. Still a work in
 progress so collaboration welcome.
 
-https://github.com/cgwire/edl-parser
+https://github.com/cgwire/edl-reader
 
 Usage::
 
     from edl import Parser
     parser = Parser("23.98")
     with open("file.edl") as f:
         edl = parser.parse(f)
```

