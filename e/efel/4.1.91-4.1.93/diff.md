# Comparing `tmp/efel-4.1.91.tar.gz` & `tmp/efel-4.1.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efel-4.1.91.tar", last modified: Thu Apr 13 10:40:04 2023, max compression
+gzip compressed data, was "efel-4.1.93.tar", last modified: Thu Apr 20 11:46:28 2023, max compression
```

## Comparing `efel-4.1.91.tar` & `efel-4.1.93.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 10:40:04.422554 efel-4.1.91/
--rw-r--r--   0 runner    (1001) docker     (122)      148 2023-04-13 10:40:01.000000 efel-4.1.91/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (122)    35151 2023-04-13 10:40:01.000000 efel-4.1.91/COPYING
--rw-r--r--   0 runner    (1001) docker     (122)     7651 2023-04-13 10:40:01.000000 efel-4.1.91/COPYING.less
--rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-04-13 10:40:01.000000 efel-4.1.91/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      126 2023-04-13 10:40:01.000000 efel-4.1.91/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1318 2023-04-13 10:40:04.422554 efel-4.1.91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7400 2023-04-13 10:40:01.000000 efel-4.1.91/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 10:40:04.422554 efel-4.1.91/efel/
--rw-r--r--   0 runner    (1001) docker     (122)    12805 2023-04-13 10:40:01.000000 efel-4.1.91/efel/DependencyV5.txt
--rw-r--r--   0 runner    (1001) docker     (122)      967 2023-04-13 10:40:01.000000 efel-4.1.91/efel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      498 2023-04-13 10:40:04.422554 efel-4.1.91/efel/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)    18462 2023-04-13 10:40:01.000000 efel-4.1.91/efel/api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 10:40:04.422554 efel-4.1.91/efel/cppcore/
--rw-r--r--   0 runner    (1001) docker     (122)     6902 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/DependencyTree.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/DependencyTree.h
--rw-r--r--   0 runner    (1001) docker     (122)    14462 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/FillFptrTable.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1700 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/FillFptrTable.h
--rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/Global.h
--rw-r--r--   0 runner    (1001) docker     (122)    69609 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/LibV1.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     7239 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/LibV1.h
--rw-r--r--   0 runner    (1001) docker     (122)    57446 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/LibV2.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     8364 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/LibV2.h
--rw-r--r--   0 runner    (1001) docker     (122)    40008 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/LibV3.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4874 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/LibV3.h
--rw-r--r--   0 runner    (1001) docker     (122)     3611 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/LibV4.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1596 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/LibV4.h
--rw-r--r--   0 runner    (1001) docker     (122)   136351 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/LibV5.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    15913 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/LibV5.h
--rw-r--r--   0 runner    (1001) docker     (122)     6931 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/Utils.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3430 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/Utils.h
--rw-r--r--   0 runner    (1001) docker     (122)    22270 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/cfeature.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3274 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/cfeature.h
--rw-r--r--   0 runner    (1001) docker     (122)    10351 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/cppcore.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1829 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/eFELLogger.h
--rw-r--r--   0 runner    (1001) docker     (122)     3597 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/efel.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2399 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/efel.h
--rw-r--r--   0 runner    (1001) docker     (122)     8378 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/mapoperations.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2832 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/mapoperations.h
--rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/types.h
--rw-r--r--   0 runner    (1001) docker     (122)    10312 2023-04-13 10:40:01.000000 efel-4.1.91/efel/io.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 10:40:04.422554 efel-4.1.91/efel/pyfeatures/
--rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-04-13 10:40:01.000000 efel-4.1.91/efel/pyfeatures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10308 2023-04-13 10:40:01.000000 efel-4.1.91/efel/pyfeatures/pyfeatures.py
--rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-04-13 10:40:01.000000 efel-4.1.91/efel/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 10:40:04.418554 efel-4.1.91/efel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1318 2023-04-13 10:40:04.000000 efel-4.1.91/efel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-04-13 10:40:04.000000 efel-4.1.91/efel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 10:40:04.000000 efel-4.1.91/efel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-04-13 10:40:04.000000 efel-4.1.91/efel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-13 10:40:04.000000 efel-4.1.91/efel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-04-13 10:40:04.422554 efel-4.1.91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4043 2023-04-13 10:40:01.000000 efel-4.1.91/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)    69513 2023-04-13 10:40:01.000000 efel-4.1.91/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 11:46:27.991787 efel-4.1.93/
+-rw-r--r--   0 runner    (1001) docker     (122)      148 2023-04-20 11:46:25.000000 efel-4.1.93/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    35151 2023-04-20 11:46:25.000000 efel-4.1.93/COPYING
+-rw-r--r--   0 runner    (1001) docker     (122)     7651 2023-04-20 11:46:25.000000 efel-4.1.93/COPYING.less
+-rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-04-20 11:46:25.000000 efel-4.1.93/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-04-20 11:46:25.000000 efel-4.1.93/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1318 2023-04-20 11:46:27.991787 efel-4.1.93/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7400 2023-04-20 11:46:25.000000 efel-4.1.93/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 11:46:27.991787 efel-4.1.93/efel/
+-rw-r--r--   0 runner    (1001) docker     (122)    12805 2023-04-20 11:46:25.000000 efel-4.1.93/efel/DependencyV5.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      967 2023-04-20 11:46:25.000000 efel-4.1.93/efel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-04-20 11:46:27.991787 efel-4.1.93/efel/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18462 2023-04-20 11:46:25.000000 efel-4.1.93/efel/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 11:46:27.991787 efel-4.1.93/efel/cppcore/
+-rw-r--r--   0 runner    (1001) docker     (122)     6902 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/DependencyTree.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/DependencyTree.h
+-rw-r--r--   0 runner    (1001) docker     (122)    14462 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/FillFptrTable.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1700 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/FillFptrTable.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/Global.h
+-rw-r--r--   0 runner    (1001) docker     (122)    69609 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/LibV1.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7239 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/LibV1.h
+-rw-r--r--   0 runner    (1001) docker     (122)    57446 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/LibV2.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8364 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/LibV2.h
+-rw-r--r--   0 runner    (1001) docker     (122)    40008 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/LibV3.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4874 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/LibV3.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3611 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/LibV4.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1596 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/LibV4.h
+-rw-r--r--   0 runner    (1001) docker     (122)   136506 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/LibV5.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    15913 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/LibV5.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6931 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/Utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3430 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/Utils.h
+-rw-r--r--   0 runner    (1001) docker     (122)    22270 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/cfeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3274 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/cfeature.h
+-rw-r--r--   0 runner    (1001) docker     (122)    10351 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/cppcore.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1829 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/eFELLogger.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3597 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/efel.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2399 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/efel.h
+-rw-r--r--   0 runner    (1001) docker     (122)     8378 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/mapoperations.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2832 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/mapoperations.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/types.h
+-rw-r--r--   0 runner    (1001) docker     (122)    10312 2023-04-20 11:46:25.000000 efel-4.1.93/efel/io.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 11:46:27.991787 efel-4.1.93/efel/pyfeatures/
+-rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-04-20 11:46:25.000000 efel-4.1.93/efel/pyfeatures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10308 2023-04-20 11:46:25.000000 efel-4.1.93/efel/pyfeatures/pyfeatures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-04-20 11:46:25.000000 efel-4.1.93/efel/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 11:46:27.987787 efel-4.1.93/efel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1318 2023-04-20 11:46:27.000000 efel-4.1.93/efel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-04-20 11:46:27.000000 efel-4.1.93/efel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 11:46:27.000000 efel-4.1.93/efel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-04-20 11:46:27.000000 efel-4.1.93/efel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-20 11:46:27.000000 efel-4.1.93/efel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-04-20 11:46:27.991787 efel-4.1.93/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4043 2023-04-20 11:46:25.000000 efel-4.1.93/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    69513 2023-04-20 11:46:25.000000 efel-4.1.93/versioneer.py
```

### Comparing `efel-4.1.91/COPYING` & `efel-4.1.93/COPYING`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/COPYING.less` & `efel-4.1.93/COPYING.less`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/LICENSE.txt` & `efel-4.1.93/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/PKG-INFO` & `efel-4.1.93/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efel
-Version: 4.1.91
+Version: 4.1.93
 Summary: Electrophys Feature Extract Library (eFEL)
 Home-page: https://github.com/BlueBrain/eFEL
 Author: BlueBrain Project, EPFL
 Maintainer: Werner Van Geit
 Maintainer-email: werner.vangeit@epfl.ch
 License: LGPLv3
 Keywords: feature,extraction,electrophysiology,BlueBrainProject
