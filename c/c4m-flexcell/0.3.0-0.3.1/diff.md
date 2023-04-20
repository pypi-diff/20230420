# Comparing `tmp/c4m_flexcell-0.3.0.tar.gz` & `tmp/c4m_flexcell-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c4m_flexcell-0.3.0.tar", last modified: Wed Mar  8 16:11:18 2023, max compression
+gzip compressed data, was "c4m_flexcell-0.3.1.tar", last modified: Thu Apr 20 14:00:35 2023, max compression
```

## Comparing `c4m_flexcell-0.3.0.tar` & `c4m_flexcell-0.3.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:11:18.683272 c4m_flexcell-0.3.0/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       96 2022-07-12 15:00:24.000000 c4m_flexcell-0.3.0/.gitignore
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1252 2022-11-01 15:19:21.000000 c4m_flexcell-0.3.0/.gitlab-ci.yml
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      484 2020-07-06 13:05:29.000000 c4m_flexcell-0.3.0/COPYRIGHT.md
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      782 2021-03-14 14:00:40.000000 c4m_flexcell-0.3.0/LICENSE.md
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:11:18.675272 c4m_flexcell-0.3.0/LICENSES/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    34523 2021-03-14 14:00:40.000000 c4m_flexcell-0.3.0/LICENSES/agpl-3.0.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13419 2020-07-06 09:58:12.000000 c4m_flexcell-0.3.0/LICENSES/cern_ohl_s_v2.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18009 2021-03-14 14:00:40.000000 c4m_flexcell-0.3.0/LICENSES/gpl-2.0.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4098 2023-03-08 16:11:18.683272 c4m_flexcell-0.3.0/PKG-INFO
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3626 2023-03-08 14:29:40.000000 c4m_flexcell-0.3.0/README.md
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:11:18.675272 c4m_flexcell-0.3.0/ReleaseNotes/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      321 2021-03-14 14:00:41.000000 c4m_flexcell-0.3.0/ReleaseNotes/v0.0.4.md
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      462 2022-08-22 13:25:11.000000 c4m_flexcell-0.3.0/ReleaseNotes/v0.1.0.md
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:11:18.675272 c4m_flexcell-0.3.0/c4m/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      149 2021-03-14 14:00:40.000000 c4m_flexcell-0.3.0/c4m/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2247 2021-05-15 12:46:28.000000 c4m_flexcell-0.3.0/c4m/cell_canvas.ipynb
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:11:18.679273 c4m_flexcell-0.3.0/c4m/flexcell/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      107 2023-03-03 18:21:14.000000 c4m_flexcell-0.3.0/c4m/flexcell/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)   622096 2022-12-05 14:11:33.000000 c4m_flexcell-0.3.0/c4m/flexcell/_cells.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)   106579 2023-03-07 17:12:53.000000 c4m_flexcell-0.3.0/c4m/flexcell/factory.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    52730 2023-03-03 18:21:47.000000 c4m_flexcell-0.3.0/c4m/flexcell/stdcell.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:11:18.679273 c4m_flexcell-0.3.0/c4m_flexcell.egg-info/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4098 2023-03-08 16:11:18.000000 c4m_flexcell-0.3.0/c4m_flexcell.egg-info/PKG-INFO
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      686 2023-03-08 16:11:18.000000 c4m_flexcell-0.3.0/c4m_flexcell.egg-info/SOURCES.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        1 2023-03-08 16:11:18.000000 c4m_flexcell-0.3.0/c4m_flexcell.egg-info/dependency_links.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       28 2023-03-08 16:11:18.000000 c4m_flexcell-0.3.0/c4m_flexcell.egg-info/requires.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        4 2023-03-08 16:11:18.000000 c4m_flexcell-0.3.0/c4m_flexcell.egg-info/top_level.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        6 2022-11-01 15:19:21.000000 c4m_flexcell-0.3.0/ci-requirements.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       61 2022-09-30 12:33:15.000000 c4m_flexcell-0.3.0/dev-requirements.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2005 2022-04-28 14:40:56.000000 c4m_flexcell-0.3.0/dodo.py
--rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)      165 2021-03-14 14:00:40.000000 c4m_flexcell-0.3.0/run_unittests.sh
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       38 2023-03-08 16:11:18.683272 c4m_flexcell-0.3.0/setup.cfg
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1394 2023-03-08 14:35:03.000000 c4m_flexcell-0.3.0/setup.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:11:18.679273 c4m_flexcell-0.3.0/test/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       84 2021-03-14 14:00:40.000000 c4m_flexcell-0.3.0/test/__init__.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:11:18.679273 c4m_flexcell-0.3.0/test/interactive/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       16 2020-07-14 09:04:04.000000 c4m_flexcell-0.3.0/test/interactive/.gitignore
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2683 2020-10-06 14:32:17.000000 c4m_flexcell-0.3.0/test/interactive/export.ipynb
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:11:18.683272 c4m_flexcell-0.3.0/test/unit/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       84 2021-03-14 14:00:40.000000 c4m_flexcell-0.3.0/test/unit/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2762 2023-03-03 17:44:42.000000 c4m_flexcell-0.3.0/test/unit/test_library.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 14:00:35.914219 c4m_flexcell-0.3.1/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       96 2022-07-12 15:00:24.000000 c4m_flexcell-0.3.1/.gitignore
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1252 2022-11-01 15:19:21.000000 c4m_flexcell-0.3.1/.gitlab-ci.yml
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      484 2020-07-06 13:05:29.000000 c4m_flexcell-0.3.1/COPYRIGHT.md
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      782 2021-03-14 14:00:40.000000 c4m_flexcell-0.3.1/LICENSE.md
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 14:00:35.906219 c4m_flexcell-0.3.1/LICENSES/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    34523 2021-03-14 14:00:40.000000 c4m_flexcell-0.3.1/LICENSES/agpl-3.0.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13419 2020-07-06 09:58:12.000000 c4m_flexcell-0.3.1/LICENSES/cern_ohl_s_v2.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18009 2021-03-14 14:00:40.000000 c4m_flexcell-0.3.1/LICENSES/gpl-2.0.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4141 2023-04-20 14:00:35.914219 c4m_flexcell-0.3.1/PKG-INFO
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3669 2023-04-20 13:56:37.000000 c4m_flexcell-0.3.1/README.md
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 14:00:35.910219 c4m_flexcell-0.3.1/ReleaseNotes/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      321 2021-03-14 14:00:41.000000 c4m_flexcell-0.3.1/ReleaseNotes/v0.0.4.md
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      462 2022-08-22 13:25:11.000000 c4m_flexcell-0.3.1/ReleaseNotes/v0.1.0.md
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 14:00:35.910219 c4m_flexcell-0.3.1/c4m/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      149 2021-03-14 14:00:40.000000 c4m_flexcell-0.3.1/c4m/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2247 2021-05-15 12:46:28.000000 c4m_flexcell-0.3.1/c4m/cell_canvas.ipynb
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 14:00:35.910219 c4m_flexcell-0.3.1/c4m/flexcell/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      107 2023-04-20 14:00:13.000000 c4m_flexcell-0.3.1/c4m/flexcell/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)   622096 2022-12-05 14:11:33.000000 c4m_flexcell-0.3.1/c4m/flexcell/_cells.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)   107025 2023-04-20 14:00:13.000000 c4m_flexcell-0.3.1/c4m/flexcell/factory.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    52730 2023-04-12 09:57:00.000000 c4m_flexcell-0.3.1/c4m/flexcell/stdcell.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 14:00:35.910219 c4m_flexcell-0.3.1/c4m_flexcell.egg-info/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4141 2023-04-20 14:00:35.000000 c4m_flexcell-0.3.1/c4m_flexcell.egg-info/PKG-INFO
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      686 2023-04-20 14:00:35.000000 c4m_flexcell-0.3.1/c4m_flexcell.egg-info/SOURCES.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        1 2023-04-20 14:00:35.000000 c4m_flexcell-0.3.1/c4m_flexcell.egg-info/dependency_links.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       28 2023-04-20 14:00:35.000000 c4m_flexcell-0.3.1/c4m_flexcell.egg-info/requires.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        4 2023-04-20 14:00:35.000000 c4m_flexcell-0.3.1/c4m_flexcell.egg-info/top_level.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        6 2022-11-01 15:19:21.000000 c4m_flexcell-0.3.1/ci-requirements.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       61 2022-09-30 12:33:15.000000 c4m_flexcell-0.3.1/dev-requirements.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2005 2022-04-28 14:40:56.000000 c4m_flexcell-0.3.1/dodo.py
+-rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)      165 2021-03-14 14:00:40.000000 c4m_flexcell-0.3.1/run_unittests.sh
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       38 2023-04-20 14:00:35.914219 c4m_flexcell-0.3.1/setup.cfg
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1394 2023-04-20 13:54:14.000000 c4m_flexcell-0.3.1/setup.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 14:00:35.910219 c4m_flexcell-0.3.1/test/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       84 2021-03-14 14:00:40.000000 c4m_flexcell-0.3.1/test/__init__.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 14:00:35.914219 c4m_flexcell-0.3.1/test/interactive/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       16 2020-07-14 09:04:04.000000 c4m_flexcell-0.3.1/test/interactive/.gitignore
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2683 2020-10-06 14:32:17.000000 c4m_flexcell-0.3.1/test/interactive/export.ipynb
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 14:00:35.914219 c4m_flexcell-0.3.1/test/unit/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       84 2021-03-14 14:00:40.000000 c4m_flexcell-0.3.1/test/unit/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2762 2023-03-03 17:44:42.000000 c4m_flexcell-0.3.1/test/unit/test_library.py
```

### Comparing `c4m_flexcell-0.3.0/.gitlab-ci.yml` & `c4m_flexcell-0.3.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `c4m_flexcell-0.3.0/LICENSE.md` & `c4m_flexcell-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `c4m_flexcell-0.3.0/LICENSES/agpl-3.0.txt` & `c4m_flexcell-0.3.1/LICENSES/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `c4m_flexcell-0.3.0/LICENSES/cern_ohl_s_v2.txt` & `c4m_flexcell-0.3.1/LICENSES/cern_ohl_s_v2.txt`

 * *Files identical despite different names*

