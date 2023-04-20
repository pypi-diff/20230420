# Comparing `tmp/digital-experiments-1.0.6.tar.gz` & `tmp/digital-experiments-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digital-experiments-1.0.6.tar", last modified: Thu Apr 20 10:07:59 2023, max compression
+gzip compressed data, was "digital-experiments-1.0.7.tar", last modified: Thu Apr 20 10:11:53 2023, max compression
```

## Comparing `digital-experiments-1.0.6.tar` & `digital-experiments-1.0.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-20 10:07:59.080059 digital-experiments-1.0.6/
--rw-r--r--   0 john       (504) staff       (20)     1051 2022-11-18 07:34:19.000000 digital-experiments-1.0.6/LICENSE
--rw-r--r--   0 john       (504) staff       (20)     2642 2023-04-20 10:07:59.079881 digital-experiments-1.0.6/PKG-INFO
--rw-r--r--   0 john       (504) staff       (20)     1008 2023-03-29 15:42:00.000000 digital-experiments-1.0.6/README.md
--rw-r--r--   0 john       (504) staff       (20)     1321 2023-04-20 10:07:29.000000 digital-experiments-1.0.6/pyproject.toml
--rw-r--r--   0 john       (504) staff       (20)       38 2023-04-20 10:07:59.080106 digital-experiments-1.0.6/setup.cfg
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-20 10:07:59.069991 digital-experiments-1.0.6/src/
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-20 10:07:59.074285 digital-experiments-1.0.6/src/digital_experiments/
--rw-r--r--   0 john       (504) staff       (20)      139 2023-04-20 10:07:29.000000 digital-experiments-1.0.6/src/digital_experiments/__init__.py
--rw-r--r--   0 john       (504) staff       (20)     6219 2023-04-04 08:39:31.000000 digital-experiments-1.0.6/src/digital_experiments/backends.py
--rw-r--r--   0 john       (504) staff       (20)     1016 2023-03-29 15:42:00.000000 digital-experiments-1.0.6/src/digital_experiments/control_center.py
--rw-r--r--   0 john       (504) staff       (20)     3301 2023-04-20 09:51:37.000000 digital-experiments-1.0.6/src/digital_experiments/experiment.py
--rw-r--r--   0 john       (504) staff       (20)      402 2023-03-29 15:42:00.000000 digital-experiments-1.0.6/src/digital_experiments/inspection.py
--rw-r--r--   0 john       (504) staff       (20)      592 2023-03-29 15:42:00.000000 digital-experiments-1.0.6/src/digital_experiments/metadata.py
--rw-r--r--   0 john       (504) staff       (20)     4450 2023-04-04 08:33:50.000000 digital-experiments-1.0.6/src/digital_experiments/minimize.py
--rw-r--r--   0 john       (504) staff       (20)      637 2023-03-29 15:42:00.000000 digital-experiments-1.0.6/src/digital_experiments/observation.py
--rw-r--r--   0 john       (504) staff       (20)      735 2023-03-29 15:42:00.000000 digital-experiments-1.0.6/src/digital_experiments/pretty.py
--rw-r--r--   0 john       (504) staff       (20)     2454 2023-04-20 10:03:31.000000 digital-experiments-1.0.6/src/digital_experiments/querying.py
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-20 10:07:59.077492 digital-experiments-1.0.6/src/digital_experiments/search/
--rw-r--r--   0 john       (504) staff       (20)     2897 2023-03-29 15:42:00.000000 digital-experiments-1.0.6/src/digital_experiments/search/skopt_suggest.py
--rw-r--r--   0 john       (504) staff       (20)     5381 2023-03-29 15:42:00.000000 digital-experiments-1.0.6/src/digital_experiments/search/space.py
--rw-r--r--   0 john       (504) staff       (20)     4218 2023-04-03 14:30:06.000000 digital-experiments-1.0.6/src/digital_experiments/search/suggest.py
--rw-r--r--   0 john       (504) staff       (20)     3545 2023-04-04 08:55:31.000000 digital-experiments-1.0.6/src/digital_experiments/util.py
--rw-r--r--   0 john       (504) staff       (20)     3464 2023-03-29 15:42:00.000000 digital-experiments-1.0.6/src/digital_experiments/version_control.py
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-20 10:07:59.076309 digital-experiments-1.0.6/src/digital_experiments.egg-info/
--rw-r--r--   0 john       (504) staff       (20)     2642 2023-04-20 10:07:59.000000 digital-experiments-1.0.6/src/digital_experiments.egg-info/PKG-INFO
--rw-r--r--   0 john       (504) staff       (20)     1049 2023-04-20 10:07:59.000000 digital-experiments-1.0.6/src/digital_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 john       (504) staff       (20)        1 2023-04-20 10:07:59.000000 digital-experiments-1.0.6/src/digital_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 john       (504) staff       (20)      160 2023-04-20 10:07:59.000000 digital-experiments-1.0.6/src/digital_experiments.egg-info/requires.txt
--rw-r--r--   0 john       (504) staff       (20)       32 2023-04-20 10:07:59.000000 digital-experiments-1.0.6/src/digital_experiments.egg-info/top_level.txt
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-20 10:07:59.079598 digital-experiments-1.0.6/tests/
--rw-r--r--   0 john       (504) staff       (20)     1861 2023-03-29 16:29:55.000000 digital-experiments-1.0.6/tests/test_backends.py
--rw-r--r--   0 john       (504) staff       (20)      377 2023-03-29 15:42:00.000000 digital-experiments-1.0.6/tests/test_control_center.py
--rw-r--r--   0 john       (504) staff       (20)      863 2023-03-29 15:42:00.000000 digital-experiments-1.0.6/tests/test_experiment.py
--rw-r--r--   0 john       (504) staff       (20)      793 2023-03-29 15:42:00.000000 digital-experiments-1.0.6/tests/test_metadata.py
--rw-r--r--   0 john       (504) staff       (20)      632 2023-03-29 15:42:00.000000 digital-experiments-1.0.6/tests/test_minimize.py
--rw-r--r--   0 john       (504) staff       (20)     1156 2023-04-20 10:06:14.000000 digital-experiments-1.0.6/tests/test_querying.py
--rw-r--r--   0 john       (504) staff       (20)     1596 2023-03-29 15:42:00.000000 digital-experiments-1.0.6/tests/test_space.py
--rw-r--r--   0 john       (504) staff       (20)     2188 2023-04-04 09:25:29.000000 digital-experiments-1.0.6/tests/test_suggest.py
--rw-r--r--   0 john       (504) staff       (20)      795 2023-03-29 15:42:00.000000 digital-experiments-1.0.6/tests/test_util.py
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-20 10:11:53.679876 digital-experiments-1.0.7/
+-rw-r--r--   0 john       (504) staff       (20)     1051 2022-11-18 07:34:19.000000 digital-experiments-1.0.7/LICENSE
+-rw-r--r--   0 john       (504) staff       (20)     2642 2023-04-20 10:11:53.679692 digital-experiments-1.0.7/PKG-INFO
+-rw-r--r--   0 john       (504) staff       (20)     1008 2023-03-29 15:42:00.000000 digital-experiments-1.0.7/README.md
+-rw-r--r--   0 john       (504) staff       (20)     1321 2023-04-20 10:11:46.000000 digital-experiments-1.0.7/pyproject.toml
+-rw-r--r--   0 john       (504) staff       (20)       38 2023-04-20 10:11:53.679928 digital-experiments-1.0.7/setup.cfg
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-20 10:11:53.673190 digital-experiments-1.0.7/src/
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-20 10:11:53.676441 digital-experiments-1.0.7/src/digital_experiments/
+-rw-r--r--   0 john       (504) staff       (20)      139 2023-04-20 10:11:46.000000 digital-experiments-1.0.7/src/digital_experiments/__init__.py
+-rw-r--r--   0 john       (504) staff       (20)     6219 2023-04-04 08:39:31.000000 digital-experiments-1.0.7/src/digital_experiments/backends.py
+-rw-r--r--   0 john       (504) staff       (20)     1016 2023-03-29 15:42:00.000000 digital-experiments-1.0.7/src/digital_experiments/control_center.py
+-rw-r--r--   0 john       (504) staff       (20)     3303 2023-04-20 10:11:29.000000 digital-experiments-1.0.7/src/digital_experiments/experiment.py
+-rw-r--r--   0 john       (504) staff       (20)      402 2023-03-29 15:42:00.000000 digital-experiments-1.0.7/src/digital_experiments/inspection.py
+-rw-r--r--   0 john       (504) staff       (20)      592 2023-03-29 15:42:00.000000 digital-experiments-1.0.7/src/digital_experiments/metadata.py
+-rw-r--r--   0 john       (504) staff       (20)     4450 2023-04-04 08:33:50.000000 digital-experiments-1.0.7/src/digital_experiments/minimize.py
+-rw-r--r--   0 john       (504) staff       (20)      637 2023-03-29 15:42:00.000000 digital-experiments-1.0.7/src/digital_experiments/observation.py
+-rw-r--r--   0 john       (504) staff       (20)      735 2023-03-29 15:42:00.000000 digital-experiments-1.0.7/src/digital_experiments/pretty.py
+-rw-r--r--   0 john       (504) staff       (20)     2454 2023-04-20 10:03:31.000000 digital-experiments-1.0.7/src/digital_experiments/querying.py
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-20 10:11:53.677873 digital-experiments-1.0.7/src/digital_experiments/search/
+-rw-r--r--   0 john       (504) staff       (20)     2897 2023-03-29 15:42:00.000000 digital-experiments-1.0.7/src/digital_experiments/search/skopt_suggest.py
+-rw-r--r--   0 john       (504) staff       (20)     5381 2023-03-29 15:42:00.000000 digital-experiments-1.0.7/src/digital_experiments/search/space.py
+-rw-r--r--   0 john       (504) staff       (20)     4218 2023-04-03 14:30:06.000000 digital-experiments-1.0.7/src/digital_experiments/search/suggest.py
+-rw-r--r--   0 john       (504) staff       (20)     3545 2023-04-04 08:55:31.000000 digital-experiments-1.0.7/src/digital_experiments/util.py
+-rw-r--r--   0 john       (504) staff       (20)     3464 2023-03-29 15:42:00.000000 digital-experiments-1.0.7/src/digital_experiments/version_control.py
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-20 10:11:53.677428 digital-experiments-1.0.7/src/digital_experiments.egg-info/
+-rw-r--r--   0 john       (504) staff       (20)     2642 2023-04-20 10:11:53.000000 digital-experiments-1.0.7/src/digital_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 john       (504) staff       (20)     1049 2023-04-20 10:11:53.000000 digital-experiments-1.0.7/src/digital_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (504) staff       (20)        1 2023-04-20 10:11:53.000000 digital-experiments-1.0.7/src/digital_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (504) staff       (20)      160 2023-04-20 10:11:53.000000 digital-experiments-1.0.7/src/digital_experiments.egg-info/requires.txt
+-rw-r--r--   0 john       (504) staff       (20)       32 2023-04-20 10:11:53.000000 digital-experiments-1.0.7/src/digital_experiments.egg-info/top_level.txt
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-20 10:11:53.679380 digital-experiments-1.0.7/tests/
+-rw-r--r--   0 john       (504) staff       (20)     1861 2023-03-29 16:29:55.000000 digital-experiments-1.0.7/tests/test_backends.py
+-rw-r--r--   0 john       (504) staff       (20)      377 2023-03-29 15:42:00.000000 digital-experiments-1.0.7/tests/test_control_center.py
+-rw-r--r--   0 john       (504) staff       (20)      863 2023-03-29 15:42:00.000000 digital-experiments-1.0.7/tests/test_experiment.py
+-rw-r--r--   0 john       (504) staff       (20)      793 2023-03-29 15:42:00.000000 digital-experiments-1.0.7/tests/test_metadata.py
+-rw-r--r--   0 john       (504) staff       (20)      632 2023-03-29 15:42:00.000000 digital-experiments-1.0.7/tests/test_minimize.py
+-rw-r--r--   0 john       (504) staff       (20)     1156 2023-04-20 10:06:14.000000 digital-experiments-1.0.7/tests/test_querying.py
+-rw-r--r--   0 john       (504) staff       (20)     1596 2023-03-29 15:42:00.000000 digital-experiments-1.0.7/tests/test_space.py
+-rw-r--r--   0 john       (504) staff       (20)     2188 2023-04-04 09:25:29.000000 digital-experiments-1.0.7/tests/test_suggest.py
+-rw-r--r--   0 john       (504) staff       (20)      795 2023-03-29 15:42:00.000000 digital-experiments-1.0.7/tests/test_util.py
```

### Comparing `digital-experiments-1.0.6/LICENSE` & `digital-experiments-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.6/PKG-INFO` & `digital-experiments-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digital-experiments
-Version: 1.0.6
+Version: 1.0.7
 Summary: Keep track of digital experiments.
 Author-email: John Gardner <gardner.john97@gmail.com>
 License: Copyright 2022 John Gardner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `digital-experiments-1.0.6/README.md` & `digital-experiments-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.6/pyproject.toml` & `digital-experiments-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digital-experiments"
-version = "1.0.6"
+version = "1.0.7"
 description = "Keep track of digital experiments."
 readme = "README.md"
 authors = [{ name = "John Gardner", email = "gardner.john97@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -41,15 +41,15 @@
     "pytest-cov",
 ]
 
 [project.urls]
 Homepage = "https://github.com/jla-gardner/digital-experiments"
 
 [tool.bumpver]
-current_version = "1.0.6"
+current_version = "1.0.7"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `digital-experiments-1.0.6/src/digital_experiments/backends.py` & `digital-experiments-1.0.7/src/digital_experiments/backends.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.6/src/digital_experiments/control_center.py` & `digital-experiments-1.0.7/src/digital_experiments/control_center.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.6/src/digital_experiments/experiment.py` & `digital-experiments-1.0.7/src/digital_experiments/experiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         self,
         include_metadata=False,
         include_id=True,
         config=None,
         metadata=None,
         result=None,
     ):