```

### Comparing `efel-4.1.91/README.md` & `efel-4.1.93/README.md`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/DependencyV5.txt` & `efel-4.1.93/efel/DependencyV5.txt`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/__init__.py` & `efel-4.1.93/efel/__init__.py`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/api.py` & `efel-4.1.93/efel/api.py`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/cppcore/DependencyTree.cpp` & `efel-4.1.93/efel/cppcore/DependencyTree.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/cppcore/DependencyTree.h` & `efel-4.1.93/efel/cppcore/DependencyTree.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/cppcore/FillFptrTable.cpp` & `efel-4.1.93/efel/cppcore/FillFptrTable.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/cppcore/FillFptrTable.h` & `efel-4.1.93/efel/cppcore/FillFptrTable.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/cppcore/Global.h` & `efel-4.1.93/efel/cppcore/Global.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/cppcore/LibV1.cpp` & `efel-4.1.93/efel/cppcore/LibV1.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/cppcore/LibV1.h` & `efel-4.1.93/efel/cppcore/LibV1.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/cppcore/LibV2.cpp` & `efel-4.1.93/efel/cppcore/LibV2.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/cppcore/LibV2.h` & `efel-4.1.93/efel/cppcore/LibV2.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/cppcore/LibV3.cpp` & `efel-4.1.93/efel/cppcore/LibV3.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/cppcore/LibV3.h` & `efel-4.1.93/efel/cppcore/LibV3.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/cppcore/LibV4.cpp` & `efel-4.1.93/efel/cppcore/LibV4.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/cppcore/LibV4.h` & `efel-4.1.93/efel/cppcore/LibV4.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/cppcore/LibV5.cpp` & `efel-4.1.93/efel/cppcore/LibV5.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -653,15 +653,15 @@
   // if the AHP_indices are already restricted make sure that we do not miss
   // the last spike
   // if(t[minima.back()] < stimend) {
   int endindex = distance(t.begin(), t.end());
   minima.push_back(endindex);
   //}
   // printf("Found %d minima\n", minima.size());
