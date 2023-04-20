# Comparing `tmp/signal_transformation-2.4.3.tar.gz` & `tmp/signal_transformation-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/signal_transformation-2.4.3.tar", last modified: Mon May  3 11:34:52 2021, max compression
+gzip compressed data, was "signal_transformation-2.5.0.tar", last modified: Thu Apr 20 09:42:27 2023, max compression
```

## Comparing `signal_transformation-2.4.3.tar` & `signal_transformation-2.5.0.tar`

### file list

```diff
@@ -1,29 +1,37 @@
-drwxr-xr-x   0 ivanov     (501) staff       (20)        0 2021-05-03 11:34:52.351858 signal_transformation-2.4.3/
--rw-r--r--   0 ivanov     (501) staff       (20)      621 2021-05-03 11:34:52.351611 signal_transformation-2.4.3/PKG-INFO
--rwxr-xr-x   0 ivanov     (501) staff       (20)     2303 2021-03-28 17:09:01.000000 signal_transformation-2.4.3/README.md
--rw-r--r--   0 ivanov     (501) staff       (20)       38 2021-05-03 11:34:52.351931 signal_transformation-2.4.3/setup.cfg
--rwxr-xr-x   0 ivanov     (501) staff       (20)     1175 2021-05-03 11:34:45.000000 signal_transformation-2.4.3/setup.py
-drwxr-xr-x   0 ivanov     (501) staff       (20)        0 2021-05-03 11:34:52.344594 signal_transformation-2.4.3/signal_transformation/
--rwxr-xr-x   0 ivanov     (501) staff       (20)        1 2019-08-12 12:35:46.000000 signal_transformation-2.4.3/signal_transformation/__init__.py
--rwxr-xr-x   0 ivanov     (501) staff       (20)     8671 2021-04-01 04:59:12.000000 signal_transformation-2.4.3/signal_transformation/helpers.py
-drwxr-xr-x   0 ivanov     (501) staff       (20)        0 2021-05-03 11:34:52.346742 signal_transformation-2.4.3/signal_transformation/images/
--rw-r--r--   0 ivanov     (501) staff       (20)        0 2021-02-22 11:30:08.000000 signal_transformation-2.4.3/signal_transformation/images/__init__.py
-drwxr-xr-x   0 ivanov     (501) staff       (20)        0 2021-05-03 11:34:52.347225 signal_transformation-2.4.3/signal_transformation/images/bin/
--rw-r--r--   0 ivanov     (501) staff       (20)        0 2021-02-22 11:30:08.000000 signal_transformation-2.4.3/signal_transformation/images/bin/__init__.py
--rw-r--r--   0 ivanov     (501) staff       (20)    16805 2021-02-23 07:41:51.000000 signal_transformation-2.4.3/signal_transformation/images/bin/imagenet_to_tf_records
-drwxr-xr-x   0 ivanov     (501) staff       (20)        0 2021-05-03 11:34:52.349055 signal_transformation-2.4.3/signal_transformation/voice/
--rw-r--r--   0 ivanov     (501) staff       (20)      193 2021-03-30 05:59:34.000000 signal_transformation-2.4.3/signal_transformation/voice/SpectFormat.py
--rw-r--r--   0 ivanov     (501) staff       (20)        0 2021-02-22 11:30:08.000000 signal_transformation-2.4.3/signal_transformation/voice/__init__.py
-drwxr-xr-x   0 ivanov     (501) staff       (20)        0 2021-05-03 11:34:52.350860 signal_transformation-2.4.3/signal_transformation/voice/bin/
--rw-r--r--   0 ivanov     (501) staff       (20)        0 2021-03-18 07:20:34.000000 signal_transformation-2.4.3/signal_transformation/voice/bin/__init__.py
--rw-r--r--   0 ivanov     (501) staff       (20)     1288 2021-04-01 04:54:46.000000 signal_transformation-2.4.3/signal_transformation/voice/bin/vox_to_metadata
--rw-r--r--   0 ivanov     (501) staff       (20)     2577 2021-03-28 17:09:01.000000 signal_transformation-2.4.3/signal_transformation/voice/bin/wav_to_tf_records
--rwxr-xr-x   0 ivanov     (501) staff       (20)     2353 2021-03-31 05:54:15.000000 signal_transformation-2.4.3/signal_transformation/voice/lrtr.py
--rwxr-xr-x   0 ivanov     (501) staff       (20)    12050 2021-05-03 11:34:45.000000 signal_transformation-2.4.3/signal_transformation/voice/tftr.py
--rwxr-xr-x   0 ivanov     (501) staff       (20)     5635 2021-02-22 11:30:08.000000 signal_transformation-2.4.3/signal_transformation/voice/vad.py
-drwxr-xr-x   0 ivanov     (501) staff       (20)        0 2021-05-03 11:34:52.346385 signal_transformation-2.4.3/signal_transformation.egg-info/
--rw-r--r--   0 ivanov     (501) staff       (20)      621 2021-05-03 11:34:52.000000 signal_transformation-2.4.3/signal_transformation.egg-info/PKG-INFO
--rw-r--r--   0 ivanov     (501) staff       (20)      783 2021-05-03 11:34:52.000000 signal_transformation-2.4.3/signal_transformation.egg-info/SOURCES.txt
--rw-r--r--   0 ivanov     (501) staff       (20)        1 2021-05-03 11:34:52.000000 signal_transformation-2.4.3/signal_transformation.egg-info/dependency_links.txt
--rw-r--r--   0 ivanov     (501) staff       (20)       78 2021-05-03 11:34:52.000000 signal_transformation-2.4.3/signal_transformation.egg-info/requires.txt
--rw-r--r--   0 ivanov     (501) staff       (20)       22 2021-05-03 11:34:52.000000 signal_transformation-2.4.3/signal_transformation.egg-info/top_level.txt
+drwxr-xr-x   0 ivanov     (501) staff       (20)        0 2023-04-20 09:42:27.347797 signal_transformation-2.5.0/
+-rwxr-xr-x   0 ivanov     (501) staff       (20)     1072 2019-08-12 09:06:04.000000 signal_transformation-2.5.0/LICENSE
+-rw-r--r--   0 ivanov     (501) staff       (20)      600 2023-04-20 09:42:27.347681 signal_transformation-2.5.0/PKG-INFO
+-rwxr-xr-x   0 ivanov     (501) staff       (20)     2303 2021-03-28 17:09:01.000000 signal_transformation-2.5.0/README.md
+-rw-r--r--   0 ivanov     (501) staff       (20)       38 2023-04-20 09:42:27.347841 signal_transformation-2.5.0/setup.cfg
+-rwxr-xr-x   0 ivanov     (501) staff       (20)     1179 2023-04-20 09:37:23.000000 signal_transformation-2.5.0/setup.py
+drwxr-xr-x   0 ivanov     (501) staff       (20)        0 2023-04-20 09:42:27.345231 signal_transformation-2.5.0/signal_transformation/
+-rwxr-xr-x   0 ivanov     (501) staff       (20)        1 2019-08-12 12:35:46.000000 signal_transformation-2.5.0/signal_transformation/__init__.py
+-rwxr-xr-x   0 ivanov     (501) staff       (20)     8671 2021-04-01 04:59:12.000000 signal_transformation-2.5.0/signal_transformation/helpers.py
+drwxr-xr-x   0 ivanov     (501) staff       (20)        0 2023-04-20 09:42:27.346023 signal_transformation-2.5.0/signal_transformation/images/
+-rw-r--r--   0 ivanov     (501) staff       (20)        0 2021-02-22 11:30:08.000000 signal_transformation-2.5.0/signal_transformation/images/__init__.py
+drwxr-xr-x   0 ivanov     (501) staff       (20)        0 2023-04-20 09:42:27.346217 signal_transformation-2.5.0/signal_transformation/images/bin/
+-rw-r--r--   0 ivanov     (501) staff       (20)        0 2021-02-22 11:30:08.000000 signal_transformation-2.5.0/signal_transformation/images/bin/__init__.py
+-rw-r--r--   0 ivanov     (501) staff       (20)    16805 2021-02-23 07:41:51.000000 signal_transformation-2.5.0/signal_transformation/images/bin/imagenet_to_tf_records
+drwxr-xr-x   0 ivanov     (501) staff       (20)        0 2023-04-20 09:42:27.346367 signal_transformation-2.5.0/signal_transformation/tf/
+-rw-r--r--   0 ivanov     (501) staff       (20)        0 2023-04-20 08:12:57.000000 signal_transformation-2.5.0/signal_transformation/tf/__init__.py
+drwxr-xr-x   0 ivanov     (501) staff       (20)        0 2023-04-20 09:42:27.346456 signal_transformation-2.5.0/signal_transformation/torch/
+-rw-r--r--   0 ivanov     (501) staff       (20)        0 2023-04-20 08:12:34.000000 signal_transformation-2.5.0/signal_transformation/torch/__init__.py
+drwxr-xr-x   0 ivanov     (501) staff       (20)        0 2023-04-20 09:42:27.346636 signal_transformation-2.5.0/signal_transformation/torch/models/
+-rw-r--r--   0 ivanov     (501) staff       (20)        0 2023-04-20 08:13:40.000000 signal_transformation-2.5.0/signal_transformation/torch/models/__init__.py
+-rw-r--r--   0 ivanov     (501) staff       (20)     7476 2023-04-20 08:40:09.000000 signal_transformation-2.5.0/signal_transformation/torch/models/matchboxnet.py
+drwxr-xr-x   0 ivanov     (501) staff       (20)        0 2023-04-20 09:42:27.347189 signal_transformation-2.5.0/signal_transformation/voice/
+-rw-r--r--   0 ivanov     (501) staff       (20)      193 2021-03-30 05:59:34.000000 signal_transformation-2.5.0/signal_transformation/voice/SpectFormat.py
+-rw-r--r--   0 ivanov     (501) staff       (20)        0 2021-02-22 11:30:08.000000 signal_transformation-2.5.0/signal_transformation/voice/__init__.py
+drwxr-xr-x   0 ivanov     (501) staff       (20)        0 2023-04-20 09:42:27.347510 signal_transformation-2.5.0/signal_transformation/voice/bin/
+-rw-r--r--   0 ivanov     (501) staff       (20)        0 2021-03-18 07:20:34.000000 signal_transformation-2.5.0/signal_transformation/voice/bin/__init__.py
+-rw-r--r--   0 ivanov     (501) staff       (20)     1288 2021-04-01 04:54:46.000000 signal_transformation-2.5.0/signal_transformation/voice/bin/vox_to_metadata
+-rw-r--r--   0 ivanov     (501) staff       (20)     2577 2021-03-28 17:09:01.000000 signal_transformation-2.5.0/signal_transformation/voice/bin/wav_to_tf_records
+-rwxr-xr-x   0 ivanov     (501) staff       (20)     2353 2021-03-31 05:54:15.000000 signal_transformation-2.5.0/signal_transformation/voice/lrtr.py
+-rwxr-xr-x   0 ivanov     (501) staff       (20)    12050 2021-05-03 11:34:45.000000 signal_transformation-2.5.0/signal_transformation/voice/tftr.py
+-rwxr-xr-x   0 ivanov     (501) staff       (20)     5635 2021-02-22 11:30:08.000000 signal_transformation-2.5.0/signal_transformation/voice/vad.py
+drwxr-xr-x   0 ivanov     (501) staff       (20)        0 2023-04-20 09:42:27.345898 signal_transformation-2.5.0/signal_transformation.egg-info/
+-rw-r--r--   0 ivanov     (501) staff       (20)      600 2023-04-20 09:42:27.000000 signal_transformation-2.5.0/signal_transformation.egg-info/PKG-INFO
+-rw-r--r--   0 ivanov     (501) staff       (20)      965 2023-04-20 09:42:27.000000 signal_transformation-2.5.0/signal_transformation.egg-info/SOURCES.txt
+-rw-r--r--   0 ivanov     (501) staff       (20)        1 2023-04-20 09:42:27.000000 signal_transformation-2.5.0/signal_transformation.egg-info/dependency_links.txt
+-rw-r--r--   0 ivanov     (501) staff       (20)      330 2023-04-20 09:42:27.000000 signal_transformation-2.5.0/signal_transformation.egg-info/requires.txt
+-rw-r--r--   0 ivanov     (501) staff       (20)       22 2023-04-20 09:42:27.000000 signal_transformation-2.5.0/signal_transformation.egg-info/top_level.txt
```

### Comparing `signal_transformation-2.4.3/PKG-INFO` & `signal_transformation-2.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: signal_transformation
-Version: 2.4.3
-Summary: The package allows performing a transformation of an audio signal using TensorFlow or LibROSA
+Version: 2.5.0
+Summary: The package allows performing a transformation of a signal using TensorFlow, Pytorch or LibROSA
 Home-page: https://github.com/Ilyushin/signal-transformation
 Author: Eugene Ilyushin
 Author-email: eugene.ilyushin@gmail.com