-        filtered_observations = querying.filter_observations(
+        filtered_observations = querying.filtered_observations(
             self.observations, config, metadata, result
         )
         return querying.to_dataframe(
             filtered_observations, include_id, include_metadata
         )
 
     def __repr__(self):
```

### Comparing `digital-experiments-1.0.6/src/digital_experiments/metadata.py` & `digital-experiments-1.0.7/src/digital_experiments/metadata.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.6/src/digital_experiments/minimize.py` & `digital-experiments-1.0.7/src/digital_experiments/minimize.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.6/src/digital_experiments/observation.py` & `digital-experiments-1.0.7/src/digital_experiments/observation.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.6/src/digital_experiments/pretty.py` & `digital-experiments-1.0.7/src/digital_experiments/pretty.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.6/src/digital_experiments/querying.py` & `digital-experiments-1.0.7/src/digital_experiments/querying.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.6/src/digital_experiments/search/skopt_suggest.py` & `digital-experiments-1.0.7/src/digital_experiments/search/skopt_suggest.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.6/src/digital_experiments/search/space.py` & `digital-experiments-1.0.7/src/digital_experiments/search/space.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.6/src/digital_experiments/search/suggest.py` & `digital-experiments-1.0.7/src/digital_experiments/search/suggest.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.6/src/digital_experiments/util.py` & `digital-experiments-1.0.7/src/digital_experiments/util.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.6/src/digital_experiments/version_control.py` & `digital-experiments-1.0.7/src/digital_experiments/version_control.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.6/src/digital_experiments.egg-info/PKG-INFO` & `digital-experiments-1.0.7/src/digital_experiments.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digital-experiments
-Version: 1.0.6
+Version: 1.0.7
 Summary: Keep track of digital experiments.
 Author-email: John Gardner <gardner.john97@gmail.com>
 License: Copyright 2022 John Gardner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `digital-experiments-1.0.6/src/digital_experiments.egg-info/SOURCES.txt` & `digital-experiments-1.0.7/src/digital_experiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.6/tests/test_backends.py` & `digital-experiments-1.0.7/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.6/tests/test_experiment.py` & `digital-experiments-1.0.7/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.6/tests/test_metadata.py` & `digital-experiments-1.0.7/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.6/tests/test_minimize.py` & `digital-experiments-1.0.7/tests/test_minimize.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.6/tests/test_querying.py` & `digital-experiments-1.0.7/tests/test_querying.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.6/tests/test_space.py` & `digital-experiments-1.0.7/tests/test_space.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.6/tests/test_suggest.py` & `digital-experiments-1.0.7/tests/test_suggest.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.6/tests/test_util.py` & `digital-experiments-1.0.7/tests/test_util.py`

 * *Files identical despite different names*

