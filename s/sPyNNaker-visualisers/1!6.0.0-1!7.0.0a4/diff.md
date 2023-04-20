# Comparing `tmp/sPyNNaker_visualisers-1!6.0.0.tar.gz` & `tmp/sPyNNaker_visualisers-1!7.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sPyNNaker_visualisers-1!6.0.0.tar", last modified: Mon Apr 12 14:45:31 2021, max compression
+gzip compressed data, was "sPyNNaker_visualisers-1!7.0.0a4.tar", last modified: Wed Apr 19 15:14:59 2023, max compression
```

## Comparing `sPyNNaker_visualisers-1!6.0.0.tar` & `sPyNNaker_visualisers-1!7.0.0a4.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 zzalsar4  (1000) zzalsar4  (1000)        0 2021-04-12 14:45:31.037109 sPyNNaker_visualisers-1!6.0.0/
--rw-rw-r--   0 zzalsar4  (1000) zzalsar4  (1000)     1971 2021-02-17 13:30:21.000000 sPyNNaker_visualisers-1!6.0.0/CITATION.cff
--rwxr-xr-x   0 zzalsar4  (1000) zzalsar4  (1000)     1019 2020-09-21 12:34:36.000000 sPyNNaker_visualisers-1!6.0.0/LICENSE.md
--rwxr-xr-x   0 zzalsar4  (1000) zzalsar4  (1000)       63 2020-09-21 12:34:36.000000 sPyNNaker_visualisers-1!6.0.0/MANIFEST.in
--rw-r--r--   0 zzalsar4  (1000) zzalsar4  (1000)      999 2021-04-12 14:45:31.037109 sPyNNaker_visualisers-1!6.0.0/PKG-INFO
--rw-rw-r--   0 zzalsar4  (1000) zzalsar4  (1000)      196 2021-04-12 12:24:28.000000 sPyNNaker_visualisers-1!6.0.0/README.md
--rwxr-xr-x   0 zzalsar4  (1000) zzalsar4  (1000)       90 2020-09-21 12:34:36.000000 sPyNNaker_visualisers-1!6.0.0/pypi_to_import
--rw-rw-r--   0 zzalsar4  (1000) zzalsar4  (1000)      990 2021-04-12 12:31:03.000000 sPyNNaker_visualisers-1!6.0.0/requirements.txt
-drwxr-xr-x   0 zzalsar4  (1000) zzalsar4  (1000)        0 2021-04-12 14:45:31.037109 sPyNNaker_visualisers-1!6.0.0/sPyNNaker_visualisers.egg-info/
--rwxr-xr-x   0 zzalsar4  (1000) zzalsar4  (1000)      999 2021-04-12 14:45:30.000000 sPyNNaker_visualisers-1!6.0.0/sPyNNaker_visualisers.egg-info/PKG-INFO
--rwxr-xr-x   0 zzalsar4  (1000) zzalsar4  (1000)      718 2021-04-12 14:45:31.000000 sPyNNaker_visualisers-1!6.0.0/sPyNNaker_visualisers.egg-info/SOURCES.txt
--rwxr-xr-x   0 zzalsar4  (1000) zzalsar4  (1000)        1 2021-04-12 14:45:30.000000 sPyNNaker_visualisers-1!6.0.0/sPyNNaker_visualisers.egg-info/dependency_links.txt
--rwxr-xr-x   0 zzalsar4  (1000) zzalsar4  (1000)      150 2021-04-12 14:45:30.000000 sPyNNaker_visualisers-1!6.0.0/sPyNNaker_visualisers.egg-info/entry_points.txt
--rwxr-xr-x   0 zzalsar4  (1000) zzalsar4  (1000)       98 2021-04-12 14:45:30.000000 sPyNNaker_visualisers-1!6.0.0/sPyNNaker_visualisers.egg-info/requires.txt
--rwxr-xr-x   0 zzalsar4  (1000) zzalsar4  (1000)       22 2021-04-12 14:45:30.000000 sPyNNaker_visualisers-1!6.0.0/sPyNNaker_visualisers.egg-info/top_level.txt
--rw-r--r--   0 zzalsar4  (1000) zzalsar4  (1000)       38 2021-04-12 14:45:31.037109 sPyNNaker_visualisers-1!6.0.0/setup.cfg
--rw-rw-r--   0 zzalsar4  (1000) zzalsar4  (1000)     2350 2021-04-12 14:11:08.000000 sPyNNaker_visualisers-1!6.0.0/setup.py
-drwxr-xr-x   0 zzalsar4  (1000) zzalsar4  (1000)        0 2021-04-12 14:45:31.037109 sPyNNaker_visualisers-1!6.0.0/spynnaker_visualisers/
--rw-rw-r--   0 zzalsar4  (1000) zzalsar4  (1000)      960 2021-02-17 13:30:21.000000 sPyNNaker_visualisers-1!6.0.0/spynnaker_visualisers/__init__.py
--rw-rw-r--   0 zzalsar4  (1000) zzalsar4  (1000)     1146 2021-04-12 12:24:28.000000 sPyNNaker_visualisers-1!6.0.0/spynnaker_visualisers/_bigsurhack.py
--rw-rw-r--   0 zzalsar4  (1000) zzalsar4  (1000)      834 2021-04-12 12:31:03.000000 sPyNNaker_visualisers-1!6.0.0/spynnaker_visualisers/_version.py
--rw-rw-r--   0 zzalsar4  (1000) zzalsar4  (1000)    13763 2021-04-12 12:24:28.000000 sPyNNaker_visualisers-1!6.0.0/spynnaker_visualisers/glut_framework.py
--rw-rw-r--   0 zzalsar4  (1000) zzalsar4  (1000)     3997 2021-04-12 12:24:28.000000 sPyNNaker_visualisers-1!6.0.0/spynnaker_visualisers/opengl_support.py
-drwxr-xr-x   0 zzalsar4  (1000) zzalsar4  (1000)        0 2021-04-12 14:45:31.037109 sPyNNaker_visualisers-1!6.0.0/spynnaker_visualisers/raytrace/
--rw-rw-r--   0 zzalsar4  (1000) zzalsar4  (1000)      691 2021-04-12 12:24:28.000000 sPyNNaker_visualisers-1!6.0.0/spynnaker_visualisers/raytrace/__init__.py
--rw-rw-r--   0 zzalsar4  (1000) zzalsar4  (1000)     7878 2021-04-12 12:24:28.000000 sPyNNaker_visualisers-1!6.0.0/spynnaker_visualisers/raytrace/drawer.py
-drwxr-xr-x   0 zzalsar4  (1000) zzalsar4  (1000)        0 2021-04-12 14:45:31.037109 sPyNNaker_visualisers-1!6.0.0/spynnaker_visualisers/sudoku/
--rw-rw-r--   0 zzalsar4  (1000) zzalsar4  (1000)      691 2021-02-17 13:30:21.000000 sPyNNaker_visualisers-1!6.0.0/spynnaker_visualisers/sudoku/__init__.py
--rw-rw-r--   0 zzalsar4  (1000) zzalsar4  (1000)    15130 2021-04-12 12:24:28.000000 sPyNNaker_visualisers-1!6.0.0/spynnaker_visualisers/sudoku/sudoku_visualiser.py
+drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-04-19 15:14:59.534218 sPyNNaker_visualisers-1!7.0.0a4/
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5109 2023-03-10 13:09:30.000000 sPyNNaker_visualisers-1!7.0.0a4/CITATION.cff
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    11360 2023-04-17 09:39:08.000000 sPyNNaker_visualisers-1!7.0.0a4/LICENSE
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      979 2023-03-10 13:09:30.000000 sPyNNaker_visualisers-1!7.0.0a4/LICENSE_POLICY.md
+-rw-r--r--   0 brenninc  (1000) brenninc  (1000)       63 2019-06-11 14:37:19.000000 sPyNNaker_visualisers-1!7.0.0a4/MANIFEST.in
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1361 2023-04-19 15:14:59.534218 sPyNNaker_visualisers-1!7.0.0a4/PKG-INFO
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      197 2023-04-19 15:14:56.000000 sPyNNaker_visualisers-1!7.0.0a4/README.md
+-rw-r--r--   0 brenninc  (1000) brenninc  (1000)       90 2019-06-11 14:37:19.000000 sPyNNaker_visualisers-1!7.0.0a4/pypi_to_import
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      678 2023-04-18 10:28:49.000000 sPyNNaker_visualisers-1!7.0.0a4/pyproject.toml
+drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-04-19 15:14:59.534218 sPyNNaker_visualisers-1!7.0.0a4/sPyNNaker_visualisers.egg-info/
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1361 2023-04-19 15:14:59.000000 sPyNNaker_visualisers-1!7.0.0a4/sPyNNaker_visualisers.egg-info/PKG-INFO
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      733 2023-04-19 15:14:59.000000 sPyNNaker_visualisers-1!7.0.0a4/sPyNNaker_visualisers.egg-info/SOURCES.txt
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)        1 2023-04-19 15:14:59.000000 sPyNNaker_visualisers-1!7.0.0a4/sPyNNaker_visualisers.egg-info/dependency_links.txt
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)       63 2023-04-19 15:14:59.000000 sPyNNaker_visualisers-1!7.0.0a4/sPyNNaker_visualisers.egg-info/requires.txt
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)       22 2023-04-19 15:14:59.000000 sPyNNaker_visualisers-1!7.0.0a4/sPyNNaker_visualisers.egg-info/top_level.txt
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)        1 2023-04-19 15:14:59.000000 sPyNNaker_visualisers-1!7.0.0a4/sPyNNaker_visualisers.egg-info/zip-safe
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1255 2023-04-19 15:14:59.534218 sPyNNaker_visualisers-1!7.0.0a4/setup.cfg
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1336 2023-04-11 13:16:45.000000 sPyNNaker_visualisers-1!7.0.0a4/setup.py
+drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-04-19 15:14:59.534218 sPyNNaker_visualisers-1!7.0.0a4/spynnaker_visualisers/
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      866 2023-03-08 14:17:47.000000 sPyNNaker_visualisers-1!7.0.0a4/spynnaker_visualisers/__init__.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1052 2023-03-08 14:17:47.000000 sPyNNaker_visualisers-1!7.0.0a4/spynnaker_visualisers/_bigsurhack.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      735 2023-04-19 15:14:56.000000 sPyNNaker_visualisers-1!7.0.0a4/spynnaker_visualisers/_version.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    13431 2023-03-10 13:09:30.000000 sPyNNaker_visualisers-1!7.0.0a4/spynnaker_visualisers/glut_framework.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     3936 2023-03-08 14:17:47.000000 sPyNNaker_visualisers-1!7.0.0a4/spynnaker_visualisers/opengl_support.py
+drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-04-19 15:14:59.534218 sPyNNaker_visualisers-1!7.0.0a4/spynnaker_visualisers/raytrace/
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      597 2023-03-08 14:17:47.000000 sPyNNaker_visualisers-1!7.0.0a4/spynnaker_visualisers/raytrace/__init__.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     7839 2023-03-08 14:17:47.000000 sPyNNaker_visualisers-1!7.0.0a4/spynnaker_visualisers/raytrace/drawer.py
+drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-04-19 15:14:59.534218 sPyNNaker_visualisers-1!7.0.0a4/spynnaker_visualisers/sudoku/
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      597 2023-03-08 14:17:47.000000 sPyNNaker_visualisers-1!7.0.0a4/spynnaker_visualisers/sudoku/__init__.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    15185 2023-03-08 14:17:47.000000 sPyNNaker_visualisers-1!7.0.0a4/spynnaker_visualisers/sudoku/sudoku_visualiser.py
```

### Comparing `sPyNNaker_visualisers-1!6.0.0/LICENSE.md` & `sPyNNaker_visualisers-1!7.0.0a4/LICENSE_POLICY.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # License Agreement
 
