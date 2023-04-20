# Comparing `tmp/ross-rotordynamics-1.3.0.tar.gz` & `tmp/ross-rotordynamics-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/ross/ross/dist/tmpi4ou0isl/ross-rotordynamics-1.3.0.tar", last modified: Wed Nov 16 01:38:34 2022, max compression
+gzip compressed data, was "/home/runner/work/ross/ross/dist/.tmp-hnobonsc/ross-rotordynamics-1.4.0.tar", last modified: Thu Apr 20 18:44:52 2023, max compression
```

## Comparing `ross-rotordynamics-1.3.0.tar` & `ross-rotordynamics-1.4.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-16 01:38:34.000000 ross-rotordynamics-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (116)     1082 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (116)       62 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     2963 2022-11-16 01:38:34.000000 ross-rotordynamics-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2351 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       69 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-16 01:38:34.000000 ross-rotordynamics-1.3.0/ross/
--rw-r--r--   0 runner    (1001) docker     (116)      412 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    63674 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/bearing_seal_element.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-16 01:38:34.000000 ross-rotordynamics-1.3.0/ross/defects/
--rw-r--r--   0 runner    (1001) docker     (116)      104 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/defects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4271 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/defects/abs_defect.py
--rw-r--r--   0 runner    (1001) docker     (116)    20689 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/defects/crack.py
--rw-r--r--   0 runner    (1001) docker     (116)     4465 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/defects/integrate_solver.py
--rw-r--r--   0 runner    (1001) docker     (116)    34531 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/defects/misalignment.py
--rw-r--r--   0 runner    (1001) docker     (116)    16372 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/defects/rubbing.py
--rw-r--r--   0 runner    (1001) docker     (116)    22254 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/disk_element.py
--rw-r--r--   0 runner    (1001) docker     (116)     6760 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/element.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-16 01:38:34.000000 ross-rotordynamics-1.3.0/ross/fluid_flow/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/fluid_flow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    75694 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/fluid_flow/cylindrical.py
--rw-r--r--   0 runner    (1001) docker     (116)    33198 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/fluid_flow/fluid_flow.py
--rw-r--r--   0 runner    (1001) docker     (116)    16708 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/fluid_flow/fluid_flow_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (116)    15557 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/fluid_flow/fluid_flow_geometry.py
--rw-r--r--   0 runner    (1001) docker     (116)    19667 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/fluid_flow/fluid_flow_graphics.py
--rw-r--r--   0 runner    (1001) docker     (116)     8000 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/materials.py
--rw-r--r--   0 runner    (1001) docker     (116)       74 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/new_units.txt
--rw-r--r--   0 runner    (1001) docker     (116)    13358 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/plotly_theme.py
--rw-r--r--   0 runner    (1001) docker     (116)     9045 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/point_mass.py
--rw-r--r--   0 runner    (1001) docker     (116)   160006 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/results.py
--rw-r--r--   0 runner    (1001) docker     (116)   142384 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/rotor_assembly.py
--rw-r--r--   0 runner    (1001) docker     (116)    78648 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/shaft_element.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-16 01:38:34.000000 ross-rotordynamics-1.3.0/ross/stochastic/
--rw-r--r--   0 runner    (1001) docker     (116)      218 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/stochastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    18630 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/stochastic/st_bearing_seal_element.py
--rw-r--r--   0 runner    (1001) docker     (116)    11343 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/stochastic/st_disk_element.py
--rw-r--r--   0 runner    (1001) docker     (116)     8599 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/stochastic/st_materials.py
--rw-r--r--   0 runner    (1001) docker     (116)     8306 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/stochastic/st_point_mass.py
--rw-r--r--   0 runner    (1001) docker     (116)    82817 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/stochastic/st_results.py
--rw-r--r--   0 runner    (1001) docker     (116)     4005 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/stochastic/st_results_elements.py
--rw-r--r--   0 runner    (1001) docker     (116)    31534 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/stochastic/st_rotor_assembly.py
--rw-r--r--   0 runner    (1001) docker     (116)    11298 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/stochastic/st_shaft_element.py
--rw-r--r--   0 runner    (1001) docker     (116)     4937 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/units.py
--rw-r--r--   0 runner    (1001) docker     (116)    21787 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/ross/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-16 01:38:34.000000 ross-rotordynamics-1.3.0/ross_rotordynamics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2963 2022-11-16 01:38:34.000000 ross-rotordynamics-1.3.0/ross_rotordynamics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1209 2022-11-16 01:38:34.000000 ross-rotordynamics-1.3.0/ross_rotordynamics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-11-16 01:38:34.000000 ross-rotordynamics-1.3.0/ross_rotordynamics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      258 2022-11-16 01:38:34.000000 ross-rotordynamics-1.3.0/ross_rotordynamics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        5 2022-11-16 01:38:34.000000 ross-rotordynamics-1.3.0/ross_rotordynamics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      113 2022-11-16 01:38:34.000000 ross-rotordynamics-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     3260 2022-11-16 01:38:24.000000 ross-rotordynamics-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:44:52.000000 ross-rotordynamics-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-04-20 18:44:37.000000 ross-rotordynamics-1.4.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-20 18:44:37.000000 ross-rotordynamics-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-20 18:44:52.000000 ross-rotordynamics-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-20 18:44:37.000000 ross-rotordynamics-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:44:52.000000 ross-rotordynamics-1.4.0/ross/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63592 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/bearing_seal_element.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:44:52.000000 ross-rotordynamics-1.4.0/ross/defects/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/defects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/defects/abs_defect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/defects/crack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/defects/integrate_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34531 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/defects/misalignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16371 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/defects/rubbing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22254 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/disk_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/element.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:44:52.000000 ross-rotordynamics-1.4.0/ross/fluid_flow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/fluid_flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113322 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/fluid_flow/cylindrical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33197 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/fluid_flow/fluid_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16708 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/fluid_flow/fluid_flow_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15557 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/fluid_flow/fluid_flow_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19667 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/fluid_flow/fluid_flow_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/new_units.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/plotly_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9045 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/point_mass.py
+-rw-r--r--   0 runner    (1001) docker     (123)   160210 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)   142548 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/rotor_assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78702 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/shaft_element.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:44:52.000000 ross-rotordynamics-1.4.0/ross/stochastic/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/stochastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18629 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/stochastic/st_bearing_seal_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/stochastic/st_disk_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/stochastic/st_materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8306 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/stochastic/st_point_mass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82816 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/stochastic/st_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/stochastic/st_results_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31534 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/stochastic/st_rotor_assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/stochastic/st_shaft_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21798 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/ross/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:44:52.000000 ross-rotordynamics-1.4.0/ross_rotordynamics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-20 18:44:52.000000 ross-rotordynamics-1.4.0/ross_rotordynamics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-20 18:44:52.000000 ross-rotordynamics-1.4.0/ross_rotordynamics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 18:44:52.000000 ross-rotordynamics-1.4.0/ross_rotordynamics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-20 18:44:52.000000 ross-rotordynamics-1.4.0/ross_rotordynamics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-20 18:44:52.000000 ross-rotordynamics-1.4.0/ross_rotordynamics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-20 18:44:52.000000 ross-rotordynamics-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-04-20 18:44:38.000000 ross-rotordynamics-1.4.0/setup.py
```

### Comparing `ross-rotordynamics-1.3.0/PKG-INFO` & `ross-rotordynamics-1.4.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,38 @@
-Metadata-Version: 2.1
-Name: ross-rotordynamics
-Version: 1.3.0
-Summary: ROSS: Rotordynamic Open Source Software
-Home-page: https://github.com/ross-rotordynamics/ross
-Author: ROSS developers
-Author-email: raphaelts@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.md
-
-
 # Rotordynamic Open Source Software (ROSS)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ross-rotordynamics/ross/1.1.0?filepath=%2Fdocs%2Ftutorials)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ross-rotordynamics/ross/1.4.0?filepath=%2Fdocs%2Ftutorials)
 ![github actions](https://github.com/ross-rotordynamics/ross/workflows/Tests/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/ross/badge/?version=latest)](https://ross.readthedocs.io/en/latest/?badge=latest)
 <a href="https://codecov.io/gh/ross-rotordynamics/ross">
 <img src="https://codecov.io/gh/ross-rotordynamics/ross/branch/master/graph/badge.svg">
 </a>
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.02120/status.svg)](https://doi.org/10.21105/joss.02120)
 
-ROSS is a library written in Python for rotordynamic analysis. It allows the construction of rotor models and their 
-numerical simulation. Shaft elements, as a default, are modeled with the Timoshenko beam theory, which considers shear 
-and rotary inertia effects, and discretized by means of the Finite Element Method. Disks are assumed to be rigid bodies, 
-thus their strain energy is not taken into account. And bearings/seals are included as linear stiffness/damping coefficients.
+ROSS is a Python library for rotordynamic analysis, which allows the construction of rotor models and their numerical
+simulation. Shaft elements are modeled with the Timoshenko beam theory, which considers shear and rotary inertia
+effects, and discretized by means of the Finite Element Method. Disks are assumed to be rigid bodies, thus their strain
+energy is not taken into account. Bearings and seals are included as linear stiffness and damping coefficients.
 
-After defining the elements for the model, you can plot the rotor geometry and runs simulations such as static analysis, 
-Campbell Diagram, mode shapes, frequency response, and time response.
+After defining the elements for the model, you can plot the rotor geometry and run simulations such as static analysis,
+modal analysis, undamped critical speed, frequency response, unbalance response, time response, and more.
 
 You can try it out now by running the tutorial on [binder](https://mybinder.org/v2/gh/ross-rotordynamics/ross/1.1.0?filepath=%2Fdocs%2Ftutorials)
 
 # Documentation 
 Access the documentation [here](https://ross.readthedocs.io/en/latest/index.html).
-There you can find the [installation procedure](https://ross.readthedocs.io/en/latest/getting_started/installation.html), 
+The documentation provides the [installation procedure](https://ross.readthedocs.io/en/latest/getting_started/installation.html), 
 [a tutorial](https://ross.readthedocs.io/en/latest/tutorials/tutorial_part_1.html), 
 [examples](https://ross.readthedocs.io/en/latest/discussions/discussions.html) and the 
 [API reference](https://ross.readthedocs.io/en/latest/references/api.html).
 
 # Questions
-If you have any questions you can use the [Discussions](https://github.com/ross-rotordynamics/ross/discussions) area in the repository.
+If you have any questions, you can use the [Discussions](https://github.com/ross-rotordynamics/ross/discussions) area in the repository.
 
 # Contributing to ROSS
-Check [CONTRIBUTING.rst](https://github.com/ross-rotordynamics/ross/blob/master/CONTRIBUTING.rst). 
+ROSS is a community-driven project. If you want to contribute to the project, please
+check [CONTRIBUTING.rst](https://github.com/ross-rotordynamics/ross/blob/master/CONTRIBUTING.rst). 
+
+The code has been initially developed by Petrobras in cooperation with the Federal University of Rio de Janeiro (UFRJ)
+with contributions from the Federal University from Uberlândia (UFU).
+Currently, Petrobras has a cooperation agreement with UFRJ (LAVI) and UFU (LMEST) to develop and maintain the code.
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,39 +1,36 @@
-Metadata-Version: 2.1 Name: ross-rotordynamics Version: 1.3.0 Summary: ROSS:
-Rotordynamic Open Source Software Home-page: https://github.com/ross-
-rotordynamics/ross Author: ROSS developers Author-email: raphaelts@gmail.com
-License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: Implementation :: CPython Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown Provides-Extra: dev License-File:
-LICENSE.md # Rotordynamic Open Source Software (ROSS) [![Binder](https://
-mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ross-rotordynamics/
-ross/1.1.0?filepath=%2Fdocs%2Ftutorials) ![github actions](https://github.com/
-ross-rotordynamics/ross/workflows/Tests/badge.svg) [![Documentation Status]
-(https://readthedocs.org/projects/ross/badge/?version=latest)](https://
+# Rotordynamic Open Source Software (ROSS) [![Binder](https://mybinder.org/
+badge_logo.svg)](https://mybinder.org/v2/gh/ross-rotordynamics/ross/
+1.4.0?filepath=%2Fdocs%2Ftutorials) ![github actions](https://github.com/ross-
+rotordynamics/ross/workflows/Tests/badge.svg) [![Documentation Status](https://
+readthedocs.org/projects/ross/badge/?version=latest)](https://
 ross.readthedocs.io/en/latest/?badge=latest) [https://codecov.io/gh/ross-
 rotordynamics/ross/branch/master/graph/badge.svg] [![Code style: black](https:/
 /img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/
 black) [![DOI](https://joss.theoj.org/papers/10.21105/joss.02120/status.svg)]
-(https://doi.org/10.21105/joss.02120) ROSS is a library written in Python for
-rotordynamic analysis. It allows the construction of rotor models and their
-numerical simulation. Shaft elements, as a default, are modeled with the
-Timoshenko beam theory, which considers shear and rotary inertia effects, and
-discretized by means of the Finite Element Method. Disks are assumed to be
-rigid bodies, thus their strain energy is not taken into account. And bearings/
-seals are included as linear stiffness/damping coefficients. After defining the
-elements for the model, you can plot the rotor geometry and runs simulations
-such as static analysis, Campbell Diagram, mode shapes, frequency response, and
-time response. You can try it out now by running the tutorial on [binder]
-(https://mybinder.org/v2/gh/ross-rotordynamics/ross/
+(https://doi.org/10.21105/joss.02120) ROSS is a Python library for rotordynamic
+analysis, which allows the construction of rotor models and their numerical
+simulation. Shaft elements are modeled with the Timoshenko beam theory, which
+considers shear and rotary inertia effects, and discretized by means of the
+Finite Element Method. Disks are assumed to be rigid bodies, thus their strain
+energy is not taken into account. Bearings and seals are included as linear
+stiffness and damping coefficients. After defining the elements for the model,
+you can plot the rotor geometry and run simulations such as static analysis,
+modal analysis, undamped critical speed, frequency response, unbalance
+response, time response, and more. You can try it out now by running the
+tutorial on [binder](https://mybinder.org/v2/gh/ross-rotordynamics/ross/
 1.1.0?filepath=%2Fdocs%2Ftutorials) # Documentation Access the documentation
-[here](https://ross.readthedocs.io/en/latest/index.html). There you can find
-the [installation procedure](https://ross.readthedocs.io/en/latest/
+[here](https://ross.readthedocs.io/en/latest/index.html). The documentation
+provides the [installation procedure](https://ross.readthedocs.io/en/latest/
 getting_started/installation.html), [a tutorial](https://ross.readthedocs.io/
 en/latest/tutorials/tutorial_part_1.html), [examples](https://
 ross.readthedocs.io/en/latest/discussions/discussions.html) and the [API
 reference](https://ross.readthedocs.io/en/latest/references/api.html). #
-Questions If you have any questions you can use the [Discussions](https://
+Questions If you have any questions, you can use the [Discussions](https://
 github.com/ross-rotordynamics/ross/discussions) area in the repository. #
-Contributing to ROSS Check [CONTRIBUTING.rst](https://github.com/ross-
-rotordynamics/ross/blob/master/CONTRIBUTING.rst).
+Contributing to ROSS ROSS is a community-driven project. If you want to
+contribute to the project, please check [CONTRIBUTING.rst](https://github.com/
+ross-rotordynamics/ross/blob/master/CONTRIBUTING.rst). The code has been
+initially developed by Petrobras in cooperation with the Federal University of
+Rio de Janeiro (UFRJ) with contributions from the Federal University from
+UberlÃ¢ndia (UFU). Currently, Petrobras has a cooperation agreement with UFRJ
+(LAVI) and UFU (LMEST) to develop and maintain the code.
```

### Comparing `ross-rotordynamics-1.3.0/ross/bearing_seal_element.py` & `ross-rotordynamics-1.4.0/ross/bearing_seal_element.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,16 +159,14 @@
                     raise ValueError(
                         "Arguments (coefficients and frequency)"
                         " must have the same dimension"
                     )
 
         self.n = n
         self.n_link = n_link
-        self.n_l = n
-        self.n_r = n
         self.tag = tag
         self.color = color
         self.scale_factor = scale_factor
         self.dof_global_index = None
 
     def _process_coefficient(self, coefficient):
         """Helper function used to process the coefficient data."""
@@ -1151,15 +1149,14 @@
         alpha,
         cxx=None,
         cyy=None,
         tag=None,
         n_link=None,
         scale_factor=1,
     ):
-
         Kb = 13.0e6
         kyy = (
             Kb
             * n_balls ** (2.0 / 3)
             * d_balls ** (1.0 / 3)
             * fs ** (1.0 / 3)
             * (np.cos(alpha)) ** (5.0 / 3)
@@ -1269,15 +1266,14 @@
         alpha,
         cxx=None,
         cyy=None,
         tag=None,
         n_link=None,
         scale_factor=1,
     ):
-
         Kb = 1.0e9
         kyy = (
             Kb
             * n_rollers**0.9
             * l_rollers**0.8
             * fs**0.1
             * (np.cos(alpha)) ** 1.9
@@ -1897,16 +1893,14 @@
             "kyx_interpolated",
             "kzz_interpolated",
             "cxx_interpolated",
             "cyy_interpolated",
             "cxy_interpolated",
             "cyx_interpolated",
             "czz_interpolated",
-            "n_l",
-            "n_r",
             "dof_global_index",
         ]
         for p in params_to_remove:
             brg_data.pop(p)
 
         # change np.array to lists so that we can save in .toml as list(floats)
         params = [
```

### Comparing `ross-rotordynamics-1.3.0/ross/defects/abs_defect.py` & `ross-rotordynamics-1.4.0/ross/defects/abs_defect.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.3.0/ross/defects/crack.py` & `ross-rotordynamics-1.4.0/ross/defects/crack.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,14 @@
         n_crack,
         speed,
         unbalance_magnitude,
         unbalance_phase,
         crack_type="Mayes",
         print_progress=False,
     ):
-
         self.dt = dt
         self.tI = tI
         self.tF = tF
         self.depth_ratio = depth_ratio
         self.n_crack = n_crack
         self.speed = speed
         self.speedI = speed
```

### Comparing `ross-rotordynamics-1.3.0/ross/defects/integrate_solver.py` & `ross-rotordynamics-1.4.0/ross/defects/integrate_solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
     .. [1] BUTCHER, John Charles; GOODWIN, Nicolette. Numerical methods for ordinary differential equations. New York: Wiley, 2008. ..
     .. [2] CASH, Jeff R.; KARP, Alan H. A variable order Runge-Kutta method for initial value problems with rapidly varying right-hand sides.
            ACM Transactions on Mathematical Software (TOMS), v. 16, n. 3, p. 201-222, 1990. ..
 
     """
 
     def __init__(self, x0, y0, x, h, func, print_progress=False):
-
         self.x0 = x0
         self.y0 = y0
         self.x = x
         self.h = h
         self.func = func
         self.print_progress = print_progress
```

### Comparing `ross-rotordynamics-1.3.0/ross/defects/misalignment.py` & `ross-rotordynamics-1.4.0/ross/defects/misalignment.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.3.0/ross/defects/rubbing.py` & `ross-rotordynamics-1.4.0/ross/defects/rubbing.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,14 @@
         posRUB,
         speed,
         unbalance_magnitude,
         unbalance_phase,
         torque=False,
         print_progress=False,
     ):
-
         self.dt = dt
         self.tI = tI
         self.tF = tF
         self.deltaRUB = deltaRUB
         self.kRUB = kRUB
         self.cRUB = cRUB
         self.miRUB = miRUB
```

### Comparing `ross-rotordynamics-1.3.0/ross/disk_element.py` & `ross-rotordynamics-1.4.0/ross/disk_element.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.3.0/ross/element.py` & `ross-rotordynamics-1.4.0/ross/element.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.3.0/ross/fluid_flow/cylindrical.py` & `ross-rotordynamics-1.4.0/ross/fluid_flow/cylindrical.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import time
 
 import numpy as np
 from numpy.linalg import pinv
-from scipy.optimize import curve_fit, minimize
-
 from ross.bearing_seal_element import BearingElement
 from ross.units import Q_, check_units
+from scipy.optimize import curve_fit, minimize
 
 
 class THDCylindrical(BearingElement):
     """This class calculates the pressure and temperature field in oil film of
     a cylindrical bearing. It is also possible to obtain the stiffness and
     damping coefficients.
     The basic references for the code is found in :cite:t:`barbosa2018`, :cite:t:`daniel2012` and :cite:t:`nicoletti1999`.
@@ -50,30 +49,37 @@
     Describes the operation conditions of the bearing.
     speed : float, pint.Quantity
         Rotor rotational speed. Default unit is rad/s.
     load_x_direction : Float
         Load in X direction. The unit is newton.
     load_y_direction : Float
         Load in Y direction. The unit is newton.
+    operating_type : string
+        Choose the operating condition that bearing is operating.
+        - 'flooded'
+        - 'starvation'
 
     Fluid propierties
     ^^^^^^^^^^^^^^^^^
     Describes the fluid characteristics.
 
     lubricant : str
         Lubricant type. Can be:
         - 'ISOVG46'
     reference_temperature : float
         Oil reference temperature. The unit is celsius.
-    reference_viscosity : float
-        Oil viscosity at reference temperature. Unit is Pa.s.
     groove_factor : list, numpy array, tuple or float
         Ratio of oil in reservoir temperature that mixes with the circulating oil.
         Is required one factor per segment.
-
+    oil_flow: float
+        Suply oil flow to bearing. Only used when operating type 'starvation' is
+        selected. Unit is Litre per minute (l/min)
+    injection_pressure: float
+        Suply oil pressure that bearing receives at groove regions. Only used
+        when operating type 'starvation' is selected. Unit is Pascal (Pa).
 
     Turbulence Model
     ^^^^^^^^^^^^^^^^
     Turbulence model to improve analysis in higher speed.The model represents
     the turbulence by eddy diffusivities. The basic reference is found in :cite:t:`suganami1979`
 
     Reyn : Array
@@ -121,81 +127,79 @@
         Its shape is: array([excentricity, angle])
 
     Examples
     --------
     >>> from ross.fluid_flow.cylindrical import cylindrical_bearing_example
     >>> bearing = cylindrical_bearing_example()
     >>> bearing.equilibrium_pos
-    array([ 0.60678516, -0.73288691])
+    array([ 0.6873316 , -0.79393636])
     """
 
     @check_units
     def __init__(
         self,
         axial_length,
         journal_radius,
         radial_clearance,
         elements_circumferential,
         elements_axial,
-        n_y,
         n_pad,
         pad_arc_length,
         reference_temperature,
-        reference_viscosity,
         speed,
         load_x_direction,
         load_y_direction,
         groove_factor,
         lubricant,
         node,
         sommerfeld_type=2,
         initial_guess=[0.1, -0.1],
         method="perturbation",
+        operating_type="flooded",
+        injection_pressure=None,
+        oil_flow=None,
         show_coef=False,
         print_result=False,
         print_progress=False,
         print_time=False,
     ):
-
         self.axial_length = axial_length
         self.journal_radius = journal_radius
         self.radial_clearance = radial_clearance
         self.elements_circumferential = elements_circumferential
         self.elements_axial = elements_axial
-        self.n_y = n_y
         self.n_pad = n_pad
         self.reference_temperature = reference_temperature
-        self.reference_viscosity = reference_viscosity
         self.load_x_direction = load_x_direction
         self.load_y_direction = load_y_direction
         self.lubricant = lubricant
         self.fat_mixt = np.array(groove_factor)
         self.equilibrium_pos = None
         self.sommerfeld_type = sommerfeld_type
         self.initial_guess = initial_guess
         self.method = method
+        self.operating_type = operating_type
+        self.injection_pressure = injection_pressure
+        self.oil_flow = oil_flow
         self.show_coef = show_coef
         self.print_result = print_result
         self.print_progress = print_progress
         self.print_time = print_time
 
-        if self.n_y == None:
-            self.n_y = self.elements_circumferential
-
         self.betha_s_dg = pad_arc_length
         self.betha_s = pad_arc_length * np.pi / 180
 
         self.thetaI = 0
         self.thetaF = self.betha_s
         self.dtheta = (self.thetaF - self.thetaI) / (self.elements_circumferential)
 
         ##
         # Dimensionless discretization variables
 
-        self.dY = 1 / self.n_y
+        self.dY = 1 / self.elements_circumferential
         self.dZ = 1 / self.elements_axial
 
         # Z-axis direction
 
         self.Z_I = 0
         self.Z_F = 1
         Z = np.zeros((self.elements_axial + 2))
@@ -210,14 +214,16 @@
         # Dimensionalization
 
         self.dz = self.dZ * self.axial_length
         self.dy = self.dY * self.betha_s * self.journal_radius
 
         self.Zdim = self.Z * self.axial_length
 
+        self.oil_flow = self.oil_flow / 60000
+
         self.lubricant_dict = {
             "ISOVG32": {
                 "viscosity1": Q_(4.05640e-06, "reyn").to_base_units().m,
                 "temp1": Q_(40.00000, "degC").to_base_units().m,
                 "viscosity2": Q_(6.76911e-07, "reyn").to_base_units().m,
                 "temp2": Q_(100.00000, "degC").to_base_units().m,
                 "lube_density": Q_(873.99629, "kg/m³").to_base_units().m,
@@ -230,21 +236,21 @@
                 "viscosity2": Q_(8.810775697672788e-07, "reyn").to_base_units().m,
                 "temp2": Q_(100, "degC").to_base_units().m,
                 "lube_density": Q_(862.9, "kg/m³").to_base_units().m,
                 "lube_cp": Q_(1950, "J/(kg*degK)").to_base_units().m,
                 "lube_conduct": Q_(0.15, "W/(m*degC)").to_base_units().m,
             },
             "TEST": {
-                "viscosity1": Q_(2.758e-6, "reyn").to_base_units().m,
-                "temp1": Q_(121.7, "degF").to_base_units().m,
-                "viscosity2": Q_(1.119e-6, "reyn").to_base_units().m,
-                "temp2": Q_(175.7, "degF").to_base_units().m,
-                "lube_density": Q_(8.0e-5, "lbf*s²/in⁴").to_base_units().m,
-                "lube_cp": Q_(1.79959e2, "BTU*in/(lbf*s²*degF)").to_base_units().m,
-                "lube_conduct": Q_(2.00621e-6, "BTU/(in*s*degF)").to_base_units().m,
+                "viscosity1": Q_(0.04, "Pa*s").to_base_units().m,
+                "temp1": Q_(40, "degC").to_base_units().m,
+                "viscosity2": Q_(0.01, "Pa*s").to_base_units().m,
+                "temp2": Q_(100, "degC").to_base_units().m,
+                "lube_density": Q_(863.61302696, "kg/m³").to_base_units().m,
+                "lube_cp": Q_(1951.88616, "J/(kg*degK)").to_base_units().m,
+                "lube_conduct": Q_(0.15, "W/(m*degC)").to_base_units().m,
             },
         }
 
         lubricant_properties = self.lubricant_dict[self.lubricant]
         T_muI = Q_(lubricant_properties["temp1"], "degK").m_as("degC")
         T_muF = Q_(lubricant_properties["temp2"], "degK").m_as("degC")
         mu_I = lubricant_properties["viscosity1"]
@@ -252,28 +258,29 @@
         self.rho = lubricant_properties["lube_density"]
         self.Cp = lubricant_properties["lube_cp"]
         self.k_t = lubricant_properties["lube_conduct"]
 
         # Interpolation coefficients
         self.a, self.b = self._interpol(T_muI, T_muF, mu_I, mu_F)
 
+        self.reference_viscosity = self.a * (self.reference_temperature**self.b)
+
         number_of_freq = np.shape(speed)[0]
 
         kxx = np.zeros(number_of_freq)
         kxy = np.zeros(number_of_freq)
         kyx = np.zeros(number_of_freq)
         kyy = np.zeros(number_of_freq)
 
         cxx = np.zeros(number_of_freq)
         cxy = np.zeros(number_of_freq)
         cyx = np.zeros(number_of_freq)
         cyy = np.zeros(number_of_freq)
 
         for ii in range(number_of_freq):
-
             self.speed = speed[ii]
 
             self.run()
 
             coefs = self.coefficients()
             stiff = True
             for coef in coefs:
@@ -288,14 +295,668 @@
                     cxx[ii] = coef[0]
                     cxy[ii] = coef[1]
                     cyx[ii] = coef[2]
                     cyy[ii] = coef[3]
 
         super().__init__(node, kxx, cxx, kyy, kxy, kyx, cyy, cxy, cyx, speed)
 
+    def _flooded(self, n_p, Mat_coef, b_P, mu):
+        """Provides an analysis in which the bearing always receive sufficient oil feed to operate.
+
+        Parameters
+        ----------
+        n_p : integer,
+           current pad in analysis.
+        Mat_coef : np.array
+            Coeficient matrix.
+        b_P: np.array
+            Coefficients to pressure independent terms.
+        mu : np.array
+            Viscosity matrix.
+
+        Returns
+        -------
+        self.P : np.array
+            Pressure distribution in current pad vector.
+        """
+
+        ki = 0
+        kj = 0
+        k = 0
+        for ii in np.arange((self.Z_I + 0.5 * self.dZ), self.Z_F, self.dZ):
+            for jj in np.arange(
+                self.thetaI[n_p] + (self.dtheta / 2),
+                self.thetaF[n_p],
+                self.dtheta,
+            ):
+                hP = 1 - self.X * np.cos(jj) - self.Y * np.sin(jj)
+                he = (
+                    1
+                    - self.X * np.cos(jj + 0.5 * self.dtheta)
+                    - self.Y * np.sin(jj + 0.5 * self.dtheta)
+                )
+                hw = (
+                    1
+                    - self.X * np.cos(jj - 0.5 * self.dtheta)
+                    - self.Y * np.sin(jj - 0.5 * self.dtheta)
+                )
+                hn = hP
+                hs = hn
+
+                if kj == 0 and ki == 0:
+                    MU_e = 0.5 * (mu[ki, kj] + mu[ki, kj + 1])
+                    MU_w = mu[ki, kj]
+                    MU_s = mu[ki, kj]
+                    MU_n = 0.5 * (mu[ki, kj] + mu[ki + 1, kj])
+
+                if kj == 0 and ki > 0 and ki < self.elements_axial - 1:
+                    MU_e = 0.5 * (mu[ki, kj] + mu[ki, kj + 1])
+                    MU_w = mu[ki, kj]
+                    MU_s = 0.5 * (mu[ki, kj] + mu[ki - 1, kj])
+                    MU_n = 0.5 * (mu[ki, kj] + mu[ki + 1, kj])
+
+                if kj == 0 and ki == self.elements_axial - 1:
+                    MU_e = 0.5 * (mu[ki, kj] + mu[ki, kj + 1])
+                    MU_w = mu[ki, kj]
+                    MU_s = 0.5 * (mu[ki, kj] + mu[ki - 1, kj])
+                    MU_n = mu[ki, kj]
+
+                if ki == 0 and kj > 0 and kj < self.elements_circumferential - 1:
+                    MU_e = 0.5 * (mu[ki, kj] + mu[ki, kj + 1])
+                    MU_w = 0.5 * (mu[ki, kj] + mu[ki, kj - 1])
+                    MU_s = mu[ki, kj]
+                    MU_n = 0.5 * (mu[ki, kj] + mu[ki + 1, kj])
+
+                if (
+                    kj > 0
+                    and kj < self.elements_circumferential - 1
+                    and ki > 0
+                    and ki < self.elements_axial - 1
+                ):
+                    MU_e = 0.5 * (mu[ki, kj] + mu[ki, kj + 1])
+                    MU_w = 0.5 * (mu[ki, kj] + mu[ki, kj - 1])
+                    MU_s = 0.5 * (mu[ki, kj] + mu[ki - 1, kj])
+                    MU_n = 0.5 * (mu[ki, kj] + mu[ki + 1, kj])
+
+                if (
+                    ki == self.elements_axial - 1
+                    and kj > 0
+                    and kj < self.elements_circumferential - 1
+                ):
+                    MU_e = 0.5 * (mu[ki, kj] + mu[ki, kj + 1])
+                    MU_w = 0.5 * (mu[ki, kj] + mu[ki, kj - 1])
+                    MU_s = 0.5 * (mu[ki, kj] + mu[ki - 1, kj])
+                    MU_n = mu[ki, kj]
+
+                if ki == 0 and kj == self.elements_circumferential - 1:
+                    MU_e = mu[ki, kj]
+                    MU_w = 0.5 * (mu[ki, kj] + mu[ki, kj - 1])
+                    MU_s = mu[ki, kj]
+                    MU_n = 0.5 * (mu[ki, kj] + mu[ki + 1, kj])
+
+                if (
+                    kj == self.elements_circumferential - 1
+                    and ki > 0
+                    and ki < self.elements_axial - 1
+                ):
+                    MU_e = mu[ki, kj]
+                    MU_w = 0.5 * (mu[ki, kj] + mu[ki, kj - 1])
+                    MU_s = 0.5 * (mu[ki, kj] + mu[ki - 1, kj])
+                    MU_n = 0.5 * (mu[ki, kj] + mu[ki + 1, kj])
+
+                if (
+                    kj == self.elements_circumferential - 1
+                    and ki == self.elements_axial - 1
+                ):
+                    MU_e = mu[ki, kj]
+                    MU_w = 0.5 * (mu[ki, kj] + mu[ki, kj - 1])
+                    MU_s = 0.5 * (mu[ki, kj] + mu[ki - 1, kj])
+                    MU_n = mu[ki, kj]
+
+                CE = (self.dZ * he**3) / (
+                    12 * MU_e[n_p] * self.dY * self.betha_s**2
+                )
+                CW = (self.dZ * hw**3) / (
+                    12 * MU_w[n_p] * self.dY * self.betha_s**2
+                )
+                CN = (self.dY * (self.journal_radius**2) * hn**3) / (
+                    12 * MU_n[n_p] * self.dZ * self.axial_length**2
+                )
+                CS = (self.dY * (self.journal_radius**2) * hs**3) / (
+                    12 * MU_s[n_p] * self.dZ * self.axial_length**2
+                )
+                CP = -(CE + CW + CN + CS)
+
+                B = (self.dZ / (2 * self.betha_s)) * (he - hw) - (
+                    (self.Xpt * np.cos(jj) + self.Ypt * np.sin(jj)) * self.dy * self.dZ
+                )
+
+                k = k + 1
+                b_P[k - 1, 0] = B
+
+                if ki == 0 and kj == 0:
+                    Mat_coef[k - 1, k - 1] = CP - CS - CW
+                    Mat_coef[k - 1, k] = CE
+                    Mat_coef[k - 1, k + self.elements_circumferential - 1] = CN
+
+                elif kj == 0 and ki > 0 and ki < self.elements_axial - 1:
+                    Mat_coef[k - 1, k - 1] = CP - CW
+                    Mat_coef[k - 1, k] = CE
+                    Mat_coef[k - 1, k - self.elements_circumferential - 1] = CS
+                    Mat_coef[k - 1, k + self.elements_circumferential - 1] = CN
+
+                elif kj == 0 and ki == self.elements_axial - 1:
+                    Mat_coef[k - 1, k - 1] = CP - CN - CW
+                    Mat_coef[k - 1, k] = CE
+                    Mat_coef[k - 1, k - self.elements_circumferential - 1] = CS
+
+                elif ki == 0 and kj > 0 and kj < self.elements_circumferential - 1:
+                    Mat_coef[k - 1, k - 1] = CP - CS
+                    Mat_coef[k - 1, k] = CE
+                    Mat_coef[k - 1, k - 2] = CW
+                    Mat_coef[k - 1, k + self.elements_circumferential - 1] = CN
+
+                elif (
+                    ki > 0
+                    and ki < self.elements_axial - 1
+                    and kj > 0
+                    and kj < self.elements_circumferential - 1
+                ):
+                    Mat_coef[k - 1, k - 1] = CP
+                    Mat_coef[k - 1, k - 2] = CW
+                    Mat_coef[k - 1, k - self.elements_circumferential - 1] = CS
+                    Mat_coef[k - 1, k + self.elements_circumferential - 1] = CN
+                    Mat_coef[k - 1, k] = CE
+
+                elif (
+                    ki == self.elements_axial - 1
+                    and kj > 0
+                    and kj < self.elements_circumferential - 1
+                ):
+                    Mat_coef[k - 1, k - 1] = CP - CN
+                    Mat_coef[k - 1, k] = CE
+                    Mat_coef[k - 1, k - 2] = CW
+                    Mat_coef[k - 1, k - self.elements_circumferential - 1] = CS
+
+                elif ki == 0 and kj == self.elements_circumferential - 1:
+                    Mat_coef[k - 1, k - 1] = CP - CE - CS
+                    Mat_coef[k - 1, k - 2] = CW
+                    Mat_coef[k - 1, k + self.elements_circumferential - 1] = CN
+
+                elif (
+                    kj == self.elements_circumferential - 1
+                    and ki > 0
+                    and ki < self.elements_axial - 1
+                ):
+                    Mat_coef[k - 1, k - 1] = CP - CE
+                    Mat_coef[k - 1, k - 2] = CW
+                    Mat_coef[k - 1, k - self.elements_circumferential - 1] = CS
+                    Mat_coef[k - 1, k + self.elements_circumferential - 1] = CN
+
+                elif (
+                    ki == self.elements_axial - 1
+                    and kj == self.elements_circumferential - 1
+                ):
+                    Mat_coef[k - 1, k - 1] = CP - CE - CN
+                    Mat_coef[k - 1, k - 2] = CW
+                    Mat_coef[k - 1, k - self.elements_circumferential - 1] = CS
+
+                kj = kj + 1
+
+            kj = 0
+            ki = ki + 1
+
+        # Solution of pressure field end
+
+        p = np.linalg.solve(Mat_coef, b_P)
+        cont = 0
+
+        for i in np.arange(self.elements_axial):
+            for j in np.arange(self.elements_circumferential):
+                self.P[i, j, n_p] = p[cont]
+                cont = cont + 1
+
+                if self.P[i, j, n_p] < 0:
+                    self.P[i, j, n_p] = 0
+
+        # Dimensional pressure fied
+
+        self.Pdim = (
+            self.P * self.reference_viscosity * self.speed * (self.journal_radius**2)
+        ) / (self.radial_clearance**2)
+
+        return self.P
+
+    def _starvation(self, n_p, Mat_coef_st, mu, p_old, p, B, B_theta, nk):
+        """Provides an analysis in which the bearing may receive insufficient oil feed.
+
+        Parameters
+        ----------
+        n_p : integer,
+           current pad in analysis.
+        Mat_coef_st : np.array
+            Coeficient matrix.
+        mu : np.array
+            Viscosity matrix.
+        p_old : np.array
+            Past pressure matrix.
+        p : np.array
+            Current pressure matrix.
+        B: np.array
+            Coefficients to independent terms.
+        B: np.array
+            Coefficients to volumetric fraction independent terms.
+        nk: integer
+            counter.
+
+
+        Returns
+        -------
+        self.P : np.array
+            Pressure distribution in current pad vector.
+        """
+
+        while self.erro >= 0.01:
+            p_old = np.array(p)
+
+            theta_vol_old = np.array(self.theta_vol)
+
+            # cont = cont+1
+
+            k = 0
+            ki = 0
+            kj = 0
+
+            for ii in np.arange((self.Z_I + 0.5 * self.dZ), self.Z_F, self.dZ):
+                for jj in np.arange(
+                    self.thetaI[n_p] + (self.dtheta / 2),
+                    self.thetaF[n_p],
+                    self.dtheta,
+                ):
+                    hP = 1 - self.X * np.cos(jj) - self.Y * np.sin(jj)
+                    he = (
+                        1
+                        - self.X * np.cos(jj + 0.5 * self.dtheta)
+                        - self.Y * np.sin(jj + 0.5 * self.dtheta)
+                    )
+                    hw = (
+                        1
+                        - self.X * np.cos(jj - 0.5 * self.dtheta)
+                        - self.Y * np.sin(jj - 0.5 * self.dtheta)
+                    )
+                    hn = hP
+                    hs = hn
+
+                    hpt = -self.Xpt * np.cos(jj) - self.Ypt * np.sin(jj)
+
+                    if kj == 0 and ki == 0:
+                        MU_e = 0.5 * (mu[ki, kj] + mu[ki, kj + 1])
+                        MU_w = mu[ki, kj]
+                        MU_s = mu[ki, kj]
+                        MU_n = 0.5 * (mu[ki, kj] + mu[ki + 1, kj])
+
+                    if kj == 0 and ki > 0 and ki < self.elements_axial - 1:
+                        MU_e = 0.5 * (mu[ki, kj] + mu[ki, kj + 1])
+                        MU_w = mu[ki, kj]
+                        MU_s = 0.5 * (mu[ki, kj] + mu[ki - 1, kj])
+                        MU_n = 0.5 * (mu[ki, kj] + mu[ki + 1, kj])
+
+                    if kj == 0 and ki == self.elements_axial - 1:
+                        MU_e = 0.5 * (mu[ki, kj] + mu[ki, kj + 1])
+                        MU_w = mu[ki, kj]
+                        MU_s = 0.5 * (mu[ki, kj] + mu[ki - 1, kj])
+                        MU_n = mu[ki, kj]
+
+                    if ki == 0 and kj > 0 and kj < self.elements_circumferential - 1:
+                        MU_e = 0.5 * (mu[ki, kj] + mu[ki, kj + 1])
+                        MU_w = 0.5 * (mu[ki, kj] + mu[ki, kj - 1])
+                        MU_s = mu[ki, kj]
+                        MU_n = 0.5 * (mu[ki, kj] + mu[ki + 1, kj])
+
+                    if (
+                        kj > 0
+                        and kj < self.elements_circumferential - 1
+                        and ki > 0
+                        and ki < self.elements_axial - 1
+                    ):
+                        MU_e = 0.5 * (mu[ki, kj] + mu[ki, kj + 1])
+                        MU_w = 0.5 * (mu[ki, kj] + mu[ki, kj - 1])
+                        MU_s = 0.5 * (mu[ki, kj] + mu[ki - 1, kj])
+                        MU_n = 0.5 * (mu[ki, kj] + mu[ki + 1, kj])
+
+                    if (
+                        ki == self.elements_axial - 1
+                        and kj > 0
+                        and kj < self.elements_circumferential - 1
+                    ):
+                        MU_e = 0.5 * (mu[ki, kj] + mu[ki, kj + 1])
+                        MU_w = 0.5 * (mu[ki, kj] + mu[ki, kj - 1])
+                        MU_s = 0.5 * (mu[ki, kj] + mu[ki - 1, kj])
+                        MU_n = mu[ki, kj]
+
+                    if ki == 0 and kj == self.elements_circumferential - 1:
+                        MU_e = mu[ki, kj]
+                        MU_w = 0.5 * (mu[ki, kj] + mu[ki, kj - 1])
+                        MU_s = mu[ki, kj]
+                        MU_n = 0.5 * (mu[ki, kj] + mu[ki + 1, kj])
+
+                    if (
+                        kj == self.elements_circumferential - 1
+                        and ki > 0
+                        and ki < self.elements_axial - 1
+                    ):
+                        MU_e = mu[ki, kj]
+                        MU_w = 0.5 * (mu[ki, kj] + mu[ki, kj - 1])
+                        MU_s = 0.5 * (mu[ki, kj] + mu[ki - 1, kj])
+                        MU_n = 0.5 * (mu[ki, kj] + mu[ki + 1, kj])
+
+                    if (
+                        kj == self.elements_circumferential - 1
+                        and ki == self.elements_axial - 1
+                    ):
+                        MU_e = mu[ki, kj]
+                        MU_w = 0.5 * (mu[ki, kj] + mu[ki, kj - 1])
+                        MU_s = 0.5 * (mu[ki, kj] + mu[ki - 1, kj])
+                        MU_n = mu[ki, kj]
+
+                    CE = (self.dZ * he**3) / (
+                        12 * MU_e[n_p] * self.dY * self.betha_s**2
+                    )
+                    CW = (self.dZ * hw**3) / (
+                        12 * MU_w[n_p] * self.dY * self.betha_s**2
+                    )
+                    CN = (self.dY * (self.journal_radius**2) * hn**3) / (
+                        12 * MU_n[n_p] * self.dZ * self.axial_length**2
+                    )
+                    CS = (self.dY * (self.journal_radius**2) * hs**3) / (
+                        12 * MU_s[n_p] * self.dZ * self.axial_length**2
+                    )
+                    CP = -(CE + CW + CN + CS)
+
+                    # Termo Fonte
+                    KP1 = -(self.dZ / (2 * self.betha_s)) * he
+
+                    KP2 = -hpt * self.dY * self.dZ
+
+                    KP = KP1 + KP2
+
+                    KW = (self.dZ / (2 * self.betha_s)) * hw
+
+                    if (
+                        kj > 0
+                        and kj < self.elements_circumferential - 1
+                        and ki > 0
+                        and ki < self.elements_axial - 1
+                    ):  # Center region
+                        Mat_coef_st[k, k] = CP
+                        Mat_coef_st[k, k + 1] = CE
+                        Mat_coef_st[k, k - 1] = CW
+                        Mat_coef_st[k, k + self.elements_circumferential] = CN
+                        Mat_coef_st[k, k - self.elements_circumferential] = CS
+
+                        if p[k] > 0:
+                            self.theta_vol[k] = 1
+                            B[k] = -KP * self.theta_vol[k] - KW * self.theta_vol[k - 1]
+                            pp = np.zeros((nk - 1, 1))
+                            pp = np.delete(p, k)
+                            C = np.zeros((1, nk))
+                            C = Mat_coef_st[k, :]
+                            C = np.delete(C, k)
+                            p[k] = (B[k] - np.matmul(C, pp)) / Mat_coef_st[k, k]
+
+                        else:
+                            p[k] = 0
+                            B_theta[k] = -np.matmul(Mat_coef_st[k, :], p)
+                            self.theta_vol[k] = (
+                                B_theta[k] - KW * self.theta_vol[k - 1]
+                            ) / KP
+
+                    elif (
+                        kj > 0 and kj < self.elements_circumferential - 1 and ki == 0
+                    ):  # Inferior edge without corners
+                        Mat_coef_st[k, k] = CP - CS
+                        Mat_coef_st[k, k + 1] = CE
+                        Mat_coef_st[k, k - 1] = CW
+                        Mat_coef_st[k, k + self.elements_circumferential] = CN
+
+                        if p[k] > 0:
+                            self.theta_vol[k] = 1
+                            B[k] = -KP * self.theta_vol[k] - KW * self.theta_vol[k - 1]
+                            pp = np.zeros((nk - 1, 1))
+                            pp = np.delete(p, k)
+                            C = np.zeros((1, nk))
+                            C = Mat_coef_st[k, :]
+                            C = np.delete(C, k)
+                            p[k] = (B[k] - np.matmul(C, pp)) / Mat_coef_st[k, k]
+
+                        else:
+                            p[k] = 0
+                            B_theta[k] = -np.matmul(Mat_coef_st[k, :], p)
+                            self.theta_vol[k] = (
+                                B_theta[k] - KW * self.theta_vol[k - 1]
+                            ) / KP
+
+                    elif (
+                        kj > 0
+                        and kj < self.elements_circumferential - 1
+                        and ki == self.elements_axial - 1
+                    ):  # Superior edge without corners
+                        Mat_coef_st[k, k] = CP - CN
+                        Mat_coef_st[k, k + 1] = CE
+                        Mat_coef_st[k, k - 1] = CW
+                        Mat_coef_st[k, k - self.elements_circumferential] = CS
+
+                        if p[k] > 0:
+                            self.theta_vol[k] = 1
+                            B[k] = -KP * self.theta_vol[k] - KW * self.theta_vol[k - 1]
+                            pp = np.zeros((nk - 1, 1))
+                            pp = np.delete(p, k)
+                            C = np.zeros((1, nk))
+                            C = Mat_coef_st[k, :]
+                            C = np.delete(C, k)
+                            p[k] = (B[k] - np.matmul(C, pp)) / Mat_coef_st[k, k]
+
+                        else:
+                            p[k] = 0
+                            B_theta[k] = -np.matmul(Mat_coef_st[k, :], p)
+                            self.theta_vol[k] = (
+                                B_theta[k] - KW * self.theta_vol[k - 1]
+                            ) / KP
+
+                    elif (
+                        kj == 0 and ki > 0 and ki < self.elements_axial - 1
+                    ):  # Left edge without corners
+                        Mat_coef_st[k, k] = CP - CW
+                        Mat_coef_st[k, k + 1] = CE
+                        Mat_coef_st[k, k - self.elements_circumferential] = CS
+                        Mat_coef_st[k, k + self.elements_circumferential] = CN
+
+                        if p[k] > 0:
+                            self.theta_vol[k] = 1
+                            B[k] = (
+                                -KP * self.theta_vol[k]
+                                - self.theta_vol_groove[n_p] * KW
+                                - 2 * CW * self.injection_pressure
+                            )
+                            pp = np.zeros((nk - 1, 1))
+                            pp = np.delete(p, k)
+                            C = np.zeros((1, nk))
+                            C = Mat_coef_st[k, :]
+                            C = np.delete(C, k)
+                            p[k] = (B[k] - np.matmul(C, pp)) / Mat_coef_st[k, k]
+
+                        else:
+                            p[k] = 0
+                            B_theta[k] = -np.matmul(Mat_coef_st[k, :], p)
+                            self.theta_vol[k] = (
+                                B_theta[k] - self.theta_vol_groove[n_p] * KW * 1
+                            ) / KP
+
+                    elif (
+                        kj == self.elements_circumferential - 1
+                        and ki > 0
+                        and ki < self.elements_axial - 1
+                    ):  # Right edge without corners
+                        Mat_coef_st[k, k] = CP - CE
+
+                        Mat_coef_st[k, k - 1] = CW
+                        Mat_coef_st[k, k + self.elements_circumferential] = CN
+                        Mat_coef_st[k, k - self.elements_circumferential] = CS
+
+                        if p[k] > 0:
+                            self.theta_vol[k] = 1
+                            B[k] = -KP * self.theta_vol[k] - KW * self.theta_vol[k - 1]
+                            pp = np.zeros((nk - 1, 1))
+                            pp = np.delete(p, k)
+                            C = np.zeros((1, nk))
+                            C = Mat_coef_st[k, :]
+                            C = np.delete(C, k)
+                            p[k] = (B[k] - np.matmul(C, pp)) / Mat_coef_st[k, k]
+
+                        else:
+                            p[k] = 0
+                            B_theta[k] = -np.matmul(Mat_coef_st[k, :], p)
+                            self.theta_vol[k] = (
+                                B_theta[k] - KW * self.theta_vol[k - 1]
+                            ) / KP
+
+                    elif kj == 0 and ki == 0:  # Corner inferior left
+                        Mat_coef_st[k, k] = CP - CS - CW
+                        Mat_coef_st[k, k + 1] = CE
+                        Mat_coef_st[k, k + self.elements_circumferential] = CN
+
+                        if p[k] > 0:
+                            self.theta_vol[k] = 1
+                            B[k] = (
+                                -KP * self.theta_vol[k]
+                                - self.theta_vol_groove[n_p] * KW
+                                - 2 * CW * self.injection_pressure
+                            )
+                            pp = np.zeros((nk - 1, 1))
+                            pp = np.delete(p, k)
+                            C = np.zeros((1, nk))
+                            C = Mat_coef_st[k, :]
+                            C = np.delete(C, k)
+                            p[k] = (B[k] - np.matmul(C, pp)) / Mat_coef_st[k, k]
+
+                        else:
+                            p[k] = 0
+                            B_theta[k] = -np.matmul(Mat_coef_st[k, :], p)
+                            self.theta_vol[k] = (
+                                B_theta[k] - self.theta_vol_groove[n_p] * KW * 1
+                            ) / KP
+
+                    elif (
+                        kj == self.elements_circumferential - 1 and ki == 0
+                    ):  # Corner inferior right
+                        Mat_coef_st[k, k] = CP - CS - CE
+                        Mat_coef_st[k, k - 1] = CW
+                        Mat_coef_st[k, k + self.elements_circumferential] = CN
+
+                        if p[k] > 0:
+                            self.theta_vol[k] = 1
+                            B[k] = -KP * self.theta_vol[k] - KW * self.theta_vol[k - 1]
+                            pp = np.zeros((nk - 1, 1))
+                            pp = np.delete(p, k)
+                            C = np.zeros((1, nk))
+                            C = Mat_coef_st[k, :]
+                            C = np.delete(C, k)
+                            p[k] = (B[k] - np.matmul(C, pp)) / Mat_coef_st[k, k]
+
+                        else:
+                            p[k] = 0
+                            B_theta[k] = -np.matmul(Mat_coef_st[k, :], p)
+                            self.theta_vol[k] = (
+                                B_theta[k] - KW * self.theta_vol[k - 1]
+                            ) / KP
+
+                    elif (
+                        kj == 0 and ki == self.elements_axial - 1
+                    ):  # Corner superior left
+                        Mat_coef_st[k, k] = CP - CN - CW
+                        Mat_coef_st[k, k + 1] = CE
+                        Mat_coef_st[k, k - self.elements_circumferential] = CS
+
+                        if p[k] > 0:
+                            self.theta_vol[k] = 1
+                            B[k] = (
+                                -KP * self.theta_vol[k]
+                                - self.theta_vol_groove[n_p] * KW
+                                - 2 * CW * self.injection_pressure
+                            )
+                            pp = np.zeros((nk - 1, 1))
+                            pp = np.delete(p, k)
+                            C = np.zeros((1, nk))
+                            C = Mat_coef_st[k, :]
+                            C = np.delete(C, k)
+                            p[k] = (B[k] - np.matmul(C, pp)) / Mat_coef_st[k, k]
+
+                        else:
+                            p[k] = 0
+                            B_theta[k] = -np.matmul(Mat_coef_st[k, :], p)
+                            self.theta_vol[k] = (
+                                B_theta[k] - self.theta_vol_groove[n_p] * KW * 1
+                            ) / KP
+
+                    elif (
+                        kj == self.elements_circumferential - 1
+                        and ki == self.elements_axial - 1
+                    ):  # Corner superior right
+                        Mat_coef_st[k, k] = CP - CN - CE
+                        Mat_coef_st[k, k - 1] = CW
+                        Mat_coef_st[k, k - self.elements_circumferential] = CS
+
+                        if p[k] > 0:
+                            self.theta_vol[k] = 1
+                            B[k] = -KP * self.theta_vol[k] - KW * self.theta_vol[k - 1]
+                            pp = np.zeros((nk - 1, 1))
+                            pp = np.delete(p, k)
+                            C = np.zeros((1, nk))
+                            C = Mat_coef_st[k, :]
+                            C = np.delete(C, k)
+                            p[k] = (B[k] - np.matmul(C, pp)) / Mat_coef_st[k, k]
+
+                        else:
+                            p[k] = 0
+                            B_theta[k] = -np.matmul(Mat_coef_st[k, :], p)
+                            self.theta_vol[k] = (
+                                B_theta[k] - KW * self.theta_vol[k - 1]
+                            ) / KP
+
+                    k = k + 1
+                    kj = kj + 1
+
+                kj = 0
+                ki = ki + 1
+
+            self.erro = np.linalg.norm(p - p_old) + np.linalg.norm(
+                self.theta_vol - theta_vol_old
+            )
+
+        cont = 0
+
+        for i in np.arange(self.elements_axial):
+            for j in np.arange(self.elements_circumferential):
+                self.P[i, j, n_p] = p[cont]
+
+                self.Theta_vol[i, j, n_p] = self.theta_vol[cont]
+
+                cont = cont + 1
+
+                if self.P[i, j, n_p] < 0:
+                    self.P[i, j, n_p] = 0
+
+        # Dimensional pressure fied
+
+        self.Pdim = (
+            self.P * self.reference_viscosity * self.speed * (self.journal_radius**2)
+        ) / (self.radial_clearance**2)
+
+        return self.P
+
     def _forces(self, initial_guess, y0, xpt0, ypt0):
         """Calculates the forces in Y and X direction.
 
         Parameters
         ----------
         initial_guess : array, float
             If the other parameters are None, initial_guess is an array with eccentricity
@@ -312,14 +973,15 @@
         Returns
         -------
         Fhx : float
             Force in X direction. The unit is newton.
         Fhy : float
             Force in Y direction. The unit is newton.
         """
+
         if y0 is None and xpt0 is None and ypt0 is None:
             self.initial_guess = initial_guess
 
             xr = (
                 self.initial_guess[0]
                 * self.radial_clearance
                 * np.cos(self.initial_guess[1])
@@ -356,35 +1018,28 @@
         )
 
         self.thetaF = np.radians(
             [pad + (180 / self.n_pad) + (self.betha_s_dg / 2) for pad in pad_ct]
         )
 
         Ytheta = [
-            np.linspace(t1, t2, self.elements_circumferential)
+            np.linspace(
+                t1 + self.dtheta / 2,
+                t2 - self.dtheta / 2,
+                self.elements_circumferential,
+            )
             for t1, t2 in zip(self.thetaI, self.thetaF)
         ]
 
-        self.pad_ct = [ang for ang in range(0, 360, int(360 / self.n_pad))]
+        self.theta_vol_groove = 0.8 * np.ones(self.n_pad)
 
-        self.thetaI = np.radians(
-            [pad + (180 / self.n_pad) - (self.betha_s_dg / 2) for pad in self.pad_ct]
-        )
-
-        self.thetaF = np.radians(
-            [pad + (180 / self.n_pad) + (self.betha_s_dg / 2) for pad in self.pad_ct]
-        )
-
-        Ytheta = [
-            np.linspace(t1, t2, self.elements_circumferential)
-            for t1, t2 in zip(self.thetaI, self.thetaF)
-        ]
-
-        while (T_mist[0] - T_conv) >= 1e-2:
+        T_end = np.ones(self.n_pad)
 
+        while (T_mist[0] - T_conv) >= 0.5:
+            nk = (self.elements_axial) * (self.elements_circumferential)
             self.P = np.zeros(
                 (self.elements_axial, self.elements_circumferential, self.n_pad)
             )
             dPdy = np.zeros(
                 (self.elements_axial, self.elements_circumferential, self.n_pad)
             )
             dPdz = np.zeros(
@@ -396,290 +1051,86 @@
             T_new = (
                 np.ones(
                     (self.elements_axial, self.elements_circumferential, self.n_pad)
                 )
                 * 1.2
             )
 
-            T_conv = T_mist[0]
+            self.Theta_vol = np.zeros(
+                (self.elements_axial, self.elements_circumferential, self.n_pad)
+            )
 
             mu_new = 1.1 * np.ones(
                 (self.elements_axial, self.elements_circumferential, self.n_pad)
             )
             mu_turb = 1.3 * np.ones(
                 (self.elements_axial, self.elements_circumferential, self.n_pad)
             )
 
-            PP = np.zeros(((self.elements_axial), (2 * self.elements_circumferential)))
+            T_conv = T_mist[0]
+
+            self.H = np.ones((self.elements_circumferential, self.n_pad))
+
+            U = 0.5 * np.ones(
+                (self.elements_axial, self.elements_circumferential, self.n_pad)
+            )
+
+            self.V = np.zeros(
+                (self.elements_axial, self.elements_circumferential, self.n_pad)
+            )
 
-            nk = (self.elements_axial) * (self.elements_circumferential)
+            self.Qedim = np.ones(self.n_pad)
+
+            self.Qsdim = np.ones(self.n_pad)
+
+            self.Qldim = np.ones(self.n_pad)
 
-            Mat_coef = np.zeros((nk, nk))
-            Mat_coef_T = np.zeros((nk, nk))
-            b = np.zeros((nk, 1))
             b_T = np.zeros((nk, 1))
 
-            for n_p in np.arange(self.n_pad):
+            b_P = np.zeros((nk, 1))
+
+            Mat_coef = np.zeros((nk, nk))  # Coeficients matrix
 
-                T_ref = T_mist[n_p - 1]
+            B = np.zeros((nk, 1))  # Termo fonte for pressure
 
-                # Temperature convergence while
+            for n_p in np.arange(self.n_pad):
+                T_ref = T_mist[n_p]
 
                 while (
                     np.linalg.norm(T_new[:, :, n_p] - T[:, :, n_p])
                     / np.linalg.norm(T[:, :, n_p])
-                    >= 1e-3
+                    >= 0.01
                 ):
-
-                    T_ref = T_mist[n_p - 1]
+                    T_ref = T_mist[n_p]
 
                     mu = mu_new
+
                     self.mu_l = mu_new
 
                     T[:, :, n_p] = T_new[:, :, n_p]
 
-                    ki = 0
-                    kj = 0
-                    k = 0
+                    self.erro = 1
 
-                    # Solution of pressure field initialization
+                    p_old = np.zeros((nk, 1))
 
-                    for ii in np.arange((self.Z_I + 0.5 * self.dZ), self.Z_F, self.dZ):
-                        for jj in np.arange(
-                            self.thetaI[n_p] + (self.dtheta / 2),
-                            self.thetaF[n_p],
-                            self.dtheta,
-                        ):
+                    self.theta_vol = np.zeros((nk, 1))  # Theta volumetric vector
 
-                            hP = 1 - self.X * np.cos(jj) - self.Y * np.sin(jj)
-                            he = (
-                                1
-                                - self.X * np.cos(jj + 0.5 * self.dtheta)
-                                - self.Y * np.sin(jj + 0.5 * self.dtheta)
-                            )
-                            hw = (
-                                1
-                                - self.X * np.cos(jj - 0.5 * self.dtheta)
-                                - self.Y * np.sin(jj - 0.5 * self.dtheta)
-                            )
-                            hn = hP
-                            hs = hn
+                    Mat_coef_st = np.zeros((nk, nk))  # Coeficients matrix
 
-                            if kj == 0 and ki == 0:
-                                MU_e = 0.5 * (mu[ki, kj] + mu[ki, kj + 1])
-                                MU_w = mu[ki, kj]
-                                MU_s = mu[ki, kj]
-                                MU_n = 0.5 * (mu[ki, kj] + mu[ki + 1, kj])
+                    Mat_coef_T = np.zeros((nk, nk))
 
-                            if kj == 0 and ki > 0 and ki < self.elements_axial - 1:
-                                MU_e = 0.5 * (mu[ki, kj] + mu[ki, kj + 1])
-                                MU_w = mu[ki, kj]
-                                MU_s = 0.5 * (mu[ki, kj] + mu[ki - 1, kj])
-                                MU_n = 0.5 * (mu[ki, kj] + mu[ki + 1, kj])
+                    p = np.ones((nk, 1))  # Pressure vector
 
-                            if kj == 0 and ki == self.elements_axial - 1:
-                                MU_e = 0.5 * (mu[ki, kj] + mu[ki, kj + 1])
-                                MU_w = mu[ki, kj]
-                                MU_s = 0.5 * (mu[ki, kj] + mu[ki - 1, kj])
-                                MU_n = mu[ki, kj]
+                    B_theta = np.zeros((nk, 1))
 
-                            if (
-                                ki == 0
-                                and kj > 0
-                                and kj < self.elements_circumferential - 1
-                            ):
-                                MU_e = 0.5 * (mu[ki, kj] + mu[ki, kj + 1])
-                                MU_w = 0.5 * (mu[ki, kj] + mu[ki, kj - 1])
-                                MU_s = mu[ki, kj]
-                                MU_n = 0.5 * (mu[ki, kj] + mu[ki + 1, kj])
+                    if self.operating_type == "flooded":
+                        self._flooded(n_p, Mat_coef, b_P, mu)
 
-                            if (
-                                kj > 0
-                                and kj < self.elements_circumferential - 1
-                                and ki > 0
-                                and ki < self.elements_axial - 1
-                            ):
-                                MU_e = 0.5 * (mu[ki, kj] + mu[ki, kj + 1])
-                                MU_w = 0.5 * (mu[ki, kj] + mu[ki, kj - 1])
-                                MU_s = 0.5 * (mu[ki, kj] + mu[ki - 1, kj])
-                                MU_n = 0.5 * (mu[ki, kj] + mu[ki + 1, kj])
-
-                            if (
-                                ki == self.elements_axial - 1
-                                and kj > 0
-                                and kj < self.elements_circumferential - 1
-                            ):
-                                MU_e = 0.5 * (mu[ki, kj] + mu[ki, kj + 1])
-                                MU_w = 0.5 * (mu[ki, kj] + mu[ki, kj - 1])
-                                MU_s = 0.5 * (mu[ki, kj] + mu[ki - 1, kj])
-                                MU_n = mu[ki, kj]
-
-                            if ki == 0 and kj == self.elements_circumferential - 1:
-                                MU_e = mu[ki, kj]
-                                MU_w = 0.5 * (mu[ki, kj] + mu[ki, kj - 1])
-                                MU_s = mu[ki, kj]
-                                MU_n = 0.5 * (mu[ki, kj] + mu[ki + 1, kj])
-
-                            if (
-                                kj == self.elements_circumferential - 1
-                                and ki > 0
-                                and ki < self.elements_axial - 1
-                            ):
-                                MU_e = mu[ki, kj]
-                                MU_w = 0.5 * (mu[ki, kj] + mu[ki, kj - 1])
-                                MU_s = 0.5 * (mu[ki, kj] + mu[ki - 1, kj])
-                                MU_n = 0.5 * (mu[ki, kj] + mu[ki + 1, kj])
-
-                            if (
-                                kj == self.elements_circumferential - 1
-                                and ki == self.elements_axial - 1
-                            ):
-                                MU_e = mu[ki, kj]
-                                MU_w = 0.5 * (mu[ki, kj] + mu[ki, kj - 1])
-                                MU_s = 0.5 * (mu[ki, kj] + mu[ki - 1, kj])
-                                MU_n = mu[ki, kj]
-
-                            CE = (self.dZ * he**3) / (
-                                12 * MU_e[n_p] * self.dY * self.betha_s**2
-                            )
-                            CW = (self.dZ * hw**3) / (
-                                12 * MU_w[n_p] * self.dY * self.betha_s**2
-                            )
-                            CN = (self.dY * (self.journal_radius**2) * hn**3) / (
-                                12 * MU_n[n_p] * self.dZ * self.axial_length**2
-                            )
-                            CS = (self.dY * (self.journal_radius**2) * hs**3) / (
-                                12 * MU_s[n_p] * self.dZ * self.axial_length**2
-                            )
-                            CP = -(CE + CW + CN + CS)
-
-                            B = (self.dZ / (2 * self.betha_s)) * (he - hw) - (
-                                (self.Ypt * np.cos(jj) + self.Xpt * np.sin(jj))
-                                * self.dy
-                                * self.dZ
-                            )
-
-                            k = k + 1
-                            b[k - 1, 0] = B
-
-                            if ki == 0 and kj == 0:
-                                Mat_coef[k - 1, k - 1] = CP - CS - CW
-                                Mat_coef[k - 1, k] = CE
-                                Mat_coef[
-                                    k - 1, k + self.elements_circumferential - 1
-                                ] = CN
-
-                            elif kj == 0 and ki > 0 and ki < self.elements_axial - 1:
-                                Mat_coef[k - 1, k - 1] = CP - CW
-                                Mat_coef[k - 1, k] = CE
-                                Mat_coef[
-                                    k - 1, k - self.elements_circumferential - 1
-                                ] = CS
-                                Mat_coef[
-                                    k - 1, k + self.elements_circumferential - 1
-                                ] = CN
-
-                            elif kj == 0 and ki == self.elements_axial - 1:
-                                Mat_coef[k - 1, k - 1] = CP - CN - CW
-                                Mat_coef[k - 1, k] = CE
-                                Mat_coef[
-                                    k - 1, k - self.elements_circumferential - 1
-                                ] = CS
-
-                            elif ki == 0 and kj > 0 and kj < self.n_y - 1:
-                                Mat_coef[k - 1, k - 1] = CP - CS
-                                Mat_coef[k - 1, k] = CE
-                                Mat_coef[k - 1, k - 2] = CW
-                                Mat_coef[
-                                    k - 1, k + self.elements_circumferential - 1
-                                ] = CN
-
-                            elif (
-                                ki > 0
-                                and ki < self.elements_axial - 1
-                                and kj > 0
-                                and kj < self.n_y - 1
-                            ):
-                                Mat_coef[k - 1, k - 1] = CP
-                                Mat_coef[k - 1, k - 2] = CW
-                                Mat_coef[
-                                    k - 1, k - self.elements_circumferential - 1
-                                ] = CS
-                                Mat_coef[
-                                    k - 1, k + self.elements_circumferential - 1
-                                ] = CN
-                                Mat_coef[k - 1, k] = CE
-
-                            elif (
-                                ki == self.elements_axial - 1
-                                and kj > 0
-                                and kj < self.n_y - 1
-                            ):
-                                Mat_coef[k - 1, k - 1] = CP - CN
-                                Mat_coef[k - 1, k] = CE
-                                Mat_coef[k - 1, k - 2] = CW
-                                Mat_coef[
-                                    k - 1, k - self.elements_circumferential - 1
-                                ] = CS
-
-                            elif ki == 0 and kj == self.n_y - 1:
-                                Mat_coef[k - 1, k - 1] = CP - CE - CS
-                                Mat_coef[k - 1, k - 2] = CW
-                                Mat_coef[
-                                    k - 1, k + self.elements_circumferential - 1
-                                ] = CN
-
-                            elif (
-                                kj == self.n_y - 1
-                                and ki > 0
-                                and ki < self.elements_axial - 1
-                            ):
-                                Mat_coef[k - 1, k - 1] = CP - CE
-                                Mat_coef[k - 1, k - 2] = CW
-                                Mat_coef[
-                                    k - 1, k - self.elements_circumferential - 1
-                                ] = CS
-                                Mat_coef[
-                                    k - 1, k + self.elements_circumferential - 1
-                                ] = CN
-
-                            elif ki == self.elements_axial - 1 and kj == self.n_y - 1:
-                                Mat_coef[k - 1, k - 1] = CP - CE - CN
-                                Mat_coef[k - 1, k - 2] = CW
-                                Mat_coef[
-                                    k - 1, k - self.elements_circumferential - 1
-                                ] = CS
-
-                            kj = kj + 1
-
-                        kj = 0
-                        ki = ki + 1
-
-                    # Solution of pressure field end
-
-                    p = np.linalg.solve(Mat_coef, b)
-                    cont = 0
-
-                    for i in np.arange(self.elements_axial):
-                        for j in np.arange(self.elements_circumferential):
-
-                            self.P[i, j, n_p] = p[cont]
-                            cont = cont + 1
-
-                            if self.P[i, j, n_p] < 0:
-                                self.P[i, j, n_p] = 0
-
-                    # Dimensional pressure fied
-
-                    self.Pdim = (
-                        self.P
-                        * self.reference_viscosity
-                        * self.speed
-                        * (self.journal_radius**2)
-                    ) / (self.radial_clearance**2)
+                    elif self.operating_type == "starvation":
+                        self._starvation(n_p, Mat_coef_st, mu, p_old, p, B, B_theta, nk)
 
                     ki = 0
                     kj = 0
                     k = 0
 
                     # Solution of temperature field initialization
 
@@ -687,15 +1138,14 @@
                         (self.Z_I + 0.5 * self.dZ), (self.Z_F), self.dZ
                     ):
                         for jj in np.arange(
                             self.thetaI[n_p] + (self.dtheta / 2),
                             self.thetaF[n_p],
                             self.dtheta,
                         ):
-
                             # Pressure gradients
 
                             if kj == 0 and ki == 0:
                                 dPdy[ki, kj, n_p] = (self.P[ki, kj + 1, n_p] - 0) / (
                                     2 * self.dY
                                 )
                                 dPdz[ki, kj, n_p] = (self.P[ki + 1, kj, n_p] - 0) / (
@@ -783,39 +1233,49 @@
                                     2 * self.dY
                                 )
                                 dPdz[ki, kj, n_p] = (0 - self.P[ki - 1, kj, n_p]) / (
                                     2 * self.dZ
                                 )
 
                             HP = 1 - self.X * np.cos(jj) - self.Y * np.sin(jj)
-                            hpt = -self.Ypt * np.cos(jj) + self.Xpt * np.sin(jj)
+                            hpt = -self.Xpt * np.cos(jj) - self.Ypt * np.sin(jj)
+                            self.H[kj, n_p] = HP
 
                             mu_p = mu[ki, kj, n_p]
 
-                            Reyn[ki, kj, n_p] = (
-                                self.rho
-                                * self.speed
-                                * self.journal_radius
-                                * (HP / self.axial_length)
-                                * self.radial_clearance
-                                / (self.reference_viscosity)
-                            )
+                            if self.operating_type == "starvation":
+                                Reyn[ki, kj, n_p] = (
+                                    self.Theta_vol[ki, kj, n_p]
+                                    * self.rho
+                                    * self.speed
+                                    * self.journal_radius
+                                    * (HP / self.axial_length)
+                                    * self.radial_clearance
+                                    / (self.reference_viscosity * mu_p)
+                                )
 
-                            if Reyn[ki, kj, n_p] <= 500:
+                            else:
+                                Reyn[ki, kj, n_p] = (
+                                    self.rho
+                                    * self.speed
+                                    * self.journal_radius
+                                    * (HP / self.axial_length)
+                                    * self.radial_clearance
+                                    / (self.reference_viscosity * mu_p)
+                                )
 
+                            if Reyn[ki, kj, n_p] <= 500:
                                 self.delta_turb = 0
 
-                            elif Reyn[ki, kj, n_p] > 400 and Reyn[ki, kj, n_p] <= 1000:
-
+                            elif Reyn[ki, kj, n_p] > 500 and Reyn[ki, kj, n_p] <= 1000:
                                 self.delta_turb = 1 - (
                                     (1000 - Reyn[ki, kj, n_p]) / 500
                                 ) ** (1 / 8)
 
                             elif Reyn[ki, kj, n_p] > 1000:
-
                                 self.delta_turb = 1
 
                             dudy = ((HP / mu_turb[ki, kj, n_p]) * dPdy[ki, kj, n_p]) - (
                                 self.speed / HP
                             )
 
                             dwdy = (HP / mu_turb[ki, kj, n_p]) * dPdz[ki, kj, n_p]
@@ -835,14 +1295,21 @@
 
                             emv = 0.4 * (x_wall - (10.7 * np.tanh(x_wall / 10.7)))
 
                             mu_turb[ki, kj, n_p] = mu_p * (1 + (self.delta_turb * emv))
 
                             mi_t = mu_turb[ki, kj, n_p]
 
+                            U[ki, kj, n_p] = (
+                                -(HP**2)
+                                / (12 * mi_t * self.betha_s)
+                                * dPdy[ki, kj, n_p]
+                                + 1 / 2
+                            )
+
                             AE = -(self.k_t * HP * self.dZ) / (
                                 self.rho
                                 * self.Cp
                                 * self.speed
                                 * ((self.betha_s * self.journal_radius) ** 2)
                                 * self.dY
                             )
@@ -1011,72 +1478,79 @@
                                 Mat_coef_T[
                                     k - 1, k - self.elements_circumferential - 1
                                 ] = AS
                                 b_T[k - 1, 0] = b_T[k - 1, 0] - 2 * AW * (
                                     T_ref / self.reference_temperature
                                 )
 
-                            elif ki == 0 and kj > 0 and kj < self.n_y - 1:
+                            elif (
+                                ki == 0
+                                and kj > 0
+                                and kj < self.elements_circumferential - 1
+                            ):
                                 Mat_coef_T[k - 1, k - 1] = AP + AS
                                 Mat_coef_T[k - 1, k] = AE
                                 Mat_coef_T[k - 1, k - 2] = AW
                                 Mat_coef_T[
                                     k - 1, k + self.elements_circumferential - 1
                                 ] = AN
 
                             elif (
                                 ki > 0
                                 and ki < self.elements_axial - 1
                                 and kj > 0
-                                and kj < self.n_y - 1
+                                and kj < self.elements_circumferential - 1
                             ):
                                 Mat_coef_T[k - 1, k - 1] = AP
                                 Mat_coef_T[k - 1, k - 2] = AW
                                 Mat_coef_T[
                                     k - 1, k - self.elements_circumferential - 1
                                 ] = AS
                                 Mat_coef_T[
                                     k - 1, k + self.elements_circumferential - 1
                                 ] = AN
                                 Mat_coef_T[k - 1, k] = AE
 
                             elif (
                                 ki == self.elements_axial - 1
                                 and kj > 0
-                                and kj < self.n_y - 1
+                                and kj < self.elements_circumferential - 1
                             ):
                                 Mat_coef_T[k - 1, k - 1] = AP + AN
                                 Mat_coef_T[k - 1, k] = AE
                                 Mat_coef_T[k - 1, k - 2] = AW
                                 Mat_coef_T[
                                     k - 1, k - self.elements_circumferential - 1
                                 ] = AS
 
-                            elif ki == 0 and kj == self.n_y - 1:
+                            elif ki == 0 and kj == self.elements_circumferential - 1:
                                 Mat_coef_T[k - 1, k - 1] = AP + AE + AS
                                 Mat_coef_T[k - 1, k - 2] = AW
                                 Mat_coef_T[
                                     k - 1, k + self.elements_circumferential - 1
                                 ] = AN
 
                             elif (
-                                kj == self.n_y - 1
+                                kj == self.elements_circumferential - 1
                                 and ki > 0
                                 and ki < self.elements_axial - 1
                             ):
                                 Mat_coef_T[k - 1, k - 1] = AP + AE
                                 Mat_coef_T[k - 1, k - 2] = AW
                                 Mat_coef_T[
                                     k - 1, k - self.elements_circumferential - 1
                                 ] = AS
                                 Mat_coef_T[
                                     k - 1, k + self.elements_circumferential - 1
                                 ] = AN
 
-                            elif ki == self.elements_axial - 1 and kj == self.n_y - 1:
+                            elif (
+                                ki == self.elements_axial - 1
+                                and kj == self.elements_circumferential - 1
+                            ):
                                 Mat_coef_T[k - 1, k - 1] = AP + AE + AN
                                 Mat_coef_T[k - 1, k - 2] = AW
                                 Mat_coef_T[
                                     k - 1, k - self.elements_circumferential - 1
                                 ] = AS
 
                             kj = kj + 1
@@ -1087,85 +1561,124 @@
                     # Solution of temperature field end
 
                     t = np.linalg.solve(Mat_coef_T, b_T)
                     cont = 0
 
                     for i in np.arange(self.elements_axial):
                         for j in np.arange(self.elements_circumferential):
-
                             T_new[i, j, n_p] = t[cont]
                             cont = cont + 1
 
                     Tdim = T_new * self.reference_temperature
 
-                    T_end = np.sum(Tdim[:, -1, n_p]) / self.elements_axial
+                    T_end[n_p] = np.sum(Tdim[:, -1, n_p]) / self.elements_axial
 
-                    T_mist[n_p] = (
-                        self.fat_mixt[n_p] * self.reference_temperature
-                        + (1 - self.fat_mixt[n_p]) * T_end
+                    if self.operating_type == "flooded":
+                        T_mist[n_p - 1] = (
+                            self.fat_mixt[n_p] * self.reference_temperature
+                            + (1 - self.fat_mixt[n_p]) * T_end[n_p]
+                        )
+
+                    mu_new[:, :, n_p] = (
+                        self.a * (Tdim[:, :, n_p]) ** self.b
+                    ) / self.reference_viscosity
+
+            if self.operating_type == "starvation":
+                for n_p in np.arange(self.n_pad):
+                    self.Qedim[n_p] = (
+                        self.radial_clearance
+                        * self.H[0, n_p]
+                        * self.speed
+                        * self.journal_radius
+                        * self.axial_length
+                        * self.Theta_vol[0, 0, n_p]
+                        * (np.mean(U[:, 0, n_p]))
                     )
 
-                    for i in np.arange(self.elements_axial):
-                        for j in np.arange(self.elements_circumferential):
+                    self.Qsdim[n_p] = (
+                        self.radial_clearance
+                        * self.H[-1, n_p]
+                        * self.speed
+                        * self.journal_radius
+                        * self.axial_length
+                        * self.Theta_vol[0, -1, n_p]
+                        * (np.mean(U[:, -1, n_p]))
+                    )
+
+                geometry_factor = np.ones(self.n_pad)
+
+                for n_p in np.arange(self.n_pad):
+                    geometry_factor[n_p] = (self.Qedim[n_p] + self.Qsdim[n_p - 1]) / (
+                        np.sum(self.Qedim) + np.sum(self.Qsdim)
+                    )
 
-                            mu_new[i, j, n_p] = (
-                                self.a * (Tdim[i, j, n_p]) ** self.b
-                            ) / self.reference_viscosity
+                for n_p in np.arange(self.n_pad):
+                    T_mist[n_p] = (
+                        (self.Qsdim[n_p - 1] * T_end[n_p - 1])
+                        + (
+                            self.reference_temperature
+                            * geometry_factor[n_p]
+                            * self.oil_flow
+                        )
+                    ) / (geometry_factor[n_p] * self.oil_flow + self.Qsdim[n_p - 1])
+
+                    self.theta_vol_groove[n_p] = (
+                        0.8
+                        * (geometry_factor[n_p] * self.oil_flow + self.Qsdim[n_p - 1])
+                        / self.Qedim[n_p]
+                    )
 
-        PP = np.zeros(
-            ((self.elements_axial), (self.n_pad * self.elements_circumferential))
+                    if self.theta_vol_groove[n_p] > 1:
+                        self.theta_vol_groove[n_p] = 1
+
+        PPlot = np.zeros(
+            (self.elements_axial, self.elements_circumferential * self.n_pad)
         )
 
-        i = 0
         for i in range(self.elements_axial):
-
-            PP[i] = self.Pdim[i, :, :].ravel("F")
+            PPlot[i] = self.Pdim[i, :, :].ravel("F")
 
         Ytheta = np.array(Ytheta)
         Ytheta = Ytheta.flatten()
 
         auxF = np.zeros((2, len(Ytheta)))
 
         auxF[0, :] = np.cos(Ytheta)
         auxF[1, :] = np.sin(Ytheta)
 
-        dA = self.dy * self.dz
-
-        auxP = PP * dA
-
-        vector_auxF_x = auxF[0, :]
-        vector_auxF_y = auxF[1, :]
+        fx1 = np.trapz(PPlot * auxF[0, :], self.journal_radius * Ytheta)
+        Fhx = -np.trapz(fx1, self.axial_length * self.Z[1 : self.elements_axial + 1])
 
-        auxFx = auxP * vector_auxF_x
-        auxFy = auxP * vector_auxF_y
+        fy1 = np.trapz(PPlot * auxF[1, :], self.journal_radius * Ytheta)
+        Fhy = -np.trapz(fy1, self.axial_length * self.Z[1 : self.elements_axial + 1])
+        F1 = Fhx
+        F2 = Fhy
 
-        fxj = -np.sum(auxFx)
-        fyj = -np.sum(auxFy)
+        Fhx = F1
+        Fhy = F2
 
-        Fhx = fxj
-        Fhy = fyj
         self.Fhx = Fhx
         self.Fhy = Fhy
         return Fhx, Fhy
 
     def run(self):
         """This method runs the optimization to find the equilibrium position of
         the rotor's center.
 
-
         """
+
         args = self.print_progress
         t1 = time.time()
         res = minimize(
             self._score,
             self.initial_guess,
             args,
             method="Nelder-Mead",
-            tol=10e-3,
-            options={"maxiter": 1000},
+            tol=10e-2,
+            options={"maxiter": 1e4},
         )
         self.equilibrium_pos = res.x
         t2 = time.time()
 
         if self.print_result:
             print(res)
 
@@ -1196,15 +1709,15 @@
 
         def viscosity(x, a, b):
             return a * (x**b)
 
         xdata = [T_muI, T_muF]  # changed boundary conditions to avoid division by ]
         ydata = [mu_I, mu_F]
 
-        popt, pcov = curve_fit(viscosity, xdata, ydata, p0=(6.0, -1.0))
+        popt, pcov = curve_fit(viscosity, xdata, ydata, p0=(6.0, 1.0))
         a, b = popt
 
         return a, b
 
     def coefficients(self):
         """Calculates the dynamic coefficients of stiffness "k" and damping "c".
         Basic reference is found at :cite:t:`lund1978`
@@ -1292,28 +1805,28 @@
         Kyx = -self.sommerfeld(Auinitial_guess1[1], Auinitial_guess2[1]) * (
             (Auinitial_guess1[1] - Auinitial_guess2[1]) / (epix / self.radial_clearance)
         )
         Kyy = -self.sommerfeld(Auinitial_guess3[1], Auinitial_guess4[1]) * (
             (Auinitial_guess3[1] - Auinitial_guess4[1]) / (epiy / self.radial_clearance)
         )
 
-        Cxx = -self.sommerfeld(Auinitial_guess5[0], Auinitial_guess6[0]) * (
-            (Auinitial_guess6[0] - Auinitial_guess5[0])
+        Cxx = -self.sommerfeld(Auinitial_guess5[0], Auinitial_guess6[1]) * (
+            (Auinitial_guess5[0] - Auinitial_guess6[0])
             / (epixpt / self.radial_clearance / self.speed)
         )
-        Cxy = -self.sommerfeld(Auinitial_guess7[0], Auinitial_guess8[0]) * (
-            (Auinitial_guess8[0] - Auinitial_guess7[0])
+        Cxy = -self.sommerfeld(Auinitial_guess7[0], Auinitial_guess8[1]) * (
+            (Auinitial_guess7[0] - Auinitial_guess8[0])
             / (epiypt / self.radial_clearance / self.speed)
         )
-        Cyx = -self.sommerfeld(Auinitial_guess5[1], Auinitial_guess6[1]) * (
-            (Auinitial_guess6[1] - Auinitial_guess5[1])
+        Cyx = -self.sommerfeld(Auinitial_guess5[0], Auinitial_guess6[1]) * (
+            (Auinitial_guess5[1] - Auinitial_guess6[1])
             / (epixpt / self.radial_clearance / self.speed)
         )
-        Cyy = -self.sommerfeld(Auinitial_guess7[1], Auinitial_guess8[1]) * (
-            (Auinitial_guess8[1] - Auinitial_guess7[1])
+        Cyy = -self.sommerfeld(Auinitial_guess7[0], Auinitial_guess8[1]) * (
+            (Auinitial_guess7[1] - Auinitial_guess8[1])
             / (epiypt / self.radial_clearance / self.speed)
         )
 
         kxx = (
             np.sqrt((self.load_x_direction**2) + (self.load_y_direction**2))
             / self.radial_clearance
         ) * Kxx
@@ -1350,500 +1863,807 @@
         return (kxx, kxy, kyx, kyy), (cxx, cxy, cyx, cyy)
 
     def _lund_method(self):
         """In this method a small amplitude whirl of the journal center (a first
         order perturbation solution) is aplied. The four stiffness coefficients,
         and the four damping coefficients is obtained by integration of the pressure
         field.
-
-
         """
 
-        p = self.P
-
-        initial_guess = self.equilibrium_pos
-
-        dZ = 1 / self.elements_axial
-
-        Z1 = 0
-        Z2 = 1
-        Z = np.arange(Z1 + 0.5 * dZ, Z2, dZ)
-        Zdim = Z * self.axial_length
-
-        Ytheta = np.zeros((self.n_pad, self.elements_circumferential))
-
-        # Dimensionless
-        xr = initial_guess[0] * self.radial_clearance * np.cos(initial_guess[1])
-        yr = initial_guess[0] * self.radial_clearance * np.sin(initial_guess[1])
-        Y = yr / self.radial_clearance
-        X = xr / self.radial_clearance
+        Ytheta = [
+            np.linspace(
+                t1 + self.dtheta / 2,
+                t2 - self.dtheta / 2,
+                self.elements_circumferential,
+            )
+            for t1, t2 in zip(self.thetaI, self.thetaF)
+        ]
 
         nk = (self.elements_axial) * (self.elements_circumferential)
 
         gamma = 0.001
 
-        wp = gamma * self.speed
-
-        Mat_coef = np.zeros((nk, nk))
-
-        bX = np.zeros((nk, 1)).astype(complex)
-
-        bY = np.zeros((nk, 1)).astype(complex)
-
-        hX = np.zeros((self.n_pad, self.elements_circumferential))
+        HX = -np.cos(Ytheta)
 
-        hY = np.zeros((self.n_pad, self.elements_circumferential))
+        HY = -np.sin(Ytheta)
 
         PX = np.zeros(
             (self.elements_axial, self.elements_circumferential, self.n_pad)
         ).astype(complex)
 
         PY = np.zeros(
             (self.elements_axial, self.elements_circumferential, self.n_pad)
         ).astype(complex)
 
-        H = np.zeros((2, 2)).astype(complex)
-
-        n_p = 0
-
-        for n_p in np.arange(self.n_pad):
-
-            Ytheta[n_p, :] = np.arange(
-                self.thetaI[n_p] + (self.dtheta / 2), self.thetaF[n_p], self.dtheta
+        if self.operating_type == "flooded":
+            self.theta_vol_groove = np.ones(self.n_pad)
+            self.Theta_vol = np.ones(
+                (self.elements_axial, self.elements_circumferential, self.n_pad)
             )
 
-            ki = 0
-            kj = 0
-
-            k = 0
-
-            for ii in np.arange((self.Z_I + 0.5 * self.dZ), self.Z_F, self.dZ):
-                for jj in np.arange(
-                    self.thetaI[n_p] + (self.dtheta / 2), self.thetaF[n_p], self.dtheta
-                ):
-
-                    hP = 1 - X * np.cos(jj) - Y * np.sin(jj)
-                    he = (
-                        1
-                        - X * np.cos(jj + 0.5 * self.dtheta)
-                        - self.Y * np.sin(jj + 0.5 * self.dtheta)
-                    )
-                    hw = (
-                        1
-                        - X * np.cos(jj - 0.5 * self.dtheta)
-                        - self.Y * np.sin(jj - 0.5 * self.dtheta)
-                    )
-                    hn = hP
-                    hs = hn
-
-                    hXP = -np.cos(jj)
-                    hXe = -np.cos(jj + 0.5 * self.dtheta)
-                    hXw = -np.cos(jj - 0.5 * self.dtheta)
-                    hXn = hXP
-                    hXs = hXn
-
-                    hYP = -np.sin(jj)
-                    hYe = -np.sin(jj + 0.5 * self.dtheta)
-                    hYw = -np.sin(jj - 0.5 * self.dtheta)
-                    hYn = hYP
-                    hYs = hYn
-
-                    if ki == 0:
-                        hX[n_p, kj] = hXP
-                        hY[n_p, kj] = hYP
-
-                    if kj == 0 and ki == 0:
-                        MU_e = 0.5 * (
-                            self.mu_l[ki, kj, n_p] + self.mu_l[ki, kj + 1, n_p]
-                        )
-                        MU_w = self.mu_l[ki, kj, n_p]
-                        MU_s = self.mu_l[ki, kj, n_p]
-                        MU_n = 0.5 * (
-                            self.mu_l[ki, kj, n_p] + self.mu_l[ki + 1, kj, n_p]
-                        )
-
-                        pE = p[ki, kj + 1, n_p]
-                        pW = -p[ki, kj, n_p]
-                        pN = p[ki + 1, kj, n_p]
-                        pS = -p[ki, kj, n_p]
-
-                    if kj == 0 and ki > 0 and ki < self.elements_axial - 1:
-                        MU_e = 0.5 * (
-                            self.mu_l[ki, kj, n_p] + self.mu_l[ki, kj + 1, n_p]
-                        )
-                        MU_w = self.mu_l[ki, kj, n_p]
-                        MU_s = 0.5 * (
-                            self.mu_l[ki, kj, n_p] + self.mu_l[ki - 1, kj, n_p]
-                        )
-                        MU_n = 0.5 * (
-                            self.mu_l[ki, kj, n_p] + self.mu_l[ki + 1, kj, n_p]
-                        )
-
-                        pE = p[ki, kj + 1, n_p]
-                        pW = -p[ki, kj, n_p]
-                        pN = p[ki + 1, kj, n_p]
-                        pS = p[ki - 1, kj, n_p]
-
-                    if kj == 0 and ki == self.elements_axial - 1:
-                        MU_e = 0.5 * (
-                            self.mu_l[ki, kj, n_p] + self.mu_l[ki, kj + 1, n_p]
-                        )
-                        MU_w = self.mu_l[ki, kj, n_p]
-                        MU_s = 0.5 * (
-                            self.mu_l[ki, kj, n_p] + self.mu_l[ki - 1, kj, n_p]
-                        )
-                        MU_n = self.mu_l[ki, kj, n_p]
-
-                        pE = p[ki, kj + 1, n_p]
-                        pW = -p[ki, kj, n_p]
-                        pN = -p[ki, kj, n_p]
-                        pS = p[ki - 1, kj, n_p]
+        for n_p in np.arange(self.n_pad):
+            erro = 1
 
-                    if ki == 0 and kj > 0 and kj < self.elements_circumferential - 1:
-                        MU_e = 0.5 * (
-                            self.mu_l[ki, kj, n_p] + self.mu_l[ki, kj + 1, n_p]
-                        )
-                        MU_w = 0.5 * (
-                            self.mu_l[ki, kj, n_p] + self.mu_l[ki, kj - 1, n_p]
-                        )
-                        MU_s = self.mu_l[ki, kj, n_p]
-                        MU_n = 0.5 * (
-                            self.mu_l[ki, kj, n_p] + self.mu_l[ki + 1, kj, n_p]
-                        )
+            while erro > 1e-6:
+                PX_old = np.array(PX)
+                PY_old = np.array(PY)
 
-                        pE = p[ki, kj + 1, n_p]
-                        pW = p[ki, kj - 1, n_p]
-                        pN = p[ki + 1, kj, n_p]
-                        pS = -p[ki, kj, n_p]
+                Mat_coef = np.zeros((nk, nk))
+                Mat_coefX = np.zeros((nk, nk))
+                Mat_coefY = np.zeros((nk, nk))
 
-                    if (
-                        kj > 0
-                        and kj < self.elements_circumferential - 1
-                        and ki > 0
-                        and ki < self.elements_axial - 1
-                    ):
-                        MU_e = 0.5 * (
-                            self.mu_l[ki, kj, n_p] + self.mu_l[ki, kj + 1, n_p]
-                        )
-                        MU_w = 0.5 * (
-                            self.mu_l[ki, kj, n_p] + self.mu_l[ki, kj - 1, n_p]
-                        )
-                        MU_s = 0.5 * (
-                            self.mu_l[ki, kj, n_p] + self.mu_l[ki - 1, kj, n_p]
-                        )
-                        MU_n = 0.5 * (
-                            self.mu_l[ki, kj, n_p] + self.mu_l[ki + 1, kj, n_p]
-                        )
+                ki = 0
+                kj = 0
 
-                        pE = p[ki, kj + 1, n_p]
-                        pW = p[ki, kj - 1, n_p]
-                        pN = p[ki + 1, kj, n_p]
-                        pS = p[ki - 1, kj, n_p]
+                k = 0
 
-                    if (
-                        ki == self.elements_axial - 1
-                        and kj > 0
-                        and kj < self.elements_circumferential - 1
+                for ii in np.arange((self.Z_I + 0.5 * self.dZ), self.Z_F, self.dZ):
+                    for jj in np.arange(
+                        self.thetaI[n_p] + (self.dtheta / 2),
+                        self.thetaF[n_p],
+                        self.dtheta,
                     ):
-                        MU_e = 0.5 * (
-                            self.mu_l[ki, kj, n_p] + self.mu_l[ki, kj + 1, n_p]
-                        )
-                        MU_w = 0.5 * (
-                            self.mu_l[ki, kj, n_p] + self.mu_l[ki, kj - 1, n_p]
-                        )
-                        MU_s = 0.5 * (
-                            self.mu_l[ki, kj, n_p] + self.mu_l[ki - 1, kj, n_p]
-                        )
-                        MU_n = self.mu_l[ki, kj, n_p]
-
-                        pE = p[ki, kj + 1, n_p]
-                        pW = p[ki, kj - 1, n_p]
-                        pN = -p[ki, kj, n_p]
-                        pS = p[ki - 1, kj, n_p]
-
-                    if ki == 0 and kj == self.elements_circumferential - 1:
-                        MU_e = self.mu_l[ki, kj, n_p]
-                        MU_w = 0.5 * (
-                            self.mu_l[ki, kj, n_p] + self.mu_l[ki, kj - 1, n_p]
-                        )
-                        MU_s = self.mu_l[ki, kj, n_p]
-                        MU_n = 0.5 * (
-                            self.mu_l[ki, kj, n_p] + self.mu_l[ki + 1, kj, n_p]
-                        )
-
-                        pE = -p[ki, kj, n_p]
-                        pW = p[ki, kj - 1, n_p]
-                        pN = p[ki + 1, kj, n_p]
-                        pS = -p[ki, kj, n_p]
+                        if self.P[ki, kj, n_p] > 0:
+                            HP = 1 - self.X * np.cos(jj) - self.Y * np.sin(jj)
+                            He = (
+                                1
+                                - self.X * np.cos(jj + 0.5 * self.dtheta)
+                                - self.Y * np.sin(jj + 0.5 * self.dtheta)
+                            )
+                            Hw = (
+                                1
+                                - self.X * np.cos(jj - 0.5 * self.dtheta)
+                                - self.Y * np.sin(jj - 0.5 * self.dtheta)
+                            )
 
-                    if (
-                        kj == self.elements_circumferential - 1
-                        and ki > 0
-                        and ki < self.elements_axial - 1
-                    ):
-                        MU_e = self.mu_l[ki, kj, n_p]
-                        MU_w = 0.5 * (
-                            self.mu_l[ki, kj, n_p] + self.mu_l[ki, kj - 1, n_p]
-                        )
-                        MU_s = 0.5 * (
-                            self.mu_l[ki, kj, n_p] + self.mu_l[ki - 1, kj, n_p]
-                        )
-                        MU_n = 0.5 * (
-                            self.mu_l[ki, kj, n_p] + self.mu_l[ki + 1, kj, n_p]
-                        )
+                            HXP = -np.cos(jj)
+                            HXe = -np.cos(jj + 0.5 * self.dtheta)
+                            HXw = -np.cos(jj - 0.5 * self.dtheta)
+
+                            HYP = -np.sin(jj)
+                            HYe = -np.sin(jj + 0.5 * self.dtheta)
+                            HYw = -np.sin(jj - 0.5 * self.dtheta)
 
-                        pE = -p[ki, kj, n_p]
-                        pW = p[ki, kj - 1, n_p]
-                        pN = p[ki + 1, kj, n_p]
-                        pS = p[ki - 1, kj, n_p]
+                            HXptP = 0
+                            HYptP = 0
 
-                    if (
-                        kj == self.elements_circumferential - 1
-                        and ki == self.elements_axial - 1
-                    ):
-                        MU_e = self.mu_l[ki, kj, n_p]
-                        MU_w = 0.5 * (
-                            self.mu_l[ki, kj, n_p] + self.mu_l[ki, kj - 1, n_p]
-                        )
-                        MU_s = 0.5 * (
-                            self.mu_l[ki, kj, n_p] + self.mu_l[ki - 1, kj, n_p]
-                        )
-                        MU_n = self.mu_l[ki, kj, n_p]
+                            if kj == 0 and ki == 0:
+                                MU_e = 0.5 * (
+                                    self.mu_l[ki, kj, n_p] + self.mu_l[ki, kj + 1, n_p]
+                                )
+                                MU_w = self.mu_l[ki, kj, n_p]
+                                MU_s = self.mu_l[ki, kj, n_p]
+                                MU_n = 0.5 * (
+                                    self.mu_l[ki, kj, n_p] + self.mu_l[ki + 1, kj, n_p]
+                                )
 
-                        pE = -p[ki, kj, n_p]
-                        pW = p[ki, kj - 1, n_p]
-                        pN = -p[ki, kj, n_p]
-                        pS = p[ki - 1, kj, n_p]
+                            if kj == 0 and ki > 0 and ki < self.elements_axial - 1:
+                                MU_e = 0.5 * (
+                                    self.mu_l[ki, kj, n_p] + self.mu_l[ki, kj + 1, n_p]
+                                )
+                                MU_w = self.mu_l[ki, kj, n_p]
+                                MU_s = 0.5 * (
+                                    self.mu_l[ki, kj, n_p] + self.mu_l[ki - 1, kj, n_p]
+                                )
+                                MU_n = 0.5 * (
+                                    self.mu_l[ki, kj, n_p] + self.mu_l[ki + 1, kj, n_p]
+                                )
 
-                    pP = p[ki, kj, n_p]
+                            if kj == 0 and ki == self.elements_axial - 1:
+                                MU_e = 0.5 * (
+                                    self.mu_l[ki, kj, n_p] + self.mu_l[ki, kj + 1, n_p]
+                                )
+                                MU_w = self.mu_l[ki, kj, n_p]
+                                MU_s = 0.5 * (
+                                    self.mu_l[ki, kj, n_p] + self.mu_l[ki - 1, kj, n_p]
+                                )
+                                MU_n = self.mu_l[ki, kj, n_p]
 
-                    CE = (self.dZ * he**3) / (12 * MU_e * self.dY * self.betha_s**2)
-                    CW = (self.dZ * hw**3) / (12 * MU_w * self.dY * self.betha_s**2)
-                    CN = (self.dY * (self.journal_radius**2) * hn**3) / (
-                        12 * MU_n * self.dZ * self.axial_length**2
-                    )
-                    CS = (self.dY * (self.journal_radius**2) * hs**3) / (
-                        12 * MU_s * self.dZ * self.axial_length**2
-                    )
+                            if (
+                                ki == 0
+                                and kj > 0
+                                and kj < self.elements_circumferential - 1
+                            ):
+                                MU_e = 0.5 * (
+                                    self.mu_l[ki, kj, n_p] + self.mu_l[ki, kj + 1, n_p]
+                                )
+                                MU_w = 0.5 * (
+                                    self.mu_l[ki, kj, n_p] + self.mu_l[ki, kj - 1, n_p]
+                                )
+                                MU_s = self.mu_l[ki, kj, n_p]
+                                MU_n = 0.5 * (
+                                    self.mu_l[ki, kj, n_p] + self.mu_l[ki + 1, kj, n_p]
+                                )
 
-                    CP = -(CE + CW + CN + CS)
+                            if (
+                                kj > 0
+                                and kj < self.elements_circumferential - 1
+                                and ki > 0
+                                and ki < self.elements_axial - 1
+                            ):
+                                MU_e = 0.5 * (
+                                    self.mu_l[ki, kj, n_p] + self.mu_l[ki, kj + 1, n_p]
+                                )
+                                MU_w = 0.5 * (
+                                    self.mu_l[ki, kj, n_p] + self.mu_l[ki, kj - 1, n_p]
+                                )
+                                MU_s = 0.5 * (
+                                    self.mu_l[ki, kj, n_p] + self.mu_l[ki - 1, kj, n_p]
+                                )
+                                MU_n = 0.5 * (
+                                    self.mu_l[ki, kj, n_p] + self.mu_l[ki + 1, kj, n_p]
+                                )
 
-                    BXE = -(self.dZ / (self.dY * self.betha_s**2)) * (
-                        (3 * he**2 * hXe) / (12 * MU_e)
-                    )
+                            if (
+                                ki == self.elements_axial - 1
+                                and kj > 0
+                                and kj < self.elements_circumferential - 1
+                            ):
+                                MU_e = 0.5 * (
+                                    self.mu_l[ki, kj, n_p] + self.mu_l[ki, kj + 1, n_p]
+                                )
+                                MU_w = 0.5 * (
+                                    self.mu_l[ki, kj, n_p] + self.mu_l[ki, kj - 1, n_p]
+                                )
+                                MU_s = 0.5 * (
+                                    self.mu_l[ki, kj, n_p] + self.mu_l[ki - 1, kj, n_p]
+                                )
+                                MU_n = self.mu_l[ki, kj, n_p]
 
-                    BYE = -(self.dZ / (self.dY * self.betha_s**2)) * (
-                        (3 * he**2 * hYe) / (12 * MU_e)
-                    )
+                            if ki == 0 and kj == self.elements_circumferential - 1:
+                                MU_e = self.mu_l[ki, kj, n_p]
+                                MU_w = 0.5 * (
+                                    self.mu_l[ki, kj, n_p] + self.mu_l[ki, kj - 1, n_p]
+                                )
+                                MU_s = self.mu_l[ki, kj, n_p]
+                                MU_n = 0.5 * (
+                                    self.mu_l[ki, kj, n_p] + self.mu_l[ki + 1, kj, n_p]
+                                )
 
-                    BXW = -(self.dZ / (self.dY * self.betha_s**2)) * (
-                        (3 * hw**2 * hXw) / (12 * MU_w)
-                    )
+                            if (
+                                kj == self.elements_circumferential - 1
+                                and ki > 0
+                                and ki < self.elements_axial - 1
+                            ):
+                                MU_e = self.mu_l[ki, kj, n_p]
+                                MU_w = 0.5 * (
+                                    self.mu_l[ki, kj, n_p] + self.mu_l[ki, kj - 1, n_p]
+                                )
+                                MU_s = 0.5 * (
+                                    self.mu_l[ki, kj, n_p] + self.mu_l[ki - 1, kj, n_p]
+                                )
+                                MU_n = 0.5 * (
+                                    self.mu_l[ki, kj, n_p] + self.mu_l[ki + 1, kj, n_p]
+                                )
 
-                    BYW = -(self.dZ / (self.dY * self.betha_s**2)) * (
-                        (3 * hw**2 * hYw) / (12 * MU_w)
-                    )
+                            if (
+                                kj == self.elements_circumferential - 1
+                                and ki == self.elements_axial - 1
+                            ):
+                                MU_e = self.mu_l[ki, kj, n_p]
+                                MU_w = 0.5 * (
+                                    self.mu_l[ki, kj, n_p] + self.mu_l[ki, kj - 1, n_p]
+                                )
+                                MU_s = 0.5 * (
+                                    self.mu_l[ki, kj, n_p] + self.mu_l[ki - 1, kj, n_p]
+                                )
+                                MU_n = self.mu_l[ki, kj, n_p]
 
-                    BXN = -(
-                        (self.journal_radius**2)
-                        * self.dY
-                        / (self.dZ * self.axial_length**2)
-                    ) * ((3 * hn**2 * hXn) / (12 * MU_n))
-
-                    BYN = -(
-                        (self.journal_radius**2)
-                        * self.dY
-                        / (self.dZ * self.axial_length**2)
-                    ) * ((3 * hn**2 * hYn) / (12 * MU_n))
-
-                    BXS = -(
-                        (self.journal_radius**2)
-                        * self.dY
-                        / (self.dZ * self.axial_length**2)
-                    ) * ((3 * hs**2 * hXs) / (12 * MU_s))
-
-                    BYS = -(
-                        (self.journal_radius**2)
-                        * self.dY
-                        / (self.dZ * self.axial_length**2)
-                    ) * ((3 * hs**2 * hYs) / (12 * MU_s))
-
-                    BXP = -(BXE + BXW + BXN + BXS)
-
-                    BYP = -(BYE + BYW + BYN + BYS)
-
-                    BX = (
-                        (self.dZ / (2 * self.betha_s)) * (hXe - hXw)
-                        + (self.dY * self.dZ * 1j * gamma * hXP)
-                        + BXE * pE
-                        + BXW * pW
-                        + BXN * pN
-                        + BXS * pS
-                        + BXP * pP
-                    )
+                            CE = (
+                                1
+                                / self.betha_s**2
+                                * He**3
+                                / (12 * MU_e)
+                                * self.dZ
+                                / self.dY
+                            )
+                            CW = (
+                                1
+                                / self.betha_s**2
+                                * Hw**3
+                                / (12 * MU_w)
+                                * self.dZ
+                                / self.dY
+                            )
+                            CN = (
+                                (self.journal_radius / self.axial_length) ** 2
+                                * HP**3
+                                / (12 * MU_n)
+                                * self.dY
+                                / self.dZ
+                            )
+                            CS = (
+                                (self.journal_radius / self.axial_length) ** 2
+                                * HP**3
+                                / (12 * MU_s)
+                                * self.dY
+                                / self.dZ
+                            )
+                            CP = -(CE + CW + CN + CS)
 
-                    BY = (
-                        (self.dZ / (2 * self.betha_s)) * (hYe - hYw)
-                        + (self.dY * self.dZ * 1j * gamma * hYP)
-                        + BYE * pE
-                        + BYW * pW
-                        + BYN * pN
-                        + BYS * pS
-                        + BYP * pP
-                    )
+                            CXE = (
+                                -1
+                                / self.betha_s**2
+                                * He**2
+                                * HXe
+                                / (4 * MU_e)
+                                * self.dZ
+                                / self.dY
+                            )
+                            CXW = (
+                                -1
+                                / self.betha_s**2
+                                * Hw**2
+                                * HXw
+                                / (4 * MU_w)
+                                * self.dZ
+                                / self.dY
+                            )
+                            CXN = (
+                                -((self.journal_radius / self.axial_length) ** 2)
+                                * HP**2
+                                * HXP
+                                / (4 * MU_n)
+                                * self.dY
+                                / self.dZ
+                            )
+                            CXS = (
+                                -((self.journal_radius / self.axial_length) ** 2)
+                                * HP**2
+                                * HXP
+                                / (4 * MU_s)
+                                * self.dY
+                                / self.dZ
+                            )
+                            CXP = -(CXE + CXW + CXN + CXS)
 
-                    k = k + 1
-                    bX[k - 1, 0] = BX
-                    bY[k - 1, 0] = BY
+                            CYE = (
+                                -1
+                                / self.betha_s**2
+                                * He**2
+                                * HYe
+                                / (4 * MU_e)
+                                * self.dZ
+                                / self.dY
+                            )
+                            CYW = (
+                                -1
+                                / self.betha_s**2
+                                * Hw**2
+                                * HYw
+                                / (4 * MU_w)
+                                * self.dZ
+                                / self.dY
+                            )
+                            CYN = (
+                                -((self.journal_radius / self.axial_length) ** 2)
+                                * HP**2
+                                * HYP
+                                / (4 * MU_n)
+                                * self.dY
+                                / self.dZ
+                            )
+                            CYS = (
+                                -((self.journal_radius / self.axial_length) ** 2)
+                                * HP**2
+                                * HYP
+                                / (4 * MU_s)
+                                * self.dY
+                                / self.dZ
+                            )
+                            CYP = -(CYE + CYW + CYN + CYS)
 
-                    if ki == 0 and kj == 0:
-                        Mat_coef[k - 1, k - 1] = CP - CS - CW
-                        Mat_coef[k - 1, k] = CE
-                        Mat_coef[k - 1, k + self.elements_circumferential - 1] = CN
-
-                    elif kj == 0 and ki > 0 and ki < self.elements_axial - 1:
-                        Mat_coef[k - 1, k - 1] = CP - CW
-                        Mat_coef[k - 1, k] = CE
-                        Mat_coef[k - 1, k - self.elements_circumferential - 1] = CS
-                        Mat_coef[k - 1, k + self.elements_circumferential - 1] = CN
-
-                    elif kj == 0 and ki == self.elements_axial - 1:
-                        Mat_coef[k - 1, k - 1] = CP - CN - CW
-                        Mat_coef[k - 1, k] = CE
-                        Mat_coef[k - 1, k - self.elements_circumferential - 1] = CS
-
-                    elif ki == 0 and kj > 0 and kj < self.elements_circumferential - 1:
-                        Mat_coef[k - 1, k - 1] = CP - CS
-                        Mat_coef[k - 1, k] = CE
-                        Mat_coef[k - 1, k - 2] = CW
-                        Mat_coef[k - 1, k + self.elements_circumferential - 1] = CN
+                            KXW = -1 / (2 * self.betha_s) * HXw * self.dZ
+                            KXP = (
+                                1 / (2 * self.betha_s) * HXe * self.dZ
+                                + (HXptP + 1j * gamma * HXP) * self.dY * self.dZ
+                            )
 
-                    if (
-                        ki > 0
-                        and ki < self.elements_axial - 1
-                        and kj > 0
-                        and kj < self.elements_circumferential - 1
-                    ):
-                        Mat_coef[k - 1, k - 1] = CP
-                        Mat_coef[k - 1, k - 2] = CW
-                        Mat_coef[k - 1, k - self.elements_circumferential - 1] = CS
-                        Mat_coef[k - 1, k + self.elements_circumferential - 1] = CN
-                        Mat_coef[k - 1, k] = CE
+                            KYW = -1 / (2 * self.betha_s) * HYw * self.dZ
+                            KYP = (
+                                1 / (2 * self.betha_s) * HYe * self.dZ
+                                + (HYptP + 1j * gamma * HYP) * self.dY * self.dZ
+                            )
 
-                    elif (
-                        ki == self.elements_axial - 1
-                        and kj > 0
-                        and kj < self.elements_circumferential - 1
-                    ):
-                        Mat_coef[k - 1, k - 1] = CP - CN
-                        Mat_coef[k - 1, k] = CE
-                        Mat_coef[k - 1, k - 2] = CW
-                        Mat_coef[k - 1, k - self.elements_circumferential - 1] = CS
-
-                    elif ki == 0 and kj == self.elements_circumferential - 1:
-                        Mat_coef[k - 1, k - 1] = CP - CE - CS
-                        Mat_coef[k - 1, k - 2] = CW
-                        Mat_coef[k - 1, k + self.elements_circumferential - 1] = CN
+                            PP = self.P[:, :, n_p].flatten()
 
-                    elif (
-                        kj == self.elements_circumferential - 1
-                        and ki > 0
-                        and ki < self.elements_axial - 1
-                    ):
-                        Mat_coef[k - 1, k - 1] = CP - CE
-                        Mat_coef[k - 1, k - 2] = CW
-                        Mat_coef[k - 1, k - self.elements_circumferential - 1] = CS
-                        Mat_coef[k - 1, k + self.elements_circumferential - 1] = CN
+                            PPX = PX[:, :, n_p].flatten()
+                            PPX = np.delete(PPX, k)
 
-                    elif (
-                        ki == self.elements_axial - 1
-                        and kj == self.elements_circumferential - 1
-                    ):
-                        Mat_coef[k - 1, k - 1] = CP - CE - CN
-                        Mat_coef[k - 1, k - 2] = CW
-                        Mat_coef[k - 1, k - self.elements_circumferential - 1] = CS
+                            PPY = PY[:, :, n_p].flatten()
+                            PPY = np.delete(PPY, k)
 
-                    kj = kj + 1
+                            if kj == 0 and ki == 0:
+                                Mat_coef[k, k] = CP - CW - CS
+                                Mat_coef[k, k + 1] = CE
+                                Mat_coef[k, k + self.elements_circumferential] = CN
+
+                                Mat_coefX[k, k] = CXP - CXW - CXS
+                                Mat_coefX[k, k + 1] = CXE
+                                Mat_coefX[k, k + self.elements_circumferential] = CXN
+
+                                Mat_coefY[k, k] = CYP - CYW - CYS
+                                Mat_coefY[k, k + 1] = CYE
+                                Mat_coefY[k, k + self.elements_circumferential] = CYN
+
+                                C = Mat_coef[k, :].T
+                                C = np.delete(C, k)
+
+                                CX = Mat_coefX[k, :].T
+                                CY = Mat_coefY[k, :].T
+
+                                BX = (
+                                    np.matmul(CX, PP)
+                                    + KXW * self.theta_vol_groove[n_p]
+                                    + KXP * self.Theta_vol[ki, kj, n_p]
+                                    + 2 * CXW * self.injection_pressure
+                                )
+                                BY = (
+                                    np.matmul(CY, PP)
+                                    + KYW * self.theta_vol_groove[n_p]
+                                    + KYP * self.Theta_vol[ki, kj, n_p]
+                                    + 2 * CYW * self.injection_pressure
+                                )
+
+                                PX[ki, kj, n_p] = (BX - np.matmul(C, PPX)) / Mat_coef[
+                                    k, k
+                                ]
+                                PY[ki, kj, n_p] = (BY - np.matmul(C, PPY)) / Mat_coef[
+                                    k, k
+                                ]
 
-                kj = 0
-                ki = ki + 1
+                            if kj == 0 and ki > 0 and ki < self.elements_axial - 1:
+                                Mat_coef[k, k] = CP - CW
+                                Mat_coef[k, k + 1] = CE
+                                Mat_coef[k, k + self.elements_circumferential] = CN
+                                Mat_coef[k, k - self.elements_circumferential] = CS
+
+                                Mat_coefX[k, k] = CXP - CXW
+                                Mat_coefX[k, k + 1] = CXE
+                                Mat_coefX[k, k + self.elements_circumferential] = CXN
+                                Mat_coefX[k, k - self.elements_circumferential] = CXS
+
+                                Mat_coefY[k, k] = CYP - CYW
+                                Mat_coefY[k, k + 1] = CYE
+                                Mat_coefY[k, k + self.elements_circumferential] = CYN
+                                Mat_coefY[k, k - self.elements_circumferential] = CYS
+
+                                C = Mat_coef[k, :].T
+                                C = np.delete(C, k)
+
+                                CX = Mat_coefX[k, :].T
+                                CY = Mat_coefY[k, :].T
+
+                                BX = (
+                                    np.matmul(CX, PP)
+                                    + KXW * self.theta_vol_groove[n_p]
+                                    + KXP * self.Theta_vol[ki, kj, n_p]
+                                    + 2 * CXW * self.injection_pressure
+                                )
+                                BY = (
+                                    np.matmul(CY, PP)
+                                    + KYW * self.theta_vol_groove[n_p]
+                                    + KYP * self.Theta_vol[ki, kj, n_p]
+                                    + 2 * CYW * self.injection_pressure
+                                )
+
+                                PX[ki, kj, n_p] = (BX - np.matmul(C, PPX)) / Mat_coef[
+                                    k, k
+                                ]
+                                PY[ki, kj, n_p] = (BY - np.matmul(C, PPY)) / Mat_coef[
+                                    k, k
+                                ]
 
-                #    ###################### Solution of pressure field #######################
+                            if kj == 0 and ki == self.elements_axial - 1:
+                                Mat_coef[k, k] = CP - CW - CN
+                                Mat_coef[k, k + 1] = CE
+                                Mat_coef[k, k - self.elements_circumferential] = CS
+
+                                Mat_coefX[k, k] = CXP - CXW - CXN
+                                Mat_coefX[k, k + 1] = CXE
+                                Mat_coefX[k, k - self.elements_circumferential] = CXS
+
+                                Mat_coefY[k, k] = CYP - CYW - CYN
+                                Mat_coefY[k, k + 1] = CYE
+                                Mat_coefY[k, k - self.elements_circumferential] = CYS
+
+                                C = Mat_coef[k, :].T
+                                C = np.delete(C, k)
+
+                                CX = Mat_coefX[k, :].T
+                                CY = Mat_coefY[k, :].T
+
+                                BX = (
+                                    np.matmul(CX, PP)
+                                    + KXW * self.theta_vol_groove[n_p]
+                                    + KXP * self.Theta_vol[ki, kj, n_p]
+                                    + 2 * CXW * self.injection_pressure
+                                )
+                                BY = (
+                                    np.matmul(CY, PP)
+                                    + KYW * self.theta_vol_groove[n_p]
+                                    + KYP * self.Theta_vol[ki, kj, n_p]
+                                    + 2 * CYW * self.injection_pressure
+                                )
+
+                                PX[ki, kj, n_p] = (BX - np.matmul(C, PPX)) / Mat_coef[
+                                    k, k
+                                ]
+                                PY[ki, kj, n_p] = (BY - np.matmul(C, PPY)) / Mat_coef[
+                                    k, k
+                                ]
 
-            pX = np.linalg.solve(Mat_coef, bX)
+                            if (
+                                ki == 0
+                                and kj > 0
+                                and kj < self.elements_circumferential - 1
+                            ):
+                                Mat_coef[k, k] = CP - CS
+                                Mat_coef[k, k + 1] = CE
+                                Mat_coef[k, k - 1] = CW
+                                Mat_coef[k, k + self.elements_circumferential] = CN
+
+                                Mat_coefX[k, k] = CXP - CXS
+                                Mat_coefX[k, k + 1] = CXE
+                                Mat_coefX[k, k - 1] = CXW
+                                Mat_coefX[k, k + self.elements_circumferential] = CXN
+
+                                Mat_coefY[k, k] = CYP - CYS
+                                Mat_coefY[k, k + 1] = CYE
+                                Mat_coefY[k, k - 1] = CYW
+                                Mat_coefY[k, k + self.elements_circumferential] = CYN
+
+                                C = Mat_coef[k, :].T
+                                C = np.delete(C, k)
+
+                                CX = Mat_coefX[k, :].T
+                                CY = Mat_coefY[k, :].T
+
+                                BX = (
+                                    np.matmul(CX, PP)
+                                    + KXW * self.Theta_vol[ki, kj - 1, n_p]
+                                    + KXP * self.Theta_vol[ki, kj, n_p]
+                                )
+                                BY = (
+                                    np.matmul(CY, PP)
+                                    + KYW * self.Theta_vol[ki, kj - 1, n_p]
+                                    + KYP * self.Theta_vol[ki, kj, n_p]
+                                )
+
+                                PX[ki, kj, n_p] = (BX - np.matmul(C, PPX)) / Mat_coef[
+                                    k, k
+                                ]
+                                PY[ki, kj, n_p] = (BY - np.matmul(C, PPY)) / Mat_coef[
+                                    k, k
+                                ]
 
-            pY = np.linalg.solve(Mat_coef, bY)
+                            if (
+                                kj > 0
+                                and kj < self.elements_circumferential - 1
+                                and ki > 0
+                                and ki < self.elements_axial - 1
+                            ):
+                                Mat_coef[k, k] = CP
+                                Mat_coef[k, k + 1] = CE
+                                Mat_coef[k, k - 1] = CW
+                                Mat_coef[k, k + self.elements_circumferential] = CN
+                                Mat_coef[k, k - self.elements_circumferential] = CS
+
+                                Mat_coefX[k, k] = CXP
+                                Mat_coefX[k, k + 1] = CXE
+                                Mat_coefX[k, k - 1] = CXW
+                                Mat_coefX[k, k + self.elements_circumferential] = CXN
+                                Mat_coefX[k, k - self.elements_circumferential] = CXS
+
+                                Mat_coefY[k, k] = CYP
+                                Mat_coefY[k, k + 1] = CYE
+                                Mat_coefY[k, k - 1] = CYW
+                                Mat_coefY[k, k + self.elements_circumferential] = CYN
+                                Mat_coefY[k, k - self.elements_circumferential] = CYS
+
+                                C = Mat_coef[k, :].T
+                                C = np.delete(C, k)
+
+                                CX = Mat_coefX[k, :].T
+                                CY = Mat_coefY[k, :].T
+
+                                BX = (
+                                    np.matmul(CX, PP)
+                                    + KXW * self.Theta_vol[ki, kj - 1, n_p]
+                                    + KXP * self.Theta_vol[ki, kj, n_p]
+                                )
+                                BY = (
+                                    np.matmul(CY, PP)
+                                    + KYW * self.Theta_vol[ki, kj - 1, n_p]
+                                    + KYP * self.Theta_vol[ki, kj, n_p]
+                                )
+
+                                PX[ki, kj, n_p] = (BX - np.matmul(C, PPX)) / Mat_coef[
+                                    k, k
+                                ]
+                                PY[ki, kj, n_p] = (BY - np.matmul(C, PPY)) / Mat_coef[
+                                    k, k
+                                ]
 
-            cont = 0
+                            if (
+                                ki == self.elements_axial - 1
+                                and kj > 0
+                                and kj < self.elements_circumferential - 1
+                            ):
+                                Mat_coef[k, k] = CP - CN
+                                Mat_coef[k, k + 1] = CE
+                                Mat_coef[k, k - 1] = CW
+                                Mat_coef[k, k - self.elements_circumferential] = CS
+
+                                Mat_coefX[k, k] = CXP - CXN
+                                Mat_coefX[k, k + 1] = CXE
+                                Mat_coefX[k, k - 1] = CXW
+                                Mat_coefX[k, k - self.elements_circumferential] = CXS
+
+                                Mat_coefY[k, k] = CYP - CYN
+                                Mat_coefY[k, k + 1] = CYE
+                                Mat_coefY[k, k - 1] = CYW
+                                Mat_coefY[k, k - self.elements_circumferential] = CYS
+
+                                C = Mat_coef[k, :].T
+                                C = np.delete(C, k)
+
+                                CX = Mat_coefX[k, :].T
+                                CY = Mat_coefY[k, :].T
+
+                                BX = (
+                                    np.matmul(CX, PP)
+                                    + KXW * self.Theta_vol[ki, kj - 1, n_p]
+                                    + KXP * self.Theta_vol[ki, kj, n_p]
+                                )
+                                BY = (
+                                    np.matmul(CY, PP)
+                                    + KYW * self.Theta_vol[ki, kj - 1, n_p]
+                                    + KYP * self.Theta_vol[ki, kj, n_p]
+                                )
+
+                                PX[ki, kj, n_p] = (BX - np.matmul(C, PPX)) / Mat_coef[
+                                    k, k
+                                ]
+                                PY[ki, kj, n_p] = (BY - np.matmul(C, PPY)) / Mat_coef[
+                                    k, k
+                                ]
 
-            for i in np.arange(self.elements_axial):
-                for j in np.arange(self.elements_circumferential):
+                            if ki == 0 and kj == self.elements_circumferential - 1:
+                                Mat_coef[k, k] = CP - CE - CS
+                                Mat_coef[k, k - 1] = CW
+                                Mat_coef[k, k + self.elements_circumferential] = CN
+
+                                Mat_coefX[k, k] = CXP - CXE - CXS
+                                Mat_coefX[k, k - 1] = CXW
+                                Mat_coefX[k, k + self.elements_circumferential] = CXN
+
+                                Mat_coefY[k, k] = CYP - CYE - CYS
+                                Mat_coefY[k, k - 1] = CYW
+                                Mat_coefY[k, k + self.elements_circumferential] = CYN
+
+                                C = Mat_coef[k, :].T
+                                C = np.delete(C, k)
+
+                                CX = Mat_coefX[k, :].T
+                                CY = Mat_coefY[k, :].T
+
+                                BX = (
+                                    np.matmul(CX, PP)
+                                    + KXW * self.Theta_vol[ki, kj - 1, n_p]
+                                    + KXP * self.Theta_vol[ki, kj, n_p]
+                                )
+                                BY = (
+                                    np.matmul(CY, PP)
+                                    + KYW * self.Theta_vol[ki, kj - 1, n_p]
+                                    + KYP * self.Theta_vol[ki, kj, n_p]
+                                )
+
+                                PX[ki, kj, n_p] = (BX - np.matmul(C, PPX)) / Mat_coef[
+                                    k, k
+                                ]
+                                PY[ki, kj, n_p] = (BY - np.matmul(C, PPY)) / Mat_coef[
+                                    k, k
+                                ]
 
-                    PX[i, j, n_p] = pX[cont]
-                    PY[i, j, n_p] = pY[cont]
-                    cont = cont + 1
+                            if (
+                                kj == self.elements_circumferential - 1
+                                and ki > 0
+                                and ki < self.elements_axial - 1
+                            ):
+                                Mat_coef[k, k] = CP - CE
+                                Mat_coef[k, k - 1] = CW
+                                Mat_coef[k, k + self.elements_circumferential] = CN
+                                Mat_coef[k, k - self.elements_circumferential] = CS
+
+                                Mat_coefX[k, k] = CXP - CXE
+                                Mat_coefX[k, k - 1] = CXW
+                                Mat_coefX[k, k + self.elements_circumferential] = CXN
+                                Mat_coefX[k, k - self.elements_circumferential] = CXS
+
+                                Mat_coefY[k, k] = CYP - CYE
+                                Mat_coefY[k, k - 1] = CYW
+                                Mat_coefY[k, k + self.elements_circumferential] = CYN
+                                Mat_coefY[k, k - self.elements_circumferential] = CYS
+
+                                C = Mat_coef[k, :].T
+                                C = np.delete(C, k)
+
+                                CX = Mat_coefX[k, :].T
+                                CY = Mat_coefY[k, :].T
+
+                                BX = (
+                                    np.matmul(CX, PP)
+                                    + KXW * self.Theta_vol[ki, kj - 1, n_p]
+                                    + KXP * self.Theta_vol[ki, kj, n_p]
+                                )
+                                BY = (
+                                    np.matmul(CY, PP)
+                                    + KYW * self.Theta_vol[ki, kj - 1, n_p]
+                                    + KYP * self.Theta_vol[ki, kj, n_p]
+                                )
+
+                                PX[ki, kj, n_p] = (BX - np.matmul(C, PPX)) / Mat_coef[
+                                    k, k
+                                ]
+                                PY[ki, kj, n_p] = (BY - np.matmul(C, PPY)) / Mat_coef[
+                                    k, k
+                                ]
 
-        PPlotX = np.zeros(
-            (self.elements_axial, self.elements_circumferential * self.n_pad)
-        ).astype(complex)
-        PPlotY = np.zeros(
-            (self.elements_axial, self.elements_circumferential * self.n_pad)
-        ).astype(complex)
+                            if (
+                                kj == self.elements_circumferential - 1
+                                and ki == self.elements_axial - 1
+                            ):
+                                Mat_coef[k, k] = CP - CE - CN
+                                Mat_coef[k, k - 1] = CW
+                                Mat_coef[k, k - self.elements_circumferential] = CS
+
+                                Mat_coefX[k, k] = CXP - CXE - CXN
+                                Mat_coefX[k, k - 1] = CXW
+                                Mat_coefX[k, k - self.elements_circumferential] = CXS
+
+                                Mat_coefY[k, k] = CYP - CYE - CYN
+                                Mat_coefY[k, k - 1] = CYW
+                                Mat_coefY[k, k - self.elements_circumferential] = CYS
+
+                                C = Mat_coef[k, :].T
+                                C = np.delete(C, k)
+
+                                CX = Mat_coefX[k, :].T
+                                CY = Mat_coefY[k, :].T
+
+                                BX = (
+                                    np.matmul(CX, PP)
+                                    + KXW * self.Theta_vol[ki, kj - 1, n_p]
+                                    + KXP * self.Theta_vol[ki, kj, n_p]
+                                )
+                                BY = (
+                                    np.matmul(CY, PP)
+                                    + KYW * self.Theta_vol[ki, kj - 1, n_p]
+                                    + KYP * self.Theta_vol[ki, kj, n_p]
+                                )
+
+                                PX[ki, kj, n_p] = (BX - np.matmul(C, PPX)) / Mat_coef[
+                                    k, k
+                                ]
+                                PY[ki, kj, n_p] = (BY - np.matmul(C, PPY)) / Mat_coef[
+                                    k, k
+                                ]
 
-        i = 0
-        for i in range(self.elements_axial):
+                        k = k + 1
+                        kj = kj + 1
 
-            PPlotX[i] = PX[i, :, :].ravel("F")
-            PPlotY[i] = PY[i, :, :].ravel("F")
+                    kj = 0
+                    ki = ki + 1
 
-        Ytheta = Ytheta.flatten()
+                erro = np.linalg.norm(PX - PX_old) + np.linalg.norm(PY - PY_old)
 
-        PPlotXdim = (
-            PPlotX
+        PXdim = (
+            PX
             * (self.reference_viscosity * self.speed * (self.journal_radius**2))
             / (self.radial_clearance**3)
         )
 
-        PPlotYdim = (
-            PPlotY
+        PYdim = (
+            PY
             * (self.reference_viscosity * self.speed * (self.journal_radius**2))
             / (self.radial_clearance**3)
         )
 
-        hX = hX.flatten()
-        hY = hY.flatten()
+        PXPlot = np.zeros(
+            (self.elements_axial, self.elements_circumferential * self.n_pad)
+        ).astype(complex)
+        PYPlot = np.zeros(
+            (self.elements_axial, self.elements_circumferential * self.n_pad)
+        ).astype(complex)
 
-        aux_intXX = PPlotXdim * hX.T
+        for i in range(self.elements_axial):
+            PXPlot[i] = PXdim[i, :, :].ravel("F")
+            PYPlot[i] = PYdim[i, :, :].ravel("F")
 
-        aux_intXY = PPlotXdim * hY.T
+        Ytheta = np.array(Ytheta).flatten()
 
-        aux_intYX = PPlotYdim * hX.T
+        HX = HX.flatten()
+        HY = HY.flatten()
 
-        aux_intYY = PPlotYdim * hY.T
+        kxx = -np.real(
+            np.trapz(
+                np.trapz(PXPlot * HX, Ytheta * self.journal_radius),
+                self.Zdim[1 : self.elements_axial + 1],
+            )
+        )
 
-        H[0, 0] = -np.trapz(np.trapz(aux_intXX, Ytheta * self.journal_radius), Zdim)
+        kxy = -np.real(
+            np.trapz(
+                np.trapz(PYPlot * HX, Ytheta * self.journal_radius),
+                self.Zdim[1 : self.elements_axial + 1],
+            )
+        )
 
-        H[0, 1] = -np.trapz(np.trapz(aux_intXY, Ytheta * self.journal_radius), Zdim)
+        kyx = -np.real(
+            np.trapz(
+                np.trapz(PXPlot * HY, Ytheta * self.journal_radius),
+                self.Zdim[1 : self.elements_axial + 1],
+            )
+        )
 
-        H[1, 0] = -np.trapz(np.trapz(aux_intYX, Ytheta * self.journal_radius), Zdim)
+        kyy = -np.real(
+            np.trapz(
+                np.trapz(PYPlot * HY, Ytheta * self.journal_radius),
+                self.Zdim[1 : self.elements_axial + 1],
+            )
+        )
 
-        H[1, 1] = -np.trapz(np.trapz(aux_intYY, Ytheta * self.journal_radius), Zdim)
+        cxx = -np.imag(
+            np.trapz(
+                np.trapz(PXPlot * HX, Ytheta * self.journal_radius),
+                self.Zdim[1 : self.elements_axial + 1],
+            )
+        ) / (gamma * self.speed)
 
-        K = np.real(H)
-        C = np.imag(H) / wp
+        cxy = -np.imag(
+            np.trapz(
+                np.trapz(PYPlot * HX, Ytheta * self.journal_radius),
+                self.Zdim[1 : self.elements_axial + 1],
+            )
+        ) / (gamma * self.speed)
 
-        kxx = K[0, 0]
-        kxy = K[0, 1]
-        kyx = K[1, 0]
-        kyy = K[1, 1]
+        cyx = -np.imag(
+            np.trapz(
+                np.trapz(PXPlot * HY, Ytheta * self.journal_radius),
+                self.Zdim[1 : self.elements_axial + 1],
+            )
+        ) / (gamma * self.speed)
 
-        cxx = C[0, 0]
-        cxy = C[0, 1]
-        cyx = C[1, 0]
-        cyy = C[1, 1]
+        cyy = -np.imag(
+            np.trapz(
+                np.trapz(PYPlot * HY, Ytheta * self.journal_radius),
+                self.Zdim[1 : self.elements_axial + 1],
+            )
+        ) / (gamma * self.speed)
 
         return (kxx, kxy, kyx, kyy), (cxx, cxy, cyx, cyy)
 
     def _score(self, x, print_progress=False):
         """This method used to set the objective function of minimize optimization.
 
         Parameters
@@ -1853,14 +2673,15 @@
            resultant force provide by oil film.
 
         Returns
         -------
         Score coefficient.
 
         """
+
         Fhx, Fhy = self._forces(x, None, None, None)
         score = np.sqrt(
             ((self.load_x_direction + Fhx) ** 2) + ((self.load_y_direction + Fhy) ** 2)
         )
         if print_progress:
             print(f"Score: ", score)
             print("============================================")
@@ -1883,14 +2704,15 @@
             Force in y direction. The unit is newton.
 
         Returns
         -------
         Ss : float
             Sommerfeld number.
         """
+
         if self.sommerfeld_type == 1:
             S = (
                 self.reference_viscosity
                 * ((self.journal_radius) ** 3)
                 * self.axial_length
                 * self.speed
             ) / (
@@ -1924,33 +2746,34 @@
     --------
     >>> bearing = cylindrical_bearing_example()
     >>> bearing.axial_length
     0.263144
     """
 
     bearing = THDCylindrical(
-        axial_length=0.263144,
-        journal_radius=0.2,
-        radial_clearance=1.95e-4,
+        axial_length=(0.263144),
+        journal_radius=(0.2),
+        radial_clearance=(1.95e-4),
         elements_circumferential=11,
         elements_axial=3,
-        n_y=None,
         n_pad=2,
         pad_arc_length=176,
         reference_temperature=50,
-        reference_viscosity=0.02,
         speed=Q_([900], "RPM"),
         load_x_direction=0,
         load_y_direction=-112814.91,
         groove_factor=[0.52, 0.48],
         lubricant="ISOVG32",
         node=3,
         sommerfeld_type=2,
         initial_guess=[0.1, -0.1],
         method="perturbation",
+        operating_type="flooded",
+        injection_pressure=0,
+        oil_flow=37.86,
         show_coef=False,
         print_result=False,
         print_progress=False,
         print_time=False,
     )
 
     return bearing
```

### Comparing `ross-rotordynamics-1.3.0/ross/fluid_flow/fluid_flow.py` & `ross-rotordynamics-1.4.0/ross/fluid_flow/fluid_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,14 @@
         immediately_calculate_pressure_matrix_numerically=True,
         bearing_type=None,
         shape_geometry="cylindrical",
         preload=0.4,
         displacement=0,
         max_depth=None,
     ):
-
         self.nz = nz
         self.ntheta = ntheta
         self.n_interv_z = nz - 1
         self.n_interv_theta = ntheta - 1
         self.length = length
         self.ltheta = 2.0 * np.pi
         self.dz = length / self.n_interv_z
```

### Comparing `ross-rotordynamics-1.3.0/ross/fluid_flow/fluid_flow_coefficients.py` & `ross-rotordynamics-1.4.0/ross/fluid_flow/fluid_flow_coefficients.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.3.0/ross/fluid_flow/fluid_flow_geometry.py` & `ross-rotordynamics-1.4.0/ross/fluid_flow/fluid_flow_geometry.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.3.0/ross/fluid_flow/fluid_flow_graphics.py` & `ross-rotordynamics-1.4.0/ross/fluid_flow/fluid_flow_graphics.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.3.0/ross/materials.py` & `ross-rotordynamics-1.4.0/ross/materials.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,30 +27,33 @@
     already provided.
 
     Parameters
     ----------
     name : str
         Material name.
     rho : float, pint.Quantity
-        Density (N/m**3).
-    E : float, pint.Quantity
+        Density (kg/m**3).
+    E : float, pint.Quantity, optional
         Young's modulus (N/m**2).
-    G_s : float,
+    G_s : float, pint.Quantity, optional
         Shear modulus (N/m**2).
-    Poisson : float
+    Poisson : float, optional
         Poisson ratio (dimensionless).
-    color : str
+    color : str, optional
         Color that will be used on plots.
 
     Examples
     --------
+    >>> from ross.units import Q_
     >>> AISI4140 = Material(name="AISI4140", rho=7850, E=203.2e9, G_s=80e9)
-    >>> Steel = Material(name="Steel", rho=7810, E=211e9, G_s=81.2e9)
+    >>> Steel = Material(name="Steel", rho=Q_(7.81, 'g/cm**3'), E=211e9, G_s=81.2e9)
     >>> AISI4140.Poisson
     0.27
+    >>> Steel.rho
+    7809.999999999999
     """
 
     @check_units
     def __init__(
         self, name, rho, E=None, G_s=None, Poisson=None, color="#525252", **kwargs
     ):
         self.name = str(name)
```

### Comparing `ross-rotordynamics-1.3.0/ross/plotly_theme.py` & `ross-rotordynamics-1.4.0/ross/plotly_theme.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.3.0/ross/point_mass.py` & `ross-rotordynamics-1.4.0/ross/point_mass.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.3.0/ross/results.py` & `ross-rotordynamics-1.4.0/ross/results.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,17 +151,20 @@
             if key == "rotor":
                 aux_file = str(file)[:-5] + "_rotor" + str(file)[-5:]
                 from ross.rotor_assembly import Rotor
 
                 data[key] = Rotor.load(aux_file)
 
             elif isinstance(value, Iterable):
-                data[key] = np.array(value)
-                if data[key].dtype in str_type:
-                    data[key] = np.array(value).astype(np.complex128)
+                try:
+                    data[key] = np.array(value)
+                    if data[key].dtype in str_type:
+                        data[key] = np.array(value).astype(np.complex128)
+                except:
+                    data[key] = value
 
         return cls.read_toml_data(data)
 
 
 class Orbit(Results):
     r"""Class used to construct orbits for a node in a mode or deflected shape.
 
@@ -592,15 +595,14 @@
         orientation="major",
         title=None,
         length_units="m",
         phase_units="rad",
         fig=None,
         **kwargs,
     ):
-
         if fig is None:
             fig = go.Figure()
 
         xn = self.xn.copy()
         yn = self.yn.copy()
         zn = self.zn.copy()
 
@@ -1074,17 +1076,17 @@
         damping_name = "Log. Dec."
         damping_value = self.log_dec[mode]
         if damping_parameter == "damping_ratio":
             damping_name = "Damping ratio"
             damping_value = self.damping_ratio[mode]
 
         frequency = {
-            "wd": f"ω<sub>d</sub> = {Q_(self.wd[mode], 'rad/s').to(frequency_units).m:.1f}",
-            "wn": f"ω<sub>n</sub> = {Q_(self.wn[mode], 'rad/s').to(frequency_units).m:.1f}",
-            "speed": f"Speed = {Q_(self.speed, 'rad/s').to(frequency_units).m:.1f}",
+            "wd": f"ω<sub>d</sub> = {Q_(self.wd[mode], 'rad/s').to(frequency_units).m:.2f}",
+            "wn": f"ω<sub>n</sub> = {Q_(self.wn[mode], 'rad/s').to(frequency_units).m:.2f}",
+            "speed": f"Speed = {Q_(self.speed, 'rad/s').to(frequency_units).m:.2f}",
         }
 
         shape = self.shapes[mode]
         fig = shape.plot_3d(length_units=length_units, phase_units=phase_units, fig=fig)
 
         if title is None:
             title = ""
@@ -1108,15 +1110,15 @@
             title=dict(
                 text=(
                     f"{title}<br>"
                     f"Mode {mode} | "
                     f"{frequency['speed']} {frequency_units} | "
                     f"whirl: {self.whirl_direction()[mode]} | "
                     f"{frequency[frequency_type]} {frequency_units} | "
-                    f"{damping_name} = {damping_value:.1f}"
+                    f"{damping_name} = {damping_value:.2f}"
                 ),
                 x=0.5,
                 xanchor="center",
             ),
             **kwargs,
         )
 
@@ -1174,17 +1176,17 @@
             damping_name = "Damping ratio"
             damping_value = self.damping_ratio[mode]
 
         if fig is None:
             fig = go.Figure()
 
         frequency = {
-            "wd": f"ω<sub>d</sub> = {Q_(self.wd[mode], 'rad/s').to(frequency_units).m:.1f}",
-            "wn": f"ω<sub>n</sub> = {Q_(self.wn[mode], 'rad/s').to(frequency_units).m:.1f}",
-            "speed": f"Speed = {Q_(self.speed, 'rad/s').to(frequency_units).m:.1f}",
+            "wd": f"ω<sub>d</sub> = {Q_(self.wd[mode], 'rad/s').to(frequency_units).m:.2f}",
+            "wn": f"ω<sub>n</sub> = {Q_(self.wn[mode], 'rad/s').to(frequency_units).m:.2f}",
+            "speed": f"Speed = {Q_(self.speed, 'rad/s').to(frequency_units).m:.2f}",
         }
 
         shape = self.shapes[mode]
         fig = shape.plot_2d(fig=fig)
 
         if title is None:
             title = ""
@@ -1195,15 +1197,15 @@
             title=dict(
                 text=(
                     f"{title}<br>"
                     f"Mode {mode} | "
                     f"{frequency['speed']} {frequency_units} | "
                     f"whirl: {self.whirl_direction()[mode]} | "
                     f"{frequency[frequency_type]} {frequency_units} | "
-                    f"{damping_name} = {damping_value:.1f}"
+                    f"{damping_name} = {damping_value:.2f}"
                 ),
                 x=0.5,
                 xanchor="center",
             ),
             **kwargs,
         )
 
@@ -1578,37 +1580,34 @@
         fig=None,
         **mag_kwargs,
     ):
         """Plot frequency response (magnitude) using Plotly.
 
         This method plots the frequency response magnitude given an output and
         an input using Plotly.
-        It is possible to plot displacement, velocity and accelaration responses,
-        depending on the unit entered in 'amplitude_units'. If '[length]/[force]',
-        it displays the displacement; If '[speed]/[force]', it displays the velocity;
-        If '[acceleration]/[force]', it displays the acceleration.
+        It is possible to plot the magnitude with different units, depending on the unit entered in 'amplitude_units'. If '[length]/[force]', it displays the displacement unit (m); If '[speed]/[force]', it displays the velocity unit (m/s); If '[acceleration]/[force]', it displays the acceleration  unit (m/s**2).
 
         Parameters
         ----------
         inp : int
             Input.
         out : int
             Output.
         frequency_units : str, optional
             Units for the x axis.
             Default is "rad/s"
         amplitude_units : str, optional
             Units for the response magnitude.
             Acceptable units dimensionality are:
 
-            '[length]' - Displays the displacement;
+            '[length]' - Displays the magnitude with units (m/N);
 
-            '[speed]' - Displays the velocity;
+            '[speed]' - Displays the magnitude with units (m/s/N);
 
-            '[acceleration]' - Displays the acceleration.
+            '[acceleration]' - Displays the magnitude with units (m/s**2/N).
 
             Default is "m/N" 0 to peak.
             To use peak to peak use '<unit> pkpk' (e.g. 'm/N pkpk')
         fig : Plotly graph_objects.Figure()
             The figure object with the plot.
         mag_kwargs : optional
             Additional key word arguments can be passed to change the plot layout only
@@ -1624,26 +1623,24 @@
         idof = self.dof_dict[str(inp % self.number_dof)]
         outn = out // self.number_dof
         odof = self.dof_dict[str(out % self.number_dof)]
 
         frequency_range = Q_(self.speed_range, "rad/s").to(frequency_units).m
 
         dummy_var = Q_(1, amplitude_units)
+        y_label = "Magnitude"
         if dummy_var.check("[length]/[force]"):
             mag = np.abs(self.freq_resp)
             mag = Q_(mag, "m/N").to(amplitude_units).m
-            y_label = "Displacement"
         elif dummy_var.check("[speed]/[force]"):
             mag = np.abs(self.velc_resp)
             mag = Q_(mag, "m/s/N").to(amplitude_units).m
-            y_label = "Velocity"
         elif dummy_var.check("[acceleration]/[force]"):
             mag = np.abs(self.accl_resp)
             mag = Q_(mag, "m/s**2/N").to(amplitude_units).m
-            y_label = "Acceleration"
         else:
             raise ValueError(
                 "Not supported unit. Options are '[length]/[force]', '[speed]/[force]', '[acceleration]/[force]'"
             )
 
         if fig is None:
             fig = go.Figure()
@@ -1695,19 +1692,19 @@
         frequency_units : str, optional
             Units for the x axis.
             Default is "rad/s"
         amplitude_units : str, optional
             Units for the response magnitude.
             Acceptable units dimensionality are:
 
-            '[length]' - Displays the displacement;
+            '[length]' - Displays the magnitude with units (m/N);
 
-            '[speed]' - Displays the velocity;
+            '[speed]' - Displays the magnitude with units (m/s/N);
 
-            '[acceleration]' - Displays the acceleration.
+            '[acceleration]' - Displays the magnitude with units (m/s**2/N).
 
             Default is "m/N" 0 to peak.
             To use peak to peak use '<unit> pkpk' (e.g. 'm/N pkpk')
         phase_units : str, optional
             Units for the x axis.
             Default is "rad"
         fig : Plotly graph_objects.Figure()
@@ -1918,37 +1915,35 @@
         using Plotly.
 
         This method returns a subplot with:
             - Frequency vs Amplitude;
             - Frequency vs Phase Angle;
             - Polar plot Amplitude vs Phase Angle;
 
-        Amplitude can be displacement, velocity or accelaration responses,
-        depending on the unit entered in 'amplitude_units'. If '[length]/[force]',
-        it displays the displacement; If '[speed]/[force]', it displays the velocity;
-        If '[acceleration]/[force]', it displays the acceleration.
+        Amplitude magnitude unit can be displacement, velocity or accelaration responses,
+        depending on the unit entered in 'amplitude_units'. If '[length]/[force]', it displays the displacement unit (m); If '[speed]/[force]', it displays the velocity unit (m/s); If '[acceleration]/[force]', it displays the acceleration  unit (m/s**2).
 
         Parameters
         ----------
         inp : int
             Input.
         out : int
             Output.
         frequency_units : str, optional
             Units for the x axis.
             Default is "rad/s"
         amplitude_units : str, optional
             Units for the response magnitude.
             Acceptable units dimensionality are:
 
-            '[length]' - Displays the displacement;
+            '[length]' - Displays the magnitude with units (m/N);
 
-            '[speed]' - Displays the velocity;
+            '[speed]' - Displays the magnitude with units (m/s/N);
 
-            '[acceleration]' - Displays the acceleration.
+            '[acceleration]' - Displays the magnitude with units (m/s**2/N).
 
             Default is "m/N" 0 to peak.
             To use peak to peak use '<unit> pkpk' (e.g. 'm/N pkpk')
         phase_units : str, optional
             Units for the x axis.
             Default is "rad"
         mag_kwargs : optional
@@ -2711,15 +2706,14 @@
         dofx = ndof * node - fix_dof
         dofy = ndof * node + 1 - fix_dof
 
         # Relative angle between probes (90°)
         Rel_ang = np.exp(1j * np.pi / 2)
 
         for i, f in enumerate(self.speed_range):
-
             # Foward and Backward vectors
             fow = response[dofx, i] / 2 + Rel_ang * response[dofy, i] / 2
             back = (
                 np.conj(response[dofx, i]) / 2
                 + Rel_ang * np.conj(response[dofy, i]) / 2
             )
 
@@ -3453,15 +3447,14 @@
         w_shaft,
         disk_forces,
         bearing_forces,
         nodes,
         nodes_pos,
         Vx_axis,
     ):
-
         self.deformation = deformation
         self.Vx = Vx
         self.Bm = Bm
         self.w_shaft = w_shaft
         self.disk_forces = disk_forces
         self.bearing_forces = bearing_forces
         self.nodes = nodes
@@ -3595,15 +3588,15 @@
                 showlegend=False,
             ),
             row=row,
             col=col,
         )
 
         # fig - plot arrows indicating shaft weight distribution
-        text = "{:.1f}".format(Q_(self.w_shaft, "N").to(force_units).m)
+        text = "{:.2f}".format(Q_(self.w_shaft, "N").to(force_units).m)
         ini = nodes_pos[0]
         fin = nodes_pos[-1]
         arrows_list = np.arange(ini, 1.01 * fin, (fin - ini) / 5.0)
         for node in arrows_list:
             fig.add_annotation(
                 x=Q_(node, "m").to(rotor_length_units).m,
                 y=0,
```

### Comparing `ross-rotordynamics-1.3.0/ross/rotor_assembly.py` & `ross-rotordynamics-1.4.0/ross/rotor_assembly.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,14 @@
         bearing_elements=None,
         point_mass_elements=None,
         min_w=None,
         max_w=None,
         rated_w=None,
         tag=None,
     ):
-
         self.parameters = {"min_w": min_w, "max_w": max_w, "rated_w": rated_w}
         self.tag = "Rotor 0" if tag is None else tag
 
         ####################################################
         # Config attributes
         ####################################################
 
@@ -173,14 +172,17 @@
             point_mass_elements = []
 
         for i, disk in enumerate(disk_elements):
             if disk.tag is None:
                 disk.tag = "Disk " + str(i)
 
         for i, brg in enumerate(bearing_elements):
+            # add n_l and n_r to bearing elements
+            brg.n_l = brg.n
+            brg.n_r = brg.n
             if not isinstance(brg, SealElement) and brg.tag is None:
                 brg.tag = "Bearing " + str(i)
             elif isinstance(brg, SealElement) and brg.tag is None:
                 brg.tag = "Seal " + str(i)
 
         for i, p_mass in enumerate(point_mass_elements):
             if p_mass.tag is None:
@@ -963,15 +965,14 @@
                [     0.,    479.,      0.,    160.,      0.,      0.],
                [     0.,      0.,      0.,      0.,      0.,      0.]])
         """
 
         Kst0 = np.zeros((self.ndof, self.ndof))
 
         if self.number_dof == 6:
-
             for elm in self.shaft_elements:
                 dofs = list(elm.dof_global_index.values())
                 try:
                     Kst0[np.ix_(dofs, dofs)] += elm.Kst()
                 except TypeError:
                     Kst0[np.ix_(dofs, dofs)] += elm.Kst()
 
@@ -2882,20 +2883,20 @@
         vx = -vx
 
         # Calculate bending moment
         # Each line represents an element, each column a station from the element
         mx = np.zeros_like(vx)
         for j in range(mx.shape[0]):
             if j == 0:
-                mx[j] = [0, 0.5 * sum(vx[j]) * np.diff(vx_axis[j])]
+                mx[j] = [0, 0.5 * sum(vx[j]) * np.diff(vx_axis[j])[0]]
             if j == mx.shape[0] - 1:
-                mx[j] = [-0.5 * sum(vx[j]) * np.diff(vx_axis[j]), 0]
+                mx[j] = [-0.5 * sum(vx[j]) * np.diff(vx_axis[j])[0], 0]
             else:
                 mx[j, 0] = mx[j - 1, 1]
-                mx[j, 1] = mx[j, 0] + 0.5 * sum(vx[j]) * np.diff(vx_axis[j])
+                mx[j, 1] = mx[j, 0] + 0.5 * sum(vx[j]) * np.diff(vx_axis[j])[0]
 
         # flattening arrays
         vx = vx.flatten()
         vx_axis = vx_axis.flatten()
         mx = mx.flatten()
 
         self.disk_forces_nodal = disk_force_nodal
@@ -3139,16 +3140,16 @@
                 aux_DiskEl.n_l = nel_r * DiskEl.n_l
                 aux_DiskEl.n_r = nel_r * DiskEl.n_r
                 disk_elements.append(aux_DiskEl)
 
             for Brg_SealEl in brg_seal_data:
                 aux_Brg_SealEl = deepcopy(Brg_SealEl)
                 aux_Brg_SealEl.n = nel_r * Brg_SealEl.n
-                aux_Brg_SealEl.n_l = nel_r * Brg_SealEl.n_l
-                aux_Brg_SealEl.n_r = nel_r * Brg_SealEl.n_r
+                aux_Brg_SealEl.n_l = nel_r * Brg_SealEl.n
+                aux_Brg_SealEl.n_r = nel_r * Brg_SealEl.n
                 bearing_elements.append(aux_Brg_SealEl)
 
             regions.append(disk_elements)
             regions.append(bearing_elements)
 
             return regions
 
@@ -3257,15 +3258,14 @@
         bearing_elements=None,
         point_mass_elements=None,
         min_w=None,
         max_w=None,
         rated_w=None,
         tag=None,
     ):
-
         self.parameters = {"min_w": min_w, "max_w": max_w, "rated_w": rated_w}
         if tag is None:
             self.tag = "Rotor 0"
 
         ####################################################
         # Config attributes
         ####################################################
@@ -3303,14 +3303,16 @@
             point_mass_elements = []
 
         for i, disk in enumerate(disk_elements):
             if disk.tag is None:
                 disk.tag = "Disk " + str(i)
 
         for i, brg in enumerate(bearing_elements):
+            brg.n_l = brg.n
+            brg.n_r = brg.n
             if brg.__class__.__name__ == "BearingElement" and brg.tag is None:
                 brg.tag = "Bearing " + str(i)
             if brg.__class__.__name__ == "SealElement" and brg.tag is None:
                 brg.tag = "Seal " + str(i)
 
         for i, p_mass in enumerate(point_mass_elements):
             if p_mass.tag is None:
```

### Comparing `ross-rotordynamics-1.3.0/ross/shaft_element.py` & `ross-rotordynamics-1.4.0/ross/shaft_element.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,16 @@
 
         [x_0, y_0, \alpha_0, \beta_0, x_1, y_1, \alpha_1, \beta_1]^T
     Where :math:`\alpha_0` and :math:`\alpha_1` are the bending on the yz plane
     and :math:`\beta_0` and :math:`\beta_1` are the bending on the xz plane.
 
     Parameters
     ----------
-
+    L : float, pint.Quantity
+        Element length (m).
     idl : float, pint.Quantity
         Inner diameter of the element at the left position (m).
     odl : float, pint.Quantity
         Outer diameter of the element at the left position (m).
     idr : float, pint.Quantity, optional
         Inner diameter of the element at the right position (m).
         Default is equal to idl value (cylindrical element).
@@ -144,15 +145,14 @@
         torque=0,
         shear_effects=True,
         rotary_inertia=True,
         gyroscopic=True,
         shear_method_calc="cowper",
         tag=None,
     ):
-
         if idr is None:
             idr = idl
         if odr is None:
             odr = odl
 
         if material is None:
             raise AttributeError("Material is not defined.")
@@ -1317,15 +1317,14 @@
         shear_effects=True,
         rotary_inertia=True,
         gyroscopic=True,
         alpha=0,
         beta=0,
         tag=None,
     ):
-
         if idr is None:
             idr = idl
         if odr is None:
             odr = odl
 
         if material is None:
             raise AttributeError("Material is not defined.")
```

### Comparing `ross-rotordynamics-1.3.0/ross/stochastic/st_bearing_seal_element.py` & `ross-rotordynamics-1.4.0/ross/stochastic/st_bearing_seal_element.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,14 @@
         cyx=0,
         frequency=None,
         tag=None,
         n_link=None,
         scale_factor=1,
         is_random=None,
     ):
-
         if "frequency" in is_random:
             raise ValueError("frequency can not be a random variable")
 
         if kyy is None:
             kyy = kxx
             if "kxx" in is_random and "kyy" not in is_random:
                 is_random.append("kyy")
```

### Comparing `ross-rotordynamics-1.3.0/ross/stochastic/st_disk_element.py` & `ross-rotordynamics-1.4.0/ross/stochastic/st_disk_element.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.3.0/ross/stochastic/st_materials.py` & `ross-rotordynamics-1.4.0/ross/stochastic/st_materials.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.3.0/ross/stochastic/st_point_mass.py` & `ross-rotordynamics-1.4.0/ross/stochastic/st_point_mass.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.3.0/ross/stochastic/st_results.py` & `ross-rotordynamics-1.4.0/ross/stochastic/st_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1593,15 +1593,14 @@
         dofy = ndof * node + 1 - fix_dof
 
         # Relative angle between probes (90°)
         Rel_ang = np.exp(1j * np.pi / 2)
 
         for j in range(size):
             for i, f in enumerate(self.frequency_range):
-
                 # Foward and Backward vectors
                 fow = response[j, dofx, i] / 2 + Rel_ang * response[j, dofy, i] / 2
                 back = (
                     np.conj(response[j, dofx, i]) / 2
                     + Rel_ang * np.conj(response[j, dofy, i]) / 2
                 )
```

### Comparing `ross-rotordynamics-1.3.0/ross/stochastic/st_results_elements.py` & `ross-rotordynamics-1.4.0/ross/stochastic/st_results_elements.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.3.0/ross/stochastic/st_rotor_assembly.py` & `ross-rotordynamics-1.4.0/ross/stochastic/st_rotor_assembly.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.3.0/ross/stochastic/st_shaft_element.py` & `ross-rotordynamics-1.4.0/ross/stochastic/st_shaft_element.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,14 @@
         torque=0,
         shear_effects=True,
         rotary_inertia=True,
         gyroscopic=True,
         shear_method_calc="cowper",
         is_random=None,
     ):
-
         if idr is None:
             idr = idl
             if "idl" in is_random and "idr" not in is_random:
                 is_random.append("idr")
         if odr is None:
             odr = odl
             if "odl" in is_random and "odr" not in is_random:
```

### Comparing `ross-rotordynamics-1.3.0/ross/units.py` & `ross-rotordynamics-1.4.0/ross/units.py`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.3.0/ross/utils.py` & `ross-rotordynamics-1.4.0/ross/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -344,15 +344,15 @@
     >>> fig = rs.visualize_matrix(rotor, "K", frequency=100)
 
     Visualizing Gyroscopic Matrix:
     >>> fig = rs.visualize_matrix(rotor, "G")
     """
     A = np.zeros((rotor.ndof, rotor.ndof))
     # E will store element's names and contributions to the global matrix
-    E = np.zeros((rotor.ndof, rotor.ndof), dtype=np.object)
+    E = np.zeros((rotor.ndof, rotor.ndof), dtype=object)
 
     M, N = E.shape
     for i in range(M):
         for j in range(N):
             E[i, j] = []
 
     for elm in rotor.elements:
@@ -404,15 +404,15 @@
     y_axis = dof_string_list[::-1]
     fig = go.Figure()
     fig.add_trace(
         go.Heatmap(
             x=x_axis,
             y=y_axis,
             z=A[::-1],
-            customdata=np.array(data["elements"]).reshape(A.shape)[::-1],
+            customdata=np.array(data["elements"], dtype=object).reshape(A.shape)[::-1],
             coloraxis="coloraxis",
             hovertemplate=(
                 "<b>Value: %{z:.3e}<b><br>" + "<b>Elements:<b><br> %{customdata}"
             ),
             name="<b>Matrix {}</b>".format(matrix),
         )
     )
```

### Comparing `ross-rotordynamics-1.3.0/ross_rotordynamics.egg-info/SOURCES.txt` & `ross-rotordynamics-1.4.0/ross_rotordynamics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ross-rotordynamics-1.3.0/setup.py` & `ross-rotordynamics-1.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,18 +93,21 @@
     # entry_points={
     #     'console_scripts': ['mycli=mymodule:cli'],
     # },
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     package_data={"": ["new_units.txt"]},
     include_package_data=True,
-    license="MIT",
+    license="Apache License 2.0",
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
-        "License :: OSI Approved :: MIT License",
+        "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: Implementation :: CPython",
     ],
 )
```

