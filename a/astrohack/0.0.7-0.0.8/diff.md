# Comparing `tmp/astrohack-0.0.7.tar.gz` & `tmp/astrohack-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrohack-0.0.7.tar", last modified: Mon Apr 17 18:01:16 2023, max compression
+gzip compressed data, was "astrohack-0.0.8.tar", last modified: Wed Apr 19 22:05:05 2023, max compression
```

## Comparing `astrohack-0.0.7.tar` & `astrohack-0.0.8.tar`

### file list

```diff
@@ -1,87 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.481204 astrohack-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-17 18:00:59.000000 astrohack-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 18:00:59.000000 astrohack-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-17 18:01:16.477204 astrohack-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-17 18:00:59.000000 astrohack-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:00:59.000000 astrohack-0.0.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-17 18:00:59.000000 astrohack-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 18:01:16.481204 astrohack-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.469204 astrohack-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.473204 astrohack-0.0.7/src/astrohack/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.473204 astrohack-0.0.7/src/astrohack/_classes/
--rw-r--r--   0 runner    (1001) docker     (123)    27476 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_classes/antenna_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    19699 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_classes/base_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_classes/polygon_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_classes/ring_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_classes/telescope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.473204 astrohack-0.0.7/src/astrohack/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.473204 astrohack-0.0.7/src/astrohack/_utils/_dask_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_dask_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_dio_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    19092 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)    33916 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.477204 astrohack-0.0.7/src/astrohack/_utils/_logger/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_logger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4932 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_logger/_astrohack_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    27130 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_panel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.477204 astrohack-0.0.7/src/astrohack/_utils/_parm_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_parm_utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2158 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_parm_utils/_check_logger_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_parm_utils/_check_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25433 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/gaussfitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/astrohack_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.469204 astrohack-0.0.7/src/astrohack/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.477204 astrohack-0.0.7/src/astrohack/data/telescopes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.477204 astrohack-0.0.7/src/astrohack/data/telescopes/aca_7m.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/aca_7m.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.477204 astrohack-0.0.7/src/astrohack/data/telescopes/alma_da.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/alma_da.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/alma_da.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.477204 astrohack-0.0.7/src/astrohack/data/telescopes/alma_dv.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/alma_dv.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.477204 astrohack-0.0.7/src/astrohack/data/telescopes/alma_tp.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/alma_tp.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.477204 astrohack-0.0.7/src/astrohack/data/telescopes/vla.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/vla.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/vla.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/vla.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.477204 astrohack-0.0.7/src/astrohack/data/telescopes/vlba.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/vlba.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/vlba.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/vlba.zarr/.zmetadata
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/dio.py
--rw-r--r--   0 runner    (1001) docker     (123)    15467 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/extract_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/gdown_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/holog.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/locit.py
--rw-r--r--   0 runner    (1001) docker     (123)    12796 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/profiling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.477204 astrohack-0.0.7/src/astrohack/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/visualization/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.473204 astrohack-0.0.7/src/astrohack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-17 18:01:16.000000 astrohack-0.0.7/src/astrohack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-17 18:01:16.000000 astrohack-0.0.7/src/astrohack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 18:01:16.000000 astrohack-0.0.7/src/astrohack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-17 18:01:16.000000 astrohack-0.0.7/src/astrohack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 18:01:16.000000 astrohack-0.0.7/src/astrohack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.477204 astrohack-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    19791 2023-04-17 18:00:59.000000 astrohack-0.0.7/tests/test_class_base_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-17 18:00:59.000000 astrohack-0.0.7/tests/test_class_ring_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.333531 astrohack-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-19 22:04:49.000000 astrohack-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 22:04:49.000000 astrohack-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-19 22:05:05.329531 astrohack-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-19 22:04:49.000000 astrohack-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:04:49.000000 astrohack-0.0.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-19 22:04:49.000000 astrohack-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 22:05:05.333531 astrohack-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.321531 astrohack-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.325531 astrohack-0.0.8/src/astrohack/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.325531 astrohack-0.0.8/src/astrohack/_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    27827 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_classes/antenna_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19699 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_classes/base_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_classes/polygon_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_classes/ring_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_classes/telescope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.325531 astrohack-0.0.8/src/astrohack/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.325531 astrohack-0.0.8/src/astrohack/_utils/_dask_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_dask_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_dio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16118 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_extract_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_extract_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17045 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14284 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.329531 astrohack-0.0.8/src/astrohack/_utils/_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_logger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4932 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_logger/_astrohack_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28177 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.329531 astrohack-0.0.8/src/astrohack/_utils/_parm_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_parm_utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2158 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_parm_utils/_check_logger_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_parm_utils/_check_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25433 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/_utils/gaussfitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/astrohack_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.321531 astrohack-0.0.8/src/astrohack/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.329531 astrohack-0.0.8/src/astrohack/data/telescopes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.329531 astrohack-0.0.8/src/astrohack/data/telescopes/aca_7m.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/aca_7m.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.329531 astrohack-0.0.8/src/astrohack/data/telescopes/alma_da.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/alma_da.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/alma_da.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.329531 astrohack-0.0.8/src/astrohack/data/telescopes/alma_dv.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/alma_dv.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.329531 astrohack-0.0.8/src/astrohack/data/telescopes/alma_tp.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/alma_tp.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.329531 astrohack-0.0.8/src/astrohack/data/telescopes/vla.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/vla.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/vla.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/vla.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.329531 astrohack-0.0.8/src/astrohack/data/telescopes/vlba.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/vlba.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/vlba.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/data/telescopes/vlba.zarr/.zmetadata
+-rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/dio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14604 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/extract_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/gdown_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11513 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/locit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/profiling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.329531 astrohack-0.0.8/src/astrohack/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-19 22:04:49.000000 astrohack-0.0.8/src/astrohack/visualization/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.325531 astrohack-0.0.8/src/astrohack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-19 22:05:05.000000 astrohack-0.0.8/src/astrohack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-19 22:05:05.000000 astrohack-0.0.8/src/astrohack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 22:05:05.000000 astrohack-0.0.8/src/astrohack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-19 22:05:05.000000 astrohack-0.0.8/src/astrohack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-19 22:05:05.000000 astrohack-0.0.8/src/astrohack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:05.329531 astrohack-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-04-19 22:04:49.000000 astrohack-0.0.8/tests/test_class_antenna_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19791 2023-04-19 22:04:49.000000 astrohack-0.0.8/tests/test_class_base_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-19 22:04:49.000000 astrohack-0.0.8/tests/test_class_ring_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-19 22:04:49.000000 astrohack-0.0.8/tests/test_class_telescope.py
```

### Comparing `astrohack-0.0.7/LICENSE` & `astrohack-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.7/PKG-INFO` & `astrohack-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrohack
-Version: 0.0.7
+Version: 0.0.8
 Summary: Holography Antenna Commissioning Kit
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `astrohack-0.0.7/README.md` & `astrohack-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.7/pyproject.toml` & `astrohack-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "astrohack"
-version = "0.0.7"
+version = "0.0.8"
 description = "Holography Antenna Commissioning Kit"
 authors = [
     {name = "Jan-Willem Steeb", email="jsteeb@nrao.edu"},
     {name = "Joshua Hoskins", email="jhoskins@nrao.edu"}, 
     {name = "Victor de Souza Magalhaes", email="vdesouza@nrao.edu"}
 ]
 license = {file = "LICENSE.txt"}
```

