# Comparing `tmp/pyiron_gui-0.0.8.tar.gz` & `tmp/pyiron_gui-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron_gui-0.0.8.tar", last modified: Fri Sep  2 09:51:05 2022, max compression
+gzip compressed data, was "pyiron_gui-0.0.9.tar", last modified: Mon Nov 21 18:58:35 2022, max compression
```

## Comparing `pyiron_gui-0.0.8.tar` & `pyiron_gui-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 09:51:05.398573 pyiron_gui-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1622 2022-09-02 09:50:58.000000 pyiron_gui-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-09-02 09:50:58.000000 pyiron_gui-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      854 2022-09-02 09:51:05.398573 pyiron_gui-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      843 2022-09-02 09:50:58.000000 pyiron_gui-0.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 09:51:05.394573 pyiron_gui-0.0.8/pyiron_gui/
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-09-02 09:50:58.000000 pyiron_gui-0.0.8/pyiron_gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18705 2022-09-02 09:50:58.000000 pyiron_gui-0.0.8/pyiron_gui/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 09:51:05.398573 pyiron_gui-0.0.8/pyiron_gui/project/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-02 09:50:58.000000 pyiron_gui-0.0.8/pyiron_gui/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1947 2022-09-02 09:50:58.000000 pyiron_gui-0.0.8/pyiron_gui/project/project.py
--rw-r--r--   0 runner    (1001) docker     (121)    29511 2022-09-02 09:50:58.000000 pyiron_gui-0.0.8/pyiron_gui/project/project_browser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 09:51:05.398573 pyiron_gui-0.0.8/pyiron_gui/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-02 09:50:58.000000 pyiron_gui-0.0.8/pyiron_gui/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3078 2022-09-02 09:50:58.000000 pyiron_gui-0.0.8/pyiron_gui/utils/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 09:51:05.398573 pyiron_gui-0.0.8/pyiron_gui/widgets/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-02 09:50:58.000000 pyiron_gui-0.0.8/pyiron_gui/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      840 2022-09-02 09:50:58.000000 pyiron_gui-0.0.8/pyiron_gui/widgets/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 09:51:05.398573 pyiron_gui-0.0.8/pyiron_gui/wrapper/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-02 09:50:58.000000 pyiron_gui-0.0.8/pyiron_gui/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13917 2022-09-02 09:50:58.000000 pyiron_gui-0.0.8/pyiron_gui/wrapper/widgets.py
--rw-r--r--   0 runner    (1001) docker     (121)     3684 2022-09-02 09:50:58.000000 pyiron_gui-0.0.8/pyiron_gui/wrapper/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 09:51:05.398573 pyiron_gui-0.0.8/pyiron_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      854 2022-09-02 09:51:05.000000 pyiron_gui-0.0.8/pyiron_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-09-02 09:51:05.000000 pyiron_gui-0.0.8/pyiron_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-02 09:51:05.000000 pyiron_gui-0.0.8/pyiron_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-09-02 09:51:05.000000 pyiron_gui-0.0.8/pyiron_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-09-02 09:51:05.000000 pyiron_gui-0.0.8/pyiron_gui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-09-02 09:51:05.398573 pyiron_gui-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1385 2022-09-02 09:51:04.000000 pyiron_gui-0.0.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    70144 2022-09-02 09:50:58.000000 pyiron_gui-0.0.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-21 18:58:35.607617 pyiron_gui-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (122)     1593 2022-11-21 18:58:31.000000 pyiron_gui-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2022-11-21 18:58:31.000000 pyiron_gui-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      854 2022-11-21 18:58:35.607617 pyiron_gui-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2022-11-21 18:58:31.000000 pyiron_gui-0.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-21 18:58:35.607617 pyiron_gui-0.0.9/pyiron_gui/
+-rw-r--r--   0 runner    (1001) docker     (122)      363 2022-11-21 18:58:31.000000 pyiron_gui-0.0.9/pyiron_gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      496 2022-11-21 18:58:35.607617 pyiron_gui-0.0.9/pyiron_gui/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4512 2022-11-21 18:58:31.000000 pyiron_gui-0.0.9/pyiron_gui/monkey_patching.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-21 18:58:35.607617 pyiron_gui-0.0.9/pyiron_gui/project/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-21 18:58:31.000000 pyiron_gui-0.0.9/pyiron_gui/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1947 2022-11-21 18:58:31.000000 pyiron_gui-0.0.9/pyiron_gui/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29511 2022-11-21 18:58:31.000000 pyiron_gui-0.0.9/pyiron_gui/project/project_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-21 18:58:35.607617 pyiron_gui-0.0.9/pyiron_gui/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-21 18:58:31.000000 pyiron_gui-0.0.9/pyiron_gui/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3078 2022-11-21 18:58:31.000000 pyiron_gui-0.0.9/pyiron_gui/utils/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-21 18:58:35.607617 pyiron_gui-0.0.9/pyiron_gui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-21 18:58:31.000000 pyiron_gui-0.0.9/pyiron_gui/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2022-11-21 18:58:31.000000 pyiron_gui-0.0.9/pyiron_gui/widgets/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-21 18:58:35.607617 pyiron_gui-0.0.9/pyiron_gui/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-21 18:58:31.000000 pyiron_gui-0.0.9/pyiron_gui/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13917 2022-11-21 18:58:31.000000 pyiron_gui-0.0.9/pyiron_gui/wrapper/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3684 2022-11-21 18:58:31.000000 pyiron_gui-0.0.9/pyiron_gui/wrapper/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-21 18:58:35.603617 pyiron_gui-0.0.9/pyiron_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      854 2022-11-21 18:58:35.000000 pyiron_gui-0.0.9/pyiron_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      619 2022-11-21 18:58:35.000000 pyiron_gui-0.0.9/pyiron_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-21 18:58:35.000000 pyiron_gui-0.0.9/pyiron_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2022-11-21 18:58:35.000000 pyiron_gui-0.0.9/pyiron_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2022-11-21 18:58:35.000000 pyiron_gui-0.0.9/pyiron_gui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2022-11-21 18:58:35.607617 pyiron_gui-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1384 2022-11-21 18:58:35.000000 pyiron_gui-0.0.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    70144 2022-11-21 18:58:31.000000 pyiron_gui-0.0.9/versioneer.py
```

### Comparing `pyiron_gui-0.0.8/LICENSE` & `pyiron_gui-0.0.9/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-BSD 3-Clause License
-
-Copyright (c) 2020, Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-* Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
-
-* Redistributions in binary form must reproduce the above copyright notice,
-  this list of conditions and the following disclaimer in the documentation
-  and/or other materials provided with the distribution.
-
-* Neither the name of the copyright holder nor the names of its
-  contributors may be used to endorse or promote products derived from
-  this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2020, Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice,
+  this list of conditions and the following disclaimer in the documentation
+  and/or other materials provided with the distribution.
+
+* Neither the name of the copyright holder nor the names of its
+  contributors may be used to endorse or promote products derived from
+  this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `pyiron_gui-0.0.8/PKG-INFO` & `pyiron_gui-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_gui
-Version: 0.0.8
+Version: 0.0.9
 Summary: Repository for GUI plugins to the pyiron IDE.
 Home-page: https://github.com/pyiron/pyiron_gui
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: siemer@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyiron_gui-0.0.8/README.rst` & `pyiron_gui-0.0.9/README.rst`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-pyiron_gui
-============
-.. image:: https://coveralls.io/repos/github/pyiron/pyiron_gui/badge.svg?branch=master
-    :target: https://coveralls.io/github/pyiron/pyiron_gui?branch=master
-    :alt: Coverage Status
-
-.. image:: https://anaconda.org/conda-forge/pyiron_gui/badges/latest_release_date.svg
-    :target: https://anaconda.org/conda-forge/pyiron_gui/
-    :alt: Release_Date
-
-.. image:: https://github.com/pyiron/pyiron_gui/workflows/Python%20package/badge.svg
-    :target: https://github.com/pyiron//pyiron_gui/actions
-    :alt: Build Status
-
-    
-This repository is for GUI extensions to the overall pyiron framework.
-
-Getting started:
-----------------
-Test pyiron with mybinder:
-
-.. image:: https://mybinder.org/badge_logo.svg
-     :target: https://mybinder.org/v2/gh/pyiron/pyiron_gui/master
-     :alt: mybinder
+pyiron_gui
+============
+.. image:: https://coveralls.io/repos/github/pyiron/pyiron_gui/badge.svg?branch=master
+    :target: https://coveralls.io/github/pyiron/pyiron_gui?branch=master
+    :alt: Coverage Status
+
+.. image:: https://anaconda.org/conda-forge/pyiron_gui/badges/latest_release_date.svg
+    :target: https://anaconda.org/conda-forge/pyiron_gui/
+    :alt: Release_Date
+
+.. image:: https://github.com/pyiron/pyiron_gui/workflows/Python%20package/badge.svg
+    :target: https://github.com/pyiron//pyiron_gui/actions
+    :alt: Build Status
+
+    
+This repository is for GUI extensions to the overall pyiron framework.
+
+Getting started:
+----------------
+Test pyiron with mybinder:
+
+.. image:: https://mybinder.org/badge_logo.svg
+     :target: https://mybinder.org/v2/gh/pyiron/pyiron_gui/master
+     :alt: mybinder
```

### Comparing `pyiron_gui-0.0.8/pyiron_gui/project/project.py` & `pyiron_gui-0.0.9/pyiron_gui/project/project.py`

 * *Files identical despite different names*

### Comparing `pyiron_gui-0.0.8/pyiron_gui/project/project_browser.py` & `pyiron_gui-0.0.9/pyiron_gui/project/project_browser.py`

 * *Files identical despite different names*

### Comparing `pyiron_gui-0.0.8/pyiron_gui/utils/decorators.py` & `pyiron_gui-0.0.9/pyiron_gui/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `pyiron_gui-0.0.8/pyiron_gui/widgets/widgets.py` & `pyiron_gui-0.0.9/pyiron_gui/widgets/widgets.py`

 * *Files identical despite different names*

