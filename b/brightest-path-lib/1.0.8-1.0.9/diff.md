# Comparing `tmp/brightest-path-lib-1.0.8.tar.gz` & `tmp/brightest-path-lib-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brightest-path-lib-1.0.8.tar", last modified: Tue Apr 18 17:50:50 2023, max compression
+gzip compressed data, was "brightest-path-lib-1.0.9.tar", last modified: Tue Apr 18 19:04:41 2023, max compression
```

## Comparing `brightest-path-lib-1.0.8.tar` & `brightest-path-lib-1.0.9.tar`

### file list

```diff
@@ -1,32 +1,55 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 17:50:50.461558 brightest-path-lib-1.0.8/
--rw-r--r--   0 runner     (501) staff       (20)    35148 2023-04-18 17:50:00.000000 brightest-path-lib-1.0.8/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      115 2023-04-18 17:50:00.000000 brightest-path-lib-1.0.8/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)      601 2023-04-18 17:50:50.461182 brightest-path-lib-1.0.8/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1493 2023-04-18 17:50:00.000000 brightest-path-lib-1.0.8/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 17:50:50.449508 brightest-path-lib-1.0.8/brightest_path_lib/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 17:50:50.455358 brightest-path-lib-1.0.8/brightest_path_lib/cost/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 17:50:50.455839 brightest-path-lib-1.0.8/brightest_path_lib/cost/__pythran__/
--rw-------   0 runner     (501) staff       (20)    19226 2023-04-18 17:50:50.000000 brightest-path-lib-1.0.8/brightest_path_lib/cost/__pythran__/reciprocal_transonic.cpp
--rw-r--r--   0 runner     (501) staff       (20)     2739 2023-04-18 17:50:00.000000 brightest-path-lib-1.0.8/brightest_path_lib/cost/reciprocal_transonic.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 17:50:50.456400 brightest-path-lib-1.0.8/brightest_path_lib/heuristic/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 17:50:50.456848 brightest-path-lib-1.0.8/brightest_path_lib/heuristic/__pythran__/
--rw-------   0 runner     (501) staff       (20)    34397 2023-04-18 17:50:50.000000 brightest-path-lib-1.0.8/brightest_path_lib/heuristic/__pythran__/euclidean_transonic.cpp
--rw-r--r--   0 runner     (501) staff       (20)     3309 2023-04-18 17:50:00.000000 brightest-path-lib-1.0.8/brightest_path_lib/heuristic/euclidean_transonic.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 17:50:50.454824 brightest-path-lib-1.0.8/brightest_path_lib.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)      601 2023-04-18 17:50:49.000000 brightest-path-lib-1.0.8/brightest_path_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      710 2023-04-18 17:50:50.000000 brightest-path-lib-1.0.8/brightest_path_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-18 17:50:49.000000 brightest-path-lib-1.0.8/brightest_path_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)      146 2023-04-18 17:50:49.000000 brightest-path-lib-1.0.8/brightest_path_lib.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       19 2023-04-18 17:50:49.000000 brightest-path-lib-1.0.8/brightest_path_lib.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)      121 2023-04-18 17:50:00.000000 brightest-path-lib-1.0.8/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)       38 2023-04-18 17:50:50.461671 brightest-path-lib-1.0.8/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     2568 2023-04-18 17:50:00.000000 brightest-path-lib-1.0.8/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 17:50:50.460630 brightest-path-lib-1.0.8/tests/
--rw-r--r--   0 runner     (501) staff       (20)     4514 2023-04-18 17:50:00.000000 brightest-path-lib-1.0.8/tests/test_astar.py
--rw-r--r--   0 runner     (501) staff       (20)     1874 2023-04-18 17:50:00.000000 brightest-path-lib-1.0.8/tests/test_bidirectional_node.py
--rw-r--r--   0 runner     (501) staff       (20)      611 2023-04-18 17:50:00.000000 brightest-path-lib-1.0.8/tests/test_brightest_path_lib.py
--rw-r--r--   0 runner     (501) staff       (20)     1919 2023-04-18 17:50:00.000000 brightest-path-lib-1.0.8/tests/test_euclidean_heuristic.py
--rw-r--r--   0 runner     (501) staff       (20)     1586 2023-04-18 17:50:00.000000 brightest-path-lib-1.0.8/tests/test_image_stats.py
--rw-r--r--   0 runner     (501) staff       (20)     4700 2023-04-18 17:50:00.000000 brightest-path-lib-1.0.8/tests/test_nbastar.py
--rw-r--r--   0 runner     (501) staff       (20)     1065 2023-04-18 17:50:00.000000 brightest-path-lib-1.0.8/tests/test_node.py
--rw-r--r--   0 runner     (501) staff       (20)     1591 2023-04-18 17:50:00.000000 brightest-path-lib-1.0.8/tests/test_reciprocal_cost_func.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 19:04:41.666605 brightest-path-lib-1.0.9/
+-rw-r--r--   0 runner     (501) staff       (20)    35148 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      115 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)      601 2023-04-18 19:04:41.666179 brightest-path-lib-1.0.9/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1493 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 19:04:41.649041 brightest-path-lib-1.0.9/brightest_path_lib/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/brightest_path_lib/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 19:04:41.652911 brightest-path-lib-1.0.9/brightest_path_lib/algorithm/
+-rw-r--r--   0 runner     (501) staff       (20)       65 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/brightest_path_lib/algorithm/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    16504 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/brightest_path_lib/algorithm/astar.py
+-rw-r--r--   0 runner     (501) staff       (20)    24691 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/brightest_path_lib/algorithm/nbastar.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 19:04:41.655136 brightest-path-lib-1.0.9/brightest_path_lib/cost/
+-rw-r--r--   0 runner     (501) staff       (20)      112 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/brightest_path_lib/cost/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 19:04:41.655723 brightest-path-lib-1.0.9/brightest_path_lib/cost/__pythran__/
+-rw-------   0 runner     (501) staff       (20)    19226 2023-04-18 19:04:41.000000 brightest-path-lib-1.0.9/brightest_path_lib/cost/__pythran__/reciprocal_transonic.cpp
+-rw-r--r--   0 runner     (501) staff       (20)      788 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/brightest_path_lib/cost/cost.py
+-rw-r--r--   0 runner     (501) staff       (20)     2542 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/brightest_path_lib/cost/reciprocal.py
+-rw-r--r--   0 runner     (501) staff       (20)     2739 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/brightest_path_lib/cost/reciprocal_transonic.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 19:04:41.657547 brightest-path-lib-1.0.9/brightest_path_lib/heuristic/
+-rw-r--r--   0 runner     (501) staff       (20)      118 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/brightest_path_lib/heuristic/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 19:04:41.658038 brightest-path-lib-1.0.9/brightest_path_lib/heuristic/__pythran__/
+-rw-------   0 runner     (501) staff       (20)    34397 2023-04-18 19:04:41.000000 brightest-path-lib-1.0.9/brightest_path_lib/heuristic/__pythran__/euclidean_transonic.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     2888 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/brightest_path_lib/heuristic/euclidean.py
+-rw-r--r--   0 runner     (501) staff       (20)     3309 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/brightest_path_lib/heuristic/euclidean_transonic.py
+-rw-r--r--   0 runner     (501) staff       (20)      936 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/brightest_path_lib/heuristic/heuristic.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 19:04:41.659216 brightest-path-lib-1.0.9/brightest_path_lib/image/
+-rw-r--r--   0 runner     (501) staff       (20)       29 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/brightest_path_lib/image/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3369 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/brightest_path_lib/image/stats.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 19:04:41.660375 brightest-path-lib-1.0.9/brightest_path_lib/input/
+-rw-r--r--   0 runner     (501) staff       (20)       67 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/brightest_path_lib/input/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      290 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/brightest_path_lib/input/inputs.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 19:04:41.661827 brightest-path-lib-1.0.9/brightest_path_lib/node/
+-rw-r--r--   0 runner     (501) staff       (20)       72 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/brightest_path_lib/node/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5996 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/brightest_path_lib/node/bidirectional_node.py
+-rw-r--r--   0 runner     (501) staff       (20)     2406 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/brightest_path_lib/node/node.py
+-rw-r--r--   0 runner     (501) staff       (20)     4132 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/brightest_path_lib/sandbox.py
+-rw-r--r--   0 runner     (501) staff       (20)     4209 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/brightest_path_lib/sandbox2.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 19:04:41.651459 brightest-path-lib-1.0.9/brightest_path_lib.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)      601 2023-04-18 19:04:41.000000 brightest-path-lib-1.0.9/brightest_path_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1409 2023-04-18 19:04:41.000000 brightest-path-lib-1.0.9/brightest_path_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-18 19:04:41.000000 brightest-path-lib-1.0.9/brightest_path_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)      146 2023-04-18 19:04:41.000000 brightest-path-lib-1.0.9/brightest_path_lib.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       19 2023-04-18 19:04:41.000000 brightest-path-lib-1.0.9/brightest_path_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)      121 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)       38 2023-04-18 19:04:41.666722 brightest-path-lib-1.0.9/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     2602 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 19:04:41.665542 brightest-path-lib-1.0.9/tests/
+-rw-r--r--   0 runner     (501) staff       (20)     4514 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/tests/test_astar.py
+-rw-r--r--   0 runner     (501) staff       (20)     1874 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/tests/test_bidirectional_node.py
+-rw-r--r--   0 runner     (501) staff       (20)      611 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/tests/test_brightest_path_lib.py
+-rw-r--r--   0 runner     (501) staff       (20)     1919 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/tests/test_euclidean_heuristic.py
+-rw-r--r--   0 runner     (501) staff       (20)     1586 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/tests/test_image_stats.py
+-rw-r--r--   0 runner     (501) staff       (20)     4700 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/tests/test_nbastar.py
+-rw-r--r--   0 runner     (501) staff       (20)     1065 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/tests/test_node.py
+-rw-r--r--   0 runner     (501) staff       (20)     1591 2023-04-18 19:03:54.000000 brightest-path-lib-1.0.9/tests/test_reciprocal_cost_func.py
```

### Comparing `brightest-path-lib-1.0.8/LICENSE` & `brightest-path-lib-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.8/PKG-INFO` & `brightest-path-lib-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brightest-path-lib
-Version: 1.0.8
+Version: 1.0.9
 Summary: A library of path-finding algorithms to find the brightest path between two points.
 Home-page: https://github.com/mapmanager/brightest-path-lib
 Author: Vasudha Jha
 License: GNU General Public License, Version 3
 Project-URL: Issues, https://github.com/mapmanager/brightest-path-lib/issues
 Project-URL: CI, https://github.com/mapmanager/brightest-path-lib/actions
 Project-URL: Changelog, https://github.com/mapmanager/brightest-path-lib/releases