### Comparing `astrohack-0.0.7/src/astrohack/_classes/antenna_surface.py` & `astrohack-0.0.8/src/astrohack/_classes/antenna_surface.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             if inputxds.dims['chan'] != 1:
                 raise Exception("Only single channel holographies supported")
             self.wavelength = clight / inputxds.chan.values[0]
         else:
             self.wavelength = inputxds.attrs['wavelength']
 
         self.amplitude = inputxds["AMPLITUDE"].values[0, 0, 0, :, :]
-        self.phase = inputxds["ANGLE"].values[0, 0, 0, :, :]
+        self.phase = inputxds["CORRECTED_PHASE"].values[0, 0, 0, :, :]
 
         self.npoint = np.sqrt(inputxds.dims['l'] ** 2 + inputxds.dims['m'] ** 2)
         self.amp_unit = 'V'
         self.u_axis = inputxds.u_prime.values * self.wavelength
         self.v_axis = inputxds.v_prime.values * self.wavelength
         self.computephase = False
 
@@ -98,14 +98,15 @@
         # Arrays
         self.amplitude = inputxds['AMPLITUDE'].values
         self.phase = inputxds['PHASE'].values
         self.deviation = inputxds['DEVIATION'].values
         self.mask = inputxds['MASK']
         self.u_axis = inputxds.u.values
         self.v_axis = inputxds.u.values
+        self.panel_distribution = inputxds['PANEL_DISTRIBUTION'].values
 
         if self.solved:
             self.phase_residuals = inputxds['PHASE_RESIDUALS'].values
             self.residuals = inputxds['RESIDUALS'].values
             self.phase_corrections = inputxds['PHASE_CORRECTIONS'].values
             self.corrections = inputxds['CORRECTIONS'].values
             self.panel_pars = inputxds['PANEL_PARAMETERS'].values
@@ -573,15 +574,19 @@
         """
         Export screw adjustments for all panels onto an ASCII file
         Args:
             filename: ASCII file name/path
             unit: unit for panel screw adjustments ['mm','miliinches']
         """
         outfile = "Screw adjustments for {0:s} {1:s} antenna\n".format(self.telescope.name, self.antenna_name)
-        outfile += "Adjustments are in " + unit + lnbr
+        outfile += "Adjustments are in " + unit + 2*lnbr
+        outfile += "Lower means away from subreflector" + lnbr
+        outfile += "Raise means toward the subreflector" + lnbr
+        outfile += "LOWER the panel if the number is POSITIVE" + lnbr
+        outfile += "RAISE the panel if the number is NEGATIVE" + lnbr
         outfile += 2 * lnbr
         outfile += "{0:8s}".format('Panel')
         nscrews = len(self.telescope.screw_description)
         for screw in self.telescope.screw_description:
             outfile += "{0:11s}".format(screw)
         outfile += lnbr
         fac = _convert_unit('m', unit, 'length')
```

### Comparing `astrohack-0.0.7/src/astrohack/_classes/base_panel.py` & `astrohack-0.0.8/src/astrohack/_classes/base_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.7/src/astrohack/_classes/polygon_panel.py` & `astrohack-0.0.8/src/astrohack/_classes/polygon_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.7/src/astrohack/_classes/ring_panel.py` & `astrohack-0.0.8/src/astrohack/_classes/ring_panel.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 from matplotlib import pyplot as plt
 from astrohack._classes.base_panel import BasePanel
