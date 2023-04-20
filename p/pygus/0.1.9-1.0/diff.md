# Comparing `tmp/pygus-0.1.9.tar.gz` & `tmp/pygus-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygus-0.1.9.tar", max compression
+gzip compressed data, was "pygus-1.0.tar", max compression
```

## Comparing `pygus-0.1.9.tar` & `pygus-1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2022-10-31 16:02:43.286749 pygus-0.1.9/LICENSE
--rw-r--r--   0        0        0     1541 2022-12-20 14:05:39.918640 pygus-0.1.9/README-pypi.md
--rw-r--r--   0        0        0     1426 2022-12-20 15:18:05.762311 pygus-0.1.9/pyproject.toml
--rw-r--r--   0        0        0        0 2022-10-31 16:02:43.362975 pygus-0.1.9/src/__init__.py
--rw-r--r--   0        0        0        0 2022-10-31 16:02:43.363021 pygus-0.1.9/src/gus/__init__.py
--rw-r--r--   0        0        0    27375 2022-10-31 16:02:43.363160 pygus-0.1.9/src/gus/agents.py
--rw-r--r--   0        0        0     7340 2022-10-31 16:02:43.363241 pygus-0.1.9/src/gus/allometrics.py
--rw-r--r--   0        0        0     3069 2022-10-31 16:02:43.363326 pygus-0.1.9/src/gus/inputs/allometrics.json
--rw-r--r--   0        0        0       95 2022-10-31 16:02:43.363377 pygus-0.1.9/src/gus/inputs/scenario.json
--rw-r--r--   0        0        0      264 2022-10-31 16:02:43.363427 pygus-0.1.9/src/gus/inputs/site.json
--rw-r--r--   0        0        0     5932 2022-10-31 16:02:43.363500 pygus-0.1.9/src/gus/inputs/trees.csv
--rw-r--r--   0        0        0    15486 2022-10-31 16:02:43.363727 pygus-0.1.9/src/gus/models.py
--rw-r--r--   0        0        0  1566870 2022-10-31 16:02:43.370857 pygus-0.1.9/src/gus/outputs/trees_yearly.json
--rw-r--r--   0        0        0     1062 2022-10-31 16:02:43.370958 pygus-0.1.9/src/gus/utilities.py
--rw-r--r--   0        0        0     1680 2022-10-31 16:02:43.371014 pygus-0.1.9/src/gus/weather.py
--rw-r--r--   0        0        0        0 2022-10-31 16:02:43.371038 pygus-0.1.9/src/impacts/__init__.py
--rw-r--r--   0        0        0     3233 2022-10-31 16:02:43.371220 pygus-0.1.9/src/impacts/carbon.py
--rw-r--r--   0        0        0    29289 2022-10-31 16:02:43.371475 pygus-0.1.9/src/impacts/water.py
--rw-r--r--   0        0        0     2643 1970-01-01 00:00:00.000000 pygus-0.1.9/setup.py
--rw-r--r--   0        0        0     3228 1970-01-01 00:00:00.000000 pygus-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-10-31 16:02:43.286749 pygus-1.0/LICENSE
+-rw-r--r--   0        0        0     1541 2023-02-22 17:36:23.738197 pygus-1.0/README-pypi.md
+-rw-r--r--   0        0        0      134 2023-04-20 10:39:32.247844 pygus-1.0/pygus/__init__.py
+-rw-r--r--   0        0        0      156 2023-04-20 10:39:32.248007 pygus-1.0/pygus/gus/__init__.py
+-rw-r--r--   0        0        0    27311 2023-04-20 10:39:32.248384 pygus-1.0/pygus/gus/agents.py
+-rw-r--r--   0        0        0     7484 2023-04-20 10:39:32.248656 pygus-1.0/pygus/gus/allometrics.py
+-rw-r--r--   0        0        0     3069 2023-04-20 10:39:32.248771 pygus-1.0/pygus/gus/inputs/allometrics.json
+-rw-r--r--   0        0        0       95 2023-04-20 10:39:32.248836 pygus-1.0/pygus/gus/inputs/scenario.json
+-rw-r--r--   0        0        0      264 2023-04-20 10:39:32.248895 pygus-1.0/pygus/gus/inputs/site.json
+-rw-r--r--   0        0        0     5932 2023-04-20 10:39:32.248983 pygus-1.0/pygus/gus/inputs/trees.csv
+-rw-r--r--   0        0        0    15469 2023-04-20 10:39:32.249144 pygus-1.0/pygus/gus/models.py
+-rw-r--r--   0        0        0  1566870 2023-04-20 10:39:32.257838 pygus-1.0/pygus/gus/outputs/trees_yearly.json
+-rw-r--r--   0        0        0     2241 2023-04-20 12:41:09.601132 pygus-1.0/pygus/gus/utilities.py
+-rw-r--r--   0        0        0     1701 2023-04-20 10:39:32.258149 pygus-1.0/pygus/gus/weather.py
+-rw-r--r--   0        0        0       58 2023-04-20 10:39:32.258299 pygus-1.0/pygus/impacts/__init__.py
+-rw-r--r--   0        0        0     3214 2023-04-20 10:39:32.258425 pygus-1.0/pygus/impacts/carbon.py
+-rw-r--r--   0        0        0    32960 2023-04-20 10:39:32.258637 pygus-1.0/pygus/impacts/water.py
+-rw-r--r--   0        0        0     1499 2023-04-20 12:46:01.662170 pygus-1.0/pyproject.toml
+-rw-r--r--   0        0        0     2655 1970-01-01 00:00:00.000000 pygus-1.0/setup.py
+-rw-r--r--   0        0        0     3262 1970-01-01 00:00:00.000000 pygus-1.0/PKG-INFO
```

### Comparing `pygus-0.1.9/LICENSE` & `pygus-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygus-0.1.9/README-pypi.md` & `pygus-1.0/README-pypi.md`

 * *Files identical despite different names*

### Comparing `pygus-0.1.9/pyproject.toml` & `pygus-1.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
-name = "pyGus"
-version = "0.1.9"
+name = "pyGUS"
+version = "1.0"
 description = "Green Urban Scenarios - A digital twin representation, simulation of urban forests and their impact analysis."
 authors = ["Bulent Ozel <bulent@lucidminds.ai>"] 
 maintainers = [
     "Oguzhan Yayla <oguzhan@lucidminds.ai>", 
     "Marko Petrovic <marko@lucidminds.ai>", 
     "Axel Nilsson <axel@darkmatterlabs.org>"
 ]
@@ -20,15 +20,15 @@
     'Programming Language :: Python',
     'Programming Language :: Python :: 3 :: Only',
     'Topic :: Software Development :: Libraries',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: Utilities'
 ]
 packages = [
-    {include = "src"},
+    {include = "pygus"},
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.8.0"
 ipython = "^7.27.0"
 mesa = "^0.8.9"
@@ -36,21 +36,25 @@
 pandas = "^1.3.3"
 pytest = "^7.1.2"
 fuzzywuzzy = "^0.18.0"
 matplotlib = "^3.4.3"
 seaborn = "^0.11.2"
 portray = "^1.7.0"
 termcolor = "^2.1.1"
+utm = "^0.7.0"
+
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.portray]
-modules = ["src"]
+modules = ["pygus"]
 
 
 [tool.portray.mkdocs.theme]
 name = "readthedocs"
 
 [[tool.portray.mkdocs.nav]]
 Home = "README.md"
```

### Comparing `pygus-0.1.9/src/gus/agents.py` & `pygus-1.0/pygus/gus/agents.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 
 # Basic Python packages
 import numpy as np
 
 # Mesa Packages
 from mesa import Agent
 
+
 class Tree(Agent):
     """A generic Tree agent with basic structural attributes and a growth model.
 
     It inherits the generic mesa.Agent class.
     """
+
     # Def: Carbon storage cap in sequestration calculations. A tree with that amount of CARBON or above this level
     # has a constant yearly sequestration which is 25kg/year.
     # Unit: Kg
     # Ref: iTree, 2020
     carbon_storage_cap = 7500
     sequestration_at_maturity = 25
 
@@ -28,43 +30,46 @@
     decomposition_coeff = 0.1
 
     # Fixed rates for crown light exposure to sunlight (CLE).
     # 0.44: Forest conditions with a closed, or nearly closed canopy,
     # 0.56: Park conditions
     # 1.0:  Open-grown conditions, street trees.
     # Source: iTree
-    sun_exposure_rates = {
-        'forest': 0.44,
-        'park': 0.56,
-        'street': 1.0,
-        'pocket':0.56}
+    sun_exposure_rates = {"forest": 0.44, "park": 0.56, "street": 1.0, "pocket": 0.56}
 
     # Condition multipliers. Used at adjusting growth rates.
     # Ref: Fleming, 1988, and Nowak 2002b
     condition_multiplier = {
-        'excellent': 1,
-        'good': 1,
-        'fair': 1,
-        'poor': 0.76,
-        'critical': 0.42,
-        'dying': 0.15,
-        'dead': 0}
+        "excellent": 1,
+        "good": 1,
+        "fair": 1,
+        "poor": 0.76,
+        "critical": 0.42,
+        "dying": 0.15,
+        "dead": 0,
+    }
 
     # Ref: Root to shoot ratio (Cairns et al. 1997)
     root_to_shoot_ratio = 0.26
 
     # Biomass ratio at crown to trunk: Needs validation
     crown_to_trunk_ratio = 0.05
 
-    def __init__(self, unique_id, model, dbh, species,
-                 height=None,
-                 kind="deciduous",
-                 fixed_sun_exposure=False,
-                 condition=None,
-                 dieback=None):
+    def __init__(
+        self,
+        unique_id,
+        model,
+        dbh,
+        species,
+        height=None,
+        kind="deciduous",
+        fixed_sun_exposure=False,
+        condition=None,
+        dieback=None,
+    ):
         """The constructor method.
 
         Args:
             unique_id: (:obj:`int`): a unique agent id
             model: (Mesa.Model): the underlying Mesa model.
             dbh: (:obj:`float`): the DBH measure which is diameter in cm of the trunk
                 usually measured at 1.3m from the ground.
@@ -89,31 +94,31 @@
         self.kind = kind
         self.species = model.species.fuzzymatching(species)
         self.dbh = dbh
         self.fixed_sun_exposure = fixed_sun_exposure
         self.overlap_ratio = 0
 
         # Initialize canonical growth functions
-        self.f_tree_height = self.model.species.get_eqn(self.species,'height')
+        self.f_tree_height = self.model.species.get_eqn(self.species, "height")
         self.f_biomass = self.model.species.get_eqn_biomass(self.species)
-        self.f_crown_width = self.model.species.get_eqn(self.species,'crown_width')
-        self.f_crown_height = self.model.species.get_eqn(self.species,'crown_height')
-        
+        self.f_crown_width = self.model.species.get_eqn(self.species, "crown_width")
+        self.f_crown_height = self.model.species.get_eqn(self.species, "crown_height")
+
         # Record initial allometries
         if height:
             self.tree_height = height
         else:
             self.tree_height = self.f_tree_height(self.dbh)
         self.crown_width = self.f_crown_width(self.dbh)
         self.crown_height = self.f_crown_height(self.dbh)
 
         # dieback related initializations:
         # Note: this needs to be handled at the initialization module
         self.dieback = 0
-        self.condition = 'excellent'
+        self.condition = "excellent"
         if dieback and condition:
             self.condition = condition
             self.dieback = dieback
         elif dieback:
             self.condition = self._get_condition_class(dieback)
             self.dieback = dieback
         elif condition:
@@ -124,23 +129,25 @@
             self.condition = self._get_condition_class(self.dieback)
 
         self.diameter_growth = model.species.get_diameter_growth(species)
         # Slow, moderate and fast growing species respectively.
         # c(0.23, 0.33, 0.43) in inch/yr Source: https://database.itreetools.org/#/splash
         # Converted into cm.
 
-        #Default crown light exposure based on site types.
+        # Default crown light exposure based on site types.
         self.cle = Tree.sun_exposure_rates[self.model.site_type]
         # Crown light exposure to sunlight (CLE).
         # CLE <- c(0.44, 0.56, 1)
         # (1) Forest conditions with a closed, or nearly closed canopy,
         # (2) Park conditions
         # (3) Open-grown conditions.
 
-        self.average_height_at_maturity = model.species.get_height_at_maturity(self.species)
+        self.average_height_at_maturity = model.species.get_height_at_maturity(
+            self.species
+        )
         # Avg height at maturity for the given species.
 
         self.biomass = self.compute_biomass()  # In Kg
         self.carbon_storage = Tree.carbon_coeff * self.biomass  # In Kg
 
         # Amount of carbon release due to dead portion.
         self.decomposition = 0  # In Kg
@@ -174,53 +181,53 @@
             None
 
         Todo:
             None
         """
         # Once the replaced tree agents are removed from the model, this line will be idle and s
         # should be removed too.
-        if self.condition == 'replaced':
+        if self.condition == "replaced":
             return
 
         # The tree is dead and its carbon release schedule is accounted.
         if self.death_acc:
             self._reset_release_track()
             if np.random.uniform(0, 1) < self.expected_care:
                 self.replace()
             return
 
-        if self.condition == 'dead':
+        if self.condition == "dead":
             self.compute_decomposition()
             return
 
         # check frost free days for the past year.
         frost_free_days = self.model.WeatherAPI.check_frost_free_days()
-        #print('Tree: {} checks ffdays = {} ...'.format(self.unique_id, frost_free_days))
+        # print('Tree: {} checks ffdays = {} ...'.format(self.unique_id, frost_free_days))
 
         # compute the light exposure
         self.compute_light_exposure()
 
         # check state of the health of the tree
-        #print('Tree: {} checks dieback ...'.format(self.unique_id))
+        # print('Tree: {} checks dieback ...'.format(self.unique_id))
         self.check_dieback()
 
         # compute the growth
-        #print('Tree: {} grows ...'.format(self.unique_id))
+        # print('Tree: {} grows ...'.format(self.unique_id))
         self.grow(frost_free_days)
 
         # compute the total biomass
         self.compute_biomass()
-        #print('Tree: {} biomass ...'.format(self.unique_id))
+        # print('Tree: {} biomass ...'.format(self.unique_id))
 
         # compute the amount of new carbon sequestration
         self.compute_sequestration()