```

### Comparing `brightest-path-lib-1.0.8/README.md` & `brightest-path-lib-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.8/brightest_path_lib/cost/__pythran__/reciprocal_transonic.cpp` & `brightest-path-lib-1.0.9/brightest_path_lib/cost/__pythran__/reciprocal_transonic.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -298,15 +298,15 @@
 
 
 static PyMethodDef Methods[] = {
     {
     "__for_method__ReciprocalTransonic__minimum_step_cost",
     (PyCFunction)__pythran_wrapall___for_method__ReciprocalTransonic__minimum_step_cost,
     METH_VARARGS | METH_KEYWORDS,
-    "calculates the minimum step cost\n""\n""    Supported prototypes:\n""\n""    - __for_method__ReciprocalTransonic__minimum_step_cost(float64)\n""\n""        Returns\n""        -------\n""        float\n""            the minimum step cost\n"""},{
+    "calculates the minimum step cost\n""\n""        Returns\n""        -------\n""        float\n""            the minimum step cost\n""\n""\n""    Supported prototypes:\n""\n""    - __for_method__ReciprocalTransonic__minimum_step_cost(float64)"},{
     "__for_method__ReciprocalTransonic__cost_of_moving_to",
     (PyCFunction)__pythran_wrapall___for_method__ReciprocalTransonic__cost_of_moving_to,
     METH_VARARGS | METH_KEYWORDS,
     "calculates the cost of moving to a point\n""\n""    Supported prototypes:\n""\n""    - __for_method__ReciprocalTransonic__cost_of_moving_to(float64, float64, float64, float64, float64)\n""\n""        Parameters\n""        ----------\n""        intensity_at_new_point : float\n""            The intensity of the new point under consideration\n""\n""        Returns\n""        -------\n""        float\n""            the cost of moving to the new point\n""\n""        Notes\n""        -----\n""        - To cope with zero intensities, RECIPROCAL_MIN is added to the intensities in the range before reciprocal calculation\n""        - We set the maximum intensity <= RECIPROCAL_MAX so that the intensity is between RECIPROCAL MIN and RECIPROCAL_MAX\n""\n"""},
     {NULL, NULL, 0, NULL}
 };
 
