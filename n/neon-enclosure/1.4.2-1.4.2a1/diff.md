# Comparing `tmp/neon_enclosure-1.4.2-py3-none-any.whl.zip` & `tmp/neon_enclosure-1.4.2a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 11975 bytes, number of entries: 12
--rw-r--r--  2.0 unx     1831 b- defN 23-Apr-20 01:35 neon_enclosure/__init__.py
--rw-r--r--  2.0 unx     2616 b- defN 23-Apr-20 01:35 neon_enclosure/__main__.py
--rw-r--r--  2.0 unx     3660 b- defN 23-Apr-20 01:35 neon_enclosure/service.py
--rw-r--r--  2.0 unx     1832 b- defN 23-Apr-20 01:35 neon_enclosure/admin/__init__.py
--rw-r--r--  2.0 unx     2564 b- defN 23-Apr-20 01:35 neon_enclosure/admin/__main__.py
--rw-r--r--  2.0 unx     2406 b- defN 23-Apr-20 01:35 neon_enclosure/admin/service.py
--rw-r--r--  2.0 unx     1634 b- defN 23-Apr-20 01:36 neon_enclosure-1.4.2.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     2695 b- defN 23-Apr-20 01:36 neon_enclosure-1.4.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-20 01:36 neon_enclosure-1.4.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       72 b- defN 23-Apr-20 01:36 neon_enclosure-1.4.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       15 b- defN 23-Apr-20 01:36 neon_enclosure-1.4.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1040 b- defN 23-Apr-20 01:36 neon_enclosure-1.4.2.dist-info/RECORD
-12 files, 20457 bytes uncompressed, 10209 bytes compressed:  50.1%
+Zip file size: 12009 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     1831 b- defN 23-Apr-20 01:26 neon_enclosure/__init__.py
+-rw-r--r--  2.0 unx     2616 b- defN 23-Apr-20 01:26 neon_enclosure/__main__.py
+-rw-r--r--  2.0 unx     3660 b- defN 23-Apr-20 01:26 neon_enclosure/service.py
+-rw-r--r--  2.0 unx     1832 b- defN 23-Apr-20 01:26 neon_enclosure/admin/__init__.py
+-rw-r--r--  2.0 unx     2564 b- defN 23-Apr-20 01:26 neon_enclosure/admin/__main__.py
+-rw-r--r--  2.0 unx     2406 b- defN 23-Apr-20 01:26 neon_enclosure/admin/service.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-Apr-20 01:26 neon_enclosure-1.4.2a1.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     2702 b- defN 23-Apr-20 01:26 neon_enclosure-1.4.2a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-20 01:26 neon_enclosure-1.4.2a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       71 b- defN 23-Apr-20 01:26 neon_enclosure-1.4.2a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       15 b- defN 23-Apr-20 01:26 neon_enclosure-1.4.2a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1052 b- defN 23-Apr-20 01:26 neon_enclosure-1.4.2a1.dist-info/RECORD
+12 files, 20475 bytes uncompressed, 10219 bytes compressed:  50.1%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: neon_enclosure/admin/__main__.py
 Comment: 
 
 Filename: neon_enclosure/admin/service.py
 Comment: 
 
-Filename: neon_enclosure-1.4.2.dist-info/LICENSE.md
+Filename: neon_enclosure-1.4.2a1.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_enclosure-1.4.2.dist-info/METADATA
+Filename: neon_enclosure-1.4.2a1.dist-info/METADATA
 Comment: 
 
-Filename: neon_enclosure-1.4.2.dist-info/WHEEL
+Filename: neon_enclosure-1.4.2a1.dist-info/WHEEL
 Comment: 
 