-        #print('Tree: {} sequestration ...'.format(self.unique_id))
+        # print('Tree: {} sequestration ...'.format(self.unique_id))
 
         # compute the amount of carbon release due to decomposition
-        #print('Tree: {} decomposition ...'.format(self.unique_id))
+        # print('Tree: {} decomposition ...'.format(self.unique_id))
         self.compute_decomposition()
 
     def grow(self, frost_free_days):
         """The method updates DBH of the tree. Currently it is an annual growth in cm.
 
         Args:
             frost_free_days: (:obj:`int`): the number of observed frost free days
@@ -256,15 +263,15 @@
             delta_dbh = 0.0222 + 2.1729 * (1.25 - height_ratio)
         else:
             delta_dbh = self.diameter_growth * self.cle * (1 - self.dieback)
 
         # Adjust the growth rate according to health condition.
         delta_dbh *= Tree.condition_multiplier[self.condition]
         self.dbh += delta_dbh * (frost_free_days / 153)
-       
+
         # Update the tree height based on the updated dbh.
         self.update_tree_height(generic=False)
         # Update the change at canopy.
         self.update_crown_width()
         self.update_crown_height()
 
     def estimate_tree_height(self):
@@ -303,29 +310,29 @@
 
         Args:
             None
         Returns:
             None
         """
         self.tree_height += Tree.condition_multiplier[self.condition] * 0.15
-    
+
     def update_crown_height(self):
-        """Computes the vertical length of the tree crown based on 
+        """Computes the vertical length of the tree crown based on
         the species and its current dbh.
 
         Args:
             None
         Returns:
             (:obj:`float`): Current crown width in meters
         """
         self.crown_height = self.f_crown_height(self.dbh)
         return self.crown_height
-  
+
     def update_crown_width(self):
-        """Computes the horizontal length of the tree crown based on 
+        """Computes the horizontal length of the tree crown based on
         the species and its current dbh.
 
         Args:
             None
         Returns:
             (:obj:`float`): Current crown width in meters
         """
@@ -348,38 +355,37 @@
             Canopy overlap ratio is used as proxy to determine available CLE. The model assumes that
             a taller neighbourung tree reduces sun light exposure.
 
         Todo:
             * The assumption needs to be revisited and validated.
             * The model needs to be revised in case the same location is shared by other species.
         """
-        if self.fixed_sun_exposure: return
+        if self.fixed_sun_exposure:
+            return
 
-        #cellmates = self.model.grid.get_cell_list_contents([self.pos])
+        # cellmates = self.model.grid.get_cell_list_contents([self.pos])
         posns_list = self.model.grid.get_neighborhood(
-            self.pos,
-            moore = False,
-            include_center = False,
-            radius = 1)
+            self.pos, moore=False, include_center=False, radius=1
+        )
         neighboors = self.model.grid.get_cell_list_contents(posns_list)
         self.overlap_ratio = 0
         combined_overlap = 0
         for t in neighboors:
             t_w = t.crown_width
             t_h = t.tree_height
-            # 0.5 multiplier is a mean multiplier to correct square shaped assumption on tree crown shape. 
+            # 0.5 multiplier is a mean multiplier to correct square shaped assumption on tree crown shape.
             overlap = max(0, 0.5 * (self.crown_width + t_w) - self.model.dt_resolution)
             # 0.25 multiplier is to account one of the four sides of the grid cell.
             overlap_ratio = 0.25 * min(1, (overlap / self.crown_width))
             # a taller tree creates more shading
             combined_overlap += overlap_ratio * (t_h / (t_h + self.tree_height))
-            self.overlap_ratio += overlap_ratio 
+            self.overlap_ratio += overlap_ratio
         # Cases needs to be inspected
         self.overlap_ratio = min(1, self.overlap_ratio)
-        light_loss_multiplier = 0.75 # arbitrary to be fixed with empirical data. 
+        light_loss_multiplier = 0.75  # arbitrary to be fixed with empirical data.
         self.cle = max(0, 1 - light_loss_multiplier * combined_overlap)
 
         # try:
         #     total_dbh = sum([t.dbh for t in cellmates])
         #     cle = self.dbh / total_dbh
         # except ZeroDivisionError as err:
         #     print(self.unique_id, err)
@@ -391,38 +397,32 @@
 
         Args:
             None
         Returns:
             (:obj:`float`):  contagion risk a value within the inclusive range [0,0.9]
         """
         posns_list = self.model.grid.get_neighborhood(
-            self.pos,
-            moore = False,
-            include_center = False,
-            radius = 1)
+            self.pos, moore=False, include_center=False, radius=1
+        )
         neighboors = self.model.grid.get_cell_list_contents(posns_list)
         count_neighboors = len(neighboors)
-        if count_neighboors == 0: return 0
+        if count_neighboors == 0:
+            return 0
 
         contagion_risk = 0
         for atree in neighboors:
             contagion_risk += atree.dieback
         if count_neighboors > 4:
             contagion_risk /= count_neighboors
         else:
             contagion_risk /= 4
-        #TODO: 0.9 is an adjustment parameter that needs calibration.
+        # TODO: 0.9 is an adjustment parameter that needs calibration.
         return 0.9 * contagion_risk
- 
-  
-    def check_dieback(
-            self,
-            stochastic=True,
-            risk_rate=0.005,
-            healing_rate=0.005):
+
+    def check_dieback(self, stochastic=True, risk_rate=0.005, healing_rate=0.005):
         """The dieback calculation for the tree. It is a path dependent.
         A 'random walk' from latest state is considered. The new rate is drawn from
         a uniform distribution between -1 * healing_rate and risk_rate. A tree with
         a dieback ratio 1 can not recover.
 
         Args:
             risk_rate: (:obj:`float`): A mean risk rate used to draw a random dieback ratio.
@@ -432,17 +432,18 @@
         Returns:
             (:obj:`float`): dieback ratio.
 
         Todo:
             Update the data either using measured dieback for species or
             a site/species specific distribution function.
         """
+
         def register_death():
             self.dieback = 1.0
-            self.condition = 'dead'
+            self.condition = "dead"
 
         # The dieback model below is based on Nowak et al (1986, 2002b:p13)
         # Mortality rate:
         #  100% for dead trees
         #  1.96% for good-excellent and DBH < 3inches
         #  1.46% for good-excellent and DBH > 3inches
         #  3.32% for fair condition
@@ -455,54 +456,62 @@
         elif self.model.maintenance_scope > 1:
             dr = 1
         else:
             dr = 4
 
         if self.dieback >= 1:
             register_death()
-        elif self.condition == 'dead':
+        elif self.condition == "dead":
             register_death()
-        elif self.condition in ('good', 'excellent') and self.dbh < 7.62 and risk <= 0.0196 * dr:
+        elif (
+            self.condition in ("good", "excellent")
+            and self.dbh < 7.62
+            and risk <= 0.0196 * dr
+        ):
             register_death()
-        elif self.condition in ('good', 'excellent') and self.dbh >= 7.62 and risk <= 0.0146 * dr:
+        elif (
+            self.condition in ("good", "excellent")
+            and self.dbh >= 7.62
+            and risk <= 0.0146 * dr
+        ):
             register_death()
-        elif self.condition == 'fair' and risk <= 0.0332 * dr:
+        elif self.condition == "fair" and risk <= 0.0332 * dr:
             register_death()
-        elif self.condition == 'poor' and risk <= 0.0886 * dr:
+        elif self.condition == "poor" and risk <= 0.0886 * dr:
             register_death()
-        elif self.condition == 'critical' and risk <= 0.1308 * dr:
+        elif self.condition == "critical" and risk <= 0.1308 * dr:
             register_death()
-        elif self.condition == 'dying' and risk <= min(0.9, 0.5 * dr):
+        elif self.condition == "dying" and risk <= min(0.9, 0.5 * dr):
             register_death()
         else:
             # The dieback model below is path dependent and depends on
-            # (i) the latest condition of the tree, 
-            # (ii) the age via DBH and  
+            # (i) the latest condition of the tree,
+            # (ii) the age via DBH and
             # (iii) the health of neighboring trees.
-            # the new rate is drawn from a 
+            # the new rate is drawn from a
             # uniform distribution between -1 * healing_rate and risk_rate.
             if stochastic:
                 contagion_risk = self.compute_contagion_risk()
-                #multiplier = Tree.condition_multiplier[self.condition] * np.sqrt(self.dbh)
-                if self.condition == 'excellent':
+                # multiplier = Tree.condition_multiplier[self.condition] * np.sqrt(self.dbh)
+                if self.condition == "excellent":
                     if np.random.uniform(0, 1) < 0.5:
                         self.dieback -= 0.001
                     else:
                         self.dieback += 0.001
-                elif self.condition == 'good':
+                elif self.condition == "good":
                     if np.random.uniform(0, 1) < 0.5:
                         self.dieback -= 0.005
                     else:
                         self.dieback += 0.005
                 else:
                     multiplier = (1 - contagion_risk) * np.sqrt(self.dbh) / dr
                     if multiplier > 0.01:
                         heal_range = -1 * multiplier * healing_rate
                         die_range = risk_rate / multiplier
-                        #die_range = risk_rate
+                        # die_range = risk_rate
                         self.dieback += np.random.uniform(heal_range, die_range)
                 self.dieback = min(1, self.dieback)
                 self.dieback = max(0, self.dieback)
                 self.condition = self._get_condition_class(self.dieback)
         return self.dieback
 
     def _get_condition_class(self, dieback):
@@ -515,27 +524,27 @@
             (:obj:`str`): condition class.
 
         Note:
              The class brackets are based on Nowak 2002b.
         """
 
         if dieback < 0.01:
-            condition = 'excellent'
+            condition = "excellent"
         elif dieback <= 0.10:
-            condition = 'good'
+            condition = "good"
         elif dieback <= 0.25:
-            condition = 'fair'
+            condition = "fair"
         elif dieback <= 0.50:
-            condition = 'poor'
+            condition = "poor"
         elif dieback <= 0.75:
-            condition = 'critical'
+            condition = "critical"
         elif dieback <= 0.99:
-            condition = 'dying'
+            condition = "dying"
         else:
-            condition = 'dead'
+            condition = "dead"
         self.condition = condition
         return condition
 
     def _estimate_dieback(self, condition):
         """Draws a crown dieback ratio based on the condition class.
 
         Args:
@@ -544,25 +553,25 @@
         Returns:
             (:obj:`str`): (:obj:`float`): percent crown lost.
 
         Note:
              This is used when percent crown data is missing but condition of
              of a tree is given a qualitatively. Condition class brackets are based on Nowak 2002b.
         """
-        if condition == 'excellent':
+        if condition == "excellent":
             self.dieback = np.random.uniform(0, 0.01)
-        elif condition == 'good':
+        elif condition == "good":
             self.dieback = np.random.uniform(0.01, 0.11)
-        elif condition == 'fair':
+        elif condition == "fair":
             dieback = np.random.uniform(0.11, 0.26)
-        elif condition == 'poor':
+        elif condition == "poor":
             self.dieback = np.random.uniform(0.26, 0.51)
-        elif condition == 'critical':
+        elif condition == "critical":
             self.dieback = np.random.uniform(0.51, 0.76)
-        elif condition == 'dying':
+        elif condition == "dying":
             self.dieback = np.random.uniform(0.76, 0.99)
         else:
             self.dieback = 1.0
         return self.dieback
 
     def compute_biomass(self, ignore_height=True) -> float:
         """The biomass calculation for the tree, in KG.
@@ -577,15 +586,15 @@
         Todo:
             Update the generic biomass.
 
         """
         self.biomass = self.f_biomass(self.dbh)
         carbon_estimate = self.biomass * Tree.carbon_coeff
         if carbon_estimate > Tree.carbon_storage_cap:
-            #self.biomass = (1 / Tree.carbon_coeff) * Tree.carbon_storage_cap
+            # self.biomass = (1 / Tree.carbon_coeff) * Tree.carbon_storage_cap
             self.biomass = Tree.carbon_storage_cap
         return self.biomass
 
     def _reset_release_track(self):
         """The resetting state variables that is being observed by data collectors.
 
         Args:
@@ -612,15 +621,15 @@
         Todo:
             This module on carbon release from alive trees due to partial diebacks or
             crown loss needs to be revised.
         """
 
         # self.release = self.decomposition_rate * self.dieback * self.carbon_storage
         self._reset_release_track()
-        if self.condition == 'dead':
+        if self.condition == "dead":
             self._compute_decomposition_dead()
             return
         # the tree is alive
         self._compute_decomposition_alive()
 
     def _compute_decomposition_alive(self):
         """The amount of carbon release in KG due to partial diebacks.
@@ -705,45 +714,41 @@
 
         carbon_storage_lag = self.carbon_storage
         carbon_estimate = self.biomass * Tree.carbon_coeff
         # min() function prevents carbon storage from over estimation for very
         # large trees
         self.carbon_storage = min(carbon_estimate, Tree.carbon_storage_cap)
 
-        if (carbon_estimate >= Tree.carbon_storage_cap):
+        if carbon_estimate >= Tree.carbon_storage_cap:
             self.annual_gross_carbon_sequestration = Tree.sequestration_at_maturity
             return self.annual_gross_carbon_sequestration
 
         sequestration = self.carbon_storage - carbon_storage_lag
         # Double check and raise a warning message here.
         if sequestration < 0:
             sequestration = Tree.sequestration_at_maturity
             self.carbon_storage = carbon_storage_lag
 
         self.annual_gross_carbon_sequestration = sequestration
         return self.annual_gross_carbon_sequestration
 
     def replace(self) -> int:
-        """ In case of a maintenance project in place a new young tree or sapling is planted
+        """In case of a maintenance project in place a new young tree or sapling is planted
         at the location where the tree is dead.
 
         Args:
             None
         Returns:
             (:obj:`int`): new agent id.
 
         """
-        self.condition = 'replaced'
+        self.condition = "replaced"
 
         # Replacing with the site specific minimum sapling.
-        dbh = np.random.uniform(self.model.sapling_dbh, self.model.sapling_dbh+1)
+        dbh = np.random.uniform(self.model.sapling_dbh, self.model.sapling_dbh + 1)
         id = self.model.next_id()
         new_tree = Tree(
-            id,
-            self.model,
-            dbh,
-            self.species,
-            condition='excellent',
-            dieback=0)
+            id, self.model, dbh, self.species, condition="excellent", dieback=0
+        )
         self.model.grid.place_agent(new_tree, self.pos)
         self.model.schedule.add(new_tree)
         return id
```

### Comparing `pygus-0.1.9/src/gus/allometrics.py` & `pygus-1.0/pygus/gus/allometrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Importing Python Libraries
 import numpy as np
 import json
 from fuzzywuzzy import process
 
 
-class Species():
+class Species:
     """Object that holds standard tree growth rate by species at different sites.
     Source: https://database.itreetools.org/#/speciesSearch
 
     Todo:
         Consider to convert this into a db or API.
     """
 
@@ -39,15 +39,15 @@
             species: (:obj:`string`): name of the species in 'genusName_speciesName' format. Ex
             'picea_abies'. Use the iTree naming scheme: https://database.itreetools.org/#/speciesSearch
 
         Returns:
             (:obj:`float`): the standard growth per year in cm.
         """
         if species in self.parameters.keys():