@@ -349,16 +349,16 @@
                                                      ""
                 );
                 #endif
                 if(! theModule)
                     PYTHRAN_RETURN;
                 PyObject * theDoc = Py_BuildValue("(sss)",
                                                   "0.12.1",
-                                                  "2023-04-18 17:50:50.438816",
-                                                  "837ab9168b906b083b44ff44080768d36d3cd2f0bf45a5bc7adc69f2e573c716");
+                                                  "2023-04-18 19:04:41.632359",
+                                                  "437594492678aa5480d24b4e8550f8810fb608091fdbb308aa7037a9dc92c24f");
                 if(! theDoc)
                     PYTHRAN_RETURN;
                 PyModule_AddObject(theModule,
                                    "__pythran__",
                                    theDoc);
 
                 PyModule_AddObject(theModule, "__transonic__", __transonic__);
```

### Comparing `brightest-path-lib-1.0.8/brightest_path_lib/cost/reciprocal_transonic.py` & `brightest-path-lib-1.0.9/brightest_path_lib/cost/reciprocal_transonic.py`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.8/brightest_path_lib/heuristic/__pythran__/euclidean_transonic.cpp` & `brightest-path-lib-1.0.9/brightest_path_lib/heuristic/__pythran__/euclidean_transonic.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 #ifdef _OPENMP
 #include <omp.h>
 #endif
 #include <pythonic/include/types/ndarray.hpp>
 #include <pythonic/include/types/float64.hpp>
 #include <pythonic/include/types/int64.hpp>
 #include <pythonic/types/float64.hpp>
-#include <pythonic/types/ndarray.hpp>
 #include <pythonic/types/int64.hpp>
+#include <pythonic/types/ndarray.hpp>
 #include <pythonic/include/builtins/TypeError.hpp>
 #include <pythonic/include/builtins/ValueError.hpp>
 #include <pythonic/include/builtins/len.hpp>
 #include <pythonic/include/builtins/pythran/is_none.hpp>
 #include <pythonic/include/builtins/pythran/or_.hpp>
 #include <pythonic/include/builtins/pythran/static_if.hpp>
 #include <pythonic/include/builtins/tuple.hpp>
@@ -509,16 +509,16 @@
                                                      ""
                 );
                 #endif
                 if(! theModule)
                     PYTHRAN_RETURN;
                 PyObject * theDoc = Py_BuildValue("(sss)",
                                                   "0.12.1",
-                                                  "2023-04-18 17:50:50.344238",
-                                                  "c05d11336916ffc5577dc142faff358aeb635b45ebb631a4918a6d5f79c4c890");
+                                                  "2023-04-18 19:04:41.512778",
+                                                  "c851a0a3829d72e9a86f3c46e4c833fc15e1ae5d90eab8ca29115df81a059458");
                 if(! theDoc)
                     PYTHRAN_RETURN;
                 PyModule_AddObject(theModule,
                                    "__pythran__",
                                    theDoc);
 
                 PyModule_AddObject(theModule, "__transonic__", __transonic__);
```

