# Comparing `tmp/hi-ml-multimodal-0.2.0.tar.gz` & `tmp/hi-ml-multimodal-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hi-ml-multimodal-0.2.0.tar", last modified: Wed Mar 22 17:47:33 2023, max compression
+gzip compressed data, was "hi-ml-multimodal-0.2.1.tar", last modified: Thu Apr 20 13:56:27 2023, max compression
```

## Comparing `hi-ml-multimodal-0.2.0.tar` & `hi-ml-multimodal-0.2.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-03-22 17:47:33.720553 hi-ml-multimodal-0.2.0/
--rw-r--r--   0 fernando  (1000) fernando  (1000)       63 2023-03-06 16:22:52.000000 hi-ml-multimodal-0.2.0/MANIFEST.in
--rw-r--r--   0 fernando  (1000) fernando  (1000)     4864 2023-03-22 17:47:33.720553 hi-ml-multimodal-0.2.0/PKG-INFO
--rw-r--r--   0 fernando  (1000) fernando  (1000)     4254 2023-03-22 17:37:23.000000 hi-ml-multimodal-0.2.0/README.md
--rw-r--r--   0 fernando  (1000) fernando  (1000)      161 2023-03-20 20:56:01.000000 hi-ml-multimodal-0.2.0/requirements_run.txt
--rw-r--r--   0 fernando  (1000) fernando  (1000)       38 2023-03-22 17:47:33.720553 hi-ml-multimodal-0.2.0/setup.cfg
--rw-r--r--   0 fernando  (1000) fernando  (1000)     1509 2023-03-22 17:42:45.000000 hi-ml-multimodal-0.2.0/setup.py
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-03-22 17:47:33.710934 hi-ml-multimodal-0.2.0/src/
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-03-22 17:47:33.720553 hi-ml-multimodal-0.2.0/src/health_multimodal/
--rw-r--r--   0 fernando  (1000) fernando  (1000)      369 2023-03-22 17:42:45.000000 hi-ml-multimodal-0.2.0/src/health_multimodal/__init__.py
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-03-22 17:47:33.720553 hi-ml-multimodal-0.2.0/src/health_multimodal/common/
--rw-r--r--   0 fernando  (1000) fernando  (1000)      472 2023-03-20 20:56:01.000000 hi-ml-multimodal-0.2.0/src/health_multimodal/common/__init__.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)      607 2023-03-20 20:56:01.000000 hi-ml-multimodal-0.2.0/src/health_multimodal/common/device.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     5396 2023-03-22 17:37:23.000000 hi-ml-multimodal-0.2.0/src/health_multimodal/common/visualization.py
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-03-22 17:47:33.720553 hi-ml-multimodal-0.2.0/src/health_multimodal/image/
--rw-r--r--   0 fernando  (1000) fernando  (1000)     1056 2023-03-22 17:37:23.000000 hi-ml-multimodal-0.2.0/src/health_multimodal/image/__init__.py
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-03-22 17:47:33.720553 hi-ml-multimodal-0.2.0/src/health_multimodal/image/data/
--rw-r--r--   0 fernando  (1000) fernando  (1000)      346 2022-07-01 12:45:09.000000 hi-ml-multimodal-0.2.0/src/health_multimodal/image/data/__init__.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     2883 2023-02-06 15:30:24.000000 hi-ml-multimodal-0.2.0/src/health_multimodal/image/data/io.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     3315 2023-02-06 15:30:24.000000 hi-ml-multimodal-0.2.0/src/health_multimodal/image/data/transforms.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     3764 2023-03-20 20:56:01.000000 hi-ml-multimodal-0.2.0/src/health_multimodal/image/inference_engine.py
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-03-22 17:47:33.720553 hi-ml-multimodal-0.2.0/src/health_multimodal/image/model/
--rw-r--r--   0 fernando  (1000) fernando  (1000)      526 2023-03-22 17:37:23.000000 hi-ml-multimodal-0.2.0/src/health_multimodal/image/model/__init__.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     7623 2023-03-20 20:56:01.000000 hi-ml-multimodal-0.2.0/src/health_multimodal/image/model/encoder.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     5860 2023-03-22 17:37:23.000000 hi-ml-multimodal-0.2.0/src/health_multimodal/image/model/model.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     3772 2023-02-06 15:30:24.000000 hi-ml-multimodal-0.2.0/src/health_multimodal/image/model/modules.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     3225 2023-03-22 17:37:23.000000 hi-ml-multimodal-0.2.0/src/health_multimodal/image/model/pretrained.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     3174 2023-02-20 17:28:48.000000 hi-ml-multimodal-0.2.0/src/health_multimodal/image/model/resnet.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)    11909 2023-03-20 20:56:01.000000 hi-ml-multimodal-0.2.0/src/health_multimodal/image/model/transformer.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     1183 2023-03-20 20:56:01.000000 hi-ml-multimodal-0.2.0/src/health_multimodal/image/model/types.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     1781 2023-03-22 17:37:23.000000 hi-ml-multimodal-0.2.0/src/health_multimodal/image/utils.py
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-03-22 17:47:33.720553 hi-ml-multimodal-0.2.0/src/health_multimodal/text/
--rw-r--r--   0 fernando  (1000) fernando  (1000)     1123 2023-03-22 17:37:23.000000 hi-ml-multimodal-0.2.0/src/health_multimodal/text/__init__.py
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-03-22 17:47:33.720553 hi-ml-multimodal-0.2.0/src/health_multimodal/text/data/
--rw-r--r--   0 fernando  (1000) fernando  (1000)      346 2022-07-01 12:45:09.000000 hi-ml-multimodal-0.2.0/src/health_multimodal/text/data/__init__.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     2775 2023-02-20 16:21:32.000000 hi-ml-multimodal-0.2.0/src/health_multimodal/text/data/io.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     5188 2023-02-20 16:21:32.000000 hi-ml-multimodal-0.2.0/src/health_multimodal/text/inference_engine.py
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-03-22 17:47:33.720553 hi-ml-multimodal-0.2.0/src/health_multimodal/text/model/
--rw-r--r--   0 fernando  (1000) fernando  (1000)      575 2022-07-27 21:15:34.000000 hi-ml-multimodal-0.2.0/src/health_multimodal/text/model/__init__.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)      889 2022-07-01 12:45:09.000000 hi-ml-multimodal-0.2.0/src/health_multimodal/text/model/configuration_cxrbert.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     6168 2023-03-06 13:29:04.000000 hi-ml-multimodal-0.2.0/src/health_multimodal/text/model/modelling_cxrbert.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     2563 2023-03-22 17:37:23.000000 hi-ml-multimodal-0.2.0/src/health_multimodal/text/utils.py
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-03-22 17:47:33.720553 hi-ml-multimodal-0.2.0/src/health_multimodal/vlp/
--rw-r--r--   0 fernando  (1000) fernando  (1000)      584 2022-07-27 21:15:34.000000 hi-ml-multimodal-0.2.0/src/health_multimodal/vlp/__init__.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     7806 2023-02-20 16:21:32.000000 hi-ml-multimodal-0.2.0/src/health_multimodal/vlp/inference_engine.py
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-03-22 17:47:33.720553 hi-ml-multimodal-0.2.0/src/hi_ml_multimodal.egg-info/
--rw-r--r--   0 fernando  (1000) fernando  (1000)     4864 2023-03-22 17:47:33.000000 hi-ml-multimodal-0.2.0/src/hi_ml_multimodal.egg-info/PKG-INFO
--rw-r--r--   0 fernando  (1000) fernando  (1000)     1494 2023-03-22 17:47:33.000000 hi-ml-multimodal-0.2.0/src/hi_ml_multimodal.egg-info/SOURCES.txt
--rw-r--r--   0 fernando  (1000) fernando  (1000)        1 2023-03-22 17:47:33.000000 hi-ml-multimodal-0.2.0/src/hi_ml_multimodal.egg-info/dependency_links.txt
--rw-r--r--   0 fernando  (1000) fernando  (1000)      161 2023-03-22 17:47:33.000000 hi-ml-multimodal-0.2.0/src/hi_ml_multimodal.egg-info/requires.txt
--rw-r--r--   0 fernando  (1000) fernando  (1000)       18 2023-03-22 17:47:33.000000 hi-ml-multimodal-0.2.0/src/hi_ml_multimodal.egg-info/top_level.txt
+drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-04-20 13:56:27.334885 hi-ml-multimodal-0.2.1/
+-rw-r--r--   0 fernando  (1000) fernando  (1000)       63 2023-03-06 16:22:52.000000 hi-ml-multimodal-0.2.1/MANIFEST.in
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     4864 2023-04-20 13:56:27.334885 hi-ml-multimodal-0.2.1/PKG-INFO
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     4254 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/README.md
+-rw-r--r--   0 fernando  (1000) fernando  (1000)      161 2023-04-20 13:54:43.000000 hi-ml-multimodal-0.2.1/requirements_run.txt
+-rw-r--r--   0 fernando  (1000) fernando  (1000)       38 2023-04-20 13:56:27.334885 hi-ml-multimodal-0.2.1/setup.cfg
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     1510 2023-04-20 13:54:46.000000 hi-ml-multimodal-0.2.1/setup.py
+drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-04-20 13:56:27.325276 hi-ml-multimodal-0.2.1/src/
+drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-04-20 13:56:27.325276 hi-ml-multimodal-0.2.1/src/health_multimodal/
+-rw-r--r--   0 fernando  (1000) fernando  (1000)      369 2023-04-20 13:54:46.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/__init__.py
+drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-04-20 13:56:27.325276 hi-ml-multimodal-0.2.1/src/health_multimodal/common/
+-rw-r--r--   0 fernando  (1000) fernando  (1000)      472 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/common/__init__.py
+-rw-r--r--   0 fernando  (1000) fernando  (1000)      605 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/common/device.py
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     5245 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/common/visualization.py
+drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-04-20 13:56:27.334885 hi-ml-multimodal-0.2.1/src/health_multimodal/image/
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     1056 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/image/__init__.py
+drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-04-20 13:56:27.334885 hi-ml-multimodal-0.2.1/src/health_multimodal/image/data/
+-rw-r--r--   0 fernando  (1000) fernando  (1000)      346 2022-07-01 12:45:09.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/image/data/__init__.py
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     2835 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/image/data/io.py
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     3332 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/image/data/transforms.py
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     3764 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/image/inference_engine.py
+drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-04-20 13:56:27.334885 hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/
+-rw-r--r--   0 fernando  (1000) fernando  (1000)      526 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/__init__.py
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     7625 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/encoder.py
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     5725 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/model.py
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     3731 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/modules.py
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     4625 2023-04-20 13:54:43.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/pretrained.py
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     3186 2023-04-20 13:54:43.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/resnet.py
+-rw-r--r--   0 fernando  (1000) fernando  (1000)    11818 2023-04-20 13:54:43.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/transformer.py
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     1329 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/types.py
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     1778 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/image/utils.py
+drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-04-20 13:56:27.334885 hi-ml-multimodal-0.2.1/src/health_multimodal/text/
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     1123 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/text/__init__.py
+drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-04-20 13:56:27.334885 hi-ml-multimodal-0.2.1/src/health_multimodal/text/data/
+-rw-r--r--   0 fernando  (1000) fernando  (1000)      346 2022-07-01 12:45:09.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/text/data/__init__.py
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     2617 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/text/data/io.py
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     5045 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/text/inference_engine.py
+drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-04-20 13:56:27.334885 hi-ml-multimodal-0.2.1/src/health_multimodal/text/model/
+-rw-r--r--   0 fernando  (1000) fernando  (1000)      575 2022-07-27 21:15:34.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/text/model/__init__.py
+-rw-r--r--   0 fernando  (1000) fernando  (1000)      889 2022-07-01 12:45:09.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/text/model/configuration_cxrbert.py
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     5785 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/text/model/modelling_cxrbert.py
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     2544 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/text/utils.py
+drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-04-20 13:56:27.334885 hi-ml-multimodal-0.2.1/src/health_multimodal/vlp/
+-rw-r--r--   0 fernando  (1000) fernando  (1000)      584 2022-07-27 21:15:34.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/vlp/__init__.py
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     7552 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/vlp/inference_engine.py
+drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-04-20 13:56:27.334885 hi-ml-multimodal-0.2.1/src/hi_ml_multimodal.egg-info/
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     4864 2023-04-20 13:56:27.000000 hi-ml-multimodal-0.2.1/src/hi_ml_multimodal.egg-info/PKG-INFO
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     1494 2023-04-20 13:56:27.000000 hi-ml-multimodal-0.2.1/src/hi_ml_multimodal.egg-info/SOURCES.txt
+-rw-r--r--   0 fernando  (1000) fernando  (1000)        1 2023-04-20 13:56:27.000000 hi-ml-multimodal-0.2.1/src/hi_ml_multimodal.egg-info/dependency_links.txt
+-rw-r--r--   0 fernando  (1000) fernando  (1000)      161 2023-04-20 13:56:27.000000 hi-ml-multimodal-0.2.1/src/hi_ml_multimodal.egg-info/requires.txt
+-rw-r--r--   0 fernando  (1000) fernando  (1000)       18 2023-04-20 13:56:27.000000 hi-ml-multimodal-0.2.1/src/hi_ml_multimodal.egg-info/top_level.txt
```

### Comparing `hi-ml-multimodal-0.2.0/PKG-INFO` & `hi-ml-multimodal-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: hi-ml-multimodal
-Version: 0.2.0
+Version: 0.2.1
 Summary: Microsoft Health Futures package to work with multi-modal health data
 Home-page: https://github.com/microsoft/hi-ml
 Author: Biomedical Imaging Team @ Microsoft Health Futures
 Author-email: innereyedev@microsoft.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 # HI-ML Multimodal Toolbox
 
 This toolbox provides models for multimodal health data.
 The code is available on [GitHub][1] and [Hugging Face 🤗][6].
 
 ## Getting started
 
 The best way to get started is by running the [phrase grounding notebook][2] and the [examples](#examples).
-All the dependencies will be installed upon execution, so Python 3.7 and [Jupyter][3] are the only requirements to get started.
+All the dependencies will be installed upon execution, so Python 3.9 and [Jupyter][3] are the only requirements to get started.
 
 The notebook can also be run on [Binder][4], without the need to download any code or install any libraries:
 
 [![Binder](https://mybinder.org/badge_logo.svg)][4]
 
 ## Installation
```

### Comparing `hi-ml-multimodal-0.2.0/README.md` & `hi-ml-multimodal-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 This toolbox provides models for multimodal health data.
 The code is available on [GitHub][1] and [Hugging Face 🤗][6].
 
 ## Getting started
 
 The best way to get started is by running the [phrase grounding notebook][2] and the [examples](#examples).
-All the dependencies will be installed upon execution, so Python 3.7 and [Jupyter][3] are the only requirements to get started.
+All the dependencies will be installed upon execution, so Python 3.9 and [Jupyter][3] are the only requirements to get started.
 
 The notebook can also be run on [Binder][4], without the need to download any code or install any libraries:
 
 [![Binder](https://mybinder.org/badge_logo.svg)][4]
 
 ## Installation
```

### Comparing `hi-ml-multimodal-0.2.0/setup.py` & `hi-ml-multimodal-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #  ------------------------------------------------------------------------------------------
 
 from pathlib import Path
 from setuptools import find_namespace_packages, setup  # type: ignore
 
 
 long_description = Path("README.md").read_text(encoding="utf-8")
-version = "0.2.0"
+version = "0.2.1"
 package_name = "hi-ml-multimodal"
 install_requires = Path("requirements_run.txt").read_text().splitlines()
 
 description = "Microsoft Health Futures package to work with multi-modal health data"
 
 setup(
     name=package_name,
@@ -24,15 +24,15 @@
     author="Biomedical Imaging Team @ Microsoft Health Futures",
     author_email="innereyedev@microsoft.com",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Medical Science Apps.",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.7"
+        "Programming Language :: Python :: 3.9",
     ],
     license="MIT License",
     packages=find_namespace_packages(where="src"),
     package_dir={"": "src"},
     include_package_data=True,
     install_requires=install_requires,
 )
```

### Comparing `hi-ml-multimodal-0.2.0/src/health_multimodal/common/device.py` & `hi-ml-multimodal-0.2.1/src/health_multimodal/common/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,10 +8,10 @@
 
 
 def get_module_device(module: torch.nn.Module) -> torch.device:
     """
     Returns the device of the module
     """
     device = next(module.parameters()).device  # type: ignore
-    assert (isinstance(device, torch.device))
+    assert isinstance(device, torch.device)
 
     return device
```

### Comparing `hi-ml-multimodal-0.2.0/src/health_multimodal/common/visualization.py` & `hi-ml-multimodal-0.2.1/src/health_multimodal/common/visualization.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,20 +38,20 @@
 def _get_isolines_levels(step_size: float) -> np.ndarray:
     num_steps = np.floor(round(1 / step_size)).astype(int)
     levels = np.linspace(step_size, 1, num_steps)
     return levels
 
 
 def _plot_isolines(
-        image: TypeArrayImage,
-        heatmap: np.ndarray,
-        axis: plt.Axes,
-        title: Optional[str] = None,
-        colormap: str = "RdBu_r",
-        step: float = 0.25,
+    image: TypeArrayImage,
+    heatmap: np.ndarray,
+    axis: plt.Axes,
+    title: Optional[str] = None,
+    colormap: str = "RdBu_r",
+    step: float = 0.25,
 ) -> None:
     """Plot an image and overlay heatmap isolines on it.
 
     :param image: Input image.
     :param heatmap: Heatmap of the same size as the image.
     :param axis: Axis to plot the image on.
     :param title: Title used for the axis.
@@ -71,21 +71,21 @@
     axis.clabel(contours, inline=True, fontsize=10)
     axis.axis("off")
     if title is not None:
         axis.set_title(title)
 
 
 def _plot_heatmap(
-        image: TypeArrayImage,
-        heatmap: np.ndarray,
-        figure: plt.Figure,
-        axis: plt.Axes,
-        colormap: str = "RdBu_r",
-        title: Optional[str] = None,
-        alpha: float = 0.5,
+    image: TypeArrayImage,
+    heatmap: np.ndarray,
+    figure: plt.Figure,
+    axis: plt.Axes,
+    colormap: str = "RdBu_r",
+    title: Optional[str] = None,
+    alpha: float = 0.5,
 ) -> None:
     """Plot a heatmap overlaid on an image.
 
     :param image: Input image.
     :param heatmap: Input heatmap of the same size as the image.
     :param figure: Figure to plot the images on.
     :param axis: Axis to plot the images on.
@@ -104,17 +104,16 @@
     plt.setp(colorbar.ax.get_yticklabels(), ha="right")
     axis.axis("off")
     if title is not None:
         axis.set_title(title)
 
 
 def plot_phrase_grounding_similarity_map(
-        image_path: Path,
-        similarity_map: np.ndarray,
-        bboxes: Optional[List[Tuple[float, float, float, float]]] = None) -> plt.Figure:
+    image_path: Path, similarity_map: np.ndarray, bboxes: Optional[List[Tuple[float, float, float, float]]] = None
+) -> plt.Figure:
     """Plot visualization of the input image, the similarity heatmap and the heatmap isolines.
 
     :param image_path: Path to the input image.
     :param similarity_map: Phase grounding similarity map of the same size as the image.
     :param bboxes: Optional list of bounding boxes to plot on the image.
     """
     fig, axes = plt.subplots(1, 3, figsize=(15, 6))
@@ -123,24 +122,24 @@
     _plot_isolines(image, similarity_map, axis=axes[1], title="Similarity isolines")
     _plot_heatmap(image, similarity_map, figure=fig, axis=axes[2], title="Similarity heatmap")
     if bboxes is not None:
         _plot_bounding_boxes(ax=axes[1], bboxes=bboxes)
     return fig
 
 
-def _plot_bounding_boxes(ax: plt.Axes,
-                         bboxes: List[Tuple[float, float, float, float]],
-                         linewidth: float = 1.5,
-                         alpha: float = 0.45) -> None:
+def _plot_bounding_boxes(
+    ax: plt.Axes, bboxes: List[Tuple[float, float, float, float]], linewidth: float = 1.5, alpha: float = 0.45
+) -> None:
     """
     Plot bounding boxes on an existing axes object.
 
     :param ax: The axes object to plot the bounding boxes on.
     :param bboxes: A list of bounding box coordinates as (x, y, width, height) tuples.
     :param linewidth: Optional line width for the bounding box edges (default is 2).
     :param alpha: Optional opacity for the bounding box edges (default is 1.0).
     """
     for bbox in bboxes:
         x, y, width, height = bbox
-        rect = patches.Rectangle((x, y), width, height, linewidth=linewidth, edgecolor='k',
-                                 facecolor='none', linestyle='--', alpha=alpha)
+        rect = patches.Rectangle(
+            (x, y), width, height, linewidth=linewidth, edgecolor='k', facecolor='none', linestyle='--', alpha=alpha
+        )
         ax.add_patch(rect)
```

### Comparing `hi-ml-multimodal-0.2.0/src/health_multimodal/image/__init__.py` & `hi-ml-multimodal-0.2.1/src/health_multimodal/image/__init__.py`

 * *Files identical despite different names*

### Comparing `hi-ml-multimodal-0.2.0/src/health_multimodal/image/data/io.py` & `hi-ml-multimodal-0.2.1/src/health_multimodal/image/data/io.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,18 +24,15 @@
         Passing ``None`` is equivalent to using percentiles ``(0, 100)`` (but faster).
     :returns: Array with ``0`` and ``255`` as minimum and maximum values.
     """
     array = array.astype(float)
     if percentiles is not None:
         len_percentiles = len(percentiles)
         if len_percentiles != 2:
-            message = (
-                'The value for percentiles should be a sequence of length 2,'
-                f' but has length {len_percentiles}'
-            )
+            message = 'The value for percentiles should be a sequence of length 2,' f' but has length {len_percentiles}'
             raise ValueError(message)
         a, b = percentiles
         if a >= b:
             raise ValueError(f'Percentiles must be in ascending order, but a sequence "{percentiles}" was passed')
         if a < 0 or b > 100:
             raise ValueError(f'Percentiles must be in the range [0, 100], but a sequence "{percentiles}" was passed')
         cutoff: np.ndarray = np.percentile(array, percentiles)
```

### Comparing `hi-ml-multimodal-0.2.0/src/health_multimodal/image/data/transforms.py` & `hi-ml-multimodal-0.2.1/src/health_multimodal/image/data/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,10 +61,11 @@
                 two_dims = len(transform.size) == 2
                 same_sizes = transform.size[0] == transform.size[1]
                 is_square = two_dims and same_sizes
                 assert is_square, "Only square center crop supported"
                 crop_size_from_transforms = transform.size[0]
             else:
                 raise ValueError(
-                    f"Crop size has already been set to {crop_size_from_transforms} in a previous transform")
+                    f"Crop size has already been set to {crop_size_from_transforms} in a previous transform"
+                )
 
     return resize_size_from_transforms, crop_size_from_transforms
```

### Comparing `hi-ml-multimodal-0.2.0/src/health_multimodal/image/inference_engine.py` & `hi-ml-multimodal-0.2.1/src/health_multimodal/image/inference_engine.py`

 * *Files identical despite different names*

### Comparing `hi-ml-multimodal-0.2.0/src/health_multimodal/image/model/__init__.py` & `hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/__init__.py`

 * *Files identical despite different names*

### Comparing `hi-ml-multimodal-0.2.0/src/health_multimodal/image/model/encoder.py` & `hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/encoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,21 +38,19 @@
             encoder_class = resnet18
         elif self.img_encoder_type in [ImageEncoderType.RESNET50, ImageEncoderType.RESNET50_MULTI_IMAGE]:
             encoder_class = resnet50
         else:
             supported = ImageEncoderType.get_members(multi_image_encoders_only=False)
             raise NotImplementedError(f"Image encoder type \"{self.img_encoder_type}\" must be in {supported}")
 
-        encoder = encoder_class(pretrained=True, **kwargs)
+        encoder = encoder_class(pretrained=False, **kwargs)
 
         return encoder
 
-    def forward(self,
-                current_image: torch.Tensor,
-                return_patch_embeddings: bool = False) -> ImageEncoderOutputType:
+    def forward(self, current_image: torch.Tensor, return_patch_embeddings: bool = False) -> ImageEncoderOutputType:
         """Get image global and patch embeddings"""
 
         patch_emb = self.encoder(current_image)
         avg_pooled_emb = torch.flatten(torch.nn.functional.adaptive_avg_pool2d(patch_emb, (1, 1)), 1)
         if return_patch_embeddings:
             return patch_emb, avg_pooled_emb
 
@@ -95,27 +93,34 @@
         super().__init__(img_encoder_type)
 
         output_dim = 256  # The aggregate feature dim of the encoder is `2 * output_dim` i.e. [f_static, f_diff]
         grid_shape = (14, 14)  # Spatial dimensions of patch grid.
 
         backbone_output_feature_dim = get_encoder_output_dim(self.encoder, device=get_module_device(self))
 
-        self.backbone_to_vit = nn.Conv2d(in_channels=backbone_output_feature_dim, out_channels=output_dim,
-                                         kernel_size=1, stride=1, padding=0, bias=False)
+        self.backbone_to_vit = nn.Conv2d(
+            in_channels=backbone_output_feature_dim,
+            out_channels=output_dim,
+            kernel_size=1,
+            stride=1,
+            padding=0,
+            bias=False,
+        )
         self.vit_pooler = VisionTransformerPooler(input_dim=output_dim, grid_shape=grid_shape)
 
         # Missing image embedding
         self.missing_previous_emb = nn.Parameter(torch.zeros(1, output_dim, 1, 1))
-        trunc_normal_(self.missing_previous_emb, std=.02)
-
-    def forward(self,  # type: ignore[override]
-                current_image: torch.Tensor,
-                previous_image: Optional[torch.Tensor] = None,
-                return_patch_embeddings: bool = False) -> ImageEncoderOutputType:
+        trunc_normal_(self.missing_previous_emb, std=0.02)
 
+    def forward(  # type: ignore[override]
+        self,
+        current_image: torch.Tensor,
+        previous_image: Optional[torch.Tensor] = None,
+        return_patch_embeddings: bool = False,
+    ) -> ImageEncoderOutputType:
         batch_size = current_image.shape[0]
 
         if previous_image is not None:
             assert current_image.shape == previous_image.shape
             x = torch.cat([current_image, previous_image], dim=0)
             x = super().forward(x, return_patch_embeddings=True)[0]
             x = self.backbone_to_vit(x)
```

### Comparing `hi-ml-multimodal-0.2.0/src/health_multimodal/image/model/model.py` & `hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,39 +17,46 @@
 from .encoder import get_encoder_from_type, get_encoder_output_dim, MultiImageEncoder
 from .modules import MLP, MultiTaskModel
 from .types import ImageModelOutput
 
 
 class BaseImageModel(nn.Module, ABC):
     """Abstract class for image models."""
+
     @abstractmethod
     def forward(self, *args: Any, **kwargs: Any) -> ImageModelOutput:
         raise NotImplementedError
 
     @abstractmethod
     def get_patchwise_projected_embeddings(self, input_img: torch.Tensor, normalize: bool) -> torch.Tensor:
         raise NotImplementedError
 
 
 class ImageModel(BaseImageModel):
     """Image encoder module"""
 
-    def __init__(self,
-                 img_encoder_type: str,
-                 joint_feature_size: int,
-                 freeze_encoder: bool = False,
-                 pretrained_model_path: Optional[Union[str, Path]] = None,
-                 **downstream_classifier_kwargs: Any):
+    def __init__(
+        self,
+        img_encoder_type: str,
+        joint_feature_size: int,
+        freeze_encoder: bool = False,
+        pretrained_model_path: Optional[Union[str, Path]] = None,
+        **downstream_classifier_kwargs: Any,
+    ):
         super().__init__()
 
         # Initiate encoder, projector, and classifier
         self.encoder = get_encoder_from_type(img_encoder_type)
         self.feature_size = get_encoder_output_dim(self.encoder, device=get_module_device(self.encoder))
-        self.projector = MLP(input_dim=self.feature_size, output_dim=joint_feature_size,
-                             hidden_dim=joint_feature_size, use_1x1_convs=True)
+        self.projector = MLP(
+            input_dim=self.feature_size,
+            output_dim=joint_feature_size,
+            hidden_dim=joint_feature_size,
+            use_1x1_convs=True,
+        )
         self.downstream_classifier_kwargs = downstream_classifier_kwargs
         self.classifier = self.create_downstream_classifier() if downstream_classifier_kwargs else None
 
         # Initialise the mode of modules
         self.freeze_encoder = freeze_encoder
         self.train()
 
@@ -74,19 +81,21 @@
 
     def forward_post_encoder(self, patch_x: torch.Tensor, pooled_x: torch.Tensor) -> ImageModelOutput:
         with torch.set_grad_enabled(not self.freeze_encoder):
             projected_patch_embeddings = self.projector(patch_x)
             projected_global_embedding = torch.mean(projected_patch_embeddings, dim=(2, 3))
 
         logits = self.classifier(pooled_x) if self.classifier else None
-        return ImageModelOutput(img_embedding=pooled_x,
-                                patch_embeddings=patch_x,
-                                class_logits=logits,
-                                projected_patch_embeddings=projected_patch_embeddings,
-                                projected_global_embedding=projected_global_embedding)
+        return ImageModelOutput(
+            img_embedding=pooled_x,
+            patch_embeddings=patch_x,
+            class_logits=logits,
+            projected_patch_embeddings=projected_patch_embeddings,
+            projected_global_embedding=projected_global_embedding,
+        )
 
     def create_downstream_classifier(self, **kwargs: Any) -> MultiTaskModel:
         """Create the classification module for the downstream task."""
         downstream_classifier_kwargs = kwargs if kwargs else self.downstream_classifier_kwargs
         return MultiTaskModel(self.feature_size, **downstream_classifier_kwargs)
 
     @torch.no_grad()
@@ -107,16 +116,15 @@
 
 
 class MultiImageModel(ImageModel):
     def __init__(self, **kwargs: Any) -> None:
         super().__init__(**kwargs)
         assert isinstance(self.encoder, MultiImageEncoder), "MultiImageModel only supports MultiImageEncoder"
 
-    def forward(self,  # type: ignore[override]
-                current_image: torch.Tensor,
-                previous_image: Optional[torch.Tensor] = None) -> ImageModelOutput:
-
+    def forward(  # type: ignore[override]
+        self, current_image: torch.Tensor, previous_image: Optional[torch.Tensor] = None
+    ) -> ImageModelOutput:
         with torch.set_grad_enabled(not self.freeze_encoder):
-            patch_x, pooled_x = self.encoder(current_image=current_image,
-                                             previous_image=previous_image,
-                                             return_patch_embeddings=True)
+            patch_x, pooled_x = self.encoder(
+                current_image=current_image, previous_image=previous_image, return_patch_embeddings=True
+            )
         return self.forward_post_encoder(patch_x, pooled_x)
```

### Comparing `hi-ml-multimodal-0.2.0/src/health_multimodal/image/model/modules.py` & `hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/modules.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,19 +15,17 @@
 
     :param input_dim: Input embedding feature size
     :param hidden_dim: Hidden layer size in MLP
     :param output_dim: Output projection size
     :param use_1x1_convs: Use 1x1 conv kernels instead of 2D linear transformations for speed and memory efficiency.
     """
 
-    def __init__(self,
-                 input_dim: int,
-                 output_dim: int,
-                 hidden_dim: Optional[int] = None,
-                 use_1x1_convs: bool = False) -> None:
+    def __init__(
+        self, input_dim: int, output_dim: int, hidden_dim: Optional[int] = None, use_1x1_convs: bool = False
+    ) -> None:
         super().__init__()
 
         if use_1x1_convs:
             linear_proj_1_args = {'in_channels': input_dim, 'out_channels': hidden_dim, 'kernel_size': 1, 'bias': False}
             linear_proj_2_args = {'in_channels': hidden_dim, 'out_channels': output_dim, 'kernel_size': 1, 'bias': True}
             normalisation_layer: Callable = nn.BatchNorm2d
             projection_layer: Callable = nn.Conv2d
@@ -40,15 +38,16 @@
         self.output_dim = output_dim
         self.input_dim = input_dim
         if hidden_dim is not None:
             self.model = nn.Sequential(
                 projection_layer(**linear_proj_1_args),
                 normalisation_layer(hidden_dim),
                 nn.ReLU(inplace=True),
-                projection_layer(**linear_proj_2_args))
+                projection_layer(**linear_proj_2_args),
+            )
         else:
             self.model = nn.Linear(input_dim, output_dim)  # type: ignore
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         """forward pass of the multi-layer perceptron"""
         x = self.model(x)
         return x
@@ -62,15 +61,14 @@
     :param input_dim: Number of dimensions of the input feature map.
     :param classifier_hidden_dim: Number of dimensions of hidden features in the MLP.
     :param num_classes: Number of output classes per task.
     :param num_tasks: Number of classification tasks or heads required.
     """
 
     def __init__(self, input_dim: int, classifier_hidden_dim: Optional[int], num_classes: int, num_tasks: int):
-
         super().__init__()
 
         self.num_classes = num_classes
         self.num_tasks = num_tasks
 
         for task in range(num_tasks):
             # TODO check if softmax not needed here.
```

### Comparing `hi-ml-multimodal-0.2.0/src/health_multimodal/image/model/pretrained.py` & `hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/pretrained.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 #  -------------------------------------------------------------------------------------------
 
 from __future__ import annotations
 
 import tempfile
 from pathlib import Path
 
+from torch.hub import load_state_dict_from_url
 from torchvision.datasets.utils import download_url
+from torchvision.models.resnet import model_urls
 
 from .model import ImageModel
-from .types import ImageEncoderType
+from .types import ImageEncoderType, ImageEncoderWeightTypes
 
 
 JOINT_FEATURE_SIZE = 128
 
 BIOMED_VLP_CXR_BERT_SPECIALIZED = "microsoft/BiomedVLP-CXR-BERT-specialized"
 BIOMED_VLP_BIOVIL_T = "microsoft/BiomedVLP-BioViL-T"
 HF_URL = "https://huggingface.co"
@@ -24,15 +26,17 @@
 BIOVIL_T_COMMIT_TAG = "v1.0"
 
 BIOVIL_IMAGE_WEIGHTS_NAME = "biovil_image_resnet50_proj_size_128.pt"
 BIOVIL_IMAGE_WEIGHTS_URL = f"{HF_URL}/{BIOMED_VLP_CXR_BERT_SPECIALIZED}/resolve/{CXR_BERT_COMMIT_TAG}/{BIOVIL_IMAGE_WEIGHTS_NAME}"  # noqa: E501
 BIOVIL_IMAGE_WEIGHTS_MD5 = "02ce6ee460f72efd599295f440dbb453"
 
 BIOVIL_T_IMAGE_WEIGHTS_NAME = "biovil_t_image_model_proj_size_128.pt"
-BIOVIL_T_IMAGE_WEIGHTS_URL = f"{HF_URL}/{BIOMED_VLP_BIOVIL_T}/resolve/{BIOVIL_T_COMMIT_TAG}/{BIOVIL_T_IMAGE_WEIGHTS_NAME}"  # noqa: E501
+BIOVIL_T_IMAGE_WEIGHTS_URL = (
+    f"{HF_URL}/{BIOMED_VLP_BIOVIL_T}/resolve/{BIOVIL_T_COMMIT_TAG}/{BIOVIL_T_IMAGE_WEIGHTS_NAME}"  # noqa: E501
+)
 BIOVIL_T_IMAGE_WEIGHTS_MD5 = "a83080e2f23aa584a4f2b24c39b1bb64"
 
 
 def _download_biovil_image_model_weights() -> Path:
     """Download image model weights from Hugging Face.
 
     More information available at https://huggingface.co/microsoft/BiomedVLP-CXR-BERT-specialized.
@@ -50,18 +54,15 @@
 def _download_biovil_t_image_model_weights() -> Path:
     """Download image model weights from Hugging Face.
 
     More information available at https://huggingface.co/microsoft/microsoft/BiomedVLP-BioViL-T.
     """
     root_dir = tempfile.gettempdir()
     download_url(
-        BIOVIL_T_IMAGE_WEIGHTS_URL,
-        root=root_dir,
-        filename=BIOVIL_T_IMAGE_WEIGHTS_NAME,
-        md5=BIOVIL_T_IMAGE_WEIGHTS_MD5
+        BIOVIL_T_IMAGE_WEIGHTS_URL, root=root_dir, filename=BIOVIL_T_IMAGE_WEIGHTS_NAME, md5=BIOVIL_T_IMAGE_WEIGHTS_MD5
     )
     return Path(root_dir, BIOVIL_T_IMAGE_WEIGHTS_NAME)
 
 
 def get_biovil_image_encoder(pretrained: bool = True) -> ImageModel:
     """Download weights from Hugging Face and instantiate the image model."""
     resnet_checkpoint_path = _download_biovil_image_model_weights() if pretrained else None
@@ -75,11 +76,49 @@
 
 
 def get_biovil_t_image_encoder() -> ImageModel:
     """Download weights from Hugging Face and instantiate the image model."""
 
     biovilt_checkpoint_path = _download_biovil_t_image_model_weights()
     model_type = ImageEncoderType.RESNET50_MULTI_IMAGE
-    image_model = ImageModel(img_encoder_type=model_type,
-                             joint_feature_size=JOINT_FEATURE_SIZE,
-                             pretrained_model_path=biovilt_checkpoint_path)
+    image_model = ImageModel(
+        img_encoder_type=model_type,
+        joint_feature_size=JOINT_FEATURE_SIZE,
+        pretrained_model_path=biovilt_checkpoint_path,
+    )
+    return image_model
+
+
+def get_imagenet_init_encoder() -> ImageModel:
+    """Download ImageNet pre-trained weights and instantiate the image model."""
+
+    state_dict = load_state_dict_from_url(model_urls[ImageEncoderType.RESNET50])
+    image_model = ImageModel(
+        img_encoder_type=ImageEncoderType.RESNET50,
+        joint_feature_size=JOINT_FEATURE_SIZE,
+        pretrained_model_path=None,
+    )
+    image_model.encoder.encoder.load_state_dict(state_dict)
+    return image_model
+
+
+def get_image_encoder(weights: str) -> ImageModel:
+    """Instantiate image model with random or pre-trained weights.
+    :param weights: Select one of `random`, `imagenet`, `biovil`, `biovil_t`
+    """
+
+    if weights == ImageEncoderWeightTypes.RANDOM:
+        image_model = ImageModel(
+            img_encoder_type=ImageEncoderType.RESNET50,
+            joint_feature_size=JOINT_FEATURE_SIZE,
+            pretrained_model_path=None,
+        )
+    elif weights == ImageEncoderWeightTypes.IMAGENET:
+        image_model = get_imagenet_init_encoder()
+    elif weights == ImageEncoderWeightTypes.BIOVIL:
+        image_model = get_biovil_image_encoder()
+    elif weights == ImageEncoderWeightTypes.BIOVIL_T:
+        image_model = get_biovil_t_image_encoder()
+    else:
+        raise ValueError(f"Weights option not found: {weights}")
+
     return image_model
```

### Comparing `hi-ml-multimodal-0.2.0/src/health_multimodal/image/model/resnet.py` & `hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/resnet.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,17 @@
     The forward function is updated to return the penultimate layer
     activations, which are required to obtain image patch embeddings.
     """
 
     def __init__(self, **kwargs: Any) -> None:
         super().__init__(**kwargs)
 
-    def forward(self, x: torch.Tensor,
-                return_intermediate_layers: bool = False) -> Union[torch.Tensor, TypeSkipConnections]:
+    def forward(
+        self, x: torch.Tensor, return_intermediate_layers: bool = False
+    ) -> Union[torch.Tensor, TypeSkipConnections]:
         """ResNetHIML forward pass. Optionally returns intermediate layers using the
         ``return_intermediate_layers`` argument.
 
         :param return_intermediate_layers: If ``True``, return layers x0-x4 as a tuple,
             otherwise return x4 only.
         """
 
@@ -43,16 +44,22 @@
 
         if return_intermediate_layers:
             return x0, x1, x2, x3, x4
         else:
             return x4
 
 
-def _resnet(arch: str, block: Type[Union[BasicBlock, Bottleneck]], layers: List[int],
-            pretrained: bool, progress: bool, **kwargs: Any) -> ResNetHIML:
+def _resnet(
+    arch: str,
+    block: Type[Union[BasicBlock, Bottleneck]],
+    layers: List[int],
+    pretrained: bool,
+    progress: bool,
+    **kwargs: Any
+) -> ResNetHIML:
     """Instantiate a custom :class:`ResNet` model.
 
     Adapted from :mod:`torchvision.models.resnet`.
     """
     model = ResNetHIML(block=block, layers=layers, **kwargs)
     if pretrained:
         state_dict = load_state_dict_from_url(model_urls[arch], progress=progress)
```

### Comparing `hi-ml-multimodal-0.2.0/src/health_multimodal/image/model/transformer.py` & `hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,34 +28,44 @@
     :param num_blocks: Number of blocks per attention layer
     :param norm_layer: Normalisation layer
 
     `self.type_embed`: Is used to characterise prior and current scans, and
                        create permutation variance across modalities/series.
     """
 
-    def __init__(self,
-                 input_dim: int,
-                 grid_shape: Tuple[int, int],
-                 num_heads: int = 8,
-                 num_blocks: int = 3,
-                 norm_layer: Any = partial(nn.LayerNorm, eps=1e-6)):
+    def __init__(
+        self,
+        input_dim: int,
+        grid_shape: Tuple[int, int],
+        num_heads: int = 8,
+        num_blocks: int = 3,
+        norm_layer: Any = partial(nn.LayerNorm, eps=1e-6),
+    ):
         super().__init__()
 
-        block_kwargs = dict(dim=input_dim, num_heads=num_heads, mlp_ratio=1., drop=0.10, attn_drop=0.10,
-                            drop_path=0.25, act_layer=nn.GELU, norm_layer=norm_layer)
+        block_kwargs = dict(
+            dim=input_dim,
+            num_heads=num_heads,
+            mlp_ratio=1.0,
+            drop=0.10,
+            attn_drop=0.10,
+            drop_path=0.25,
+            act_layer=nn.GELU,
+            norm_layer=norm_layer,
+        )
         self.blocks = nn.ModuleList([Block(**block_kwargs) for _ in range(num_blocks)])
         self.norm_post = norm_layer(input_dim)
         self.grid_shape = grid_shape
         self.num_patches = grid_shape[0] * grid_shape[1]
         self.num_blocks = num_blocks
 
         # Temporal positional embeddings
         num_series: int = 2
         self.type_embed = nn.Parameter(torch.zeros(num_series, 1, input_dim))
-        trunc_normal_(self.type_embed, std=.02)
+        trunc_normal_(self.type_embed, std=0.02)
 
         # Positional embeddings 1 x L x C (L: Sequence length, C: Feature dimension)
         self.pos_drop = nn.Dropout(p=0.10)
         pos_embed_class = SinePositionEmbedding(embedding_dim=input_dim // 2, normalize=True)
         pos_embed = pos_embed_class(mask=torch.ones([1, grid_shape[0], grid_shape[1]]))  # 1 x L x C
         self.register_buffer("pos_embed", pos_embed, persistent=False)
 
@@ -77,23 +87,22 @@
         pos_embed = self.pos_embed.repeat(B, 1, 1)  # type: ignore
 
         # Final token activations (B x 2L x C)
         token_features = self.forward_after_reshape(x=current_image, pos_embed=pos_embed, x_previous=previous_image)
 
         # Extract the patch features of current image
         cur_img_token_id = 0
-        current_token_features = token_features[:, cur_img_token_id:self.num_patches+cur_img_token_id]
+        current_token_features = token_features[:, cur_img_token_id : self.num_patches + cur_img_token_id]
         current_patch_features = current_token_features.transpose(1, 2).view(B, C, H, W)
 
         return current_patch_features
 
-    def forward_after_reshape(self,
-                              x: torch.Tensor,
-                              pos_embed: torch.Tensor,
-                              x_previous: Optional[torch.Tensor] = None) -> torch.Tensor:
+    def forward_after_reshape(
+        self, x: torch.Tensor, pos_embed: torch.Tensor, x_previous: Optional[torch.Tensor] = None
+    ) -> torch.Tensor:
         B, L, _ = x.shape  # Batch, Sequence length, Feature dimension
 
         # Positional and type embeddings
         type_embed = self.type_embed[0].expand(B, L, -1)
         if x_previous is not None:
             x = torch.cat((x, x_previous), dim=1)
             pos_embed = torch.cat((pos_embed, pos_embed), dim=1)
@@ -111,15 +120,15 @@
             x = block(x=x, pos_and_type_embed=pos_and_type_embed)
         x = self.norm_post(x)
 
         return x
 
     def _init_weights(self, m: nn.Module) -> None:
         if isinstance(m, nn.Linear):
-            trunc_normal_(m.weight, std=.02)
+            trunc_normal_(m.weight, std=0.02)
             if isinstance(m, nn.Linear) and m.bias is not None:
                 nn.init.constant_(m.bias, 0)
         elif isinstance(m, nn.LayerNorm):
             nn.init.constant_(m.bias, 0)
             nn.init.constant_(m.weight, 1.0)
 
 
@@ -130,39 +139,37 @@
     The content builds on top of the TIMM library (vision_transformer.py) and differs by the following:
         - Defines a custom `MultiHeadAttentionLayer` which does not only apply `self-attention` but it can be
             generalised to arbitrary (query, key, value) input tuples. This feature can be valuable to process
             more than 2 scans at a time.
         - `Self-attention` specific use-case can still be invoked by calling the `forward_as_mhsa` method.
     """
 
-    def __init__(self,
-                 dim: int,
-                 num_heads: int = 8,
-                 qkv_bias: bool = False,
-                 attn_drop: float = 0.,
-                 proj_drop: float = 0.) -> None:
+    def __init__(
+        self, dim: int, num_heads: int = 8, qkv_bias: bool = False, attn_drop: float = 0.0, proj_drop: float = 0.0
+    ) -> None:
         super().__init__()
         self.num_heads = num_heads
         assert dim % num_heads == 0, f"The embedding dim ({dim}) must be divisible by the number of heads ({num_heads})"
         head_dim = dim // num_heads
-        self.scale = head_dim ** -0.5
+        self.scale = head_dim**-0.5
         self.return_attention = False
 
         self.proj_q = nn.Linear(dim, dim, bias=qkv_bias)
         self.proj_k = nn.Linear(dim, dim, bias=qkv_bias)
         self.proj_v = nn.Linear(dim, dim, bias=qkv_bias)
 
         self.attn_drop = nn.Dropout(attn_drop)
         self.proj = nn.Linear(dim, dim)
         self.proj_drop = nn.Dropout(proj_drop)
 
     def forward(self, k: torch.Tensor, q: torch.Tensor, v: torch.Tensor) -> MultiHeadAttentionOutput:
         B, N, C = v.shape
-        assert C % self.num_heads == 0, \
-            f"The embedding dim ({C}) must be divisible by the number of heads ({self.num_heads})"
+        assert (
+            C % self.num_heads == 0
+        ), f"The embedding dim ({C}) must be divisible by the number of heads ({self.num_heads})"
 
         w_q = self.proj_q(q).reshape(B, N, self.num_heads, C // self.num_heads).permute(0, 2, 1, 3)
         w_k = self.proj_k(k).reshape(B, N, self.num_heads, C // self.num_heads).permute(0, 2, 1, 3)
         w_v = self.proj_v(v).reshape(B, N, self.num_heads, C // self.num_heads).permute(0, 2, 1, 3)
 
         attn = (w_q @ w_k.transpose(-2, -1)) * self.scale
         attn = attn.softmax(dim=-1)
@@ -191,22 +198,32 @@
             generalised to arbitrary (query, key, value) tuples. This can be valuable to process more than 2 scans.
 
     Positional and type embeddings are handled in a similar fashion as DETR object localisation paper
     https://alcinos.github.io/detr_page/, where a fixed set of sine/cos positional embeddings are used
     in an additive manner to Q and K tensors.
     """
 
-    def __init__(self, dim: int, num_heads: int, mlp_ratio: float = 1., qkv_bias: bool = False, drop: float = 0.,
-                 attn_drop: float = 0., drop_path: float = 0., act_layer: Callable = nn.GELU,
-                 norm_layer: Callable = nn.LayerNorm) -> None:
+    def __init__(
+        self,
+        dim: int,
+        num_heads: int,
+        mlp_ratio: float = 1.0,
+        qkv_bias: bool = False,
+        drop: float = 0.0,
+        attn_drop: float = 0.0,
+        drop_path: float = 0.0,
+        act_layer: Callable = nn.GELU,
+        norm_layer: Callable = nn.LayerNorm,
+    ) -> None:
         super().__init__()
         self.norm1 = norm_layer(dim)
-        self.attn = MultiHeadAttentionLayer(dim=dim, num_heads=num_heads, qkv_bias=qkv_bias,
-                                            attn_drop=attn_drop, proj_drop=drop)
-        self.drop_path = DropPath(drop_path) if drop_path > 0. else nn.Identity()
+        self.attn = MultiHeadAttentionLayer(
+            dim=dim, num_heads=num_heads, qkv_bias=qkv_bias, attn_drop=attn_drop, proj_drop=drop
+        )
+        self.drop_path = DropPath(drop_path) if drop_path > 0.0 else nn.Identity()
         self.norm2 = norm_layer(dim)
         mlp_hidden_dim = int(dim * mlp_ratio)
         self.mlp = Mlp(in_features=dim, hidden_features=mlp_hidden_dim, act_layer=act_layer, drop=drop)
 
     def with_pos_and_type_embed(self, tensor: torch.Tensor, emb: Optional[torch.Tensor]) -> torch.Tensor:
         # Add positional embeddings to key and query tensors
         return tensor if emb is None else tensor + emb
@@ -215,25 +232,23 @@
         x_with_emb = self.with_pos_and_type_embed(self.norm1(x), emb=pos_and_type_embed)
         x = x + self.drop_path(self.attn.forward_as_mhsa(x_with_emb).mha_output)
         x = x + self.drop_path(self.mlp(self.norm2(x)))
 
         return x
 
 
-class SinePositionEmbedding():
+class SinePositionEmbedding:
     """
     This is a more standard version of the position embedding, very similar to the one used by the Attention is all you
     need paper, generalized to work on images.
     """
 
-    def __init__(self,
-                 embedding_dim: int = 64,
-                 temperature: int = 10000,
-                 normalize: bool = False,
-                 scale: float = None) -> None:
+    def __init__(
+        self, embedding_dim: int = 64, temperature: int = 10000, normalize: bool = False, scale: Optional[float] = None
+    ) -> None:
         super().__init__()
         self.embedding_dim = embedding_dim
         self.temperature = temperature
         self.normalize = normalize
         if scale is not None and normalize is False:
             raise ValueError("normalize should be True if scale is passed")
         if scale is None:
```

### Comparing `hi-ml-multimodal-0.2.0/src/health_multimodal/image/model/types.py` & `hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from enum import Enum, unique
 from typing import List
 
 import torch
 
 
 @dataclass
-class ImageModelOutput():
+class ImageModelOutput:
     img_embedding: torch.Tensor
     patch_embeddings: torch.Tensor
     projected_global_embedding: torch.Tensor
     class_logits: torch.Tensor
     projected_patch_embeddings: torch.Tensor
 
 
@@ -31,7 +31,15 @@
 
     @classmethod
     def get_members(cls, multi_image_encoders_only: bool) -> List[ImageEncoderType]:
         if multi_image_encoders_only:
             return [cls.RESNET18_MULTI_IMAGE, cls.RESNET50_MULTI_IMAGE]
         else:
             return [member for member in cls]
+
+
+@unique
+class ImageEncoderWeightTypes(str, Enum):
+    RANDOM = "random"
+    IMAGENET = "imagenet"
+    BIOVIL = "biovil"
+    BIOVIL_T = "biovil_t"
```

### Comparing `hi-ml-multimodal-0.2.0/src/health_multimodal/image/utils.py` & `hi-ml-multimodal-0.2.1/src/health_multimodal/image/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,12 +34,12 @@
     elif image_model_type == ImageModelType.BIOVIL:
         image_model = get_biovil_image_encoder()
         transform_center_crop_size = 480
     else:
         raise ValueError(f"Unknown image_model_type: {image_model_type}")
 
     transform = create_chest_xray_transform_for_inference(
-        resize=TRANSFORM_RESIZE,
-        center_crop_size=transform_center_crop_size)
+        resize=TRANSFORM_RESIZE, center_crop_size=transform_center_crop_size
+    )
     image_inference = ImageInferenceEngine(image_model=image_model, transform=transform)
 
     return image_inference
```

### Comparing `hi-ml-multimodal-0.2.0/src/health_multimodal/text/__init__.py` & `hi-ml-multimodal-0.2.1/src/health_multimodal/text/__init__.py`

 * *Files identical despite different names*

### Comparing `hi-ml-multimodal-0.2.0/src/health_multimodal/text/data/io.py` & `hi-ml-multimodal-0.2.1/src/health_multimodal/text/data/io.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,18 +35,17 @@
         :param verbose: If set to True, will log the sentence after tokenization.
         :return: A 2D tensor containing the tokenized sentences
         """
         prompts = [prompts] if isinstance(prompts, str) else prompts
         self.assert_special_tokens_not_present(" ".join(prompts))
 
         prompts = [prompt.rstrip("!?.") for prompt in prompts]  # removes punctuation from end of prompt
-        tokenizer_output = self.tokenizer.batch_encode_plus(batch_text_or_text_pairs=prompts,
-                                                            add_special_tokens=True,
-                                                            padding='longest',
-                                                            return_tensors='pt')
+        tokenizer_output = self.tokenizer.batch_encode_plus(
+            batch_text_or_text_pairs=prompts, add_special_tokens=True, padding='longest', return_tensors='pt'
+        )
         if verbose:
             for prompt in tokenizer_output.input_ids:
                 input_tokens = self.tokenizer.convert_ids_to_tokens(prompt.tolist())
                 logger.info(f"Input tokens: {input_tokens}")
 
         return tokenizer_output
```

### Comparing `hi-ml-multimodal-0.2.0/src/health_multimodal/text/inference_engine.py` & `hi-ml-multimodal-0.2.1/src/health_multimodal/text/inference_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,45 +38,47 @@
         tokenizer_output = super().tokenize_input_prompts(prompts, verbose=verbose)
         device = next(self.model.parameters()).device
         tokenizer_output.input_ids = tokenizer_output.input_ids.to(device)
         tokenizer_output.attention_mask = tokenizer_output.attention_mask.to(device)
 
         max_length = tokenizer_output.input_ids.shape[1]
         if tokenizer_output.input_ids.shape[1] > self.max_allowed_input_length:
-            raise ValueError(f"The sequence length of the input ({max_length}) is "
-                             f"longer than the maximum allowed sequence length ({self.max_allowed_input_length}).")
+            raise ValueError(
+                f"The sequence length of the input ({max_length}) is "
+                f"longer than the maximum allowed sequence length ({self.max_allowed_input_length})."
+            )
 
         return tokenizer_output
 
     @torch.no_grad()
-    def get_embeddings_from_prompt(self,
-                                   prompts: Union[str, List[str]],
-                                   normalize: bool = True,
-                                   verbose: bool = True) -> torch.Tensor:
+    def get_embeddings_from_prompt(
+        self, prompts: Union[str, List[str]], normalize: bool = True, verbose: bool = True
+    ) -> torch.Tensor:
         """Generate L2-normalised embeddings for a list of input text prompts.
 
         :param prompts: Input text prompt(s) either in string or list of string format.
         :param normalize: If True, L2-normalise the embeddings.
         :param verbose: If set to True, tokenized words are displayed in the console.
         :return: Tensor of shape (batch_size, embedding_size).
         """
 
         assert self.is_in_eval()
         tokenizer_output = self.tokenize_input_prompts(prompts=prompts, verbose=verbose)
         txt_emb = self.model.get_projected_text_embeddings(  # type: ignore
             input_ids=tokenizer_output.input_ids,
             attention_mask=tokenizer_output.attention_mask,
-            normalize_embeddings=normalize)
+            normalize_embeddings=normalize,
+        )
 
         return txt_emb
 
     @torch.no_grad()
-    def get_pairwise_similarities(self,
-                                  prompt_set_1: Union[str, List[str]],
-                                  prompt_set_2: Union[str, List[str]]) -> torch.Tensor:
+    def get_pairwise_similarities(
+        self, prompt_set_1: Union[str, List[str]], prompt_set_2: Union[str, List[str]]
+    ) -> torch.Tensor:
         """Compute pairwise cosine similarities between the embeddings of the given prompts."""
 
         emb_1 = self.get_embeddings_from_prompt(prompts=prompt_set_1, verbose=False)
         emb_2 = self.get_embeddings_from_prompt(prompts=prompt_set_2, verbose=False)
         sim = torch.diag(torch.mm(emb_1, emb_2.t())).detach()
 
         return sim
@@ -93,16 +95,17 @@
 
         assert self.is_in_eval()
 
         # Tokenize the input prompts
         tokenized_prompts = self.tokenize_input_prompts(prompts)
 
         # Collect all token predictions
-        text_model_output = self.model.forward(input_ids=tokenized_prompts.input_ids,
-                                               attention_mask=tokenized_prompts.attention_mask)
+        text_model_output = self.model.forward(
+            input_ids=tokenized_prompts.input_ids, attention_mask=tokenized_prompts.attention_mask
+        )
         logits = text_model_output.logits
         logits = logits.detach()
 
         predicted_token_ids = torch.argmax(logits, dim=-1)  # Batch x Seq
 
         # Identify the masked token indices
         batch_size = predicted_token_ids.shape[0]
```

### Comparing `hi-ml-multimodal-0.2.0/src/health_multimodal/text/model/__init__.py` & `hi-ml-multimodal-0.2.1/src/health_multimodal/text/model/__init__.py`

 * *Files identical despite different names*

### Comparing `hi-ml-multimodal-0.2.0/src/health_multimodal/text/model/configuration_cxrbert.py` & `hi-ml-multimodal-0.2.1/src/health_multimodal/text/model/configuration_cxrbert.py`

 * *Files identical despite different names*

### Comparing `hi-ml-multimodal-0.2.0/src/health_multimodal/text/model/modelling_cxrbert.py` & `hi-ml-multimodal-0.2.1/src/health_multimodal/text/model/modelling_cxrbert.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,30 +77,32 @@
         inputs_embeds: Optional[torch.Tensor] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         output_cls_projected_embedding: Optional[bool] = None,
         return_dict: Optional[bool] = None,
         **kwargs: Any
     ) -> Union[BERTTupleOutput, CXRBertOutput]:
-
         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
 
-        bert_for_masked_lm_output = super().forward(input_ids=input_ids,
-                                                    attention_mask=attention_mask,
-                                                    token_type_ids=token_type_ids,
-                                                    position_ids=position_ids,
-                                                    head_mask=head_mask,
-                                                    inputs_embeds=inputs_embeds,
-                                                    output_attentions=output_attentions,
-                                                    output_hidden_states=True,
-                                                    return_dict=True)
+        bert_for_masked_lm_output = super().forward(
+            input_ids=input_ids,
+            attention_mask=attention_mask,
+            token_type_ids=token_type_ids,
+            position_ids=position_ids,
+            head_mask=head_mask,
+            inputs_embeds=inputs_embeds,
+            output_attentions=output_attentions,
+            output_hidden_states=True,
+            return_dict=True,
+        )
 
         last_hidden_state = bert_for_masked_lm_output.hidden_states[-1]
-        cls_projected_embedding = self.cls_projection_head(
-            last_hidden_state[:, 0, :]) if output_cls_projected_embedding else None
+        cls_projected_embedding = (
+            self.cls_projection_head(last_hidden_state[:, 0, :]) if output_cls_projected_embedding else None
+        )
 
         if return_dict:
             return CXRBertOutput(
                 last_hidden_state=last_hidden_state,
                 logits=bert_for_masked_lm_output.logits,
                 cls_projected_embedding=cls_projected_embedding,
                 hidden_states=bert_for_masked_lm_output.hidden_states if output_hidden_states else None,
@@ -108,32 +110,33 @@
             )
         else:
             return (
                 last_hidden_state,
                 bert_for_masked_lm_output.logits,
                 cls_projected_embedding,
                 bert_for_masked_lm_output.hidden_states,
-                bert_for_masked_lm_output.attentions,)
+                bert_for_masked_lm_output.attentions,
+            )
 
-    def get_projected_text_embeddings(self,
-                                      input_ids: torch.Tensor,
-                                      attention_mask: torch.Tensor,
-                                      normalize_embeddings: bool = True) -> torch.Tensor:
+    def get_projected_text_embeddings(
+        self, input_ids: torch.Tensor, attention_mask: torch.Tensor, normalize_embeddings: bool = True
+    ) -> torch.Tensor:
         """
         Returns l2-normalised projected cls token embeddings for the given input token ids and attention mask.
         The joint latent space is trained using a contrastive objective between image and text data modalities.
 
         :param input_ids: (batch_size, sequence_length)
         :param attention_mask: (batch_size, sequence_length)
         :param normalize_embeddings: Whether to l2-normalise the embeddings.
         :return: (batch_size, projection_size)
         """
 
-        outputs = self.forward(input_ids=input_ids, attention_mask=attention_mask,
-                               output_cls_projected_embedding=True, return_dict=True)
+        outputs = self.forward(
+            input_ids=input_ids, attention_mask=attention_mask, output_cls_projected_embedding=True, return_dict=True
+        )
         assert isinstance(outputs, CXRBertOutput)
 
         cls_projected_embedding = outputs.cls_projected_embedding
         assert cls_projected_embedding is not None
 
         if normalize_embeddings:
             return F.normalize(cls_projected_embedding, dim=1)
```

### Comparing `hi-ml-multimodal-0.2.0/src/health_multimodal/text/utils.py` & `hi-ml-multimodal-0.2.1/src/health_multimodal/text/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,35 +3,39 @@
 #  Licensed under the MIT License (MIT). See LICENSE in the repo root for license information.
 #  -------------------------------------------------------------------------------------------
 
 
 from enum import Enum, unique
 from typing import Tuple
 
-from ..image.model.pretrained import (BIOMED_VLP_BIOVIL_T, BIOMED_VLP_CXR_BERT_SPECIALIZED, BIOVIL_T_COMMIT_TAG,
-                                      CXR_BERT_COMMIT_TAG)
+from ..image.model.pretrained import (
+    BIOMED_VLP_BIOVIL_T,
+    BIOMED_VLP_CXR_BERT_SPECIALIZED,
+    BIOVIL_T_COMMIT_TAG,
+    CXR_BERT_COMMIT_TAG,
+)
 from .inference_engine import TextInferenceEngine
 from .model import CXRBertModel, CXRBertTokenizer
 
 
 @unique
 class BertEncoderType(str, Enum):
     CXR_BERT = "cxr_bert"
     BIOVIL_T_BERT = "biovil_t_bert"
 
 
 def get_biovil_t_bert() -> Tuple[CXRBertTokenizer, CXRBertModel]:
-    """Load the BioViL-T Bert model and tokenizer from the `Hugging Face Hub <https://huggingface.co/microsoft/BiomedVLP-BioViL-T>`_."""  # noqa: E501
+    """Load the BioViL-T Bert model and tokenizer from the `Hugging Face Hub <https://huggingface.co/microsoft/BiomedVLP-BioViL-T>`_."""  # noqa: B950
     tokenizer = CXRBertTokenizer.from_pretrained(BIOMED_VLP_BIOVIL_T, revision=BIOVIL_T_COMMIT_TAG)
     text_model = CXRBertModel.from_pretrained(BIOMED_VLP_BIOVIL_T, revision=BIOVIL_T_COMMIT_TAG)
     return tokenizer, text_model
 
 
 def get_cxr_bert() -> Tuple[CXRBertTokenizer, CXRBertModel]:
-    """Load the CXR-BERT model and tokenizer from the `Hugging Face Hub <https://huggingface.co/microsoft/BiomedVLP-CXR-BERT-specialized>`_."""  # noqa: E501
+    """Load the CXR-BERT model and tokenizer from the `Hugging Face Hub <https://huggingface.co/microsoft/BiomedVLP-CXR-BERT-specialized>`_."""  # noqa: B950
     tokenizer = CXRBertTokenizer.from_pretrained(BIOMED_VLP_CXR_BERT_SPECIALIZED, revision=CXR_BERT_COMMIT_TAG)
     text_model = CXRBertModel.from_pretrained(BIOMED_VLP_CXR_BERT_SPECIALIZED, revision=CXR_BERT_COMMIT_TAG)
     return tokenizer, text_model
 
 
 def get_bert_inference(bert_encoder_type: BertEncoderType = BertEncoderType.BIOVIL_T_BERT) -> TextInferenceEngine:
     """Create a :class:`TextInferenceEngine` for a text encoder model.
```

### Comparing `hi-ml-multimodal-0.2.0/src/health_multimodal/vlp/__init__.py` & `hi-ml-multimodal-0.2.1/src/health_multimodal/vlp/__init__.py`

 * *Files identical despite different names*

### Comparing `hi-ml-multimodal-0.2.0/src/health_multimodal/vlp/inference_engine.py` & `hi-ml-multimodal-0.2.1/src/health_multimodal/vlp/inference_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,24 +17,22 @@
 from health_multimodal.image import ImageInferenceEngine
 from health_multimodal.text import TextInferenceEngine
 
 
 class ImageTextInferenceEngine:
     """Functions related to inference on :class:`ImageTextModel`."""
 
-    def __init__(self,
-                 image_inference_engine: ImageInferenceEngine,
-                 text_inference_engine: TextInferenceEngine) -> None:
+    def __init__(
+        self, image_inference_engine: ImageInferenceEngine, text_inference_engine: TextInferenceEngine
+    ) -> None:
         self.image_inference_engine = image_inference_engine
         self.text_inference_engine = text_inference_engine
 
     @torch.no_grad()
-    def get_similarity_score_from_raw_data(self,
-                                           image_path: Path,
-                                           query_text: Union[List[str], str]) -> float:
+    def get_similarity_score_from_raw_data(self, image_path: Path, query_text: Union[List[str], str]) -> float:
         """Compute the cosine similarity score between an image and one or more strings.
 
         If multiple strings are passed, their embeddings are averaged before L2-normalization.
 
         :param image_path: Path to the input chest X-ray, either a DICOM or JPEG file.
         :param query_text: Input radiology text phrase.
         :return: The similarity score between the image and the text.
@@ -52,18 +50,17 @@
         text_embedding = text_embedding.mean(dim=0)
         text_embedding = F.normalize(text_embedding, dim=0, p=2)
 
         cos_similarity = image_embedding @ text_embedding.t()
 
         return cos_similarity.item()
 
-    def get_similarity_map_from_raw_data(self,
-                                         image_path: Path,
-                                         query_text: str,
-                                         interpolation: str = "nearest") -> np.ndarray:
+    def get_similarity_map_from_raw_data(
+        self, image_path: Path, query_text: str, interpolation: str = "nearest"
+    ) -> np.ndarray:
         """Return a heatmap of the similarities between each patch embedding from the image and the text embedding.
 
         :param image_path: Path to the input chest X-ray, either a DICOM or JPEG file.
         :param query_text: Input radiology text phrase.
         :param interpolation: Interpolation method to upsample the heatmap so it matches the input image size.
             See :func:`torch.nn.functional.interpolate` for more details.
         :return: A heatmap of the similarities between each patch embedding from the image and the text embedding,
@@ -87,38 +84,44 @@
             crop_size=self.image_inference_engine.crop_size,
             val_img_transform=self.image_inference_engine.transform,
             interpolation=interpolation,
         )
         return resized_sim_map
 
     @staticmethod
-    def _get_similarity_map_from_embeddings(projected_patch_embeddings: torch.Tensor,
-                                            projected_text_embeddings: torch.Tensor,
-                                            sigma: float = 1.5) -> torch.Tensor:
+    def _get_similarity_map_from_embeddings(
+        projected_patch_embeddings: torch.Tensor, projected_text_embeddings: torch.Tensor, sigma: float = 1.5
+    ) -> torch.Tensor:
         """Get smoothed similarity map for a given image patch embeddings and text embeddings.
 
         :param projected_patch_embeddings: [n_patches_h, n_patches_w, feature_size]
         :param projected_text_embeddings: [1, feature_size]
         :return: similarity_map: similarity map of shape [n_patches_h, n_patches_w]
         """
         n_patches_h, n_patches_w, feature_size = projected_patch_embeddings.shape
         assert feature_size == projected_text_embeddings.shape[1]
         assert projected_text_embeddings.shape[0] == 1
         assert projected_text_embeddings.dim() == 2
         patch_wise_similarity = projected_patch_embeddings.view(-1, feature_size) @ projected_text_embeddings.t()
         patch_wise_similarity = patch_wise_similarity.reshape(n_patches_h, n_patches_w).cpu().numpy()
-        smoothed_similarity_map = torch.tensor(ndimage.gaussian_filter(
-            patch_wise_similarity, sigma=(sigma, sigma), order=0))
+        smoothed_similarity_map = torch.tensor(
+            ndimage.gaussian_filter(patch_wise_similarity, sigma=(sigma, sigma), order=0)
+        )
         return smoothed_similarity_map
 
     @staticmethod
     def convert_similarity_to_image_size(
-            similarity_map: torch.Tensor, width: int, height: int, resize_size: Optional[int],
-            crop_size: Optional[int], val_img_transform: Optional[Callable] = None,
-            interpolation: str = "nearest") -> np.ndarray:
+        similarity_map: torch.Tensor,
+        width: int,
+        height: int,
+        resize_size: Optional[int],
+        crop_size: Optional[int],
+        val_img_transform: Optional[Callable] = None,
+        interpolation: str = "nearest",
+    ) -> np.ndarray:
         """
         Convert similarity map from raw patch grid to original image size,
         taking into account whether the image has been resized and/or cropped prior to entering the network.
         """
         n_patches_h, n_patches_w = similarity_map.shape[0], similarity_map.shape[1]
         target_shape = 1, 1, n_patches_h, n_patches_w
         smallest_dimension = min(height, width)
```

### Comparing `hi-ml-multimodal-0.2.0/src/hi_ml_multimodal.egg-info/PKG-INFO` & `hi-ml-multimodal-0.2.1/src/hi_ml_multimodal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: hi-ml-multimodal
-Version: 0.2.0
+Version: 0.2.1
 Summary: Microsoft Health Futures package to work with multi-modal health data
 Home-page: https://github.com/microsoft/hi-ml
 Author: Biomedical Imaging Team @ Microsoft Health Futures
 Author-email: innereyedev@microsoft.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 # HI-ML Multimodal Toolbox
 
 This toolbox provides models for multimodal health data.
 The code is available on [GitHub][1] and [Hugging Face 🤗][6].
 
 ## Getting started
 
 The best way to get started is by running the [phrase grounding notebook][2] and the [examples](#examples).
-All the dependencies will be installed upon execution, so Python 3.7 and [Jupyter][3] are the only requirements to get started.
+All the dependencies will be installed upon execution, so Python 3.9 and [Jupyter][3] are the only requirements to get started.
 
 The notebook can also be run on [Binder][4], without the need to download any code or install any libraries:
 
 [![Binder](https://mybinder.org/badge_logo.svg)][4]
 
 ## Installation
```

### Comparing `hi-ml-multimodal-0.2.0/src/hi_ml_multimodal.egg-info/SOURCES.txt` & `hi-ml-multimodal-0.2.1/src/hi_ml_multimodal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

