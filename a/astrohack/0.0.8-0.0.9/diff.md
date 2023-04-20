# Comparing `tmp/astrohack-0.0.8.tar.gz` & `tmp/astrohack-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrohack-0.0.8.tar", last modified: Wed Apr 19 22:05:05 2023, max compression
+gzip compressed data, was "astrohack-0.0.9.tar", last modified: Thu Apr 20 15:57:58 2023, max compression
```

## Comparing `astrohack-0.0.8.tar` & `astrohack-0.0.9.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.333531 astrohack-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-19 22:04:49.000000 astrohack-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 22:04:49.000000 astrohack-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-19 22:05:05.329531 astrohack-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-19 22:04:49.000000 astrohack-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:04:49.000000 astrohack-0.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-19 22:04:49.000000 astrohack-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 22:05:05.333531 astrohack-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.321531 astrohack-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.325531 astrohack-0.0.8/src/astrohack/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.325531 astrohack-0.0.8/src/astrohack/_classes/
--rw-r--r--   0 runner    (1001) docker     (123)    27827 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_classes/antenna_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    19699 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_classes/base_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_classes/polygon_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_classes/ring_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_classes/telescope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.325531 astrohack-0.0.8/src/astrohack/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.325531 astrohack-0.0.8/src/astrohack/_utils/_dask_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_dask_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_dio.py
--rw-r--r--   0 runner    (1001) docker     (123)    16118 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_extract_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_extract_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    17045 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)    14284 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.329531 astrohack-0.0.8/src/astrohack/_utils/_logger/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_logger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4932 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_logger/_astrohack_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    28177 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_panel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.329531 astrohack-0.0.8/src/astrohack/_utils/_parm_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_parm_utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2158 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_parm_utils/_check_logger_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_parm_utils/_check_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25433 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/gaussfitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/astrohack_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.321531 astrohack-0.0.8/src/astrohack/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.329531 astrohack-0.0.8/src/astrohack/data/telescopes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.329531 astrohack-0.0.8/src/astrohack/data/telescopes/aca_7m.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/aca_7m.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.329531 astrohack-0.0.8/src/astrohack/data/telescopes/alma_da.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/alma_da.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/alma_da.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.329531 astrohack-0.0.8/src/astrohack/data/telescopes/alma_dv.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/alma_dv.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.329531 astrohack-0.0.8/src/astrohack/data/telescopes/alma_tp.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/alma_tp.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.329531 astrohack-0.0.8/src/astrohack/data/telescopes/vla.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/vla.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/vla.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/vla.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.329531 astrohack-0.0.8/src/astrohack/data/telescopes/vlba.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/vlba.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/vlba.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/vlba.zarr/.zmetadata
--rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/dio.py
--rw-r--r--   0 runner    (1001) docker     (123)    14604 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/extract_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/gdown_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11513 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/holog.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/locit.py
--rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/profiling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.329531 astrohack-0.0.8/src/astrohack/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/visualization/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.325531 astrohack-0.0.8/src/astrohack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-19 22:05:05.000000 astrohack-0.0.8/src/astrohack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-19 22:05:05.000000 astrohack-0.0.8/src/astrohack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 22:05:05.000000 astrohack-0.0.8/src/astrohack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-19 22:05:05.000000 astrohack-0.0.8/src/astrohack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-19 22:05:05.000000 astrohack-0.0.8/src/astrohack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.329531 astrohack-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-04-19 22:04:49.000000 astrohack-0.0.8/tests/test_class_antenna_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    19791 2023-04-19 22:04:49.000000 astrohack-0.0.8/tests/test_class_base_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-19 22:04:49.000000 astrohack-0.0.8/tests/test_class_ring_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-19 22:04:49.000000 astrohack-0.0.8/tests/test_class_telescope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.421033 astrohack-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-20 15:57:39.000000 astrohack-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 15:57:39.000000 astrohack-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-20 15:57:58.421033 astrohack-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-20 15:57:39.000000 astrohack-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:39.000000 astrohack-0.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-20 15:57:39.000000 astrohack-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 15:57:58.421033 astrohack-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.409033 astrohack-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.413033 astrohack-0.0.9/src/astrohack/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.413033 astrohack-0.0.9/src/astrohack/_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    27827 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_classes/antenna_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19699 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_classes/base_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_classes/polygon_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_classes/ring_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_classes/telescope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.417033 astrohack-0.0.9/src/astrohack/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.417033 astrohack-0.0.9/src/astrohack/_utils/_dask_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_dask_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_dio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16308 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_extract_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_extract_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17045 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14284 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.417033 astrohack-0.0.9/src/astrohack/_utils/_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_logger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4932 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_logger/_astrohack_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28177 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.417033 astrohack-0.0.9/src/astrohack/_utils/_parm_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_parm_utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2158 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_parm_utils/_check_logger_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_parm_utils/_check_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25433 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/gaussfitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/astrohack_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.409033 astrohack-0.0.9/src/astrohack/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.417033 astrohack-0.0.9/src/astrohack/data/telescopes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.417033 astrohack-0.0.9/src/astrohack/data/telescopes/aca_7m.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/aca_7m.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.417033 astrohack-0.0.9/src/astrohack/data/telescopes/alma_da.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/alma_da.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/alma_da.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.417033 astrohack-0.0.9/src/astrohack/data/telescopes/alma_dv.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/alma_dv.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.421033 astrohack-0.0.9/src/astrohack/data/telescopes/alma_tp.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/alma_tp.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.421033 astrohack-0.0.9/src/astrohack/data/telescopes/vla.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/vla.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/vla.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/vla.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.421033 astrohack-0.0.9/src/astrohack/data/telescopes/vlba.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/vlba.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/vlba.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/vlba.zarr/.zmetadata
+-rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/dio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14674 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/extract_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/gdown_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/locit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12842 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/profiling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.421033 astrohack-0.0.9/src/astrohack/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/visualization/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.413033 astrohack-0.0.9/src/astrohack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-20 15:57:58.000000 astrohack-0.0.9/src/astrohack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-20 15:57:58.000000 astrohack-0.0.9/src/astrohack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:57:58.000000 astrohack-0.0.9/src/astrohack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-20 15:57:58.000000 astrohack-0.0.9/src/astrohack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 15:57:58.000000 astrohack-0.0.9/src/astrohack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.421033 astrohack-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-04-20 15:57:39.000000 astrohack-0.0.9/tests/test_class_antenna_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19791 2023-04-20 15:57:39.000000 astrohack-0.0.9/tests/test_class_base_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-20 15:57:39.000000 astrohack-0.0.9/tests/test_class_ring_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-20 15:57:39.000000 astrohack-0.0.9/tests/test_class_telescope.py
```

### Comparing `astrohack-0.0.8/LICENSE` & `astrohack-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/PKG-INFO` & `astrohack-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrohack
-Version: 0.0.8
+Version: 0.0.9
 Summary: Holography Antenna Commissioning Kit
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `astrohack-0.0.8/README.md` & `astrohack-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/pyproject.toml` & `astrohack-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "astrohack"
-version = "0.0.8"
+version = "0.0.9"
 description = "Holography Antenna Commissioning Kit"
 authors = [
     {name = "Jan-Willem Steeb", email="jsteeb@nrao.edu"},
     {name = "Joshua Hoskins", email="jhoskins@nrao.edu"}, 
     {name = "Victor de Souza Magalhaes", email="vdesouza@nrao.edu"}
 ]
 license = {file = "LICENSE.txt"}
```