-Filename: neon_enclosure-1.4.2.dist-info/entry_points.txt
+Filename: neon_enclosure-1.4.2a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_enclosure-1.4.2.dist-info/top_level.txt
+Filename: neon_enclosure-1.4.2a1.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_enclosure-1.4.2.dist-info/RECORD
+Filename: neon_enclosure-1.4.2a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `neon_enclosure-1.4.2.dist-info/LICENSE.md` & `neon_enclosure-1.4.2a1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_enclosure-1.4.2.dist-info/METADATA` & `neon_enclosure-1.4.2a1.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: neon-enclosure
-Version: 1.4.2
+Version: 1.4.2a1
 Summary: Neon Enclosure Module
 Home-page: https://github.com/NeonGeckoCom/neon-enclosure
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
 Requires-Dist: ovos-PHAL (~=0.0.4)
 Requires-Dist: neon-utils[network] (~=1.3)
 Requires-Dist: ovos-utils[extras] (~=0.0.32)
 Requires-Dist: ovos-bus-client (~=0.0.3)
 Requires-Dist: ovos-backend-client (~=0.0.6)
 Provides-Extra: docker
 Requires-Dist: ovos-phal-plugin-homeassistant (~=0.0.1) ; extra == 'docker'
@@ -51,9 +51,7 @@
 -e PULSE_SERVER=unix:${XDG_RUNTIME_DIR}/pulse/native \
 -e PULSE_COOKIE=/home/neon/.config/pulse/cookie \
 neon_enclosure
 ```
 
 >*Note:* The above example assumes Docker data is stored in the standard user locations `~/.local/share` and `~/.config`.
 > You may want to change these values to some other path to separate container and host system data.
-
-
```

## Comparing `neon_enclosure-1.4.2.dist-info/RECORD` & `neon_enclosure-1.4.2a1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 neon_enclosure/__init__.py,sha256=UDwbScPcnqA05m_zQmXnY6YeoL5j6NS_TaLj0mQdU_8,1831
 neon_enclosure/__main__.py,sha256=pX8kUAiDtx8qCdNKSKT1LkA61R8qiu_nNC3_Qf1WWOI,2616
 neon_enclosure/service.py,sha256=ntd4ky4nfdtDEkWEKn8wRJkrqQFX1_N9l0HDXQwDcfI,3660
 neon_enclosure/admin/__init__.py,sha256=FCW9FTGwZxZm9BbxptD2ri02MXw5mq0YtuIfJ0Rm0SA,1832
 neon_enclosure/admin/__main__.py,sha256=iBkWDpV1GCLCclglNExFJguzd_Qz_C-mWLnEp1nMePE,2564
 neon_enclosure/admin/service.py,sha256=UrD0RLVFi-27A0wnFFfQjVlmo-GHWxEyma1Q0W8TLqE,2406
-neon_enclosure-1.4.2.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
-neon_enclosure-1.4.2.dist-info/METADATA,sha256=2IFILidanlGS2WcMxIEULeXeO7VSKJbzT0hu1ISGODE,2695
-neon_enclosure-1.4.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-neon_enclosure-1.4.2.dist-info/entry_points.txt,sha256=uzMIZUfekH259QhTGnvUzwqpTFXAuyDhpPRsXL-7FFs,72
-neon_enclosure-1.4.2.dist-info/top_level.txt,sha256=JyzbDWcL_LA7RBt9baW_93Ep9FDpe-ukXCsowuQm2Ug,15
-neon_enclosure-1.4.2.dist-info/RECORD,,
+neon_enclosure-1.4.2a1.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
+neon_enclosure-1.4.2a1.dist-info/METADATA,sha256=xtiOCUGPLfeJBps4HnqMmBXnGKnay-NeuMq80OZ1CSs,2702
+neon_enclosure-1.4.2a1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+neon_enclosure-1.4.2a1.dist-info/entry_points.txt,sha256=B38ve9l9IDVVfjPQFWLh0CYSoOJ454sgGWq3dfu6EPU,71
+neon_enclosure-1.4.2a1.dist-info/top_level.txt,sha256=JyzbDWcL_LA7RBt9baW_93Ep9FDpe-ukXCsowuQm2Ug,15
+neon_enclosure-1.4.2a1.dist-info/RECORD,,
```

