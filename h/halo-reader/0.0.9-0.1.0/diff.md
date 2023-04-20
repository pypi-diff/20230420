# Comparing `tmp/halo-reader-0.0.9.tar.gz` & `tmp/halo-reader-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halo-reader-0.0.9.tar", last modified: Thu Apr 13 12:01:53 2023, max compression
+gzip compressed data, was "halo-reader-0.1.0.tar", last modified: Thu Apr 20 14:35:56 2023, max compression
```

## Comparing `halo-reader-0.0.9.tar` & `halo-reader-0.1.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:01:53.755583 halo-reader-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-13 12:01:23.000000 halo-reader-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-13 12:01:23.000000 halo-reader-0.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-13 12:01:53.755583 halo-reader-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-13 12:01:23.000000 halo-reader-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-13 12:01:23.000000 halo-reader-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 12:01:53.755583 halo-reader-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-13 12:01:23.000000 halo-reader-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:01:53.743583 halo-reader-0.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:01:53.747583 halo-reader-0.0.9/src/halo_reader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-13 12:01:53.000000 halo-reader-0.0.9/src/halo_reader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-13 12:01:53.000000 halo-reader-0.0.9/src/halo_reader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 12:01:53.000000 halo-reader-0.0.9/src/halo_reader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-13 12:01:53.000000 halo-reader-0.0.9/src/halo_reader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 12:01:52.000000 halo-reader-0.0.9/src/halo_reader.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-13 12:01:53.000000 halo-reader-0.0.9/src/halo_reader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-13 12:01:53.000000 halo-reader-0.0.9/src/halo_reader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:01:53.747583 halo-reader-0.0.9/src/haloboard/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloboard/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:01:53.747583 halo-reader-0.0.9/src/haloboard/static/
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloboard/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloboard/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:01:53.747583 halo-reader-0.0.9/src/haloboard/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloboard/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloboard/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:01:53.747583 halo-reader-0.0.9/src/halodata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/halodata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/halodata/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:01:53.751583 halo-reader-0.0.9/src/haloreader/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/attenuated_backscatter_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/background_correction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:01:53.751583 halo-reader-0.0.9/src/haloreader/background_reader/
--rw-r--r--   0 runner    (1001) docker     (123)   794000 2023-04-13 12:01:51.000000 halo-reader-0.0.9/src/haloreader/background_reader/background_reader.c
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/background_reader/background_reader.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:01:53.755583 halo-reader-0.0.9/src/haloreader/data_reader/
--rw-r--r--   0 runner    (1001) docker     (123)   834129 2023-04-13 12:01:52.000000 halo-reader-0.0.9/src/haloreader/data_reader/data_reader.c
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/data_reader/data_reader.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/grammar_header.lark
--rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/halo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/read.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/scantype.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/type_guards.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:01:53.755583 halo-reader-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-13 12:01:23.000000 halo-reader-0.0.9/tests/test_halo_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:56.973374 halo-reader-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-20 14:35:35.000000 halo-reader-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-20 14:35:35.000000 halo-reader-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-20 14:35:56.973374 halo-reader-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-20 14:35:35.000000 halo-reader-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-20 14:35:35.000000 halo-reader-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 14:35:56.973374 halo-reader-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-20 14:35:35.000000 halo-reader-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:56.965374 halo-reader-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:56.965374 halo-reader-0.1.0/src/halo_reader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-20 14:35:56.000000 halo-reader-0.1.0/src/halo_reader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-20 14:35:56.000000 halo-reader-0.1.0/src/halo_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:35:56.000000 halo-reader-0.1.0/src/halo_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-20 14:35:56.000000 halo-reader-0.1.0/src/halo_reader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:35:56.000000 halo-reader-0.1.0/src/halo_reader.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-20 14:35:56.000000 halo-reader-0.1.0/src/halo_reader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-20 14:35:56.000000 halo-reader-0.1.0/src/halo_reader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:56.965374 halo-reader-0.1.0/src/haloboard/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloboard/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:56.969374 halo-reader-0.1.0/src/haloboard/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloboard/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloboard/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:56.969374 halo-reader-0.1.0/src/haloboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloboard/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloboard/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:56.969374 halo-reader-0.1.0/src/halodata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/halodata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/halodata/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:56.969374 halo-reader-0.1.0/src/haloreader/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/attenuated_backscatter_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/background_correction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:56.969374 halo-reader-0.1.0/src/haloreader/background_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)   794000 2023-04-20 14:35:55.000000 halo-reader-0.1.0/src/haloreader/background_reader/background_reader.c
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/background_reader/background_reader.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:56.973374 halo-reader-0.1.0/src/haloreader/data_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)   834129 2023-04-20 14:35:56.000000 halo-reader-0.1.0/src/haloreader/data_reader/data_reader.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/data_reader/data_reader.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/grammar_header.lark
+-rw-r--r--   0 runner    (1001) docker     (123)    15136 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/halo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/scantype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/type_guards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:56.973374 halo-reader-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-20 14:35:35.000000 halo-reader-0.1.0/tests/test_halo_reader.py
```

### Comparing `halo-reader-0.0.9/LICENSE` & `halo-reader-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.9/PKG-INFO` & `halo-reader-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halo-reader
-Version: 0.0.9
+Version: 0.1.0
 Summary: HALO Photonics wind doppler lidar file reader
 Author-email: Niko Leskinen <niko.leskinen@fmi.fi>
 License: MIT License
         
         Copyright (c) 2022 Finnish Meteorological Institute
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `halo-reader-0.0.9/README.md` & `halo-reader-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.9/pyproject.toml` & `halo-reader-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.9/setup.py` & `halo-reader-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.9/src/halo_reader.egg-info/PKG-INFO` & `halo-reader-0.1.0/src/halo_reader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halo-reader
-Version: 0.0.9
+Version: 0.1.0
 Summary: HALO Photonics wind doppler lidar file reader
 Author-email: Niko Leskinen <niko.leskinen@fmi.fi>
 License: MIT License
         
         Copyright (c) 2022 Finnish Meteorological Institute
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `halo-reader-0.0.9/src/halo_reader.egg-info/SOURCES.txt` & `halo-reader-0.1.0/src/halo_reader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.9/src/haloboard/app.py` & `halo-reader-0.1.0/src/haloboard/app.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.9/src/haloboard/static/favicon.ico` & `halo-reader-0.1.0/src/haloboard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.9/src/haloboard/static/style.css` & `halo-reader-0.1.0/src/haloboard/static/style.css`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.9/src/haloboard/templates/index.html` & `halo-reader-0.1.0/src/haloboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.9/src/halodata/datasets.py` & `halo-reader-0.1.0/src/halodata/datasets.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.9/src/haloreader/attenuated_backscatter_coefficient.py` & `halo-reader-0.1.0/src/haloreader/attenuated_backscatter_coefficient.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.9/src/haloreader/attribute.py` & `halo-reader-0.1.0/src/haloreader/attribute.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.9/src/haloreader/background_correction.py` & `halo-reader-0.1.0/src/haloreader/background_correction.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.9/src/haloreader/background_reader/background_reader.c` & `halo-reader-0.1.0/src/haloreader/background_reader/background_reader.c`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.9/src/haloreader/background_reader/background_reader.pyx` & `halo-reader-0.1.0/src/haloreader/background_reader/background_reader.pyx`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.9/src/haloreader/cli.py` & `halo-reader-0.1.0/src/haloreader/cli.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.9/src/haloreader/data_reader/data_reader.c` & `halo-reader-0.1.0/src/haloreader/data_reader/data_reader.c`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.9/src/haloreader/data_reader/data_reader.pyx` & `halo-reader-0.1.0/src/haloreader/data_reader/data_reader.pyx`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.9/src/haloreader/grammar_header.lark` & `halo-reader-0.1.0/src/haloreader/grammar_header.lark`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.9/src/haloreader/halo.py` & `halo-reader-0.1.0/src/haloreader/halo.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,14 +75,16 @@
 
         halo = Halo(**halo_attrs)
         if not isinstance(halo.time.data, np.ndarray):
             raise TypeError
         if not _is_increasing(halo.time.data):
             halo.remove_profiles_with_duplicate_time()
         if not _is_increasing(halo.time.data):