-            return self.parameters[species]['diameter_growth']
+            return self.parameters[species]["diameter_growth"]
         else:
             # Return moderate growth rate.
             return 0.8382
 
     def get_height_at_maturity(self, species):
         """Observed avg total height of the tree for the given species.
 
@@ -55,15 +55,15 @@
             species: (:obj:`string`): name of the species in 'genusName_speciesName' format. Ex
             'picea_abies'. Use the iTree naming scheme: https://database.itreetools.org/#/speciesSearch
 
         Returns:
             (:obj:`int`): Avg height in meters.
         """
         if species in self.parameters.keys():
-            return self.parameters[species]['height_at_maturity']
+            return self.parameters[species]["height_at_maturity"]
         else:
             # Return moderate growth rate.
             return 25
 
     def list_species(self):
         """List existing species whose carbon related parameters exist within the library.
 
@@ -72,145 +72,155 @@
 
         Returns:
             (:obj:`list` of `String`): List of species names.
         """
         return list(self.parameters.keys())
 
     def fuzzymatching(self, species):
-        """ Fuzzy matching species name.
+        """Fuzzy matching species name.
 
         Args:
             species: (:obj:`string`): name of the species
 
         Returns:
             (:obj:`string`): Species name in 'genusName_speciesName' format
             that has highest matching score.
 
         Note:
             If the best matching has a poor score (<10% similarity) then
             betula_pendula is passed on as default.
         """
         highest, score = process.extractOne(species, self.list_species())
         if score < 10:
-            highest = 'betula_pendula'
+            highest = "betula_pendula"
         return highest
 
     def get_eqn(self, species_name, allometry_type):
-        """ The method retrieves parameters of a given growth function
+        """The method retrieves parameters of a given growth function
         and sets its constant paramters and returns a function to be used
         by the tree agents.
 
         Args:
             species_name: (:obj:`string`): name of the species
             allometry_type: (:obj:`string`): type of of growth can be height, canopy_width
                 canopy_height.
 
         Returns:
             (:obj:`f(string)->float`): the growth function
 
         """
-        eq_type, params = self.get_form_and_constants(
-            species_name, allometry_type)
-        if eq_type == 'exponential':
+        eq_type, params = self.get_form_and_constants(species_name, allometry_type)
+        if eq_type == "exponential":
             return Species.fit_exponential(params)
-        elif eq_type == 'polynomial':
+        elif eq_type == "polynomial":
             return Species.fit_polynomial(params)
-        elif eq_type == 'parametric':
+        elif eq_type == "parametric":
             return Species.fit_parametric(params)
         else:
-            raise NameError('Equation {} for {} type is not implemented.'.format(
-                eq_type, allometry_type))
+            raise NameError(
+                "Equation {} for {} type is not implemented.".format(
+                    eq_type, allometry_type
+                )
+            )
 
     def get_eqn_biomass(self, species_name):
-        """ The method retrieves constants of a bimomass function for the given species
-        and returns the species specific function. 
+        """The method retrieves constants of a bimomass function for the given species
+        and returns the species specific function.
 
         Args:
             species_name: (:obj:`string`): name of the species
 
         Returns:
             (:obj:`f(string)->float`): the biomass function
 
         Note:
-            Refactoring note: Consider to re implement this by the generic function above. 
+            Refactoring note: Consider to re implement this by the generic function above.
         """
-        eq_type, params = self.get_form_and_constants(species_name, 'biomass')
-        A = params['A']
-        B = params['B']
-        C = params['C']
-        if eq_type == 'mass_1':
-            return lambda dbh: 1.0 * (np.e ** (A + B * np.log(dbh) + C / 2)) / (1 - Species.root_to_shoot_ratio)
-        elif eq_type == 'mass_2':
-            return lambda dbh: 1.0 * (A * pow(dbh, B + C)) / (1 - Species.root_to_shoot_ratio)
+        eq_type, params = self.get_form_and_constants(species_name, "biomass")
+        A = params["A"]
+        B = params["B"]
+        C = params["C"]
+        if eq_type == "mass_1":
+            return (
+                lambda dbh: 1.0
+                * (np.e ** (A + B * np.log(dbh) + C / 2))
+                / (1 - Species.root_to_shoot_ratio)
+            )
+        elif eq_type == "mass_2":
+            return (
+                lambda dbh: 1.0
+                * (A * pow(dbh, B + C))
+                / (1 - Species.root_to_shoot_ratio)
+            )
 
     def get_form_and_constants(self, species_name, allometry_type):
-        """ The method retrieves parameters and type of a growth function for
+        """The method retrieves parameters and type of a growth function for
         the given species.
 
         Args:
             species_name: (:obj:`string`): name of the species
             allometry_type: (:obj:`string`): type of of growth can be height, canopy_width
                 canopy_height.
 
         Returns:
             (:obj:`(string, dict`)
         """
-        form = self.parameters[species_name]['equations'][allometry_type]['equation_type']
-        params = self.parameters[species_name]['equations'][allometry_type]['params']
+        form = self.parameters[species_name]["equations"][allometry_type][
+            "equation_type"
+        ]
+        params = self.parameters[species_name]["equations"][allometry_type]["params"]
         return (form, params)
 
     @staticmethod
     def filter_dbh_size(dbh, minv, maxv):
-        """Utility function to assure the range of dbh that can be used by the growth functions
-        """
+        """Utility function to assure the range of dbh that can be used by the growth functions"""
         # converting the dbh in cm into inche
         dbh = max(minv, 0.393700787 * dbh)
         return min(maxv, dbh)
 
     @staticmethod
     def fit_polynomial(params):
-        """Static method that sets the constant of a second degree polynomial function.
-        """
-        B0 = params['B0']
-        B1 = params['B1']
-        B2 = params['B2']
-        DBHMin = params['DBHMin']
-        DBHMax = params['DBHMax']
+        """Static method that sets the constant of a second degree polynomial function."""
+        B0 = params["B0"]
+        B1 = params["B1"]
+        B2 = params["B2"]
+        DBHMin = params["DBHMin"]
+        DBHMax = params["DBHMax"]
 
         def fit_pol(dbh):
             # converting the dbh in cm into inche
             dbh = min(DBHMax, max(DBHMin, 0.393700787 * dbh))
             estimate = B0 + (B1 * dbh) + (B2 * dbh * dbh)
             # converting into meters
             return max(0, 0.3048 * estimate)
+
         return fit_pol
 
     @staticmethod
     def fit_exponential(params):
-        """Static method that sets the constant of the exponential function.
-        """
-        B0 = params['B0']
-        B1 = params['B1']
-        DBHMin = params['DBHMin']
-        DBHMax = params['DBHMax']
+        """Static method that sets the constant of the exponential function."""
+        B0 = params["B0"]
+        B1 = params["B1"]
+        DBHMin = params["DBHMin"]
+        DBHMax = params["DBHMax"]
 
         def fit_exp(dbh):
             # converting the dbh in cm into inche
             dbh = min(DBHMax, max(DBHMin, 0.393700787 * dbh))
             estimate = np.exp(B0 + B1 * np.log(dbh))
             # converting into meters
             return max(0, 0.3048 * estimate)
+
         return fit_exp
 
     @staticmethod
     def fit_parametric(params):
-        """Static method that sets the constant of the exponential function.
-        """
-        B0 = params['B0']
-        B1 = params['B1']
-        B2 = params['B2']
+        """Static method that sets the constant of the exponential function."""
+        B0 = params["B0"]
+        B1 = params["B1"]
+        B2 = params["B2"]
 
         def fit_parametric(dbh):
-            estimate = B0 + B1 * (dbh ** B2)
+            estimate = B0 + B1 * (dbh**B2)
             return max(0, estimate)
 
         return fit_parametric
```

### Comparing `pygus-0.1.9/src/gus/inputs/allometrics.json` & `pygus-1.0/pygus/gus/inputs/allometrics.json`

 * *Files identical despite different names*

### Comparing `pygus-0.1.9/src/gus/inputs/trees.csv` & `pygus-1.0/pygus/gus/inputs/trees.csv`

 * *Files identical despite different names*

### Comparing `pygus-0.1.9/src/gus/models.py` & `pygus-1.0/pygus/gus/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,180 +15,172 @@
 from mesa.datacollection import DataCollector
 
 # Importing needed GUS objects
 from .agents import Tree
 from .allometrics import Species
 from .weather import WeatherSim
 
+
 class Urban(Model):
-    """A generic urban green space model. To be tailored according to specific sites.
-    """
-    # Used to hold the scaling of actual physical space within the digital space. 
+    """A generic urban green space model. To be tailored according to specific sites."""
+
+    # Used to hold the scaling of actual physical space within the digital space.
     # It shows the size of each cell (square) in meters.
     # TODO: this needs to be brought up as a parameter and placed within the groups
-    #      of parameters that handle physical to digital twin mapping.  
-    dt_resolution = 2 #in meters
+    #      of parameters that handle physical to digital twin mapping.
+    dt_resolution = 2  # in meters
 
-    site_types = ['park','street','forest','pocket']
+    site_types = ["park", "street", "forest", "pocket"]
 
-    def __init__(self,
-        population,
-        species_composition,
-        site_config,
-        scenario,
-        batch=False):
+    def __init__(
+        self, population, species_composition, site_config, scenario, batch=False
+    ):
         """The constructor method.
 
         Args:
             population: (:obj:`pd.DataFrame`): A dataframe tree properties are read from a site.
-            species_composition (:obj:`str`): The name of the file that keeps allometrics of the tree species for the site. 
+            species_composition (:obj:`str`): The name of the file that keeps allometrics of the tree species for the site.
             site_config: (:obj:`string`): name of the json file.
             scenario: (:obj:`dict`): Python dictionary that holds experiment parameters.
             batch: (:obj:`bool`): Mesa parameter to control single vs batch runs.
         Returns:
             None
 
         Note:
             First release model.
 
         Todo:
-            Check for hard coded constants and parameterize further.  
+            Check for hard coded constants and parameterize further.
         """
         super().__init__()
         # Setting MESA specific parameters
         width = int(max(population.xpos)) + 1
-        height = int(max(population.ypos)) + 1
-        self.grid = MultiGrid(width, height, torus=False)
-                # to be parameterized and set during initialization.
+        length = int(max(population.ypos)) + 1
+        self.grid = MultiGrid(width, length, torus=False)
+        # to be parameterized and set during initialization.
         self.schedule = RandomActivation(self)
-        
+
         self._load_site_parameters(site_config)
         self._load_experiment_parameters(scenario)
 
         # Load species composition and their allometrics
         self.species = Species(species_composition)  # will be used by agents.
-    
+
         # Test that the df is complete or raise keyerror
-        for attribute in ['dbh', 'species', 'condition', 'xpos', 'ypos']:
+        for attribute in ["dbh", "species", "condition", "xpos", "ypos"]:
             population[attribute]
 
         # copy and import df
         self.df = population
         self.num_agents = len(population)
         self.sapling_dbh = min(population.dbh)
         # Each entry index i, represents number of years since the biomass is decay period.
-        self.release_bins = {'slow': np.zeros(10),  # for dead root and standing tree.
-                             'fast': np.zeros(10)  # for mulched biomass
-                             }
+        self.release_bins = {
+            "slow": np.zeros(10),  # for dead root and standing tree.
+            "fast": np.zeros(10),  # for mulched biomass
+        }
 
         # Create agents.
         for index, row in self.df.iterrows():
             # Tree init
-            a = Tree(row.id, self,
-                     dbh=row.dbh,
-                     species=row.species,
-                     condition=row.condition)
+            a = Tree(
+                row.id, self, dbh=row.dbh, species=row.species, condition=row.condition
+            )
             self.schedule.add(a)
 
             # Place trees on the plot sequentially
             # based on their id/index.
             # TODO: This snippet may need to be converted into a function as part of
             # initilisartion module and x,y points need to be part of input DB.
-            #x = int(index % self.grid.width)
-            #y = int(index / self.grid.height)
+            # x = int(index % self.grid.width)
+            # y = int(index / self.grid.height)
 
             # # Add the agent to a random grid cell
