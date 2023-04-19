# Comparing `tmp/neon_speech-3.2.2a0-py3-none-any.whl.zip` & `tmp/neon_speech-3.2.2a2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 23520 bytes, number of entries: 14
--rw-r--r--  2.0 unx     1831 b- defN 23-Apr-12 01:13 neon_speech/__init__.py
--rw-r--r--  2.0 unx     2632 b- defN 23-Apr-12 01:13 neon_speech/__main__.py
--rw-r--r--  2.0 unx     5085 b- defN 23-Apr-12 01:13 neon_speech/cli.py
--rw-r--r--  2.0 unx     9996 b- defN 23-Apr-12 01:13 neon_speech/listener.py
--rw-r--r--  2.0 unx     4810 b- defN 23-Apr-12 01:13 neon_speech/mic.py
--rw-r--r--  2.0 unx    21797 b- defN 23-Apr-12 01:13 neon_speech/service.py
--rw-r--r--  2.0 unx     4396 b- defN 23-Apr-12 01:13 neon_speech/stt.py
--rw-r--r--  2.0 unx     4294 b- defN 23-Apr-12 01:13 neon_speech/utils.py
--rw-r--r--  2.0 unx     1634 b- defN 23-Apr-12 01:13 neon_speech-3.2.2a0.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     2551 b- defN 23-Apr-12 01:13 neon_speech-3.2.2a0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 01:13 neon_speech-3.2.2a0.dist-info/WHEEL
--rw-r--r--  2.0 unx      111 b- defN 23-Apr-12 01:13 neon_speech-3.2.2a0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-12 01:13 neon_speech-3.2.2a0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1143 b- defN 23-Apr-12 01:13 neon_speech-3.2.2a0.dist-info/RECORD
-14 files, 60384 bytes uncompressed, 21628 bytes compressed:  64.2%
+Zip file size: 23535 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     1831 b- defN 23-Apr-19 22:25 neon_speech/__init__.py
+-rw-r--r--  2.0 unx     2632 b- defN 23-Apr-19 22:25 neon_speech/__main__.py
+-rw-r--r--  2.0 unx     5085 b- defN 23-Apr-19 22:25 neon_speech/cli.py
+-rw-r--r--  2.0 unx     9996 b- defN 23-Apr-19 22:25 neon_speech/listener.py
+-rw-r--r--  2.0 unx     4810 b- defN 23-Apr-19 22:25 neon_speech/mic.py
+-rw-r--r--  2.0 unx    21837 b- defN 23-Apr-19 22:25 neon_speech/service.py
+-rw-r--r--  2.0 unx     4396 b- defN 23-Apr-19 22:25 neon_speech/stt.py
+-rw-r--r--  2.0 unx     4294 b- defN 23-Apr-19 22:25 neon_speech/utils.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-Apr-19 22:25 neon_speech-3.2.2a2.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     2551 b- defN 23-Apr-19 22:25 neon_speech-3.2.2a2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 22:25 neon_speech-3.2.2a2.dist-info/WHEEL
+-rw-r--r--  2.0 unx      111 b- defN 23-Apr-19 22:25 neon_speech-3.2.2a2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-Apr-19 22:25 neon_speech-3.2.2a2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1143 b- defN 23-Apr-19 22:25 neon_speech-3.2.2a2.dist-info/RECORD
+14 files, 60424 bytes uncompressed, 21643 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: neon_speech/stt.py
 Comment: 
 
 Filename: neon_speech/utils.py
 Comment: 
 
-Filename: neon_speech-3.2.2a0.dist-info/LICENSE.md
+Filename: neon_speech-3.2.2a2.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_speech-3.2.2a0.dist-info/METADATA
+Filename: neon_speech-3.2.2a2.dist-info/METADATA
 Comment: 
 
-Filename: neon_speech-3.2.2a0.dist-info/WHEEL
+Filename: neon_speech-3.2.2a2.dist-info/WHEEL
 Comment: 
 