### Comparing `brightest-path-lib-1.0.8/brightest_path_lib/heuristic/euclidean_transonic.py` & `brightest-path-lib-1.0.9/brightest_path_lib/heuristic/euclidean_transonic.py`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.8/brightest_path_lib.egg-info/PKG-INFO` & `brightest-path-lib-1.0.9/brightest_path_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brightest-path-lib
-Version: 1.0.8
+Version: 1.0.9
 Summary: A library of path-finding algorithms to find the brightest path between two points.
 Home-page: https://github.com/mapmanager/brightest-path-lib
 Author: Vasudha Jha
 License: GNU General Public License, Version 3
 Project-URL: Issues, https://github.com/mapmanager/brightest-path-lib/issues
 Project-URL: CI, https://github.com/mapmanager/brightest-path-lib/actions
 Project-URL: Changelog, https://github.com/mapmanager/brightest-path-lib/releases
```

### Comparing `brightest-path-lib-1.0.8/setup.py` & `brightest-path-lib-1.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 import sys
 from transonic.dist import ParallelBuildExt, make_backend_files, init_transonic_extensions
 
 here = Path(__file__).parent.absolute()
 sys.path.insert(0, ".")
 
-VERSION = "1.0.8"
+VERSION = "1.0.9"
 TRANSONIC_BACKEND = "pythran"
 
 build_dependencies_backends = {
     "pythran": ["pythran"],
     "cython": ["cython"],
     "python": [],
     "numba": ["numba"],
@@ -44,14 +44,20 @@
     return extensions
 
 
 def create_extensions():
     transonize()
     return create_pythran_extensions()
 
+# packages = find_packages(include=[
+#         "brightest_path_lib",
+#         "brightest_path_lib.*",
+#         ])
+packages = find_packages(exclude=["tests"])
+print(f"found packages: {packages}")
 
 setup(
     name="brightest-path-lib",
     description="A library of path-finding algorithms to find the brightest path between two points.",
     author="Vasudha Jha",
     url="https://github.com/mapmanager/brightest-path-lib",
     project_urls={
@@ -59,20 +65,15 @@
         "CI": "https://github.com/mapmanager/brightest-path-lib/actions",
         "Changelog": "https://github.com/mapmanager/brightest-path-lib/releases",
     },
     license="GNU General Public License, Version 3",
     version=VERSION,
     #packages=["brightest_path_lib"],
     #packages=find_packages(),
-    packages=find_packages(include=[
-        "brightest_path_lib",
-        "brightest_path_lib.*",
-        "brightest_path_lib.algorithm",
-        "brightest_path_lib.input"
-        ]),
+    packages=packages,
     setup_requires=setup_requires,
     install_requires=["numpy", "transonic"],
     extras_require={
         'dev': [
             'mkdocs',
             'mkdocs-material',
             'mkdocs-jupyter',
```

### Comparing `brightest-path-lib-1.0.8/tests/test_astar.py` & `brightest-path-lib-1.0.9/tests/test_astar.py`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.8/tests/test_bidirectional_node.py` & `brightest-path-lib-1.0.9/tests/test_bidirectional_node.py`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.8/tests/test_brightest_path_lib.py` & `brightest-path-lib-1.0.9/tests/test_brightest_path_lib.py`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.8/tests/test_euclidean_heuristic.py` & `brightest-path-lib-1.0.9/tests/test_euclidean_heuristic.py`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.8/tests/test_image_stats.py` & `brightest-path-lib-1.0.9/tests/test_image_stats.py`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.8/tests/test_nbastar.py` & `brightest-path-lib-1.0.9/tests/test_nbastar.py`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.8/tests/test_node.py` & `brightest-path-lib-1.0.9/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.8/tests/test_reciprocal_cost_func.py` & `brightest-path-lib-1.0.9/tests/test_reciprocal_cost_func.py`

 * *Files identical despite different names*