-            #x = self.random.randrange(self.grid.width)
-            #y = self.random.randrange(self.grid.height)
+            # x = self.random.randrange(self.grid.width)
+            # y = self.random.randrange(self.grid.height)
 
             # # Locate the trees based on actual physical positioning
             x = row.xpos
             y = row.ypos
             self.grid.place_agent(a, (x, y))
 
         # This variable below works as an indexer while adding new trees to the population during the run time.
         self.current_id = max(population.id)
 
         # Collecting model and agent level data
         self.datacollector = DataCollector(
             model_reporters={
-                "Storage": lambda m: self.aggregate(
-                    m,
-                    'carbon_storage'),
-                "Seq": lambda m: self.aggregate(
-                    m,
-                    'annual_gross_carbon_sequestration'),
+                "Storage": lambda m: self.aggregate(m, "carbon_storage"),
+                "Seq": lambda m: self.aggregate(m, "annual_gross_carbon_sequestration"),
                 # "Sequestrated": self.aggregate_sequestration,
                 "Released": self.compute_current_carbon_release,
                 "Alive": lambda m: self.count(
                     m,
-                    'condition',
-                    lambda x: x in ['excellent', 'good', 'fair', 'poor', 'critical', 'dying']),
-                "Dead": lambda m: self.count(
-                    m,
-                    'condition',
-                    lambda x: x == 'dead'),
+                    "condition",
+                    lambda x: x
+                    in ["excellent", "good", "fair", "poor", "critical", "dying"],
+                ),
+                "Dead": lambda m: self.count(m, "condition", lambda x: x == "dead"),
                 "Critical": lambda m: self.count(
-                    m,
-                    'condition',
-                    lambda x: x == 'critical'),
-                "Dying": lambda m: self.count(
-                    m,
-                    'condition',
-                    lambda x: x == 'dying'),
-                "Poor": lambda m: self.count(
-                    m,
-                    'condition',
-                    lambda x: x == 'poor'),
+                    m, "condition", lambda x: x == "critical"
+                ),
+                "Dying": lambda m: self.count(m, "condition", lambda x: x == "dying"),
+                "Poor": lambda m: self.count(m, "condition", lambda x: x == "poor"),
                 "Replaced": lambda m: self.count(
-                    m,
-                    'condition',
-                    lambda x: x == 'replaced'),
+                    m, "condition", lambda x: x == "replaced"
+                ),
                 "Seq_std": self.agg_std_sequestration,
             },
             agent_reporters={
-                "species": 'species',
-                "dbh": 'dbh',
-                "height": 'tree_height',
-                "crownH": 'crown_height',
-                "crownW": 'crown_width',
+                "species": "species",
+                "dbh": "dbh",
+                "height": "tree_height",
+                "crownH": "crown_height",
+                "crownW": "crown_width",
                 "canopy_overlap": "overlap_ratio",
                 "cle": "cle",
-                "condition": 'condition',
-                "dieback": 'dieback',
-                "biomass": 'biomass',
-                "seq": 'annual_gross_carbon_sequestration',
+                "condition": "condition",
+                "dieback": "dieback",
+                "biomass": "biomass",
+                "seq": "annual_gross_carbon_sequestration",
                 "carbon": "carbon_storage",
-                "deroot": 'decomposing_root',
-                "detrunk": 'decomposing_trunk',
-                "mulched": 'mulched',
-                "burnt": 'immediate_release',
-                "coordinates": 'pos',})
-        logging.info("Initialisation of the Digital Twins of {} trees on a {} by {} digital space is complete!".format(self.num_agents,width,height))
+                "deroot": "decomposing_root",
+                "detrunk": "decomposing_trunk",
+                "mulched": "mulched",
+                "burnt": "immediate_release",
+                "coordinates": "pos",
+            },
+        )
+        logging.info(
+            "Initialisation of the Digital Twins of {} trees on a {} by {} digital space is complete!".format(
+                self.num_agents, width, length
+            )
+        )
 
     def step(self):
         """Customized MESA method that sets the major components of scenario analyses process.
 
         Args:
             None
 
         Returns:
             None
 
         Note:
+            None
 
         Todo:
-
+            None
         """
         logging.info("Year:{}".format(self.schedule.time + 1))
         self.get_weather_projection()
 
         logging.info("Agents are working ...")
         self.schedule.step()
-        
+
         logging.info("Yearly data is being collected ...")
         self.datacollector.collect(self)
         # print('Step:{}'.format(self.schedule.time))
         # print(self.release_bins['slow'])
         # print(self.release_bins['fast'])
 
     def _load_experiment_parameters(self, experiment):
@@ -196,72 +188,84 @@
 
         Args:
             experiment: (:obj:`dict`): Python dictionary that holds experiment parameters.
 
         Returns:
             None
         Todo:
+            None
 
         """
 
         # Read denisty to set the digital twin resolution which is defined as
         # the cell size in terms of actual distance.
-        if 'maintenance_scope' in experiment.keys():
-            #maintenance_scope: (:obj:`int`): It can be 0:None,1:base, 2:cared)
-            self.maintenance_scope = experiment['maintenance_scope']
+        if "maintenance_scope" in experiment.keys():
+            # maintenance_scope: (:obj:`int`): It can be 0:None,1:base, 2:cared)
+            self.maintenance_scope = experiment["maintenance_scope"]
         else:
-            logging.warning("Maintenance scope is not given. A high maintenance site is assumed.")
+            logging.warning(
+                "Maintenance scope is not given. A high maintenance site is assumed."
+            )
             self.maintenance_scope = 2
-        
 
     def _load_site_parameters(self, config_file):
         """Loads site configuration information.
 
         Args:
             config_file: (:obj:`string`): name of the json file.
 
         Returns:
             None
         Todo:
+            None
 
         """
         try:
             f = open(config_file)
         except IOError as e:
             print(str(e))
         params = json.loads(f.read())
-        
-        #read site type
-        stype = 'park' #default type
-        if 'project_site_type' in params.keys():
-            if params['project_site_type'] in Urban.site_types:
-                stype = params['project_site_type']
+
+        # read site type
+        stype = "park"  # default type
+        if "project_site_type" in params.keys():
+            if params["project_site_type"] in Urban.site_types:
+                stype = params["project_site_type"]
             else:
-                logging.warning("Undefined site type recognized. Park type will be used.")
+                logging.warning(
+                    "Undefined site type recognized. Park type will be used."
+                )
         else:
-            logging.warning("Site type is not provided. Park type will be used.")   
+            logging.warning("Site type is not provided. Park type will be used.")
         self.site_type = stype
-        
+
         # Read in growth season mean and variance to be used by weather forecasting module.
         try:
-            self.season_mean = params['weather']['growth_season_mean']
-            self.season_var = params['weather']['growth_season_var']
+            self.season_mean = params["weather"]["growth_season_mean"]
+            self.season_var = params["weather"]["growth_season_var"]
         except KeyError:
             self.season_mean = 153
             self.season_var = 7
-            logging.warning("Tree growth season mean and variance is not provided as expected. Global average is used.")
+            logging.warning(
+                "Tree growth season mean and variance is not provided as expected. Global average is used."
+            )
 
         # Read denisty to set the digital twin resolution which is defined as
         # the cell size in terms of actual distance.
-        if 'area_tree_density_per_hectare' in params.keys():
-            self.dt_resolution = np.sqrt(10000 / params['area_tree_density_per_hectare'])
+        if "area_tree_density_per_hectare" in params.keys():
+            self.dt_resolution = np.sqrt(
+                10000 / params["area_tree_density_per_hectare"]
+            )
             # The distance between the center of two tree trunks in meters. Even spatial distribution is assumed.
         else:
-            logging.warning("area_tree_density_per_hectare is not given the default {} meters is used the distance from the clossest tree trunks.".format(self.dt_resolution)) 
-    
+            logging.warning(
+                "area_tree_density_per_hectare is not given the default {} meters is used the distance from the clossest tree trunks.".format(
+                    self.dt_resolution
+                )
+            )
 
     def get_weather_projection(self):
         """The method retrieves wetaher projection for the current iteration,
         eg. year, at the moment it uses a simulated projections on the go,
         instead previously computed estimates or forecasts can be used as well.
 
         Args:
@@ -279,112 +283,118 @@
         """
         # The avg season length is based on iTree Glasgow estimates (see iTree 2015 report)
         # These variables need to be parameterrized and read-in through site (model) specific
         # initialization module.
         # season_mean = 200
 
         self.WeatherAPI = WeatherSim(
-            season_length=self.season_mean, season_var=self.season_var)
+            season_length=self.season_mean, season_var=self.season_var
+        )
 
     @staticmethod
     def aggregate(model, var, func=lambda x, y: x + y, init=0):
         """A higher order function that aggregates a given variable.
 
         The aggregation function and the initial conditions can be specified.
         """
-        return reduce(func, [eval('a.{}'.format(var))
-                      for a in model.schedule.agents], init)
+        return reduce(
+            func, [eval("a.{}".format(var)) for a in model.schedule.agents], init
+        )
 
     @staticmethod
     def count(model, memory, predicate):
         """A higher order function for counting agents that satisfy a specific attribute."""
         return len(
             list(
                 filter(
-                    predicate, [
-                        eval(
-                            'a.{}'.format(memory)) for a in model.schedule.agents])))
+                    predicate,
+                    [eval("a.{}".format(memory)) for a in model.schedule.agents],
+                )
+            )
+        )
 
     @staticmethod
     def aggregate_sequestration(model):
         """The function that accumulates yearly sequestration data from all trees within the site.
 
         Args:
             model: (:obj:`Urban`): an urban forest model.
 
 
         Returns:
             (:obj:float`): total sequestration in Kg.
         Note:
+            None
         Todo:
+            None
         """
-        captured = [
-            a.annual_gross_carbon_sequestration for a in model.schedule.agents]
+        captured = [a.annual_gross_carbon_sequestration for a in model.schedule.agents]
         return sum(captured)
 
     @staticmethod
     def agg_std_sequestration(model):
         """The function estimates the standard deviation for yearly sequestration data from all trees within the site.
 
         Args:
             model: (:obj:`Urban`): an urban forest model.
 
 
         Returns:
             (:obj:float`): total sequestration in Kg.
         """
-        captured = [
-            a.annual_gross_carbon_sequestration for a in model.schedule.agents]
+        captured = [a.annual_gross_carbon_sequestration for a in model.schedule.agents]
         return np.std(captured)
 
     @staticmethod
     def compute_current_carbon_release(model):
         """The function that accumulates yearly sequestration data from all trees within the site.
 
         Args:
             model: (:obj:`Urban`): an urban forest model.
 
 
         Returns:
             (:obj:float`): total sequestration in Kg.
         Note:
+            None
         Todo:
+            None
         """
         # roll current bins stored as np.array
-        model.release_bins['slow'] = np.roll(model.release_bins['slow'], 1)
-        model.release_bins['fast'] = np.roll(model.release_bins['fast'], 1)
+        model.release_bins["slow"] = np.roll(model.release_bins["slow"], 1)
+        model.release_bins["fast"] = np.roll(model.release_bins["fast"], 1)
 
         # aggregate required type of release (mulched, etc)
-        mulched = Urban.aggregate(model, 'mulched')
-        standing = Urban.aggregate(model, 'decomposing_trunk')
-        root = Urban.aggregate(model, 'decomposing_root')
-        immediate = Urban.aggregate(model, 'immediate_release')
+        mulched = Urban.aggregate(model, "mulched")
+        standing = Urban.aggregate(model, "decomposing_trunk")
+        root = Urban.aggregate(model, "decomposing_root")
+        immediate = Urban.aggregate(model, "immediate_release")
 
         # add new potential releases into release bins
-        model.release_bins['slow'][0] = standing + root
-        model.release_bins['fast'][0] = mulched
+        model.release_bins["slow"][0] = standing + root
+        model.release_bins["fast"][0] = mulched
 
         # compute and aggregate release
         def update_release(type):
             carbon_release = 0
             for i in range(len(model.release_bins[type])):
                 mass = model.release_bins[type][i]
                 rate = Urban.compute_carbon_release_rate(i + 1, type)
                 released = rate * mass
                 carbon_release += released
                 model.release_bins[type][i] -= released
             return carbon_release
 
-        carbon_release_slow = update_release('slow')
-        carbon_release_fast = update_release('fast')
+        carbon_release_slow = update_release("slow")
+        carbon_release_fast = update_release("fast")
 
         return carbon_release_fast + carbon_release_slow + immediate
 
     @staticmethod
-    def compute_carbon_release_rate(year, state='fast'):
+    def compute_carbon_release_rate(year, state="fast"):
         """Determines a carbon release rate.
 
         Args:
 
             year: (:obj:`int`) or (:obj:`float`): time passed since the biomass is dead.
             state: (:obj:`str`): Represents exposure type can be one of ('standing', 'mulched', 'root', 'fast', 'slow',)
 
@@ -403,9 +413,9 @@
             When k = 5, in the first 3 years around 40% is released, which corresponds to
             empirical reports for carbon release for standing dead trees as well as underground roots.
 
             check:
                 import scipy.integrate as integrate
                 integrate.quad(f, 0, 20) > 0.96 for k in (2:5).
         """
-        k = 2 if state in ('mulched', 'fast') else 5
+        k = 2 if state in ("mulched", "fast") else 5
         return 1 / k * np.exp(-1 * year / k)
```

### Comparing `pygus-0.1.9/src/gus/outputs/trees_yearly.json` & `pygus-1.0/pygus/gus/outputs/trees_yearly.json`

 * *Files identical despite different names*

### Comparing `pygus-0.1.9/src/gus/weather.py` & `pygus-1.0/pygus/gus/weather.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 import numpy as np
 
-class WeatherSim():
+
+class WeatherSim:
     """The environment objects that simulates the weather."""
 
     # Yearly mean frost free days at a given site.
     # Source for 153 iTree, Nowak et.al., 2020.
     ffdays_mean = 153
     # Yearly variance in frost free days for a given site.
     ffdays_var = 7
@@ -30,21 +31,22 @@
         if season_length:
             self.ffdays_mean = season_length
         if season_var:
             self.ffdays_var = season_var
 
         # Drawing frost free days for the given year from a normal distriburion
         # where the mean is based on iTree's proxy variable.
-        self.frost_free_days_ref = np.random.normal(
-            self.ffdays_mean, self.ffdays_var)
+        self.frost_free_days_ref = np.random.normal(self.ffdays_mean, self.ffdays_var)
 
     def check_frost_free_days(self):
         """The method generates frost free days based on mean and variance of a given site.
 
         Args:
             None
         Returns:
             (:obj:`int`): Number of frost free days.
         Note:
+            None
         Todo:
+            None
         """
-        return self.frost_free_days_ref
+        return self.frost_free_days_ref
```

### Comparing `pygus-0.1.9/src/impacts/carbon.py` & `pygus-1.0/pygus/impacts/carbon.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,76 +1,77 @@
 # -*- coding: utf-8 -*-
 
 # Carbon storage estimation.
 
 from ..gus.allometrics import Species
 
-class Carbon():
+
+class Carbon:
     """Species specific biomass and carbon storage estimator."""
 
     #  Unit: Kg, Ref: iTree, 2020
     storage_cap = 7500
 
     # The coeff is used to estimate carbon storage through biomass.
     # The stock of carbon is estimated by multiplying tree biomass by 0.5 (Chow and Rolfe 1989).
     coeff = 0.5
 
     def __init__(self, allometrics, species_name=None):
         """Constructor method.
 
         Args:
-            allometrics (:obj:`str`): The name of the file that keeps allometrics of the tree species for the site. 
+            allometrics (:obj:`str`): The name of the file that keeps allometrics of the tree species for the site.
             species_name: (:obj:`string`): name of the species in 'genusName_speciesName' format.
                 Ex: 'picea_abies'. Use the iTree naming scheme: https://database.itreetools.org/#/speciesSearch
 
         Returns:
             None
         """
-        self.Allometrics = Species(allometrics)      
+        self.Allometrics = Species(allometrics)
         if species_name:
             self.species_name = self.Allometrics.fuzzymatching(species_name)
-            self.f_biomass =self.Allometrics.get_eqn_biomass(species_name)
+            self.f_biomass = self.Allometrics.get_eqn_biomass(species_name)
 
-    def compute_carbon_storage(self, dbh, species_name = 'decidu', height=None) -> float:
+    def compute_carbon_storage(self, dbh, species_name="decidu", height=None) -> float:
         """The carbon storage calculation for a tree, in KG.
 
         Args:
             dbh: (:obj:`float`): the DBH measure which is diameter in cm of the trunk usually measured at 1.3m from the ground.
             species_name: (:obj:`string`): name of the species in 'genusName_speciesName' format.
                 Ex: 'picea_abies'. Use the iTree naming scheme: https://database.itreetools.org/#/speciesSearch
             height: (:obj:`float`): The tree height in meters.
 
         Returns:
             (:obj:`float`): Carbon in Kg.
-        
+
         TODO:
             Update the method to allow receive the height data and use the allometric equations
             with height parameter.
 
         """
         # Load species composition and their allometrics
         self.species_name = self.Allometrics.fuzzymatching(species_name)
-        self.f_biomass =self.Allometrics.get_eqn_biomass(species_name)
+        self.f_biomass = self.Allometrics.get_eqn_biomass(species_name)
         biomass = self.f_biomass(dbh)
         carbon_estimate = biomass * Carbon.coeff
         # min() function prevents carbon storage from over estimation for very large trees
         carbon_storage = min(carbon_estimate, Carbon.storage_cap)
         return carbon_storage
 
-    def compute_biomass(self, dbh, species_name = 'decidu', height=None) -> float:
+    def compute_biomass(self, dbh, species_name="decidu", height=None) -> float:
         """The carbon storage calculation for a tree, in KG.
 
         Args:
             species_name: (:obj:`string`): name of the species in 'genusName_speciesName' format.
                     Ex: 'picea_abies'. Use the iTree naming scheme: https://database.itreetools.org/#/speciesSearch
             dbh: (:obj:`float`): the DBH measure which is diameter in cm of the trunk usually measured at 1.3m from the ground.
             height: (:obj:`float`): The tree height in meters.
 
         Returns:
             (:obj:`float`): Carbon in Kg.
 
         TODO:
-            Convert and extend this into carbon estimation object. 
+            Convert and extend this into carbon estimation object.
 
         """
         carbon_estimate = self.compute_carbon_storage(dbh, species_name)
         return carbon_estimate / Carbon.coeff
```

### Comparing `pygus-0.1.9/src/impacts/water.py` & `pygus-1.0/pygus/impacts/water.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 import numpy as np
 from scipy import stats
 
 # Time series operations
 import glob
 from datetime import datetime
 
-class Calibration():
+
+class Calibration:
     """Water retention and impact estimate related parameters setting."""
+
     # Conversion coefficient meter to millimeter
     m_to_mm = 1
 
     # Extinction coefficient =0.7 for trees and 0.3 for shrubs (Wang et al. 2008)
     kappa = 0.7
 
     # Shade factor, is the percentage of sky covered by foliage and branches within
@@ -36,71 +38,78 @@
     maximum_impervious_cover_storage = 0.0015 * m_to_mm
 
     # Specific pervious cover storage of water (=0.001 m).
     maximum_pervious_cover_storage = 0.001 * m_to_mm
 
     def __init__(
         self,
-        leaf_transition_days = 28,
-        leaf_storage = 0.0002,
-        pervios_storage_max = 0.0010,
-        impervios_storage_max = 0.0015
-        ):
+        leaf_transition_days=28,
+        leaf_storage=0.0002,
+        pervios_storage_max=0.0010,
+        impervios_storage_max=0.0015,
+    ):
         """The constructor method.
 
         Args:
             leaf_transition_days: (:obj:`int`): Leaf-on leaf_off transition days
             leaf_storage: (:obj:`float`): Specific leaf storage of water.
             pervios_storage_max: (:obj:`float`): Specific pervious cover storage of water
             impervios_storage_max: (:obj:`float`): Specific impervious cover storage of water
         Returns:
             None
         Note:
+            None
 
         TODO:
             * pass optional settings as key word parameters.
         """
         self.leaf_storage = leaf_storage * Calibration.m_to_mm
         self.leaf_transition_days = leaf_transition_days