### Comparing `c4m_flexcell-0.3.0/LICENSES/gpl-2.0.txt` & `c4m_flexcell-0.3.1/LICENSES/gpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `c4m_flexcell-0.3.0/PKG-INFO` & `c4m_flexcell-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c4m_flexcell
-Version: 0.3.0
+Version: 0.3.1
 Summary: PDKMaster based scalable standard cell library
 Author: Staf Verhaegen
 Author-email: staf@fibraservi.eu
 License: GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+
 Project-URL: Source Code, https://gitlab.com/Chips4Makers/c4m-flexcell
 Project-URL: Bug Tracker, https://gitlab.com/Chips4Makers/c4m-flexcell/issues
 Requires-Python: ~=3.6
@@ -15,14 +15,15 @@
 
 A standard cell library is a collection of cells that perform certain digital functions. It consists of so-called combinatorial cells which perform a binary logic function and sequential cells sync internal signal with a clock signal.
 
 Standard cells are introduced into an [ASIC](https://en.wikipedia.org/wiki/Application-specific_integrated_circuit) [EDA](https://en.wikipedia.org/wiki/Electronic_design_automation) flow during the synthesis step. This is the step where a (RTL) logic design into a netlist consisting only of the cells from your standard cell library. Later on these cells are then placed next to each and the inputs and outputs of each cell connected to each other. The former is called placement and the latter routing.
 
 ## Release History
 
+* v0.3.1: small update for Coriolis export
 * v0.3.0: Update for [release v0.9.0 of PDKMaster](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.9.0/ReleaseNotes/v0.9.0.md); replace Library-> StdCellFactory to follow common usage of a factory to generate cells.
 * v0.2.0: Small updates for changing PDKMaster API
 * [v0.1.0](https://gitlab.com/Chips4Makers/c4m-flexcell/-/blob/v0.1.0/ReleaseNotes/v0.1.0.md)
 * [v0.0.4](https://gitlab.com/Chips4Makers/c4m-flexcell/-/blob/v0.1.0/ReleaseNotes/v0.0.4.md)
 
 ## Rationale
```

### Comparing `c4m_flexcell-0.3.0/README.md` & `c4m_flexcell-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 A standard cell library is a collection of cells that perform certain digital functions. It consists of so-called combinatorial cells which perform a binary logic function and sequential cells sync internal signal with a clock signal.
 
 Standard cells are introduced into an [ASIC](https://en.wikipedia.org/wiki/Application-specific_integrated_circuit) [EDA](https://en.wikipedia.org/wiki/Electronic_design_automation) flow during the synthesis step. This is the step where a (RTL) logic design into a netlist consisting only of the cells from your standard cell library. Later on these cells are then placed next to each and the inputs and outputs of each cell connected to each other. The former is called placement and the latter routing.
 
 ## Release History
 
+* v0.3.1: small update for Coriolis export
 * v0.3.0: Update for [release v0.9.0 of PDKMaster](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.9.0/ReleaseNotes/v0.9.0.md); replace Library-> StdCellFactory to follow common usage of a factory to generate cells.
 * v0.2.0: Small updates for changing PDKMaster API
 * [v0.1.0](https://gitlab.com/Chips4Makers/c4m-flexcell/-/blob/v0.1.0/ReleaseNotes/v0.1.0.md)
 * [v0.0.4](https://gitlab.com/Chips4Makers/c4m-flexcell/-/blob/v0.1.0/ReleaseNotes/v0.0.4.md)
 
 ## Rationale
```

### Comparing `c4m_flexcell-0.3.0/c4m/cell_canvas.ipynb` & `c4m_flexcell-0.3.1/c4m/cell_canvas.ipynb`

 * *Files identical despite different names*

### Comparing `c4m_flexcell-0.3.0/c4m/flexcell/_cells.py` & `c4m_flexcell-0.3.1/c4m/flexcell/_cells.py`

 * *Files identical despite different names*

### Comparing `c4m_flexcell-0.3.0/c4m/flexcell/factory.py` & `c4m_flexcell-0.3.1/c4m/flexcell/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,23 +4,40 @@
 import os
 
 from pdkmaster.typing import OptMultiT, cast_OptMultiT, cast_OptMultiT_n
 from pdkmaster.technology import (
     property_ as _prp, geometry as _geo, primitive as _prm, technology_ as _tch,
 )
 from pdkmaster.design import (
-    circuit as _ckt, layout as _lay, cell as _cell, routinggauge as _rg,
+    circuit as _ckt, layout as _lay, routinggauge as _rg,
     library as _lbry, factory as _fab,
 )
+from pdkmaster.io.coriolis import CoriolisExportSpec
 
 from ._cells import _cells, _oldcells
 from .stdcell import _StdCellConverter
 
 
-__all__ = ["StdCellCanvas", "StdCellFactory"]
+__all__ = ["coriolis_export_spec", "StdCellFactory"]
+
+
+def _direction_cb(net_name: str) -> str:
+    if net_name == "vdd":
+        return "supply"
+    elif net_name == "vss":
+        return "ground"
+    elif net_name == "ck":
+        return "clock"
+    elif net_name in ("nq", "q", "one", "zero"):
+        return "out"
+    else:
+        return "in"
+coriolis_export_spec = CoriolisExportSpec(
+    globalnets=("vdd", "vss"), net_direction_cb=_direction_cb,
+)
 
 
 class StdCellCanvas:
     """The CellCanvas class describes the rules a generated standard cell has to
     fullfil.
 
     Parameters:
@@ -56,15 +73,15 @@
         if nmos not in tech.primitives:
             raise ValueError(
                 f"provided nmos transistor {nmos.name} not of technology '{tech.name}'",
             )
         if nimplant is None:
             nimplant = nmos.implant[0]
         else:
-            if nimplant.type_ != _prm.nImplT:
+            if nimplant.type_ != _prm.nImpl:
                 raise ValueError(
                     f"nimplant '{nimplant.name}' is not n type",
                 )
             if nimplant not in nmos.implant:
                 raise NotImplementedError(
                     f"nimplant '{nimplant.name}' not part of nmos implants"
                 )
@@ -72,15 +89,15 @@
         if pmos not in tech.primitives:
             raise ValueError(
                 f"provided pmos transistor {pmos.name} not of technology '{tech.name}'",
             )
         if pimplant is None:
             pimplant = pmos.implant[0]
         else:
-            if pimplant.type_ != _prm.pImplT:
+            if pimplant.type_ != _prm.pImpl:
                 raise ValueError(
                     f"pimplant '{pimplant.name}' is not p type",
                 )
             if pimplant not in pmos.implant:
                 raise NotImplementedError(
                     f"pimplant '{pimplant.name}' not part of pmos implants"
                 )
```

### Comparing `c4m_flexcell-0.3.0/c4m/flexcell/stdcell.py` & `c4m_flexcell-0.3.1/c4m/flexcell/stdcell.py`

 * *Files identical despite different names*

### Comparing `c4m_flexcell-0.3.0/c4m_flexcell.egg-info/PKG-INFO` & `c4m_flexcell-0.3.1/c4m_flexcell.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c4m-flexcell
-Version: 0.3.0
+Version: 0.3.1
 Summary: PDKMaster based scalable standard cell library
 Author: Staf Verhaegen
 Author-email: staf@fibraservi.eu
 License: GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+
 Project-URL: Source Code, https://gitlab.com/Chips4Makers/c4m-flexcell
 Project-URL: Bug Tracker, https://gitlab.com/Chips4Makers/c4m-flexcell/issues
 Requires-Python: ~=3.6
@@ -15,14 +15,15 @@
 
 A standard cell library is a collection of cells that perform certain digital functions. It consists of so-called combinatorial cells which perform a binary logic function and sequential cells sync internal signal with a clock signal.
 
 Standard cells are introduced into an [ASIC](https://en.wikipedia.org/wiki/Application-specific_integrated_circuit) [EDA](https://en.wikipedia.org/wiki/Electronic_design_automation) flow during the synthesis step. This is the step where a (RTL) logic design into a netlist consisting only of the cells from your standard cell library. Later on these cells are then placed next to each and the inputs and outputs of each cell connected to each other. The former is called placement and the latter routing.
 
 ## Release History
 
+* v0.3.1: small update for Coriolis export
 * v0.3.0: Update for [release v0.9.0 of PDKMaster](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.9.0/ReleaseNotes/v0.9.0.md); replace Library-> StdCellFactory to follow common usage of a factory to generate cells.
 * v0.2.0: Small updates for changing PDKMaster API
 * [v0.1.0](https://gitlab.com/Chips4Makers/c4m-flexcell/-/blob/v0.1.0/ReleaseNotes/v0.1.0.md)
 * [v0.0.4](https://gitlab.com/Chips4Makers/c4m-flexcell/-/blob/v0.1.0/ReleaseNotes/v0.0.4.md)
 
 ## Rationale
```

### Comparing `c4m_flexcell-0.3.0/c4m_flexcell.egg-info/SOURCES.txt` & `c4m_flexcell-0.3.1/c4m_flexcell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `c4m_flexcell-0.3.0/dodo.py` & `c4m_flexcell-0.3.1/dodo.py`

 * *Files identical despite different names*

### Comparing `c4m_flexcell-0.3.0/setup.py` & `c4m_flexcell-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     author_email="staf@fibraservi.eu",
     description="PDKMaster based scalable standard cell library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+",
     python_requires="~=3.6",
     setup_requires=["setuptools_scm"],
-    install_requires=["setuptools", "PDKMaster==0.9.*"],
+    install_requires=["setuptools", "PDKMaster~=0.9.1"],
     include_package_data=True,
     packages=_packages,
     project_urls={
         #"Documentation": "???",
         "Source Code": "https://gitlab.com/Chips4Makers/c4m-flexcell",
         "Bug Tracker": "https://gitlab.com/Chips4Makers/c4m-flexcell/issues",
     },
```

### Comparing `c4m_flexcell-0.3.0/test/interactive/export.ipynb` & `c4m_flexcell-0.3.1/test/interactive/export.ipynb`

 * *Files identical despite different names*

### Comparing `c4m_flexcell-0.3.0/test/unit/test_library.py` & `c4m_flexcell-0.3.1/test/unit/test_library.py`

 * *Files identical despite different names*

