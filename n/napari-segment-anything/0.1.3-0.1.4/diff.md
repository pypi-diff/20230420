# Comparing `tmp/napari-segment-anything-0.1.3.tar.gz` & `tmp/napari-segment-anything-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-segment-anything-0.1.3.tar", last modified: Mon Apr 10 18:27:40 2023, max compression
+gzip compressed data, was "napari-segment-anything-0.1.4.tar", last modified: Wed Apr 19 22:32:08 2023, max compression
```

## Comparing `napari-segment-anything-0.1.3.tar` & `napari-segment-anything-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:27:40.828027 napari-segment-anything-0.1.3/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)    11358 2023-04-05 19:05:13.000000 napari-segment-anything-0.1.3/LICENSE
--rw-rw-r--   0 jordao    (1000) jordao    (1000)       96 2023-04-05 19:05:13.000000 napari-segment-anything-0.1.3/MANIFEST.in
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     5504 2023-04-10 18:27:40.828027 napari-segment-anything-0.1.3/PKG-INFO
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     4188 2023-04-10 15:53:01.000000 napari-segment-anything-0.1.3/README.md
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      180 2023-04-05 19:05:13.000000 napari-segment-anything-0.1.3/pyproject.toml
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1829 2023-04-10 18:27:40.828027 napari-segment-anything-0.1.3/setup.cfg
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:27:40.828027 napari-segment-anything-0.1.3/src/
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:27:40.828027 napari-segment-anything-0.1.3/src/napari_segment_anything/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      102 2023-04-10 18:26:52.000000 napari-segment-anything-0.1.3/src/napari_segment_anything/__init__.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:27:40.828027 napari-segment-anything-0.1.3/src/napari_segment_anything/_tests/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2023-04-05 19:05:13.000000 napari-segment-anything-0.1.3/src/napari_segment_anything/_tests/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2540 2023-04-08 00:22:57.000000 napari-segment-anything-0.1.3/src/napari_segment_anything/_tests/test_widget.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     7283 2023-04-08 00:22:57.000000 napari-segment-anything-0.1.3/src/napari_segment_anything/_widget.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      320 2023-04-05 20:29:57.000000 napari-segment-anything-0.1.3/src/napari_segment_anything/napari.yaml
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2157 2023-04-10 17:47:09.000000 napari-segment-anything-0.1.3/src/napari_segment_anything/utils.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:27:40.828027 napari-segment-anything-0.1.3/src/napari_segment_anything.egg-info/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     5504 2023-04-10 18:27:40.000000 napari-segment-anything-0.1.3/src/napari_segment_anything.egg-info/PKG-INFO
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      615 2023-04-10 18:27:40.000000 napari-segment-anything-0.1.3/src/napari_segment_anything.egg-info/SOURCES.txt
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        1 2023-04-10 18:27:40.000000 napari-segment-anything-0.1.3/src/napari_segment_anything.egg-info/dependency_links.txt
--rw-rw-r--   0 jordao    (1000) jordao    (1000)       80 2023-04-10 18:27:40.000000 napari-segment-anything-0.1.3/src/napari_segment_anything.egg-info/entry_points.txt
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      111 2023-04-10 18:27:40.000000 napari-segment-anything-0.1.3/src/napari_segment_anything.egg-info/requires.txt
--rw-rw-r--   0 jordao    (1000) jordao    (1000)       24 2023-04-10 18:27:40.000000 napari-segment-anything-0.1.3/src/napari_segment_anything.egg-info/top_level.txt
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-19 22:32:08.822553 napari-segment-anything-0.1.4/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)    11358 2023-04-05 19:05:13.000000 napari-segment-anything-0.1.4/LICENSE
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)       96 2023-04-05 19:05:13.000000 napari-segment-anything-0.1.4/MANIFEST.in
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     5504 2023-04-19 22:32:08.822553 napari-segment-anything-0.1.4/PKG-INFO
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     4188 2023-04-10 15:53:01.000000 napari-segment-anything-0.1.4/README.md
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      180 2023-04-05 19:05:13.000000 napari-segment-anything-0.1.4/pyproject.toml
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1829 2023-04-19 22:32:08.822553 napari-segment-anything-0.1.4/setup.cfg
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-19 22:32:08.818553 napari-segment-anything-0.1.4/src/
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-19 22:32:08.822553 napari-segment-anything-0.1.4/src/napari_segment_anything/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      102 2023-04-19 22:29:59.000000 napari-segment-anything-0.1.4/src/napari_segment_anything/__init__.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-19 22:32:08.822553 napari-segment-anything-0.1.4/src/napari_segment_anything/_tests/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2023-04-05 19:05:13.000000 napari-segment-anything-0.1.4/src/napari_segment_anything/_tests/__init__.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2540 2023-04-08 00:22:57.000000 napari-segment-anything-0.1.4/src/napari_segment_anything/_tests/test_widget.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     7412 2023-04-19 22:29:19.000000 napari-segment-anything-0.1.4/src/napari_segment_anything/_widget.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      320 2023-04-05 20:29:57.000000 napari-segment-anything-0.1.4/src/napari_segment_anything/napari.yaml
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2157 2023-04-10 17:47:09.000000 napari-segment-anything-0.1.4/src/napari_segment_anything/utils.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-19 22:32:08.822553 napari-segment-anything-0.1.4/src/napari_segment_anything.egg-info/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     5504 2023-04-19 22:32:08.000000 napari-segment-anything-0.1.4/src/napari_segment_anything.egg-info/PKG-INFO
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      615 2023-04-19 22:32:08.000000 napari-segment-anything-0.1.4/src/napari_segment_anything.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        1 2023-04-19 22:32:08.000000 napari-segment-anything-0.1.4/src/napari_segment_anything.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)       80 2023-04-19 22:32:08.000000 napari-segment-anything-0.1.4/src/napari_segment_anything.egg-info/entry_points.txt
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      111 2023-04-19 22:32:08.000000 napari-segment-anything-0.1.4/src/napari_segment_anything.egg-info/requires.txt
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)       24 2023-04-19 22:32:08.000000 napari-segment-anything-0.1.4/src/napari_segment_anything.egg-info/top_level.txt
```

### Comparing `napari-segment-anything-0.1.3/LICENSE` & `napari-segment-anything-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-segment-anything-0.1.3/PKG-INFO` & `napari-segment-anything-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-segment-anything
-Version: 0.1.3
+Version: 0.1.4
 Summary: Napari plugin of Segment Anything Model (SAM)
 Home-page: https://github.com/jookuma/napari-segment-anything
 Author: Jordao Bragantini
 Author-email: jordao.bragantini@czbiohub.org
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/jookuma/napari-segment-anything/issues
 Project-URL: Documentation, https://github.com/jookuma/napari-segment-anything#README.md
