# Comparing `tmp/ccs_fit-0.21.2.tar.gz` & `tmp/ccs_fit-0.21.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccs_fit-0.21.2.tar", max compression
+gzip compressed data, was "ccs_fit-0.21.3.tar", max compression
```

## Comparing `ccs_fit-0.21.2.tar` & `ccs_fit-0.21.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    35149 2023-04-13 09:48:30.530750 ccs_fit-0.21.2/LICENSE
--rw-r--r--   0        0        0     7895 2023-04-13 09:48:30.530750 ccs_fit-0.21.2/README.md
--rw-r--r--   0        0        0     2483 2023-04-13 09:49:11.491304 ccs_fit-0.21.2/pyproject.toml
--rw-r--r--   0        0        0     1027 2023-04-13 09:48:31.494759 ccs_fit-0.21.2/src/ccs_fit/__init__.py
--rw-r--r--   0        0        0     9636 2023-04-13 09:48:31.494759 ccs_fit-0.21.2/src/ccs_fit/ase_calculator/buck.py
--rw-r--r--   0        0        0     7934 2023-04-13 09:48:31.494759 ccs_fit-0.21.2/src/ccs_fit/ase_calculator/ccs_ase_G2B.py
--rw-r--r--   0        0        0    10653 2023-04-13 09:48:31.494759 ccs_fit-0.21.2/src/ccs_fit/ase_calculator/ccs_ase_calculator.py
--rw-r--r--   0        0        0      488 2023-04-13 09:48:31.494759 ccs_fit-0.21.2/src/ccs_fit/common/__init__.py
--rw-r--r--   0        0        0      628 2023-04-13 09:48:31.494759 ccs_fit-0.21.2/src/ccs_fit/common/exceptions.py
--rw-r--r--   0        0        0     1476 2023-04-13 09:48:31.494759 ccs_fit-0.21.2/src/ccs_fit/common/io.py
--rw-r--r--   0        0        0      486 2023-04-13 09:48:31.494759 ccs_fit-0.21.2/src/ccs_fit/common/math/__init__.py
--rw-r--r--   0        0        0     1071 2023-04-13 09:48:31.494759 ccs_fit-0.21.2/src/ccs_fit/common/math/ewald.py
--rw-r--r--   0        0        0     2156 2023-04-13 09:48:31.494759 ccs_fit-0.21.2/src/ccs_fit/common/neighborlist.py
--rw-r--r--   0        0        0      488 2023-04-13 09:48:31.494759 ccs_fit-0.21.2/src/ccs_fit/data/__init__.py
--rw-r--r--   0        0        0      854 2023-04-13 09:48:31.494759 ccs_fit-0.21.2/src/ccs_fit/data/conversion.py
--rw-r--r--   0        0        0      805 2023-04-13 09:48:31.494759 ccs_fit-0.21.2/src/ccs_fit/debugging_tools/timing.py
--rw-r--r--   0        0        0      488 2023-04-13 09:48:31.494759 ccs_fit-0.21.2/src/ccs_fit/fitting/__init__.py
--rw-r--r--   0        0        0    13479 2023-04-13 09:48:31.494759 ccs_fit-0.21.2/src/ccs_fit/fitting/main copy.py
--rw-r--r--   0        0        0    14597 2023-04-13 09:48:31.494759 ccs_fit-0.21.2/src/ccs_fit/fitting/main.py
--rw-r--r--   0        0        0    23883 2023-04-13 09:48:31.494759 ccs_fit-0.21.2/src/ccs_fit/fitting/objective.py
--rw-r--r--   0        0        0    11717 2023-04-13 09:48:31.494759 ccs_fit-0.21.2/src/ccs_fit/fitting/spline_functions.py
--rw-r--r--   0        0        0    20046 2023-04-13 09:48:31.494759 ccs_fit-0.21.2/src/ccs_fit/ppmd_interface/ccs_ppmd.py
--rw-r--r--   0        0        0     6913 2023-04-13 09:48:31.494759 ccs_fit-0.21.2/src/ccs_fit/regression_tool/regression.py
--rw-r--r--   0        0        0      488 2023-04-13 09:48:31.494759 ccs_fit-0.21.2/src/ccs_fit/scripts/__init__.py
--rw-r--r--   0        0        0     7361 2023-04-13 09:48:31.494759 ccs_fit-0.21.2/src/ccs_fit/scripts/ccs_build_db copy.py
--rw-r--r--   0        0        0     7229 2023-04-13 09:48:31.494759 ccs_fit-0.21.2/src/ccs_fit/scripts/ccs_build_db.py
--rw-r--r--   0        0        0     8555 2023-04-13 09:48:31.494759 ccs_fit-0.21.2/src/ccs_fit/scripts/ccs_export_FF.py
--rw-r--r--   0        0        0     4155 2023-04-13 09:48:31.494759 ccs_fit-0.21.2/src/ccs_fit/scripts/ccs_export_sktable.py
--rw-r--r--   0        0        0     8503 2023-04-13 09:48:31.494759 ccs_fit-0.21.2/src/ccs_fit/scripts/ccs_fetch.py
--rw-r--r--   0        0        0     2537 2023-04-13 09:48:31.494759 ccs_fit-0.21.2/src/ccs_fit/scripts/ccs_fit.py
--rw-r--r--   0        0        0     6482 2023-04-13 09:48:31.494759 ccs_fit-0.21.2/src/ccs_fit/scripts/ccs_prune.py
--rw-r--r--   0        0        0     6754 2023-04-13 09:48:31.494759 ccs_fit-0.21.2/src/ccs_fit/scripts/ccs_validate.py
--rw-r--r--   0        0        0     1784 2023-04-13 09:48:31.494759 ccs_fit-0.21.2/src/ccs_fit/scripts/jsonTotable.py
--rw-r--r--   0        0        0     9120 1970-01-01 00:00:00.000000 ccs_fit-0.21.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-20 11:11:06.787547 ccs_fit-0.21.3/LICENSE
+-rw-r--r--   0        0        0     7895 2023-04-20 11:11:06.787547 ccs_fit-0.21.3/README.md
+-rw-r--r--   0        0        0     2483 2023-04-20 11:12:05.735938 ccs_fit-0.21.3/pyproject.toml
+-rw-r--r--   0        0        0     1027 2023-04-20 11:11:07.995555 ccs_fit-0.21.3/src/ccs_fit/__init__.py
+-rw-r--r--   0        0        0     9636 2023-04-20 11:11:07.995555 ccs_fit-0.21.3/src/ccs_fit/ase_calculator/buck.py
+-rw-r--r--   0        0        0     7934 2023-04-20 11:11:07.995555 ccs_fit-0.21.3/src/ccs_fit/ase_calculator/ccs_ase_G2B.py
+-rw-r--r--   0        0        0    10653 2023-04-20 11:11:07.995555 ccs_fit-0.21.3/src/ccs_fit/ase_calculator/ccs_ase_calculator.py
+-rw-r--r--   0        0        0      488 2023-04-20 11:11:07.995555 ccs_fit-0.21.3/src/ccs_fit/common/__init__.py
+-rw-r--r--   0        0        0      628 2023-04-20 11:11:07.995555 ccs_fit-0.21.3/src/ccs_fit/common/exceptions.py
+-rw-r--r--   0        0        0     1476 2023-04-20 11:11:07.995555 ccs_fit-0.21.3/src/ccs_fit/common/io.py
+-rw-r--r--   0        0        0      486 2023-04-20 11:11:07.995555 ccs_fit-0.21.3/src/ccs_fit/common/math/__init__.py
+-rw-r--r--   0        0        0     1071 2023-04-20 11:11:07.995555 ccs_fit-0.21.3/src/ccs_fit/common/math/ewald.py
+-rw-r--r--   0        0        0     2156 2023-04-20 11:11:07.995555 ccs_fit-0.21.3/src/ccs_fit/common/neighborlist.py
+-rw-r--r--   0        0        0      488 2023-04-20 11:11:07.995555 ccs_fit-0.21.3/src/ccs_fit/data/__init__.py
+-rw-r--r--   0        0        0      854 2023-04-20 11:11:07.995555 ccs_fit-0.21.3/src/ccs_fit/data/conversion.py
+-rw-r--r--   0        0        0      805 2023-04-20 11:11:07.995555 ccs_fit-0.21.3/src/ccs_fit/debugging_tools/timing.py
+-rw-r--r--   0        0        0      488 2023-04-20 11:11:07.995555 ccs_fit-0.21.3/src/ccs_fit/fitting/__init__.py
+-rw-r--r--   0        0        0    13479 2023-04-20 11:11:07.995555 ccs_fit-0.21.3/src/ccs_fit/fitting/main copy.py
+-rw-r--r--   0        0        0    14597 2023-04-20 11:11:07.995555 ccs_fit-0.21.3/src/ccs_fit/fitting/main.py
+-rw-r--r--   0        0        0    23883 2023-04-20 11:11:07.995555 ccs_fit-0.21.3/src/ccs_fit/fitting/objective.py
+-rw-r--r--   0        0        0    11717 2023-04-20 11:11:07.999555 ccs_fit-0.21.3/src/ccs_fit/fitting/spline_functions.py
+-rw-r--r--   0        0        0    20046 2023-04-20 11:11:07.999555 ccs_fit-0.21.3/src/ccs_fit/ppmd_interface/ccs_ppmd.py
+-rw-r--r--   0        0        0     6913 2023-04-20 11:11:07.999555 ccs_fit-0.21.3/src/ccs_fit/regression_tool/regression.py
+-rw-r--r--   0        0        0      488 2023-04-20 11:11:07.999555 ccs_fit-0.21.3/src/ccs_fit/scripts/__init__.py
+-rw-r--r--   0        0        0     7361 2023-04-20 11:11:07.999555 ccs_fit-0.21.3/src/ccs_fit/scripts/ccs_build_db copy.py
+-rw-r--r--   0        0        0     7229 2023-04-20 11:11:07.999555 ccs_fit-0.21.3/src/ccs_fit/scripts/ccs_build_db.py
+-rw-r--r--   0        0        0     8555 2023-04-20 11:11:07.999555 ccs_fit-0.21.3/src/ccs_fit/scripts/ccs_export_FF.py
+-rw-r--r--   0        0        0     4155 2023-04-20 11:11:07.999555 ccs_fit-0.21.3/src/ccs_fit/scripts/ccs_export_sktable.py
+-rw-r--r--   0        0        0     8590 2023-04-20 11:11:07.999555 ccs_fit-0.21.3/src/ccs_fit/scripts/ccs_fetch.py
+-rw-r--r--   0        0        0     2537 2023-04-20 11:11:07.999555 ccs_fit-0.21.3/src/ccs_fit/scripts/ccs_fit.py
+-rw-r--r--   0        0        0     6482 2023-04-20 11:11:07.999555 ccs_fit-0.21.3/src/ccs_fit/scripts/ccs_prune.py
+-rw-r--r--   0        0        0     6754 2023-04-20 11:11:07.999555 ccs_fit-0.21.3/src/ccs_fit/scripts/ccs_validate.py
+-rw-r--r--   0        0        0     1784 2023-04-20 11:11:07.999555 ccs_fit-0.21.3/src/ccs_fit/scripts/jsonTotable.py
+-rw-r--r--   0        0        0     9120 1970-01-01 00:00:00.000000 ccs_fit-0.21.3/PKG-INFO
```

### Comparing `ccs_fit-0.21.2/LICENSE` & `ccs_fit-0.21.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.2/README.md` & `ccs_fit-0.21.3/README.md`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.2/pyproject.toml` & `ccs_fit-0.21.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ccs_fit"
-version = "0.21.2"
+version = "0.21.3"
 description = "Fitting tools for repulsive two body interactions using curvature constrained splines."
 authors = [
     "Akshay Krishna AK",
     "Jolla Kullgren <jolla.kullgren@kemi.uu.se>",
     "Eddie Wadbro <eddie.wadbro@umu.se>"
     ]
 maintainers = [
```

