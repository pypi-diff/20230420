# Comparing `tmp/thronescli-2.6.0-py3-none-any.whl.zip` & `tmp/thronescli-2.6.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 9732 bytes, number of entries: 8
+Zip file size: 9731 bytes, number of entries: 8
 -rw-r--r--  2.0 unx        0 b- defN 22-Oct-11 08:00 thronescli/__init__.py
--rw-r--r--  2.0 unx    34519 b- defN 23-Jan-05 16:20 thronescli/thronescli.py
--rw-r--r--  2.0 unx       28 b- defN 23-Jan-05 16:21 thronescli-2.6.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      400 b- defN 23-Jan-05 16:21 thronescli-2.6.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-05 16:21 thronescli-2.6.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       58 b- defN 23-Jan-05 16:21 thronescli-2.6.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-Jan-05 16:21 thronescli-2.6.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      658 b- defN 23-Jan-05 16:21 thronescli-2.6.0.dist-info/RECORD
-8 files, 35766 bytes uncompressed, 8568 bytes compressed:  76.0%
+-rw-r--r--  2.0 unx    34519 b- defN 23-Apr-20 11:38 thronescli/thronescli.py
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-20 11:39 thronescli-2.6.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      400 b- defN 23-Apr-20 11:39 thronescli-2.6.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-20 11:39 thronescli-2.6.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       58 b- defN 23-Apr-20 11:39 thronescli-2.6.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-20 11:39 thronescli-2.6.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      658 b- defN 23-Apr-20 11:39 thronescli-2.6.1.dist-info/RECORD
+8 files, 35766 bytes uncompressed, 8567 bytes compressed:  76.0%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: thronescli/__init__.py
 Comment: 
 
 Filename: thronescli/thronescli.py
 Comment: 
 
-Filename: thronescli-2.6.0.dist-info/LICENSE.txt
+Filename: thronescli-2.6.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: thronescli-2.6.0.dist-info/METADATA
+Filename: thronescli-2.6.1.dist-info/METADATA
 Comment: 
 
-Filename: thronescli-2.6.0.dist-info/WHEEL
+Filename: thronescli-2.6.1.dist-info/WHEEL
 Comment: 
 
-Filename: thronescli-2.6.0.dist-info/entry_points.txt
+Filename: thronescli-2.6.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: thronescli-2.6.0.dist-info/top_level.txt
+Filename: thronescli-2.6.1.dist-info/top_level.txt
 Comment: 
 
-Filename: thronescli-2.6.0.dist-info/RECORD
+Filename: thronescli-2.6.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## thronescli/thronescli.py

```diff
@@ -22,15 +22,15 @@
     option,
     pass_context,
     secho,
     style,
 )
 
 
-__version__ = "2.6.0"
+__version__ = "2.6.1"
 
 
 CARDS_URL = "http://thronesdb.com/api/public/cards/"
 CARD_TYPES = ["agenda", "attachment", "character", "event", "location", "plot", "title"]
 CARD_TYPES_LOYAL = ["attachment", "character", "event", "location", "plot"]
 CARD_TYPES_UNIQUE = ["attachment", "character", "location"]
 FACTIONS = {
@@ -456,20 +456,20 @@
                 re_compile(value, flags=flags) for value in options["text_isnt"]
             )
 
 
 def preprocess_case(options):
     """Preprocess relevant options for case comparison."""
     # These options are always case insensitive
-    opts = ("trait", "trait_isnt", "set", "keyword", "keyword_isnt")
+    opts = ("set", "keyword", "keyword_isnt")
     for opt in opts:
         options[opt] = tuple(value.lower() for value in options[opt])
     if not options["case"] and not options["regex"]:
         # These options respect the case and regex options
-        opts = ("text", "text_isnt", "illustrator")
+        opts = ("text", "text_isnt", "trait", "trait_isnt", "illustrator")
         for opt in opts:
             options[opt] = tuple(value.lower() for value in options[opt])
         if options["name"]:
             options["name"] = [name.lower() for name in options["name"]]
 
 
 def preprocess_faction(options):
```

## Comparing `thronescli-2.6.0.dist-info/RECORD` & `thronescli-2.6.1.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 thronescli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-thronescli/thronescli.py,sha256=x8reTlAbJjT2vEms2Vfp8hm1_rw3fgMPx5siDkQcdqA,34519
-thronescli-2.6.0.dist-info/LICENSE.txt,sha256=gXTQQLfolayWvMUeX4r2iu0aLNmBMNGmjF0Jpfhq0ys,28
-thronescli-2.6.0.dist-info/METADATA,sha256=LPqogYZZFVQs4b_suRFtakTEMq1KDLXCqeKQ8jY31Q4,400
-thronescli-2.6.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-thronescli-2.6.0.dist-info/entry_points.txt,sha256=8PSAjgf48GZLf8bFo0SgEG7qdCoBpj7PVZWIDsHGWo8,58
-thronescli-2.6.0.dist-info/top_level.txt,sha256=yipOsDlmwLg8PxtOn7QnZ33ReRh7exKWRwIU7JdDHZk,11
-thronescli-2.6.0.dist-info/RECORD,,
+thronescli/thronescli.py,sha256=ZAeC7KwQrNE1t_QchVeUTHd5W1TtrPqZa5pWQleWh-0,34519
+thronescli-2.6.1.dist-info/LICENSE.txt,sha256=gXTQQLfolayWvMUeX4r2iu0aLNmBMNGmjF0Jpfhq0ys,28
+thronescli-2.6.1.dist-info/METADATA,sha256=ElFBpDbUar1DbAaRH2a02GzTUcl6avg-fignxxyqYTA,400
+thronescli-2.6.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+thronescli-2.6.1.dist-info/entry_points.txt,sha256=8PSAjgf48GZLf8bFo0SgEG7qdCoBpj7PVZWIDsHGWo8,58
+thronescli-2.6.1.dist-info/top_level.txt,sha256=yipOsDlmwLg8PxtOn7QnZ33ReRh7exKWRwIU7JdDHZk,11
+thronescli-2.6.1.dist-info/RECORD,,
```

