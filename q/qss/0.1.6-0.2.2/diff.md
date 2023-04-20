# Comparing `tmp/qss-0.1.6.tar.gz` & `tmp/qss-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qss-0.1.6.tar", last modified: Tue Mar 21 00:24:29 2023, max compression
+gzip compressed data, was "qss-0.2.2.tar", last modified: Thu Apr 20 21:38:42 2023, max compression
```

## Comparing `qss-0.1.6.tar` & `qss-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 00:24:29.917382 qss-0.1.6/
--rw-r--r--   0 root         (0) root         (0)    11356 2023-03-21 00:24:22.000000 qss-0.1.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8240 2023-03-21 00:24:29.917382 qss-0.1.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7888 2023-03-21 00:24:22.000000 qss-0.1.6/README.md
--rw-r--r--   0 root         (0) root         (0)      102 2023-03-21 00:24:22.000000 qss-0.1.6/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 00:24:29.917382 qss-0.1.6/qss/
--rw-r--r--   0 root         (0) root         (0)       24 2023-03-21 00:24:22.000000 qss-0.1.6/qss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7926 2023-03-21 00:24:22.000000 qss-0.1.6/qss/admm.py
--rw-r--r--   0 root         (0) root         (0)     8652 2023-03-21 00:24:22.000000 qss-0.1.6/qss/descent.py
--rw-r--r--   0 root         (0) root         (0)     5372 2023-03-21 00:24:22.000000 qss-0.1.6/qss/linearoperator.py
--rw-r--r--   0 root         (0) root         (0)     3565 2023-03-21 00:24:22.000000 qss-0.1.6/qss/matrix.py
--rw-r--r--   0 root         (0) root         (0)     7853 2023-03-21 00:24:22.000000 qss-0.1.6/qss/polish.py
--rw-r--r--   0 root         (0) root         (0)     1809 2023-03-21 00:24:22.000000 qss-0.1.6/qss/precondition.py
--rw-r--r--   0 root         (0) root         (0)    16762 2023-03-21 00:24:22.000000 qss-0.1.6/qss/proximal.py
--rw-r--r--   0 root         (0) root         (0)    13089 2023-03-21 00:24:22.000000 qss-0.1.6/qss/qss.py
--rw-r--r--   0 root         (0) root         (0)     3994 2023-03-21 00:24:22.000000 qss-0.1.6/qss/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 00:24:29.917382 qss-0.1.6/qss.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8240 2023-03-21 00:24:29.000000 qss-0.1.6/qss.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      327 2023-03-21 00:24:29.000000 qss-0.1.6/qss.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-21 00:24:29.000000 qss-0.1.6/qss.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-03-21 00:24:29.000000 qss-0.1.6/qss.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-21 00:24:29.000000 qss-0.1.6/qss.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-21 00:24:29.917382 qss-0.1.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      610 2023-03-21 00:24:22.000000 qss-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 21:38:42.135013 qss-0.2.2/
+-rw-r--r--   0 root         (0) root         (0)    11356 2023-04-20 21:38:35.000000 qss-0.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8240 2023-04-20 21:38:42.135013 qss-0.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7888 2023-04-20 21:38:35.000000 qss-0.2.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-20 21:38:35.000000 qss-0.2.2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 21:38:42.135013 qss-0.2.2/qss/
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-20 21:38:35.000000 qss-0.2.2/qss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8996 2023-04-20 21:38:35.000000 qss-0.2.2/qss/admm.py
+-rw-r--r--   0 root         (0) root         (0)     8652 2023-04-20 21:38:35.000000 qss-0.2.2/qss/descent.py
+-rw-r--r--   0 root         (0) root         (0)     5372 2023-04-20 21:38:35.000000 qss-0.2.2/qss/linearoperator.py
+-rw-r--r--   0 root         (0) root         (0)     3565 2023-04-20 21:38:35.000000 qss-0.2.2/qss/matrix.py
+-rw-r--r--   0 root         (0) root         (0)     7853 2023-04-20 21:38:35.000000 qss-0.2.2/qss/polish.py
+-rw-r--r--   0 root         (0) root         (0)     1809 2023-04-20 21:38:35.000000 qss-0.2.2/qss/precondition.py
+-rw-r--r--   0 root         (0) root         (0)    17379 2023-04-20 21:38:35.000000 qss-0.2.2/qss/proximal.py
+-rw-r--r--   0 root         (0) root         (0)    13268 2023-04-20 21:38:35.000000 qss-0.2.2/qss/qss.py
+-rw-r--r--   0 root         (0) root         (0)     5639 2023-04-20 21:38:35.000000 qss-0.2.2/qss/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 21:38:42.135013 qss-0.2.2/qss.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8240 2023-04-20 21:38:42.000000 qss-0.2.2/qss.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      327 2023-04-20 21:38:42.000000 qss-0.2.2/qss.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 21:38:42.000000 qss-0.2.2/qss.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-20 21:38:42.000000 qss-0.2.2/qss.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-20 21:38:42.000000 qss-0.2.2/qss.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 21:38:42.135013 qss-0.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      610 2023-04-20 21:38:35.000000 qss-0.2.2/setup.py
```

### Comparing `qss-0.1.6/LICENSE` & `qss-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qss-0.1.6/PKG-INFO` & `qss-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qss
-Version: 0.1.6
+Version: 0.2.2
 Summary: QSS: Quadratic-Separable Solver
 Home-page: https://github.com/lukevolpatti/qss
 Author: Luke Volpatti
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/lukevolpatti/qss/issues
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `qss-0.1.6/README.md` & `qss-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `qss-0.1.6/qss/admm.py` & `qss-0.2.2/qss/admm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 import scipy as sp
 import time
