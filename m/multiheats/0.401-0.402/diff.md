# Comparing `tmp/multiheats-0.401.tar.gz` & `tmp/multiheats-0.402.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiheats-0.401.tar", last modified: Wed Apr  5 16:05:19 2023, max compression
+gzip compressed data, was "multiheats-0.402.tar", last modified: Thu Apr 20 08:13:36 2023, max compression
```

## Comparing `multiheats-0.401.tar` & `multiheats-0.402.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 cmergny   (1000) cmergny   (1000)        0 2023-04-05 16:05:19.289377 multiheats-0.401/
--rw-r--r--   0 cmergny   (1000) cmergny   (1000)    35150 2023-02-15 14:47:35.000000 multiheats-0.401/COPYING
--rw-r--r--   0 cmergny   (1000) cmergny   (1000)     6059 2023-04-05 16:05:19.289377 multiheats-0.401/PKG-INFO
--rw-r--r--   0 cmergny   (1000) cmergny   (1000)     5872 2023-04-04 17:13:46.000000 multiheats-0.401/README.md
--rw-r--r--   0 cmergny   (1000) cmergny   (1000)       38 2023-04-05 16:05:19.292711 multiheats-0.401/setup.cfg
--rw-r--r--   0 cmergny   (1000) cmergny   (1000)      714 2023-04-05 16:05:09.000000 multiheats-0.401/setup.py
-drwxr-xr-x   0 cmergny   (1000) cmergny   (1000)        0 2023-04-05 16:05:19.289377 multiheats-0.401/src/
-drwxr-xr-x   0 cmergny   (1000) cmergny   (1000)        0 2023-04-05 16:05:19.289377 multiheats-0.401/src/multiheats/
--rw-r--r--   0 cmergny   (1000) cmergny   (1000)        0 2023-02-10 17:09:31.000000 multiheats-0.401/src/multiheats/__init__.py
--rw-rw-r--   0 cmergny   (1000) cmergny   (1000)     1303 2023-02-15 14:46:00.000000 multiheats-0.401/src/multiheats/constants.py
--rw-r--r--   0 cmergny   (1000) cmergny   (1000)     3080 2023-04-04 12:22:11.000000 multiheats-0.401/src/multiheats/create_profiles.py
--rw-r--r--   0 cmergny   (1000) cmergny   (1000)     1945 2023-04-05 09:57:57.000000 multiheats-0.401/src/multiheats/main.py
--rw-r--r--   0 cmergny   (1000) cmergny   (1000)     3153 2023-04-03 15:46:57.000000 multiheats-0.401/src/multiheats/solar_flux.py
--rw-r--r--   0 cmergny   (1000) cmergny   (1000)     8469 2023-04-04 15:57:48.000000 multiheats-0.401/src/multiheats/solvers.py
--rw-r--r--   0 cmergny   (1000) cmergny   (1000)     3850 2023-03-22 22:16:09.000000 multiheats-0.401/src/multiheats/visualise.py
-drwxr-xr-x   0 cmergny   (1000) cmergny   (1000)        0 2023-04-05 16:05:19.289377 multiheats-0.401/src/multiheats.egg-info/
--rw-r--r--   0 cmergny   (1000) cmergny   (1000)     6059 2023-04-05 16:05:19.000000 multiheats-0.401/src/multiheats.egg-info/PKG-INFO
--rw-r--r--   0 cmergny   (1000) cmergny   (1000)      460 2023-04-05 16:05:19.000000 multiheats-0.401/src/multiheats.egg-info/SOURCES.txt
--rw-r--r--   0 cmergny   (1000) cmergny   (1000)        1 2023-04-05 16:05:19.000000 multiheats-0.401/src/multiheats.egg-info/dependency_links.txt
--rw-r--r--   0 cmergny   (1000) cmergny   (1000)       61 2023-04-05 16:05:19.000000 multiheats-0.401/src/multiheats.egg-info/requires.txt
--rw-r--r--   0 cmergny   (1000) cmergny   (1000)       11 2023-04-05 16:05:19.000000 multiheats-0.401/src/multiheats.egg-info/top_level.txt
-drwxr-xr-x   0 cmergny   (1000) cmergny   (1000)        0 2023-04-05 16:05:19.289377 multiheats-0.401/tests/
--rw-r--r--   0 cmergny   (1000) cmergny   (1000)     3615 2023-04-04 17:27:05.000000 multiheats-0.401/tests/test_solv_ana.py
--rw-r--r--   0 cmergny   (1000) cmergny   (1000)     8158 2023-03-24 01:18:22.000000 multiheats-0.401/tests/test_solv_spencer.py
+drwxr-xr-x   0 cmergny   (1000) cmergny   (1000)        0 2023-04-20 08:13:36.755818 multiheats-0.402/
+-rw-r--r--   0 cmergny   (1000) cmergny   (1000)    35150 2023-02-15 14:47:35.000000 multiheats-0.402/COPYING
+-rw-r--r--   0 cmergny   (1000) cmergny   (1000)     6500 2023-04-20 08:13:36.755818 multiheats-0.402/PKG-INFO
+-rw-r--r--   0 cmergny   (1000) cmergny   (1000)     6219 2023-04-05 16:33:59.000000 multiheats-0.402/README.md
+-rw-r--r--   0 cmergny   (1000) cmergny   (1000)       38 2023-04-20 08:13:36.755818 multiheats-0.402/setup.cfg
+-rw-r--r--   0 cmergny   (1000) cmergny   (1000)      833 2023-04-20 08:13:33.000000 multiheats-0.402/setup.py
+drwxr-xr-x   0 cmergny   (1000) cmergny   (1000)        0 2023-04-20 08:13:36.755818 multiheats-0.402/src/
+drwxr-xr-x   0 cmergny   (1000) cmergny   (1000)        0 2023-04-20 08:13:36.755818 multiheats-0.402/src/multiheats/
+-rw-r--r--   0 cmergny   (1000) cmergny   (1000)        0 2023-02-10 17:09:31.000000 multiheats-0.402/src/multiheats/__init__.py
+-rw-rw-r--   0 cmergny   (1000) cmergny   (1000)     1303 2023-02-15 14:46:00.000000 multiheats-0.402/src/multiheats/constants.py
+-rw-r--r--   0 cmergny   (1000) cmergny   (1000)     3081 2023-04-14 09:40:48.000000 multiheats-0.402/src/multiheats/create_profiles.py
+-rw-r--r--   0 cmergny   (1000) cmergny   (1000)     1988 2023-04-19 14:27:50.000000 multiheats-0.402/src/multiheats/main.py
+-rw-r--r--   0 cmergny   (1000) cmergny   (1000)     3103 2023-04-17 14:40:28.000000 multiheats-0.402/src/multiheats/solar_flux.py
+-rw-r--r--   0 cmergny   (1000) cmergny   (1000)     8817 2023-04-10 19:24:31.000000 multiheats-0.402/src/multiheats/solvers.py
+-rw-r--r--   0 cmergny   (1000) cmergny   (1000)     3850 2023-03-22 22:16:09.000000 multiheats-0.402/src/multiheats/visualise.py
+drwxr-xr-x   0 cmergny   (1000) cmergny   (1000)        0 2023-04-20 08:13:36.755818 multiheats-0.402/src/multiheats.egg-info/
+-rw-r--r--   0 cmergny   (1000) cmergny   (1000)     6500 2023-04-20 08:13:36.000000 multiheats-0.402/src/multiheats.egg-info/PKG-INFO
+-rw-r--r--   0 cmergny   (1000) cmergny   (1000)      460 2023-04-20 08:13:36.000000 multiheats-0.402/src/multiheats.egg-info/SOURCES.txt
+-rw-r--r--   0 cmergny   (1000) cmergny   (1000)        1 2023-04-20 08:13:36.000000 multiheats-0.402/src/multiheats.egg-info/dependency_links.txt
+-rw-r--r--   0 cmergny   (1000) cmergny   (1000)       61 2023-04-20 08:13:36.000000 multiheats-0.402/src/multiheats.egg-info/requires.txt
+-rw-r--r--   0 cmergny   (1000) cmergny   (1000)       11 2023-04-20 08:13:36.000000 multiheats-0.402/src/multiheats.egg-info/top_level.txt
+drwxr-xr-x   0 cmergny   (1000) cmergny   (1000)        0 2023-04-20 08:13:36.755818 multiheats-0.402/tests/
+-rw-r--r--   0 cmergny   (1000) cmergny   (1000)     3615 2023-04-08 15:00:35.000000 multiheats-0.402/tests/test_solv_ana.py
+-rw-r--r--   0 cmergny   (1000) cmergny   (1000)     8158 2023-03-24 01:18:22.000000 multiheats-0.402/tests/test_solv_spencer.py
```

### Comparing `multiheats-0.401/COPYING` & `multiheats-0.402/COPYING`

 * *Files identical despite different names*

### Comparing `multiheats-0.401/PKG-INFO` & `multiheats-0.402/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-Metadata-Version: 2.1
-Name: multiheats
-Version: 0.401
-Summary: MultIHeaTS is a Multi-layered Implicit Heat Transfer Solver.
-Description-Content-Type: text/markdown
-License-File: COPYING
-
 <div align="center">
 
 # MultIHeaTS
 
 MultIHeaTS is a Multi-layered Implicit Heat Transfer Solver. 
 
 It is an implicit numerical model that simulates and predicts the surface temperature in 1D multi-layered planetary surfaces exposed to solar radiation.