-License: UNKNOWN
-Description: The package allows performing a transformation of an audio signal using TensorFlow or LibROSA
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+The package allows performing a transformation of a signal using TensorFlow, Pytorch or LibROSA
```

### Comparing `signal_transformation-2.4.3/README.md` & `signal_transformation-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `signal_transformation-2.4.3/setup.py` & `signal_transformation-2.5.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,19 +6,19 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fh:
     requirements = fh.readlines()
 
 setuptools.setup(
     name="signal_transformation",
-    version="2.4.3",
+    version="2.5.0",
     author="Eugene Ilyushin",
     author_email="eugene.ilyushin@gmail.com",
-    description="The package allows performing a transformation of an audio signal using TensorFlow or LibROSA",
-    long_description="The package allows performing a transformation of an audio signal using TensorFlow or LibROSA",
+    description="The package allows performing a transformation of a signal using TensorFlow, Pytorch or LibROSA",
+    long_description="The package allows performing a transformation of a signal using TensorFlow, Pytorch or LibROSA",
     long_description_content_type="text/markdown",
     url="https://github.com/Ilyushin/signal-transformation",
     packages=setuptools.find_packages(),
     scripts=[
         'signal_transformation/images/bin/imagenet_to_tf_records',
         'signal_transformation/voice/bin/wav_to_tf_records',
         'signal_transformation/voice/bin/vox_to_metadata'
```