+from astrohack._utils._constants import twopi
 
 
 class RingPanel(BasePanel):
     # This class describes and treats panels that are arranged in
     # rings on the Antenna surface
 
     def __init__(self, kind, angle, ipanel, label, inrad, ourad, margin=0.20, screw_scheme=None, screw_offset=None):
@@ -67,27 +68,24 @@
         nscrews = len(scheme)
         screws = np.ndarray([nscrews, 2])
 
         for iscrew in range(nscrews):
             if scheme[iscrew] == 'c':
                 screws[iscrew, :] = self.center
             else:
-                if scheme[iscrew][1] == 'l':
-                    screws[iscrew, :] = np.cos(self.theta1), np.sin(self.theta1)
-                    xoff = offset
-                else:
-                    screws[iscrew, :] = np.cos(self.theta2), np.sin(self.theta2)
-                    xoff = -offset
                 if scheme[iscrew][0] == 'i':
-                    screws[iscrew, :] *= self.inrad
-                    yoff = offset
+                    radius = self.inrad + offset
+                else:
+                    radius = self.ourad - offset
+                deltatheta = offset / radius
+                if scheme[iscrew][1] == 'l':
+                    theta = self.theta1 + deltatheta
                 else:
-                    screws[iscrew, :] *= self.ourad
-                    yoff = -offset
-                screws[iscrew, :] += xoff, yoff
+                    theta = self.theta2 - deltatheta
+                screws[iscrew] = radius*np.cos(theta), radius*np.sin(theta)
         return screws
 
     def is_inside(self, rad, phi):
         """
         Check if a point is inside a panel using polar coordinates
         Args:
             rad: radius of the point
```

### Comparing `astrohack-0.0.7/src/astrohack/_classes/telescope.py` & `astrohack-0.0.8/src/astrohack/_classes/telescope.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.7/src/astrohack/_utils/_algorithms.py` & `astrohack-0.0.8/src/astrohack/_utils/_algorithms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.7/src/astrohack/_utils/_constants.py` & `astrohack-0.0.8/src/astrohack/_utils/_constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,7 +30,10 @@
 twopi = 2.0*constants.pi
 fourpi = 4.0*constants.pi
 
 # https://github.com/casacore/casacore/blob/dbf28794ef446bbf4e6150653dbe404379a3c429/measures/Measures/Stokes.h
 pol_codes_RL = np.array([5, 6, 7, 8]) #'RR','RL','LR','LL'
 pol_codes_XY = np.array([9, 10, 11, 12]) #['XX','XY','YX','YY']
 pol_str = np.array(['0','I','Q','U','V','RR','RL','LR','LL','XX','XY','YX','YY'])
+
+#Plot types
+plot_types = ['deviation', 'phase', 'ancillary']
```

### Comparing `astrohack-0.0.7/src/astrohack/_utils/_conversion.py` & `astrohack-0.0.8/src/astrohack/_utils/_conversion.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.7/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py` & `astrohack-0.0.8/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.7/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py` & `astrohack-0.0.8/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.7/src/astrohack/_utils/_dio_classes.py` & `astrohack-0.0.8/src/astrohack/_utils/_dio.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,57 +3,73 @@
 from astrohack._utils._io import _load_image_xds
 from prettytable import PrettyTable
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 from astrohack._utils._io import _read_meta_data
 from astrohack._utils._io import _load_holog_file
 from astrohack._utils._io import _load_image_file
 from astrohack._utils._io import _load_panel_file
+from astrohack._utils._io import _load_point_file
 
 from astrohack._classes.antenna_surface import AntennaSurface
 from astrohack._classes.telescope import Telescope
 
 
 class AstrohackDataFile:
     def __init__(self, file_stem, path='./'):
                         
         self._image_path = None
         self._holog_path = None
+        self._panel_path = None
+        self._point_path = None
 
         self.holog = None
         self.image = None
+        self.panel = None
+        self.point = None
             
         self._verify_holog_files(file_stem, path)
             
 
     def _verify_holog_files(self, file_stem, path):
         logger = _get_astrohack_logger()
         logger.info("Verifying {stem}.* files in path={path} ...".format(stem=file_stem, path=path))
 
         file_path = "{path}/{stem}.holog.zarr".format(path=path, stem=file_stem)
             
         if os.path.isdir(file_path):
             logger.info("Found {stem}.holog.zarr directory ...".format(stem=file_stem))
+            
             self._holog_path = file_path
             self.holog = AstrohackHologFile(file_path)
                 
 
         file_path = "{path}/{stem}.image.zarr".format(path=path, stem=file_stem)
 
         if os.path.isdir(file_path):
             logger.info("Found {stem}.image.zarr directory ...".format(stem=file_stem))
+            
             self._image_path = file_path
             self.image = AstrohackImageFile(file_path)
 
         file_path = "{path}/{stem}.panel.zarr".format(path=path, stem=file_stem)
 
         if os.path.isdir(file_path):
             logger.info("Found {stem}.panel.zarr directory ...".format(stem=file_stem))
+            
             self._image_path = file_path
             self.panel = AstrohackPanelFile(file_path)
 
+        file_path = "{path}/{stem}.point.zarr".format(path=path, stem=file_stem)
+
+        if os.path.isdir(file_path):
+            logger.info("Found {stem}.point.zarr directory ...".format(stem=file_stem))
+            
+            self._point_path = file_path
+            self.point = AstrohackPointFile(file_path)
+
 class AstrohackImageFile(dict):
     """
         Data class for holography image data.
     """
     def __init__(self, file):
         super().__init__()
 
@@ -67,18 +83,16 @@
         return super().__setitem__(key, value)
         
     def is_open(self):
         return self._open
 
     def open(self, file=None):
         """ Open hologgraphy file.
