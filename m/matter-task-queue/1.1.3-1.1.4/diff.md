# Comparing `tmp/matter_task_queue-1.1.3-py3-none-any.whl.zip` & `tmp/matter_task_queue-1.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8740 bytes, number of entries: 10
+Zip file size: 8737 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      134 b- defN 20-Feb-02 00:00 matter_task_queue/__about__.py
 -rw-r--r--  2.0 unx      353 b- defN 20-Feb-02 00:00 matter_task_queue/__init__.py
 -rw-r--r--  2.0 unx     1228 b- defN 20-Feb-02 00:00 matter_task_queue/base_task.py
 -rw-r--r--  2.0 unx     3862 b- defN 20-Feb-02 00:00 matter_task_queue/celery_config.py
--rw-r--r--  2.0 unx      901 b- defN 20-Feb-02 00:00 matter_task_queue/config.py
+-rw-r--r--  2.0 unx      843 b- defN 20-Feb-02 00:00 matter_task_queue/config.py
 -rw-r--r--  2.0 unx     3232 b- defN 20-Feb-02 00:00 matter_task_queue/utils.py
-?rw-r--r--  2.0 unx     4757 b- defN 20-Feb-02 00:00 matter_task_queue-1.1.3.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 matter_task_queue-1.1.3.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1068 b- defN 20-Feb-02 00:00 matter_task_queue-1.1.3.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      858 b- defN 20-Feb-02 00:00 matter_task_queue-1.1.3.dist-info/RECORD
-10 files, 16480 bytes uncompressed, 7264 bytes compressed:  55.9%
+?rw-r--r--  2.0 unx     4757 b- defN 20-Feb-02 00:00 matter_task_queue-1.1.4.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 matter_task_queue-1.1.4.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1068 b- defN 20-Feb-02 00:00 matter_task_queue-1.1.4.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      858 b- defN 20-Feb-02 00:00 matter_task_queue-1.1.4.dist-info/RECORD
+10 files, 16422 bytes uncompressed, 7261 bytes compressed:  55.8%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: matter_task_queue/config.py
 Comment: 
 
 Filename: matter_task_queue/utils.py
 Comment: 
 
-Filename: matter_task_queue-1.1.3.dist-info/METADATA
+Filename: matter_task_queue-1.1.4.dist-info/METADATA
 Comment: 
 
-Filename: matter_task_queue-1.1.3.dist-info/WHEEL
+Filename: matter_task_queue-1.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: matter_task_queue-1.1.3.dist-info/licenses/LICENSE
+Filename: matter_task_queue-1.1.4.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: matter_task_queue-1.1.3.dist-info/RECORD
+Filename: matter_task_queue-1.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## matter_task_queue/__about__.py

```diff
@@ -1,4 +1,4 @@
 # SPDX-FileCopyrightText: 2023-present Rômulo Jales <romulo@thisismatter.com>
 #
 # SPDX-License-Identifier: MIT
-__version__ = "1.1.3"
+__version__ = "1.1.4"
```

## matter_task_queue/config.py

```diff
@@ -12,13 +12,12 @@
         cls.DEBUG = os.getenv("DEBUG", "false").lower() == "true"
 
         cls.INSTANCE_NAME = os.environ["INSTANCE_NAME"]
         cls.AWS_REGION = os.getenv("AWS_REGION", "eu-central-1")
         cls.CELERY_LOG_LEVEL = os.environ.get("CELERY_LOG_LEVEL", "INFO").upper()
         cls.CELERY_LOG_FILE_PATH = os.getenv("CELERY_LOG_FILE_PATH", "/tmp/celery.txt")
         cls.SENTRY_DSN = os.getenv("SENTRY_DSN")
-
-        cls.AWS_ENDPOINT_URL = os.environ["AWS_ENDPOINT_URL"] if cls.ENV != "test" else os.getenv("AWS_ENDPOINT_URL")
+        cls.AWS_ENDPOINT_URL = os.getenv("AWS_ENDPOINT_URL")
         cls.CELERY_BROKER_URL = os.environ["CELERY_BROKER_URL"] if cls.ENV != "test" else os.getenv("CELERY_BROKER_URL")
 
 
 Config()
```

## Comparing `matter_task_queue-1.1.3.dist-info/METADATA` & `matter_task_queue-1.1.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matter-task-queue
-Version: 1.1.3
+Version: 1.1.4
 Summary: A template for new Matter's library
 Project-URL: Documentation, https://github.com/Matter-Tech/matter-task-queue#readme
 Project-URL: Issues, https://github.com/Matter-Tech/matter-task-queue/issues
 Project-URL: Source, https://github.com/Matter-Tech/matter-task-queue
 Author-email: Tomer Sasson <tomer@thisismatter.com>
 License-Expression: MIT
 License-File: LICENSE
```

## Comparing `matter_task_queue-1.1.3.dist-info/licenses/LICENSE` & `matter_task_queue-1.1.4.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `matter_task_queue-1.1.3.dist-info/RECORD` & `matter_task_queue-1.1.4.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-matter_task_queue/__about__.py,sha256=5jZ_bunLB35tAJtOWPCPdLieY39QQan3HeQVIaOJFNk,134
+matter_task_queue/__about__.py,sha256=WOh1xF9ccUiVsppwx5CE-CJV7Ep5icyBwKtPmcCrLGU,134
 matter_task_queue/__init__.py,sha256=VZQFnoZIVpJBsw_NI3KOJxuShkSuzedEMIm3x0ZSE4M,353
 matter_task_queue/base_task.py,sha256=6J-CkaNo3PoERYwfcq2N6WKvUkm7eE1ZtGqqv9ms7nk,1228
 matter_task_queue/celery_config.py,sha256=651NRkHE1CeVETvAG4TCmJFKygj_gLveCxUrAyZMVOQ,3862
-matter_task_queue/config.py,sha256=1SZH75s5HGu7CcQKqGVxLuVwRR8L61MSIycMpy9daBM,901
+matter_task_queue/config.py,sha256=QDrbfX2XClj04xwCd_ooxyqcBKcwpn0K7X-SUnAv-pM,843
 matter_task_queue/utils.py,sha256=V5vlCW39lRJvorJka7kAAt2IRSebgmAGVXydOYHwdQ0,3232
-matter_task_queue-1.1.3.dist-info/METADATA,sha256=uLCJbIuioKS2W_MSpn4GU9U1g-nlAkl_cUtg8-N023Q,4757
-matter_task_queue-1.1.3.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
-matter_task_queue-1.1.3.dist-info/licenses/LICENSE,sha256=bqRY4B_u4xSKzKFb3ML8l0nCWvMXyzEGwY2B2hteV8g,1068
-matter_task_queue-1.1.3.dist-info/RECORD,,
+matter_task_queue-1.1.4.dist-info/METADATA,sha256=C19VQ3yZ1y_phE2xAHYJqemuCB3Eml5hjXCMbpm8FZI,4757
+matter_task_queue-1.1.4.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
+matter_task_queue-1.1.4.dist-info/licenses/LICENSE,sha256=bqRY4B_u4xSKzKFb3ML8l0nCWvMXyzEGwY2B2hteV8g,1068
+matter_task_queue-1.1.4.dist-info/RECORD,,
```