-        self.maximum_impervious_cover_storage = impervios_storage_max * Calibration.m_to_mm
+        self.maximum_impervious_cover_storage = (
+            impervios_storage_max * Calibration.m_to_mm
+        )
         self.maximum_pervious_cover_storage = pervios_storage_max * Calibration.m_to_mm
 
     def set_surface_storage_rates(
-        self, leaf_storage=None,
-        pervios_storage_max=None,
-        impervios_storage_max=None):
-        """Setting specific water storage rates. 
+        self, leaf_storage=None, pervios_storage_max=None, impervios_storage_max=None
+    ):
+        """Setting specific water storage rates.
 
         Args:
             leaf_storage: (:obj:`float`): Specific leaf storage of water.
             pervios_storage_max: (:obj:`float`): Specific pervious cover storage of water
             impervios_storage_max: (:obj:`float`): Specific impervious cover storage of water
         Returns:
             None
         Note:
-
+            None
         Todo:
-
+            None
         """
         if leaf_storage:
             self.leaf_storage = leaf_storage * Calibration.m_to_mm
         if impervios_storage_max:
-            self.maximum_impervious_cover_storage = impervios_storage_max * Calibration.m_to_mm
+            self.maximum_impervious_cover_storage = (
+                impervios_storage_max * Calibration.m_to_mm
+            )
         if pervios_storage_max:
-            self.maximum_pervious_cover_storage = pervios_storage_max * Calibration.m_to_mm
-    
+            self.maximum_pervious_cover_storage = (
+                pervios_storage_max * Calibration.m_to_mm
+            )
+
 
 def compute_leaf_area_index(
     dbh,
     tree_height,
     crown_height,
     crown_width,
-    crown_missing = 0,
-    shade_factor = Calibration.avg_shade_factor):
-    """The function given allometrics of a tree computes its leaf, bark and plant area indices. 
+    crown_missing=0,
+    shade_factor=Calibration.avg_shade_factor,
+):
+    """The function given allometrics of a tree computes its leaf, bark and plant area indices.
 
     Args:
         dbh: (:obj:`float`): the diameter in cm of the trunk usually measured at 1.3m from the ground.
         tree_height: (:obj:`float`): The tree height in meters.
         crown_height: (:obj:`float`): The vertical length of tree crown in meters.
         crown_width: (:obj:`float`): The horizontal length (diameter) of tree crown in meters.
         crown_missing: (:obj:`float`): The percentage loss of the crown.
@@ -122,415 +131,553 @@
     beta_0 = -4.3309
     beta_1 = 0.2942
     beta_2 = 0.7312
     beta_3 = 5.7217
     beta_4 = 0.0148
 
     def compute_under_canopy_area(crown_width):
-        return pow((crown_width/2),2) * np.pi
-    
+        return pow((crown_width / 2), 2) * np.pi
+
     def compute_bark_area(dbh, tree_height, crown_height):
         # * 0.01 converts DBH(cm) into meter.
         return np.pi * (dbh * 0.01) * (tree_height - crown_height)
 
     # Outer surface area estimate below is based on Gacka-Grzesikiewicz (1980).
     under_canopy = compute_under_canopy_area(cw)
-    crown_surface = np.pi  * crown_width * (crown_height + crown_width)/2
-    bark_area = compute_bark_area(dbh,th,ch)
-    leaf_area = (1-loss) * np.exp(beta_0 + beta_1 * th + beta_2 * cw + beta_3 * sf - beta_4 * crown_surface)
+    crown_surface = np.pi * crown_width * (crown_height + crown_width) / 2
+    bark_area = compute_bark_area(dbh, th, ch)
+    leaf_area = (1 - loss) * np.exp(
+        beta_0 + beta_1 * th + beta_2 * cw + beta_3 * sf - beta_4 * crown_surface
+    )
     leaf_area_index = leaf_area / under_canopy
     bark_area_index = bark_area / under_canopy
     plant_area_index = leaf_area_index + bark_area_index
     return (leaf_area_index, bark_area_index, plant_area_index)
 
 
 def pai_seasons(x, leaf_on_start, leaf_off_start, leaf_transition_days):
     """The method updates Plant Area Index (PAI) with respect to leaf on-off seasons.
 
     Args:
         A data frame "x" with following variables:
         Date_time: (:obj:`time`): date and time
         BAI: Bark Area Index
         LAI: Leaf Area Index
-        conifers: it taks value "true" if conifers and "false" otherwise 
-        
+        conifers: it taks value "true" if conifers and "false" otherwise
+
         leaf_on_start: a day in the year when the leaf on season starts. In the case of Glasgow it is April 14 (day 105).
                         See also other sources: https://weatherspark.com/y/147740/Average-Weather-at-Glasgow-Airport-United-Kingdom-Year-Round
         leaf_off_start: a day in the year when the leaf off season starts. In the case of Glasgow it is November 2 (day 307).
         leaf_transition_days: the number of days that the leaf on-off transition last.
-        
+
 
     Returns:
         An array of values of Plant Area Indexes (PAI) over time.
 
     Note:
         The function is built upon the following paper:
-        Wang, Jun, Theodore A. Endreny, and David J. Nowak. “Mechanistic Simulation of Tree 
-        Effects in an Urban Water Balance Model 1.” JAWRA Journal of the American Water Resources 
-        Association 44, no. 1 (February 2008): 75–85. https://doi.org/10.1111/j.1752-1688.2007.00139.x   
-
-    Todo:
-    """
-    x = x.assign(PAI = np.where(x['Conifers'], x['BAI']+x['LAI'],
-                                np.where(x.Date_time.dt.day_of_year < leaf_on_start, x['BAI'],
-                                    np.where(((x.Date_time.dt.day_of_year >= leaf_on_start) & (x.Date_time.dt.day_of_year < leaf_off_start)),
-                                    x['LAI']/(1+np.exp(-0.37*(x.Date_time.dt.day_of_year-(leaf_on_start+leaf_transition_days/2)))) + x['BAI'],
-                                    x['LAI']/(1+np.exp(-0.37*((leaf_off_start+leaf_transition_days/2)-x.Date_time.dt.day_of_year))) + x['BAI'])))
+        Wang, Jun, Theodore A. Endreny, and David J. Nowak. “Mechanistic Simulation of Tree
+        Effects in an Urban Water Balance Model 1.” JAWRA Journal of the American Water Resources
+        Association 44, no. 1 (February 2008): 75–85. https://doi.org/10.1111/j.1752-1688.2007.00139.x
+
+    Todo:
+        None
+    """
+    x = x.assign(
+        PAI=np.where(
+            x["Conifers"],
+            x["BAI"] + x["LAI"],
+            np.where(
+                x.Date_time.dt.day_of_year < leaf_on_start,
+                x["BAI"],
+                np.where(
+                    (
+                        (x.Date_time.dt.day_of_year >= leaf_on_start)
+                        & (x.Date_time.dt.day_of_year < leaf_off_start)
+                    ),
+                    x["LAI"]
+                    / (
+                        1
+                        + np.exp(
+                            -0.37
+                            * (
+                                x.Date_time.dt.day_of_year
+                                - (leaf_on_start + leaf_transition_days / 2)
+                            )
+                        )
+                    )
+                    + x["BAI"],
+                    x["LAI"]
+                    / (
+                        1
+                        + np.exp(
+                            -0.37
+                            * (
+                                (leaf_off_start + leaf_transition_days / 2)
+                                - x.Date_time.dt.day_of_year
+                            )
+                        )
+                    )
+                    + x["BAI"],
+                ),
+            ),
+        )
     )
-    return x['PAI']
+    return x["PAI"]
+
 
 def lmbd(temperature):
     """The method calculates latent heat of vaporization.
 
     Args:
-        Temperature in [C]     
+        Temperature in [C]
 
     Returns:
         latent heat of vaporization in [MJ/Kg]
 
     Note:
         The function is built upon the following book:
             Maidment, David R and others. “Handbook of Hydrology, McGraw-Hil.” Inc., New York, NY, 1992.
-            
+
             And a paper:
-                Hirabayashi, Satoshi. “I-Tree Eco United States County-Based Hydrologic Estimates.” 
-                Washington, DC: US Department of Agriculture, Forest Service, 2015.  
+                Hirabayashi, Satoshi. “I-Tree Eco United States County-Based Hydrologic Estimates.”
+                Washington, DC: US Department of Agriculture, Forest Service, 2015.
 
     Todo:
+        None
     """
-    return 2.501-0.002361*temperature
+    return 2.501 - 0.002361 * temperature
+
 
 def e_s(temperature):
     """The method calculates saturated vapor pressure.
 
     Args:
-        Temperature in [C]   
+        Temperature in [C]
 
     Returns:
         Saturated vapor pressure in [kPa]
 
     Note:
             The function is built upon the following book:
             Maidment, David R and others. “Handbook of Hydrology, McGraw-Hil.” Inc., New York, NY, 1992.
-            
+
             And a paper:
-                Hirabayashi, Satoshi. “I-Tree Eco United States County-Based Hydrologic Estimates.” 
-                Washington, DC: US Department of Agriculture, Forest Service, 2015. 
+                Hirabayashi, Satoshi. “I-Tree Eco United States County-Based Hydrologic Estimates.”
+                Washington, DC: US Department of Agriculture, Forest Service, 2015.
 
     Todo:
+        None
     """
-    return 0.6108*np.exp(17.27*temperature/(237.3+temperature))
+    return 0.6108 * np.exp(17.27 * temperature / (237.3 + temperature))
+
 
 def e(dew_point_temperature):
     """The method calculates vapor pressure.
 
     Args:
-        Dew point temperature in [C]   
+        Dew point temperature in [C]
 
     Returns:
         Vapor pressure in [kPa]
 
     Note:
             The function is built upon the following book:
             Maidment, David R and others. “Handbook of Hydrology, McGraw-Hil.” Inc., New York, NY, 1992.
-            
+
             And a paper:
-                Hirabayashi, Satoshi. “I-Tree Eco United States County-Based Hydrologic Estimates.” 
-                Washington, DC: US Department of Agriculture, Forest Service, 2015. 
+                Hirabayashi, Satoshi. “I-Tree Eco United States County-Based Hydrologic Estimates.”
+                Washington, DC: US Department of Agriculture, Forest Service, 2015.
 
     Todo:
+        None
     """