### Comparing `ccs_fit-0.21.2/src/ccs_fit/__init__.py` & `ccs_fit-0.21.3/src/ccs_fit/__init__.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.2/src/ccs_fit/ase_calculator/buck.py` & `ccs_fit-0.21.3/src/ccs_fit/ase_calculator/buck.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.2/src/ccs_fit/ase_calculator/ccs_ase_G2B.py` & `ccs_fit-0.21.3/src/ccs_fit/ase_calculator/ccs_ase_G2B.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.2/src/ccs_fit/ase_calculator/ccs_ase_calculator.py` & `ccs_fit-0.21.3/src/ccs_fit/ase_calculator/ccs_ase_calculator.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.2/src/ccs_fit/common/exceptions.py` & `ccs_fit-0.21.3/src/ccs_fit/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.2/src/ccs_fit/common/io.py` & `ccs_fit-0.21.3/src/ccs_fit/common/io.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.2/src/ccs_fit/common/math/ewald.py` & `ccs_fit-0.21.3/src/ccs_fit/common/math/ewald.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.2/src/ccs_fit/common/neighborlist.py` & `ccs_fit-0.21.3/src/ccs_fit/common/neighborlist.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.2/src/ccs_fit/data/conversion.py` & `ccs_fit-0.21.3/src/ccs_fit/data/conversion.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.2/src/ccs_fit/debugging_tools/timing.py` & `ccs_fit-0.21.3/src/ccs_fit/debugging_tools/timing.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.2/src/ccs_fit/fitting/main copy.py` & `ccs_fit-0.21.3/src/ccs_fit/fitting/main copy.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.2/src/ccs_fit/fitting/main.py` & `ccs_fit-0.21.3/src/ccs_fit/fitting/main.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.2/src/ccs_fit/fitting/objective.py` & `ccs_fit-0.21.3/src/ccs_fit/fitting/objective.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.2/src/ccs_fit/fitting/spline_functions.py` & `ccs_fit-0.21.3/src/ccs_fit/fitting/spline_functions.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.2/src/ccs_fit/ppmd_interface/ccs_ppmd.py` & `ccs_fit-0.21.3/src/ccs_fit/ppmd_interface/ccs_ppmd.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.2/src/ccs_fit/regression_tool/regression.py` & `ccs_fit-0.21.3/src/ccs_fit/regression_tool/regression.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.2/src/ccs_fit/scripts/ccs_build_db copy.py` & `ccs_fit-0.21.3/src/ccs_fit/scripts/ccs_build_db copy.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.2/src/ccs_fit/scripts/ccs_build_db.py` & `ccs_fit-0.21.3/src/ccs_fit/scripts/ccs_build_db.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.2/src/ccs_fit/scripts/ccs_export_FF.py` & `ccs_fit-0.21.3/src/ccs_fit/scripts/ccs_export_FF.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.2/src/ccs_fit/scripts/ccs_export_sktable.py` & `ccs_fit-0.21.3/src/ccs_fit/scripts/ccs_export_sktable.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.2/src/ccs_fit/scripts/ccs_fetch.py` & `ccs_fit-0.21.3/src/ccs_fit/scripts/ccs_fetch.py`

 * *Files 5% similar despite different names*