+import os
 from qss import proximal
 from qss import matrix
 from qss import util
 
 # Constants
 RHO_MIN = 1e-6
 RHO_MAX = 1e6
@@ -110,14 +111,29 @@
     data, kkt_system, options, rho_controller, x, y, equil_scaling, obj_scale, **kwargs
 ):
     if options["verbose"]:
         print("")
         print("ADMM solve".center(util.PRINT_WIDTH))
         util.print_header()
         admm_start_time = time.time()
+    if options["debug"]:
+        debug_start = time.strftime("%Y%m%d_%H%M%S") + f"_{int(np.round(np.modf(time.time())[0],4)*1e4)}"
+        statement = "####################\ndebug start: "
+        statement += debug_start + "\n"
+        ws = options["warm_start"]
+        statement += f"warm start: {ws}\n"
+        statement += '####################'
+        print(statement)
+        fn_x = debug_start + f"__passed_x.txt"
+        fn_y = debug_start + f"__passed_y.txt"
+        folder_loc = 'debug/'
+        if not os.path.exists(folder_loc):
+            os.makedirs(folder_loc)
+        np.savetxt(folder_loc + fn_x, x)
+        np.savetxt(folder_loc + fn_y, y)
 
     # Unpacking data
     P = data["P"]
     q = data["q"]
     r = data["r"]
     g = data["g"]
     A = data["A"]
@@ -147,14 +163,22 @@
 
     iter_num = 0
     refactorization_count = 0
     total_refactorization_time = 0
     finished = False
 
     while not finished:
+        if options["debug"] and (iter_num <= 5 or iter_num % 10 == 0):
+            folder_loc = 'debug/'
+            if not os.path.exists(folder_loc):
+                os.makedirs(folder_loc)
+            fn_x = debug_start + f"_{iter_num:04}_x.txt"
+            fn_z = debug_start + f"_{iter_num:04}_z.txt"
+            np.savetxt(folder_loc + fn_x, xk1)
+            np.savetxt(folder_loc + fn_z, zk)
         iter_num += 1
         rho_vec = rho_controller.get_rho_vec()
         if schedule_alpha and max_iter < np.inf:
             alpha = alpha_init * (max_iter - iter_num + 1) / max_iter
         else:
             alpha = alpha_init
```

### Comparing `qss-0.1.6/qss/descent.py` & `qss-0.2.2/qss/descent.py`

 * *Files identical despite different names*

### Comparing `qss-0.1.6/qss/linearoperator.py` & `qss-0.2.2/qss/linearoperator.py`

 * *Files identical despite different names*

### Comparing `qss-0.1.6/qss/matrix.py` & `qss-0.2.2/qss/matrix.py`

 * *Files identical despite different names*

### Comparing `qss-0.1.6/qss/polish.py` & `qss-0.2.2/qss/polish.py`

 * *Files identical despite different names*

### Comparing `qss-0.1.6/qss/precondition.py` & `qss-0.2.2/qss/precondition.py`

 * *Files identical despite different names*

### Comparing `qss-0.1.6/qss/proximal.py` & `qss-0.2.2/qss/proximal.py`

 * *Files 9% similar despite different names*

```diff
@@ -472,28 +472,25 @@
         ls[is_bool_indices == 0] = 0
         rs[is_bool_indices == 0] = 0
 
         return ls, rs
 
 
 class GCollection:
-    def __init__(self, g_list, dim):
+    def __init__(self, g_list, dim, relax=False):
         self._g_list = []
         self._is_convex = True
         self._all_zeros = True
         self._full_g = False
         self.dim = dim
         self.bool_ranges = np.vstack(
             [np.full((len(g_list), dim), False), np.full((1, dim), True)]
         )
 
         for i, g in enumerate(g_list):
-            weight = 1
-            scale = 1
-            shift = 0
             if "args" in g and "weight" in g["args"]:
                 weight = g["args"]["weight"]
             else:
                 weight = 1
             if "args" in g and "scale" in g["args"]:
                 scale = g["args"]["scale"]
             else:
@@ -526,21 +523,28 @@
             elif name == "is_zero":
                 func = IsZero(weight, scale, shift)
             elif name == "pos":
                 func = Pos(weight, scale, shift)
             elif name == "neg":
                 func = Neg(weight, scale, shift)
             elif name == "card":
-                func = Card(weight, scale, shift)
+                if not relax:
+                    func = Card(weight, scale, shift)
+                else:
+                    func = Abs(weight, scale, shift)
             elif name == "card_constr":
-                if "args" in g and "k" in g["args"]:
-                    k = g["args"]["k"]
-                else: 
-                    k = 1
-                func = CardConstr(weight, scale, shift, k)
+                if not relax:
+                    if "args" in g and "k" in g["args"]:
+                        k = g["args"]["k"]
+                    else:
+                        k = 1
+                    func = CardConstr(weight, scale, shift, k)
+                else:
+                    # TODO: check this relaxation
+                    func = Abs(1e-1, scale, shift)
             elif name == "quantile":
                 if "args" in g and "tau" in g["args"]:
                     tau = g["args"]["tau"]
                 else:
                     tau = 0.5
                 func = Quantile(weight, scale, shift, tau)
             elif name == "huber":
@@ -548,23 +552,32 @@
                     M = g["args"]["M"]
                     if M <= 0:
                         raise ValueError("Huber parameter M must be > 0.")
                 else:
                     M = 1
                 func = Huber(weight, scale, shift, M)
             elif name == "is_int":
-                func = IsInt(weight, scale, shift)
+                if not relax:
+                    func = IsInt(weight, scale, shift)
+                else:
+                    func = Zero(weight, scale, shift)
             elif name == "is_finite_set":
                 if "args" in g and "S" in g["args"]:
-                    S = g["args"]["S"]
+                    value_set = g["args"]["S"]
                 else:
                     raise ValueError("is_finite_set set must be specified.")
-                func = IsFiniteSet(weight, scale, shift, S)
+                if not relax:
+                    func = IsFiniteSet(weight, scale, shift, value_set)
+                else:
+                    func = IsBound(weight, scale, shift, min(value_set), max(value_set))
             elif name == "is_bool":
-                func = IsBool(weight, scale, shift)
+                if not relax:
+                    func = IsBool(weight, scale, shift)
+                else:
+                    func = IsBound(weight, scale, shift, 0, 1)
 
             if not func._is_convex:
                 self._is_convex = False
             self._g_list.append({"range": range, "func": func})
 
             if name != "zero":
                 self._all_zeros = False
```

### Comparing `qss-0.1.6/qss/qss.py` & `qss-0.2.2/qss/qss.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,31 +18,30 @@
         data,
     ):
 
         # Checking quadratic part
         if "P" not in data:
             raise ValueError("P matrix must be specified.")
 
-        self._data = {}
-        self._data["dim"] = data["P"].shape[0]
+        data_dim = data["P"].shape[0]
 
         if "q" not in data:
             raise ValueError("q vector must be specified.")
         if "r" not in data:
             raise ValueError("r scalar must be specified.")
         if data["P"].shape[0] != data["P"].shape[1]:
             raise ValueError("P must be a square matrix")
-        if len(data["q"]) != self._data["dim"]:
+        if len(data["q"]) != data_dim:
             raise ValueError("q dimensions must correspond to P.")
 
         # Checking constraints
         if "A" in data and data["A"] is not None:
             if "b" not in data or data["b"] is None:
                 raise ValueError("Constraint vector not specified.")
-            if data["A"].shape[1] != self._data["dim"]:
+            if data["A"].shape[1] != data_dim:
                 raise ValueError(
                     "Constraint matrix column number must correspond to P."
                 )
             if data["A"].shape[0] != len(data["b"]):
                 raise ValueError("A and b dimensions must correspond.")
 
         if "b" in data and data["b"] is not None:
@@ -58,54 +57,31 @@
                 if "weight" in "args":
                     if g["args"]["weight"] < 0:
                         raise ValueError("Weight must be >= 0.")
             if "range" not in g:
                 raise ValueError("g function range must be specified.")
             if g["range"][0] < 0:
                 raise ValueError("Range out of bounds.")
-            if g["range"][1] > self._data["dim"]:
+            if g["range"][1] > data_dim:
                 raise ValueError("Range out of bounds.")
             if g["range"][0] > g["range"][1]:
                 raise ValueError("Start index must be <= end index.")
             ranges.append(g["range"])
         ranges = sorted(ranges, key=lambda x: x[0])
         for i in range(len(ranges) - 1):
             if ranges[i][1] > ranges[i + 1][0]:
                 raise ValueError("g function ranges must not overlap.")
 
         # Making copies of the input data and storing
-        if type(data["P"]) is not linearoperator.LinearOperator:
-            self._data["P"] = data["P"].copy()
+        self._data = util.copy_problem_data(data)
+        
+        if self._data["g"]._is_convex:
+            self._relaxed_data = None
         else:
-            self._data["P"] = data["P"]
-        self._data["q"] = np.copy(data["q"])
-        self._data["r"] = data["r"]
-        self._data["g"] = proximal.GCollection(data["g"], self._data["dim"])
-
-        self._data["abstract_constr"] = False
-        if ("A" in data) and (type(data["A"]) is linearoperator.LinearOperator):
-            self._data["A"] = data["A"]  # TODO: in future, copy w/ linop .copy()
-            self._data["b"] = np.copy(data["b"])
-            self._data["abstract_constr"] = True
-            self._data["has_constr"] = True
-            self._data["constr_dim"] = data["A"].shape[0]
-        elif ("A" not in data) or (data["A"] is None) or (data["A"].nnz == 0):
-            # TODO: get rid of this placeholder when QSS is more object-oriented, i.e.,
-            # when all problem data is passed around together.
-            # I'm using the placeholder for now to avoid littering precondition.py with
-            # 'if' statements.
-            self._data["A"] = sp.sparse.csc_matrix((1, self._data["dim"]))
-            self._data["b"] = np.zeros(1)
-            self._data["has_constr"] = False
-            self._data["constr_dim"] = 1
-        else:
-            self._data["A"] = data["A"].copy()
-            self._data["b"] = np.copy(data["b"])
-            self._data["has_constr"] = True
-            self._data["constr_dim"] = data["A"].shape[0]
+            self._relaxed_data = util.copy_problem_data(data, relax=True)
 
         # Unscaled data
         self._unscaled_data = {}
 
         # Scaling information
         self._scaling = {}
         self._reset_scaling()
@@ -135,14 +111,15 @@
         self._options["line_search"] = None
         self._options["algorithms"] = None
         self._options["rho_update"] = None
         self._options["schedule_alpha"] = None
         self._options["random_init"] = None
         self._options["init_seed"] = None
         self._options["verbose"] = None
+        self._options["debug"] = None
         return
 
     def _reset_scaling(self):
         self._scaling["equil_scaling"] = np.ones(self._data["dim"])
         self._scaling["obj_scale"] = 1
 
     def _reset_iterates(self, random=False):
@@ -164,27 +141,28 @@
 
     def solve(
         self,
         eps_abs=1e-5,
         eps_rel=1e-5,
         alpha=1.4,
         rho=0.1,
-        max_iter=[np.inf],
+        max_iter=10000,
         precond=False,
         warm_start=False,
         reg=True,
         use_iter_refinement=False,
         descent_method="momentum",
         line_search=True,
         algorithms=["admm"],
         rho_update="adaptive",
         schedule_alpha=False,
         random_init=False,
         init_seed=1234,
         verbose=False,
+        debug=False
     ):
 
         self._options["eps_abs"] = eps_abs
         self._options["eps_rel"] = eps_rel
         self._options["alpha"] = alpha
         self._options["rho"] = rho
         self._options["max_iter"] = max_iter
@@ -196,23 +174,25 @@
         self._options["line_search"] = line_search
         self._options["algorithms"] = algorithms
         self._options["rho_update"] = rho_update
         self._options["schedule_alpha"] = schedule_alpha
         self._options["random_init"] = random_init
         self._options["init_seed"] = init_seed
         self._options["verbose"] = verbose