### Comparing `signal_transformation-2.4.3/signal_transformation/helpers.py` & `signal_transformation-2.5.0/signal_transformation/helpers.py`

 * *Files identical despite different names*

### Comparing `signal_transformation-2.4.3/signal_transformation/images/bin/imagenet_to_tf_records` & `signal_transformation-2.5.0/signal_transformation/images/bin/imagenet_to_tf_records`

 * *Files identical despite different names*

### Comparing `signal_transformation-2.4.3/signal_transformation/voice/bin/vox_to_metadata` & `signal_transformation-2.5.0/signal_transformation/voice/bin/vox_to_metadata`

 * *Files identical despite different names*

### Comparing `signal_transformation-2.4.3/signal_transformation/voice/bin/wav_to_tf_records` & `signal_transformation-2.5.0/signal_transformation/voice/bin/wav_to_tf_records`

 * *Files identical despite different names*

### Comparing `signal_transformation-2.4.3/signal_transformation/voice/lrtr.py` & `signal_transformation-2.5.0/signal_transformation/voice/lrtr.py`

 * *Files identical despite different names*

### Comparing `signal_transformation-2.4.3/signal_transformation/voice/tftr.py` & `signal_transformation-2.5.0/signal_transformation/voice/tftr.py`

 * *Files identical despite different names*