-
         Args:self =_
             file (str, optional): Path to holography file. Defaults to None.
-
         Returns:
             bool: bool describing whether the file was opened properly
         """
         logger = _get_astrohack_logger()
         if file is None:
             file = self.file
         
@@ -106,19 +120,17 @@
             table.add_row([ant, list(self[ant].keys())])
         
         print(table)
 
 
     def select(self, ant=None, ddi=None, polar=False):
         """Select data on the basis of ddi, scan, ant. This is a convenience function.
-
         Args:
             ddi (int, optional): Data description ID. Defaults to None.
             ant (int, optional): Antenna ID. Defaults to None.
-
         Returns:
             xarray.Dataset: xarray dataset of corresponding ddi, scan, antenna ID.
         """
         logger = _get_astrohack_logger()
         
         if ant is None and ddi is None:
             logger.info("No selections made ...")
@@ -148,19 +160,17 @@
         return super().__setitem__(key, value)
 
     def is_open(self):
         return self._open
 
     def open(self, file=None, dask_load=False):
         """ Open hologgraphy file.
-
         Args:self =_
             file (str, optional): Path to holography file. Defaults to None.
             dask_load (bool, optional): If True the file is loaded with Dask. Defaults to False.
-
         Returns:
             bool: bool describing whether the file was opened properly
         """
         logger = _get_astrohack_logger()
 
         if file is None:
             file = self.file
@@ -179,46 +189,43 @@
 
     def summary(self):
         """
             Prints summary table of holog file.
         """
 
         table = PrettyTable()
-        table.field_names = ["ddi", "scan", "antenna"]
+        table.field_names = ["ddi", "map", "antenna"]
         table.align = "l"
         
         for ddi in self.keys():
             for scan in self[ddi].keys():
                 table.add_row([ddi, scan, list(self[ddi][scan].keys())])
         
         print(table)
 
     def select(self, ddi=None, scan=None, ant=None):
         """ Select data on the basis of ddi, scan, ant. This is a convenience function.
-
         Args:
             ddi (int, optional): Data description ID. Defaults to None.
             scan (int, optional): Scan number. Defaults to None.
             ant (int, optional): Antenna ID. Defaults to None.
-
         Returns:
             xarray.Dataset: xarray dataset of corresponding ddi, scan, antenna ID.
         """
         logger = _get_astrohack_logger()
         
         if ant is None or ddi is None or scan is None:
             logger.info("No selections made ...")
             return self
         else:
             return self[ddi][scan][ant]
 
     @property
     def meta_data(self):
         """ Holog file meta data.
-
         Returns:
             JSON: JSON file of holography meta data.
         """
 
         return self._meta_data
 
 class AstrohackPanelFile(dict):
@@ -238,18 +245,16 @@
         return super().__setitem__(key, value)
         
     def is_open(self):
         return self._open
 
     def open(self, file=None):
         """ Open panel file.
-
         Args:self =_
             file (str, optional): Path to holography file. Defaults to None.
-
         Returns:
             bool: bool describing whether the file was opened properly
         """
         logger = _get_astrohack_logger()
 
         if file is None:
             file = self.file
@@ -275,20 +280,79 @@
         table.align = "l"
         
         for ant in self.keys():
             table.add_row([ant, list(self[ant].keys())])
         
         print(table)
 
-    def review_antenna(self, antenna, ddi):
+    def get_antenna(self, antenna, ddi):
         """
         Return an AntennaSurface object for interaction
         Args:
             antenna: Which antenna in to be used
             ddi: Which ddi is to be used