+        self._options["debug"] = debug
 
         np.random.seed(1234)
 
         if self._options["verbose"]:
             util.print_info()
             start_time = time.time()
 
         # Reset problem parameters if not warm starting
         if not self._options["warm_start"]:
+            if self._options["debug"]: print('### DEBUG ###\nresetting iterates\n#############')
             self._reset_iterates(self._options["random_init"])
             self._rho_controller = None
 
         # Preconditioning
         if self._options["precond"] and not self._data["abstract_constr"]:
             if self._options["verbose"]:
                 precond_start_time = time.time()
@@ -250,23 +230,22 @@
                 "{} {}{}".format(
                     "initial factorization time:".ljust(util.BULLET_WIDTH),
                     format(time.time() - factorization_start_time, ".2e"),
                     "s",
                 )
             )
 
-        if self._data["g"]._is_convex or not self._options["rho_update"] == "schedule":
-            max_iter_list = self._options[
-                "max_iter"
-            ]  # TODO get rid of this or make more elegant
-            if type(max_iter_list) is int:
-                max_iter_list = [max_iter_list]
-            if type(max_iter_list) is not list:
-                raise ValueError("max_iter should be an integer or a list.")
-            for i, algorithm in enumerate(algorithms):
+        if self._data["g"]._is_convex and not self._options["rho_update"] == "schedule":
+            if self._options["verbose"]:
+                print('(standard algorithm)')
+            max_iter_list = np.atleast_1d(self._options["max_iter"])
+            if not (isinstance(max_iter_list[0], int)
+                    or isinstance(max_iter_list[0], np.int64)):
+                raise ValueError("max_iter should be an integer or a list of integers.")
+            for i, algorithm in enumerate(np.atleast_1d(algorithms)):
                 if i == 0 and algorithm == "proj_sd":
                     self._iterates["x"] = sp.sparse.linalg.lsqr(
                         self._data["A"], self._data["b"], atol=1e-12, btol=1e-12
                     )[0]
                 self._options["max_iter"] = max_iter_list[i]
                 if algorithm == "proj_sd":
                     self._iterates = descent.proj_sd(
@@ -285,16 +264,43 @@
                         **self._iterates,
                         **self._scaling,
                     )
                 else:
                     raise ValueError("Invalid algorithm specified")
 
             self._options["max_iter"] = max_iter_list
+        elif not self._data["g"]._is_convex:
+            if self._options["verbose"]:
+                print('(nonconvex warm-start algorithm)')
+            max_iter_list = np.atleast_1d(self._options["max_iter"])
+            if not (isinstance(max_iter_list[0], int)
+                    or isinstance(max_iter_list[0], np.int64)):
+                raise ValueError("max_iter should be an integer or a list of integers.")
+            # I am only implementing this for ADMM --BM 4/4/23
+            if len(max_iter_list) == 1:
+                max_iter_list = np.r_[max_iter_list, max_iter_list]
+            data_list = [self._relaxed_data, self._data]
+            warm_start_list = [False, True]
+
+            for i, data in enumerate(data_list):
+                self._options["max_iter"] = max_iter_list[i]
+                self._options["warm_start"] = warm_start_list[i]
+                self._iterates = admm.admm(
+                    data,
+                    self._kkt_system,
+                    self._options,
+                    self._rho_controller,
+                    **self._iterates,
+                    **self._scaling,
+                )
 
+            self._options["max_iter"] = max_iter_list
         else:
+            if self._options["verbose"]:
+                print('(scheduled algorithm)')
             orig_max_iter = self._options["max_iter"]
             orig_rho = self._options["rho"]
             orig_warm_start = self._options["warm_start"]
 
             num_rhos = 5
             max_rho = 1e3
```

### Comparing `qss-0.1.6/qss.egg-info/PKG-INFO` & `qss-0.2.2/qss.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qss
-Version: 0.1.6
+Version: 0.2.2
 Summary: QSS: Quadratic-Separable Solver
 Home-page: https://github.com/lukevolpatti/qss
 Author: Luke Volpatti
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/lukevolpatti/qss/issues
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `qss-0.1.6/setup.py` & `qss-0.2.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="qss",
-    version="0.1.6",
+    version="0.2.2",
     author="Luke Volpatti",
     description="QSS: Quadratic-Separable Solver",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["numpy", "scipy", "qdldl", "cvxpy"],
     url="https://github.com/lukevolpatti/qss",
     project_urls={
```