-Up to date information for the whole [SpiNNakerManchester Projects](https://github.com/SpiNNakerManchester) can be found [here](http://spinnakermanchester.github.io/common_pages/4.0.0/LicenseAgreement.html)
+Up to date information for the whole [SpiNNakerManchester Projects](https://github.com/SpiNNakerManchester) can be found [here](https://spinnakermanchester.github.io/latest/LicenseAgreement.html)
 
-As shown there the software is currently being released under the GPL version 3 license listed [here](http://www.gnu.org/copyleft/gpl.html)
+As shown there the software is currently being released under the Apache License 2.0 listed [here](https://www.apache.org/licenses/LICENSE-2.0)
 
 
 # Paper Authorship
 
-See: [here](http://spinnakermanchester.github.io/common_pages/4.0.0/LicenseAgreement.html#paper-authorship)
+See: [here](https://spinnakermanchester.github.io/latest/LicenseAgreement.html#paper-authorship)
 
 # Modifications
 
-See: [here](http://spinnakermanchester.github.io/common_pages/4.0.0/LicenseAgreement.html#modifications)
+See: [here](https://spinnakermanchester.github.io/latest/LicenseAgreement.html#modifications)
 
 # Contributors
 
 For up to date information on Contributors see the graphs/contributors pages on each project.
 
 For example [https://github.com/SpiNNakerManchester/sPyNNakerVisualisers/graphs/contributors](https://github.com/SpiNNakerManchester/sPyNNakerVisualisers/graphs/contributors)
 
-[Combined list](http://spinnakermanchester.github.io/common_pages/4.0.0/LicenseAgreement.html#contributors)
+[Combined list](https://spinnakermanchester.github.io/latest/LicenseAgreement.html#contributors)
```

### Comparing `sPyNNaker_visualisers-1!6.0.0/sPyNNaker_visualisers.egg-info/SOURCES.txt` & `sPyNNaker_visualisers-1!7.0.0a4/sPyNNaker_visualisers.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 CITATION.cff
-LICENSE.md
+LICENSE
+LICENSE_POLICY.md
 MANIFEST.in
 README.md
 pypi_to_import
-requirements.txt
+pyproject.toml
+setup.cfg
 setup.py
 sPyNNaker_visualisers.egg-info/PKG-INFO
 sPyNNaker_visualisers.egg-info/SOURCES.txt
 sPyNNaker_visualisers.egg-info/dependency_links.txt
-sPyNNaker_visualisers.egg-info/entry_points.txt
 sPyNNaker_visualisers.egg-info/requires.txt
 sPyNNaker_visualisers.egg-info/top_level.txt
+sPyNNaker_visualisers.egg-info/zip-safe
 spynnaker_visualisers/__init__.py
 spynnaker_visualisers/_bigsurhack.py
 spynnaker_visualisers/_version.py
 spynnaker_visualisers/glut_framework.py
 spynnaker_visualisers/opengl_support.py
 spynnaker_visualisers/raytrace/__init__.py
 spynnaker_visualisers/raytrace/drawer.py
```

### Comparing `sPyNNaker_visualisers-1!6.0.0/spynnaker_visualisers/__init__.py` & `sPyNNaker_visualisers-1!7.0.0a4/spynnaker_visualisers/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-# Copyright (c) 2018-2021 The University of Manchester
+# Copyright (c) 2017 The University of Manchester
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+#     https://www.apache.org/licenses/LICENSE-2.0
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
 from spynnaker_visualisers._version import __version__  # NOQA
 from spynnaker_visualisers._version import __version_name__  # NOQA
 from spynnaker_visualisers._version import __version_month__  # NOQA
 from spynnaker_visualisers._version import __version_year__  # NOQA
```

### Comparing `sPyNNaker_visualisers-1!6.0.0/spynnaker_visualisers/glut_framework.py` & `sPyNNaker_visualisers-1!7.0.0a4/spynnaker_visualisers/glut_framework.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 """
 A basic framework that implements the basic system handling for a GUI
 application that uses OpenGL and GLUT to do the GUI work.
 """
-# The MIT License
 #
-# Copyright (c) 2010 Paul Solt, PaulSolt@gmail.com
+# Copyright (c) 2017 The University of Manchester
+# Based on work Copyright (c) 2010 Paul Solt, PaulSolt@gmail.com
+# Originally released under the MIT License
 #
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-# The above copyright notice and this permission notice shall be included in
-# all copies or substantial portions of the Software.
+#     https://www.apache.org/licenses/LICENSE-2.0
 #
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-# THE SOFTWARE.
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 #
 # @author: Converted to Python by Donal Fellows
 
 from datetime import datetime
 import os
 import traceback
 import OpenGL.error
@@ -120,14 +115,15 @@
         self.frame_time_elapsed = 0.0
         self.frame_time = 0.0
         self.frame_rate_timer = _PerformanceTimer()
         self.display_timer = _PerformanceTimer()
         self.elapsed_time_in_seconds = 0.0
         self._logged_errors = set()
 
+    # pylint: disable=unsupported-binary-operation
     def start_framework(self, args, title, width, height, posx, posy, fps, *,
                         display_mode=GLUT.GLUT_RGB | GLUT.GLUT_DOUBLE):
         """ start_framework will initialize framework and start the GLUT run\
             loop. It must be called after the GlutFramework class is created\
             to start the application.
 
         Not expected to return.
@@ -218,15 +214,15 @@
         :param x: the x coordinate of the mouse
         :param y: the y coordinate of the mouse
         """
 
     def special_keyboard_down(self, key, x, y):
         """ The keyboard function is called when a special key is pressed down\
             (F1 keys, Home, Inser, Delete, Page Up/Down, End, arrow keys).\
-            http://www.opengl.org/resources/libraries/glut/spec3/node54.html
+            https://www.opengl.org/resources/libraries/glut/spec3/node54.html
 
         :param key: the key press
         :param x: the x coordinate of the mouse
         :param y: the y coordinate of the mouse
         """
 
     def special_keyboard_up(self, key, x, y):
@@ -312,15 +308,15 @@
             disable(blend, line_smooth)
 
     @staticmethod
     def _terminate(exit_code=0):
         """
         Because sys.exit() doesn't always work in the ctype-handled callbacks.
         """
-        os._exit(exit_code)
+        os._exit(exit_code)  # pylint: disable=protected-access
 
     def __display_framework(self):
         if not GLUT.glutGetWindow():
             return
         try:
             return self.display_framework()
         except Exception:
```

### Comparing `sPyNNaker_visualisers-1!6.0.0/spynnaker_visualisers/opengl_support.py` & `sPyNNaker_visualisers-1!7.0.0a4/spynnaker_visualisers/opengl_support.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-# Copyright (c) 2018-2021 The University of Manchester
+# Copyright (c) 2018 The University of Manchester
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+#     https://www.apache.org/licenses/LICENSE-2.0
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
 """
 This file makes the OpenGL interface a little more python-pretty. It's
 massively incomplete; feel free to add to it as required.
 """
 
 from contextlib import contextmanager
 try:
     # this fails in <=2020 versions of Python on OS X 11.x
-    import OpenGL.GL  # noqa: F401
+    import OpenGL.GL  # noqa: F401  # pylint: disable=unused-import
 except ImportError:
     # Hack for macOS Big Sur
     from ._bigsurhack import patch_ctypes
     patch_ctypes()
 import OpenGL.GL as GL
 
 # pylint: disable=invalid-name
```

### Comparing `sPyNNaker_visualisers-1!6.0.0/spynnaker_visualisers/raytrace/drawer.py` & `sPyNNaker_visualisers-1!7.0.0a4/spynnaker_visualisers/raytrace/drawer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-# Copyright (c) 2018-2021 The University of Manchester
+# Copyright (c) 2017 The University of Manchester
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+#     https://www.apache.org/licenses/LICENSE-2.0
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
 import socket
 import struct
 import sys
 import threading
 from numpy import dot, cross, array, zeros, cos, sin, uint8, uint32
 from numpy.linalg import norm
@@ -72,14 +71,15 @@
 
     def init(self):
         gl.enable(gl.blend, gl.depth_test)
         gl.blend_function(gl.src_alpha, gl.one_minus_src_alpha)
 
     def display(self, dTime):
         gl.clear_color(1.0, 1.0, 1.0, 0.001)
+        # pylint: disable=unsupported-binary-operation
         gl.clear(gl.color_buffer_bit | gl.depth_buffer_bit)
         gl.draw_pixels(
             self._win_width, self._win_height, gl.rgb, gl.unsigned_byte,
             self._viewing_frame.data)
 
     def reshape(self, width, height):
         self._win_width = min(width, self._width)
```

### Comparing `sPyNNaker_visualisers-1!6.0.0/spynnaker_visualisers/sudoku/sudoku_visualiser.py` & `sPyNNaker_visualisers-1!7.0.0a4/spynnaker_visualisers/sudoku/sudoku_visualiser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-# Copyright (c) 2018-2021 The University of Manchester
+# Copyright (c) 2017 The University of Manchester
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+#     https://www.apache.org/licenses/LICENSE-2.0
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
 # encoding: utf-8
 """ A live plotter for the sPyNNaker Sudoku network.
 """
 from argparse import ArgumentParser, REMAINDER
 import sys
 from threading import Condition, RLock
@@ -278,15 +277,17 @@
     @staticmethod
     def _start_display():
         point_size(1.0)
         clear(color_buffer_bit)
         clear_color(1.0, 1.0, 1.0, 1.0)
         color(0.0, 0.0, 0.0, 1.0)
 
-    def _print_text(self, prompt):  # FIXME positioning
+    # TODO positioning
+    # https://github.com/SpiNNakerManchester/sPyNNakerVisualisers/issues/23
+    def _print_text(self, prompt):
         # Guesstimate of length of prompt in pixels
         plen = len(prompt) * 4
         self.write_large(
             self.window_width / 2 - plen, self.window_height - 50, prompt)
 
     def _draw_cells(self, width, height):
         color(0.0, 0.0, 0.0, 1.0)
@@ -340,27 +341,28 @@
     @staticmethod
     def _check_cell(values, correct, x, y, row, col):
         value = values[y * 9 + x]
         if value == values[row * 9 + col]:
             correct[y * 9 + x] = False
 
 
+# https://github.com/SpiNNakerManchester/sPyNNakerVisualisers/issues/24
 def sudoku_visualiser(args, port=19999, neurons=5, ms=100, database=None):
     """ Make a visualiser, connecting a LiveEventConnection that listens to a\
         population labelled "Cells" to a GLUT GUI.
     """
     # Set up the application
     cells = ["Cells"]
     connection = LiveEventConnection(
         "LiveSpikeReceiver", receive_labels=cells, local_port=port)
     plotter = SudokuPlot(args, neurons, ms, database is None)
     for label in cells:
         plotter.connect_callbacks(connection, label)
     if database is not None:
-        # FIXME: This concept not present on Python side!
+        # TODO: This concept not present on Python side!
         # connection.set_database(database)
         sys.stderr.write("Database setting not currently supported")
     plotter.main_loop()
 
 
 def main(argv=None):
     """ The main script.\
```