@@ -32,53 +25,74 @@
 Showcase of what the solver can output for a bi-layer surface profile on Japet. Note that here the interface is located around 32 cm.
 Additional figures may be found in the *examples* directory.
 
 
 
 ## Dependencies
 
-- a shell
+- python
 - git
-- conda
 
-You can find conda at https://www.anaconda.com/ although I would suggest installing it directly from the command line.
+<details>
+  <summary>Depecrated method</summary>
+
+  If you want to use conda env:
+  
+  You can find conda at https://www.anaconda.com/ although I would suggest installing it directly from the command line.
 Make sure conda is installed by tiping:
 ```bash
 conda
 ```
 It should return a help message.
+</details>
+
+
+
 
 ## Installation
 
 Copy the project localy using git clone:
 
 ```bash
 git clone git@gitlab.dsi.universite-paris-saclay.fr:cyril.mergny/multiheats.git
 ```
-then cd to the path of the repositery on you computer
+then cd to the path of the repositery on you computer and create a venv environment:
 
 ```bash
 cd path_to_multiheats/
+python -m venv mheats
+source mheats/bin/activate
+```
+
+To install the package then you just need to type:
+```bash
+pip install --upgrade pip
+pip install -e .
 ```
 
-Then install the required conda environment ( an alternative method using pip is in WIP):
+<details>
+  <summary>Click for conda install (Not recommended)</summary>
+
+
+Install the required conda environment :
 
 ```bash
 conda env create -f environment.yml
 ```