```diff
@@ -145,14 +145,15 @@
                 ce["energy_dftb"] = EREF
             dict_species = defaultdict(int)
             struct.charges = []
             for elem in struct.get_chemical_symbols():
                 dict_species[elem] += 1
                 if mode == "CCS+Q":
                     struct.charges.append(charge_dict[elem])
+            dict_species = {key: value for key, value in sorted(dict_species.items())}
             atom_pair = it.combinations_with_replacement(
                 dict_species.keys(), 2)
             if mode == "CCS+Q":
                 lattice = Lattice(struct.get_cell())
                 coords = struct.get_scaled_positions()
                 ew_struct = Structure(
                     lattice,
```

### Comparing `ccs_fit-0.21.2/src/ccs_fit/scripts/ccs_fit.py` & `ccs_fit-0.21.3/src/ccs_fit/scripts/ccs_fit.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.2/src/ccs_fit/scripts/ccs_prune.py` & `ccs_fit-0.21.3/src/ccs_fit/scripts/ccs_prune.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.2/src/ccs_fit/scripts/ccs_validate.py` & `ccs_fit-0.21.3/src/ccs_fit/scripts/ccs_validate.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.2/src/ccs_fit/scripts/jsonTotable.py` & `ccs_fit-0.21.3/src/ccs_fit/scripts/jsonTotable.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.2/PKG-INFO` & `ccs_fit-0.21.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccs-fit
-Version: 0.21.2
+Version: 0.21.3
 Summary: Fitting tools for repulsive two body interactions using curvature constrained splines.
 Home-page: https://github.com/Teoroo-CMC/CCS
 License: GPL-3
 Keywords: Curvature,Constrained,Splines,Two-Body,Interatomic,Repulsive,Fitting
 Author: Akshay Krishna AK
 Maintainer: Jolla Kullgren
 Maintainer-email: jolla.kullgren@kemi.uu.se
```

