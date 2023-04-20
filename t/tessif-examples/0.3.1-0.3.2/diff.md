# Comparing `tmp/tessif-examples-0.3.1.tar.gz` & `tmp/tessif-examples-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tessif-examples-0.3.1.tar", max compression
+gzip compressed data, was "tessif-examples-0.3.2.tar", max compression
```

## Comparing `tessif-examples-0.3.1.tar` & `tessif-examples-0.3.2.tar`

### file list

```diff
@@ -1,36 +1,40 @@
--rw-r--r--   0        0        0     1062 2023-02-28 13:57:44.256487 tessif-examples-0.3.1/LICENSE
--rw-r--r--   0        0        0     5611 2023-02-28 13:57:44.256487 tessif-examples-0.3.1/README.rst
--rw-r--r--   0        0        0     1533 2023-02-28 13:57:44.272487 tessif-examples-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      129 2023-02-28 13:57:44.272487 tessif-examples-0.3.1/src/tessif_examples/__init__.py
--rw-r--r--   0        0        0      754 2023-02-28 13:57:44.272487 tessif-examples-0.3.1/src/tessif_examples/basic/__init__.py
--rw-r--r--   0        0        0     3667 2023-02-28 13:57:44.272487 tessif-examples-0.3.1/src/tessif_examples/basic/chp.py
--rw-r--r--   0        0        0     2566 2023-02-28 13:57:44.272487 tessif-examples-0.3.1/src/tessif_examples/basic/connected_es.py
--rw-r--r--   0        0        0     4086 2023-02-28 13:57:44.272487 tessif-examples-0.3.1/src/tessif_examples/basic/emission_objective.py
--rw-r--r--   0        0        0     3698 2023-02-28 13:57:44.272487 tessif-examples-0.3.1/src/tessif_examples/basic/expansion_plan_example.py
--rw-r--r--   0        0        0     9276 2023-02-28 13:57:44.272487 tessif-examples-0.3.1/src/tessif_examples/basic/fpwe.py
--rw-r--r--   0        0        0     3180 2023-02-28 13:57:44.272487 tessif-examples-0.3.1/src/tessif_examples/basic/mwe.py
--rw-r--r--   0        0        0     6198 2023-02-28 13:57:44.272487 tessif-examples-0.3.1/src/tessif_examples/basic/simple_transformer_grid_es.py
--rw-r--r--   0        0        0     3324 2023-02-28 13:57:44.272487 tessif-examples-0.3.1/src/tessif_examples/basic/storage_example.py
--rw-r--r--   0        0        0     3401 2023-02-28 13:57:44.272487 tessif-examples-0.3.1/src/tessif_examples/basic/storage_fixed_ratio_expansion_example.py
--rw-r--r--   0        0        0     2674 2023-02-28 13:57:44.272487 tessif-examples-0.3.1/src/tessif_examples/basic/time_varying_efficiency_transformer.py
--rw-r--r--   0        0        0     3692 2023-02-28 13:57:44.272487 tessif-examples-0.3.1/src/tessif_examples/basic/zero_costs_es.py
--rw-r--r--   0        0        0      358 2023-02-28 13:57:44.272487 tessif-examples-0.3.1/src/tessif_examples/data/load_profiles/Car_Charging.csv
--rw-r--r--   0        0        0     1273 2023-02-28 13:57:44.272487 tessif-examples-0.3.1/src/tessif_examples/data/load_profiles/Loads.csv
--rw-r--r--   0        0        0      991 2023-02-28 13:57:44.272487 tessif-examples-0.3.1/src/tessif_examples/data/load_profiles/Renewable_Energy.csv
--rw-r--r--   0        0        0   667691 2023-02-28 13:57:44.276487 tessif-examples-0.3.1/src/tessif_examples/data/load_profiles/component_scenario_profiles.csv
--rw-r--r--   0        0        0   475533 2023-02-28 13:57:44.276487 tessif-examples-0.3.1/src/tessif_examples/data/load_profiles/el_demand_HH_2019.csv
--rw-r--r--   0        0        0   138415 2023-02-28 13:57:44.280487 tessif-examples-0.3.1/src/tessif_examples/data/load_profiles/solar_HH_2019.csv
--rw-r--r--   0        0        0   408648 2023-02-28 13:57:44.280487 tessif-examples-0.3.1/src/tessif_examples/data/load_profiles/th_demand_HH_2019.csv
--rw-r--r--   0        0        0   200160 2023-02-28 13:57:44.280487 tessif-examples-0.3.1/src/tessif_examples/data/load_profiles/wind_HH_2019.csv
--rw-r--r--   0        0        0      371 2023-02-28 13:57:44.280487 tessif-examples-0.3.1/src/tessif_examples/paths.py
--rw-r--r--   0        0        0      336 2023-02-28 13:57:44.280487 tessif-examples-0.3.1/src/tessif_examples/scientific/__init__.py
--rw-r--r--   0        0        0    27706 2023-02-28 13:57:44.280487 tessif-examples-0.3.1/src/tessif_examples/scientific/component_focused.py
--rw-r--r--   0        0        0    45190 2023-02-28 13:57:44.280487 tessif-examples-0.3.1/src/tessif_examples/scientific/grid_focused.py
--rw-r--r--   0        0        0    26247 2023-02-28 13:57:44.280487 tessif-examples-0.3.1/src/tessif_examples/scientific/hamburg_inspired.py
--rw-r--r--   0        0        0      280 2023-02-28 13:57:44.280487 tessif-examples-0.3.1/src/tessif_examples/specialized/__init__.py
--rw-r--r--   0        0        0    34235 2023-02-28 13:57:44.280487 tessif-examples-0.3.1/src/tessif_examples/specialized/generic_grid.py
--rw-r--r--   0        0        0    10476 2023-02-28 13:57:44.284487 tessif-examples-0.3.1/src/tessif_examples/specialized/self_similar_system_model.py
--rw-r--r--   0        0        0     4758 2023-02-28 13:57:44.284487 tessif-examples-0.3.1/src/tessif_examples/specialized/variable_chp.py
--rw-r--r--   0        0        0     2455 2023-02-28 13:57:44.284487 tessif-examples-0.3.1/src/tessif_examples/utils.py
--rw-r--r--   0        0        0     6646 1970-01-01 00:00:00.000000 tessif-examples-0.3.1/setup.py
--rw-r--r--   0        0        0     6320 1970-01-01 00:00:00.000000 tessif-examples-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-20 14:38:40.229343 tessif-examples-0.3.2/LICENSE
+-rw-r--r--   0        0        0     5611 2023-04-20 14:38:40.229343 tessif-examples-0.3.2/README.rst
+-rw-r--r--   0        0        0     1533 2023-04-20 14:38:40.245343 tessif-examples-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      129 2023-04-20 14:38:40.245343 tessif-examples-0.3.2/src/tessif_examples/__init__.py
+-rw-r--r--   0        0        0      853 2023-04-20 14:38:40.245343 tessif-examples-0.3.2/src/tessif_examples/basic/__init__.py
+-rw-r--r--   0        0        0     3667 2023-04-20 14:38:40.245343 tessif-examples-0.3.2/src/tessif_examples/basic/chp.py
+-rw-r--r--   0        0        0     2566 2023-04-20 14:38:40.245343 tessif-examples-0.3.2/src/tessif_examples/basic/connected_es.py
+-rw-r--r--   0        0        0     4086 2023-04-20 14:38:40.245343 tessif-examples-0.3.2/src/tessif_examples/basic/emission_objective.py
+-rw-r--r--   0        0        0     3698 2023-04-20 14:38:40.245343 tessif-examples-0.3.2/src/tessif_examples/basic/expansion_plan_example.py
+-rw-r--r--   0        0        0     9276 2023-04-20 14:38:40.245343 tessif-examples-0.3.2/src/tessif_examples/basic/fpwe.py
+-rw-r--r--   0        0        0     3180 2023-04-20 14:38:40.245343 tessif-examples-0.3.2/src/tessif_examples/basic/mwe.py
+-rw-r--r--   0        0        0     6198 2023-04-20 14:38:40.245343 tessif-examples-0.3.2/src/tessif_examples/basic/simple_transformer_grid_es.py
+-rw-r--r--   0        0        0     6059 2023-04-20 14:38:40.245343 tessif-examples-0.3.2/src/tessif_examples/basic/statistical_identification_example.py
+-rw-r--r--   0        0        0     3324 2023-04-20 14:38:40.245343 tessif-examples-0.3.2/src/tessif_examples/basic/storage_example.py
+-rw-r--r--   0        0        0     3401 2023-04-20 14:38:40.245343 tessif-examples-0.3.2/src/tessif_examples/basic/storage_fixed_ratio_expansion_example.py
+-rw-r--r--   0        0        0     2674 2023-04-20 14:38:40.245343 tessif-examples-0.3.2/src/tessif_examples/basic/time_varying_efficiency_transformer.py
+-rw-r--r--   0        0        0     3692 2023-04-20 14:38:40.245343 tessif-examples-0.3.2/src/tessif_examples/basic/zero_costs_es.py
+-rw-r--r--   0        0        0      358 2023-04-20 14:38:40.245343 tessif-examples-0.3.2/src/tessif_examples/data/load_profiles/Car_Charging.csv
+-rw-r--r--   0        0        0     1273 2023-04-20 14:38:40.245343 tessif-examples-0.3.2/src/tessif_examples/data/load_profiles/Loads.csv
+-rw-r--r--   0        0        0      991 2023-04-20 14:38:40.245343 tessif-examples-0.3.2/src/tessif_examples/data/load_profiles/Renewable_Energy.csv
+-rw-r--r--   0        0        0   667691 2023-04-20 14:38:40.249343 tessif-examples-0.3.2/src/tessif_examples/data/load_profiles/component_scenario_profiles.csv
+-rw-r--r--   0        0        0   475533 2023-04-20 14:38:40.249343 tessif-examples-0.3.2/src/tessif_examples/data/load_profiles/el_demand_HH_2019.csv
+-rw-r--r--   0        0        0   138415 2023-04-20 14:38:40.253343 tessif-examples-0.3.2/src/tessif_examples/data/load_profiles/solar_HH_2019.csv
+-rw-r--r--   0        0        0   408648 2023-04-20 14:38:40.253343 tessif-examples-0.3.2/src/tessif_examples/data/load_profiles/th_demand_HH_2019.csv
+-rw-r--r--   0        0        0   200160 2023-04-20 14:38:40.253343 tessif-examples-0.3.2/src/tessif_examples/data/load_profiles/wind_HH_2019.csv
+-rw-r--r--   0        0        0      371 2023-04-20 14:38:40.253343 tessif-examples-0.3.2/src/tessif_examples/paths.py
+-rw-r--r--   0        0        0      205 2023-04-20 14:38:40.253343 tessif-examples-0.3.2/src/tessif_examples/plausibility/__init__.py
+-rw-r--r--   0        0        0     3315 2023-04-20 14:38:40.253343 tessif-examples-0.3.2/src/tessif_examples/plausibility/chp_emissions.py
+-rw-r--r--   0        0        0     2919 2023-04-20 14:38:40.253343 tessif-examples-0.3.2/src/tessif_examples/plausibility/storage_emissions.py
+-rw-r--r--   0        0        0      336 2023-04-20 14:38:40.253343 tessif-examples-0.3.2/src/tessif_examples/scientific/__init__.py
+-rw-r--r--   0        0        0    27706 2023-04-20 14:38:40.253343 tessif-examples-0.3.2/src/tessif_examples/scientific/component_focused.py
+-rw-r--r--   0        0        0    45190 2023-04-20 14:38:40.253343 tessif-examples-0.3.2/src/tessif_examples/scientific/grid_focused.py
+-rw-r--r--   0        0        0    26324 2023-04-20 14:38:40.257343 tessif-examples-0.3.2/src/tessif_examples/scientific/hamburg_inspired.py
+-rw-r--r--   0        0        0      280 2023-04-20 14:38:40.257343 tessif-examples-0.3.2/src/tessif_examples/specialized/__init__.py
+-rw-r--r--   0        0        0    34235 2023-04-20 14:38:40.257343 tessif-examples-0.3.2/src/tessif_examples/specialized/generic_grid.py
+-rw-r--r--   0        0        0    10476 2023-04-20 14:38:40.257343 tessif-examples-0.3.2/src/tessif_examples/specialized/self_similar_system_model.py
+-rw-r--r--   0        0        0     4758 2023-04-20 14:38:40.257343 tessif-examples-0.3.2/src/tessif_examples/specialized/variable_chp.py
+-rw-r--r--   0        0        0     2455 2023-04-20 14:38:40.257343 tessif-examples-0.3.2/src/tessif_examples/utils.py
+-rw-r--r--   0        0        0     6679 1970-01-01 00:00:00.000000 tessif-examples-0.3.2/setup.py
+-rw-r--r--   0        0        0     6320 1970-01-01 00:00:00.000000 tessif-examples-0.3.2/PKG-INFO
```

### Comparing `tessif-examples-0.3.1/LICENSE` & `tessif-examples-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tessif-examples-0.3.1/README.rst` & `tessif-examples-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `tessif-examples-0.3.1/pyproject.toml` & `tessif-examples-0.3.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tessif-examples"
-version = "0.3.1"
+version = "0.3.2"
 description = "Tessif Examples Library"
 authors = ["Mathias Ammon <tz3ma.coding@use.startmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/tZ3ma/tessif_examples"
 homepage = "https://github.com/tZ3ma/tessif_examples"
 keywords = ["tessif", "examples"]
```