+            halo.remove_profiles_with_non_increasing_time()
+        if not _is_increasing(halo.time.data):
             raise ValueError("Time must be increasing")
         return halo
 
     def remove_profiles_with_duplicate_time(self) -> None:
         if not is_ndarray(self.time.data):
             raise TypeError
         mask = _duplicate_time_mask(self.time.data)
@@ -100,14 +102,36 @@
                         for i, d in enumerate(halo_attr.dimensions)
                     )
                 )
                 if not is_fancy_index(index):
                     raise TypeError
                 halo_attr.data = halo_attr.data[index]
 
+    def remove_profiles_with_non_increasing_time(self) -> None:
+        if not is_ndarray(self.time.data):
+            raise TypeError
+        mask = _non_increasing_time_mask(self.time.data)
+        for attr_name in self.__dataclass_fields__.keys():
+            halo_attr = getattr(self, attr_name)
+            if (
+                isinstance(halo_attr, Variable)
+                and is_ndarray(halo_attr.data)
+                and isinstance(halo_attr.dimensions, tuple)
+                and self.time.name in halo_attr.dimensions
+            ):
+                index = tuple(
+                    (
+                        mask if d == self.time.name else slice(None)
+                        for i, d in enumerate(halo_attr.dimensions)
+                    )
+                )
+                if not is_fancy_index(index):
+                    raise TypeError
+                halo_attr.data = halo_attr.data[index]
+
     def convert_time_unit2cloudnet_time(self) -> None:
         _convert_timevar_unit2cloudnet_time(self.time)
         _convert_timevar_unit2cloudnet_time(self.metadata.start_time)
 
     def correct_background(self, halobg: HaloBg) -> None:
         if not is_ndarray(self.range.data):
             raise TypeError