### Comparing `astrohack-0.0.8/src/astrohack/_classes/antenna_surface.py` & `astrohack-0.0.9/src/astrohack/_classes/antenna_surface.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/_classes/base_panel.py` & `astrohack-0.0.9/src/astrohack/_classes/base_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/_classes/polygon_panel.py` & `astrohack-0.0.9/src/astrohack/_classes/polygon_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/_classes/ring_panel.py` & `astrohack-0.0.9/src/astrohack/_classes/ring_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/_classes/telescope.py` & `astrohack-0.0.9/src/astrohack/_classes/telescope.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/_utils/_algorithms.py` & `astrohack-0.0.9/src/astrohack/_utils/_algorithms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/_utils/_constants.py` & `astrohack-0.0.9/src/astrohack/_utils/_constants.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/_utils/_conversion.py` & `astrohack-0.0.9/src/astrohack/_utils/_conversion.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py` & `astrohack-0.0.9/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py` & `astrohack-0.0.9/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/_utils/_dio.py` & `astrohack-0.0.9/src/astrohack/_utils/_dio.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/_utils/_extract_holog.py` & `astrohack-0.0.9/src/astrohack/_utils/_extract_holog.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,15 +323,15 @@
 
     coords = {"time": time_vis, "chan": chan, "pol": pol}
 
     for map_ant_index in vis_map_dict.keys():
         if map_ant_index not in flagged_mapping_antennas:
             map_ant_tag = 'ant_' + ant_names[map_ant_index] #'ant_' + str(map_ant_index)
 