-
         Returns:
             AntennaSurface object contaning relevant information for panel adjustments
         """
         xds = _load_image_xds(self.file, antenna, ddi)
         telescope = Telescope(xds.attrs['telescope_name'])
+        
         return AntennaSurface(xds, telescope, reread=True)
+
+
+class AstrohackPointFile(dict):
+    """
+        Data Class to interact ith holography pointing data.
+    """
+    def __init__(self, file):
+        super().__init__()
+        
+        self.file = file
+        self._meta_data = None
+        self._open = False
+
+
+    def __getitem__(self, key):
+        return super().__getitem__(key)
+    
+    def __setitem__(self, key, value):
+        return super().__setitem__(key, value)
+
+    def is_open(self):
+        return self._open
+
+    def open(self, file=None, dask_load=False):
+        """ Open pointing file.
+        Args:self =_
+            file (str, optional): Path to pointing file. Defaults to None.
+            dask_load (bool, optional): If True the file is loaded with Dask. Defaults to False.
+        Returns:
+            bool: bool describing whether the file was opened properly
+        """
+        logger = _get_astrohack_logger()
+
+        if file is None:
+            file = self.file
+
+        try:
+            _load_point_file(file=file, dask_load=dask_load, pnt_dict=self)
+            self._open = True
+
+        except Exception as e:
+            logger.error("[AstrohackPointFile]: {}".format(e))
+            self._open = False
+        
+        return self._open
+
+    def summary(self):
+        """
+            Prints summary table of pointing file.
+        """
+
+        table = PrettyTable()
+        table.field_names = ["antenna"]
+        table.align = "l"
+        
+        for ant in self.keys():
+            table.add_row(ant)
+        
+        print(table)
```

### Comparing `astrohack-0.0.7/src/astrohack/_utils/_holog.py` & `astrohack-0.0.8/src/astrohack/_utils/_holog.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 from scipy.interpolate import griddata
 from casacore import tables as ctables
 
 from astrohack._classes.telescope import Telescope
 
 from astrohack._utils._io import _load_holog_file
 from astrohack._utils._io import _read_meta_data
-from astrohack._utils._io import _extract_scan_time_dict
-from astrohack._utils._io import _make_ant_pnt_chunk
-from astrohack._utils._io import _load_pnt_dict
+from astrohack._utils._io import _load_point_file
 
 from astrohack._utils._panel import _phase_fitting_block
 
 from astrohack._utils._algorithms import _chunked_average
 from astrohack._utils._algorithms import _find_peak_beam_value
 from astrohack._utils._algorithms import _find_nearest
 from astrohack._utils._algorithms import _calc_coords
@@ -28,14 +26,15 @@
 
 from astrohack._utils._imaging import _parallactic_derotation
 from astrohack._utils._imaging import _mask_circular_disk
 from astrohack._utils._imaging import _calculate_aperture_pattern
 
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 
+from numba import njit
 
 def _holog_chunk(holog_chunk_params):
     """ Process chunk holography data along the antenna axis. Works with holography file to properly grid , normalize, average and correct data
         and returns the aperture pattern.
 
     Args:
         holog_chunk_params (dict): Dictionary containing holography parameters.
@@ -279,15 +278,15 @@
     ###To Do: Add Paralactic angle as a non-dimension coordinate dependant on time.
     xds = xr.Dataset()
 
     xds["BEAM"] = xr.DataArray(beam_grid, dims=["time", "chan", "pol", "l", "m"])
     xds["APERTURE"] = xr.DataArray(aperture_grid, dims=["time", "chan", "pol", "u", "v"])
     
     xds["AMPLITUDE"] = xr.DataArray(amplitude, dims=["time", "chan", "pol", "u_prime", "v_prime"])
-    xds["ANGLE"] = xr.DataArray(phase_corrected_angle, dims=["time", "chan", "pol", "u_prime", "v_prime"])
+    xds["CORRECTED_PHASE"] = xr.DataArray(phase_corrected_angle, dims=["time", "chan", "pol", "u_prime", "v_prime"])
 
     xds.attrs["ant_id"] = holog_chunk_params["ant_id"]
     xds.attrs["ant_name"] = ant_name
     xds.attrs["telescope_name"] = meta_data['telescope_name']
     xds.attrs["time_centroid"] = np.array(time_centroid)
     xds.attrs["ddi"] = ddi
 
@@ -430,75 +429,7 @@
     try:
         with open(output_meta_file, "w") as json_file:
             json.dump(ant_holog_dict, json_file)
 
     except Exception as error:
         logger.error("[_create_holog_meta_data] {error}".format(error=error))
 
-def _make_ant_pnt_dict(ms_name, pnt_name, parallel=True):
-    """Top level function to extract subset of pointing table data into a dictionary of xarray dataarrays.
-
-    Args:
-        ms_name (str): Measurement file name.
-        pnt_name (str): Output pointing dictionary file name.
-        parallel (bool, optional): Process in parallel. Defaults to True.
-
-    Returns:
-        dict: pointing dictionary of xarray dataarrays
-    """
-
-    #Get antenna names and ids
-    ctb = ctables.table(
-        os.path.join(ms_name, "ANTENNA"),
-        readonly=True,
-        lockoptions={"option": "usernoread"},
-    )
-
-    antenna_name = ctb.getcol("NAME")
-    antenna_id = np.arange(len(antenna_name))
-
-    ctb.close()
-    
-
-    
-    ###########################################################################################
-    #Get scans with start and end times.
-    ctb = ctables.table(
-        ms_name,
-        readonly=True,
-        lockoptions={"option": "usernoread"},
-    )
-
-    scan_ids = ctb.getcol("SCAN_NUMBER")
-    time = ctb.getcol("TIME")
-    ddi = ctb.getcol("DATA_DESC_ID")
-    ctb.close()
-
-    scan_time_dict = _extract_scan_time_dict(time, scan_ids, ddi)
-    ###########################################################################################
-    pnt_parms = {
-        'pnt_name': pnt_name,
-        'scan_time_dict': scan_time_dict
-    }
-
-    if parallel:
-        delayed_pnt_list = []
-        for id in antenna_id:
-            pnt_parms['ant_id'] = id
-            pnt_parms['ant_name'] = antenna_name[id]
-
-            delayed_pnt_list.append(
-                dask.delayed(_make_ant_pnt_chunk)(
-                    ms_name, 
-                    pnt_parms
-                )
-            )
-        dask.compute(delayed_pnt_list)
-    else:
-        for id in antenna_id:
-            pnt_parms['ant_id'] = id
-            pnt_parms['ant_name'] = antenna_name[id]
-
-            _make_ant_pnt_chunk(ms_name, pnt_parms)
-
-    return _load_pnt_dict(pnt_name)
-
```

### Comparing `astrohack-0.0.7/src/astrohack/_utils/_imaging.py` & `astrohack-0.0.8/src/astrohack/_utils/_imaging.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.7/src/astrohack/_utils/_logger/_astrohack_logger.py` & `astrohack-0.0.8/src/astrohack/_utils/_logger/_astrohack_logger.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.7/src/astrohack/_utils/_panel.py` & `astrohack-0.0.8/src/astrohack/_utils/_panel.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 
 from numba import njit
 
 from astrohack._utils._conversion import _convert_unit
 from astrohack._utils._algorithms import _least_squares_fit_block