@@ -362,9 +386,30 @@
     return bool(np.all(np.diff(time) > 0))
 
 
 def _duplicate_time_mask(time: np.ndarray) -> np.ndarray:
     _mask = np.isclose(np.diff(time), 0)
     nremoved = _mask.sum()
     if nremoved > 0:
-        log.debug("Removed %d profiles (duplicate timestamps)", nremoved)
+        log.debug("Removed %d/%d profiles (duplicate timestamps)", nremoved, len(time))
     return np.logical_not(np.insert(_mask, 0, False))
+
+
+def _non_increasing_time_mask(time: np.ndarray) -> np.ndarray:
+    if len(time) == 0:
+        return np.zeros_like(time, dtype=bool)
+    _mask = np.zeros_like(time, dtype=bool)
+    largest_time = time[0]
+    for i, current_time in enumerate(time[1:], start=1):
+        if current_time <= largest_time:
+            _mask[i] = True
+        else:
+            largest_time = current_time
+    nremoved = _mask.sum()
+    if nremoved > 0:
+        log.debug(
+            "Removed %d/%d profiles (non-increasing timestamps)", nremoved, len(time)
+        )
+    mask = np.logical_not(_mask)
+    if not is_ndarray(mask):
+        raise TypeError
+    return mask
```

### Comparing `halo-reader-0.0.9/src/haloreader/metadata.py` & `halo-reader-0.1.0/src/haloreader/metadata.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.9/src/haloreader/read.py` & `halo-reader-0.1.0/src/haloreader/read.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.9/src/haloreader/scantype.py` & `halo-reader-0.1.0/src/haloreader/scantype.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.9/src/haloreader/screen.py` & `halo-reader-0.1.0/src/haloreader/screen.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.9/src/haloreader/transformer.py` & `halo-reader-0.1.0/src/haloreader/transformer.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.9/src/haloreader/type_guards.py` & `halo-reader-0.1.0/src/haloreader/type_guards.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.9/src/haloreader/utils.py` & `halo-reader-0.1.0/src/haloreader/utils.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.9/src/haloreader/variable.py` & `halo-reader-0.1.0/src/haloreader/variable.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.9/tests/test_halo_reader.py` & `halo-reader-0.1.0/tests/test_halo_reader.py`

 * *Files identical despite different names*