-            direction = np.take(pnt_map_dict[map_ant_tag], indicies, axis=0)
+            direction = np.take(pnt_map_dict[map_ant_tag]["DIRECTIONAL_COSINES"].values, indicies, axis=0)
 
             parallactic_samples = _calculate_parallactic_angle_chunk(
                 time_samples=time_samples,
                 observing_location=observing_location[map_ant_index],
                 direction=direction
             )
 
@@ -342,15 +342,19 @@
             )
 
             xds["WEIGHT"] = xr.DataArray(
                 weight_map_dict[map_ant_index], dims=["time", "chan", "pol"]
             )
 
             xds["DIRECTIONAL_COSINES"] = xr.DataArray(
-                pnt_map_dict[map_ant_tag], dims=["time", "lm"]
+                pnt_map_dict[map_ant_tag]["DIRECTIONAL_COSINES"].values, dims=["time", "lm"]
+            )
+            
+            xds["POINTING_OFFSET"] = xr.DataArray(
+                pnt_map_dict[map_ant_tag]["POINTING_OFFSET"].values, dims=["time", "az_el"]
             )
 
             xds.attrs["holog_map_key"] = holog_map_key
             #xds.attrs["ant_id"] = map_ant_tag
             xds.attrs["ddi"] = ddi
             xds.attrs["parallactic_samples"] = parallactic_samples
             xds.attrs["telescope_name"] = telescope_name
@@ -450,11 +454,10 @@
     pnt_map_dict = {}
     
     for antenna in map_ant_ids:
         pnt_map_dict[antenna] = np.zeros((n_time_vis, 2))
         pnt_map_dict[antenna] = (
             pnt_ant_dict[antenna]
             .interp(time=time_vis, method="nearest")
-            .DIRECTIONAL_COSINES.values
         )
 
     return pnt_map_dict
```

### Comparing `astrohack-0.0.8/src/astrohack/_utils/_extract_point.py` & `astrohack-0.0.9/src/astrohack/_utils/_extract_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
     ### NB: Compare with calulation using WCS in astropy.
     l = np.cos(target[:, 1]) * np.sin(target[:, 0] - direction[:, 0])
     m = np.sin(target[:, 1]) * np.cos(direction[:, 1]) - np.cos(target[:, 1]) * np.sin(
         direction[:, 1]
     ) * np.cos(target[:, 0] - direction[:, 0])
 
     pnt_xds["DIRECTIONAL_COSINES"] = xr.DataArray(
-        np.array([l, m]).T, dims=("time", "ra_dec")
+        np.array([l, m]).T, dims=("time", "lm")
     )
     
     ###############
 
     mapping_scans = {}
     time_tree = spatial.KDTree(direction_time[:,None]) #Use for nearest interpolation
     
@@ -172,14 +172,15 @@
             sub_lm = np.abs(pnt_xds["DIRECTIONAL_COSINES"].isel(time=slice(time_index[0],time_index[1]))).mean()
             
             if sub_lm > 10**-12: #Antenna is mapping since lm is non-zero
                 scan_list.append(scan_id)
         mapping_scans[ddi_id] = scan_list
             
     pnt_xds.attrs['mapping_scans'] = [mapping_scans]