-Finally you need to make multiheats a python package by typing:
+Please note that the environment.yml file has been deleted in newer versions. It can be found on older commits. Finally you need to make multiheats a python package by typing:
 ```bash
 pip install -e .
 ```
-(It is in my plans to replace the conda env by packaging all dependancies in pip.)
+</details>
+
 
 # How to use
-Make sure to activate the conda environment before executing anything:
+Make sure to activate the python environment before executing anything:
 ```bash
-conda activate multitheats
+source mheats/bin/activate
 ```
 
 There is an example script that you can run to see what the algorithm ouptut for a pre-defined profile.
 
 ```bash
 cd path_to_multiheats/examples/
 ./run_example.sh
```

### Comparing `multiheats-0.401/README.md` & `multiheats-0.402/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: multiheats
+Version: 0.402
+Summary: MultIHeaTS is a Multi-layered Implicit Heat Transfer Solver.
+Project-URL: Homepage, https://gitlab.dsi.universite-paris-saclay.fr/cyril.mergny/multiheats/
+Description-Content-Type: text/markdown
+License-File: COPYING
+
 <div align="center">
 
 # MultIHeaTS
 
 MultIHeaTS is a Multi-layered Implicit Heat Transfer Solver. 
 
 It is an implicit numerical model that simulates and predicts the surface temperature in 1D multi-layered planetary surfaces exposed to solar radiation.
@@ -25,53 +33,74 @@
 Showcase of what the solver can output for a bi-layer surface profile on Japet. Note that here the interface is located around 32 cm.
 Additional figures may be found in the *examples* directory.
 
 
 
 ## Dependencies
 
