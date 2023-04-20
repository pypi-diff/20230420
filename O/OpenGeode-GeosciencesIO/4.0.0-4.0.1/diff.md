# Comparing `tmp/OpenGeode_GeosciencesIO-4.0.0-cp39-cp39-win_amd64.whl.zip` & `tmp/OpenGeode_GeosciencesIO-4.0.1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,13 @@
-Zip file size: 4291 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat       91 b- defN 23-Apr-14 07:16 opengeode_geosciencesio/__init__.py
--rw-rw-rw-  2.0 fat     1233 b- defN 23-Apr-14 07:16 opengeode_geosciencesio/mesh.py
--rw-rw-rw-  2.0 fat     1265 b- defN 23-Apr-14 07:16 opengeode_geosciencesio/model.py
--rw-rw-rw-  2.0 fat     3334 b- defN 23-Apr-14 07:17 OpenGeode_GeosciencesIO-4.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-14 07:17 OpenGeode_GeosciencesIO-4.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       24 b- defN 23-Apr-14 07:17 OpenGeode_GeosciencesIO-4.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      630 b- defN 23-Apr-14 07:17 OpenGeode_GeosciencesIO-4.0.0.dist-info/RECORD
-7 files, 6677 bytes uncompressed, 3157 bytes compressed:  52.7%
+Zip file size: 322084 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat       91 b- defN 23-Apr-20 08:58 opengeode_geosciencesio/__init__.py
+-rw-rw-rw-  2.0 fat     1233 b- defN 23-Apr-20 08:58 opengeode_geosciencesio/mesh.py
+-rw-rw-rw-  2.0 fat     1265 b- defN 23-Apr-20 08:58 opengeode_geosciencesio/model.py
+-rw-rw-rw-  2.0 fat   136704 b- defN 23-Apr-20 08:59 opengeode_geosciencesio/bin/OpenGeode-GeosciencesIO_mesh.dll
+-rw-rw-rw-  2.0 fat   348672 b- defN 23-Apr-20 08:59 opengeode_geosciencesio/bin/OpenGeode-GeosciencesIO_model.dll
+-rw-rw-rw-  2.0 fat   125952 b- defN 23-Apr-20 08:59 opengeode_geosciencesio/bin/opengeode_geosciencesio_py_mesh.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   125440 b- defN 23-Apr-20 08:59 opengeode_geosciencesio/bin/opengeode_geosciencesio_py_model.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     3334 b- defN 23-Apr-20 08:59 OpenGeode_GeosciencesIO-4.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-20 08:59 OpenGeode_GeosciencesIO-4.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       24 b- defN 23-Apr-20 08:59 OpenGeode_GeosciencesIO-4.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1144 b- defN 23-Apr-20 08:59 OpenGeode_GeosciencesIO-4.0.1.dist-info/RECORD
+11 files, 743959 bytes uncompressed, 320090 bytes compressed:  57.0%
```

## zipnote {}

```diff
@@ -3,20 +3,32 @@
 
 Filename: opengeode_geosciencesio/mesh.py
 Comment: 
 
 Filename: opengeode_geosciencesio/model.py
 Comment: 
 
-Filename: OpenGeode_GeosciencesIO-4.0.0.dist-info/METADATA
+Filename: opengeode_geosciencesio/bin/OpenGeode-GeosciencesIO_mesh.dll
 Comment: 
 
-Filename: OpenGeode_GeosciencesIO-4.0.0.dist-info/WHEEL
+Filename: opengeode_geosciencesio/bin/OpenGeode-GeosciencesIO_model.dll
 Comment: 
 
-Filename: OpenGeode_GeosciencesIO-4.0.0.dist-info/top_level.txt
+Filename: opengeode_geosciencesio/bin/opengeode_geosciencesio_py_mesh.cp39-win_amd64.pyd
 Comment: 
 
-Filename: OpenGeode_GeosciencesIO-4.0.0.dist-info/RECORD
+Filename: opengeode_geosciencesio/bin/opengeode_geosciencesio_py_model.cp39-win_amd64.pyd
+Comment: 
+
+Filename: OpenGeode_GeosciencesIO-4.0.1.dist-info/METADATA
+Comment: 
+
+Filename: OpenGeode_GeosciencesIO-4.0.1.dist-info/WHEEL
+Comment: 
+
+Filename: OpenGeode_GeosciencesIO-4.0.1.dist-info/top_level.txt
+Comment: 
+
+Filename: OpenGeode_GeosciencesIO-4.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `OpenGeode_GeosciencesIO-4.0.0.dist-info/METADATA` & `OpenGeode_GeosciencesIO-4.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: OpenGeode-GeosciencesIO
-Version: 4.0.0
+Version: 4.0.1
 Summary: Input/Output formats for OpenGeode-Geosciences
 Home-page: https://github.com/Geode-solutions/OpenGeode-GeosciencesIO
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Requires-Dist: opengeode-core (==14.*,>=14.0.0)
-Requires-Dist: opengeode-geosciences (==7.*,>=7.0.0)
+Requires-Dist: opengeode-core (==14.*,>=14.0.1)
+Requires-Dist: opengeode-geosciences (==7.*,>=7.0.3)
 
 <h1 align="center">OpenGeode-GeosciencesIO<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">Input/Output formats for OpenGeode-Geosciences</h3>
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/OpenGeode-GeosciencesIO/workflows/CI/badge.svg" alt="Build Status">
   <img src="https://github.com/Geode-solutions/OpenGeode-GeosciencesIO/workflows/CD/badge.svg" alt="Deploy Status">
```

### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: OpenGeode-GeosciencesIO Version: 4.0.0 Summary:
+Metadata-Version: 2.1 Name: OpenGeode-GeosciencesIO Version: 4.0.1 Summary:
 Input/Output formats for OpenGeode-Geosciences Home-page: https://github.com/
 Geode-solutions/OpenGeode-GeosciencesIO Author: Geode-solutions Author-email:
 contact@geode-solutions.com License: MIT Platform: UNKNOWN Description-Content-
-Type: text/markdown Requires-Dist: opengeode-core (==14.*,>=14.0.0) Requires-
-Dist: opengeode-geosciences (==7.*,>=7.0.0)
+Type: text/markdown Requires-Dist: opengeode-core (==14.*,>=14.0.1) Requires-
+Dist: opengeode-geosciences (==7.*,>=7.0.3)
             ****** OpenGeode-GeosciencesIOby Geode-solutions ******
            **** Input/Output formats for OpenGeode-Geosciences ****
        [Build Status] [Deploy Status] [Coverage Status] [Version] [PyPI]
              [Windows support] [Ubuntu support] [Red Hat support]
          [Language] [License] [Semantic-release] [Slack_invite] [DOI]
 --- ## Introduction OpenGeode-GeosciencesIO provides input and output formats
 for [OpenGeode-Geosciences] objects. [OpenGeode-Geosciences]: https://
```

