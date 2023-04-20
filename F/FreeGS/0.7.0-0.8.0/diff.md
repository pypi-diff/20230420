# Comparing `tmp/FreeGS-0.7.0.tar.gz` & `tmp/FreeGS-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeGS-0.7.0.tar", last modified: Mon Apr 17 16:12:39 2023, max compression
+gzip compressed data, was "FreeGS-0.8.0.tar", last modified: Thu Apr 20 15:26:07 2023, max compression
```

## Comparing `FreeGS-0.7.0.tar` & `FreeGS-0.8.0.tar`

### file list

```diff
@@ -1,56 +1,141 @@
-drwxr-xr-x   0 peter     (1000) users      (100)        0 2023-04-17 16:12:39.166091 FreeGS-0.7.0/
-drwxr-xr-x   0 peter     (1000) users      (100)        0 2023-04-17 16:12:39.162091 FreeGS-0.7.0/FreeGS.egg-info/
--rw-r--r--   0 peter     (1000) users      (100)     7552 2023-04-17 16:12:39.000000 FreeGS-0.7.0/FreeGS.egg-info/PKG-INFO
--rw-r--r--   0 peter     (1000) users      (100)     1081 2023-04-17 16:12:39.000000 FreeGS-0.7.0/FreeGS.egg-info/SOURCES.txt
--rw-r--r--   0 peter     (1000) users      (100)        1 2023-04-17 16:12:39.000000 FreeGS-0.7.0/FreeGS.egg-info/dependency_links.txt
--rw-r--r--   0 peter     (1000) users      (100)       52 2023-04-17 16:12:39.000000 FreeGS-0.7.0/FreeGS.egg-info/requires.txt
--rw-r--r--   0 peter     (1000) users      (100)        7 2023-04-17 16:12:39.000000 FreeGS-0.7.0/FreeGS.egg-info/top_level.txt
--rw-r--r--   0 peter     (1000) users      (100)     7651 2022-10-10 08:00:46.000000 FreeGS-0.7.0/LICENSE
--rw-r--r--   0 peter     (1000) users      (100)     7552 2023-04-17 16:12:39.166091 FreeGS-0.7.0/PKG-INFO
--rw-r--r--   0 peter     (1000) users      (100)     6739 2023-04-17 16:11:10.000000 FreeGS-0.7.0/README.md
-drwxr-xr-x   0 peter     (1000) users      (100)        0 2023-04-17 16:12:39.166091 FreeGS-0.7.0/freegs/
--rw-r--r--   0 peter     (1000) users      (100)     1073 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/__init__.py
--rw-r--r--   0 peter     (1000) users      (100)    12250 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/_aeqdsk.py
--rw-r--r--   0 peter     (1000) users      (100)     3218 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/_divgeo.py
--rw-r--r--   0 peter     (1000) users      (100)     3023 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/_fileutils.py
--rw-r--r--   0 peter     (1000) users      (100)     7807 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/_geqdsk.py
--rw-r--r--   0 peter     (1000) users      (100)      198 2023-03-17 16:15:33.000000 FreeGS-0.7.0/freegs/_version.py
--rw-r--r--   0 peter     (1000) users      (100)     6183 2022-10-10 08:00:46.000000 FreeGS-0.7.0/freegs/boundary.py
--rw-r--r--   0 peter     (1000) users      (100)     8386 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/coil.py
--rw-r--r--   0 peter     (1000) users      (100)     9985 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/control.py
--rw-r--r--   0 peter     (1000) users      (100)    16601 2022-10-10 08:00:46.000000 FreeGS-0.7.0/freegs/critical.py
--rw-r--r--   0 peter     (1000) users      (100)      287 2022-10-10 08:00:46.000000 FreeGS-0.7.0/freegs/divgeo.py
--rw-r--r--   0 peter     (1000) users      (100)     8858 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/dump.py
--rw-r--r--   0 peter     (1000) users      (100)    42373 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/equilibrium.py
--rw-r--r--   0 peter     (1000) users      (100)     7117 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/fieldtracer.py
--rw-r--r--   0 peter     (1000) users      (100)    10087 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/filament_coil.py
--rwxr-xr-x   0 peter     (1000) users      (100)    15345 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/geqdsk.py
--rw-r--r--   0 peter     (1000) users      (100)     8512 2022-10-10 08:00:46.000000 FreeGS-0.7.0/freegs/gradshafranov.py
--rw-r--r--   0 peter     (1000) users      (100)    15798 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/jtor.py
--rw-r--r--   0 peter     (1000) users      (100)    60565 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/machine.py
--rw-r--r--   0 peter     (1000) users      (100)    11049 2022-10-10 08:00:46.000000 FreeGS-0.7.0/freegs/multigrid.py
--rw-r--r--   0 peter     (1000) users      (100)     6443 2022-10-10 08:00:46.000000 FreeGS-0.7.0/freegs/optimise.py
--rw-r--r--   0 peter     (1000) users      (100)     5144 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/optimiser.py
--rw-r--r--   0 peter     (1000) users      (100)     7244 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/picard.py
--rw-r--r--   0 peter     (1000) users      (100)     3402 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/plotting.py
--rw-r--r--   0 peter     (1000) users      (100)     5126 2022-10-10 08:00:46.000000 FreeGS-0.7.0/freegs/polygons.py
--rw-r--r--   0 peter     (1000) users      (100)     7276 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/pre_calc_coil.py
--rw-r--r--   0 peter     (1000) users      (100)     3818 2022-10-10 08:00:46.000000 FreeGS-0.7.0/freegs/quadrature.py
--rw-r--r--   0 peter     (1000) users      (100)     7165 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/shaped_coil.py
--rw-r--r--   0 peter     (1000) users      (100)     2963 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/test_aeqdsk.py
--rw-r--r--   0 peter     (1000) users      (100)     2758 2022-10-10 08:00:46.000000 FreeGS-0.7.0/freegs/test_critical.py
--rw-r--r--   0 peter     (1000) users      (100)     1455 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/test_equilibrium.py
--rw-r--r--   0 peter     (1000) users      (100)      685 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/test_fileutils.py
--rw-r--r--   0 peter     (1000) users      (100)      996 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/test_geqdsk.py
--rw-r--r--   0 peter     (1000) users      (100)      918 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/test_jtor.py
--rw-r--r--   0 peter     (1000) users      (100)     1649 2022-10-10 08:00:46.000000 FreeGS-0.7.0/freegs/test_linearsolve.py
--rw-r--r--   0 peter     (1000) users      (100)     1940 2022-10-10 08:00:46.000000 FreeGS-0.7.0/freegs/test_machine.py
--rw-r--r--   0 peter     (1000) users      (100)     2755 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/test_multi_coil.py
--rw-r--r--   0 peter     (1000) users      (100)     1474 2022-10-10 08:00:46.000000 FreeGS-0.7.0/freegs/test_optimise.py
--rw-r--r--   0 peter     (1000) users      (100)     4036 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/test_optimiser.py
--rw-r--r--   0 peter     (1000) users      (100)     1574 2022-10-10 08:00:46.000000 FreeGS-0.7.0/freegs/test_polygons.py
--rw-r--r--   0 peter     (1000) users      (100)     1251 2022-10-10 08:00:46.000000 FreeGS-0.7.0/freegs/test_quadrature.py
--rw-r--r--   0 peter     (1000) users      (100)     1306 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/test_readwrite.py
--rw-r--r--   0 peter     (1000) users      (100)     1535 2022-10-10 08:00:46.000000 FreeGS-0.7.0/freegs/test_shaped_coil.py
--rw-r--r--   0 peter     (1000) users      (100)       38 2023-04-17 16:12:39.166091 FreeGS-0.7.0/setup.cfg
--rw-r--r--   0 peter     (1000) users      (100)     1242 2023-04-17 16:12:30.000000 FreeGS-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:26:07.559838 FreeGS-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:26:07.527838 FreeGS-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:26:07.535838 FreeGS-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-20 15:25:51.000000 FreeGS-0.8.0/.github/workflows/benchmark.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-20 15:25:51.000000 FreeGS-0.8.0/.github/workflows/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-20 15:25:51.000000 FreeGS-0.8.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-20 15:25:51.000000 FreeGS-0.8.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-20 15:25:51.000000 FreeGS-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-20 15:25:51.000000 FreeGS-0.8.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-04-20 15:25:51.000000 FreeGS-0.8.0/01-freeboundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-20 15:25:51.000000 FreeGS-0.8.0/02-read-geqdsk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-20 15:25:51.000000 FreeGS-0.8.0/03-mast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-20 15:25:51.000000 FreeGS-0.8.0/04-read-mast-geqdsk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-20 15:25:51.000000 FreeGS-0.8.0/05-fixed-boundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-20 15:25:51.000000 FreeGS-0.8.0/06-xpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-20 15:25:51.000000 FreeGS-0.8.0/07-increase-resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-20 15:25:51.000000 FreeGS-0.8.0/08-mast-upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-20 15:25:51.000000 FreeGS-0.8.0/09-metal-wall.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-20 15:25:51.000000 FreeGS-0.8.0/10-mastu-connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-20 15:25:51.000000 FreeGS-0.8.0/11-optimise-coils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-04-20 15:25:51.000000 FreeGS-0.8.0/12-limited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-20 15:25:51.000000 FreeGS-0.8.0/13-coil-limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-20 15:25:51.000000 FreeGS-0.8.0/14-read-geqdsk-constrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-20 15:25:51.000000 FreeGS-0.8.0/15-sensorMeasurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-20 15:25:51.000000 FreeGS-0.8.0/16-DIIID.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-20 15:25:51.000000 FreeGS-0.8.0/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:26:07.535838 FreeGS-0.8.0/FreeGS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-04-20 15:26:07.000000 FreeGS-0.8.0/FreeGS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-04-20 15:26:07.000000 FreeGS-0.8.0/FreeGS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:26:07.000000 FreeGS-0.8.0/FreeGS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-20 15:26:07.000000 FreeGS-0.8.0/FreeGS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 15:26:07.000000 FreeGS-0.8.0/FreeGS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-20 15:25:51.000000 FreeGS-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)   249217 2023-04-20 15:25:51.000000 FreeGS-0.8.0/MAST-example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-04-20 15:26:07.559838 FreeGS-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-04-20 15:25:51.000000 FreeGS-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:26:07.535838 FreeGS-0.8.0/asv_bench/
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-04-20 15:25:51.000000 FreeGS-0.8.0/asv_bench/asv.conf.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:26:07.535838 FreeGS-0.8.0/asv_bench/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:25:51.000000 FreeGS-0.8.0/asv_bench/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-20 15:25:51.000000 FreeGS-0.8.0/asv_bench/benchmarks/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:26:07.539838 FreeGS-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)   457418 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/RogMethod.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:26:07.547838 FreeGS-0.8.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.boundary.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.coil.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.control.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.critical.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.divgeo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.dump.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.equilibrium.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.fieldtracer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.filament_coil.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.geqdsk.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.gradshafranov.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.jtor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.machine.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.multi_coil.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.multigrid.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.optimise.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.optimiser.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.picard.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.plotting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.polygons.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.pre_calc_coil.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.quadrature.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.shaped_coil.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.test_critical.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.test_equilibrium.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.test_filament_coil.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.test_jtor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.test_linearsolve.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.test_machine.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.test_optimise.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.test_optimiser.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.test_polygons.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.test_quadrature.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.test_readwrite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.test_sensors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/freegs.test_shaped_coil.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21269 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/creating_equilibria.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/diagnostics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    70434 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/freegs_convergence.png
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/input_and_output.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    34253 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/nonlinear_solve.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/optimisation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   112830 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/optimiser.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-20 15:25:51.000000 FreeGS-0.8.0/docs/tests.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:26:07.559838 FreeGS-0.8.0/freegs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/_divgeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-20 15:26:07.000000 FreeGS-0.8.0/freegs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/boundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8669 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/coil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16595 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16601 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/critical.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/divgeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42651 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/equilibrium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/fieldtracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10957 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/filament_coil.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16196 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/geqdsk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/gradshafranov.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/jtor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72315 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8984 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/multi_coil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11049 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/multigrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/optimise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/optimiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/picard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/polygons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/pre_calc_coil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/quadrature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/shaped_coil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/test_critical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/test_equilibrium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/test_filament_coil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/test_jtor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/test_linearsolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/test_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/test_optimise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/test_optimiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/test_polygons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/test_quadrature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/test_readwrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9019 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-20 15:25:51.000000 FreeGS-0.8.0/freegs/test_shaped_coil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-20 15:25:51.000000 FreeGS-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-20 15:25:51.000000 FreeGS-0.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 15:26:07.559838 FreeGS-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 15:25:51.000000 FreeGS-0.8.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-20 15:25:51.000000 FreeGS-0.8.0/test-01-compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-20 15:25:51.000000 FreeGS-0.8.0/test-convergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21285 2023-04-20 15:25:51.000000 FreeGS-0.8.0/tutorial.ipynb
```

### Comparing `FreeGS-0.7.0/FreeGS.egg-info/PKG-INFO` & `FreeGS-0.8.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,34 @@
-Metadata-Version: 2.1
-Name: FreeGS
-Version: 0.7.0
-Summary: Free boundary Grad-Shafranov solver for tokamak plasma equilibria
-Home-page: https://github.com/bendudson/freegs
-Author: Ben Dudson
-Author-email: benjamin.dudson@york.ac.uk
-License: LGPL
-Platform: any
-Classifier: Programming Language :: Python
-Classifier: Development Status :: 3 - Alpha
-Classifier: Natural Language :: English
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Scientific/Engineering :: Physics
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 FreeGS: Free boundary Grad-Shafranov solver
 ===========================================
 
 [![License](https://img.shields.io/badge/license-GPL-blue.svg)](https://img.shields.io/badge/license-GPL-blue.svg)
 [![py3comp](https://img.shields.io/badge/py3-compatible-brightgreen.svg)](https://img.shields.io/badge/py3-compatible-brightgreen.svg)
-[![Build Status](https://github.com/bendudson/freegs/workflows/Tests/badge.svg)](https://github.com/bendudson/freegs/workflows/Tests/badge.svg)
-[![codecov](https://codecov.io/gh/bendudson/freegs/branch/master/graph/badge.svg?token=4dc6aHbu7K)](https://codecov.io/gh/bendudson/freegs)
+[![Build Status](https://github.com/freegs-plasma/freegs/workflows/Tests/badge.svg)](https://github.com/freegs-plasma/freegs/workflows/Tests/badge.svg)
+[![codecov](https://codecov.io/gh/freegs-plasma/freegs/branch/master/graph/badge.svg?token=4dc6aHbu7K)](https://codecov.io/gh/freegs-plasma/freegs)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/freegs-plasma/freegs/tutorial?labpath=tutorial.ipynb)
 
 This Python module calculates plasma equilibria for tokamak fusion experiments,
 by solving the Grad-Shafranov equation with free boundaries. Given a set of coils,
 plasma profiles and shape, FreeGS finds the currents in the coils which produce
 a steady-state solution in force balance.
 
 **Note** This is a work in progress, and probably contains bugs. 
 There is a feature wishlist in issues, suggestions and contributions welcome!
 
 Installing
 ----------
 
-A public vesion of FreeGS is available on PyPI 
+FreeGS is available on PyPI 
 
     $ pip install --user freegs
 
-or clone/download the internal TE version and run setup:
+or clone/download this repository and run setup:
 
-    $ git clone http://tokamak-devlin/gitlab/physics/freegs.git
+    $ git clone https://github.com/freegs-plasma/freegs.git
     $ cd freegs
     $ python setup.py install --user
 
 Documentation
 -------------
 
 The manual is in the `docs` subdirectory, and [hosted here on readthedocs](http://freegs.readthedocs.io/en/latest/).
@@ -62,25 +42,24 @@
 
 The tests are in the `src/` subdirectory.
 
 A convergence test is [described in the manual](https://freegs.readthedocs.io/en/latest/tests.html#convergence-test). To run:
 
     $ python test-convergence.py
 
-To-do list
-----------
-See the 'issues' board on the left hand toolbar.
-
 Examples
 --------
-(Note: some of these may no longer be working with changes to
-coil classes. Not exactly a priority to fix these at present.)
 
 The Jupyter notebooks contain examples wuth additional notes
 
+
+* [tutorial.ipynb](./tutorial.ipynb)
+
+Launch tutorial in [![MyBinder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/freegs-plasma/freegs/tutorial?labpath=tutorial.ipynb)
+
 * MAST-example.ipynb 
 
 There are also some Python scripts to run short tests
 and examples
 
     $ python 01-freeboundary.py
 
@@ -123,16 +102,14 @@
 * **gradshafranov.py**   - Greens functions and operators for the Grad-Shafranov equation
 * **jtor.py**            - Routines for calculating toroidal current density (profiles)
 * **machine.py**         - Represents the coils and power supply circuits
 * **multigrid.py**       - The multigrid solver for the linear elliptic operator
 * **picard.py**          - Nonlinear solver, iterating the profiles and constraints
 * **plotting.py**        - Plotting routines using matplotlib
 
-- more files have since been added! Check the repo.
-
 License
 -------
 
     Copyright 2016-2022 Ben Dudson, University of York, and other contributors.
     Email: benjamin.dudson@york.ac.uk
 
     This program is free software: you can redistribute it and/or modify
@@ -150,19 +127,25 @@
 
 References
 ----------
 
 * YoungMu Jeon, [Development of a free boundary Tokamak Equlibrium Solver](http://link.springer.com/article/10.3938/jkps.67.843)  [arXiv:1503.03135](https://arxiv.org/abs/1503.03135)
 * S.Jardin "Computational Methods in Plasma Physics" CRC Press
 
-Longer-term the intent is to move FreeGS development back to a public repo and to
-develop bespoke TE scripts in the eqtools python module.
 
-Public Versions
----------------
+Versions
+--------
+
+0.7.0  16th August 2022
+  - Fixes and additional features for equilibrium measurements
+  - Limited plasma detection and handling throughout code
+  - Optional adittional constraints on coil currents
+  - Constraints on coil currents when reading geqdsks
+  - Replacement of MultiCoil with FilamentCoil
+  - Addition of PreCalcCoil
 
 0.6.1  11th February 2021
   - Fixes for HDF5 reading and writing
   - Fix Numpy deprecations
   - Catch errors in optimisation measures, making that more robust
   - Fix core mask in geqdsk file reading
   - Flake8 fixes
@@ -196,9 +179,8 @@
   - Add 4th-order solver for potential
   - Add convergence test
 
 0.2.0  12th March 2019
   - Add field line tracer, `freegs.fieldtracer`
   - Add Equilibrium.Btor toroidal field calculation
   - Add Equilibrium.plasmaVolume
-  - Fix rlim, zlim saved into GEQDSK files
-
+  - Fix rlim, zlim saved into GEQDSK files
```

### Comparing `FreeGS-0.7.0/LICENSE` & `FreeGS-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FreeGS-0.7.0/PKG-INFO` & `FreeGS-0.8.0/FreeGS.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 Metadata-Version: 2.1
 Name: FreeGS
-Version: 0.7.0
+Version: 0.8.0
 Summary: Free boundary Grad-Shafranov solver for tokamak plasma equilibria
-Home-page: https://github.com/bendudson/freegs
-Author: Ben Dudson
-Author-email: benjamin.dudson@york.ac.uk
-License: LGPL
-Platform: any
+Author-email: Ben Dudson <benjamin.dudson@york.ac.uk>
+License: GNU Lesser General Public License v3 or later (LGPLv3+)
+Project-URL: project, https://github.com/freegs-plasma/freegs
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Physics
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: tests
+Provides-Extra: docs
 License-File: LICENSE
 
 FreeGS: Free boundary Grad-Shafranov solver
 ===========================================
 
 [![License](https://img.shields.io/badge/license-GPL-blue.svg)](https://img.shields.io/badge/license-GPL-blue.svg)
 [![py3comp](https://img.shields.io/badge/py3-compatible-brightgreen.svg)](https://img.shields.io/badge/py3-compatible-brightgreen.svg)
-[![Build Status](https://github.com/bendudson/freegs/workflows/Tests/badge.svg)](https://github.com/bendudson/freegs/workflows/Tests/badge.svg)
-[![codecov](https://codecov.io/gh/bendudson/freegs/branch/master/graph/badge.svg?token=4dc6aHbu7K)](https://codecov.io/gh/bendudson/freegs)
+[![Build Status](https://github.com/freegs-plasma/freegs/workflows/Tests/badge.svg)](https://github.com/freegs-plasma/freegs/workflows/Tests/badge.svg)
+[![codecov](https://codecov.io/gh/freegs-plasma/freegs/branch/master/graph/badge.svg?token=4dc6aHbu7K)](https://codecov.io/gh/freegs-plasma/freegs)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/freegs-plasma/freegs/tutorial?labpath=tutorial.ipynb)
 
 This Python module calculates plasma equilibria for tokamak fusion experiments,
 by solving the Grad-Shafranov equation with free boundaries. Given a set of coils,
 plasma profiles and shape, FreeGS finds the currents in the coils which produce
 a steady-state solution in force balance.
 
 **Note** This is a work in progress, and probably contains bugs. 
 There is a feature wishlist in issues, suggestions and contributions welcome!
 
 Installing
 ----------
 
-A public vesion of FreeGS is available on PyPI 
+FreeGS is available on PyPI 
 
     $ pip install --user freegs
 
-or clone/download the internal TE version and run setup:
+or clone/download this repository and run setup:
 
-    $ git clone http://tokamak-devlin/gitlab/physics/freegs.git
+    $ git clone https://github.com/freegs-plasma/freegs.git
     $ cd freegs
     $ python setup.py install --user
 
 Documentation
 -------------
 
 The manual is in the `docs` subdirectory, and [hosted here on readthedocs](http://freegs.readthedocs.io/en/latest/).
@@ -62,25 +64,24 @@
 
 The tests are in the `src/` subdirectory.
 
 A convergence test is [described in the manual](https://freegs.readthedocs.io/en/latest/tests.html#convergence-test). To run:
 
     $ python test-convergence.py
 
-To-do list
-----------
-See the 'issues' board on the left hand toolbar.
-
 Examples
 --------
-(Note: some of these may no longer be working with changes to
-coil classes. Not exactly a priority to fix these at present.)
 
 The Jupyter notebooks contain examples wuth additional notes
 
+
+* [tutorial.ipynb](./tutorial.ipynb)
+
+Launch tutorial in [![MyBinder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/freegs-plasma/freegs/tutorial?labpath=tutorial.ipynb)
+
 * MAST-example.ipynb 
 
 There are also some Python scripts to run short tests
 and examples
 
     $ python 01-freeboundary.py
 
@@ -123,16 +124,14 @@
 * **gradshafranov.py**   - Greens functions and operators for the Grad-Shafranov equation
 * **jtor.py**            - Routines for calculating toroidal current density (profiles)
 * **machine.py**         - Represents the coils and power supply circuits
 * **multigrid.py**       - The multigrid solver for the linear elliptic operator
 * **picard.py**          - Nonlinear solver, iterating the profiles and constraints
 * **plotting.py**        - Plotting routines using matplotlib
 
-- more files have since been added! Check the repo.
-
 License
 -------
 
     Copyright 2016-2022 Ben Dudson, University of York, and other contributors.
     Email: benjamin.dudson@york.ac.uk
 
     This program is free software: you can redistribute it and/or modify
@@ -150,19 +149,25 @@
 
 References
 ----------
 
 * YoungMu Jeon, [Development of a free boundary Tokamak Equlibrium Solver](http://link.springer.com/article/10.3938/jkps.67.843)  [arXiv:1503.03135](https://arxiv.org/abs/1503.03135)
 * S.Jardin "Computational Methods in Plasma Physics" CRC Press
 
-Longer-term the intent is to move FreeGS development back to a public repo and to
-develop bespoke TE scripts in the eqtools python module.
 
-Public Versions
----------------
+Versions
+--------
+
+0.7.0  16th August 2022
+  - Fixes and additional features for equilibrium measurements
+  - Limited plasma detection and handling throughout code
+  - Optional adittional constraints on coil currents
+  - Constraints on coil currents when reading geqdsks
+  - Replacement of MultiCoil with FilamentCoil
+  - Addition of PreCalcCoil
 
 0.6.1  11th February 2021
   - Fixes for HDF5 reading and writing
   - Fix Numpy deprecations
   - Catch errors in optimisation measures, making that more robust
   - Fix core mask in geqdsk file reading
   - Flake8 fixes
@@ -197,8 +202,7 @@
   - Add convergence test
 
 0.2.0  12th March 2019
   - Add field line tracer, `freegs.fieldtracer`
   - Add Equilibrium.Btor toroidal field calculation
   - Add Equilibrium.plasmaVolume
   - Fix rlim, zlim saved into GEQDSK files
-
```

### Comparing `FreeGS-0.7.0/README.md` & `FreeGS-0.8.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,56 @@
+Metadata-Version: 2.1
+Name: FreeGS
+Version: 0.8.0
+Summary: Free boundary Grad-Shafranov solver for tokamak plasma equilibria
+Author-email: Ben Dudson <benjamin.dudson@york.ac.uk>
+License: GNU Lesser General Public License v3 or later (LGPLv3+)
+Project-URL: project, https://github.com/freegs-plasma/freegs
+Classifier: Programming Language :: Python
+Classifier: Development Status :: 3 - Alpha
+Classifier: Natural Language :: English
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Scientific/Engineering :: Physics
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: tests
+Provides-Extra: docs
+License-File: LICENSE
+
 FreeGS: Free boundary Grad-Shafranov solver
 ===========================================
 
 [![License](https://img.shields.io/badge/license-GPL-blue.svg)](https://img.shields.io/badge/license-GPL-blue.svg)
 [![py3comp](https://img.shields.io/badge/py3-compatible-brightgreen.svg)](https://img.shields.io/badge/py3-compatible-brightgreen.svg)
-[![Build Status](https://github.com/bendudson/freegs/workflows/Tests/badge.svg)](https://github.com/bendudson/freegs/workflows/Tests/badge.svg)
-[![codecov](https://codecov.io/gh/bendudson/freegs/branch/master/graph/badge.svg?token=4dc6aHbu7K)](https://codecov.io/gh/bendudson/freegs)
+[![Build Status](https://github.com/freegs-plasma/freegs/workflows/Tests/badge.svg)](https://github.com/freegs-plasma/freegs/workflows/Tests/badge.svg)
+[![codecov](https://codecov.io/gh/freegs-plasma/freegs/branch/master/graph/badge.svg?token=4dc6aHbu7K)](https://codecov.io/gh/freegs-plasma/freegs)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/freegs-plasma/freegs/tutorial?labpath=tutorial.ipynb)
 
 This Python module calculates plasma equilibria for tokamak fusion experiments,
 by solving the Grad-Shafranov equation with free boundaries. Given a set of coils,
 plasma profiles and shape, FreeGS finds the currents in the coils which produce
 a steady-state solution in force balance.
 
 **Note** This is a work in progress, and probably contains bugs. 
 There is a feature wishlist in issues, suggestions and contributions welcome!
 
 Installing
 ----------
 
-A public vesion of FreeGS is available on PyPI 
+FreeGS is available on PyPI 
 
     $ pip install --user freegs
 
-or clone/download the internal TE version and run setup:
+or clone/download this repository and run setup:
 
-    $ git clone http://tokamak-devlin/gitlab/physics/freegs.git
+    $ git clone https://github.com/freegs-plasma/freegs.git
     $ cd freegs
     $ python setup.py install --user
 
 Documentation
 -------------
 
 The manual is in the `docs` subdirectory, and [hosted here on readthedocs](http://freegs.readthedocs.io/en/latest/).
@@ -41,25 +64,24 @@
 
 The tests are in the `src/` subdirectory.
 
 A convergence test is [described in the manual](https://freegs.readthedocs.io/en/latest/tests.html#convergence-test). To run:
 
     $ python test-convergence.py
 
-To-do list
-----------
-See the 'issues' board on the left hand toolbar.
-
 Examples
 --------
-(Note: some of these may no longer be working with changes to
-coil classes. Not exactly a priority to fix these at present.)
 
 The Jupyter notebooks contain examples wuth additional notes
 
+
+* [tutorial.ipynb](./tutorial.ipynb)
+
+Launch tutorial in [![MyBinder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/freegs-plasma/freegs/tutorial?labpath=tutorial.ipynb)
+
 * MAST-example.ipynb 
 
 There are also some Python scripts to run short tests
 and examples
 
     $ python 01-freeboundary.py
 
@@ -102,16 +124,14 @@
 * **gradshafranov.py**   - Greens functions and operators for the Grad-Shafranov equation
 * **jtor.py**            - Routines for calculating toroidal current density (profiles)
 * **machine.py**         - Represents the coils and power supply circuits
 * **multigrid.py**       - The multigrid solver for the linear elliptic operator
 * **picard.py**          - Nonlinear solver, iterating the profiles and constraints
 * **plotting.py**        - Plotting routines using matplotlib
 
-- more files have since been added! Check the repo.
-
 License
 -------
 
     Copyright 2016-2022 Ben Dudson, University of York, and other contributors.
     Email: benjamin.dudson@york.ac.uk
 
     This program is free software: you can redistribute it and/or modify
@@ -129,19 +149,25 @@
 
 References
 ----------
 
 * YoungMu Jeon, [Development of a free boundary Tokamak Equlibrium Solver](http://link.springer.com/article/10.3938/jkps.67.843)  [arXiv:1503.03135](https://arxiv.org/abs/1503.03135)
 * S.Jardin "Computational Methods in Plasma Physics" CRC Press
 
-Longer-term the intent is to move FreeGS development back to a public repo and to
-develop bespoke TE scripts in the eqtools python module.
 
-Public Versions
----------------
+Versions
+--------
+
+0.7.0  16th August 2022
+  - Fixes and additional features for equilibrium measurements
+  - Limited plasma detection and handling throughout code
+  - Optional adittional constraints on coil currents
+  - Constraints on coil currents when reading geqdsks
+  - Replacement of MultiCoil with FilamentCoil
+  - Addition of PreCalcCoil
 
 0.6.1  11th February 2021
   - Fixes for HDF5 reading and writing
   - Fix Numpy deprecations
   - Catch errors in optimisation measures, making that more robust
   - Fix core mask in geqdsk file reading
   - Flake8 fixes
@@ -176,8 +202,7 @@
   - Add convergence test
 
 0.2.0  12th March 2019
   - Add field line tracer, `freegs.fieldtracer`
   - Add Equilibrium.Btor toroidal field calculation
   - Add Equilibrium.plasmaVolume
   - Fix rlim, zlim saved into GEQDSK files
-
```

### Comparing `FreeGS-0.7.0/freegs/__init__.py` & `FreeGS-0.8.0/freegs/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,22 +25,26 @@
 GNU Lesser General Public License for more details.
 
 You should have received a copy of the GNU Lesser General Public License
 along with FreeGS.  If not, see <http://www.gnu.org/licenses/>.
 
 """
 
-__version__ = "0.7.0"
+from importlib_metadata import metadata
 
 from .equilibrium import Equilibrium
 
 from . import jtor
 
 from . import machine
 
 from . import control
 
 from .picard import solve
 
 from .dump import OutputFile
 
 from . import plotting
+
+
+__version__ = metadata(__package__)["Version"]
+__author__ = metadata(__package__)["Author"]
```

### Comparing `FreeGS-0.7.0/freegs/_divgeo.py` & `FreeGS-0.8.0/freegs/_divgeo.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 You should have received a copy of the GNU Lesser General Public License
 along with FreeGS.  If not, see <http://www.gnu.org/licenses/>.
 
 """
 import numpy as np
 
-from ._fileutils import ChunkOutput, write_1d, write_2d
+from freeqdsk._fileutils import ChunkOutput, write_1d, write_2d
 
 
 def write(data, fh, label=None):
     """
     Write a DivGeo file, given a dictionary of data
 
     data - dictionary
```

### Comparing `FreeGS-0.7.0/freegs/boundary.py` & `FreeGS-0.8.0/freegs/boundary.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.7.0/freegs/coil.py` & `FreeGS-0.8.0/freegs/coil.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Poloidal field coil
 
 Used in machine to define coils. Can also be a base class for other coil types.
 
 License
 -------
 
-Copyright 2016-2019 Ben Dudson, University of York. Email: benjamin.dudson@york.ac.uk
+Copyright 2016-2022 FreeGS contributors
 
 This file is part of FreeGS.
 
 FreeGS is free software: you can redistribute it and/or modify
 it under the terms of the GNU Lesser General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -23,14 +23,16 @@
 You should have received a copy of the GNU Lesser General Public License
 along with FreeGS.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 from .gradshafranov import Greens, GreensBr, GreensBz, mu0
 import numpy as np
 import numbers
+from shapely.geometry import Point
+import warnings
 
 
 class AreaCurrentLimit:
     """
     Calculate the coil area based on a fixed current density limit
     """
 
@@ -56,15 +58,15 @@
     """
     Represents a poloidal field coil
 
     public members
     --------------
 
     R, Z - Location of the coil
-    current - current in the coil in Amps
+    current - current in each turn of the coil in Amps
     turns   - Number of turns
     control - enable or disable control system
     area    - Cross-section area in m^2
 
     The total toroidal current carried by the coil is current * turns
     """
 
@@ -164,15 +166,15 @@
         """
         Calculate forces on the coils in Newtons
 
         Returns an array of two elements: [ Fr, Fz ]
 
 
         Force on coil due to its own current:
-            Lorentz self‐forces on curved current loops
+            Lorentz self-forces on curved current loops
             Physics of Plasmas 1, 3425 (1998); https://doi.org/10.1063/1.870491
             David A. Garren and James Chen
         """
         current = self.current  # current per turn
         total_current = current * self.turns  # Total toroidal current
 
         # Calculate field at this coil due to all other coils
@@ -201,14 +203,20 @@
             [
                 (total_current * Bz + self_fr)
                 * Ltor,  # Jphi x Bz = Fr, self force always outwards
                 -total_current * Br * Ltor,
             ]
         )  # Jphi x Br = - Fz
 
+    def inShape(self, polygon):
+        if polygon.contains(Point(self.R, self.Z)):
+            return 1
+        else:
+            return 0
+
     def __repr__(self):
         return "Coil(R={0}, Z={1}, current={2:.1f}, turns={3}, control={4})".format(
             self.R, self.Z, self.current, self.turns, self.control
         )
 
     def __eq__(self, other):
         return (
@@ -242,19 +250,21 @@
 
     @property
     def area(self):
         """
         The cross-section area of the coil in m^2
         """
         if isinstance(self._area, numbers.Number):
-            assert self._area > 0
+            if not self._area > 0:
+                warnings.warn(f"Coil area {self._area:3.2f} <= 0")
             return self._area
         # Calculate using functor
         area = self._area(self)
-        assert area > 0
+        if not area > 0:
+            warnings.warn(f"Coil area {area:3.2f} <= 0")
         return area
 
     @area.setter
     def area(self, area):
         self._area = area
 
     def plot(self, axis=None, show=False):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `FreeGS-0.7.0/freegs/critical.py` & `FreeGS-0.8.0/freegs/critical.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.7.0/freegs/dump.py` & `FreeGS-0.8.0/freegs/dump.py`

 * *Files 8% similar despite different names*

```diff
@@ -141,16 +141,16 @@
 
         equilibrium_group.create_dataset("current", data=equilibrium.plasmaCurrent())
         equilibrium_group["current"].attrs["title"] = "Plasma current [Amps]"
 
         psi_id = equilibrium_group.create_dataset("psi", data=equilibrium.psi())
         psi_id.dims[0].label = "R"
         psi_id.dims[1].label = "Z"
-        psi_id.dims.create_scale(equilibrium_group["R_1D"], "R")
-        psi_id.dims.create_scale(equilibrium_group["Z_1D"], "Z")
+        equilibrium_group["R_1D"].make_scale("R")
+        equilibrium_group["Z_1D"].make_scale("Z")
         psi_id.dims[0].attach_scale(equilibrium_group["R_1D"])
         psi_id.dims[1].attach_scale(equilibrium_group["Z_1D"])
 
         plasma_psi_id = equilibrium_group.create_dataset(
             "plasma_psi", data=equilibrium.plasma_psi
         )
         plasma_psi_id.dims[0].label = "R"
```

### Comparing `FreeGS-0.7.0/freegs/equilibrium.py` & `FreeGS-0.8.0/freegs/equilibrium.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,16 @@
         Zmin=-1.0,
         Zmax=1.0,
         nx=65,
         ny=65,
         boundary=freeBoundary,
         psi=None,
         current=0.0,
-        order=4
+        order=4,
+        check_limited=False,
     ):
         """Initialises a plasma equilibrium
 
         Rmin, Rmax  - Range of major radius R [m]
         Zmin, Zmax  - Range of height Z [m]
 
         nx - Resolution in R. This must be 2^n + 1
@@ -90,20 +91,25 @@
 
         self._applyBoundary = boundary
 
         self.Rmin = Rmin
         self.Rmax = Rmax
         self.Zmin = Zmin
         self.Zmax = Zmax
+        self.nx = nx
+        self.ny = ny
 
         self.R_1D = linspace(Rmin, Rmax, nx)
         self.Z_1D = linspace(Zmin, Zmax, ny)
         self.R, self.Z = meshgrid(self.R_1D, self.Z_1D, indexing="ij")
 
-        self.check_limited = False
+        self.dR = self.R[1, 0] - self.R[0, 0]
+        self.dZ = self.Z[0, 1] - self.Z[0, 0]
+
+        self.check_limited = check_limited
         self.is_limited = False
         self.Rlim = None
         self.Zlim = None
 
         if psi is None:
             # Starting guess for psi
             xx, yy = meshgrid(linspace(0, 1, nx), linspace(0, 1, ny), indexing="ij")
@@ -115,14 +121,15 @@
             psi[:, -1] = 0.0
 
         # Calculate coil Greens functions. This is an optimisation,
         # used in self.psi() to speed up calculations
         self._pgreen = tokamak.createPsiGreens(self.R, self.Z)
 
         self._current = current  # Plasma current
+        self.Jtor = None
 
         self._updatePlasmaPsi(psi)  # Needs to be after _pgreen
 
         # Create the solver
         if order == 2:
             generator = GSsparse(Rmin, Rmax, Zmin, Zmax)
         elif order == 4:
@@ -240,17 +247,17 @@
         """
         return self.plasmaBz(R, Z) + self.tokamak.Bz(R, Z)
 
     def Bpol(self, R, Z):
         """
         Total poloidal magnetic field
         """
-        Br = self.Br(R,Z)
-        Bz = self.Bz(R,Z)
-        return np.sqrt(Br*Br + Bz*Bz)
+        Br = self.Br(R, Z)
+        Bz = self.Bz(R, Z)
+        return np.sqrt(Br * Br + Bz * Bz)
 
     def Btor(self, R, Z):
         """
         Toroidal magnetic field
         """
         # Normalised psi
         psi_norm = (self.psiRZ(R, Z) - self.psi_axis) / (self.psi_bndry - self.psi_axis)
@@ -266,18 +273,18 @@
 
         return fpol / R
 
     def Btot(self, R, Z):
         """
         Total magnetic field
         """
-        Br = self.Br(R,Z)
-        Bz = self.Bz(R,Z)
-        Btor = self. Btor(R,Z)
-        return np.sqrt(Br*Br + Bz*Bz + Btor*Btor)       
+        Br = self.Br(R, Z)
+        Bz = self.Bz(R, Z)
+        Btor = self.Btor(R, Z)
+        return np.sqrt(Br * Br + Bz * Bz + Btor * Btor)
 
     def psi(self):
         """
         Total poloidal flux (psi), including contribution from
         plasma and external coils.
         """
         # return self.plasma_psi + self.tokamak.psi(self.R, self.Z)
@@ -338,54 +345,54 @@
             # An array which doesn't include psinorm = 0 or 1
             psinorm = linspace(1.0 / (npsi + 1), 1.0, npsi, endpoint=False)
             return psinorm, critical.find_safety(self, psinorm=psinorm)
 
         result = critical.find_safety(self, psinorm=psinorm)
         # Convert to a scalar if only one result
         if len(result) == 1:
-            return np.asscalar(result)
+            return result[0]
         return result
 
-    def tor_flux(self, psi = None):
+    def tor_flux(self, psi=None):
         """
         Calculates toroidal flux at specified values of poloidal flux.
         >>> q = drho/dpsi
         """
         psiN = (psi - self.psi_axis) / (self.psi_bndry - self.psi_axis)
         # Get safety factor of these flux surfaces
         qvals = self.q(psiN)
 
         # Integrate q wrt psi to get rho. rho = 0 @ psiN = 0
-        result = cumtrapz(qvals,psi,initial=0.0)*(-1./(2.*np.pi))
+        result = cumtrapz(qvals, psi, initial=0.0) * (-1.0 / (2.0 * np.pi))
 
         # Convert to a scalar if only one result
         if len(result) == 1:
-            return np.asscalar(result)
+            return result[0]
         return result
 
-    def rhotor(self, psi = None):
+    def rhotor(self, psi=None):
         """
         Calculates normalised toroidal flux at specified values of
         poloidal flux.
          >>> rhotor = sqrt ( tor_flux/max(tor_flux)).
-        
+
         Maximum toroidal flux shoud be at LCFS.
         """
 
         torflux = self.tor_flux(psi)
 
-        psi = np.linspace(self.psi_axis,self.psi_bndry,101,endpoint=True)
+        psi = np.linspace(self.psi_axis, self.psi_bndry, 101, endpoint=True)
         torflux_for_LCFS = self.tor_flux(psi)
 
         max_torflux = np.max(torflux_for_LCFS)
 
-        result = np.sqrt(torflux/max_torflux)
+        result = np.sqrt(torflux / max_torflux)
 
         if len(result) == 1:
-            return np.asscalar(result)
+            return result[0]
         return result
 
     def pprime(self, psinorm):
         """
         Return p' at given normalised psi
         """
         return self._profiles.pprime(psinorm)
@@ -462,16 +469,17 @@
 
         self._updatePlasmaPsi(plasma_psi)
 
         # Update plasma current
         dR = self.R[1, 0] - self.R[0, 0]
         dZ = self.Z[0, 1] - self.Z[0, 0]
         self._current = romb(romb(Jtor)) * dR * dZ
+        self.Jtor = Jtor
 
-    def _updateBoundaryPsi(self,psi=None):
+    def _updateBoundaryPsi(self, psi=None):
         """
         For an input psi the magnetic axis and boundary psi are identified along
         with the core mask.
 
         Various logical checks occur, depending on whether or not the user
         wishes to check if the plasma is limited or not, as well as whether
         or not any xpoints are present.
@@ -481,102 +489,101 @@
             psi = self.psi()
 
         opt, xpt = critical.find_critical(self.R, self.Z, psi)
 
         psi = psi
 
         if opt:
-        # Magnetic axis flux taken as primary o-point flux
+            # Magnetic axis flux taken as primary o-point flux
             self.psi_axis = opt[0][2]
-
-            '''
+            """
             Several options depending on if user wishes to check
             if the plasma becomes limited.
-            '''
+            """
 
             # The user wishes to check if the plasma is limited
-            if(self.check_limited and self.tokamak.wall):
-
+            if self.check_limited and self.tokamak.wall:
                 # A wall has actually been provided, proceed with checking
 
                 # Obtain flux on machine limit points
                 Rlimit = self.tokamak.limit_points_R
                 Zlimit = self.tokamak.limit_points_Z
 
-                '''
+                """
                 If an xpoint is present (plasma is potentianlly diverted)
                 then we must remove any limit points above/below the
                 primary xpoint as the PFR may land on these points,
                 which would break the algorithm (at present) for extracting the boundary
                 flux if the plasma were to infact be limited. There is a more advanced
                 version of this alogorithm that is more robust that will be
                 added in the future.
-                '''
+                """
 
                 if xpt:
-                    limit_args = np.ravel(np.argwhere(abs(Zlimit)<abs(0.75*xpt[0][1])))
+                    limit_args = np.ravel(
+                        np.argwhere(abs(Zlimit) < abs(0.75 * xpt[0][1]))
+                    )
                     Rlimit = Rlimit[limit_args]
                     Zlimit = Zlimit[limit_args]
 
                 # Obtain the flux psi at these limiter points
                 R = np.asarray(self.R[:, 0])
                 Z = np.asarray(self.Z[0, :])
 
                 # psi is transposed due to how FreeGS meshgrids R,Z
-                psi_2d = interpolate.interp2d(x=R,y=Z,z=psi.T)
-                
+                psi_2d = interpolate.interp2d(x=R, y=Z, z=psi.T)
+
                 # Get psi at the limit points
                 psi_limit_points = np.zeros(len(Rlimit))
                 for i in range(len(Rlimit)):
-                    psi_limit_points[i] = psi_2d(Rlimit[i],Zlimit[i])[0]
+                    psi_limit_points[i] = psi_2d(Rlimit[i], Zlimit[i])[0]
 
                 # Get index of maximum psi value
                 indMax = np.argmax(psi_limit_points)
-                
+
                 # Extract R,Z of the contact point
                 self.Rlim = Rlimit[indMax]
                 self.Zlim = Zlimit[indMax]
 
                 # Obtain maximum psi
                 self.psi_limit = psi_limit_points[indMax]
 
                 # Check if any xpoints are present
                 if xpt:
-
                     # Get flux from the primary xpoint
                     self.psi_xpt = xpt[0][2]
 
                     # Choose between diverted or limited flux
-                    self.psi_bndry = max(self.psi_xpt,self.psi_limit)
+                    self.psi_bndry = max(self.psi_xpt, self.psi_limit)
 
                     if self.psi_bndry == self.psi_limit:
                         self.is_limited = True
 
                     else:
                         self.is_limited = False
 
                     # Mask the core
-                    self.mask = critical.core_mask(self.R, self.Z, psi, opt, xpt, self.psi_bndry)
+                    self.mask = critical.core_mask(
+                        self.R, self.Z, psi, opt, xpt, self.psi_bndry
+                    )
 
                     # Use interpolation to find if a point is in the core.
                     self.mask_func = interpolate.RectBivariateSpline(
                         self.R[:, 0], self.Z[0, :], self.mask
                     )
 
                 else:
-
                     # No xpoints, therefore psi_bndry = psi_limit
                     self.psi_bndry = self.psi_limit
                     self.is_limited = True
                     self.mask = None
 
             else:
                 # Either a wall was not provided or the user did not wish to
                 # check if the plasma was limited
-
                 if xpt:
                     self.psi_xpt = xpt[0][2]
                     self.psi_bndry = self.psi_xpt
                     self.mask = critical.core_mask(self.R, self.Z, psi, opt, xpt)
 
                     # Use interpolation to find if a point is in the core.
                     self.mask_func = interpolate.RectBivariateSpline(
@@ -737,58 +744,56 @@
 
         R0 = R(P3) + 0.5*(R(P1)-R(P3))
         z0 = 0.5*(Z(P1)+Z(P3))
         """
 
         # Get points along the LCFS
         separatrix = self.separatrix(npoints=npoints)  # Array [:,2]
-        
+
         Rlcfs = np.array([i[0] for i in separatrix])
         Zlcfs = np.array([i[1] for i in separatrix])
 
         ind_P1 = np.argmax(Rlcfs)
         ind_P3 = np.argmin(Rlcfs)
 
-        P1 = np.array([Rlcfs[ind_P1],Zlcfs[ind_P1]])
-        P3 = np.array([Rlcfs[ind_P3],Zlcfs[ind_P3]])
+        P1 = np.array([Rlcfs[ind_P1], Zlcfs[ind_P1]])
+        P3 = np.array([Rlcfs[ind_P3], Zlcfs[ind_P3]])
 
-        R0 = P3[0] + 0.5*(P1[0]-P3[0])
-        z0 = 0.5*(P1[1]+P3[1])
+        R0 = P3[0] + 0.5 * (P1[0] - P3[0])
+        z0 = 0.5 * (P1[1] + P3[1])
 
-        C = np.array([R0,z0])
+        C = np.array([R0, z0])
 
         return C
 
     def Rgeometric(self, npoints=360):
-        """Locates major radius R of the geometric major radius.
-        """
+        """Locates major radius R of the geometric major radius."""
         return self.geometricAxis(npoints=npoints)[0]
 
     def Zgeometric(self, npoints=360):
-        """Locates the height z of the geometric axis.
-        """
+        """Locates the height z of the geometric axis."""
         return self.geometricAxis(npoints=npoints)[1]
 
     def minorRadius(self, npoints=360):
         """Calculates minor radius of the plasma, a. First locates the
         extrema points in R of the LCFS, wherein P3 is at the IMP and
         P1 is at the OMP.
 
         a = 0.5*(R(P1) - R(P3))
         """
 
         # Get points along the LCFS
         separatrix = self.separatrix(npoints=npoints)  # Array [:,2]
-        
+
         Rlcfs = np.array([i[0] for i in separatrix])
 
         R_P1 = np.max(Rlcfs)
         R_P3 = np.min(Rlcfs)
 
-        return 0.5*(R_P1 - R_P3)
+        return 0.5 * (R_P1 - R_P3)
 
     def aspectRatio(self, npoints=360):
         """Calculates the plasma aspect ratio.
 
         A = R0/a where R0 = major radius, a = minor radius.
         """
         return self.Rgeometric(npoints=npoints) / self.minorRadius(npoints=npoints)
@@ -810,67 +815,67 @@
         at the lower extent of the plasma.
 
         kappa = (Z(P2) - Z(P4))/a
         """
 
         # Get points along the LCFS
         separatrix = self.separatrix(npoints=npoints)  # Array [:,2]
-        
+
         Zlcfs = np.array([i[1] for i in separatrix])
 
         Z_P2 = np.max(Zlcfs)
         Z_P4 = np.min(Zlcfs)
 
         a = self.minorRadius(npoints=npoints)
 
-        return 0.5*(Z_P2 - Z_P4)/a
+        return 0.5 * (Z_P2 - Z_P4) / a
 
     def elongationUpper(self, npoints=360):
         """Calculates the upper elongation, kappa_u, of the plasma. A large number
         of points should be supplied such that any primary xpoint(s) on
         the LCFS are captured. The R,Z of the primary x-point is NOT
         itself included in the R,Z of the LCFS as the plasma may be limited.
         P2 is the point at the upper extent of the plasma.
 
         kappa_u = (Z(P2) - z0)/a
         """
 
         # Get points along the LCFS
         separatrix = self.separatrix(npoints=npoints)  # Array [:,2]
-        
+
         Zlcfs = np.array([i[1] for i in separatrix])
 
         Z_P2 = np.max(Zlcfs)
 
         z0 = self.Zgeometric(npoints=npoints)
         a = self.minorRadius(npoints=npoints)
 
-        return (Z_P2 - z0)/a
+        return (Z_P2 - z0) / a
 
     def elongationLower(self, npoints=360):
         """Calculates the lower elongation, kappa_l, of the plasma. A large number
         of points should be supplied such that any primary xpoint(s) on
         the LCFS are captured. The R,Z of the primary x-point is NOT
         itself included in the R,Z of the LCFS as the plasma may be limited.
         P2 is the point at the upper extent of the plasma.
 
         kappa_u = (z0 - Z(P4))/a
         """
 
         # Get points along the LCFS
         separatrix = self.separatrix(npoints=npoints)  # Array [:,2]
-        
+
         Zlcfs = np.array([i[1] for i in separatrix])
 
         Z_P4 = np.min(Zlcfs)
 
         z0 = self.Zgeometric(npoints=npoints)
         a = self.minorRadius(npoints=npoints)
 
-        return (z0 - Z_P4)/a
+        return (z0 - Z_P4) / a
 
     def effectiveElongation(self, npoints=360):
         """Calculates plasma effective elongation using the plasma volume"""
         return self.plasmaVolume() / (
             2.0
             * np.pi
             * self.Rgeometric(npoints=npoints)
@@ -893,15 +898,15 @@
         ind_P2 = np.argmax(Zlcfs)
 
         R_P2 = Rlcfs[ind_P2]
 
         R0 = self.Rgeometric(npoints=npoints)
         a = self.minorRadius(npoints=npoints)
 
-        return (R0 - R_P2)/a
+        return (R0 - R_P2) / a
 
     def triangularityLower(self, npoints=360):
         """Calculates plasma upper triangularity, delta_u.
         P4 is the point at the lower extent of the plasma.
 
         tri_l = (R0 - R(P4))/a
         """
@@ -914,27 +919,27 @@
         ind_P2 = np.argmax(Zlcfs)
 
         R_P2 = Rlcfs[ind_P2]
 
         R0 = self.Rgeometric(npoints=npoints)
         a = self.minorRadius(npoints=npoints)
 
-        return (R0 - R_P2)/a
+        return (R0 - R_P2) / a
 
     def triangularity(self, npoints=360):
         """Calculates plasma triangularity, delta.
 
         Here delta is defined as the average of the upper
         and lower triangularities.
         """
 
         tri_u = self.triangularityUpper(npoints=npoints)
         tri_l = self.triangularityLower(npoints=npoints)
 
-        return 0.5*(tri_u + tri_l)
+        return 0.5 * (tri_u + tri_l)
 
     def shafranovShift(self, npoints=360):
         """Calculates the plasma shafranov shift
         [delta_shafR,delta_shafZ] where
 
         delta_shafR = Rmagnetic - Rgeo
         delta_shafR = Zmagnetic - z0
@@ -942,15 +947,15 @@
 
         Rmag = self.Rmagnetic()
         Zmag = self.Zmagnetic()
 
         Rgeo = self.Rgeometric()
         z0 = self.Zgeometric()
 
-        return np.array([Rmag-Rgeo,Zmag-z0])
+        return np.array([Rmag - Rgeo, Zmag - z0])
 
     def internalInductance1(self, npoints=360):
         """Calculates li1 plasma internal inductance"""
 
         R = self.R
         Z = self.Z
         # Produce array of Bpol^2 in (R,Z)
@@ -1033,16 +1038,16 @@
         if self.mask is not None:  # Only include points in the core
             dV *= self.mask
 
         Ip = self.plasmaCurrent()
         R_geo = self.Rgeometric(npoints=npoints)
 
         integral = romb(romb(B_polvals_2 * dV))
-        return 2 * integral / (mu0*mu0*R_geo*Ip*Ip)
-        
+        return 2 * integral / (mu0 * mu0 * R_geo * Ip * Ip)
+
     def poloidalBeta(self):
         """Calculate plasma poloidal beta by integrating the thermal pressure
         and poloidal magnetic field pressure over the plasma volume."""
 
         R = self.R
         Z = self.Z
 
@@ -1063,15 +1068,15 @@
             dV *= self.mask
 
         pressure_integral = romb(romb(pressure * dV))
         field_integral_pol = romb(romb(B_polvals_2 * dV))
         return 2 * mu0 * pressure_integral / field_integral_pol
 
     def poloidalBeta2(self):
-        """ Return the poloidal beta
+        """Return the poloidal beta
         betap = (8pi/mu0) * int(p)dRdZ / Ip^2
         """
 
         dR = self.R[1, 0] - self.R[0, 0]
         dZ = self.Z[0, 1] - self.Z[0, 0]
 
         # Normalised psi
@@ -1089,38 +1094,37 @@
             * romb(romb(pressure))
             * dR
             * dZ
             / (self.plasmaCurrent() ** 2)
         )
 
     def poloidalBeta3(self):
-        """Calculates alterantive poloidal beta definition.
-        """
+        """Calculates alterantive poloidal beta definition."""
 
         R = self.R
         Z = self.Z
 
-        dR = R[1,0] - R[0,0]
-        dZ = Z[0,1] - Z[0,0]
-        dV = 2.*np.pi * R * dR * dZ
-        
+        dR = R[1, 0] - R[0, 0]
+        dZ = Z[0, 1] - Z[0, 0]
+        dV = 2.0 * np.pi * R * dR * dZ
+
         # Normalised psi
-        psi_norm = (self.psi() - self.psi_axis)  / (self.psi_bndry - self.psi_axis)
+        psi_norm = (self.psi() - self.psi_axis) / (self.psi_bndry - self.psi_axis)
 
         # Plasma pressure
         pressure = self.pressure(psi_norm)
-        
-        if self.mask is not None: # Only include points in the core
+
+        if self.mask is not None:  # Only include points in the core
             dV *= self.mask
 
         pressure_integral = romb(romb(pressure * dV))
         Ip = self.plasmaCurrent()
         vol = self.plasmaVolume()
         r0 = self.Rgeometric()
-        return 4 * vol * pressure_integral / (mu0 * Ip * Ip * r0 )
+        return 4 * vol * pressure_integral / (mu0 * Ip * Ip * r0)
 
     def toroidalBeta(self):
         """Calculate plasma toroidal beta by integrating the thermal pressure
         and toroidal magnetic field pressure over the plasma volume."""
 
         R = self.R
         Z = self.Z
@@ -1152,20 +1156,24 @@
     def totalBeta(self):
         """Calculate plasma total beta"""
         return 1.0 / ((1.0 / self.poloidalBeta()) + (1.0 / self.toroidalBeta()))
 
     def betaN(self, npoints=360):
         """Calculate normalised plasma beta"""
         geo = self.geometricAxis()
-        Bt = self.Btor(geo[0],geo[1])
-        return 100.0*1.0e+06*self.toroidalBeta()*( (self.minorRadius()*Bt) / (self.plasmaCurrent()) )
+        Bt = self.Btor(geo[0], geo[1])
+        return (
+            100.0
+            * 1.0e06
+            * self.toroidalBeta()
+            * ((self.minorRadius() * Bt) / (self.plasmaCurrent()))
+        )
 
     def pressure_ave(self):
-        """Calculate average pressure, Pa.
-        """
+        """Calculate average pressure, Pa."""
 
         R = self.R
         Z = self.Z
 
         # Produce array of Btor in (R,Z)
         B_torvals_2 = self.Btor(R, Z) ** 2
 
@@ -1179,58 +1187,58 @@
         # Plasma pressure
         pressure = self.pressure(psi_norm)
 
         if self.mask is not None:  # Only include points in the core
             dV *= self.mask
 
         pressure_integral = romb(romb(pressure * dV))
-        plasmaVolume      = romb(romb(dV))
+        plasmaVolume = romb(romb(dV))
 
-        return pressure_integral/plasmaVolume
+        return pressure_integral / plasmaVolume
 
     def w_th(self):
         """
         Stored thermal energy in plasma, J.
         """
 
         R = self.R
         Z = self.Z
 
-        dR = R[1,0] - R[0,0]
-        dZ = Z[0,1] - Z[0,0]
-        dV = 2.*np.pi * R * dR * dZ
-        
+        dR = R[1, 0] - R[0, 0]
+        dZ = Z[0, 1] - Z[0, 0]
+        dV = 2.0 * np.pi * R * dR * dZ
+
         # Normalised psi
-        psi_norm = (self.psi() - self.psi_axis)  / (self.psi_bndry - self.psi_axis)
-        
+        psi_norm = (self.psi() - self.psi_axis) / (self.psi_bndry - self.psi_axis)
+
         # Plasma pressure
         pressure = self.pressure(psi_norm)
 
-        if self.mask is not None: # Only include points in the core
+        if self.mask is not None:  # Only include points in the core
             dV *= self.mask
 
         pressure_integral = romb(romb(pressure * dV))
-        thermal_energy = (3./2.)*pressure_integral
+        thermal_energy = (3.0 / 2.0) * pressure_integral
 
         return thermal_energy
 
     def qcyl(self):
         """
         Cylindrical safety factor.
         """
 
         eps = self.inverseAspectRatio()
         a = self.minorRadius()
 
-        btor = self.fvac()/self.Rgeometric()
+        btor = self.fvac() / self.Rgeometric()
         Ip = self.plasmaCurrent()
 
         kappa = self.elongation()
 
-        val = 0.5 * (1 + kappa * kappa) * ((2. * np.pi * a * eps * btor) / (mu0 * Ip))
+        val = 0.5 * (1 + kappa * kappa) * ((2.0 * np.pi * a * eps * btor) / (mu0 * Ip))
 
         return val
 
 
 def refine(eq, nx=None, ny=None):
     """
     Double grid resolution, returning a new equilibrium
```

### Comparing `FreeGS-0.7.0/freegs/fieldtracer.py` & `FreeGS-0.8.0/freegs/fieldtracer.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
     ft = FieldTracer(eq)
 
     # Find the edge of the plasma
     psi = eq.psi()
     opoint, xpoint = critical.find_critical(eq.R, eq.Z, psi)
 
     r0, z0, psi_axis = opoint[0]
-    psi_bndry = eq.psi_bndry #xpoint[0][2]
+    psi_bndry = eq.psi_bndry
 
     # Find outboard midplane
     psifunc = interpolate.RectBivariateSpline(
         eq.R[:, 0], eq.Z[0, :], (psi - psi_axis) / (psi_bndry - psi_axis)
     )
 
     rmid, zmid = critical.find_psisurface(
```

### Comparing `FreeGS-0.7.0/freegs/filament_coil.py` & `FreeGS-0.8.0/freegs/filament_coil.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,152 +24,157 @@
 
 import numpy as np
 from . import polygons
 from shapely import geometry
 from .coil import Coil, AreaCurrentLimit
 from .gradshafranov import Greens, GreensBr, GreensBz
 
-def populate_with_fils(shape,Nfils):
+
+def populate_with_fils(shape, Nfils):
     """
     Takes the 2D cross section of a PF coil, via shape, and populates it
     (somewhat) uniformally with ~Nfils point sources representing filaments.
     """
 
     Rshape = np.array([i[0] for i in shape])
     Zshape = np.array([i[1] for i in shape])
-    Rshape = np.append(Rshape,Rshape[0])
-    Zshape = np.append(Zshape,Zshape[0])
+    Rshape = np.append(Rshape, Rshape[0])
+    Zshape = np.append(Zshape, Zshape[0])
     rmin = np.min(Rshape)
     rmax = np.max(Rshape)
     zmin = np.min(Zshape)
     zmax = np.max(Zshape)
 
     my_polygon = geometry.Polygon(shape)
 
-    '''
+    """
     How this works: Start by roughly estimating the d = dR, dZ spacing
     between the points, using the shape area and Nfils.
-    '''
+    """
 
     A = abs(polygons.area(shape))
-    d = np.sqrt(A/Nfils)
+    d = np.sqrt(A / Nfils)
 
-    '''
+    """
     Now we create a (staggered) grid across the bounding box containing
     the supplied shape. We then scan through each point on the grid and
     check if it lies inside the shape. We count the number of points that
     lie inside the shape. If this is less than Nfils, increase the grid
     resolution a little until eventually the number of points inside the grid
     => Nfils. Once this is obtained, linearly interpolate in dR,dZ to better
     estimate the d(=dR,dZ) that will give as close to Nfils points inside the shape
     as possible.
-    '''
+    """
 
     # Track d vs nInside
     d_data = []
     nInside_data = []
-    
+
     nInside = 0
 
     while nInside < Nfils:
 
         nInside = 0
-        i = 0 # Row counter used for staggering every other row
+        i = 0  # Row counter used for staggering every other row
         # Create the (non-staggered) grid points for the given d(=dR,dZ)
-        Rgrid = np.arange(rmin,rmax,d,dtype=float)
-        Zgrid = np.arange(zmin,zmax,d,dtype=float)
+        Rgrid = np.arange(rmin, rmax, d, dtype=float)
+        Zgrid = np.arange(zmin, zmax, d, dtype=float)
 
         nR = len(Rgrid)
         nZ = len(Zgrid)
 
         for i in range(nZ):
 
             zpoint = Zgrid[i]
-            
-            if i % 2: # Every other row, stagger R coords by 0.5*dR
-                offset = 0.5*d
+
+            if i % 2:  # Every other row, stagger R coords by 0.5*dR
+                offset = 0.5 * d
             else:
 
                 offset = 0.0
 
             for j in range(nR):
-                
+
                 rpoint = Rgrid[j] + offset
 
-                point = geometry.Point(rpoint,zpoint)
+                point = geometry.Point(rpoint, zpoint)
                 if my_polygon.contains(point):
                     nInside += 1
-    
+
         # End of looping over points. Note d and nInside
         d_data.append(d)
         nInside_data.append(nInside)
 
         # Shrink spacing by 0.5%
         d *= 0.995
 
     # Finished and have got nInside >= Nfils
     d_data = np.asarray(d_data)
     nInside = np.asarray(nInside_data)
 
     # Now linearly interpolate to get the d that corresponds
     # to the closest nInside to Nfils
-    d_opt = np.interp([Nfils*1.1],nInside_data,d_data)
+    d_opt = np.interp([Nfils * 1.1], nInside_data, d_data)
 
     # Now get the locations of the filaments for this d = d_opt where nInside ~ Nfils
     rfils = []
     zfils = []
 
     # Number of filaments landing inside
     nInside = 0
 
-    i = 0 # Row counter used for staggering every other row
+    i = 0  # Row counter used for staggering every other row
     # Create the (non-staggered) grid points for the given d(=dR,dZ)
-    Rgrid = np.arange(rmin,rmax,d_opt,dtype=float)
-    Zgrid = np.arange(zmin,zmax,d_opt,dtype=float)
+    Rgrid = np.arange(rmin, rmax, d_opt, dtype=float)
+    Zgrid = np.arange(zmin, zmax, d_opt, dtype=float)
 
     nR = len(Rgrid)
     nZ = len(Zgrid)
 
     for i in range(nZ):
 
         zpoint = Zgrid[i]
-        
-        if i % 2: # Every other row, stagger R coords by 0.5*dR
-            offset = 0.5*d_opt
+
+        if i % 2:  # Every other row, stagger R coords by 0.5*dR
+            offset = 0.5 * d_opt
         else:
 
             offset = 0.0
 
         for j in range(nR):
-            
+
             rpoint = Rgrid[j] + offset
 
-            point = geometry.Point(rpoint,zpoint)
+            point = geometry.Point(rpoint, zpoint)
 
             if my_polygon.contains(point):
                 nInside += 1
                 rfils.append(rpoint)
                 zfils.append(zpoint)
 
     rfils = np.asarray(rfils)
     zfils = np.asarray(zfils)
 
     return rfils, zfils
-                    
+
+
 class FilamentCoil(Coil):
     """
     This class represents a coil broken down into multiple
     filaments, with each filament acting as a point source
     of current.
 
+    Note: Filaments are wired in parallel, so a the current
+    through a single turn is shared between the filaments.
+
     public members
     --------------
 
     R, Z    - Location of the coil
-    current - current in the coil in Amps
+    current - current in each turn of the coil in Amps
     turns   - Number of turns
     control - enable or disable control system
     area    - Cross-section area in m^2
 
     The total toroidal current carried by the coil is current * turns
     """
 
@@ -178,46 +183,63 @@
         [
             (str("RZlen"), int),  # Length of R and Z arrays
             (str("R"), "500f8"),  # Up to 100 points
             (str("Z"), "500f8"),
             (str("current"), np.float64),
             (str("turns"), int),
             (str("control"), bool),
-            (str("npoints"), int)
+            (str("npoints"), int),
         ]
     )
 
-    def __init__(self, Rfil=None, Zfil=None, shape=None, current=0.0, Nfils=50, turns=1, control=True):
+    def __init__(
+        self,
+        Rfil=None,
+        Zfil=None,
+        shape=None,
+        current=0.0,
+        Nfils=50,
+        turns=1,
+        control=True,
+    ):
         """
         Inputs
         ------
         shape   - Outline of the coil shape as a list of points [(r1,z1), (r2,z2), ...]
                   Must have more than two points. If not provided, plotting the coil
         may not be entirely accurate.
 
         Rfil, Zfil - Locations of coil filaments (lists/arrays). This is optional.
         If these are not provided then the filaments themselves are populated
         automatically across the cross-section of the coil.
 
         current - current in each turn of the coil in Amps
         Nfils   - Number of filaments. Only used when Rfil is None.
         turns   - Number of turns in point coil(s) block. Total block current is current * turns
-                  This is only used if R,Z are a single point
         control - enable or disable control system.
 
+        Note: The number of filaments does not equal the number of turns; each turn
+        of the coil might consist of multiple filaments.
+
         """
 
         if shape is None:
-
-            minR = min(Rfil)
-            maxR = max(Rfil)
-            minZ = min(Zfil)
-            maxZ = max(Zfil)
-
-            shape = [(minR,minZ),(minR,maxZ),(maxR,maxZ),(maxR,minZ),(minR,minZ)]
+            # Note: NumPy min/max works with float where builtin doesn't
+            minR = np.min(Rfil)
+            maxR = np.max(Rfil)
+            minZ = np.min(Zfil)
+            maxZ = np.max(Zfil)
+
+            shape = [
+                (minR, minZ),
+                (minR, maxZ),
+                (maxR, maxZ),
+                (maxR, minZ),
+                (minR, minZ),
+            ]
 
         assert len(shape) > 2
 
         # Find the geometric middle of the coil
         # The R,Z properties have accessor functions to handle modifications
         self._R_centre = sum(r for r, z in shape) / len(shape)
         self._Z_centre = sum(z for r, z in shape) / len(shape)
@@ -227,111 +249,123 @@
         self.control = control
         self._area = abs(polygons.area(shape))
         self.shape = shape
 
         if Rfil is None:
             # No filaments provided. Need to populate the coil cross
             # section with -Nfils filaments.
+            Rfil, Zfil = populate_with_fils(self.shape, Nfils)
 
-            Rfil, Zfil = populate_with_fils(self.shape,Nfils)
-        
         Rfil = np.asarray(Rfil)
         Zfil = np.asarray(Zfil)
-        self.points = np.array(list(zip(Rfil,Zfil)))
-
-        self.npoints = len(Rfil)
+        if Rfil.ndim == 0:
+            self.points = [(Rfil, Zfil)]
+            self.npoints = 1
+        else:
+            self.points = np.array(list(zip(Rfil, Zfil)))
+            self.npoints = len(Rfil)
 
     def controlPsi(self, R, Z):
         """
         Calculate poloidal flux at (R,Z) due to a unit current
+
+        Note: This is multiplied by current to get coil Psi
         """
         result = 0.0
         for R_fil, Z_fil in self.points:
             result += Greens(R_fil, Z_fil, R, Z)
-        result = result / float(self.npoints)
+        result = result * self.turns / float(self.npoints)
         return result
 
     def controlBr(self, R, Z):
         """
         Calculate radial magnetic field Br at (R,Z) due to a unit current
         """
         result = 0.0
         for R_fil, Z_fil in self.points:
             result += GreensBr(R_fil, Z_fil, R, Z)
-        result = result / float(self.npoints)
+        result = result * self.turns / float(self.npoints)
         return result
 
     def controlBz(self, R, Z):
         """
         Calculate axial magnetic field Br at (R,Z) due to a unit current
         """
         result = 0.0
         for R_fil, Z_fil in self.points:
             result += GreensBz(R_fil, Z_fil, R, Z)
-        result = result / float(self.npoints)
+        result = result * self.turns / float(self.npoints)
         return result
 
+    def inShape(self,polygon):
+        counter = 0
+        for r, z in self.points:
+            if polygon.contains(geometry.Point(r, z)):
+                counter += 1 / self.npoints
+        return counter
+
     def __repr__(self):
-        return ("FilamentCoil({0}, current={1:.1f}, turns={2}, control={3})"
-                .format(self.points, self.current, self.turns, self.control))
+        return "FilamentCoil({0}, current={1:.1f}, turns={2}, control={3})".format(
+            self.points, self.current, self.turns, self.control
+        )
 
     @property
     def R(self):
         """
         Major radius of the coil in m
         """
-        return self._R
+        return self._R_centre
 
     @R.setter
     def R(self, Rnew):
         # Need to shift all points
-        Rshift = Rnew - self._R
-        self.points = [(r + Rshift, z) for r,z in self.points]
-        self._R = Rnew
+        Rshift = Rnew - self._R_centre
+        self.points = [(r + Rshift, z) for r, z in self.points]
+        self._R_centre = Rnew
 
     @property
     def Z(self):
         """
         Height of the coil in m
         """
-        return self._Z
+        return self._Z_centre
 
     @Z.setter
     def Z(self, Znew):
         # Need to shift all points
-        Zshift = Znew - self._Z
-        self.points = [(r, z + Zshift) for r,z in self.points]
-        self._Z = Znew
+        Zshift = Znew - self._Z_centre
+        self.points = [(r, z + Zshift) for r, z in self.points]
+        self._Z_centre = Znew
 
     @property
     def area(self):
         return self._area
-        
+
     @area.setter
     def area(self, area):
         raise ValueError("Area of a FilamentCoil is fixed")
 
     def plot(self, axis=None, show=False):
         """
         Plot the coil points, using axis if given
         """
         import matplotlib.pyplot as plt
-        
+
         if axis is None:
             fig = plt.figure()
             axis = fig.add_subplot(111)
 
         r = [r for r, z in self.shape]
         z = [z for r, z in self.shape]
         axis.fill(r, z, color="gray")
         axis.plot(r, z, color="black")
 
-        r = [r for r,z in self.points]
-        z = [z for r,z in self.points]
-        axis.plot(r,z,'kx')
-        
+        r = [r for r, z in self.points]
+        z = [z for r, z in self.points]
+        axis.plot(r, z, "kx")
+
         # Quadrature points
-        #rquad = [r for r,z,w in self._points]
-        #zquad = [z for r,z,w in self._points]
-        #axis.plot(rquad, zquad, 'ro')
-        
+        # rquad = [r for r,z,w in self._points]
+        # zquad = [z for r,z,w in self._points]
+        # axis.plot(rquad, zquad, 'ro')
+
         return axis
```

### Comparing `FreeGS-0.7.0/freegs/geqdsk.py` & `FreeGS-0.8.0/freegs/geqdsk.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,38 +19,39 @@
 GNU Lesser General Public License for more details.
 
 You should have received a copy of the GNU Lesser General Public License
 along with FreeGS.  If not, see <http://www.gnu.org/licenses/>.
 
 """
 
-from . import _geqdsk
 from . import critical
 from .equilibrium import Equilibrium
 from .machine import Wall
 from . import jtor
 from . import control
 from . import picard
 from .gradshafranov import mu0
 
+
+from freeqdsk import geqdsk
 from scipy import interpolate
 from numpy import (
     linspace,
     reshape,
     ravel,
     zeros,
     clip,
 )
 import math
 import numpy as np
 
 from scipy.integrate import romb
 
 
-def write(eq, fh, label=None, oxpoints=None, fileformat=_geqdsk.write):
+def write(eq, fh, label=None, oxpoints=None, fileformat=geqdsk.write):
     """
     Write a GEQDSK equilibrium file, given a FreeGS Equilibrium object
 
     eq - Equilibrium object
     fh - file handle
 
     label - Text label to put in the file
@@ -160,14 +161,15 @@
     axis=None,
     pause=0.0001,
     cocos=1,
     domain=None,
     blend=0.0,
     fit_sol=False,
     maxits=50,
+    current_bounds=None,
 ):
     """
     Reads a G-EQDSK format file
 
     fh : File handle
     machine : Machine object defining coil locations
     rtol : float
@@ -199,14 +201,18 @@
         This is particularly for reading SCENE input, which is not valid
         outside the separatrix.
         If True, the whole domain is used in the fitting.
         This is useful if the locations of strike points need to be constrained.
     maxits : integer
         Maximum number of iterations. Set to None for no limit.
         If this limit is exceeded then a RuntimeError is raised.
+    current_bounds: List of tuples
+        Optional list of tuples representing constraints on coil currents to be used
+        when reconstructing the equilibrium from the geqdsk file.
+        [(l1,u1),(l2,u2)...(lN,uN)]
 
     A nonlinear solve will be performed, using Picard iteration
 
     Returns
     -------
 
     An Equilibrium object eq. In addition, the following is available:
@@ -222,15 +228,15 @@
     if fit_sol and domain:
         raise ValueError("Sorry, fit_sol cannot be used with the domain keyword")
 
     if axis is not None:
         show = True
 
     # Read the data as a Dictionary
-    data = _geqdsk.read(fh, cocos=cocos)
+    data = geqdsk.read(fh, cocos=cocos)
 
     # If data contains a limiter, set the machine wall
     if "rlim" in data:
         if len(data["rlim"]) > 3:
             machine.wall = Wall(data["rlim"], data["zlim"])
         else:
             print("Fewer than 3 points given for limiter/wall. Ignoring.")
@@ -324,22 +330,24 @@
         tokamak=machine,
         Rmin=data["rleft"],
         Rmax=data["rleft"] + data["rdim"],
         Zmin=data["zmid"] - 0.5 * data["zdim"],
         Zmax=data["zmid"] + 0.5 * data["zdim"],
         nx=nx,
         ny=ny,  # Number of grid points
+        check_limited=True,
+        psi=psi,
     )
     # Grid spacing
     dR = eq.R[1, 0] - eq.R[0, 0]
     dZ = eq.Z[0, 1] - eq.Z[0, 0]
 
-    # Create masking function: 1 inside plasma, 0 outside
-    opoint, xpoint = critical.find_critical(eq.R, eq.Z, psi)
-    mask = critical.core_mask(eq.R, eq.Z, psi, opoint, xpoint, psi_bndry)
+    psi_bndry = eq.psi_bndry
+    psi_axis = eq.psi_axis
+    mask = eq.mask
 
     # Toroidal current
     Jtor = eq.R * pprime_func(psi_norm) + ffprime_func(psi_norm) / (eq.R * mu0)
     Jtor *= mask
 
     # Quick calculation of total toroidal current
     print("CURRENT: ", romb(romb(Jtor)) * dR * dZ)
@@ -362,38 +370,46 @@
         # Create an interpolation function for Jtor and the input psi
         Jtor_func = interpolate.RectBivariateSpline(eq.R[:, 0], eq.Z[0, :], Jtor)
         psi_func = interpolate.RectBivariateSpline(eq.R[:, 0], eq.Z[0, :], psi)
 
         # Create a new Equilibrium object
         # (replacing previous 'eq')
         eq = Equilibrium(
-            tokamak=machine, Rmin=Rmin, Rmax=Rmax, Zmin=Zmin, Zmax=Zmax, nx=nx, ny=ny
+            tokamak=machine,
+            Rmin=Rmin,
+            Rmax=Rmax,
+            Zmin=Zmin,
+            Zmax=Zmax,
+            nx=nx,
+            ny=ny,
+            check_limited=True,
         )
 
         # Interpolate Jtor and psi onto new grid
         Jtor = Jtor_func(eq.R, eq.Z, grid=False)
         psi = psi_func(eq.R, eq.Z, grid=False)
 
+        psi_bndry = eq.psi_bndry
+        psi_axis = eq.psi_axis
+        mask = eq.mask
+
         # Update the mask function by calculating normalised psi
         # on the new grid
         psi_norm = clip((psi - psi_axis) / (psi_bndry - psi_axis), 0.0, 1.0)
 
-        # Create masking function: 1 inside plasma, 0 outside
-        opoint, xpoint = critical.find_critical(eq.R, eq.Z, psi)
-        mask = critical.core_mask(eq.R, eq.Z, psi, opoint, xpoint, psi_bndry)
-
     # Note: Here we have
     #   eq : Equilibrium object
     #   Jtor : 2D array (nx,ny) Toroidal current density
     #   psi  : 2D array (nx,ny) Input poloidal flux
     #   psi_norm : 2D array (nx,ny) Normalised input poloidal flux
     #   mask : 2D array (nx,ny) 1 inside plasma, 0 outside
 
     # Perform a linear solve to calculate psi
     # using known Jtor
+    eq.check_limited = True
     eq.solve(profiles, Jtor=Jtor)
 
     print(
         "Plasma current: {0} Amps, input: {1} Amps".format(
             eq.plasmaCurrent(), data["cpasma"]
         )
     )
@@ -421,19 +437,30 @@
         # Draw separatrix if there is an X-point
         if len(xpoint) > 0:
             axis.contour(eq.R, eq.Z, psi, levels=[xpoint[0][2]], colors="r")
 
     # Find best fit for coil currents
     # First create a control system (see control.py)
     if fit_sol:
-        controlsystem = control.ConstrainPsi2D(psi)  # Fit entire domain
+        # Fit entire domain
+        if current_bounds is not None:
+            controlsystem = control.ConstrainPsi2DAdvanced(
+                psi, current_lims=current_bounds
+            )
+        else:
+            controlsystem = control.ConstrainPsi2D(psi)
     else:
-        controlsystem = control.ConstrainPsi2D(
-            psi, weights=mask
-        )  # Remove SOL from fitting
+        # Remove SOL from fitting
+        if current_bounds is not None:
+            controlsystem = control.ConstrainPsi2DAdvanced(
+                psi, weights=mask, current_lims=current_bounds
+            )
+        else:
+            controlsystem = control.ConstrainPsi2D(psi, weights=mask)
+
     # Run control system to find coil currents
     controlsystem(eq)
 
     if show:
         axis.contour(eq.R, eq.Z, eq.psi(), 50, colors="r")
         plt.pause(1)
 
@@ -441,25 +468,32 @@
     machine.printCurrents()
 
     ####################################################################
     # Refine the equilibrium to ensure consistency
     # Solve using Picard iteration
     #
 
-    controlsystem = control.ConstrainPsiNorm2D(psi_norm, weights=mask)
+    if current_bounds is not None:
+        controlsystem = control.ConstrainPsiNorm2DAdvanced(
+            psi_norm, weights=mask, current_lims=current_bounds
+        )
+        maxits = 1000  # Constrained coil currents may require many iterations
+    else:
+        controlsystem = control.ConstrainPsiNorm2D(psi_norm, weights=mask)
     picard.solve(
         eq,  # The equilibrium to adjust
         profiles,  # The toroidal current profile function
         controlsystem,
         show=show,
         axis=axis,
         pause=pause,
         rtol=rtol,
         blend=blend,
         maxits=maxits,
+        check_limited=True,
     )
 
     print(
         "Plasma current: {0} Amps, input: {1} Amps".format(
             eq.plasmaCurrent(), data["cpasma"]
         )
     )
```

### Comparing `FreeGS-0.7.0/freegs/gradshafranov.py` & `FreeGS-0.8.0/freegs/gradshafranov.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.7.0/freegs/jtor.py` & `FreeGS-0.8.0/freegs/jtor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,9 @@
 """
- Classes representing plasma profiles.
-
- These must have the following methods:
-
-   Jtor(R, Z, psi, psi_bndry=None)
-      -> Return a numpy array of toroidal current density [J/m^2]
-   pprime(psinorm)
-      -> return p' at given normalised psi
-   ffprime(psinorm)
-      -> return ff' at given normalised psi
-   pressure(psinorm)
-      -> return p at given normalised psi
-   fpol(psinorm)
-      -> return f at given normalised psi
-   fvac()
-      -> f = R*Bt in vacuum
-
+Classes representing plasma profiles.
 
 Copyright 2016 Ben Dudson, University of York. Email: benjamin.dudson@york.ac.uk
 
 This file is part of FreeGS.
 
 FreeGS is free software: you can redistribute it and/or modify
 it under the terms of the GNU Lesser General Public License as published by
@@ -37,17 +21,18 @@
 import matplotlib.pyplot as plt
 from scipy.integrate import romb, quad  # Romberg integration
 from . import critical
 from .gradshafranov import mu0
 
 from numpy import clip, zeros, reshape, sqrt, pi
 import numpy as np
+import abc
 
 
-class Profile(object):
+class Profile(abc.ABC):
     """
     Base class from which profiles classes can inherit
 
     This provides two methods:
        pressure(psinorm) and fpol(psinorm)
 
     which assume that the following methods are available:
@@ -121,14 +106,36 @@
 
             # ffprime = 0.5*d/dpsi(f^2)
             # Apply boundary condition at psinorm=1 val = fvac**2
             ovals[i] = sqrt(2.0 * val + self.fvac() ** 2)
 
         return reshape(ovals, psinorm.shape)
 
+    """
+    Abstract methods that derived classes must implement.
+    """
+    @abc.abstractmethod
+    def Jtor(self, R: np.ndarray, Z: np.ndarray, psi: np.ndarray, psi_bndry=None)->np.ndarray:
+        """Return a numpy array of toroidal current density [J/m^2]"""
+        pass
+
+    @abc.abstractmethod
+    def pprime(self, psinorm: float)->float:
+        """Return p' at the given normalised psi"""
+        pass
+
+    @abc.abstractmethod
+    def ffprime(self, psinorm: float)->float:
+        """Return ff' at the given normalised psi"""
+        pass
+
+    @abc.abstractmethod
+    def fvac(self)->float:
+        """Return f = R*Bt in vacuum"""
+        pass
 
 class ConstrainBetapIp(Profile):
     """
     Constrain poloidal Beta and plasma current
 
     This is the constraint used in
     YoungMu Jeon arXiv:1503.03135
@@ -230,36 +237,36 @@
             pfunc *= mask
 
         # Integrate over plasma
         # betap = (2mu0) * (int(p)RdRdZ)/(int(B_poloidal**2)RdRdZ)
         #       = - (2L*Beta0*mu0/Raxis) * (pfunc*RdRdZ)/((int(B_poloidal**2)RdRdZ))
 
         # Produce array of Bpol in (R,Z) for core plasma
-        B_polvals_2 = self.eq.Br(R,Z)**2 + self.eq.Bz(R,Z)**2
+        B_polvals_2 = self.eq.Br(R, Z) ** 2 + self.eq.Bz(R, Z) ** 2
         if mask is not None:
             B_polvals_2 *= mask
 
-        p_int = romb(romb(pfunc * R)) * dR*dZ
-        b_int = romb(romb(B_polvals_2 *R)) * dR*dZ
-        
-        #self.betap = - (2*LBeta0*mu0/ self.Raxis) * (p_int/b_int)
-        LBeta0 = (b_int/p_int) * (- self.betap * self.Raxis)/(2*mu0)
+        p_int = romb(romb(pfunc * R)) * dR * dZ
+        b_int = romb(romb(B_polvals_2 * R)) * dR * dZ
+
+        # self.betap = - (2*LBeta0*mu0/ self.Raxis) * (p_int/b_int)
+        LBeta0 = (b_int / p_int) * (-self.betap * self.Raxis) / (2 * mu0)
 
         # Integrate current components
-        IR = romb(romb(jtorshape * R/self.Raxis)) * dR*dZ
-        I_R = romb(romb(jtorshape * self.Raxis/R)) * dR*dZ
-        
+        IR = romb(romb(jtorshape * R / self.Raxis)) * dR * dZ
+        I_R = romb(romb(jtorshape * self.Raxis / R)) * dR * dZ
+
         # Toroidal plasma current Ip is
         #
         # Ip = L * (Beta0 * IR + (1-Beta0)*I_R)
         #    = L*Beta0*(IR - I_R) + L*I_R
         #
-        #L = self.Ip / ( (Beta0*IR) + ((1.0-Beta0)*(I_R)) )
+        # L = self.Ip / ( (Beta0*IR) + ((1.0-Beta0)*(I_R)) )
 
-        L = self.Ip/I_R - LBeta0*(IR/I_R - 1)
+        L = self.Ip / I_R - LBeta0 * (IR / I_R - 1)
         Beta0 = LBeta0 / L
 
         # print("Constraints: L = %e, Beta0 = %e" % (L, Beta0))
 
         # Toroidal current
         Jtor = L * (Beta0 * R / self.Raxis + (1 - Beta0) * self.Raxis / R) * jtorshape
 
@@ -403,23 +410,22 @@
         self.L = L
         self.Beta0 = Beta0
         self.psi_bndry = psi_bndry
         self.psi_axis = psi_axis
 
         return Jtor
 
-    # Profile functions
     def pprime(self, pn):
         """
         dp/dpsi as a function of normalised psi. 0 outside core
         Calculate pprimeshape inside the core only
         """
         shape = (1.0 - np.clip(pn, 0.0, 1.0) ** self.alpha_m) ** self.alpha_n
         return self.L * self.Beta0 / self.Raxis * shape
-
+    
     def ffprime(self, pn):
         """
         f * df/dpsi as a function of normalised psi. 0 outside core.
         Calculate ffprimeshape inside the core only.
         """
         shape = (1.0 - np.clip(pn, 0.0, 1.0) ** self.alpha_m) ** self.alpha_n
         return mu0 * self.L * (1 - self.Beta0) * self.Raxis * shape
```

### Comparing `FreeGS-0.7.0/freegs/machine.py` & `FreeGS-0.8.0/freegs/machine.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,23 +19,28 @@
 GNU Lesser General Public License for more details.
 
 You should have received a copy of the GNU Lesser General Public License
 along with FreeGS.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 from .gradshafranov import Greens, GreensBr, GreensBz
-
-from numpy import linspace
 import numpy as np
+import scipy.linalg
 from scipy.interpolate import interp1d
+from scipy.special import ellipk, ellipe
+from scipy.constants import mu_0
 
 from .coil import Coil, AreaCurrentLimit
 from .shaped_coil import ShapedCoil
 from .pre_calc_coil import PreCalcCoil
 from .filament_coil import FilamentCoil
+from .multi_coil import MultiCoil
+
+from shapely.geometry import Point, LinearRing, LineString
+from shapely.geometry.polygon import Polygon
 
 # We need this for the `label` part of the Circuit dtype for writing
 # to HDF5 files. See the following for information:
 # http://docs.h5py.org/en/latest/strings.html#how-to-store-text-strings
 try:
     import h5py
 
@@ -81,14 +86,48 @@
         """
         coils - A list [ (label, Coil, multiplier) ]
         """
 
         self.coils = coils
         self.current = current
         self.control = control
+    
+    def __getitem__(self, name):
+        """Returns a coil in the circuit using circuit[coil_name]"""
+
+        for label, coil, _ in self.coils:
+            if label == name:
+                return coil
+        raise KeyError("Circuit does not contain coil with label '{0}'".format(name))
+    
+    @property
+    def current(self) -> float:
+        return self._current
+
+    @current.setter
+    def current(self, value: float):
+        """
+        When updating the circuit current, also update the current in the coils in the circuit (with multipliers)
+        """
+        self._current = value
+        for _, coil, multiplier in self.coils:
+            coil.current = multiplier * value
+
+    @property
+    def control(self) -> bool:
+        return self._control
+
+    @control.setter
+    def control(self, value: bool):
+        """
+        When updating the circuit control switch, also update the control switch in the coils in the circuit
+        """
+        self._control = value
+        for _, coil, _ in self.coils:
+            coil.control = value
 
     def psi(self, R, Z):
         """
         Calculate poloidal flux at (R,Z)
         """
         psival = 0.0
         for label, coil, multiplier in self.coils:
@@ -170,14 +209,17 @@
         Returns a dictionary of coil label -> force
         """
         forces = {}
         for label, coil, multiplier in self.coils:
             forces[label] = coil.getForces(equilibrium)
         return forces
 
+    def inShape(self, polygon):
+        return sum(coil.inShape(polygon)*multiplier for label, coil, multiplier in self.coils)
+
     def __repr__(self):
         result = "Circuit(["
         coils = [
             '("{0}", {1}, {2})'.format(label, coil, multiplier)
             for label, coil, multiplier in self.coils
         ]
         result += ", ".join(coils)
@@ -288,15 +330,15 @@
     dtype = np.dtype(
         [
             (str("Rs"), np.float64),
             (str("Zsmin"), np.float64),
             (str("Zsmax"), np.float64),
             (str("Ns"), np.float64),
             (str("current"), np.float64),
-            (str("control"), np.bool),
+            (str("control"), bool),
         ]
     )
 
     def __init__(self, Rs, Zsmin, Zsmax, Ns, current=0.0, control=True):
         """
         Rs - Radius of the solenoid
         Zsmin, Zsmax - Minimum and maximum Z
@@ -347,33 +389,33 @@
         """
         Calculate poloidal flux at (R,Z) due to a unit current
 
         R and Z should have the same dimensions, but can be multi-dimensional
         Return should have the same shape
         """
         result = 0.0
-        for Zs in linspace(self.Zsmin, self.Zsmax, self.Ns):
+        for Zs in np.linspace(self.Zsmin, self.Zsmax, self.Ns):
             result += Greens(self.Rs, Zs, R, Z)
         return result
 
     def controlBr(self, R, Z):
         """
         Calculate radial magnetic field Br at (R,Z) due to a unit current
         """
         result = 0.0
-        for Zs in linspace(self.Zsmin, self.Zsmax, self.Ns):
+        for Zs in np.linspace(self.Zsmin, self.Zsmax, self.Ns):
             result += GreensBr(self.Rs, Zs, R, Z)
         return result
 
     def controlBz(self, R, Z):
         """
         Calculate vertical magnetic field Bz at (R,Z) due to a unit current
         """
         result = 0.0
-        for Zs in linspace(self.Zsmin, self.Zsmax, self.Ns):
+        for Zs in np.linspace(self.Zsmin, self.Zsmax, self.Ns):
             result += GreensBz(self.Rs, Zs, R, Z)
         return result
 
     def getForces(self, equilibrium):
         """
         Calculate forces on the solenoid.
         Not currently implemented
@@ -438,39 +480,184 @@
     def __eq__(self, other):
         return np.allclose(self.R, other.R) and np.allclose(self.Z, other.Z)
 
     def __ne__(self, other):
         return not self == other
 
 
+class Sensor:
+    """
+    Parent class for the sensors
+    Contains general attributes that apply to all sensors
+    """
+    def __init__(self, R, Z, name=None, weight=1, status=True, measurement=None):
+
+        self.R = R
+        self.Z = Z
+        self.status = status
+        self.name = name
+        self.weight = weight
+
+        if self.status:
+            self.measurement = measurement
+
+
+    def __repr__(self):
+        return "R={R}, Z={Z}".format(R=self.R, Z=self.Z)
+
+    def __eq__(self, other):
+        return np.allclose(self.R, other.R) and np.allclose(self.Z, other.Z)
+
+    def __ne__(self, other):
+        return not self == other
+
+
+class RogowskiSensor(Sensor):
+    """
+    Represents a Rogowski sensor.
+    Consists of an ordered list of (R,Z) points (defines polygon on which sensor lies)
+    Returns current inside the loop
+    """
+
+    def __init__(self, R, Z, name=None, weight=1, status=True,
+                 measurement=None):
+
+        Sensor.__init__(self, R, Z, name=name, weight=weight, status=status, measurement=measurement)
+
+        polygonlist = [(r, z) for r, z in zip(self.R, self.Z)]
+        self.polygon = Polygon(polygonlist)
+
+    def get_measure(self, tokamak, eq):
+        """
+        Method to update the current attribute of the sensor
+        with whatever current is contained within the sensor
+        if sensor is on (status == True)
+        """
+
+        if self.status:
+
+            # coil current
+            coil_current = 0
+            for label, coil in tokamak.coils:
+                coil_current += coil.inShape(self.polygon) * coil.current
+
+            # plasma current
+            plasma_current = 0
+            if eq is not None:
+                for index, (R, Z) in enumerate(zip(eq.R.flatten(order = 'F'), eq.Z.flatten(order='F'))):
+                    gridpoint = Polygon([(R - eq.dR / 2,
+                                          Z + eq.dZ / 2), (
+                                             R + eq.dR / 2,
+                                             Z + eq.dZ / 2), (
+                                             R + eq.dR / 2,
+                                             Z - eq.dZ / 2), (
+                                             R - eq.dR / 2,
+                                             Z - eq.dZ / 2)])
+
+                    plasma_current += eq.Jtor.flatten(order='F')[index] \
+                                      * self.polygon.intersection(gridpoint).area
+
+            self.measurement = plasma_current + coil_current
+
+    def plot(self, axis):
+        axis.plot(list(self.R) + [self.R[0]],
+                  list(self.Z) + [self.Z[0]], "b")
+
+
+class PoloidalFieldSensor(Sensor):
+    """
+    Represents position of a Poloidal B field sensor.
+    Consists a single (R,Z) point, and an angle Theta
+    At which the field is measured at
+    """
+    def __init__(self, R, Z, theta, name=None, weight=1, status=True, measurement=None):
+        Sensor.__init__(self, R, Z, name=name, weight=weight, status=status,measurement=measurement)
+        self.theta = theta
+
+    def __repr__(self):
+        return "R={R}, Z={Z}, Theta={Theta}".format(R=self.R, Z=self.Z, Theta=self.theta)
+
+    def get_measure(self, tokamak, eq):
+        """
+        Updates field attribute of sensor with measured field at that
+        point/direction if sensor is on
+        """
+
+        if self.status:
+
+            field = (tokamak.Br(self.R, self.Z)) * np.cos(self.theta) + (tokamak.Bz(self.R, self.Z)) * np.sin(self.theta)
+
+            if eq is not None:
+                field += (eq.plasmaBr(self.R, self.Z)) * np.cos(self.theta) + (eq.plasmaBz(self.R, self.Z)) * np.sin(self.theta)
+
+            self.measurement = field
+
+    def plot(self, axis):
+        axis.plot(self.R, self.Z, 'mo')
+        axis.arrow(self.R, self.Z, 0.1 * np.cos(self.theta),
+                   0.1 * np.sin(self.theta))
+
+
+class FluxLoopSensor(Sensor):
+    """
+    Represents position of a Flux Loop Sensor.
+    Consists a single (R,Z) point, describing the position of the probe
+    Contains a method to find the value of flux (psi) at the position
+    """
+    def __init__(self, R, Z, name=None, weight=1, status=True, measurement=None):
+        Sensor.__init__(self, R, Z, name=name, weight=weight, status=status, measurement=measurement)
+
+    def get_measure(self, tokamak, eq):
+        """
+            Updates flux attribute with
+            poloidal flux at the point of measurement
+            if sensor is on
+        """
+        if self.status:
+            if eq is not None:
+                psi = eq.psiRZ(self.R,self.Z)
+            else:
+                psi = tokamak.psi(self.R, self.Z)
+
+            self.measurement = psi
+
+    def plot(self, axis):
+        axis.plot(self.R, self.Z, 'ro')
+
+
 class Machine:
     """
     Represents the machine (Tokamak), including
     coils and power supply circuits
 
     coils[(label, Coil|Circuit|Solenoid] - List of coils
 
     Note: a list is used rather than a dict, so that the coils
     remain ordered, and so can be updated easily by the control system.
     Instead __getitem__ is implemented to allow access to coils
 
     """
 
-    def __init__(self, coils, wall=None):
+    def __init__(self, coils, wall=None, sensors=None, nlimit=500):
         """
         coils - A list of coils [(label, Coil|Circuit|Solenoid)]
+        sensors - A list of sensors
         """
 
         self.coils = coils
         self.wall = wall
+        self.sensors = sensors
+
         self.limit_points_R = None
         self.limit_points_Z = None
 
         if self.wall is not None:
-            self.limit_points_R, self.limit_points_Z = self.generate_limit_points()
+            self.limit_points_R, self.limit_points_Z = self.generate_limit_points(
+                nlimit
+            )
 
     def __repr__(self):
         return "Machine(coils={coils}, wall={wall})".format(
             coils=self.coils, wall=self.wall
         )
 
     def __eq__(self, other):
@@ -483,44 +670,43 @@
 
     def __getitem__(self, name):
         for label, coil in self.coils:
             if label == name:
                 return coil
         raise KeyError("Machine does not contain coil with label '{0}'".format(name))
 
-    def generate_limit_points(self):
-        '''
+    def generate_limit_points(self, nlimit):
+        """
         Generate points along the machine wall that may be used to check
         if the plasma is limited or not.
-        '''
+        """
 
-        # Interpolate wall limit points (get_divcoords typically only return 8 or so points)
+        # Interpolate wall limit points.
         # Make an interpolator for point location as function of normalised distance
         # along the wall
-        points = np.array([self.wall.R,self.wall.Z]).T
-        distance = np.cumsum(np.sqrt(np.sum(np.diff(points,axis=0)**2,axis=1)))
-        distance = np.insert(distance,0,0)/distance[-1]
+        points = np.array([self.wall.R, self.wall.Z]).T
+        distance = np.cumsum(np.sqrt(np.sum(np.diff(points, axis=0) ** 2, axis=1)))
+        distance = np.insert(distance, 0, 0) / distance[-1]
 
-        interpolator = interp1d(distance,points,kind='linear',axis=0)
-        new_distances = np.linspace(0,1,500,endpoint=True)
+        interpolator = interp1d(distance, points, kind="linear", axis=0)
+        new_distances = np.linspace(0, 1, nlimit, endpoint=True)
         interpolated_points = interpolator(new_distances)
 
-        R = np.asarray(interpolated_points[:,0])
-        Z = np.asarray(interpolated_points[:,1])
+        R = np.asarray(interpolated_points[:, 0])
+        Z = np.asarray(interpolated_points[:, 1])
 
         return R, Z
 
     def psi(self, R, Z):
         """
         Poloidal flux due to coils
         """
         psi_coils = 0.0
         for label, coil in self.coils:
             psi_coils += coil.psi(R, Z)
-
         return psi_coils
 
     def createPsiGreens(self, R, Z):
         """
         An optimisation, which pre-computes the Greens functions
         and puts into arrays for each coil. This map can then be
         called at a later time, and quickly return the field
@@ -534,14 +720,15 @@
         """
         Uses the object returned by createPsiGreens to quickly
         compute the plasma psi
         """
         psi_coils = 0.0
         for label, coil in self.coils:
             psi_coils += coil.calcPsiFromGreens(pgreen[label])
+
         return psi_coils
 
     def Br(self, R, Z):
         """
         Radial magnetic field at given points
         """
         Br = 0.0
@@ -612,14 +799,37 @@
 
     def printCurrents(self):
         print("==========================")
         for label, coil in self.coils:
             print(label + " : " + str(coil))
         print("==========================")
 
+    def takeMeasurements(self, eq=None):
+        """
+        Method calling the measure method of each sensor on the machine
+        """
+        for sensor in self.sensors:
+            sensor.get_measure(self, eq)
+
+    def printMeasurements(self, eq=None):
+        """
+        Method for calling the takeMeasurements method, then printing the results
+        """
+        print("==========================")
+        self.takeMeasurements(eq=eq)
+        for sensor in self.sensors:
+            if sensor.name is not None:
+                print(sensor.name + ' '+ str(sensor) + ", Measurement=" + str(
+                    sensor.measurement))
+            else:
+                print(str(type(sensor)) + str(sensor) + " Measurement=" + str(
+                    sensor.measurement))
+        print("==========================")
+        return
+
     def getForces(self, equilibrium=None):
         """
         Calculate forces on the coils, given the plasma equilibrium.
         If no plasma equilibrium given then the forces due to
         the coils alone will be calculated.
 
         Returns a dictionary of coil label -> force
@@ -679,14 +889,15 @@
 
     wall = Wall(
         [0.75, 0.75, 1.5, 1.8, 1.8, 1.5], [-0.85, 0.85, 0.85, 0.25, -0.25, -0.85]  # R
     )  # Z
 
     return Machine(coils, wall)
 
+
 def TestTokamakLimited():
     """
     Create a simple tokamak
     """
 
     coils = [
         (
@@ -701,42 +912,117 @@
     wall = Wall(
         [0.93, 0.93, 1.5, 1.8, 1.8, 1.5], [-0.85, 0.85, 0.85, 0.25, -0.25, -0.85]  # R
     )  # Z
 
     return Machine(coils, wall)
 
 
-def DIIID():
+def TestTokamakSensor():
     """
-    PF coil set from ef20030203.d3d
-    Taken from Corsica
+    Creating a simple tokamak with sensors along the boundary
     """
 
     coils = [
-        {"label": "F1A", "R": 0.8608, "Z": 0.16830, "current": 0.0},
-        {"label": "F2A", "R": 0.8614, "Z": 0.50810, "current": 0.0},
-        {"label": "F3A", "R": 0.8628, "Z": 0.84910, "current": 0.0},
-        {"label": "F4A", "R": 0.8611, "Z": 1.1899, "current": 0.0},
-        {"label": "F5A", "R": 1.0041, "Z": 1.5169, "current": 0.0},
-        {"label": "F6A", "R": 2.6124, "Z": 0.4376, "current": 0.0},
-        {"label": "F7A", "R": 2.3733, "Z": 1.1171, "current": 0.0},
-        {"label": "F8A", "R": 1.2518, "Z": 1.6019, "current": 0.0},
-        {"label": "F9A", "R": 1.6890, "Z": 1.5874, "current": 0.0},
-        {"label": "F1B", "R": 0.8608, "Z": -0.1737, "current": 0.0},
-        {"label": "F2B", "R": 0.8607, "Z": -0.5135, "current": 0.0},
-        {"label": "F3B", "R": 0.8611, "Z": -0.8543, "current": 0.0},
-        {"label": "F4B", "R": 0.8630, "Z": -1.1957, "current": 0.0},
-        {"label": "F5B", "R": 1.0025, "Z": -1.5169, "current": 0.0},
-        {"label": "F6B", "R": 2.6124, "Z": -0.44376, "current": 0.0},
-        {"label": "F7B", "R": 2.3834, "Z": -1.1171, "current": 0.0},
-        {"label": "F8B", "R": 1.2524, "Z": -1.6027, "current": 0.0},
-        {"label": "F9B", "R": 1.6889, "Z": -1.578, "current": 0.0},
+        (
+            "P1L",
+            ShapedCoil(
+                [(0.95, -1.15), (0.95, -1.05), (1.05, -1.05), (1.05, -1.15)]),
+        ),
+        ("P1U",
+         ShapedCoil([(0.95, 1.15), (0.95, 1.05), (1.05, 1.05), (1.05, 1.15)])),
+        ("P2L", Coil(1.75, -0.6)),
+        ("P2U", Coil(1.75, 0.6)),
+    ]
+
+    wall = Wall([0.75, 0.75, 1.5, 1.8, 1.8, 1.5],[-0.85, 0.85, 0.85, 0.25, -0.25, -0.85])
+
+    sensors = [RogowskiSensor([0.77, 0.77, 1.48, 1.78, 1.78, 1.48],
+                              [-0.83, 0.83, 0.83, 0.23, -0.23, -0.83], name='Rog1')
+        , PoloidalFieldSensor(1.8, 0.14, 2.2, name='BP1')
+        , PoloidalFieldSensor(1.8, -0.14, -2.2, name='BP2')
+        , PoloidalFieldSensor(1.7, 0.475, 2.2, name='BP3')
+        , PoloidalFieldSensor(1.7, -0.475, -2.2, name='BP4')
+        , PoloidalFieldSensor(1.5, 0.85, 2.2, name='BP5')
+        , PoloidalFieldSensor(1.5, -0.85, -2.2, name='BP6')
+        , FluxLoopSensor(1.8, 0.2, name='FL1')
+        , FluxLoopSensor(1.8, -0.2, name='FL2')
+        , FluxLoopSensor(1.65, 0.52, name='FL3')
+        , FluxLoopSensor(1.65, -0.52, name='FL4')
+        , FluxLoopSensor(1.1, 0.85, name='FL5')
+        , FluxLoopSensor(1.1, -0.85, name='FL6')
+               ]
+
+    return Machine(coils, wall, sensors)
+
+
+def DIIID():
+    """
+    PF coil set and boundary from g file and GA webpage
+    """
+    coils = [
+        ("FC1",ShapedCoil([[1.6042, -1.64455], [1.7736, -1.64455], [1.7736, -1.51145], [1.6042, -1.51145]])),
+        ("FC2",ShapedCoil([[0.8354, 0.00777], [0.8862, 0.00777], [0.8862, 0.32883], [0.8354, 0.32883]])),
+        ("FC3",ShapedCoil([[0.836, 0.34757], [0.8868, 0.34757], [0.8868, 0.66863], [0.836, 0.66863]])),
+        ("FC4",ShapedCoil([[0.8374, 0.68857], [0.8882, 0.68857], [0.8882, 1.00963], [0.8374, 1.00963]])),
+        ("FC5",ShapedCoil([[0.8357, 1.02937], [0.8865, 1.02937], [0.8865, 1.35043], [0.8357, 1.35043]])),
+        ("FC6",ShapedCoil([[0.9345, 1.3876], [1.0737, 1.5268], [1.0737, 1.6462], [0.9345, 1.507]])),
+        ("FC7",ShapedCoil([[2.5298, 0.3403], [2.703, 0.3403], [2.6949, 0.5349], [2.5217, 0.5349]])),
+        ("FC8",ShapedCoil([[2.5387, 1.0325], [2.7267, 1.0325], [2.2078, 1.2017], [2.0198, 1.2017]])),
+        ("FC9",ShapedCoil([[1.13435, 1.55935], [1.36925, 1.55935], [1.36925, 1.64445], [1.13435, 1.64445]])),
+        ("FC10",ShapedCoil([[1.6043, 1.52085], [1.7737, 1.52085], [1.7737, 1.65395], [1.6043, 1.65395]])),
+        ("FC11",ShapedCoil([[0.8354, -0.33423], [0.8862, -0.33423], [0.8862, -0.01317], [0.8354, -0.01317]])),
+        ("FC12",ShapedCoil([[0.8353, -0.67403], [0.8861, -0.67403], [0.8861, -0.35297], [0.8353, -0.35297]])),
+        ("FC13",ShapedCoil([[0.8357, -1.01483], [0.8865, -1.01483], [0.8865, -0.69377], [0.8357, -0.69377]])),
+        ("FC14",ShapedCoil([[0.8376, -1.35623], [0.8884, -1.35623], [0.8884, -1.03517], [0.8376, -1.03517]])),
+        ("FC15",ShapedCoil([[0.9329, -1.507], [1.0721, -1.6462], [1.0721, -1.5268], [0.9329, -1.3876]])),
+        ("FC16",ShapedCoil([[2.5217, -0.5349], [2.6949, -0.5349], [2.703, -0.3403], [2.5298, -0.3403]])),
+        ("FC17",ShapedCoil([[2.0299, -1.2017], [2.2179, -1.2017], [2.7368, -1.0325], [2.5488, -1.0325]])),
+        ("FC18",ShapedCoil([[1.13495, -1.64525], [1.36985, -1.64525], [1.36985, -1.56015], [1.13495, -1.56015]]))
     ]
 
-    return Machine(coils)
+    R = np.array([1.016,1.016,1.016,1.016,1.016,1.016,1.016,1.016,1.016,
+        1.016,1.016,1.012,1.001,1.029,1.042,1.046,1.056,1.097,
+        1.108,1.116,1.134,1.148,1.162,1.181,1.182,1.185,1.19,
+        1.195,1.201,1.209,1.215,1.222,1.228,1.234,1.239,1.242,
+        1.248,1.258,1.263,1.28,1.28,1.28,1.31,1.328,1.361,
+        1.38,1.419,1.419,1.372,1.37167,1.37003,1.36688,1.36719,1.37178,
+        1.37224,1.38662,1.38708,1.40382,1.41127,1.41857,1.421,1.48663,1.4973,
+        1.49762,1.49745,1.49275,1.4926,1.49261,1.49279,1.4934,1.4947,1.49622,
+        1.47981,1.48082,1.48149,1.48646,1.49095,1.50305,1.59697,1.6255,1.63752,
+        1.647,1.785,2.07,2.128,2.245,2.33956,2.34708,2.34913,2.35103,
+        2.35158,2.35125,2.35051,2.34965,2.3487,2.3476,2.3402,2.32942,2.134,
+        1.786,1.768,1.768,1.682,1.372,1.372,1.42,1.42,1.273,
+        1.153,1.016,1.016,1.016,1.016,1.016,1.016,1.016,1.016])
+    Z = np.array([ 0.00000e+00,9.64000e-01,9.68000e-01,1.00100e+00,1.01900e+00,
+        1.07700e+00,1.07000e+00,1.09600e+00,1.11300e+00,1.13800e+00,
+        1.14700e+00,1.16500e+00,1.21700e+00,1.21700e+00,1.16240e+00,
+        1.16238e+00,1.16260e+00,1.16450e+00,1.16594e+00,1.16591e+00,
+        1.16896e+00,1.17175e+00,1.17556e+00,1.18300e+00,1.18350e+00,
+        1.18500e+00,1.18800e+00,1.19100e+00,1.19600e+00,1.20200e+00,
+        1.20800e+00,1.21400e+00,1.22100e+00,1.23100e+00,1.23800e+00,
+        1.24400e+00,1.25400e+00,1.27800e+00,1.29000e+00,1.33100e+00,
+        1.34700e+00,1.34800e+00,1.34800e+00,1.34800e+00,1.34800e+00,
+        1.34800e+00,1.34800e+00,1.31000e+00,1.31000e+00,1.29238e+00,
+        1.28268e+00,1.25644e+00,1.22955e+00,1.19576e+00,1.19402e+00,
+        1.16487e+00,1.16421e+00,1.15696e+00,1.15730e+00,1.16132e+00,
+        1.16400e+00,1.24050e+00,1.23458e+00,1.23428e+00,1.23174e+00,
+        1.21330e+00,1.21061e+00,1.20486e+00,1.20214e+00,1.19642e+00,
+        1.18511e+00,1.16070e+00,1.12426e+00,1.12256e+00,1.12138e+00,
+        1.11692e+00,1.11439e+00,1.11244e+00,1.09489e+00,1.08530e+00,
+        1.07988e+00,1.07700e+00,1.07700e+00,1.04000e+00,9.93000e-01,
+        7.09000e-01,4.61430e-01,4.15830e-01,2.72180e-01,1.70180e-01,
+        7.01200e-02, -3.17900e-02, -1.44350e-01, -2.14830e-01, -3.26690e-01,
+        -3.86770e-01, -4.53040e-01, -4.77570e-01, -9.73000e-01, -1.17400e+00,
+        -1.21100e+00, -1.25000e+00, -1.25000e+00, -1.25000e+00, -1.32900e+00,
+        -1.32900e+00, -1.36300e+00, -1.36300e+00, -1.36300e+00, -1.22300e+00,
+        -1.22300e+00, -8.30000e-01, -8.00000e-01, -4.15000e-01, -4.00000e-01,
+        -1.00000e-03,0.00000e+00])
+    wall = Wall(R,Z)
+
+    return Machine(coils,wall=wall)
 
 
 def MAST():
     """
     Mega-Amp Spherical Tokamak. This version has all independent coils
     so that each is powered by a separate coil
     """
```

### Comparing `FreeGS-0.7.0/freegs/multigrid.py` & `FreeGS-0.8.0/freegs/multigrid.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.7.0/freegs/optimise.py` & `FreeGS-0.8.0/freegs/optimise.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.7.0/freegs/optimiser.py` & `FreeGS-0.8.0/freegs/optimiser.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,22 @@
 You should have received a copy of the GNU Lesser General Public License
 along with FreeGS.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import random
 import copy
 import bisect
+import sys
+
+RANDOM_SEED_FOR_PYTEST = 101
+
+def _set_random_seed_if_called_in_pytest():
+    """If testing with pytest, set a random seed so that the results are deterministic"""
+    if "pytest" in sys.modules:
+        random.seed(RANDOM_SEED_FOR_PYTEST)
 
 
 def mutate(obj, controls):
     """
     Create a new object by taking an object and a set of control objects
     to change randomly
 
@@ -96,14 +104,16 @@
            generation = integer
            best = (score, object)
            population = [(score, object)]
 
     Returns the object with the lowest measure (score).
 
     """
+    _set_random_seed_if_called_in_pytest()
+
     assert N >= 4
 
     best = (measure(obj), obj)  # Highest score, candidate solution (agent)
     population = [best]  # List of (score, agent)
 
     for i in range(N - 1):
         agent = mutate(obj, controls)
```

### Comparing `FreeGS-0.7.0/freegs/picard.py` & `FreeGS-0.8.0/freegs/picard.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,30 +19,31 @@
 along with FreeGS.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 from numpy import amin, amax, array
 from . import critical
 import numpy as np
 
+
 def solve(
     eq,
     profiles,
     constrain=None,
     rtol=1e-3,
     atol=1e-10,
     blend=0.0,
     show=False,
     axis=None,
     pause=0.0001,
     psi_bndry=None,
     maxits=50,
     convergenceInfo=False,
-    check_limited = False,
-    wait_for_limited = False,
-    limit_it = 0
+    check_limited=False,
+    wait_for_limited=False,
+    limit_it=0,
 ):
     """
     Perform Picard iteration to find solution to the Grad-Shafranov equation
 
     eq       - an Equilibrium object (equilibrium.py)
     profiles - A Profile object for toroidal current (jtor.py)
 
@@ -55,15 +56,15 @@
     axis     - Specify a figure to plot onto. Default (None) creates a new figure
     pause    - Delay between output plots. If negative, waits for window to be closed
 
     maxits   - Maximum number of iterations. Set to None for no limit.
                If this limit is exceeded then a RuntimeError is raised.
 
     convergenceInfo - True/False toggle for outputting convergence data.
-    
+
     check_limited - True/False toggle to control checking for limited plasmas.
     wait_for_limited - True/False toggle to keep iterating until the plasma is limited.
     limit_it - Integer > Sometimes waiting some number of interations before checking if
     a plasma is limited can improve convergence. This sets the number of iterations to wait.
     """
 
     if constrain is not None:
@@ -87,14 +88,17 @@
 
     # Initial relative change in psi (set high to prevent immediate convergence)
     psi_relchange = 10.0
 
     # Initial psi_bndry (set low to prevent immediate convergence)
     bndry = 0.0
 
+    # Set an initial value for bndry_change (set high to prevent immediate convergence)
+    bndry_change = 10.0
+
     # Plasma assumed to not be limited at first
     has_been_limited = False
 
     # It is not yet ok to stop itterating
     ok_to_break = False
 
     psi_maxchange_iterations, psi_relchange_iterations = [], []
@@ -116,23 +120,22 @@
                 # Wait for user to close the window
                 plt.show()
             else:
                 # Update the canvas and pause
                 # Note, a short pause is needed to force drawing update
                 axis.figure.canvas.draw()
                 plt.pause(pause)
-        
 
         # Copy psi to compare at the end
         psi_last = psi.copy()
 
         # Boundary flux can also be used as a convergence criterion, so note it
         bndry_last = bndry
 
-        if((iteration>=limit_it or has_been_limited) and check_limited):
+        if (iteration >= limit_it or has_been_limited) and check_limited:
             # The user wishes to check for a limited plasma.
             # The minimum number or iterations has passed.
             # If it is ever found to be limited, keep checking for
             # further limited plasmas.
 
             eq.check_limited = True
             eq.solve(profiles, psi=psi, psi_bndry=eq.psi_bndry)
@@ -159,52 +162,61 @@
             bndry_change = bndry_last - bndry
             bndry_relchange = abs(bndry_change / bndry)
 
         else:
             # Dummy condition to prevent boundary
             # convergence when there is no boundary
             # ie set the change to > rtol
-            bndry_relchange = 2.0*rtol
+            bndry_relchange = 2.0 * rtol
 
         # Get the new psi, including coils
         psi = eq.psi()
 
         # Compare against last solution
         psi_change = psi_last - psi
         psi_maxchange = amax(abs(psi_change))
         psi_relchange = psi_maxchange / (amax(psi) - amin(psi))
 
         psi_maxchange_iterations.append(psi_maxchange)
         psi_relchange_iterations.append(psi_relchange)
 
         # User has the option to keep converging until limited
-        if(not wait_for_limited):
-			# User does not wish to wait for the plasma to become limited
+        if not wait_for_limited:
+            # User does not wish to wait for the plasma to become limited
             ok_to_break = True
 
-        elif(wait_for_limited and eq.is_limited):
+        elif wait_for_limited and eq.is_limited:
             # User wants to check if plasma limited and it is actually limited
             ok_to_break = True
 
         else:
             # The user wants to wait for a limited plasma. The plasma is not limited.
             ok_to_break = False
 
+        if show:
+            print("psi_relchange: " + str(psi_relchange))
+            print("bndry_relchange: " + str(bndry_relchange))
+            print("bndry_change: " + str(bndry_change))
+            print("\n")
+
         # Check if the changes in psi are small enough and that it is ok to start checking for convergence
-        if(((psi_maxchange < atol) or (psi_relchange < rtol)) and bndry_relchange < rtol and ok_to_break):
+        if (
+            ((psi_maxchange < atol) or (psi_relchange < rtol))
+            and ((bndry_relchange < rtol) or (abs(bndry_change) < atol))
+            and ok_to_break
+        ):
             break
 
         # Adjust the coil currents
         if constrain is not None:
             constrain(eq)
 
         psi = (1.0 - blend) * eq.psi() + blend * psi_last
 
         # Check if the maximum iterations has been exceeded
         iteration += 1
         if maxits and iteration > maxits:
             raise RuntimeError(
                 "Picard iteration failed to converge (too many iterations)"
             )
-    if convergenceInfo: 
-        return array(psi_maxchange_iterations),\
-               array(psi_relchange_iterations)
+    if convergenceInfo:
+        return array(psi_maxchange_iterations), array(psi_relchange_iterations)
```

### Comparing `FreeGS-0.7.0/freegs/plotting.py` & `FreeGS-0.8.0/freegs/plotting.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
     if axis is None:
         fig = plt.figure()
         axis = fig.add_subplot(111)
 
     return axis
 
+
 def plotConstraints(control, axis=None, show=True):
     """
     Plots constraints used for coil current control
 
     axis     - Specify the axis on which to plot
     show     - Call matplotlib.pyplot.show() before returning
 
@@ -64,23 +65,23 @@
 
     if show:
         plt.legend()
         plt.show()
 
     return axis
 
-def plotEquilibrium(eq, axis=None, show=True, oxpoints=True, wall=True):
+def plotEquilibrium(eq, axis=None, show=True, oxpoints=True, wall=True, plot_sensors=True):
     """
     Plot the equilibrium flux surfaces
 
     axis     - Specify the axis on which to plot
     show     - Call matplotlib.pyplot.show() before returning
     oxpoints - Plot X points as red circles, O points as green circles
     wall     - Plot the wall (limiter)
-
+    sensors  - Plot the sensors
     """
 
     import matplotlib.pyplot as plt
 
     R = eq.R
     Z = eq.Z
     psi = eq.psi()
@@ -97,33 +98,41 @@
     axis.set_ylabel("Height [m]")
 
     if oxpoints:
         # Add O- and X-points
         opt, xpt = critical.find_critical(eq.R, eq.Z, psi)
 
         for r, z, _ in xpt:
-            axis.plot(r, z, "ro")
+            axis.plot(r, z, "rx")
         for r, z, _ in opt:
             axis.plot(r, z, "go")
 
         if xpt:
-            psi_bndry = eq.psi_bndry #xpt[0][2]
+            psi_bndry = eq.psi_bndry  # xpt[0][2]
             axis.contour(eq.R, eq.Z, psi, levels=[psi_bndry], colors="r")
 
             # Add legend
-            axis.plot([], [], "ro", label="X-points")
+            axis.plot([], [], "rx", label="X-points")
             axis.plot([], [], "r", label="Separatrix")
         if opt:
             axis.plot([], [], "go", label="O-points")
 
     if wall and eq.tokamak.wall and len(eq.tokamak.wall.R):
         axis.plot(
             list(eq.tokamak.wall.R) + [eq.tokamak.wall.R[0]],
             list(eq.tokamak.wall.Z) + [eq.tokamak.wall.Z[0]],
             "k",
         )
 
+    if plot_sensors:
+        if eq.tokamak.sensors is not None :
+            for sensor in eq.tokamak.sensors:
+                sensor.plot(axis)
+            axis.plot([], [], 'b', label='Rogowski Coil')
+            axis.plot([], [], 'mo', label='Poloidal Field Sensor')
+            axis.plot([], [], 'ro', label='Flux Loop Sensor')
+
     if show:
         plt.legend()
         plt.show()
 
     return axis
```

### Comparing `FreeGS-0.7.0/freegs/polygons.py` & `FreeGS-0.8.0/freegs/polygons.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.7.0/freegs/pre_calc_coil.py` & `FreeGS-0.8.0/freegs/pre_calc_coil.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,22 +19,24 @@
 GNU Lesser General Public License for more details.
 
 You should have received a copy of the GNU Lesser General Public License
 along with FreeGS.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
+from scipy.interpolate import RectBivariateSpline
 from .coil import Coil, AreaCurrentLimit
 from .gradshafranov import Greens, GreensBr, GreensBz
+from . import polygons
 
 
 class PreCalcCoil(Coil):
     """
     This class represents a coil whose Green's functions have
-    already been calculate by some external code. This is useful
+    already been calculated by some external code. This is useful
     in modelling coils whose internal structure may be complex and
     whose current distribution may be highly non-uniform.
 
     The user needs to supply information on the R,Z grids that the
     Green's functions have been pre-calculated on, as well as the
     Br, Bz and psi data on said R,Z grid.
 
@@ -58,15 +60,26 @@
             (str("Z"), "10f8"),  # Note: Up to 10 points
             (str("current"), np.float64),
             (str("turns"), int),
             (str("control"), bool),
         ]
     )
 
-    def __init__(self, shape, Rgrid, Zgrid, mapBr, mapBz, mapPsi, current=0.0, turns=1, control=True):
+    def __init__(
+        self,
+        shape,
+        Rgrid,
+        Zgrid,
+        mapBr,
+        mapBz,
+        mapPsi,
+        current=0.0,
+        turns=1,
+        control=True,
+    ):
         """
         Inputs
         ------
         shape  - outline of the coil shape as a list of points [(r1,z1), (r2,z2), ...]
                  Must have more than two points
 
         Rgrid   - 1D array of R coords that maps are calculated on.
@@ -83,65 +96,65 @@
 
         # Find the geometric middle of the coil
         # The R,Z properties have accessor functions to handle modifications
         self._R_centre = sum(r for r, z in shape) / len(shape)
         self._Z_centre = sum(z for r, z in shape) / len(shape)
 
         self.current = current
-        self.turns   = turns
+        self.turns = turns
         self.control = control
-        self._area   = abs(polygons.area(shape))
-        self.shape   = shape
-        self._points = np.array([(r,z) for r, z in self.shape])
+        self._area = abs(polygons.area(shape))
+        self.shape = shape
+        self._points = np.array([(r, z) for r, z in self.shape])
 
         # Data for the pre-calculated Green's functions
-        self.Rgrid   = np.transpose(Rgrid)[:,0]
-        self.Zgrid   = np.transpose(Zgrid)[0,:]
-        self.map_psi = np.transpose(np.asarray(map_psi))
-        self.map_Br  = np.transpose(np.asarray(map_Br))
-        self.map_Bz  = np.transpose(np.asarray(map_Bz))
+        self.Rgrid = np.transpose(Rgrid)[:, 0]
+        self.Zgrid = np.transpose(Zgrid)[0, :]
+        self.mapPsi = np.transpose(np.asarray(mapPsi))
+        self.mapBr = np.transpose(np.asarray(mapBr))
+        self.mapBz = np.transpose(np.asarray(mapBz))
 
         # Interpolators for the pre-calculated Green's functions
-        self.cPsi = RectBivariateSpline(self.Rgrid,self.Zgrid,self.mapPsi)
-        self.cBr  = RectBivariateSpline(self.Rgrid,self.Zgrid,self.mapBr)
-        self.cBz  = RectBivariateSpline(self.Rgrid,self.Zgrid,self.mapBz)
+        self.cPsi = RectBivariateSpline(self.Rgrid, self.Zgrid, self.mapPsi)
+        self.cBr = RectBivariateSpline(self.Rgrid, self.Zgrid, self.mapBr)
+        self.cBz = RectBivariateSpline(self.Rgrid, self.Zgrid, self.mapBz)
 
     def controlPsi(self, R, Z):
         """
         Calculate poloidal flux at (R,Z) due to a unit current.
         """
-        
-        if isinstance(R,float) or isinstance(R,int):
-            result = self.cPsi(R,Z)[0][0]
+
+        if isinstance(R, float) or isinstance(R, int):
+            result = self.cPsi(R, Z)[0][0]
         else:
-            result = self.cPsi(R,Z,grid=False)
+            result = self.cPsi(R, Z, grid=False)
 
         return result
 
     def controlBr(self, R, Z):
         """
         Calculate radial magnetic field Br at (R,Z) due to a unit current.
         """
-        
-        if isinstance(R,float) or isinstance(R,int):
-            result = self.cBr(R,Z)[0][0]
+
+        if isinstance(R, float) or isinstance(R, int):
+            result = self.cBr(R, Z)[0][0]
         else:
-            result = self.cBr(R,Z,grid=False)
+            result = self.cBr(R, Z, grid=False)
 
         return result
 
     def controlBz(self, R, Z):
         """
         Calculate vertical magnetic field Br at (R,Z) due to a unit current.
         """
-        
-        if isinstance(R,float) or isinstance(R,int):
-            result = self.cBz(R,Z)[0][0]
+
+        if isinstance(R, float) or isinstance(R, int):
+            result = self.cBz(R, Z)[0][0]
         else:
-            result = self.cBz(R,Z,grid=False)
+            result = self.cBz(R, Z, grid=False)
 
         return result
 
     def __repr__(self):
         return "PreCalcCoil({0}, current={1:.1f}, turns={2}, control={3})".format(
             self.shape, self.current, self.turns, self.control
         )
@@ -211,20 +224,13 @@
         RZlen = len(self.shape)
         R = np.zeros(10)
         Z = np.zeros(10)
         R[:RZlen] = [R for R, Z in self.shape]
         Z[:RZlen] = [Z for R, Z in self.shape]
 
         return np.array(
-            (
-                RZlen,
-                R,
-                Z,
-                self.current,
-                self.turns,
-                self.control
-            ),
+            (RZlen, R, Z, self.current, self.turns, self.control),
             dtype=self.dtype,
         )
 
     def __ne__(self, other):
         return not self == other
```

### Comparing `FreeGS-0.7.0/freegs/quadrature.py` & `FreeGS-0.8.0/freegs/quadrature.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.7.0/freegs/shaped_coil.py` & `FreeGS-0.8.0/freegs/shaped_coil.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 You should have received a copy of the GNU Lesser General Public License
 along with FreeGS.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 from . import quadrature
 from . import polygons
 from .gradshafranov import Greens, GreensBr, GreensBz
+from shapely.geometry import Polygon
 
 import numpy as np
 
 from .coil import Coil
 
 
 class ShapedCoil(Coil):
@@ -88,38 +89,43 @@
 
         # The quadrature points to be used
         self.npoints_per_triangle = npoints
         self._points = quadrature.polygon_quad(shape, n=npoints)
 
     def controlPsi(self, R, Z):
         """
-        Calculate poloidal flux at (R,Z) due to a unit current
+        Calculate poloidal flux at (R,Z) due to a unit current in the circuit
         """
         result = 0.0
         for R_fil, Z_fil, weight in self._points:
             result += Greens(R_fil, Z_fil, R, Z) * weight
-        return result
+        # Multiply by turns so that toroidal current is current * turns
+        return result * self.turns
 
     def controlBr(self, R, Z):
         """
         Calculate radial magnetic field Br at (R,Z) due to a unit current
         """
         result = 0.0
         for R_fil, Z_fil, weight in self._points:
             result += GreensBr(R_fil, Z_fil, R, Z) * weight
-        return result
+        return result * self.turns
 
     def controlBz(self, R, Z):
         """
         Calculate vertical magnetic field Bz at (R,Z) due to a unit current
         """
         result = 0.0
         for R_fil, Z_fil, weight in self._points:
             result += GreensBz(R_fil, Z_fil, R, Z) * weight
-        return result
+        return result * self.turns
+
+    def inShape(self,polygon):
+        Shaped_Coil = Polygon([shape for shape in self.shape])
+        return (polygon.intersection(Shaped_Coil).area) / (self._area)
 
     def __repr__(self):
         return "ShapedCoil({0}, current={1:.1f}, turns={2}, control={3})".format(
             self.shape, self.current, self.turns, self.control
         )
 
     @property
```

### Comparing `FreeGS-0.7.0/freegs/test_critical.py` & `FreeGS-0.8.0/freegs/test_critical.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.7.0/freegs/test_equilibrium.py` & `FreeGS-0.8.0/freegs/test_equilibrium.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,27 +22,28 @@
     assert Rin >= eq.Rmin and Rout >= eq.Rmin
     assert Rin <= eq.Rmax and Rout <= eq.Rmax
 
 
 def test_fixed_boundary_psi():
     # This is adapted from example 5
 
-    profiles = jtor.ConstrainPaxisIp(
-        1e3, 1e5, 1.0  # Plasma pressure on axis [Pascals]  # Plasma current [Amps]
-    )  # fvac = R*Bt
-
     eq = equilibrium.Equilibrium(
         Rmin=0.1,
         Rmax=2.0,
         Zmin=-1.0,
         Zmax=1.0,
         nx=65,
         ny=65,
         boundary=boundary.fixedBoundary,
     )
+
+    profiles = jtor.ConstrainPaxisIp(
+        eq, 1e3, 1e5, 1.0  # Plasma pressure on axis [Pascals]  # Plasma current [Amps]
+    )  # fvac = R*Bt
+
     # Nonlinear solve
     picard.solve(eq, profiles)
 
     psi = eq.psi()
     assert psi[0, 0] == 0.0  # Boundary is fixed
     assert psi[32, 32] != 0.0  # Solution is not all zero
```

### Comparing `FreeGS-0.7.0/freegs/test_linearsolve.py` & `FreeGS-0.8.0/freegs/test_linearsolve.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.7.0/freegs/test_machine.py` & `FreeGS-0.8.0/freegs/test_machine.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.7.0/freegs/test_multi_coil.py` & `FreeGS-0.8.0/freegs/test_filament_coil.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,76 +1,103 @@
-from .multi_coil import MultiCoil
+from .filament_coil import FilamentCoil
 from .coil import Coil
 from .machine import Circuit
 
 import numpy as np
 
 
 def test_single():
     """
-    Test that a single turn MultiCoil is the same as a Coil
+    Test that a single turn FilamentCoil is the same as a Coil
     """
 
-    mcoil = MultiCoil(1.1, 0.2, current=100.0, mirror=False)
-    coil = MultiCoil(1.1, 0.2, current=100.0)
+    fcoil = FilamentCoil(1.1, 0.2, current=100.0)
+    coil = Coil(1.1, 0.2, current=100.0)
 
-    assert np.isclose(coil.controlPsi(0.3, 0.1), mcoil.controlPsi(0.3, 0.1))
+    assert np.isclose(coil.controlPsi(0.3, 0.1), fcoil.controlPsi(0.3, 0.1))
 
-    assert np.isclose(coil.controlBr(0.3, 0.1), mcoil.controlBr(0.3, 0.1))
+    assert np.isclose(coil.controlBr(0.3, 0.1), fcoil.controlBr(0.3, 0.1))
 
 
-def test_two_turns():
+def test_two_filaments():
     """
-    MultiCoil with two turns same as circuit with two coils
+    FilamentCoil with two filaments same as circuit with two coils at half current
     """
 
-    mcoil = MultiCoil([1.1, 1.2], [0.2, -0.3], current=100.0, mirror=False)
+    fcoil = FilamentCoil([1.1, 1.2], [0.2, -0.3])
 
     circuit = Circuit(
         [
-            ("A", Coil(1.1, 0.2, current=100.0), 1.0),
-            ("B", Coil(1.2, -0.3, current=100.0), 1.0),
+            ("A", FilamentCoil(1.1, 0.2), 0.5),
+            ("B", FilamentCoil(1.2, -0.3), 0.5),
         ]
     )
 
-    assert np.isclose(circuit.controlPsi(0.3, 0.1), mcoil.controlPsi(0.3, 0.1))
+    # Check the Greens functions (field produced by unit circuit current)
+    assert np.isclose(circuit.controlPsi(0.3, 0.1), fcoil.controlPsi(0.3, 0.1))
+    assert np.isclose(circuit.controlBr(0.3, 0.1), fcoil.controlBr(0.3, 0.1))
+    assert np.isclose(circuit.controlBz(0.3, 0.1), fcoil.controlBz(0.3, 0.1))
+
+    # Check the field, putting the same current
+    fcoil.current = 100
+    circuit.current = 100
+    assert np.isclose(circuit.psi(0.3, 0.1), fcoil.psi(0.3, 0.1))
+    assert np.isclose(circuit.Br(0.3, 0.1), fcoil.Br(0.3, 0.1))
+    assert np.isclose(circuit.Bz(0.3, 0.1), fcoil.Bz(0.3, 0.1))
+
+
+def test_two_turns():
+    """
+    FilamentCoil with two turns same as circuit with two coils
+    """
+
+    fcoil = FilamentCoil(1.1, 1.2, turns=2)
 
-    assert np.isclose(circuit.controlBr(0.3, 0.1), mcoil.controlBr(0.3, 0.1))
+    circuit = Circuit(
+        [
+            ("A", FilamentCoil(1.1, 1.2), 1.0),
+            ("B", FilamentCoil(1.1, 1.2), 1.0),
+        ]
+    )
 
-    assert np.isclose(circuit.controlBz(0.3, 0.1), mcoil.controlBz(0.3, 0.1))
+    # Check the Greens functions (field produced by unit circuit current)
+    assert np.isclose(circuit.controlPsi(0.3, 0.1), fcoil.controlPsi(0.3, 0.1))
+    assert np.isclose(circuit.controlBr(0.3, 0.1), fcoil.controlBr(0.3, 0.1))
+    assert np.isclose(circuit.controlBz(0.3, 0.1), fcoil.controlBz(0.3, 0.1))
 
 
 def test_mirrored():
     """
-    Mirrored MultiCoil the same as two coils in a circuit
+    Mirrored FilamentCoil the same as two coils in a circuit at half current
+
+    Filaments in a FilamentCoil are wired in parallel, not in serial.
     """
-    mcoil = MultiCoil(1.1, 0.2, current=100.0, mirror=True)
+    fcoil = FilamentCoil([1.1, 1.1], [0.2, -0.2])
 
     circuit = Circuit(
         [
-            ("A", Coil(1.1, 0.2, current=100.0), 1.0),
-            ("B", Coil(1.1, -0.2, current=100.0), 1.0),
+            ("A", Coil(1.1, 0.2), 0.5),
+            ("B", Coil(1.1, -0.2), 0.5),
         ]
     )
 
-    assert np.isclose(circuit.controlPsi(0.3, 0.1), mcoil.controlPsi(0.3, 0.1))
-
-    assert np.isclose(circuit.controlBr(0.3, 0.1), mcoil.controlBr(0.3, 0.1))
-
-    assert np.isclose(circuit.controlBz(0.3, 0.1), mcoil.controlBz(0.3, 0.1))
+    # Check
+    assert np.isclose(circuit.controlPsi(0.3, 0.1), fcoil.controlPsi(0.3, 0.1))
+    assert np.isclose(circuit.controlBr(0.3, 0.1), fcoil.controlBr(0.3, 0.1))
+    assert np.isclose(circuit.controlBz(0.3, 0.1), fcoil.controlBz(0.3, 0.1))
 
 
 def test_move_R():
     """
     Changing major radius property R changes all filament locations
     """
 
     dR = 0.6
-    coil1 = MultiCoil([1.1, 0.2], [1.2, -0.3], current=100.0, mirror=False)
-    coil2 = MultiCoil([1.1 + dR, 0.2 + dR], [1.2, -0.3], current=100.0, mirror=False)
+    coil1 = FilamentCoil([1.1, 0.2], [1.2, -0.3], current=100.0)
+    coil2 = FilamentCoil([1.1 + dR, 0.2 + dR], [1.2, -0.3], current=100.0)
 
     # Shift coil1 to same location as coil2
     coil1.R += dR
 
     assert np.isclose(coil1.controlPsi(0.4, 0.5), coil2.controlPsi(0.4, 0.5))
 
     assert np.isclose(coil1.controlBr(0.3, -0.2), coil2.controlBr(0.3, -0.2))
@@ -80,16 +107,16 @@
 
 def test_move_Z():
     """
     Changing height property Z changes all filament locations
     """
 
     dZ = 0.4
-    coil1 = MultiCoil([1.1, 0.2], [1.2, -0.3], current=100.0, mirror=False)
-    coil2 = MultiCoil([1.1, 0.2], [1.2 + dZ, -0.3 + dZ], current=100.0, mirror=False)
+    coil1 = FilamentCoil([1.1, 0.2], [1.2, -0.3], current=100.0)
+    coil2 = FilamentCoil([1.1, 0.2], [1.2 + dZ, -0.3 + dZ], current=100.0)
 
     # Shift coil1 to same location as coil2
     coil1.Z += dZ
 
     assert np.isclose(coil1.controlPsi(0.4, 0.5), coil2.controlPsi(0.4, 0.5))
 
     assert np.isclose(coil1.controlBr(0.3, -0.2), coil2.controlBr(0.3, -0.2))
```

### Comparing `FreeGS-0.7.0/freegs/test_optimise.py` & `FreeGS-0.8.0/freegs/test_optimise.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.7.0/freegs/test_optimiser.py` & `FreeGS-0.8.0/freegs/test_optimiser.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from . import optimiser
 
+import numpy as np
+
 # Tests and example of solving optimisation problem
 #
 # Objects being evolved are lists of coefficients,
 # and the optimiser is minimising a polynomial (a quadratic).
 #
 # Run this script to show animation of the solution, or run
 # tests using pytest.
@@ -41,15 +43,20 @@
     # The optimiser can control two coefficients,
     # and should use calculate_score to evaluate solutions
     result = optimiser.optimise(
         start_values, [ControlIndex(0), ControlIndex(1)], calculate_score, maxgen=300
     )
 
     # Answer should be close to (1,2)
-    assert abs(result[0] - 1.0) < 1e-2 and abs(result[1] - 2.0) < 1e-2
+    expected_point = np.array((1, 2))
+    start_distance = np.sqrt(np.sum((expected_point - start_values)**2))
+    result_distance = np.sqrt(np.sum((expected_point - result)**2))
+    # It should always get _closer_, even if it doesn't get particularly close
+    assert result_distance < start_distance
+    assert np.isclose(result_distance, 0, atol=1e-1)
 
 
 def test_reducing():
     # Test that the best score never goes up
     start_values = [0.1, 0.1]  # Starting guess
 
     best_score = calculate_score(start_values)
```

### Comparing `FreeGS-0.7.0/freegs/test_polygons.py` & `FreeGS-0.8.0/freegs/test_polygons.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.7.0/freegs/test_quadrature.py` & `FreeGS-0.8.0/freegs/test_quadrature.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.7.0/freegs/test_readwrite.py` & `FreeGS-0.8.0/freegs/test_readwrite.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             Rmax=2.0,
             Zmin=-1.0,
             Zmax=1.0,
             nx=17,
             ny=17,
             boundary=freegs.boundary.freeBoundaryHagenow,
         )
-        profiles = freegs.jtor.ConstrainPaxisIp(1e4, 1e6, 2.0)
+        profiles = freegs.jtor.ConstrainPaxisIp(eq, 1e4, 1e6, 2.0)
 
         # Note here the X-point locations and isoflux locations are not the same.
         # The result will be an unbalanced double null configuration, where the
         # X-points are on different flux surfaces.
         xpoints = [(1.1, -0.6), (1.1, 0.8)]
         isoflux = [(1.1, -0.6, 1.1, 0.6)]
         constrain = freegs.control.constrain(xpoints=xpoints, isoflux=isoflux)
```

### Comparing `FreeGS-0.7.0/freegs/test_shaped_coil.py` & `FreeGS-0.8.0/freegs/test_shaped_coil.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.7.0/setup.py` & `FreeGS-0.8.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,53 @@
-from setuptools import setup
-import os
+[build-system]
+requires = [
+    "setuptools >= 61.0.0",
+    "setuptools_scm[toml] >= 6.2",
+]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "FreeGS"
+description = "Free boundary Grad-Shafranov solver for tokamak plasma equilibria"
+readme = "README.md"
+requires-python = ">=3.8"
+classifiers = [
+    "Programming Language :: Python",
+    "Development Status :: 3 - Alpha",
+    "Natural Language :: English",
+    "Intended Audience :: Science/Research",
+    "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Topic :: Scientific/Engineering :: Physics"
+]
+license = {text = "GNU Lesser General Public License v3 or later (LGPLv3+)"}
+authors = [{name = "Ben Dudson", email = "benjamin.dudson@york.ac.uk"}]
+urls = {project = "https://github.com/freegs-plasma/freegs"}
+dependencies = [
+    "numpy>=1.8",
+    "scipy>=0.14",
+    "matplotlib>=1.3",
+    "h5py>=2.10.0",
+    "Shapely>=1.7.1",
+    "importlib-metadata<4.3,>=1.1.0",
+    "freeqdsk>=0.1.0",
+]
+dynamic = ["version"]
+
+[project.optional-dependencies]
+tests = [
+    "pytest",
+]
+docs = [
+    "sphinx>=3.4,<5",
+]
 
-def read(fname):
-    return open(os.path.join(os.path.dirname(__file__), fname)).read()
+[tool.setuptools]
+packages = ["freegs"]
 
-import freegs
+[tool.setuptools.dynamic]
+version = { attr = "setuptools_scm.get_version" }
 
-setup(
-    name="FreeGS",
-    version=freegs.__version__,
-    packages=["freegs"],
-
-    license="LGPL",
-    author="Ben Dudson",
-    author_email='benjamin.dudson@york.ac.uk',
-    url="https://github.com/bendudson/freegs",
-    description="Free boundary Grad-Shafranov solver for tokamak plasma equilibria",
-
-    long_description=read("README.md"),
-    long_description_content_type="text/markdown",
-    
-    install_requires=['numpy>=1.8',
-                      'scipy>=0.14',
-                      'matplotlib>=1.3',
-                      'h5py>=2.10.0'],
-    
-    platforms='any',
-
-    classifiers = [
-        'Programming Language :: Python',
-        'Development Status :: 3 - Alpha',
-        'Natural Language :: English',
-        'Intended Audience :: Science/Research',
-        'License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        'Topic :: Scientific/Engineering :: Physics'
-        ],
-)
+[tool.setuptools_scm]
+write_to = "freegs/_version.py"
```