+from astrohack._utils._constants import plot_types
 
 # global constants
 NPAR = 10
 
 
 def _phase_fitting_block(pols, wavelength, telescope, cellxy, amplitude_image, phase_image, pointing_offset,
                          focus_xy_offsets, focus_z_offset, subreflector_tilt, cassegrain_offset):
@@ -560,7 +561,26 @@
     ntime, nchan, npol = phase_image.shape[:3]
     rms = np.zeros((ntime, nchan, npol))
     for time in range(ntime):
         for chan in range(nchan):
             for pol in range(npol):
                 rms[time, chan, pol] = np.sqrt(np.nanmean(phase_image[time, chan, pol] ** 2))
     return rms
+
+def _plot_antenna_chunk(parm_dict):
+    antenna = parm_dict['this_antenna']
+    ddi = parm_dict['this_ddi']
+    destination = parm_dict['destination']
+    plot_type = parm_dict['plot_type']
+    plot_name = f'{destination}/{plot_type}_{antenna}_{ddi}.png'
+
+    surface = parm_dict['panel_mds'].get_antenna(antenna, ddi)
+    if plot_type == plot_types[0]:  # deviation plot
+        surface.plot_surface(filename=plot_name, mask=False, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'],
+                             plotphase=False, unit=parm_dict['unit'])
+    elif plot_type == plot_types[1]:  # phase plot
+        surface.plot_surface(filename=plot_name, mask=False, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'],
+                             plotphase=True, unit=parm_dict['unit'])
+    else:  # Ancillary plot
+        surface.plot_surface(filename=plot_name, mask=True, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'],
+                             plotphase=False, unit=None)
+
```

### Comparing `astrohack-0.0.7/src/astrohack/_utils/_parm_utils/_check_logger_parms.py` & `astrohack-0.0.8/src/astrohack/_utils/_parm_utils/_check_logger_parms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.7/src/astrohack/_utils/_parm_utils/_check_parms.py` & `astrohack-0.0.8/src/astrohack/_utils/_parm_utils/_check_parms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.7/src/astrohack/_utils/gaussfitter.py` & `astrohack-0.0.8/src/astrohack/_utils/gaussfitter.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.7/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs` & `astrohack-0.0.8/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.7/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata` & `astrohack-0.0.8/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.7/src/astrohack/data/telescopes/alma_da.zarr/.zattrs` & `astrohack-0.0.8/src/astrohack/data/telescopes/alma_da.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.7/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata` & `astrohack-0.0.8/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.7/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs` & `astrohack-0.0.8/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.7/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata` & `astrohack-0.0.8/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.7/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs` & `astrohack-0.0.8/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.7/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata` & `astrohack-0.0.8/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.7/src/astrohack/data/telescopes/vla.zarr/.zattrs` & `astrohack-0.0.8/src/astrohack/data/telescopes/vla.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.7/src/astrohack/data/telescopes/vla.zarr/.zmetadata` & `astrohack-0.0.8/src/astrohack/data/telescopes/vla.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.7/src/astrohack/data/telescopes/vlba.zarr/.zattrs` & `astrohack-0.0.8/src/astrohack/data/telescopes/vlba.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.7/src/astrohack/data/telescopes/vlba.zarr/.zmetadata` & `astrohack-0.0.8/src/astrohack/data/telescopes/vlba.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.7/src/astrohack/extract_holog.py` & `astrohack-0.0.8/src/astrohack/extract_holog.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,31 +8,33 @@
 from casacore import tables as ctables
 
 from astrohack._utils._constants import pol_str
 
 from astrohack._utils._conversion import _convert_ant_name_to_id
 
 from astrohack._utils._holog import _create_holog_meta_data
-from astrohack._utils._holog import _make_ant_pnt_dict
 
-from astrohack._utils._io import _load_pnt_dict 
-from astrohack._utils._io import _extract_holog_chunk 
+from astrohack._utils._extract_point import _extract_pointing
+
+from astrohack._utils._io import _load_point_file
 from astrohack._utils._io import _open_no_dask_zarr
 from astrohack._utils._io import _read_data_from_holog_json
 from astrohack._utils._io import _read_meta_data
 from astrohack._utils._io import _load_holog_file
 from astrohack._utils._io import  check_if_file_will_be_overwritten,check_if_file_exists
 
+from astrohack._utils._extract_holog import _extract_holog_chunk
+
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 from astrohack._utils._parm_utils._check_parms import _check_parms
 from astrohack._utils._utils import _remove_suffix
 from astrohack._utils._io import _load_holog_file
 
 
