# Comparing `tmp/nucliadb_dataset-2.7.0.post194-py3-none-any.whl.zip` & `tmp/nucliadb_dataset-2.7.0.post195-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
 Zip file size: 15795 bytes, number of entries: 15
--rw-r--r--  2.0 unx     1638 b- defN 23-Apr-19 20:57 nucliadb_dataset/__init__.py
--rw-r--r--  2.0 unx     3040 b- defN 23-Apr-19 20:57 nucliadb_dataset/api.py
--rw-r--r--  2.0 unx    16318 b- defN 23-Apr-19 20:57 nucliadb_dataset/dataset.py
--rw-r--r--  2.0 unx     2837 b- defN 23-Apr-19 20:57 nucliadb_dataset/export.py
--rw-r--r--  2.0 unx     2842 b- defN 23-Apr-19 20:57 nucliadb_dataset/mapping.py
--rw-r--r--  2.0 unx     3969 b- defN 23-Apr-19 20:57 nucliadb_dataset/nuclia.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 20:57 nucliadb_dataset/py.typed
--rw-r--r--  2.0 unx     3454 b- defN 23-Apr-19 20:57 nucliadb_dataset/run.py
--rw-r--r--  2.0 unx     2325 b- defN 23-Apr-19 20:57 nucliadb_dataset/settings.py
--rw-r--r--  2.0 unx     2410 b- defN 23-Apr-19 20:57 nucliadb_dataset/streamer.py
--rw-r--r--  2.0 unx     1274 b- defN 23-Apr-19 20:59 nucliadb_dataset-2.7.0.post194.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 20:59 nucliadb_dataset-2.7.0.post194.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 23-Apr-19 20:59 nucliadb_dataset-2.7.0.post194.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       17 b- defN 23-Apr-19 20:59 nucliadb_dataset-2.7.0.post194.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1307 b- defN 23-Apr-19 20:59 nucliadb_dataset-2.7.0.post194.dist-info/RECORD
+-rw-r--r--  2.0 unx     1638 b- defN 23-Apr-20 09:07 nucliadb_dataset/__init__.py
+-rw-r--r--  2.0 unx     3040 b- defN 23-Apr-20 09:07 nucliadb_dataset/api.py
+-rw-r--r--  2.0 unx    16318 b- defN 23-Apr-20 09:07 nucliadb_dataset/dataset.py
+-rw-r--r--  2.0 unx     2837 b- defN 23-Apr-20 09:07 nucliadb_dataset/export.py
+-rw-r--r--  2.0 unx     2842 b- defN 23-Apr-20 09:07 nucliadb_dataset/mapping.py
+-rw-r--r--  2.0 unx     3969 b- defN 23-Apr-20 09:07 nucliadb_dataset/nuclia.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-20 09:07 nucliadb_dataset/py.typed
+-rw-r--r--  2.0 unx     3454 b- defN 23-Apr-20 09:07 nucliadb_dataset/run.py
+-rw-r--r--  2.0 unx     2325 b- defN 23-Apr-20 09:07 nucliadb_dataset/settings.py
+-rw-r--r--  2.0 unx     2410 b- defN 23-Apr-20 09:07 nucliadb_dataset/streamer.py
+-rw-r--r--  2.0 unx     1274 b- defN 23-Apr-20 09:09 nucliadb_dataset-2.7.0.post195.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-20 09:09 nucliadb_dataset-2.7.0.post195.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 23-Apr-20 09:09 nucliadb_dataset-2.7.0.post195.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       17 b- defN 23-Apr-20 09:09 nucliadb_dataset-2.7.0.post195.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1307 b- defN 23-Apr-20 09:09 nucliadb_dataset-2.7.0.post195.dist-info/RECORD
 15 files, 41584 bytes uncompressed, 13605 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: nucliadb_dataset/settings.py
 Comment: 
 
 Filename: nucliadb_dataset/streamer.py
 Comment: 
 
-Filename: nucliadb_dataset-2.7.0.post194.dist-info/METADATA
+Filename: nucliadb_dataset-2.7.0.post195.dist-info/METADATA
 Comment: 
 
-Filename: nucliadb_dataset-2.7.0.post194.dist-info/WHEEL
+Filename: nucliadb_dataset-2.7.0.post195.dist-info/WHEEL
 Comment: 
 
-Filename: nucliadb_dataset-2.7.0.post194.dist-info/entry_points.txt
+Filename: nucliadb_dataset-2.7.0.post195.dist-info/entry_points.txt
 Comment: 
 
-Filename: nucliadb_dataset-2.7.0.post194.dist-info/top_level.txt
+Filename: nucliadb_dataset-2.7.0.post195.dist-info/top_level.txt
 Comment: 
 
-Filename: nucliadb_dataset-2.7.0.post194.dist-info/RECORD
+Filename: nucliadb_dataset-2.7.0.post195.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nucliadb_dataset/dataset.py