### Comparing `pyiron_gui-0.0.8/pyiron_gui/wrapper/widgets.py` & `pyiron_gui-0.0.9/pyiron_gui/wrapper/widgets.py`

 * *Files identical despite different names*

### Comparing `pyiron_gui-0.0.8/pyiron_gui/wrapper/wrapper.py` & `pyiron_gui-0.0.9/pyiron_gui/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyiron_gui-0.0.8/pyiron_gui.egg-info/PKG-INFO` & `pyiron_gui-0.0.9/pyiron_gui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron-gui
-Version: 0.0.8
+Version: 0.0.9
 Summary: Repository for GUI plugins to the pyiron IDE.
 Home-page: https://github.com/pyiron/pyiron_gui
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: siemer@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyiron_gui-0.0.8/pyiron_gui.egg-info/SOURCES.txt` & `pyiron_gui-0.0.9/pyiron_gui.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 versioneer.py
 pyiron_gui/__init__.py
 pyiron_gui/_version.py
+pyiron_gui/monkey_patching.py
 pyiron_gui.egg-info/PKG-INFO
 pyiron_gui.egg-info/SOURCES.txt
 pyiron_gui.egg-info/dependency_links.txt
 pyiron_gui.egg-info/requires.txt
 pyiron_gui.egg-info/top_level.txt
 pyiron_gui/project/__init__.py
 pyiron_gui/project/project.py
```

### Comparing `pyiron_gui-0.0.8/versioneer.py` & `pyiron_gui-0.0.9/versioneer.py`

 * *Files identical despite different names*