-    return 0.6108*np.exp(17.27*dew_point_temperature/(237.3+dew_point_temperature))
+    return 0.6108 * np.exp(
+        17.27 * dew_point_temperature / (237.3 + dew_point_temperature)
+    )
+
 
 def DELTA(temperature):
     """The method calculates the slope of vapor pressure temperature curve.
 
     Args:
-        Temperature in [C]   
+        Temperature in [C]
 
     Returns:
         Slope of vapor pressure temperature curve in [kPa/C]
 
     Note:
         It includes in calculation saturated vapor pressure in [kPa] which is calculated with function e_s()!
 
         The function is built upon the following book:
             Maidment, David R and others. “Handbook of Hydrology, McGraw-Hil.” Inc., New York, NY, 1992.
-            
+
             And a paper:
-                Hirabayashi, Satoshi. “I-Tree Eco United States County-Based Hydrologic Estimates.” 
-                Washington, DC: US Department of Agriculture, Forest Service, 2015. 
+                Hirabayashi, Satoshi. “I-Tree Eco United States County-Based Hydrologic Estimates.”
+                Washington, DC: US Department of Agriculture, Forest Service, 2015.
 
     Todo:
+        None
     """
-    return 4098*e_s(temperature)/(237.3+temperature)**2
+    return 4098 * e_s(temperature) / (237.3 + temperature) ** 2
+
 
 def rho_a(temperature, surface_pressure):
     """The method calculates the density of air.
 
     Args:
         Temperature in [C]
-        Surface preasure in [kPa]  
+        Surface preasure in [kPa]
 
     Returns:
         The density of air in [kg/m^3]
 
     Note:
             The function is built upon the following book:
             Maidment, David R and others. “Handbook of Hydrology, McGraw-Hil.” Inc., New York, NY, 1992.
-            
+
             And a paper:
-                Hirabayashi, Satoshi. “I-Tree Eco United States County-Based Hydrologic Estimates.” 
-                Washington, DC: US Department of Agriculture, Forest Service, 2015. 
+                Hirabayashi, Satoshi. “I-Tree Eco United States County-Based Hydrologic Estimates.”
+                Washington, DC: US Department of Agriculture, Forest Service, 2015.
 
     Todo:
+        None
     """
-    return 3.486 * surface_pressure/(275+temperature)
+    return 3.486 * surface_pressure / (275 + temperature)
+
 
 def rho_w(temperature):
     """The method calculates the density of water.
 
     Args:
         Temperature in [C]
 
     Returns:
         The density of water in [kg/m^3]
 
     Note:
             The function is built upon the following book:
             Maidment, David R and others. “Handbook of Hydrology, McGraw-Hil.” Inc., New York, NY, 1992.
-            
+
             And a paper:
-                Hirabayashi, Satoshi. “I-Tree Eco United States County-Based Hydrologic Estimates.” 
-                Washington, DC: US Department of Agriculture, Forest Service, 2015. 
+                Hirabayashi, Satoshi. “I-Tree Eco United States County-Based Hydrologic Estimates.”
+                Washington, DC: US Department of Agriculture, Forest Service, 2015.
 
     Todo:
+        None
     """
-    return 999.88 + 0.018*temperature - 0.0051*temperature**2
+    return 999.88 + 0.018 * temperature - 0.0051 * temperature**2
+
 
 def D(temperature, dew_point_temperature):
     """The method calculates vapor pressure deficit.
 
     Args:
         Temperature in [C]
-        Dew point temperature in [C]  
+        Dew point temperature in [C]
 
     Returns:
         Vapor pressure deficit in [kPa]
 
     Note:
-            It includes in calculation vapor pressure as well as saturated vapor pressure, both in [kPa], which 
+            It includes in calculation vapor pressure as well as saturated vapor pressure, both in [kPa], which
             are calculated with functions e() e_s().
 
             The function is built upon the following book:
             Maidment, David R and others. “Handbook of Hydrology, McGraw-Hil.” Inc., New York, NY, 1992.
-            
+
             And a paper:
-                Hirabayashi, Satoshi. “I-Tree Eco United States County-Based Hydrologic Estimates.” 
-                Washington, DC: US Department of Agriculture, Forest Service, 2015. 
+                Hirabayashi, Satoshi. “I-Tree Eco United States County-Based Hydrologic Estimates.”
+                Washington, DC: US Department of Agriculture, Forest Service, 2015.
 
     Todo:
+        None
     """
-    return np.maximum(e_s(temperature)-e(dew_point_temperature),0)
+    return np.maximum(e_s(temperature) - e(dew_point_temperature), 0)
+
 
 def U_t(wind_speed, wind_estimate_height):
     """The method estimates wind speed at the tree top.
 
     Args:
-        Measured wind speed [m/s] 
+        Measured wind speed [m/s]
         Wind estimate height (tree height) [m]
 
- 
+
     Returns:
         Wind speed at the tree top in [m/s]
 
     Note:
             The method is using two other parameters:
                 Wind measurement height Z_u (usually 10m) and roughness height for water d_w which are set as constants.
 
             The function is built upon the following book:
             Maidment, David R and others. “Handbook of Hydrology, McGraw-Hil.” Inc., New York, NY, 1992.
-            
+
             And a paper:
-                Hirabayashi, Satoshi. “I-Tree Eco United States County-Based Hydrologic Estimates.” 
-                Washington, DC: US Department of Agriculture, Forest Service, 2015. 
+                Hirabayashi, Satoshi. “I-Tree Eco United States County-Based Hydrologic Estimates.”
+                Washington, DC: US Department of Agriculture, Forest Service, 2015.
 
     Todo:
+        None
     """
-    return wind_speed*np.log(wind_estimate_height/d_w)/np.log(Z_u/d_w)
+    return wind_speed * np.log(wind_estimate_height / d_w) / np.log(Z_u / d_w)
+
 
 def r_a(wind_speed, wind_estimate_height, roughness_height):
     """The method calculates aerodynamic resistance.
 
     Args:
-        Measured wind speed [m/s] 
+        Measured wind speed [m/s]
         Wind estimate height (tree height) [m]
         Roughness_height [m]
- 
+
     Returns:
         Aerodynamic resistance in [m/s]
 
     Note:
             It includes in calculation wind speed at the tree top U_t.
             If roughness height is negative, a new equation is applied to calculate aerodynamic resistance for
             the evapotranspiration from the soil.
 
             The function is built upon the following book:
             Maidment, David R and others. “Handbook of Hydrology, McGraw-Hil.” Inc., New York, NY, 1992.
-            
+
             And a paper:
-                Hirabayashi, Satoshi. “I-Tree Eco United States County-Based Hydrologic Estimates.” 
-                Washington, DC: US Department of Agriculture, Forest Service, 2015. 
+                Hirabayashi, Satoshi. “I-Tree Eco United States County-Based Hydrologic Estimates.”
+                Washington, DC: US Department of Agriculture, Forest Service, 2015.
 
     Todo:
+        None
     """
     if roughness_height >= 0:
-        return 4.72*np.log(wind_estimate_height/(Z_ov*roughness_height))/(1+0.53*U_t(wind_speed, wind_estimate_height))
+        return (
+            4.72
+            * np.log(wind_estimate_height / (Z_ov * roughness_height))
+            / (1 + 0.53 * U_t(wind_speed, wind_estimate_height))
+        )
     else:
-        return 208/U_t(wind_speed, wind_estimate_height)
+        return 208 / U_t(wind_speed, wind_estimate_height)
 
-def gamma(temperature,surface_pressure):
+
+def gamma(temperature, surface_pressure):
     """The method calculates psychrometric constant.
 
     Args:
-        Temperature [C] 
+        Temperature [C]
         Surface pressure [kPa]
- 
+
     Returns:
         Psychrometric constant in [kPA/C]
 
     Note:
             It includes in calculation latent heat of vaporization lmbd().
 
             The function is built upon the following book:
             Maidment, David R and others. “Handbook of Hydrology, McGraw-Hil.” Inc., New York, NY, 1992.
-            
+
             And a paper:
-                Hirabayashi, Satoshi. “I-Tree Eco United States County-Based Hydrologic Estimates.” 
-                Washington, DC: US Department of Agriculture, Forest Service, 2015. 
+                Hirabayashi, Satoshi. “I-Tree Eco United States County-Based Hydrologic Estimates.”
+                Washington, DC: US Department of Agriculture, Forest Service, 2015.
 
     Todo:
+        None
     """
-    #return 10**(-3)*c_p*surface_pressure*10/(lmbd(temperature)*0.622)# pressure in mbar
-    return 10**(-3)*c_p*surface_pressure/(lmbd(temperature)*0.622)# pressure in kPa
+    # return 10**(-3)*c_p*surface_pressure*10/(lmbd(temperature)*0.622)# pressure in mbar
+    return (
+        10 ** (-3) * c_p * surface_pressure / (lmbd(temperature) * 0.622)
+    )  # pressure in kPa
+
 
 def r_s(pai):
     """The method calculates stomatal resistance.
 
     Args:
-        Plant area index (PAI) 
- 
+        Plant area index (PAI)
+
     Returns:
         Stomatal resistance in [s/m]
 
     Note:
             The function is built upon the following book:
             Maidment, David R and others. “Handbook of Hydrology, McGraw-Hil.” Inc., New York, NY, 1992.
-            
+
             And a paper:
-                Hirabayashi, Satoshi. “I-Tree Eco United States County-Based Hydrologic Estimates.” 
-                Washington, DC: US Department of Agriculture, Forest Service, 2015. 
+                Hirabayashi, Satoshi. “I-Tree Eco United States County-Based Hydrologic Estimates.”
+                Washington, DC: US Department of Agriculture, Forest Service, 2015.
 
     Todo:
+        None
     """
-    return 200/pai
+    return 200 / pai
+
 
 def C_leaf(temperature):
     """The method calculates water vapor concentration at the evaporating surfaces within the leaf.
 
     Args:
-        Temperature [C] 
+        Temperature [C]
 
     Returns:
         Water vapor concentration at the evaporating surfaces within the leaf in [g/m^3]
 
     Note:
             Temerature in celsius [C] is converted to kelvins [K] such that T(K) = T(C)+273.15.
-            The formula also includes saturated vapor pressure e_s() in [kPa].  
+            The formula also includes saturated vapor pressure e_s() in [kPa].
 
             The function is built upon the following book:
             Maidment, David R and others. “Handbook of Hydrology, McGraw-Hil.” Inc., New York, NY, 1992.
-            
+
             And a paper:
-                Hirabayashi, Satoshi. “I-Tree Eco United States County-Based Hydrologic Estimates.” 
-                Washington, DC: US Department of Agriculture, Forest Service, 2015. 
+                Hirabayashi, Satoshi. “I-Tree Eco United States County-Based Hydrologic Estimates.”
+                Washington, DC: US Department of Agriculture, Forest Service, 2015.
 
     Todo:
+        None
     """
-    return 2165*e_s(temperature)/(temperature+273.15)
+    return 2165 * e_s(temperature) / (temperature + 273.15)
+
 
 def C_air(dew_point_temperature, temperature):
     """The method calculates water vapor concentration in the air.
 
     Args:
-        Temperature [C] 
+        Temperature [C]
         Dew point temperature [C]
 
     Returns:
         Water vapor concentration in the air in [g/m^3]
 
     Note:
             Temerature in celsius [C] is converted to kelvins [K] such that T(K) = T(C)+273.15.
-            The formula also includes vapor pressure e() in [kPa].  
+            The formula also includes vapor pressure e() in [kPa].
 
             The function is built upon the following book:
             Maidment, David R and others. “Handbook of Hydrology, McGraw-Hil.” Inc., New York, NY, 1992.
-            
+
             And a paper:
-                Hirabayashi, Satoshi. “I-Tree Eco United States County-Based Hydrologic Estimates.” 
-                Washington, DC: US Department of Agriculture, Forest Service, 2015. 
+                Hirabayashi, Satoshi. “I-Tree Eco United States County-Based Hydrologic Estimates.”
+                Washington, DC: US Department of Agriculture, Forest Service, 2015.
 
     Todo:
+        None
     """
-    return 2165*e(dew_point_temperature)/(temperature+273.15)
+    return 2165 * e(dew_point_temperature) / (temperature + 273.15)
+
 
-def potential_evaporation(temperature, dew_point, solar_radiation, sea_level_pressure, pai, wind_speed, wind_estimate_height, roughness_height):
+def potential_evaporation(
+    temperature,
+    dew_point,
+    solar_radiation,
+    sea_level_pressure,
+    pai,
+    wind_speed,
+    wind_estimate_height,
+    roughness_height,
+):
     """The method calculate potential evaporation.
 
     Args: a data frame
-    
-    Returns: the updated ata frame 
-        
+
+    Returns: the updated ata frame
+
     Note:
+        None
 
     Todo:
+        None
     """
-    potential_evaporation = M_TO_MM*(1/(lmbd(temperature)*rho_w(temperature)))*(DELTA(temperature)*solar_radiation+(rho_a(temperature, sea_level_pressure)*c_p*D(temperature, dew_point))/r_a(wind_speed, wind_estimate_height, roughness_height))/(DELTA(temperature)+gamma(temperature, sea_level_pressure)*(1+(r_s(pai)/r_a(wind_speed, wind_estimate_height, roughness_height))))
+    potential_evaporation = (
+        M_TO_MM
+        * (1 / (lmbd(temperature) * rho_w(temperature)))
+        * (
+            DELTA(temperature) * solar_radiation
+            + (rho_a(temperature, sea_level_pressure) * c_p * D(temperature, dew_point))
+            / r_a(wind_speed, wind_estimate_height, roughness_height)
+        )
+        / (
+            DELTA(temperature)
+            + gamma(temperature, sea_level_pressure)
+            * (1 + (r_s(pai) / r_a(wind_speed, wind_estimate_height, roughness_height)))
+        )
+    )
 
     return potential_evaporation
 