### Comparing `signal_transformation-2.4.3/signal_transformation/voice/vad.py` & `signal_transformation-2.5.0/signal_transformation/voice/vad.py`

 * *Files identical despite different names*

### Comparing `signal_transformation-2.4.3/signal_transformation.egg-info/PKG-INFO` & `signal_transformation-2.5.0/signal_transformation.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: signal-transformation
-Version: 2.4.3
-Summary: The package allows performing a transformation of an audio signal using TensorFlow or LibROSA
+Version: 2.5.0
+Summary: The package allows performing a transformation of a signal using TensorFlow, Pytorch or LibROSA
 Home-page: https://github.com/Ilyushin/signal-transformation
 Author: Eugene Ilyushin
 Author-email: eugene.ilyushin@gmail.com
-License: UNKNOWN
-Description: The package allows performing a transformation of an audio signal using TensorFlow or LibROSA
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+The package allows performing a transformation of a signal using TensorFlow, Pytorch or LibROSA
```

### Comparing `signal_transformation-2.4.3/signal_transformation.egg-info/SOURCES.txt` & `signal_transformation-2.5.0/signal_transformation.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,24 @@
+LICENSE
 README.md
 setup.py
 signal_transformation/__init__.py
 signal_transformation/helpers.py
 signal_transformation.egg-info/PKG-INFO
 signal_transformation.egg-info/SOURCES.txt
 signal_transformation.egg-info/dependency_links.txt
 signal_transformation.egg-info/requires.txt
 signal_transformation.egg-info/top_level.txt
 signal_transformation/images/__init__.py
 signal_transformation/images/bin/__init__.py
 signal_transformation/images/bin/imagenet_to_tf_records
+signal_transformation/tf/__init__.py
+signal_transformation/torch/__init__.py
+signal_transformation/torch/models/__init__.py
+signal_transformation/torch/models/matchboxnet.py
 signal_transformation/voice/SpectFormat.py
 signal_transformation/voice/__init__.py
 signal_transformation/voice/lrtr.py
 signal_transformation/voice/tftr.py
 signal_transformation/voice/vad.py
 signal_transformation/voice/bin/__init__.py
 signal_transformation/voice/bin/vox_to_metadata
```

