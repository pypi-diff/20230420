# Comparing `tmp/liebre-2.2304.1-py3-none-any.whl.zip` & `tmp/liebre-2.2304.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 19957 bytes, number of entries: 13
--rw-rw-r--  2.0 unx      222 b- defN 23-Apr-19 21:05 liebre/__init__.py
+Zip file size: 19977 bytes, number of entries: 13
+-rw-rw-r--  2.0 unx      222 b- defN 23-Apr-20 10:18 liebre/__init__.py
 -rw-rw-r--  2.0 unx     8079 b- defN 23-Apr-19 20:41 liebre/consumer.py
 -rw-rw-r--  2.0 unx       46 b- defN 22-Dec-07 11:43 liebre/liebre.py
 -rw-rw-r--  2.0 unx       69 b- defN 22-Dec-07 11:44 liebre/logger.py
 -rw-rw-r--  2.0 unx      490 b- defN 23-Apr-19 20:41 liebre/message.py
 -rw-rw-r--  2.0 unx     2535 b- defN 23-Jan-17 11:16 liebre/producer.py
--rw-rw-r--  2.0 unx     7402 b- defN 23-Jan-30 23:35 liebre/rabbit_store.py
+-rw-rw-r--  2.0 unx     7439 b- defN 23-Apr-20 10:16 liebre/rabbit_store.py
 -rw-rw-r--  2.0 unx     1254 b- defN 23-Apr-19 21:05 liebre/utils.py
--rw-rw-r--  2.0 unx    35149 b- defN 23-Apr-19 21:05 liebre-2.2304.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx      730 b- defN 23-Apr-19 21:05 liebre-2.2304.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-19 21:05 liebre-2.2304.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Apr-19 21:05 liebre-2.2304.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      985 b- defN 23-Apr-19 21:05 liebre-2.2304.1.dist-info/RECORD
-13 files, 57060 bytes uncompressed, 18329 bytes compressed:  67.9%
+-rw-rw-r--  2.0 unx    35149 b- defN 23-Apr-20 10:18 liebre-2.2304.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      730 b- defN 23-Apr-20 10:18 liebre-2.2304.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-20 10:18 liebre-2.2304.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-20 10:18 liebre-2.2304.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      985 b- defN 23-Apr-20 10:18 liebre-2.2304.2.dist-info/RECORD
+13 files, 57097 bytes uncompressed, 18349 bytes compressed:  67.9%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: liebre/rabbit_store.py
 Comment: 
 
 Filename: liebre/utils.py
 Comment: 
 
-Filename: liebre-2.2304.1.dist-info/LICENSE
+Filename: liebre-2.2304.2.dist-info/LICENSE
 Comment: 
 
-Filename: liebre-2.2304.1.dist-info/METADATA
+Filename: liebre-2.2304.2.dist-info/METADATA
 Comment: 
 
-Filename: liebre-2.2304.1.dist-info/WHEEL
+Filename: liebre-2.2304.2.dist-info/WHEEL
 Comment: 
 
-Filename: liebre-2.2304.1.dist-info/top_level.txt
+Filename: liebre-2.2304.2.dist-info/top_level.txt
 Comment: 
 
-Filename: liebre-2.2304.1.dist-info/RECORD
+Filename: liebre-2.2304.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## liebre/__init__.py

```diff
@@ -2,10 +2,10 @@
 # -*- coding: utf-8 -*-
 
 from .consumer import Consumer  # noqa F401
 from .producer import Producer  # noqa F401
 
 import logging
 
-__version__ = '2.2304.1'
+__version__ = '2.2304.2'
 
 logging.getLogger('pika').propagate = False
```

## liebre/rabbit_store.py

```diff
@@ -107,25 +107,25 @@
                     logger.warning(
                         'Reconnecting... '
                         f'({retries}/{instance._max_retries})',
                         error=error
                     )
 
                     try:
-                        instance.connect()
+                        instance.connect(force=True)
                     except Exception:
                         logger.exception(
                             'Reconnecting... '
                             f'({retries}/{instance._max_retries})',
                         )
 
         return _
 
-    def connect(self):
-        if self._initialized:
+    def connect(self, force=False):
+        if not force and self._initialized:
             return
 
         self._channel = self._get_channel()
         self._declare_exchange()
 
         self._initialized = True
```

## Comparing `liebre-2.2304.1.dist-info/LICENSE` & `liebre-2.2304.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `liebre-2.2304.1.dist-info/METADATA` & `liebre-2.2304.2.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liebre
-Version: 2.2304.1
+Version: 2.2304.2
 Home-page: https://github.com/councilbox/liebre-python
 Author: 
 Author-email: 
 License: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

## Comparing `liebre-2.2304.1.dist-info/RECORD` & `liebre-2.2304.2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-liebre/__init__.py,sha256=FJcVwHo_HKjyOxjPJn2LJ3fDrbkXkIBVfsVtfsf08NU,222
+liebre/__init__.py,sha256=ws6m9vNPcOZZQVUj0wumf5Nqf48uGDaKUjHcbmZ_kJQ,222
 liebre/consumer.py,sha256=x9QjvEKackueBYGkNohW1MO9Ld4Nty5xaVNWycqfyQE,8079
 liebre/liebre.py,sha256=FZk9hm7vBsK8G16pNugputbrrEciYqJc_XRAhTCcojI,46
 liebre/logger.py,sha256=gFdT_UHqta9GXzzGK44_sDagnInpWDLKXDJ3J4ZJkmc,69
 liebre/message.py,sha256=LsyOktRKgYOs5FzllpmfuoWWKM8t9mB7-OSRFVnjXxE,490
 liebre/producer.py,sha256=P3pM3PWePHbMKj3BPGvFgCaT_lrJS336GyHREYmyx0M,2535
-liebre/rabbit_store.py,sha256=1PHFx6PlDLyZHRiCCkHGLO6fT3M3ofjXV-9ihV0Hxyk,7402
+liebre/rabbit_store.py,sha256=ZR2kZgkXtVQkO6-B4D6joG2bWxjzwVyig_0w0cZmarI,7439
 liebre/utils.py,sha256=R5guDu_P0auv2pLxW9OmXOzC5dQ1snIt5rQz2lX3LEg,1254
-liebre-2.2304.1.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-liebre-2.2304.1.dist-info/METADATA,sha256=u-smip9aRUuID7qICFQmyW6v77zBMfqZTdNND6lVEpk,730
-liebre-2.2304.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-liebre-2.2304.1.dist-info/top_level.txt,sha256=cl5ALalM53myFXDcFp7jtynIzvwoKF4RqF1x1Aw4WwY,7
-liebre-2.2304.1.dist-info/RECORD,,
+liebre-2.2304.2.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+liebre-2.2304.2.dist-info/METADATA,sha256=wA6iovBuHx-d6aFYYvmrIP0VXI9vyIT29hWzR3Pj07A,730
+liebre-2.2304.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+liebre-2.2304.2.dist-info/top_level.txt,sha256=cl5ALalM53myFXDcFp7jtynIzvwoKF4RqF1x1Aw4WwY,7
+liebre-2.2304.2.dist-info/RECORD,,
```

