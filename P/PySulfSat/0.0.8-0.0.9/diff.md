# Comparing `tmp/PySulfSat-0.0.8.tar.gz` & `tmp/PySulfSat-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySulfSat-0.0.8.tar", last modified: Tue Jan 17 19:53:33 2023, max compression
+gzip compressed data, was "PySulfSat-0.0.9.tar", last modified: Fri Jan 20 19:50:14 2023, max compression
```

## Comparing `PySulfSat-0.0.8.tar` & `PySulfSat-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 19:53:33.335717 PySulfSat-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-01-17 19:53:33.335717 PySulfSat-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-01-17 19:53:23.000000 PySulfSat-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-01-17 19:53:33.335717 PySulfSat-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-01-17 19:53:23.000000 PySulfSat-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 19:53:33.331717 PySulfSat-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 19:53:33.335717 PySulfSat-0.0.8/src/PySulfSat/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-01-17 19:53:23.000000 PySulfSat-0.0.8/src/PySulfSat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-01-17 19:53:23.000000 PySulfSat-0.0.8/src/PySulfSat/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    32253 2023-01-17 19:53:23.000000 PySulfSat-0.0.8/src/PySulfSat/core_calcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-01-17 19:53:23.000000 PySulfSat-0.0.8/src/PySulfSat/import_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-01-17 19:53:23.000000 PySulfSat-0.0.8/src/PySulfSat/mantle_melting.py
--rw-r--r--   0 runner    (1001) docker     (123)    16472 2023-01-17 19:53:23.000000 PySulfSat-0.0.8/src/PySulfSat/s6_corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-01-17 19:53:23.000000 PySulfSat-0.0.8/src/PySulfSat/scas_calc.py
--rw-r--r--   0 runner    (1001) docker     (123)    65506 2023-01-17 19:53:23.000000 PySulfSat-0.0.8/src/PySulfSat/scss_calcs2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-01-17 19:53:23.000000 PySulfSat-0.0.8/src/PySulfSat/sulf_mass_balance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 19:53:33.335717 PySulfSat-0.0.8/src/PySulfSat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-01-17 19:53:33.000000 PySulfSat-0.0.8/src/PySulfSat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-01-17 19:53:33.000000 PySulfSat-0.0.8/src/PySulfSat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 19:53:33.000000 PySulfSat-0.0.8/src/PySulfSat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-17 19:53:33.000000 PySulfSat-0.0.8/src/PySulfSat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-17 19:53:33.000000 PySulfSat-0.0.8/src/PySulfSat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 19:50:14.565988 PySulfSat-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-01-20 19:50:14.565988 PySulfSat-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-01-20 19:50:14.569989 PySulfSat-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 19:50:14.565988 PySulfSat-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 19:50:14.565988 PySulfSat-0.0.9/src/PySulfSat/
+-rw-r--r--   0 runner    (1001) docker     (123)    16520 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/Cali_BW2022.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    87168 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/Cali_Blanchard2021.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    35617 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/Cali_ChowDas22.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    45229 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/Cali_Fortin2015.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    27276 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/Cali_LiZhang22.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/Cali_Liu2021.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    19872 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/Cali_MK2015.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    41651 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/Cali_OM2022.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    75124 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/Cali_Smythe17.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    36905 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/Cali_ZT2019.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    71594 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/Smythe17.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/cali_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38417 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/core_calcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/import_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/mantle_melting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16472 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/s6_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7346 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/scas_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65506 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/scss_calcs2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/sulf_mass_balance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 19:50:14.565988 PySulfSat-0.0.9/src/PySulfSat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-01-20 19:50:14.000000 PySulfSat-0.0.9/src/PySulfSat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-01-20 19:50:14.000000 PySulfSat-0.0.9/src/PySulfSat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 19:50:14.000000 PySulfSat-0.0.9/src/PySulfSat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-20 19:50:14.000000 PySulfSat-0.0.9/src/PySulfSat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-20 19:50:14.000000 PySulfSat-0.0.9/src/PySulfSat.egg-info/top_level.txt
```

### Comparing `PySulfSat-0.0.8/PKG-INFO` & `PySulfSat-0.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySulfSat
-Version: 0.0.8
+Version: 0.0.9
 Summary: PySulfSat
 Home-page: https://github.com/PennyWieser/PySulfSat
 Author: Penny Wieser
 Author-email: penny.wieser@gmail.com
 License: UNKNOWN
 Description: [![PyPI](https://badgen.net/pypi/v/PySulfSat)](https://pypi.org/project/PySulfSat/)
         [![Build Status](https://github.com/PennyWieser/PySulfSat/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/PennyWieser/PySulfSat/actions/workflows/main.yml)
```

### Comparing `PySulfSat-0.0.8/README.md` & `PySulfSat-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `PySulfSat-0.0.8/setup.py` & `PySulfSat-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `PySulfSat-0.0.8/src/PySulfSat/__init__.py` & `PySulfSat-0.0.9/src/PySulfSat/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from PySulfSat.import_data import *
 # This has the actual SCSS calculations
 from PySulfSat.scss_calcs2 import *
 # This has stuff for performing s6+ corrections
 from PySulfSat.s6_corrections import *
 from PySulfSat.scas_calc import *
 from PySulfSat.sulf_mass_balance import *
-
+from PySulfSat.cali_plots import *
 from PySulfSat.mantle_melting import *
 
 
 # version
 from ._version import __version__
```

### Comparing `PySulfSat-0.0.8/src/PySulfSat/core_calcs.py` & `PySulfSat-0.0.9/src/PySulfSat/core_calcs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import scipy
 import scipy.optimize as optimize
 from scipy.special import erf
+from pathlib import Path
+from pickle import load
+import pickle
+PySulfSat_dir=Path(__file__).parent
 
 
 
 
 
 ## Anhydrous Molar masses, used for ONeill (2021). Doesnt include P2O5, Cr2O3 or H2O in the calculation.
 oxide_mass_liq_anhyd = {'SiO2_Liq': 60.0843, 'MgO_Liq': 40.3044,
@@ -61,14 +65,16 @@
 #
 cation_num_liq_hyd_df = pd.DataFrame.from_dict(
     cation_num_liq_hyd, orient='index').T
 cation_num_liq_hyd_df['Sample_ID_Liq'] = 'CatNum'
 cation_num_liq_hyd_df.set_index('Sample_ID_Liq', inplace=True)
 
 
+## With
+
 
 
 
 ## Anhydrous proportions, fractions, calculations from Thermobar (Wieser et al. in prep)
 
 
 def calculate_anhydrous_mol_proportions_liquid(liq_comps):
@@ -542,14 +548,15 @@
     a_drop['sum'] = a_drop.sum(axis='columns')
     Final_Calc_step = a_drop.div(a_drop['sum'], axis='rows')
     Final_Calc_step.drop(['sum'], axis='columns', inplace=True)
 
 
     return Final_Calc_step
 
+
 ## Redox calculations
 def convert_fo2_to_fe_partition(*, liq_comps, T_K, P_kbar,
                                 model="Kress1991", fo2, renorm=False, fo2_offset=0):
     '''
     Calculates Fe3Fet_Liq, FeO and Fe2O3 based on user-specified buffer
 
    Parameters
@@ -674,14 +681,27 @@
   'H2O_Liq': 18.01528}
 # Turns dictionary into a dataframe so pandas matrix math functions can be used
 oxide_mass_liq_hyd_df_redox = pd.DataFrame.from_dict(
     oxide_mass_liq_hyd_redox, orient='index').T
 oxide_mass_liq_hyd_df_redox['Sample_ID_Liq'] = 'MolWt'
 oxide_mass_liq_hyd_df_redox.set_index('Sample_ID_Liq', inplace=True)
 
+
+cation_num_liq_hyd_redox = {'SiO2_Liq': 1, 'MgO_Liq': 1, 'MnO_Liq': 1,
+'FeO_Liq': 1, 'Fe2O3_Liq': 2, 'CaO_Liq': 1, 'Al2O3_Liq': 2, 'Na2O_Liq': 2,
+'K2O_Liq': 2, 'TiO2_Liq': 1, 'P2O5_Liq': 2, 'H2O_Liq':2,
+'Cr2O3_Liq':2}
+
+cation_num_liq_hyd_df_redox = pd.DataFrame.from_dict(
+    cation_num_liq_hyd_redox, orient='index').T
+cation_num_liq_hyd_df_redox['Sample_ID_Liq'] = 'CatNum'
+cation_num_liq_hyd_df_redox.set_index('Sample_ID_Liq', inplace=True)
+
+
+
 def calculate_hydrous_mol_proportions_liquid_redox(liq_comps):
     '''Import Liq compositions using liq_comps=My_Liquids, returns anhydrous mole proportions
 
    Parameters
     -------
 
 
@@ -726,14 +746,107 @@
     mol_prop['sum'] = mol_prop.sum(axis='columns')
     mol_frac_hyd = mol_prop.div(mol_prop['sum'], axis='rows')
     mol_frac_hyd.drop(['sum'], axis='columns', inplace=True)
     mol_frac_hyd.columns = [str(col).replace('prop', 'frac')
                             for col in mol_frac_hyd.columns]
     return mol_frac_hyd
 
+## Fractions with redox
+
+oxide_mass_liq_hyd_redox = {'SiO2_Liq': 60.0843, 'MgO_Liq': 40.3044,
+'MnO_Liq': 70.9375, 'FeO_Liq': 71.8464, 'Fe2O3_Liq': 159.69, 'CaO_Liq': 56.0774,
+'Al2O3_Liq': 101.961, 'Na2O_Liq': 61.9789, 'K2O_Liq': 94.196,
+'TiO2_Liq': 79.8788, 'P2O5_Liq': 141.944, 'H2O_Liq': 18.02 }
+
+oxide_mass_liq_hyd_redox_df = pd.DataFrame.from_dict(
+    oxide_mass_liq_hyd_redox, orient='index').T
+oxide_mass_liq_hyd_redox_df['Sample_ID_Liq'] = 'MolWt'
+oxide_mass_liq_hyd_redox_df.set_index('Sample_ID_Liq', inplace=True)
+
+
+def calculate_hydrous_cat_proportions_liquid_redox(liq_comps):
+    '''Import Liq compositions using liq_comps=My_Liquids, returns hydrous cation proportions (e.g., mole proportions * no of cations)
+
+   Parameters
+    -------
+
+    liq_comps: pandas.DataFrame
+                Panda DataFrame of liquid compositions with column headings SiO2_Liq, TiO2_Liq etc.
+
+
+    Returns
+    -------
+    pandas DataFrame
+        hydrous cation proportions for the liquid with column headings of the form S_Liq_cat_prop
+
+    '''
+
+    mol_prop_no_cat_num = calculate_hydrous_mol_proportions_liquid_redox(liq_comps)
+    mol_prop_no_cat_num.columns = [str(col).replace(
+        '_mol_prop', '') for col in mol_prop_no_cat_num.columns]
+    ox_num_reindex = cation_num_liq_hyd_df_redox.reindex(
+        oxide_mass_liq_hyd_redox_df.columns, axis=1).fillna(0)
+    df_calc_comb = pd.concat([ox_num_reindex, mol_prop_no_cat_num])
+    cation_prop_hyd = df_calc_comb.multiply(
+        df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
+    cation_prop_hyd.columns = [
+        str(col) + '_cat_prop' for col in cation_prop_hyd.columns]
+
+
+
+    return cation_prop_hyd
+
+def calculate_hydrous_cat_fractions_liquid_redox(liq_comps):
+    '''Import Liq compositions using liq_comps=My_Liquids, returns hydrous cation fractions
+
+   Parameters
+    -------
+
+    liq_comps: pandas.DataFrame
+        liquid compositions with column headings SiO2_Liq, TiO2_Liq etc.
+
+
+    Returns
+    -------
+    pandas DataFrame
+        hydrous cation fractions for the liquid with column headings of the form _Liq_cat_frac,
+        as well as the initial dataframe of liquid compositions.
+
+
+    '''
+    cat_prop = calculate_hydrous_cat_proportions_liquid_redox(liq_comps=liq_comps)
+    mol_prop = calculate_hydrous_mol_fractions_liquid_redox(liq_comps=liq_comps)
+
+    cat_prop['sum'] = cat_prop.sum(axis='columns')
+    cat_frac_hyd = cat_prop.div(cat_prop['sum'], axis='rows')
+    cat_frac_hyd.drop(['sum'], axis='columns', inplace=True)
+    cat_frac_hyd.columns = [str(col).replace('prop', 'frac')
+                              for col in cat_frac_hyd.columns]
+    cat_frac_hyd = pd.concat([liq_comps, mol_prop, cat_frac_hyd], axis=1)
+
+
+
+    cation_frac_hyd2=cat_frac_hyd.rename(columns={
+                        'SiO2_Liq_cat_frac': 'Si_Liq_cat_frac',
+                        'TiO2_Liq_cat_frac': 'Ti_Liq_cat_frac',
+                        'Al2O3_Liq_cat_frac': 'Al_Liq_cat_frac',
+                        'FeO_Liq_cat_frac': 'Fe2_Liq_cat_frac',
+                        'Fe2O3_Liq_cat_frac': 'Fe3_Liq_cat_frac',
+                        'MnO_Liq_cat_frac': 'Mn_Liq_cat_frac',
+                        'MgO_Liq_cat_frac': 'Mg_Liq_cat_frac',
+                        'CaO_Liq_cat_frac': 'Ca_Liq_cat_frac',
+                        'Na2O_Liq_cat_frac': 'Na_Liq_cat_frac',
+                        'K2O_Liq_cat_frac': 'K_Liq_cat_frac',
+                        'Cr2O3_Liq_cat_frac': 'Cr_Liq_cat_frac',
+                        'P2O5_Liq_cat_frac': 'P_Liq_cat_frac',
+
+                        })
+
+    return cation_frac_hyd2
+
 
 
 def convert_fe_partition_to_fo2(*, liq_comps, T_K, P_kbar,  model="Kress1991", renorm=False):
     '''
     Calculates delta fo2 relative to QFM and NNO buffer for liq compositions with FeO and Fe2O3
 
    Parameters
@@ -808,8 +921,77 @@
     DeltaQFM=log_fo2_calc-logfo2_QFM
     DeltaNNO=log_fo2_calc-logfo2_NNO
 
 
     liq_comps_c.insert(0, 'DeltaQFM', DeltaQFM)
     liq_comps_c.insert(1, 'DeltaNNO', DeltaNNO)
     liq_comps_c.insert(2, 'fo2_calc', fo2_calc)
-    return liq_comps_c
+    return liq_comps_c
+
+
+    ## Converting between S, SO2, SO3 etc.
+mol_mass_S=32.065
+mol_mass_O=15.999
+mol_mass_SO3=mol_mass_S+mol_mass_O*3
+mol_mass_SO4=mol_mass_S+mol_mass_O*4
+mol_mass_SO2=mol_mass_S+mol_mass_O*2
+
+def convert_S_types(SO3_wt=None, SO3_ppm=None, S_wt=None, S_ppm=None, SO2_wt=None, SO2_ppm=None,
+ SO4_wt=None, SO4_ppm=None):
+    """ converts SO3 in wt% into S in ppm
+    """
+    params = {
+        "a": SO3_wt,
+        "ab": SO3_ppm,
+        "b": S_wt,
+        "c": S_ppm,
+        "d": SO2_wt,
+        "de": SO2_ppm,
+        "e": SO4_wt,
+        "f": SO4_ppm
+    }
+
+    not_none_params = {k:v for k, v in params.items() if v is not None}
+    if len(not_none_params)>1:
+        raise TypeError('Please only enter one input type, the function returns a dataframe of all the other outputs')
+
+    else:
+        if S_ppm is not None:
+            moles_s=(S_ppm/10**4)/mol_mass_S
+        if S_wt is not None:
+            moles_s=S_wt/mol_mass_S
+        if SO3_wt is not None:
+            moles_s=SO3_wt/mol_mass_SO3
+        if SO3_ppm is not None:
+            moles_s=(SO3_ppm/10**4)/mol_mass_SO3
+
+        if SO4_wt is not None:
+            moles_s=SO4_wt/mol_mass_SO4
+        if SO4_ppm is not None:
+            moles_s=(SO4_ppm/10**4)/mol_mass_SO4
+
+        if SO2_wt is not None:
+            moles_s=SO2_wt/mol_mass_SO2
+        if SO2_ppm is not None:
+            moles_s=(SO2_ppm/10**4)/mol_mass_SO2
+
+        S_wt2= moles_s*mol_mass_S
+        S_ppm2=S_wt2*10**4
+        SO2=moles_s*mol_mass_SO2
+        SO3=moles_s*mol_mass_SO3
+        SO4=moles_s*mol_mass_SO4
+
+
+        df=pd.DataFrame(data={
+                                'S_wt': S_wt2,
+                                'S_ppm': S_ppm2,
+                                'SO2_wt': SO2,
+                                'SO2_ppm': SO2*10**4,
+                                'SO3_wt': SO3,
+                                'SO3_ppm': SO3*10**4,
+                                'SO4_wt': SO4,
+                                'SO4_ppm': SO4*10**4})
+
+
+
+        return df
+
```

### Comparing `PySulfSat-0.0.8/src/PySulfSat/import_data.py` & `PySulfSat-0.0.9/src/PySulfSat/import_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,14 +84,17 @@
 
     my_input_c = my_input.copy()
 
     if "Sample_ID_Liq" not in my_input_c:
         my_input_c['Sample_ID_Liq'] = my_input.index
 
     if suffix is not None:
+        if any(my_input.columns.str.contains("FeOT")) and (all(my_input.columns.str.contains("FeOt")==False)):
+            raise ValueError("No FeOt column found. You've got a column heading with FeOT. Change to a lower case t")
+
         my_input_c=my_input_c.add_suffix(suffix)
 
     if any(my_input.columns.str.contains("FeO_")) and (all(my_input.columns.str.contains("FeOt_")==False)):
         raise ValueError("No FeOt found. You've got a column heading with FeO. To avoid errors based on common EPMA outputs"
     " thermobar only recognises columns with FeOt for all phases except liquid"
     " where you can also enter a Fe3Fet_Liq heading used for equilibrium tests")
 
@@ -107,15 +110,15 @@
 
     myLiquids1 = my_input_c.reindex(df_ideal_liq.columns, axis=1).fillna(0)
     myLiquids1 = myLiquids1.apply(pd.to_numeric, errors='coerce').fillna(0)
     myLiquids1[myLiquids1 < 0] = 0
     print('We have replaced all missing liquid oxides and strings with zeros. ')
 
     cols2=myLiquids1.columns
-    my_input_c=my_input.copy()
+    #my_input_c=my_input.copy()
     for col in cols2:
         if col in my_input_c.columns:
             my_input_c=my_input_c.drop(columns=col)
 
     out=pd.concat([myLiquids1, my_input_c], axis=1)
     return out
```

### Comparing `PySulfSat-0.0.8/src/PySulfSat/mantle_melting.py` & `PySulfSat-0.0.9/src/PySulfSat/mantle_melting.py`

 * *Files identical despite different names*

### Comparing `PySulfSat-0.0.8/src/PySulfSat/s6_corrections.py` & `PySulfSat-0.0.9/src/PySulfSat/s6_corrections.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,15 +257,15 @@
     df_Species2=df_Species.copy()
     df_Species2.drop(['SCAS_Tot_check', 'SCSS_Tot_check', 'SCSS_Tot_check'], axis=1, inplace=True)
     return df_Species2
 
 
 def calculate_BW2022_CS6(*, df, T_K):
     """ Calculates logCs6 and Cs6 using the expression of
-    Boulanger and Wood, 2022. Also converts into the same form as ONeill and Mavrogenes
+    Boulliung and Wood, 2022. Also converts into the same form as ONeill and Mavrogenes
 
     Parameters
     -----------
     df: pandas Dataframe
         input dataframe of liquid compositions with _Liq after each oxide
```

### Comparing `PySulfSat-0.0.8/src/PySulfSat/scas_calc.py` & `PySulfSat-0.0.9/src/PySulfSat/scas_calc.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,17 +153,17 @@
 
     df_c.insert(0, 'Calc SCAS (ppm)', Smelt)
 
     return df_c
 
 
 ## Masotta et al. (2013) calculations
-def calculate_Masotta2014_SCAS(liq_comps, T_K):
-    """ Calculates S6+ dissolved in the melt using Masotta et al. 2014,
-    doi: http://dx.doi.org/10.1016/j.gca.2015.02.0330
+def calculate_MK2015_SCAS(liq_comps, T_K):
+    """ Calculates S6+ dissolved in the melt using Masotta and Kepler (2015)
+    doi: https://doi.org/10.1016/j.gca.2015.02.033
 
     Parameters
     -------
 
     liq_comps: pandas.DataFrame
                 Panda DataFrame of liquid compositions with column headings SiO2_Liq, TiO2_Liq etc.
```

### Comparing `PySulfSat-0.0.8/src/PySulfSat/scss_calcs2.py` & `PySulfSat-0.0.9/src/PySulfSat/scss_calcs2.py`

 * *Files identical despite different names*

### Comparing `PySulfSat-0.0.8/src/PySulfSat/sulf_mass_balance.py` & `PySulfSat-0.0.9/src/PySulfSat/sulf_mass_balance.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 
 
-st_ratio=1/22.6436 #4.4163750000000000000E-02
- #1/22.220
+st_ratio=1/22.6436 # From https://doi.org/10.1016/S0016-7037(01)00611-1
 
-def convert_d34_to_3432S(d34S=None):
+
+def convert_d34_to_3432S(d34S, st_ratio=1/22.6436):
+    """ Converts d34S to 3432S using a st ratio (34/32S value)
+    """
     S3432=((d34S/1000)+1)*(st_ratio)
     return S3432
 
-def convert_3432S_to_d34(S3432=None):
+def convert_3432S_to_d34(S3432, st_ratio=1/22.6436):
+    """ Converts d34S to 3432S using a st ratio (34/32S value)
+    """
     d34S=(((S3432)/(st_ratio)) -1)*1000
     return d34S
 
+def calculate_std_ratio_used(d34S, S3432=1/22.6436):
+    """ When you have both a d34S value and a S3432 value,
+    calculates what ratio was used by the study
+    """
+    S3432_standard=(1000*S3432)/(d34S+1000)
+
+    return S3432_standard
+
 
 def crystallize_S_incomp(S_init=1200, F_melt=None):
     """
     Calculates amount of S remaining in the melt for different melt fractoins (F_melt)
     assuming S is completely incompatible in silicate minerals
```

### Comparing `PySulfSat-0.0.8/src/PySulfSat.egg-info/PKG-INFO` & `PySulfSat-0.0.9/src/PySulfSat.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySulfSat
-Version: 0.0.8
+Version: 0.0.9
 Summary: PySulfSat
 Home-page: https://github.com/PennyWieser/PySulfSat
 Author: Penny Wieser
 Author-email: penny.wieser@gmail.com
 License: UNKNOWN
 Description: [![PyPI](https://badgen.net/pypi/v/PySulfSat)](https://pypi.org/project/PySulfSat/)
         [![Build Status](https://github.com/PennyWieser/PySulfSat/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/PennyWieser/PySulfSat/actions/workflows/main.yml)
```