```diff
@@ -164,15 +164,15 @@
 
             else:
                 raise KeyError("Not a valid task")
         elif trainset is None and task is None:
             raise AttributeError("Trainset or task needs to be defined")
 
         if trainset is None:
-            raise AttributeError("Trainset cloud not be defined")
+            raise AttributeError("Trainset could not be defined")
 
         self.trainset = trainset
         self.client = client
         self.knowledgebox = KnowledgeBox(self.client)
         self.streamer = Streamer(self.trainset, self.client)
 
         if self.trainset.type == TaskType.PARAGRAPH_CLASSIFICATION:
```

## Comparing `nucliadb_dataset-2.7.0.post194.dist-info/METADATA` & `nucliadb_dataset-2.7.0.post195.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucliadb-dataset
-Version: 2.7.0.post194
+Version: 2.7.0.post195
 Summary: NucliaDB Train Python client
 Home-page: https://github.com/nuclia/nucliadb
 Author: nucliadb Authors
 Author-email: nucliadb@nuclia.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -26,16 +26,16 @@
 Requires-Dist: boto3
 Requires-Dist: google-auth
 Requires-Dist: google-cloud-storage
 Requires-Dist: boto3-stubs
 Requires-Dist: google-auth-stubs
 Requires-Dist: types-google-cloud-ndb
 Requires-Dist: types-boto3
-Requires-Dist: nucliadb-protos (==2.7.0-post194)
-Requires-Dist: nucliadb-sdk (==2.7.0-post194)
+Requires-Dist: nucliadb-protos (==2.7.0-post195)
+Requires-Dist: nucliadb-sdk (==2.7.0-post195)
 
 # NUCLIADB TRAIN CLIENT
 
 Library to connect NucliaDB to Training APIs
 
 ## INSTALL
```

## Comparing `nucliadb_dataset-2.7.0.post194.dist-info/RECORD` & `nucliadb_dataset-2.7.0.post195.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 nucliadb_dataset/__init__.py,sha256=1xWjTkFCocGr2kNaP3phSsh5Q-V1uEBYCe6ESeeCyxo,1638
 nucliadb_dataset/api.py,sha256=PbOwmD_ZP6jO78cOwyaSoONxCYKG5C-AFHD4uOcAcMY,3040
-nucliadb_dataset/dataset.py,sha256=7S8aLjhyIK5q4YRpLYyfOpqEkFlkpR1c5WDGEhxR0ig,16318
+nucliadb_dataset/dataset.py,sha256=uN7U2SLQ4OuDsJ_xDiAeJCIn6dD-1ZQ5SCQMgqVwBG8,16318
 nucliadb_dataset/export.py,sha256=Y0vvLs8c7Wou70_hs51QgMIUfcIxVxng9PWSafvF9yg,2837
 nucliadb_dataset/mapping.py,sha256=QXWqNiM23UrIufNmoCJLBbsqLR5ZPUHK7utHQac3OeE,2842
 nucliadb_dataset/nuclia.py,sha256=U47IZuaDEtpDtAE_4-C3ChsOG8NDJ55MVDTyXaJZI8M,3969
 nucliadb_dataset/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nucliadb_dataset/run.py,sha256=Rqxn4PeE9p8eev8HMtuli7l_ZYXGOWzV1yzh3Oqdr_4,3454
 nucliadb_dataset/settings.py,sha256=2cBWjTf6LnJ9TSHcalpRPcS_P5ofGmYiirdCqJl28go,2325
 nucliadb_dataset/streamer.py,sha256=ufa-crVmfLiW123JQQBi7UGusOdB_2lgL0YzVXqbzP4,2410
-nucliadb_dataset-2.7.0.post194.dist-info/METADATA,sha256=E3FHyLzCtyOyN1Alf6-umTQvBRvF_188ZnqL3X1_TCg,1274
-nucliadb_dataset-2.7.0.post194.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-nucliadb_dataset-2.7.0.post194.dist-info/entry_points.txt,sha256=Sxj3LTMMj6lcS_C3I3Ke4R2vFTngQUL7opC0RQJ1qIc,61
-nucliadb_dataset-2.7.0.post194.dist-info/top_level.txt,sha256=aJtDe54tz6060E0uyk1rdTRAU4FPWo5if1fYFQGvdqU,17
-nucliadb_dataset-2.7.0.post194.dist-info/RECORD,,
+nucliadb_dataset-2.7.0.post195.dist-info/METADATA,sha256=OW7nwM8Y0PCLi2Byqn7SqefbyFA7lRwQL6Q7UUm-lg8,1274
+nucliadb_dataset-2.7.0.post195.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+nucliadb_dataset-2.7.0.post195.dist-info/entry_points.txt,sha256=Sxj3LTMMj6lcS_C3I3Ke4R2vFTngQUL7opC0RQJ1qIc,61
+nucliadb_dataset-2.7.0.post195.dist-info/top_level.txt,sha256=aJtDe54tz6060E0uyk1rdTRAU4FPWo5if1fYFQGvdqU,17
+nucliadb_dataset-2.7.0.post195.dist-info/RECORD,,
```