-- a shell
+- python
 - git
-- conda
 
-You can find conda at https://www.anaconda.com/ although I would suggest installing it directly from the command line.
+<details>
+  <summary>Depecrated method</summary>
+
+  If you want to use conda env:
+  
+  You can find conda at https://www.anaconda.com/ although I would suggest installing it directly from the command line.
 Make sure conda is installed by tiping:
 ```bash
 conda
 ```
 It should return a help message.
+</details>
+
+
+
 
 ## Installation
 
 Copy the project localy using git clone:
 
 ```bash
 git clone git@gitlab.dsi.universite-paris-saclay.fr:cyril.mergny/multiheats.git
 ```
-then cd to the path of the repositery on you computer
+then cd to the path of the repositery on you computer and create a venv environment:
 
 ```bash
 cd path_to_multiheats/
+python -m venv mheats
+source mheats/bin/activate
+```
+
+To install the package then you just need to type:
+```bash
+pip install --upgrade pip
+pip install -e .
 ```
 
-Then install the required conda environment ( an alternative method using pip is in WIP):
+<details>
+  <summary>Click for conda install (Not recommended)</summary>
+
+
+Install the required conda environment :
 
 ```bash
 conda env create -f environment.yml
 ```
-Finally you need to make multiheats a python package by typing:
+Please note that the environment.yml file has been deleted in newer versions. It can be found on older commits. Finally you need to make multiheats a python package by typing:
 ```bash
 pip install -e .
 ```
-(It is in my plans to replace the conda env by packaging all dependancies in pip.)
+</details>
+
 
 # How to use
-Make sure to activate the conda environment before executing anything:
+Make sure to activate the python environment before executing anything:
 ```bash
-conda activate multitheats
+source mheats/bin/activate
 ```
 
 There is an example script that you can run to see what the algorithm ouptut for a pre-defined profile.
 
 ```bash
 cd path_to_multiheats/examples/
 ./run_example.sh
```

### Comparing `multiheats-0.401/src/multiheats/constants.py` & `multiheats-0.402/src/multiheats/constants.py`

 * *Files identical despite different names*

### Comparing `multiheats-0.401/src/multiheats/create_profiles.py` & `multiheats-0.402/src/multiheats/create_profiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,26 +11,26 @@
     """
     Surface profile used by the termal model.
     You may change properties directly in the code.
 
     """
 
     def __init__(self) -> None:
-        self.nx = 100
+        self.nx = 30
         self.lat = 0
         self.long = 0
         self.eps = 0.94  # Emissivity
         x0 = 0  # Surface depth (m)
         xf = 5  # Total depth (m)
 
         self.qheat = np.full(self.nx, 0)
         power = 3
         spaces = np.linspace(x0, xf ** (1 / power), self.nx)
         self.spaces = spaces ** (power)