-from astrohack._utils._dio_classes import AstrohackHologFile
+from astrohack._utils._dio import AstrohackHologFile
 def extract_holog(
     ms_name,
     holog_obs_dict,
     holog_name=None,
     point_name=None,
     data_col="DATA",
     parallel=False,
@@ -105,60 +107,40 @@
             }
             holog_obs_description['ddi'] = [0]
 
     """
     logger = _get_astrohack_logger()
     
     
+    ######### Parameter Checking #########
     extract_holog_parms = _check_extract_holog_parms(ms_name,
                                 holog_obs_dict,
                                 holog_name,
                                 point_name,
                                 data_col,
                                 parallel,
                                 overwrite)
     
     check_if_file_exists(extract_holog_parms['ms_name'])
     check_if_file_will_be_overwritten(extract_holog_parms['holog_name'],extract_holog_parms['overwrite'])
     check_if_file_will_be_overwritten(extract_holog_parms['point_name'],extract_holog_parms['overwrite'])
-
+    #######################################
+        
+    ############# Exstract pointing infromation and save to point.zarr #############
 #    try:
-#        pnt_dict = _load_pnt_dict(extract_holog_parms['point_name'])
+#        pnt_dict = _load_point_file(extract_holog_parms['point_name'])
 #    except:
 #        pnt_dict = _make_ant_pnt_dict(extract_holog_parms['ms_name'], extract_holog_parms['point_name'], parallel=extract_holog_parms['parallel'])
     
-    pnt_dict = _make_ant_pnt_dict(extract_holog_parms['ms_name'], extract_holog_parms['point_name'], parallel=extract_holog_parms['parallel'])
+    pnt_dict = _extract_pointing(extract_holog_parms['ms_name'], extract_holog_parms['point_name'], parallel=extract_holog_parms['parallel'])
 
-    ''' VLA datasets causeing issues.
-    if holog_obs_dict is None:
-        ant_names_list = []
-        #Create mapping antennas
-        holog_obs_dict = {}
-        for ant_id,pnt_xds in pnt_dict.items():
-            ant_name = pnt_xds.attrs['ant_name']
-            mapping_scans = pnt_xds.attrs['mapping_scans']
-            ant_names_list.append(ant_name)
-            for ddi,scans in  mapping_scans.items():
-                ddi = int(ddi)
-                for s in scans:
-                    try:
-                        holog_obs_dict[ddi][s]['map'].append(ant_name)
-                    except:
-                        holog_obs_dict.setdefault(ddi,{})[s] = {'map':[ant_name]}#dict(zip(scans, [ant_name]*len(scans)))
-       
-       
-        #Create reference antennas
-        
-        ant_names_set = set(ant_names_list)
-        for ddi,scan in holog_obs_dict.items():
-            for scan_id,ant_types in scan.items():
-                holog_obs_dict[ddi][scan_id]['ref'] = ant_names_set - set(holog_obs_dict[ddi][scan_id]['map'])
-            
-    print(holog_obs_dict)
-    '''
+    
+    
+    #### To DO: automatically create holog_obs_dict
+    # from astrohack._utils._extract_holog import _create_holog_obs_dict
 
 
     ######## Get Spectral Windows ########
     ctb = ctables.table(
         os.path.join(extract_holog_parms['ms_name'], "DATA_DESCRIPTION"),
         readonly=True,
         lockoptions={"option": "usernoread"},
@@ -256,15 +238,15 @@
         extract_holog_parms["pol_setup"]["pol"] = pol_str[pol_ctb.getcol("CORR_TYPE", startrow=pol_setup_id, nrow=1)[0, :]]
                 
         
         extract_holog_parms["telescope_name"] = obs_ctb.getcol("TELESCOPE_NAME")[0]
         
 
         for holog_map_key in holog_obs_dict.keys(): #loop over all beam_scan_ids, a beam_scan_id can conist out of more than one scan in an ms (this is the case for the VLA pointed mosiacs).
-            #if isinstance(holog_map_key,int):
+
             if 'map' in holog_map_key:
                 scans = holog_obs_dict[holog_map_key]["scans"]
                 logger.info("Processing ddi: {ddi}, scans: {scans}".format(ddi=ddi, scans=scans))
             
                 map_ant_list = []
                 ref_ant_per_map_ant_list = [] #
                 
@@ -274,18 +256,16 @@
                     ref_ant_ids = np.array(_convert_ant_name_to_id(ant_names,list(holog_obs_dict[holog_map_key]['ant'][map_ant_str])))
                     map_ant_id = _convert_ant_name_to_id(ant_names,map_ant_str)[0]
 
                     ref_ant_per_map_ant_list.append(ref_ant_ids)
                     map_ant_list.append(map_ant_id)
                     
                     ref_ant_per_map_ant_name_list.append(list(holog_obs_dict[holog_map_key]['ant'][map_ant_str]))
-                    map_ant_name_list.append(map_ant_str) #
-                    
-                    
-                    
+                    map_ant_name_list.append(map_ant_str)
+
                 extract_holog_parms["ref_ant_per_map_ant_tuple"] = tuple(ref_ant_per_map_ant_list)
                 extract_holog_parms["map_ant_tuple"] = tuple(map_ant_list)
                 
                 extract_holog_parms["ref_ant_per_map_ant_name_tuple"] = tuple(ref_ant_per_map_ant_name_list)
                 extract_holog_parms["map_ant_name_tuple"] = tuple(map_ant_name_list)
                 
                 extract_holog_parms["scans"] = scans
```

### Comparing `astrohack-0.0.7/src/astrohack/gdown_utils.py` & `astrohack-0.0.8/src/astrohack/gdown_utils.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.7/src/astrohack/holog.py` & `astrohack-0.0.8/src/astrohack/holog.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from astrohack._utils._holog import _holog_chunk
 
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 from astrohack._utils._parm_utils._check_parms import _check_parms
 from astrohack._utils._utils import _remove_suffix
    
 from astrohack._utils._io import check_if_file_will_be_overwritten, check_if_file_exists
-from astrohack._utils._dio_classes import AstrohackImageFile
+from astrohack._utils._dio import AstrohackImageFile
 
 #fp=open('holog.log','w+')
 #@profile(stream=fp)
 def holog(
     holog_name,
     grid_size,
     cell_size,
```

### Comparing `astrohack-0.0.7/src/astrohack/panel.py` & `astrohack-0.0.8/src/astrohack/panel.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from astrohack._utils._panel import _external_to_internal_parameters, _correct_phase
 import numpy as np
 
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 from astrohack._utils._parm_utils._check_parms import _check_parms
 from astrohack._utils._utils import _remove_suffix
 
-from astrohack._utils._dio_classes import AstrohackPanelFile
+from astrohack._utils._dio import AstrohackPanelFile
 
 
 def panel(image_name, panel_name=None, cutoff=0.2, panel_model=None, panel_margins=0.2, parallel=False, sel_ddi=None,
           overwrite=False):
     """Analyze holography images to derive panel adjustments
 
     :param image_name: Input holography data file name. Accepted data formats are the output from ``astrohack.holog.holog`` and AIPS holography data prepackaged using ``astrohack.panel.aips_holog_to_astrohack``.
