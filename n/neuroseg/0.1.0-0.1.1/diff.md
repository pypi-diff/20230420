# Comparing `tmp/neuroseg-0.1.0.tar.gz` & `tmp/neuroseg-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroseg-0.1.0.tar", last modified: Tue Apr 18 18:17:00 2023, max compression
+gzip compressed data, was "neuroseg-0.1.1.tar", last modified: Thu Apr 20 20:13:14 2023, max compression
```

## Comparing `neuroseg-0.1.0.tar` & `neuroseg-0.1.1.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2023-04-18 18:16:59.993296 neuroseg-0.1.0/
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     1541 2023-04-18 17:58:36.000000 neuroseg-0.1.0/LICENSE
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      143 2023-04-18 18:16:59.994893 neuroseg-0.1.0/PKG-INFO
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)       59 2023-04-18 18:15:07.000000 neuroseg-0.1.0/README.md
-drwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2023-04-18 18:16:59.632762 neuroseg-0.1.0/neuroseg/
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2021-09-21 07:00:56.000000 neuroseg-0.1.0/neuroseg/__init__.py
-drwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2023-04-18 18:16:59.722855 neuroseg-0.1.0/neuroseg/core/
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2021-09-21 07:00:56.000000 neuroseg-0.1.0/neuroseg/core/__init__.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     2487 2023-04-14 17:25:14.000000 neuroseg-0.1.0/neuroseg/core/predictor.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     2840 2023-04-14 17:25:13.000000 neuroseg-0.1.0/neuroseg/core/predictor_multilabel.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     7749 2023-04-14 17:25:13.000000 neuroseg-0.1.0/neuroseg/core/trainer.py
-drwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2023-04-18 18:16:59.792888 neuroseg-0.1.0/neuroseg/datasets/
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2021-09-21 07:00:57.000000 neuroseg-0.1.0/neuroseg/datasets/__init__.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)    24432 2023-04-14 17:25:14.000000 neuroseg-0.1.0/neuroseg/datasets/dataset.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)    10402 2021-09-21 07:00:57.000000 neuroseg-0.1.0/neuroseg/datasets/datatypes.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     3910 2023-04-14 17:25:14.000000 neuroseg-0.1.0/neuroseg/datasets/filetypes.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     3612 2023-04-14 17:25:15.000000 neuroseg-0.1.0/neuroseg/datasets/specification.py
-drwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2023-04-18 18:16:59.855739 neuroseg-0.1.0/neuroseg/nets/
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     7116 2023-04-14 17:25:13.000000 neuroseg-0.1.0/neuroseg/nets/RSUNet.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     7186 2023-04-14 17:25:12.000000 neuroseg-0.1.0/neuroseg/nets/RSUNetMulti.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2021-09-21 07:00:57.000000 neuroseg-0.1.0/neuroseg/nets/__init__.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     3597 2021-09-21 07:00:58.000000 neuroseg-0.1.0/neuroseg/nets/layers.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      582 2023-04-14 17:25:16.000000 neuroseg-0.1.0/neuroseg/nets/netcollector.py
-drwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2023-04-18 18:16:59.900622 neuroseg-0.1.0/neuroseg/training/
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2021-09-21 07:01:09.000000 neuroseg-0.1.0/neuroseg/training/__init__.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     1929 2023-04-14 17:25:12.000000 neuroseg-0.1.0/neuroseg/training/checkpoint.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     6747 2023-04-14 17:25:12.000000 neuroseg-0.1.0/neuroseg/training/logging.py
-drwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2023-04-18 18:16:59.671656 neuroseg-0.1.0/neuroseg.egg-info/
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      143 2023-04-18 18:16:59.000000 neuroseg-0.1.0/neuroseg.egg-info/PKG-INFO
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      815 2023-04-18 18:16:59.000000 neuroseg-0.1.0/neuroseg.egg-info/SOURCES.txt
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        1 2023-04-18 18:16:59.000000 neuroseg-0.1.0/neuroseg.egg-info/dependency_links.txt
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)       15 2023-04-18 18:16:59.000000 neuroseg-0.1.0/neuroseg.egg-info/top_level.txt
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      153 2023-04-18 18:17:00.006347 neuroseg-0.1.0/setup.cfg
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      272 2023-04-18 18:16:30.000000 neuroseg-0.1.0/setup.py
-drwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2023-04-18 18:16:59.984855 neuroseg-0.1.0/tests/
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)        0 2021-09-21 07:01:10.000000 neuroseg-0.1.0/tests/__init__.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     4052 2023-04-14 17:25:13.000000 neuroseg-0.1.0/tests/test_augmentations.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     7307 2023-04-14 17:25:14.000000 neuroseg-0.1.0/tests/test_core.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)     7842 2023-04-14 17:25:13.000000 neuroseg-0.1.0/tests/test_dataset.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      184 2023-04-14 17:25:14.000000 neuroseg-0.1.0/tests/test_net.py
--rwxrwxr-x   0 matt.mallory (20150) domain_users (10513)      834 2023-04-14 17:25:12.000000 neuroseg-0.1.0/tests/test_reconstruction.py
+drwxrwxr-x   0 matt.mallory (20150) domain users (10513)        0 2023-04-20 20:13:14.266587 neuroseg-0.1.1/
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)     1541 2023-04-18 17:58:36.000000 neuroseg-0.1.1/LICENSE
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)      185 2023-04-20 20:13:14.267913 neuroseg-0.1.1/PKG-INFO
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)       59 2023-04-18 18:15:07.000000 neuroseg-0.1.1/README.md
+drwxrwxr-x   0 matt.mallory (20150) domain users (10513)        0 2023-04-20 20:13:14.039979 neuroseg-0.1.1/neuroseg/
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)        0 2021-09-21 07:00:56.000000 neuroseg-0.1.1/neuroseg/__init__.py
+drwxrwxr-x   0 matt.mallory (20150) domain users (10513)        0 2023-04-20 20:13:14.111489 neuroseg-0.1.1/neuroseg/core/
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)        0 2021-09-21 07:00:56.000000 neuroseg-0.1.1/neuroseg/core/__init__.py
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)     2487 2023-04-14 17:25:14.000000 neuroseg-0.1.1/neuroseg/core/predictor.py
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)     2840 2023-04-14 17:25:13.000000 neuroseg-0.1.1/neuroseg/core/predictor_multilabel.py
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)     7749 2023-04-14 17:25:13.000000 neuroseg-0.1.1/neuroseg/core/trainer.py
+drwxrwxr-x   0 matt.mallory (20150) domain users (10513)        0 2023-04-20 20:13:14.150118 neuroseg-0.1.1/neuroseg/datasets/
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)        0 2021-09-21 07:00:57.000000 neuroseg-0.1.1/neuroseg/datasets/__init__.py
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)    24432 2023-04-14 17:25:14.000000 neuroseg-0.1.1/neuroseg/datasets/dataset.py
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)    10402 2021-09-21 07:00:57.000000 neuroseg-0.1.1/neuroseg/datasets/datatypes.py
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)     3910 2023-04-14 17:25:14.000000 neuroseg-0.1.1/neuroseg/datasets/filetypes.py
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)     3612 2023-04-14 17:25:15.000000 neuroseg-0.1.1/neuroseg/datasets/specification.py
+drwxrwxr-x   0 matt.mallory (20150) domain users (10513)        0 2023-04-20 20:13:14.194423 neuroseg-0.1.1/neuroseg/nets/
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)     7116 2023-04-14 17:25:13.000000 neuroseg-0.1.1/neuroseg/nets/RSUNet.py
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)     7186 2023-04-14 17:25:12.000000 neuroseg-0.1.1/neuroseg/nets/RSUNetMulti.py
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)        0 2021-09-21 07:00:57.000000 neuroseg-0.1.1/neuroseg/nets/__init__.py
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)     3597 2021-09-21 07:00:58.000000 neuroseg-0.1.1/neuroseg/nets/layers.py
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)      582 2023-04-14 17:25:16.000000 neuroseg-0.1.1/neuroseg/nets/netcollector.py
+drwxrwxr-x   0 matt.mallory (20150) domain users (10513)        0 2023-04-20 20:13:14.216568 neuroseg-0.1.1/neuroseg/training/
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)        0 2021-09-21 07:01:09.000000 neuroseg-0.1.1/neuroseg/training/__init__.py
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)     1929 2023-04-14 17:25:12.000000 neuroseg-0.1.1/neuroseg/training/checkpoint.py
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)     6747 2023-04-14 17:25:12.000000 neuroseg-0.1.1/neuroseg/training/logging.py
+drwxrwxr-x   0 matt.mallory (20150) domain users (10513)        0 2023-04-20 20:13:14.078567 neuroseg-0.1.1/neuroseg.egg-info/
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)      185 2023-04-20 20:13:12.000000 neuroseg-0.1.1/neuroseg.egg-info/PKG-INFO
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)      846 2023-04-20 20:13:12.000000 neuroseg-0.1.1/neuroseg.egg-info/SOURCES.txt
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)        1 2023-04-20 20:13:12.000000 neuroseg-0.1.1/neuroseg.egg-info/dependency_links.txt
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)      123 2023-04-20 20:13:12.000000 neuroseg-0.1.1/neuroseg.egg-info/requires.txt
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)       15 2023-04-20 20:13:12.000000 neuroseg-0.1.1/neuroseg.egg-info/top_level.txt
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)      153 2023-04-20 20:13:14.273508 neuroseg-0.1.1/setup.cfg
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)      466 2023-04-20 20:12:57.000000 neuroseg-0.1.1/setup.py
+drwxrwxr-x   0 matt.mallory (20150) domain users (10513)        0 2023-04-20 20:13:14.260702 neuroseg-0.1.1/tests/
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)        0 2021-09-21 07:01:10.000000 neuroseg-0.1.1/tests/__init__.py
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)     4052 2023-04-14 17:25:13.000000 neuroseg-0.1.1/tests/test_augmentations.py
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)     7307 2023-04-14 17:25:14.000000 neuroseg-0.1.1/tests/test_core.py
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)     7842 2023-04-14 17:25:13.000000 neuroseg-0.1.1/tests/test_dataset.py
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)      184 2023-04-14 17:25:14.000000 neuroseg-0.1.1/tests/test_net.py
+-rwxrwxr-x   0 matt.mallory (20150) domain users (10513)      834 2023-04-14 17:25:12.000000 neuroseg-0.1.1/tests/test_reconstruction.py
```

### Comparing `neuroseg-0.1.0/LICENSE` & `neuroseg-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neuroseg-0.1.0/neuroseg/core/predictor.py` & `neuroseg-0.1.1/neuroseg/core/predictor.py`

 * *Files identical despite different names*

### Comparing `neuroseg-0.1.0/neuroseg/core/predictor_multilabel.py` & `neuroseg-0.1.1/neuroseg/core/predictor_multilabel.py`

 * *Files identical despite different names*

### Comparing `neuroseg-0.1.0/neuroseg/core/trainer.py` & `neuroseg-0.1.1/neuroseg/core/trainer.py`

 * *Files identical despite different names*

### Comparing `neuroseg-0.1.0/neuroseg/datasets/dataset.py` & `neuroseg-0.1.1/neuroseg/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `neuroseg-0.1.0/neuroseg/datasets/datatypes.py` & `neuroseg-0.1.1/neuroseg/datasets/datatypes.py`

 * *Files identical despite different names*