+
 def potential_evapotranspiration(df):
     """The method calculate potential evapotranspiration.
 
     Args: a data frame
-    
-    Returns: the updated ata frame 
-        
+
+    Returns: the updated ata frame
+
     Note:
+        None
 
     Todo:
+        None
     """
     df = df.assign(
-        Potential_evaporation_v = lambda x: potential_evaporation(x.Temperature, x.Dew_Point, x.Solar_Radiation, x.Sea_Level_Pressure, x.PAI, x.Wind_Speed, x.height, roughness_height_trees),
-        Potential_evaporation_g = lambda x: potential_evaporation(x.Temperature, x.Dew_Point, x.Solar_Radiation, x.Sea_Level_Pressure, 1    , x.Wind_Speed, 1       , roughness_height_bare_soil),
-        PET                     = lambda x: potential_evaporation(x.Temperature, x.Dew_Point, x.Solar_Radiation, x.Sea_Level_Pressure, x.PAI, x.Wind_Speed, x.height, -1),
-        Transpiration = lambda x: 10**(-6)*(3600/x.PAI)*np.maximum((C_leaf(x.Temperature)-C_air(x.Dew_Point, x.Temperature)),0)/(r_s(x.PAI)+r_a(x.Wind_Speed, x.height, roughness_height_trees))
-        )
+        Potential_evaporation_v=lambda x: potential_evaporation(
+            x.Temperature,
+            x.Dew_Point,
+            x.Solar_Radiation,
+            x.Sea_Level_Pressure,
+            x.PAI,
+            x.Wind_Speed,
+            x.height,
+            roughness_height_trees,
+        ),
+        Potential_evaporation_g=lambda x: potential_evaporation(
+            x.Temperature,
+            x.Dew_Point,
+            x.Solar_Radiation,
+            x.Sea_Level_Pressure,
+            1,
+            x.Wind_Speed,
+            1,
+            roughness_height_bare_soil,
+        ),
+        PET=lambda x: potential_evaporation(
+            x.Temperature,
+            x.Dew_Point,
+            x.Solar_Radiation,
+            x.Sea_Level_Pressure,
+            x.PAI,
+            x.Wind_Speed,
+            x.height,
+            -1,
+        ),
+        Transpiration=lambda x: 10 ** (-6)
+        * (3600 / x.PAI)
+        * np.maximum((C_leaf(x.Temperature) - C_air(x.Dew_Point, x.Temperature)), 0)
+        / (r_s(x.PAI) + r_a(x.Wind_Speed, x.height, roughness_height_trees)),
+    )
     df = df.assign(
-        TF_average_ratio = lambda x: np.where(((x.PET>x.Transpiration) & (x.PET>0)), x.Transpiration/x.PET, np.nan)
+        TF_average_ratio=lambda x: np.where(
+            ((x.PET > x.Transpiration) & (x.PET > 0)), x.Transpiration / x.PET, np.nan
         )
+    )
 
-    df['TF_average_ratio'] = df.groupby(['AgentID','Step'])['TF_average_ratio'].transform('mean')
+    df["TF_average_ratio"] = df.groupby(["AgentID", "Step"])[
+        "TF_average_ratio"
+    ].transform("mean")
     df = df.assign(
-        Transpiration = lambda x: np.where(((x.PAI<(x.LAI+x.BAI)) | (x.Transpiration > x.PET)), x.TF_average_ratio*x.PET, x.Transpiration)
+        Transpiration=lambda x: np.where(
+            ((x.PAI < (x.LAI + x.BAI)) | (x.Transpiration > x.PET)),
+            x.TF_average_ratio * x.PET,
+            x.Transpiration,
         )
+    )
 
-    df = df.drop(columns='TF_average_ratio')
+    df = df.drop(columns="TF_average_ratio")
     return df
 
+
 def ped1(Date_time, Precipitation, Potential_evaporation, Maximum_storage, evp):
     """The method computes precipitation-evaporation dynamics for one type at a time, which can be trees, pervious cover, impervious cover...
 
     Args:
         Date_time [time identifier]
         Precipitation [amount of water hitting the surface area of the type]
         Potential_evaporation [of the type for the given weather conditions]
@@ -540,38 +687,60 @@
     Returns:
         Precipitation storage of the type for each hour.
 
     Note:
 
             The function is built upon the following book:
             Maidment, David R and others. “Handbook of Hydrology, McGraw-Hil.” Inc., New York, NY, 1992.
-            
+
             And a paper:
-                Hirabayashi, Satoshi. “I-Tree Eco United States County-Based Hydrologic Estimates.” 
-                Washington, DC: US Department of Agriculture, Forest Service, 2015. 
+                Hirabayashi, Satoshi. “I-Tree Eco United States County-Based Hydrologic Estimates.”
+                Washington, DC: US Department of Agriculture, Forest Service, 2015.
 
     Todo:
+        None
     """
-    df=pd.DataFrame({'Date_time':Date_time, 'Precipitation':Precipitation, 
-    'Potential_evaporation':Potential_evaporation})
+    df = pd.DataFrame(
+        {
+            "Date_time": Date_time,
+            "Precipitation": Precipitation,
+            "Potential_evaporation": Potential_evaporation,
+        }
+    )
     df["Storage"] = 0
-    df['Potential_evaporation_lag1'] = df.Potential_evaporation.shift(1).interpolate(limit_direction ='backward')
+    df["Potential_evaporation_lag1"] = df.Potential_evaporation.shift(1).interpolate(
+        limit_direction="backward"
+    )
     x = 0
+
     def func2(row):
         # non local variable ==> will use pre_value from the ped function
         nonlocal x
-        new_value =  new_value =  np.maximum(0,(np.minimum(Maximum_storage,x) + row['Precipitation']-
-        np.minimum(np.minimum(Maximum_storage,x),((np.minimum(Maximum_storage,x)/
-        Maximum_storage)**(evp)*row['Potential_evaporation_lag1']))))
+        new_value = new_value = np.maximum(
+            0,
+            (
+                np.minimum(Maximum_storage, x)
+                + row["Precipitation"]
+                - np.minimum(
+                    np.minimum(Maximum_storage, x),
+                    (
+                        (np.minimum(Maximum_storage, x) / Maximum_storage) ** (evp)
+                        * row["Potential_evaporation_lag1"]
+                    ),
+                )
+            ),
+        )
         x = new_value
         return new_value
+
     # This line might throw a SettingWithCopyWarning warning
-    df.loc[0:,'Storage'] = df.loc[0:,:].apply(func2, axis=1)
+    df.loc[0:, "Storage"] = df.loc[0:, :].apply(func2, axis=1)
     return df["Storage"]
 
+
 def ped3(df, evp_v, evp_g):
     """The method computes precipitation-evaporation dynamics for each tree as well as the impervious and pervious covers.
 
     Args:
         A data frame including the following variables:
         Evaporation coefficient for trees: evp_v
         Evaporation coefficient for ground: evp_g
@@ -579,119 +748,241 @@
     Returns:
         A data frame with new variables: Vegetation_storage, Impervious_cover_storage_v, Pervious_cover_storage_v for each hour.
 
     Note:
 
             The function is built upon the following book:
             Maidment, David R and others. “Handbook of Hydrology, McGraw-Hil.” Inc., New York, NY, 1992.
-            
+
             And a paper:
-                Hirabayashi, Satoshi. “I-Tree Eco United States County-Based Hydrologic Estimates.” 
-                Washington, DC: US Department of Agriculture, Forest Service, 2015. 
+                Hirabayashi, Satoshi. “I-Tree Eco United States County-Based Hydrologic Estimates.”
+                Washington, DC: US Department of Agriculture, Forest Service, 2015.
 
     Todo:
+        None
     """
-    df['Storage'] = 0
-    df['Potential_evaporation_v_lag1'] = df.Potential_evaporation_v.shift(1).interpolate(limit_direction ='backward')
-    df['Potential_evaporation_g_lag1'] = df.Potential_evaporation_g.shift(1).interpolate(limit_direction ='backward')
+    df["Storage"] = 0
+    df["Potential_evaporation_v_lag1"] = df.Potential_evaporation_v.shift(
+        1
+    ).interpolate(limit_direction="backward")
+    df["Potential_evaporation_g_lag1"] = df.Potential_evaporation_g.shift(
+        1
+    ).interpolate(limit_direction="backward")
     x = 0
     y = 0
     z = 0
+
     def func2(row):
         # non local variable ==> will use pre_value from the ped function
         nonlocal x
         nonlocal y
         nonlocal z
-        new_value_x =  np.maximum(0,(np.minimum(row['Maximum_vegetation_storage'],x) + row['Canopy_interception']-
-        np.minimum(np.minimum(row['Maximum_vegetation_storage'],x),((np.minimum(row['Maximum_vegetation_storage'],x)/
-        row['Maximum_vegetation_storage'])**(evp_v)*row['Potential_evaporation_v_lag1']))))
-
-        Precipitation_on_the_ground_with_vegetation = np.maximum(0,(new_value_x-row['Maximum_vegetation_storage']))+row['Through_canopy_precipitation']
-        
-        new_value_y = np.maximum(0,(np.minimum(MAXIMUM_IMPERVIOUS_COVER_STORAGE,y) + Precipitation_on_the_ground_with_vegetation-
-        np.minimum(np.minimum(MAXIMUM_IMPERVIOUS_COVER_STORAGE,y),((np.minimum(MAXIMUM_IMPERVIOUS_COVER_STORAGE,y)/
-        MAXIMUM_IMPERVIOUS_COVER_STORAGE)**(evp_g)*row['Potential_evaporation_g_lag1']))))
-        
-        new_value_z = np.maximum(0,(np.minimum(MAXIMUM_PERVIOUS_COVER_STORAGE,z) + Precipitation_on_the_ground_with_vegetation-
-        np.minimum(np.minimum(MAXIMUM_PERVIOUS_COVER_STORAGE,z),((np.minimum(MAXIMUM_PERVIOUS_COVER_STORAGE,z)/
-        MAXIMUM_PERVIOUS_COVER_STORAGE)**(evp_g)*row['Potential_evaporation_g_lag1']))))
+        new_value_x = np.maximum(
+            0,
+            (
+                np.minimum(row["Maximum_vegetation_storage"], x)
+                + row["Canopy_interception"]
+                - np.minimum(
+                    np.minimum(row["Maximum_vegetation_storage"], x),
+                    (
+                        (
+                            np.minimum(row["Maximum_vegetation_storage"], x)
+                            / row["Maximum_vegetation_storage"]
+                        )
+                        ** (evp_v)
+                        * row["Potential_evaporation_v_lag1"]
+                    ),
+                )
+            ),
+        )
+
+        Precipitation_on_the_ground_with_vegetation = (
+            np.maximum(0, (new_value_x - row["Maximum_vegetation_storage"]))
+            + row["Through_canopy_precipitation"]
+        )
+
+        new_value_y = np.maximum(
+            0,
+            (
+                np.minimum(MAXIMUM_IMPERVIOUS_COVER_STORAGE, y)
+                + Precipitation_on_the_ground_with_vegetation
+                - np.minimum(
+                    np.minimum(MAXIMUM_IMPERVIOUS_COVER_STORAGE, y),
+                    (
+                        (
+                            np.minimum(MAXIMUM_IMPERVIOUS_COVER_STORAGE, y)
+                            / MAXIMUM_IMPERVIOUS_COVER_STORAGE
+                        )
+                        ** (evp_g)
+                        * row["Potential_evaporation_g_lag1"]
+                    ),
+                )
+            ),
+        )
+
+        new_value_z = np.maximum(
+            0,
+            (
+                np.minimum(MAXIMUM_PERVIOUS_COVER_STORAGE, z)
+                + Precipitation_on_the_ground_with_vegetation
+                - np.minimum(
+                    np.minimum(MAXIMUM_PERVIOUS_COVER_STORAGE, z),
+                    (
+                        (
+                            np.minimum(MAXIMUM_PERVIOUS_COVER_STORAGE, z)
+                            / MAXIMUM_PERVIOUS_COVER_STORAGE
+                        )
+                        ** (evp_g)
+                        * row["Potential_evaporation_g_lag1"]
+                    ),
+                )
+            ),
+        )
         x = new_value_x
         y = new_value_y
         z = new_value_z
         return [new_value_x, new_value_y, new_value_z]
+
     # This line might throw a SettingWithCopyWarning warning
-    df.loc[0:,'Storage'] = df.loc[0:,:].apply(func2, axis=1)
-    df['Vegetation_storage'] = pd.DataFrame(df['Storage'].tolist())[0]
-    df['Impervious_cover_storage_v'] = pd.DataFrame(df['Storage'].tolist())[1]
-    df['Pervious_cover_storage_v'] = pd.DataFrame(df['Storage'].tolist())[2]
-    df = df.drop(columns='Storage')
+    df.loc[0:, "Storage"] = df.loc[0:, :].apply(func2, axis=1)
+    df["Vegetation_storage"] = pd.DataFrame(df["Storage"].tolist())[0]
+    df["Impervious_cover_storage_v"] = pd.DataFrame(df["Storage"].tolist())[1]
+    df["Pervious_cover_storage_v"] = pd.DataFrame(df["Storage"].tolist())[2]
+    df = df.drop(columns="Storage")
     return df
 
+
 def ecosystem_services(i):
     """The method parallelize the computation of water retention benefits.
 
     Args: agent index "i"
-    
-    Returns: water retention benefits for each agent [data frame] 
-        
+
+    Returns: water retention benefits for each agent [data frame]
+
     Note:
+        None
 
     Todo:
+        None
     """
     output = df_scenario[tree_population.AgentID == AGENTS[i]]
-    output = output[['Step', 'AgentID', 'height','BAI', 'LA','LAI', 'PAI', 'Conifers', 'Under_canopy_area', 'Total_under_canopy_area','Scenario', 'Precipitation_scale', 
-    'SAMPLE_AREA', 'IMPERVIOUS_COVER_SHARE', 'PERVIOUS_COVER_SHARE', 'POPULATION_AREA', 'POPULATION_SAMPLE_TREE_RATIO']]
-    output = pd.merge(output, weather_forcast, on=['Step'], how='left').sort_values(['Step', 'AgentID'])
+    output = output[
+        [
+            "Step",
+            "AgentID",
+            "height",
+            "BAI",
+            "LA",
+            "LAI",
+            "PAI",
+            "Conifers",
+            "Under_canopy_area",
+            "Total_under_canopy_area",
+            "Scenario",
+            "Precipitation_scale",
+            "SAMPLE_AREA",
+            "IMPERVIOUS_COVER_SHARE",
+            "PERVIOUS_COVER_SHARE",
+            "POPULATION_AREA",
+            "POPULATION_SAMPLE_TREE_RATIO",
+        ]
+    ]
+    output = pd.merge(output, weather_forcast, on=["Step"], how="left").sort_values(
+        ["Step", "AgentID"]
+    )
     # Calculate plant area index (PAI) in leaf-on and leaf-off seasons