@@ -248,13 +248,13 @@
     parms_passed = parms_passed and _check_parms(panel_params, 'panel_kind', [str], acceptable_data=panel_models, default="rigid")
     parms_passed = parms_passed and _check_parms(panel_params, 'panel_margins', [float], acceptable_range=[0, 0.5], default=0.2)
     parms_passed = parms_passed and _check_parms(panel_params, 'parallel', [bool], default=False)
     parms_passed = parms_passed and _check_parms(panel_params, 'sel_ddi', [list, np.array], list_acceptable_data_types=[int, np.int], default='all')
     parms_passed = parms_passed and _check_parms(panel_params, 'overwrite', [bool], default=False)
 
     if not parms_passed:
-        logger.error("extract_holog parameter checking failed.")
-        raise Exception("extract_holog parameter checking failed.")
+        logger.error("panel parameter checking failed.")
+        raise Exception("panel parameter checking failed.")
     
     return panel_params
```

### Comparing `astrohack-0.0.7/src/astrohack/profiling.py` & `astrohack-0.0.8/src/astrohack/profiling.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.7/src/astrohack/visualization/viewer.py` & `astrohack-0.0.8/src/astrohack/visualization/viewer.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -148,8 +148,8 @@
                 pn.Card(self._make_amplitude_plot, name="amplitude")
             )   
             
             golden.main.append(
                 pn.Card(self._make_angle_plot, name="angle")
             )
 
-        return golden.show()
+        return golden.show()
```

### Comparing `astrohack-0.0.7/src/astrohack.egg-info/PKG-INFO` & `astrohack-0.0.8/src/astrohack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrohack
-Version: 0.0.7
+Version: 0.0.8
 Summary: Holography Antenna Commissioning Kit
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `astrohack-0.0.7/src/astrohack.egg-info/SOURCES.txt` & `astrohack-0.0.8/src/astrohack.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -22,15 +22,17 @@
 src/astrohack/_classes/polygon_panel.py
 src/astrohack/_classes/ring_panel.py
 src/astrohack/_classes/telescope.py
 src/astrohack/_utils/__init__.py
 src/astrohack/_utils/_algorithms.py
 src/astrohack/_utils/_constants.py
 src/astrohack/_utils/_conversion.py
-src/astrohack/_utils/_dio_classes.py
+src/astrohack/_utils/_dio.py
+src/astrohack/_utils/_extract_holog.py
+src/astrohack/_utils/_extract_point.py
 src/astrohack/_utils/_holog.py
 src/astrohack/_utils/_imaging.py
 src/astrohack/_utils/_io.py
 src/astrohack/_utils/_panel.py
 src/astrohack/_utils/_utils.py
 src/astrohack/_utils/gaussfitter.py
 src/astrohack/_utils/_dask_plugins/__init__.py
@@ -58,9 +60,11 @@
 src/astrohack/data/telescopes/vla.zarr/.zgroup
 src/astrohack/data/telescopes/vla.zarr/.zmetadata
 src/astrohack/data/telescopes/vlba.zarr/.zattrs
 src/astrohack/data/telescopes/vlba.zarr/.zgroup
 src/astrohack/data/telescopes/vlba.zarr/.zmetadata
 src/astrohack/visualization/__init__.py
 src/astrohack/visualization/viewer.py
+tests/test_class_antenna_surface.py
 tests/test_class_base_panel.py
-tests/test_class_ring_panel.py
+tests/test_class_ring_panel.py
+tests/test_class_telescope.py
```

### Comparing `astrohack-0.0.7/src/astrohack.egg-info/requires.txt` & `astrohack-0.0.8/src/astrohack.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.7/tests/test_class_base_panel.py` & `astrohack-0.0.8/tests/test_class_base_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.7/tests/test_class_ring_panel.py` & `astrohack-0.0.8/tests/test_class_ring_panel.py`

 * *Files identical despite different names*