-        self.spaces = np.linspace(0, xf, self.nx)
+        # self.spaces = np.linspace(0, xf, self.nx)
 
     def monolayer_prof(self):
         """
         Generate an monolayered surface profile.
         PARAMS:
             cond - Conductivity (W.m-1.K-2)
             rho - Density (kg,m-3)
```

### Comparing `multiheats-0.401/src/multiheats/main.py` & `multiheats-0.402/src/multiheats/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,19 +15,18 @@
 __credits__ = ["Cyril Mergny"]
 __license__ = "Gnu GPL"
 __email__ = "cyril.mergny@universite-paris-saclay.fr"
 
 ### IMPORTS
 
 import numpy as np
-import matplotlib.pyplot as plt
 from tqdm import tqdm
-from matplotlib.animation import FuncAnimation
+import matplotlib.pyplot as plt
 
-from multiheats.solvers import ImplicitSolver, CrankNicolson
+from multiheats.solvers import ImplicitSolver
 from multiheats.create_profiles import Profile
 from multiheats.solar_flux import SurfFlux
 import multiheats.visualise as vis
 
 ### MAIN
 
 
@@ -44,21 +43,24 @@
     prof.temp = np.full(prof.nx, temp_eq)
 
     times = surf.times[:]
     nt = times.shape[0]
     dts = np.diff(times)
     temps = np.zeros((nt, prof.nx))
 
-    print("Computing temperature evolution...")
-    for it in tqdm(range(times.shape[0] - 1)):
-        solver = ImplicitSolver(prof)
-        solar_flux = -surf.get_flux(times[it], prof.lat, prof.long)
-        prof.temp = solver.implicit_scheme(dts[it], solar_flux)
+    solar_fluxs = -surf.get_solar_fluxs(prof.lat, prof.long)
 
-        temps[it] = prof.temp
+    solver = ImplicitSolver(prof)
+    print("Computing temperature evolution...")
+    for i in range(25):
+        for it in tqdm(range(times.shape[0] - 1)):
+            prof.temp = solver.implicit_scheme(dts[it], solar_fluxs[it])
+            temps[it] = prof.temp
+            solver.temp = prof.temp
+            solver.need_update = False
 
     print("Visualisation")
     it = 10
     # vis.use_latex()
     # vis.plot_temp(prof.spaces, temps, it, interf=prof.interf)
     # vis.plot_multi_temp(prof.spaces, temps, n_curves=10)
     anim = vis.animate_function(
```

### Comparing `multiheats-0.401/src/multiheats/solar_flux.py` & `multiheats-0.402/src/multiheats/solar_flux.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from scipy.io import readsav
-import matplotlib.pyplot as plt
 import pandas as pd
 import numpy as np
+from scipy.io import readsav
+
+# import matplotlib.pyplot as plt
 
 import multiheats.constants as cst
 
 
 class SurfFlux:
     """
     Import solar flux and albedos and generature boundary condition.
@@ -61,21 +62,20 @@
 
         mean_slr_flux = self.get_local_fluxs(lat, long).mean()
         mean_surf_flux = (1 - alb) * mean_slr_flux
 
         temp_eq = (mean_surf_flux / eps / cst.SIGMA) ** (1 / 4)
         return temp_eq
 
-    def get_flux(self, time, lat, long):
+    def get_solar_fluxs(self, lat, long):
         """
         Get flux array for a given lat and long.
         in W/m2
         """
-        itime = find_nearest(self.times, time)
-        flux = self.get_local_fluxs(lat, long)[itime]
+        flux = self.get_local_fluxs(lat, long)
         self.alb = self.get_local_albedos(lat, long)
 
         return (1 - self.alb) * flux
 
 
 def find_nearest(array, value, verbose=False):
     array = np.asarray(array)