+    
     ###############
 
     pnt_xds.attrs['ant_name'] = pnt_parms['ant_name']
     
     
     logger.info(
         "Writing pointing xds to {file}".format(
```

### Comparing `astrohack-0.0.8/src/astrohack/_utils/_holog.py` & `astrohack-0.0.9/src/astrohack/_utils/_holog.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/_utils/_imaging.py` & `astrohack-0.0.9/src/astrohack/_utils/_imaging.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/_utils/_io.py` & `astrohack-0.0.9/src/astrohack/_utils/_io.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/_utils/_logger/_astrohack_logger.py` & `astrohack-0.0.9/src/astrohack/_utils/_logger/_astrohack_logger.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/_utils/_panel.py` & `astrohack-0.0.9/src/astrohack/_utils/_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/_utils/_parm_utils/_check_logger_parms.py` & `astrohack-0.0.9/src/astrohack/_utils/_parm_utils/_check_logger_parms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/_utils/_parm_utils/_check_parms.py` & `astrohack-0.0.9/src/astrohack/_utils/_parm_utils/_check_parms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/_utils/gaussfitter.py` & `astrohack-0.0.9/src/astrohack/_utils/gaussfitter.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/astrohack_client.py` & `astrohack-0.0.9/src/astrohack/astrohack_client.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs` & `astrohack-0.0.9/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata` & `astrohack-0.0.9/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/data/telescopes/alma_da.zarr/.zattrs` & `astrohack-0.0.9/src/astrohack/data/telescopes/alma_da.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata` & `astrohack-0.0.9/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs` & `astrohack-0.0.9/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata` & `astrohack-0.0.9/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs` & `astrohack-0.0.9/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata` & `astrohack-0.0.9/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/data/telescopes/vla.zarr/.zattrs` & `astrohack-0.0.9/src/astrohack/data/telescopes/vla.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/data/telescopes/vla.zarr/.zmetadata` & `astrohack-0.0.9/src/astrohack/data/telescopes/vla.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/data/telescopes/vlba.zarr/.zattrs` & `astrohack-0.0.9/src/astrohack/data/telescopes/vlba.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/data/telescopes/vlba.zarr/.zmetadata` & `astrohack-0.0.9/src/astrohack/data/telescopes/vlba.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/dio.py` & `astrohack-0.0.9/src/astrohack/dio.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/extract_holog.py` & `astrohack-0.0.9/src/astrohack/extract_holog.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,17 @@
 
     :param parallel: Boolean for whether to process in parallel. Defaults to False
     :type parallel: bool, optional
 
     :param overwrite: Boolean for whether to overwrite current holog.zarr and point.zarr files., defaults to False
     :type overwrite: bool, optional
 
+    :return: Holography holog object.
+    :rtype: AstrohackHologFile
+
     .. _Description:
 
     **Additional Information**
 
         This function extracts the holography related information from the given measurement file. The data is restructured into an astrohack file format and saved into a file in the form of *<holog_name>.holog.zarr*. The extension *.holog.zarr* is used for all holography files. In addition, the pointing information is recorded into a holography file of format *<pointing_name>.point.zarr*. The extension *.point.zarr* is used for all holography pointing files. 
 
         **holog_obs_dict[holog_mapping_id] (dict):**
```

### Comparing `astrohack-0.0.8/src/astrohack/gdown_utils.py` & `astrohack-0.0.9/src/astrohack/gdown_utils.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/holog.py` & `astrohack-0.0.9/src/astrohack/holog.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,17 @@
         - [4]: cassegrain offset
 
     :type phase_fit: bool, optional
 
     :param overwrite: Overwrite existing files on disk, defaults to False
     :type overwrite: bool, optional
 
+    :return: Holography image object.
+    :rtype: AstrohackImageFile
+
     """
     
     logger = _get_astrohack_logger()
     
     holog_params = _check_holog_parms(
         holog_name, 
         grid_size,
```

### Comparing `astrohack-0.0.8/src/astrohack/panel.py` & `astrohack-0.0.9/src/astrohack/panel.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,17 @@
     :param parallel: Run in parallel. Defaults to False.
     :type parallel: bool, optional
     :param sel_ddi: List of DDIs to be processed. None will use all DDIs. Defaults to None.
     :type sel_ddi: list, optional
     :param overwrite: Overwrite files on disk. Defaults to False.
     :type overwrite: bool, optional
 
+    :return: Holography panel object.
+    :rtype: AstrohackPanelFile
+
     .. _Description:
 
     **Additional Information**
         Each holography in the input holog image file is processed in the following steps:
         
         .. rubric:: Code Outline
         - Phase image is converted to a physical surface deviation image.
```

### Comparing `astrohack-0.0.8/src/astrohack/profiling.py` & `astrohack-0.0.9/src/astrohack/profiling.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack/visualization/viewer.py` & `astrohack-0.0.9/src/astrohack/visualization/viewer.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack.egg-info/PKG-INFO` & `astrohack-0.0.9/src/astrohack.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrohack
-Version: 0.0.8
+Version: 0.0.9
 Summary: Holography Antenna Commissioning Kit
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `astrohack-0.0.8/src/astrohack.egg-info/SOURCES.txt` & `astrohack-0.0.9/src/astrohack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/src/astrohack.egg-info/requires.txt` & `astrohack-0.0.9/src/astrohack.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/tests/test_class_antenna_surface.py` & `astrohack-0.0.9/tests/test_class_antenna_surface.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/tests/test_class_base_panel.py` & `astrohack-0.0.9/tests/test_class_base_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/tests/test_class_ring_panel.py` & `astrohack-0.0.9/tests/test_class_ring_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.8/tests/test_class_telescope.py` & `astrohack-0.0.9/tests/test_class_telescope.py`

 * *Files identical despite different names*