```

### Comparing `napari-segment-anything-0.1.3/README.md` & `napari-segment-anything-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `napari-segment-anything-0.1.3/setup.cfg` & `napari-segment-anything-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-segment-anything-0.1.3/src/napari_segment_anything/_tests/test_widget.py` & `napari-segment-anything-0.1.4/src/napari_segment_anything/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-segment-anything-0.1.3/src/napari_segment_anything/_widget.py` & `napari-segment-anything-0.1.4/src/napari_segment_anything/_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,20 @@
 class SAMWidget(Container):
     _sam: Sam
     _predictor: SamPredictor
 
     def __init__(self, viewer: napari.Viewer, model_type: str = "default"):
         super().__init__()
         self._viewer = viewer
-
-        self._device = "cuda" if torch.cuda.is_available() else "cpu"
+        if torch.cuda.is_available():
+            self._device = "cuda"
+        elif torch.backends.mps.is_available():
+            self._device = "mps"
+        else:
+            self._device = "cpu"
 
         self._model_type_widget = ComboBox(
             value=model_type,
             choices=list(sam_model_registry.keys()),
             label="Model:",
         )
         self._model_type_widget.changed.connect(self._load_model)
```

### Comparing `napari-segment-anything-0.1.3/src/napari_segment_anything/utils.py` & `napari-segment-anything-0.1.4/src/napari_segment_anything/utils.py`

 * *Files identical despite different names*

### Comparing `napari-segment-anything-0.1.3/src/napari_segment_anything.egg-info/PKG-INFO` & `napari-segment-anything-0.1.4/src/napari_segment_anything.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-segment-anything
-Version: 0.1.3
+Version: 0.1.4
 Summary: Napari plugin of Segment Anything Model (SAM)
 Home-page: https://github.com/jookuma/napari-segment-anything
 Author: Jordao Bragantini
 Author-email: jordao.bragantini@czbiohub.org
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/jookuma/napari-segment-anything/issues
 Project-URL: Documentation, https://github.com/jookuma/napari-segment-anything#README.md
```

### Comparing `napari-segment-anything-0.1.3/src/napari_segment_anything.egg-info/SOURCES.txt` & `napari-segment-anything-0.1.4/src/napari_segment_anything.egg-info/SOURCES.txt`

 * *Files identical despite different names*