### Comparing `neuroseg-0.1.0/neuroseg/datasets/filetypes.py` & `neuroseg-0.1.1/neuroseg/datasets/filetypes.py`

 * *Files identical despite different names*

### Comparing `neuroseg-0.1.0/neuroseg/datasets/specification.py` & `neuroseg-0.1.1/neuroseg/datasets/specification.py`

 * *Files identical despite different names*

### Comparing `neuroseg-0.1.0/neuroseg/nets/RSUNet.py` & `neuroseg-0.1.1/neuroseg/nets/RSUNet.py`

 * *Files identical despite different names*

### Comparing `neuroseg-0.1.0/neuroseg/nets/RSUNetMulti.py` & `neuroseg-0.1.1/neuroseg/nets/RSUNetMulti.py`

 * *Files identical despite different names*

### Comparing `neuroseg-0.1.0/neuroseg/nets/layers.py` & `neuroseg-0.1.1/neuroseg/nets/layers.py`

 * *Files identical despite different names*

### Comparing `neuroseg-0.1.0/neuroseg/nets/netcollector.py` & `neuroseg-0.1.1/neuroseg/nets/netcollector.py`

 * *Files identical despite different names*

### Comparing `neuroseg-0.1.0/neuroseg/training/checkpoint.py` & `neuroseg-0.1.1/neuroseg/training/checkpoint.py`

 * *Files identical despite different names*