```

### Comparing `multiheats-0.401/src/multiheats/solvers.py` & `multiheats-0.402/src/multiheats/solvers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Implicit solver of the heat equation.
 """
 
 ### IMPORTS
 import numpy as np
 import scipy
-import time
 
 import multiheats.constants as cst
 
 ### CLASS
 
 
 class ImplicitSolver:
@@ -23,93 +22,104 @@
         self.cond = prof.cond
         self.rho = prof.rho
         self.cp = prof.cp
         self.qheat = prof.qheat
         self.eps = prof.eps
         self.nx = prof.spaces.shape[0]
         self.dx = np.diff(prof.spaces)
+        self.need_update = True
 
     def implicit_scheme(self, dt, solar_flux):
         """
         Solves the discretized heat equation implicitely
         with Euler Backward Scheme.
         Input: prev_temp at time it-1
         Returns: new_temp at time it np.array with shape=(nx)
         """
 
         rcoef = dt / self.rho / self.cp
-        cond = self.cond
-        dx = self.dx
-        prev_temp = np.copy(self.temp)
-        matrice = np.zeros((3, self.nx))
 
-        dkn = (cond[2:] - cond[1:-1]) / (2 * dx[1:]) + (cond[1:-1] - cond[:-2]) / (
-            2 * dx[:-1]
-        )
-
-        matrice[2, :-2] = (
-            -rcoef[1:-1] / dx[:-1] * (-dkn / 2 + 2 * cond[1:-1] / (dx[1:] + dx[:-1]))
-        )  # an
-
-        matrice[1, 1:-1] = 1 - rcoef[1:-1] / (dx[1:] * dx[:-1]) * (
-            dkn / 2 * (dx[1:] - dx[:-1]) - 2 * cond[1:-1]
-        )  # bn
-
-        matrice[0, 2:] = (
-            -rcoef[1:-1] / dx[1:] * (dkn / 2 + 2 * cond[1:-1] / (dx[1:] + dx[:-1]))
-        )  # cn
+        if self.need_update:
+            self.matrix = self.update_matrix(self.nx, self.cond, self.dx, rcoef)
 
         # Set BC
-        source = prev_temp + rcoef * self.qheat
-        s1, sN, b1, c1, aN, bN = self.set_flux_BC(dt, solar_flux)
+        source = self.temp + rcoef * self.qheat
+
+        s1, sN, b1, c1, aN, bN = self.set_flux_BC(rcoef, solar_flux)
         source[0] = s1
         source[-1] = sN
-
-        matrice[1, 0] = b1
-        matrice[1, -1] = bN
-
-        matrice[0, 1] = c1
-        matrice[2, -2] = aN
-
-        new_temp = scipy.linalg.solve_banded((1, 1), matrice, source)
+        self.matrix[1, 0] = b1
+        self.matrix[1, -1] = bN
+        self.matrix[0, 1] = c1
+        self.matrix[2, -2] = aN
+
+        new_temp = scipy.linalg.solve_banded(
+            (1, 1),
+            self.matrix,
+            source,
+            check_finite=False,
+            overwrite_b=True,
+        )
 
         return new_temp
 
-    def set_flux_BC(self, dt, solar_flux):
+    def set_flux_BC(self, rcoef, solar_flux):
         """
         Set boundary conditions for implicit Euler Scheme
         Imposed flux or imposed temperature possible.
         """
-        rcoef = dt / self.rho / self.cp
-        cond = self.cond
 
         # Set Boundary conditions
-        bc_top = solar_flux / cond[0]
-        bc_top += self.eps * cst.SIGMA / self.cond[0] * self.temp[0] ** 4
-        self.bc_top = bc_top
-        bc_bottom = 0
-
-        s1 = (
-            self.temp[0]
-            + rcoef[0] * (cond[1] - 3 * cond[0]) / self.dx[0] * bc_top
-            + rcoef[0] * self.qheat[0]
-        )
-
-        sN = (
-            self.temp[-1]
-            + rcoef[-1] * (3 * cond[-1] - cond[-2]) * bc_bottom / self.dx[-1]
-            + rcoef[-1] * self.qheat[-1]
-        )
-
-        b1 = 1 + 2 * rcoef[0] * cond[0] / self.dx[0] ** 2  # b1
-        c1 = -2 * rcoef[0] * cond[0] / self.dx[0] ** 2  # c1
-        aN = -2 * rcoef[-1] * cond[-1] / self.dx[-1] ** 2  # aN
-        bN = 1 + 2 * rcoef[-1] * cond[-1] / self.dx[-1] ** 2  # bN
+        self.bc_top = (
+            solar_flux + self.eps * cst.SIGMA * self.temp[0] ** 4
+        ) / self.cond[0]
+
+        self.bc_bottom = 0
+
+        s1 = self.temp[0] + rcoef[0] * (
+            (self.cond[1] - 3 * self.cond[0]) / self.dx[0] * self.bc_top + self.qheat[0]
+        )
+
+        sN = self.temp[-1] + rcoef[-1] * (
+            (3 * self.cond[-1] - self.cond[-2]) * self.bc_bottom / self.dx[-1]
+            + self.qheat[-1]
+        )
+
+        coef_top = rcoef[0] * self.cond[0] / self.dx[0] ** 2
+        coef_bot = rcoef[-1] * self.cond[-1] / self.dx[-1] ** 2
+
+        b1 = 1 + 2 * coef_top  # b1
+        c1 = -2 * coef_top  # c1
+        aN = -2 * coef_bot  # aN
+        bN = 1 + 2 * coef_bot  # bN
         return s1, sN, b1, c1, aN, bN
 
+    def update_matrix(self, nx, cond, dx, rcoef):
+        """
+        Update the coefficients of the tridiagonal matrix.
+        Necessary if some of the thermal properties, the grid or the timestep are changed between iterations.
+        """
+        matrix = np.zeros((3, nx))
+        dkn = (cond[2:] - cond[1:-1]) / (2 * dx[1:]) + (cond[1:-1] - cond[:-2]) / (
+            2 * dx[:-1]
+        )
+        # an
+        matrix[2, :-2] = (
+            -rcoef[1:-1] / dx[:-1] * (-dkn / 2 + 2 * cond[1:-1] / (dx[1:] + dx[:-1]))
+        )
+        # bn
+        matrix[1, 1:-1] = 1 - rcoef[1:-1] / (dx[1:] * dx[:-1]) * (
+            dkn / 2 * (dx[1:] - dx[:-1]) - 2 * cond[1:-1]
+        )
+        # cn
+        matrix[0, 2:] = (
+            -rcoef[1:-1] / dx[1:] * (dkn / 2 + 2 * cond[1:-1] / (dx[1:] + dx[:-1]))
+        )
+        return matrix
+
 
 class CrankNicolson:
     """
     Norbert Schorghofer Implementation of CN of 1D heat equation.
     Modified by C. Mergny 2023 to fit into the multiheats pipeline.
     originally written by Samar Khatiwala, 2001
     extended to variable thermal properties