-  for (size_t i = 0; i < minima.size() - 1; i++) {
+  for (size_t i = 0; i < minima.size() - 2; i++) {
     // assure that the width of the slope is bigger than 4
     int newbegin = minima[i + 1];
     int begin = minima[i];
     int width = derivative_window;
     bool skip = false;
 
     // Detect where the derivate crosses derivativethreshold, and make sure
@@ -671,14 +671,18 @@
           dvdt.begin(),
           find_if(
               // use reverse iterator to get last occurence
               // and avoid false positive long before the spike
               dvdt.rbegin() + v.size() - newbegin,
               dvdt.rbegin() + v.size() - minima[i],
               std::bind2nd(std::less_equal<double>(), derivativethreshold)).base());
+      // cover edge case to avoid going out of index in the while condition
+      if (begin > endindex - width){
+        begin = endindex - width;
+      }
       // printf("%d %d\n", newbegin, minima[i+1]);
       if (begin == minima[i]) {
         // printf("Skipping %d %d\n", newbegin, minima[i+1]);
         // could not find a spike in between these minima
         skip = true;
         break;
       }
```

### Comparing `efel-4.1.91/efel/cppcore/LibV5.h` & `efel-4.1.93/efel/cppcore/LibV5.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/cppcore/Utils.cpp` & `efel-4.1.93/efel/cppcore/Utils.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/cppcore/Utils.h` & `efel-4.1.93/efel/cppcore/Utils.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/cppcore/cfeature.cpp` & `efel-4.1.93/efel/cppcore/cfeature.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/cppcore/cfeature.h` & `efel-4.1.93/efel/cppcore/cfeature.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/cppcore/cppcore.cpp` & `efel-4.1.93/efel/cppcore/cppcore.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/cppcore/eFELLogger.h` & `efel-4.1.93/efel/cppcore/eFELLogger.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/cppcore/efel.cpp` & `efel-4.1.93/efel/cppcore/efel.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/cppcore/efel.h` & `efel-4.1.93/efel/cppcore/efel.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/cppcore/mapoperations.cpp` & `efel-4.1.93/efel/cppcore/mapoperations.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/cppcore/mapoperations.h` & `efel-4.1.93/efel/cppcore/mapoperations.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/cppcore/types.h` & `efel-4.1.93/efel/cppcore/types.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/io.py` & `efel-4.1.93/efel/io.py`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/pyfeatures/__init__.py` & `efel-4.1.93/efel/pyfeatures/__init__.py`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/pyfeatures/pyfeatures.py` & `efel-4.1.93/efel/pyfeatures/pyfeatures.py`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel/settings.py` & `efel-4.1.93/efel/settings.py`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/efel.egg-info/PKG-INFO` & `efel-4.1.93/efel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efel
-Version: 4.1.91
+Version: 4.1.93
 Summary: Electrophys Feature Extract Library (eFEL)
 Home-page: https://github.com/BlueBrain/eFEL
 Author: BlueBrain Project, EPFL
 Maintainer: Werner Van Geit
 Maintainer-email: werner.vangeit@epfl.ch
 License: LGPLv3
 Keywords: feature,extraction,electrophysiology,BlueBrainProject
```

### Comparing `efel-4.1.91/efel.egg-info/SOURCES.txt` & `efel-4.1.93/efel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/setup.py` & `efel-4.1.93/setup.py`

 * *Files identical despite different names*

### Comparing `efel-4.1.91/versioneer.py` & `efel-4.1.93/versioneer.py`

 * *Files identical despite different names*