-    output['PAI'] = pai_seasons(output[['Date_time', 'BAI', 'LAI', 'Conifers']],
-                                        Leaf_on_transition_day_start, Leaf_off_transition_day_start, 
-                                        LEAF_TRANSITION_DAYS)
+    output["PAI"] = pai_seasons(
+        output[["Date_time", "BAI", "LAI", "Conifers"]],
+        Leaf_on_transition_day_start,
+        Leaf_off_transition_day_start,
+        LEAF_TRANSITION_DAYS,
+    )
 
-    
     # Calculate potential evapotranspiration over the vegetation and ground areas
     output = potential_evapotranspiration(output)
 
     output = output.assign(
-        Canopy_cover_fraction = lambda x: 1-np.exp(-KAPPA*x.PAI),
-        Maximum_vegetation_storage = lambda x: SL*x.PAI,
-        Through_canopy_precipitation = lambda x: x.Precipitation*(1-x.Canopy_cover_fraction),
-        Canopy_interception = lambda x: x.Precipitation-x.Through_canopy_precipitation
+        Canopy_cover_fraction=lambda x: 1 - np.exp(-KAPPA * x.PAI),
+        Maximum_vegetation_storage=lambda x: SL * x.PAI,
+        Through_canopy_precipitation=lambda x: x.Precipitation
+        * (1 - x.Canopy_cover_fraction),
+        Canopy_interception=lambda x: x.Precipitation - x.Through_canopy_precipitation,
     )
 
-    output = ped3(output,
-        evp_v = 2/3, 
-        evp_g = 1
-    )
+    output = ped3(output, evp_v=2 / 3, evp_g=1)
     output = output.assign(
-        Canopy_drip = lambda x: np.maximum(0,(x.Vegetation_storage-x.Maximum_vegetation_storage)),
-        Evaporation_from_vegetation = lambda x: np.maximum(0,(x.Canopy_interception-x.Canopy_drip)),
-        Precipitation_on_the_ground_with_vegetation = lambda x: x.Canopy_drip + x.Through_canopy_precipitation,
-        Vegetation_storage = lambda x: np.minimum(x.Vegetation_storage, x.Maximum_vegetation_storage),
-        Run_off_v = lambda x: np.maximum(0,(x.Impervious_cover_storage_v-MAXIMUM_IMPERVIOUS_COVER_STORAGE)),
-        Evaporation_from_impervious_cover_v = lambda x: np.maximum(0,(x.Precipitation_on_the_ground_with_vegetation-x.Run_off_v)),
-        Impervious_cover_storage_v = lambda x: np.minimum(x.Impervious_cover_storage_v, MAXIMUM_IMPERVIOUS_COVER_STORAGE),
-        Infiltration_v = lambda x: np.maximum(0,(x.Pervious_cover_storage_v-MAXIMUM_PERVIOUS_COVER_STORAGE)),
-        Evaporation_from_pervious_cover_v = lambda x: np.maximum(0,(x.Precipitation_on_the_ground_with_vegetation-x.Infiltration_v)),
-        Pervious_cover_storage_v = lambda x: np.minimum(x.Pervious_cover_storage_v, MAXIMUM_PERVIOUS_COVER_STORAGE)
+        Canopy_drip=lambda x: np.maximum(
+            0, (x.Vegetation_storage - x.Maximum_vegetation_storage)
+        ),
+        Evaporation_from_vegetation=lambda x: np.maximum(
+            0, (x.Canopy_interception - x.Canopy_drip)
+        ),
+        Precipitation_on_the_ground_with_vegetation=lambda x: x.Canopy_drip
+        + x.Through_canopy_precipitation,
+        Vegetation_storage=lambda x: np.minimum(
+            x.Vegetation_storage, x.Maximum_vegetation_storage
+        ),
+        Run_off_v=lambda x: np.maximum(
+            0, (x.Impervious_cover_storage_v - MAXIMUM_IMPERVIOUS_COVER_STORAGE)
+        ),
+        Evaporation_from_impervious_cover_v=lambda x: np.maximum(
+            0, (x.Precipitation_on_the_ground_with_vegetation - x.Run_off_v)
+        ),
+        Impervious_cover_storage_v=lambda x: np.minimum(
+            x.Impervious_cover_storage_v, MAXIMUM_IMPERVIOUS_COVER_STORAGE
+        ),
+        Infiltration_v=lambda x: np.maximum(
+            0, (x.Pervious_cover_storage_v - MAXIMUM_PERVIOUS_COVER_STORAGE)
+        ),
+        Evaporation_from_pervious_cover_v=lambda x: np.maximum(
+            0, (x.Precipitation_on_the_ground_with_vegetation - x.Infiltration_v)
+        ),
+        Pervious_cover_storage_v=lambda x: np.minimum(
+            x.Pervious_cover_storage_v, MAXIMUM_PERVIOUS_COVER_STORAGE
+        ),
     )
 
     # Annual aggregation
-    output = output.groupby(['Scenario','Precipitation_scale','AgentID','Step']).agg(
-        Leaf_area = pd.NamedAgg(column='LA', aggfunc=np.mean),
-        Under_canopy_area = pd.NamedAgg(column='Under_canopy_area', aggfunc=np.mean),
-        SAMPLE_AREA = pd.NamedAgg(column='SAMPLE_AREA', aggfunc=np.mean),
-        IMPERVIOUS_COVER_SHARE = pd.NamedAgg(column='IMPERVIOUS_COVER_SHARE', aggfunc=np.mean),
-        PERVIOUS_COVER_SHARE = pd.NamedAgg(column='PERVIOUS_COVER_SHARE', aggfunc=np.mean),
-        POPULATION_AREA = pd.NamedAgg(column='POPULATION_AREA', aggfunc=np.mean),
-        POPULATION_SAMPLE_TREE_RATIO = pd.NamedAgg(column='POPULATION_SAMPLE_TREE_RATIO', aggfunc=np.mean),
-        Annual_precipitation = pd.NamedAgg(column='Precipitation', aggfunc=np.sum),
-        Annual_canopy_interception_loss = pd.NamedAgg(column='Evaporation_from_vegetation', aggfunc=np.sum),
-        Annual_run_off_v = pd.NamedAgg(column='Run_off_v', aggfunc=np.sum),
-        Annual_evaporation_from_impervious_cover_v = pd.NamedAgg(column='Evaporation_from_impervious_cover_v', aggfunc=np.sum),
-        Annual_infiltration_v=pd.NamedAgg(column="Infiltration_v", aggfunc=np.sum),
-        Annual_evaporation_from_pervious_cover_v=pd.NamedAgg(column="Evaporation_from_pervious_cover_v", aggfunc=np.sum),
-        Annual_transpiration=pd.NamedAgg(column="Transpiration", aggfunc=np.sum),
-        Total_under_canopy_area = pd.NamedAgg(column='Total_under_canopy_area', aggfunc=np.mean),
-    ).reset_index()
-    output['Annual_stormwater_retention'] = output.Annual_transpiration + output.Annual_canopy_interception_loss + output.Annual_evaporation_from_impervious_cover_v*output.IMPERVIOUS_COVER_SHARE + output.Annual_evaporation_from_pervious_cover_v*output.PERVIOUS_COVER_SHARE
+    output = (
+        output.groupby(["Scenario", "Precipitation_scale", "AgentID", "Step"])
+        .agg(
+            Leaf_area=pd.NamedAgg(column="LA", aggfunc=np.mean),
+            Under_canopy_area=pd.NamedAgg(column="Under_canopy_area", aggfunc=np.mean),
+            SAMPLE_AREA=pd.NamedAgg(column="SAMPLE_AREA", aggfunc=np.mean),
+            IMPERVIOUS_COVER_SHARE=pd.NamedAgg(
+                column="IMPERVIOUS_COVER_SHARE", aggfunc=np.mean
+            ),
+            PERVIOUS_COVER_SHARE=pd.NamedAgg(
+                column="PERVIOUS_COVER_SHARE", aggfunc=np.mean
+            ),
+            POPULATION_AREA=pd.NamedAgg(column="POPULATION_AREA", aggfunc=np.mean),
+            POPULATION_SAMPLE_TREE_RATIO=pd.NamedAgg(
+                column="POPULATION_SAMPLE_TREE_RATIO", aggfunc=np.mean
+            ),
+            Annual_precipitation=pd.NamedAgg(column="Precipitation", aggfunc=np.sum),
+            Annual_canopy_interception_loss=pd.NamedAgg(
+                column="Evaporation_from_vegetation", aggfunc=np.sum
+            ),
+            Annual_run_off_v=pd.NamedAgg(column="Run_off_v", aggfunc=np.sum),
+            Annual_evaporation_from_impervious_cover_v=pd.NamedAgg(
+                column="Evaporation_from_impervious_cover_v", aggfunc=np.sum
+            ),
+            Annual_infiltration_v=pd.NamedAgg(column="Infiltration_v", aggfunc=np.sum),
+            Annual_evaporation_from_pervious_cover_v=pd.NamedAgg(
+                column="Evaporation_from_pervious_cover_v", aggfunc=np.sum
+            ),
+            Annual_transpiration=pd.NamedAgg(column="Transpiration", aggfunc=np.sum),
+            Total_under_canopy_area=pd.NamedAgg(
+                column="Total_under_canopy_area", aggfunc=np.mean
+            ),
+        )
+        .reset_index()
+    )
+    output["Annual_stormwater_retention"] = (
+        output.Annual_transpiration
+        + output.Annual_canopy_interception_loss
+        + output.Annual_evaporation_from_impervious_cover_v
+        * output.IMPERVIOUS_COVER_SHARE
+        + output.Annual_evaporation_from_pervious_cover_v * output.PERVIOUS_COVER_SHARE
+    )
 
     return output
```

### Comparing `pygus-0.1.9/setup.py` & `pygus-1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['src', 'src.gus', 'src.impacts']
+['pygus', 'pygus.gus', 'pygus.impacts']
 
 package_data = \
-{'': ['*'], 'src.gus': ['inputs/*', 'outputs/trees_yearly.json']}
+{'': ['*'], 'pygus.gus': ['inputs/*', 'outputs/*']}
 
 install_requires = \
 ['fuzzywuzzy>=0.18.0,<0.19.0',
  'ipython>=7.27.0,<8.0.0',
  'matplotlib>=3.4.3,<4.0.0',
  'mesa>=0.8.9,<0.9.0',
  'numpy>=1.21.2,<2.0.0',
  'pandas>=1.3.3,<2.0.0',
  'portray>=1.7.0,<2.0.0',
  'pytest>=7.1.2,<8.0.0',
  'seaborn>=0.11.2,<0.12.0',
- 'termcolor>=2.1.1,<3.0.0']
+ 'termcolor>=2.1.1,<3.0.0',
+ 'utm>=0.7.0,<0.8.0']
 
 setup_kwargs = {
     'name': 'pygus',
-    'version': '0.1.9',
+    'version': '1.0',
     'description': 'Green Urban Scenarios - A digital twin representation, simulation of urban forests and their impact analysis.',
     'long_description': '[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)\n[![Versions](https://img.shields.io/pypi/pyversions/pygus)]()\n\n\n\n# gus\n![GUS-IMAGE](https://miro.medium.com/max/1400/1*fMM7rnq1RJCh-nFBGLUvyA.png)\n\nGreen Urban Scenarios - A digital twin representation, simulation of urban forests and their impact analysis.\n\n## Getting Started\nVisit the GUS [website documentation](https://lucidmindsai.github.io/gus/) for help with installing GUS, code documentation, and a [basic tutorial](https://github.com/lucidmindsai/gus/blob/main/notebooks/Tutorial.ipynb) to get you started. \n\n## Install from PyPi\nWe publish GUS as `pyGus` package in PyPi. Dependencies can be found in the .toml file on the GUS GitHub page. Even though installation with Poetry is possible, the most stable installation can be done via pip.\n\n```\n$ pip install pygus\n```\n\nFor further instructions and code documentation, visit [GUS Code Documentation](https://lucidmindsai.github.io/gus/)\n\n### Who maintains GUS?\nThe GUS is currently developed and maintained by [Lucidminds](https://lucidminds.ai/) and [Dark Matter Labs](https://darkmatterlabs.org/) members as part of their joint project [TreesAI](https://treesasinfrastructure.com/#/).\n\n### Notes\n* The GUS is open for PRs.\n* PRs will be reviewed by the current maintainers of the project.\n* Extensive development guidelines will be provided soon.\n* To report bugs, fixes, and questions, please use the [GitHub issues](https://github.com/lucidmindsai/gus/issues).',
     'author': 'Bulent Ozel',
     'author_email': 'bulent@lucidminds.ai',
     'maintainer': 'Oguzhan Yayla',
     'maintainer_email': 'oguzhan@lucidminds.ai',
     'url': 'https://github.com/lucidmindsai/gus',
```

### Comparing `pygus-0.1.9/PKG-INFO` & `pygus-1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygus
-Version: 0.1.9
+Version: 1.0
 Summary: Green Urban Scenarios - A digital twin representation, simulation of urban forests and their impact analysis.
 Home-page: https://github.com/lucidmindsai/gus
 License: Apache-2.0
 Author: Bulent Ozel
 Author-email: bulent@lucidminds.ai
 Maintainer: Oguzhan Yayla
 Maintainer-email: oguzhan@lucidminds.ai
@@ -31,14 +31,15 @@
 Requires-Dist: mesa (>=0.8.9,<0.9.0)
 Requires-Dist: numpy (>=1.21.2,<2.0.0)
 Requires-Dist: pandas (>=1.3.3,<2.0.0)
 Requires-Dist: portray (>=1.7.0,<2.0.0)
 Requires-Dist: pytest (>=7.1.2,<8.0.0)
 Requires-Dist: seaborn (>=0.11.2,<0.12.0)
 Requires-Dist: termcolor (>=2.1.1,<3.0.0)
+Requires-Dist: utm (>=0.7.0,<0.8.0)
 Project-URL: Repository, https://github.com/lucidmindsai/gus
 Description-Content-Type: text/markdown
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Versions](https://img.shields.io/pypi/pyversions/pygus)]()
```