```

### Comparing `multiheats-0.401/src/multiheats/visualise.py` & `multiheats-0.402/src/multiheats/visualise.py`

 * *Files identical despite different names*

### Comparing `multiheats-0.401/src/multiheats.egg-info/PKG-INFO` & `multiheats-0.402/src/multiheats.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: multiheats
-Version: 0.401
+Version: 0.402
 Summary: MultIHeaTS is a Multi-layered Implicit Heat Transfer Solver.
+Project-URL: Homepage, https://gitlab.dsi.universite-paris-saclay.fr/cyril.mergny/multiheats/
 Description-Content-Type: text/markdown
 License-File: COPYING
 
 <div align="center">
 
 # MultIHeaTS
 
@@ -32,53 +33,74 @@
 Showcase of what the solver can output for a bi-layer surface profile on Japet. Note that here the interface is located around 32 cm.
 Additional figures may be found in the *examples* directory.
 
 
 
 ## Dependencies
 
-- a shell
+- python
 - git
-- conda
 
-You can find conda at https://www.anaconda.com/ although I would suggest installing it directly from the command line.
+<details>
+  <summary>Depecrated method</summary>
+
+  If you want to use conda env:
+  
+  You can find conda at https://www.anaconda.com/ although I would suggest installing it directly from the command line.
 Make sure conda is installed by tiping:
 ```bash
 conda
 ```
 It should return a help message.
+</details>
+
+
+
 
 ## Installation
 
 Copy the project localy using git clone:
 
 ```bash
 git clone git@gitlab.dsi.universite-paris-saclay.fr:cyril.mergny/multiheats.git
 ```
-then cd to the path of the repositery on you computer
+then cd to the path of the repositery on you computer and create a venv environment:
 
 ```bash
 cd path_to_multiheats/
+python -m venv mheats
+source mheats/bin/activate
 ```
 
-Then install the required conda environment ( an alternative method using pip is in WIP):
+To install the package then you just need to type:
+```bash
+pip install --upgrade pip
+pip install -e .
+```
+
+<details>
+  <summary>Click for conda install (Not recommended)</summary>
+
+
+Install the required conda environment :
 
 ```bash
 conda env create -f environment.yml
 ```
-Finally you need to make multiheats a python package by typing:
+Please note that the environment.yml file has been deleted in newer versions. It can be found on older commits. Finally you need to make multiheats a python package by typing:
 ```bash
 pip install -e .
 ```
-(It is in my plans to replace the conda env by packaging all dependancies in pip.)
+</details>
+
 
 # How to use
-Make sure to activate the conda environment before executing anything:
+Make sure to activate the python environment before executing anything:
 ```bash
-conda activate multitheats
+source mheats/bin/activate
 ```
 
 There is an example script that you can run to see what the algorithm ouptut for a pre-defined profile.
 
 ```bash
 cd path_to_multiheats/examples/
 ./run_example.sh
```

### Comparing `multiheats-0.401/tests/test_solv_ana.py` & `multiheats-0.402/tests/test_solv_ana.py`

 * *Files identical despite different names*

### Comparing `multiheats-0.401/tests/test_solv_spencer.py` & `multiheats-0.402/tests/test_solv_spencer.py`

 * *Files identical despite different names*