-Filename: neon_speech-3.2.2a0.dist-info/entry_points.txt
+Filename: neon_speech-3.2.2a2.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_speech-3.2.2a0.dist-info/top_level.txt
+Filename: neon_speech-3.2.2a2.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_speech-3.2.2a0.dist-info/RECORD
+Filename: neon_speech-3.2.2a2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neon_speech/service.py

```diff
@@ -391,15 +391,15 @@
     def handle_internet_connected(self, _):
         """
         Handle notification from core that internet connection is established
         """
         if self.loop.stt.config["module"] != self.config["stt"]["module"]:
             LOG.info("Reloading STT module")
             self.loop.stt = STTFactory.create()
-        else:
+        elif hasattr(self.loop.stt, "results_event"):
             LOG.info(f"Internet Connected, Resetting STT Stream")
             self.loop.stt.results_event.set()
 
     def handle_offline(self, _):
         """
         Handle notification to operate in offline mode
         """
```

## Comparing `neon_speech-3.2.2a0.dist-info/LICENSE.md` & `neon_speech-3.2.2a2.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_speech-3.2.2a0.dist-info/METADATA` & `neon_speech-3.2.2a2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-speech
-Version: 3.2.2a0
+Version: 3.2.2a2
 Summary: Neon Speech Module
 Home-page: https://github.com/NeonGeckoCom/neon_speech
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

## Comparing `neon_speech-3.2.2a0.dist-info/RECORD` & `neon_speech-3.2.2a2.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 neon_speech/__init__.py,sha256=UDwbScPcnqA05m_zQmXnY6YeoL5j6NS_TaLj0mQdU_8,1831
 neon_speech/__main__.py,sha256=GYsKldh4iN7sY2kLnHtSYj1D56GQgdHuMXlUIf-d5ks,2632
 neon_speech/cli.py,sha256=2BiU-fTcmOyT3CJ6gmoCtUsP7bAUcDOt8-MkPEfMJX0,5085
 neon_speech/listener.py,sha256=Cct3GOVTrjEBUBq2pvrcDH7iixBo_6jvJCV02BeCwNE,9996
 neon_speech/mic.py,sha256=gcarKLkWfrzToACsiwRWDX5qeBizyJ0vquuqdg5EMeU,4810
-neon_speech/service.py,sha256=SXldmfNWkFVUaZnV_EG-3rxgeKQRXPxvjByclEzkjEs,21797
+neon_speech/service.py,sha256=oLQ7978avvH4eGbUFWSIV1ylWFvxh7Td1UUloMKYLrk,21837
 neon_speech/stt.py,sha256=rCl2v2m1D1-t-92Me1qyA57gfw7i9jSzs7j0bQXTGOc,4396
 neon_speech/utils.py,sha256=5RNtze-kwo-_WvYNk8GoqG8vVdkbPs6hBdpF7Pn7Iqc,4294
-neon_speech-3.2.2a0.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
-neon_speech-3.2.2a0.dist-info/METADATA,sha256=1LiMMFGLJ9tXofZpZH-5_16S6i44Vd1N71oiX3bEgU4,2551
-neon_speech-3.2.2a0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-neon_speech-3.2.2a0.dist-info/entry_points.txt,sha256=Y5nCn6RrdZVozA3UnFkIX_43MJ5TF-bmlqsz3LA_9rM,111
-neon_speech-3.2.2a0.dist-info/top_level.txt,sha256=fXNizEfCNvNDWenv5znkv_2KPpvzwwsRM7S3sG7bllw,12
-neon_speech-3.2.2a0.dist-info/RECORD,,
+neon_speech-3.2.2a2.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
+neon_speech-3.2.2a2.dist-info/METADATA,sha256=Oz2yZgJFRXkJEzZo-K3bCaY43vgJt233wKlsfB5ClfE,2551
+neon_speech-3.2.2a2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+neon_speech-3.2.2a2.dist-info/entry_points.txt,sha256=Y5nCn6RrdZVozA3UnFkIX_43MJ5TF-bmlqsz3LA_9rM,111
+neon_speech-3.2.2a2.dist-info/top_level.txt,sha256=fXNizEfCNvNDWenv5znkv_2KPpvzwwsRM7S3sG7bllw,12
+neon_speech-3.2.2a2.dist-info/RECORD,,
```