### Comparing `neuroseg-0.1.0/neuroseg/training/logging.py` & `neuroseg-0.1.1/neuroseg/training/logging.py`

 * *Files identical despite different names*

### Comparing `neuroseg-0.1.0/neuroseg.egg-info/SOURCES.txt` & `neuroseg-0.1.1/neuroseg.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.cfg
 setup.py
 neuroseg/__init__.py
 neuroseg.egg-info/PKG-INFO
 neuroseg.egg-info/SOURCES.txt
 neuroseg.egg-info/dependency_links.txt
+neuroseg.egg-info/requires.txt
 neuroseg.egg-info/top_level.txt
 neuroseg/core/__init__.py
 neuroseg/core/predictor.py
 neuroseg/core/predictor_multilabel.py
 neuroseg/core/trainer.py
 neuroseg/datasets/__init__.py
 neuroseg/datasets/dataset.py
```

### Comparing `neuroseg-0.1.0/tests/test_augmentations.py` & `neuroseg-0.1.1/tests/test_augmentations.py`

 * *Files identical despite different names*

### Comparing `neuroseg-0.1.0/tests/test_core.py` & `neuroseg-0.1.1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `neuroseg-0.1.0/tests/test_dataset.py` & `neuroseg-0.1.1/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `neuroseg-0.1.0/tests/test_reconstruction.py` & `neuroseg-0.1.1/tests/test_reconstruction.py`

 * *Files identical despite different names*