### Comparing `tessif-examples-0.3.1/src/tessif_examples/basic/__init__.py` & `tessif-examples-0.3.2/src/tessif_examples/basic/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 from .chp import create_chp
 from .connected_es import create_connected_es
 from .emission_objective import create_emission_objective
 from .expansion_plan_example import create_expansion_plan_example
 from .fpwe import create_fpwe
 from .mwe import create_mwe
 from .simple_transformer_grid_es import create_simple_transformer_grid_es
+from .statistical_identification_example import (
+    create_statistical_identification_example,
+)
 from .storage_example import create_storage_example
 from .storage_fixed_ratio_expansion_example import (
     create_storage_fixed_ratio_expansion_example,
 )
 from .time_varying_efficiency_transformer import (
     create_time_varying_efficiency_transformer,
 )
```

### Comparing `tessif-examples-0.3.1/src/tessif_examples/basic/chp.py` & `tessif-examples-0.3.2/src/tessif_examples/basic/chp.py`

 * *Files identical despite different names*

### Comparing `tessif-examples-0.3.1/src/tessif_examples/basic/connected_es.py` & `tessif-examples-0.3.2/src/tessif_examples/basic/connected_es.py`

 * *Files identical despite different names*

### Comparing `tessif-examples-0.3.1/src/tessif_examples/basic/emission_objective.py` & `tessif-examples-0.3.2/src/tessif_examples/basic/emission_objective.py`

 * *Files identical despite different names*

### Comparing `tessif-examples-0.3.1/src/tessif_examples/basic/expansion_plan_example.py` & `tessif-examples-0.3.2/src/tessif_examples/basic/expansion_plan_example.py`

 * *Files identical despite different names*

### Comparing `tessif-examples-0.3.1/src/tessif_examples/basic/fpwe.py` & `tessif-examples-0.3.2/src/tessif_examples/basic/fpwe.py`

 * *Files identical despite different names*

### Comparing `tessif-examples-0.3.1/src/tessif_examples/basic/mwe.py` & `tessif-examples-0.3.2/src/tessif_examples/basic/mwe.py`

 * *Files identical despite different names*

### Comparing `tessif-examples-0.3.1/src/tessif_examples/basic/simple_transformer_grid_es.py` & `tessif-examples-0.3.2/src/tessif_examples/basic/simple_transformer_grid_es.py`

 * *Files identical despite different names*

### Comparing `tessif-examples-0.3.1/src/tessif_examples/basic/storage_example.py` & `tessif-examples-0.3.2/src/tessif_examples/basic/storage_example.py`

 * *Files identical despite different names*

### Comparing `tessif-examples-0.3.1/src/tessif_examples/basic/storage_fixed_ratio_expansion_example.py` & `tessif-examples-0.3.2/src/tessif_examples/basic/storage_fixed_ratio_expansion_example.py`

 * *Files identical despite different names*

### Comparing `tessif-examples-0.3.1/src/tessif_examples/basic/time_varying_efficiency_transformer.py` & `tessif-examples-0.3.2/src/tessif_examples/basic/time_varying_efficiency_transformer.py`

 * *Files identical despite different names*

### Comparing `tessif-examples-0.3.1/src/tessif_examples/basic/zero_costs_es.py` & `tessif-examples-0.3.2/src/tessif_examples/basic/zero_costs_es.py`

 * *Files identical despite different names*

### Comparing `tessif-examples-0.3.1/src/tessif_examples/data/load_profiles/Loads.csv` & `tessif-examples-0.3.2/src/tessif_examples/data/load_profiles/Loads.csv`

 * *Files identical despite different names*

### Comparing `tessif-examples-0.3.1/src/tessif_examples/data/load_profiles/Renewable_Energy.csv` & `tessif-examples-0.3.2/src/tessif_examples/data/load_profiles/Renewable_Energy.csv`

 * *Files identical despite different names*

### Comparing `tessif-examples-0.3.1/src/tessif_examples/data/load_profiles/component_scenario_profiles.csv` & `tessif-examples-0.3.2/src/tessif_examples/data/load_profiles/component_scenario_profiles.csv`

 * *Files identical despite different names*

### Comparing `tessif-examples-0.3.1/src/tessif_examples/data/load_profiles/el_demand_HH_2019.csv` & `tessif-examples-0.3.2/src/tessif_examples/data/load_profiles/el_demand_HH_2019.csv`

 * *Files identical despite different names*

### Comparing `tessif-examples-0.3.1/src/tessif_examples/data/load_profiles/solar_HH_2019.csv` & `tessif-examples-0.3.2/src/tessif_examples/data/load_profiles/solar_HH_2019.csv`

 * *Files identical despite different names*

### Comparing `tessif-examples-0.3.1/src/tessif_examples/data/load_profiles/th_demand_HH_2019.csv` & `tessif-examples-0.3.2/src/tessif_examples/data/load_profiles/th_demand_HH_2019.csv`

 * *Files identical despite different names*

### Comparing `tessif-examples-0.3.1/src/tessif_examples/data/load_profiles/wind_HH_2019.csv` & `tessif-examples-0.3.2/src/tessif_examples/data/load_profiles/wind_HH_2019.csv`

 * *Files identical despite different names*

### Comparing `tessif-examples-0.3.1/src/tessif_examples/scientific/component_focused.py` & `tessif-examples-0.3.2/src/tessif_examples/scientific/component_focused.py`

 * *Files identical despite different names*

### Comparing `tessif-examples-0.3.1/src/tessif_examples/scientific/grid_focused.py` & `tessif-examples-0.3.2/src/tessif_examples/scientific/grid_focused.py`

 * *Files identical despite different names*

### Comparing `tessif-examples-0.3.1/src/tessif_examples/scientific/hamburg_inspired.py` & `tessif-examples-0.3.2/src/tessif_examples/scientific/hamburg_inspired.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,14 @@
     max_th = np.max(th_hh)
 
     # 4. Create the individual energy system components:
     in_stat = False
     cfba = 0
 
     # Global Constraints:
-
     global_constraints = {
         "name": "2019",
         "emissions": float("+inf"),
         # 'resources': float('+inf'),
     }
 
     # Fossil Sources:
@@ -575,16 +574,18 @@
         sector="power",
         carrier="solar",
         flow_rates={"electricity": nts.MinMax(min=0, max=max_pv)},
         flow_costs={"electricity": 74},
         flow_emissions={"electricity": 0},
         timeseries={"electricity": nts.MinMax(min=pv_hh, max=pv_hh)},
         expandable={"electricity": True},
-        expansion_costs={"electricity": utils.annuity(capex=1000000, n=20, wacc=0.05)},
-        expansion_limits={"electricity": nts.MinMax(min=max_pv, max=float("+inf"))},
+        expansion_costs={"electricity": utils.annuity(
+            capex=1000000, n=20, wacc=0.05)},
+        expansion_limits={"electricity": nts.MinMax(
+            min=max_pv, max=float("+inf"))},
     )
 
     won1 = components.Source(
         name="won1",
         outputs=("electricity",),
         region="HH",
         node_type="renewable",
@@ -592,16 +593,18 @@
         sector="power",
         carrier="wind",
         flow_rates={"electricity": nts.MinMax(min=0, max=max_wo)},
         flow_costs={"electricity": 61},
         flow_emissions={"electricity": 0.007},  # 0.007
         timeseries={"electricity": nts.MinMax(min=wo_hh, max=wo_hh)},
         expandable={"electricity": True},
-        expansion_costs={"electricity": utils.annuity(capex=1750000, n=20, wacc=0.05)},
-        expansion_limits={"electricity": nts.MinMax(min=max_wo, max=float("+inf"))},
+        expansion_costs={"electricity": utils.annuity(
+            capex=1750000, n=20, wacc=0.05)},
+        expansion_limits={"electricity": nts.MinMax(
+            min=max_wo, max=float("+inf"))},
     )
 
     bm_supply = components.Source(
         name="biomass supply",
         outputs=("biomass",),
         region="HH",
         node_type="renewable",
@@ -624,15 +627,16 @@
         sector="power",
         carrier="electricity",
         component="storage",
         flow_rates={"electricity": nts.MinMax(0, float("+inf"))},
         flow_costs={"electricity": 20},
         flow_emissions={"electricity": 0},
         expendable={"capacity": True, "electricity": False},
-        expansion_costs={"capacity": utils.annuity(capex=1000000, n=10, wacc=0.05)},
+        expansion_costs={"capacity": utils.annuity(
+            capex=1000000, n=10, wacc=0.05)},
     )
 
     # P2H Karoline:
 
     p2h = components.Transformer(
         name="p2h",
         inputs=("electricity",),
@@ -650,15 +654,16 @@
         flow_rates={
             "electricity": nts.MinMax(min=0, max=float("+inf")),
             "hot_water": nts.MinMax(min=0, max=45),
         },  # 45
         flow_costs={"electricity": 0, "hot_water": 0},
         flow_emissions={"electricity": 0, "hot_water": 0},  # 0.007
         expandable={"electricity": False, "hot_water": True},
-        expansion_costs={"hot_water": utils.annuity(capex=200000, n=30, wacc=0.05)},
+        expansion_costs={"hot_water": utils.annuity(
+            capex=200000, n=30, wacc=0.05)},
         expansion_limits={"hot_water": nts.MinMax(min=45, max=200)},
     )
 
     # Imported Electricity/ Heat:
 
     imel = components.Source(
         name="imported el",
```

### Comparing `tessif-examples-0.3.1/src/tessif_examples/specialized/generic_grid.py` & `tessif-examples-0.3.2/src/tessif_examples/specialized/generic_grid.py`

 * *Files identical despite different names*

### Comparing `tessif-examples-0.3.1/src/tessif_examples/specialized/self_similar_system_model.py` & `tessif-examples-0.3.2/src/tessif_examples/specialized/self_similar_system_model.py`

 * *Files identical despite different names*

### Comparing `tessif-examples-0.3.1/src/tessif_examples/specialized/variable_chp.py` & `tessif-examples-0.3.2/src/tessif_examples/specialized/variable_chp.py`

 * *Files identical despite different names*

### Comparing `tessif-examples-0.3.1/src/tessif_examples/utils.py` & `tessif-examples-0.3.2/src/tessif_examples/utils.py`

 * *Files identical despite different names*

### Comparing `tessif-examples-0.3.1/setup.py` & `tessif-examples-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 
 package_dir = \
 {'': 'src'}
 
 packages = \
 ['tessif_examples',
  'tessif_examples.basic',
+ 'tessif_examples.plausibility',
  'tessif_examples.scientific',
  'tessif_examples.specialized']
 
 package_data = \
 {'': ['*'], 'tessif_examples': ['data/load_profiles/*']}
 
 install_requires = \
 ['numpy', 'pandas', 'tessif>=0.0.25']
 
 setup_kwargs = {
     'name': 'tessif-examples',
-    'version': '0.3.1',
+    'version': '0.3.2',
     'description': 'Tessif Examples Library',
     'long_description': 'tessif-examples\n===============\n\n|PyPI| |Python Version| |License| |Status|\n\n|Stable Release| |Develop Release|\n\n|Read the Docs| |Tests| |Safety| |Pylinting| |Flake8 Linting| |Pre-Commit|\n\n|Codecov| |Codacy| |Codeclimate| |Scrutinizer|\n\n|pre-commit| |Black| |Pylint| |Flake8|\n\n.. |PyPI| image:: https://img.shields.io/pypi/v/tessif-examples.svg\n   :target: https://pypi.org/project/tessif-examples/\n   :alt: PyPI\n\n.. |Python Version| image:: https://img.shields.io/pypi/pyversions/tessif-examples\n   :target: https://pypi.org/project/tessif-examples\n   :alt: Python Version\n\n.. |License| image:: https://img.shields.io/pypi/l/tessif-examples\n   :target: https://opensource.org/licenses/MIT\n   :alt: License\n\n.. |Status| image:: https://img.shields.io/pypi/status/tessif-examples.svg\n   :target: https://pypi.org/project/tessif-examples/\n   :alt: Status\n\n.. |Stable Release| image:: https://github.com/tZ3ma/tessif-examples/workflows/Stable-PyPI-Release/badge.svg\n   :target: https://github.com/tZ3ma/tessif-examples/actions?workflow=Stable-PyPI-Release\n   :alt: Stable PyPI Release Workflow Status\n\n.. |Develop Release| image:: https://github.com/tZ3ma/tessif-examples/workflows/Develop-TestPyPI-Release/badge.svg\n   :target: https://github.com/tZ3ma/tessif-examples/actions?workflow=Develop-TestPyPI-Release\n   :alt: Develop TestPyPI Release Workflow Status\n\n.. |Read the Docs| image:: https://img.shields.io/readthedocs/tessif-examples/latest.svg?label=Read%20the%20Docs\n   :target: https://tessif-examples.readthedocs.io/\n   :alt: Read the documentation at https://tessif-examples.readthedocs.io/\n\n.. |Tests| image:: https://github.com/tZ3ma/tessif-examples/workflows/Tests-and-Coverage/badge.svg\n   :target: https://github.com/tZ3ma/tessif-examples/actions?workflow=Tests-and-Coverage\n   :alt: Tests Workflow Status\n\n.. |Safety| image:: https://github.com/tZ3ma/tessif-examples/workflows/Safety/badge.svg\n   :target: https://github.com/tZ3ma/tessif-examples/actions?workflow=Safety\n   :alt: Safety Workflow Status\n\n.. |Pylinting| image:: https://github.com/tZ3ma/tessif-examples/workflows/Pylinting/badge.svg\n   :target: https://github.com/tZ3ma/tessif-examples/actions?workflow=Pylinting\n   :alt: Pylint Workflow Status\n\n.. |Flake8 Linting| image:: https://github.com/tZ3ma/tessif-examples/workflows/Flake8-Linting/badge.svg\n   :target: https://github.com/tZ3ma/tessif-examples/actions?workflow=Flake8-Linting\n   :alt: Flake8-Linting Workflow Status\n\n.. |Pre-Commit| image:: https://github.com/tZ3ma/tessif-examples/workflows/Pre-Commit/badge.svg\n   :target: https://github.com/tZ3ma/tessif-examples/actions?workflow=Pre-Commit\n   :alt: Pre-Commit Workflow Status\n\n.. |Codecov| image:: https://codecov.io/gh/tZ3ma/tessif-examples/branch/main/graph/badge.svg\n   :target: https://codecov.io/gh/tZ3ma/tessif-examples\n   :alt: Codecov\n\n.. |Codacy| image:: https://app.codacy.com/project/badge/Grade/b278433bb9224147a2e6231d783b62e4\n   :target: https://app.codacy.com/gh/tZ3ma/tessif-examples/dashboard\n   :alt: Codacy Code Quality Status\n\n.. |Codeclimate| image:: https://api.codeclimate.com/v1/badges/ff119252f0bb7f40aecb/maintainability\n   :target: https://codeclimate.com/github/tZ3ma/tessif-examples/maintainability\n   :alt: Maintainability\n\n.. |Scrutinizer| image:: https://scrutinizer-ci.com/g/tZ3ma/tessif-examples/badges/quality-score.png?b=main\n   :target: https://scrutinizer-ci.com/g/tZ3ma/tessif-examples/\n   :alt: Scrutinizer Code Quality\n\n.. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white\n   :target: https://github.com/pre-commit/pre-commit\n   :alt: pre-commit\n\n.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/psf/black\n   :alt: Black\n\n.. |Pylint| image:: https://img.shields.io/badge/linting-pylint-yellowgreen\n   :target: https://github.com/PyCQA/pylint\n   :alt: Package uses pylint\n\n.. |Flake8| image:: https://img.shields.io/badge/linting-flake8-yellogreen\n   :target: https://github.com/pycqa/flake8\n   :alt: Package uses flake8\n\n\nTessif_ example library\n\nInstallation\n------------\n\nPlease see the `Installation Guide`_ (`Github Repo Link`_) for details.\n\n\nUsage\n-----\n\nPlease see the `Worklow Reference <Workflow-Guide_>`_ (`Github Repo Link`_) for details.\n\n\nContributing\n------------\n\nContributions are very welcome.\nTo learn more, see the `Contributor Guide`_ (`Github Repo Link`_).\n\n\nLicense\n-------\n\nDistributed under the terms of the `MIT license`_ (`Github Repo Link`_),\n*tessif-examples* is free and open source software.\n\n\nIssues\n------\n\nIf you encounter any problems,\nplease `file an issue`_ along with a detailed description.\n\nCredits\n-------\n\nThis project was created using the `Mathias Ammon <tZ3ma>`_ tweaked version of the\nHypermodern-Python_ project foundation proposed by `Claudio Jolowicz <cj>`_.\n\n.. _Tessif: https://github.com/tZ3ma/tessif\n\n.. _Hypermodern-Python: https://cjolowicz.github.io/posts/hypermodern-python-01-setup/\n.. _Hypermodern Python Cookiecutter: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n.. _cj: https://github.com/cjolowicz\n\n.. _MIT license: https://opensource.org/licenses/MIT\n.. _PyPI: https://pypi.org/\n\n.. _file an issue: https://github.com/tZ3ma/tessif-examples/issues\n.. _pip: https://pip.pypa.io/\n\n.. _tZ3ma: https://github.com/tZ3ma\n.. working on github-only\n.. _Contributor Guide: CONTRIBUTING.rst\n.. _Installation Guide: docs/source/getting_started/installation.rst\n.. _Workflow-Guide: docs/source/developer_guide/workflows.rst\n\n.. _Github Repo Link: https://github.com/tZ3ma/tessif-examples\n',
     'author': 'Mathias Ammon',
     'author_email': 'tz3ma.coding@use.startmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tZ3ma/tessif_examples',
```

### Comparing `tessif-examples-0.3.1/PKG-INFO` & `tessif-examples-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tessif-examples
-Version: 0.3.1
+Version: 0.3.2
 Summary: Tessif Examples Library
 Home-page: https://github.com/tZ3ma/tessif_examples
 License: MIT
 Keywords: tessif,examples
 Author: Mathias Ammon
 Author-email: tz3ma.coding@use.startmail.com
 Requires-Python: >=3.8,<4.0
```

