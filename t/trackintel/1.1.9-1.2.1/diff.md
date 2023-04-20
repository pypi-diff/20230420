# Comparing `tmp/trackintel-1.1.9.tar.gz` & `tmp/trackintel-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trackintel-1.1.9.tar", last modified: Mon Jun  6 23:24:56 2022, max compression
+gzip compressed data, was "trackintel-1.2.1.tar", last modified: Thu Apr 20 14:25:16 2023, max compression
```

## Comparing `trackintel-1.1.9.tar` & `trackintel-1.2.1.tar`

### file list

```diff
@@ -1,104 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-06 23:24:56.878225 trackintel-1.1.9/
--rw-r--r--   0 runner    (1001) docker     (116)      820 2022-06-06 23:24:46.000000 trackintel-1.1.9/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (116)     1091 2022-06-06 23:24:46.000000 trackintel-1.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     7309 2022-06-06 23:24:56.878225 trackintel-1.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     6735 2022-06-06 23:24:46.000000 trackintel-1.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-06-06 23:24:56.878225 trackintel-1.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     3022 2022-06-06 23:24:46.000000 trackintel-1.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-06 23:24:56.870225 trackintel-1.1.9/tests/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-06 23:24:56.874225 trackintel-1.1.9/tests/analysis/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5515 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/analysis/test_label.py
--rw-r--r--   0 runner    (1001) docker     (116)    20437 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/analysis/test_location_identification.py
--rw-r--r--   0 runner    (1001) docker     (116)     9049 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/analysis/test_modal_split.py
--rw-r--r--   0 runner    (1001) docker     (116)    19319 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/analysis/test_tracking_quality.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-06 23:24:56.874225 trackintel-1.1.9/tests/examples/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      297 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/examples/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (116)      996 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/examples/test_tutorial.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-06 23:24:56.874225 trackintel-1.1.9/tests/geogr/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/geogr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10856 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/geogr/test_distances.py
--rw-r--r--   0 runner    (1001) docker     (116)     2705 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/geogr/test_point_distances.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-06 23:24:56.874225 trackintel-1.1.9/tests/io/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     9886 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/io/test_dataset_reader.py
--rw-r--r--   0 runner    (1001) docker     (116)    15571 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/io/test_file.py
--rw-r--r--   0 runner    (1001) docker     (116)    15670 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/io/test_from_geopandas.py
--rw-r--r--   0 runner    (1001) docker     (116)    27289 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/io/test_postgis.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-06 23:24:56.874225 trackintel-1.1.9/tests/model/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1343 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/model/test_locations.py
--rw-r--r--   0 runner    (1001) docker     (116)     2248 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/model/test_positionfixes.py
--rw-r--r--   0 runner    (1001) docker     (116)     1717 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/model/test_staypoints.py
--rw-r--r--   0 runner    (1001) docker     (116)     1572 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/model/test_triplegs.py
--rw-r--r--   0 runner    (1001) docker     (116)     1725 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/model/test_trips.py
--rw-r--r--   0 runner    (1001) docker     (116)     9868 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/model/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-06 23:24:56.874225 trackintel-1.1.9/tests/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5690 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/preprocessing/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (116)    23738 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/preprocessing/test_positionfixes.py
--rw-r--r--   0 runner    (1001) docker     (116)    22618 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/preprocessing/test_staypoints.py
--rw-r--r--   0 runner    (1001) docker     (116)    30544 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/preprocessing/test_triplegs.py
--rw-r--r--   0 runner    (1001) docker     (116)    13651 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/preprocessing/test_trips.py
--rw-r--r--   0 runner    (1001) docker     (116)     3175 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/preprocessing/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-06 23:24:56.874225 trackintel-1.1.9/tests/visualization/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2112 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/visualization/test_locations.py
--rw-r--r--   0 runner    (1001) docker     (116)     4601 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/visualization/test_modal_split.py
--rw-r--r--   0 runner    (1001) docker     (116)      693 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/visualization/test_positionfixes.py
--rw-r--r--   0 runner    (1001) docker     (116)     1439 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/visualization/test_staypoints.py
--rw-r--r--   0 runner    (1001) docker     (116)     1785 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/visualization/test_triplegs.py
--rw-r--r--   0 runner    (1001) docker     (116)      847 2022-06-06 23:24:46.000000 trackintel-1.1.9/tests/visualization/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-06 23:24:56.874225 trackintel-1.1.9/trackintel/
--rw-r--r--   0 runner    (1001) docker     (116)      486 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       63 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-06 23:24:56.878225 trackintel-1.1.9/trackintel/analysis/
--rw-r--r--   0 runner    (1001) docker     (116)      687 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5702 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/analysis/labelling.py
--rw-r--r--   0 runner    (1001) docker     (116)    13241 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/analysis/location_identification.py
--rw-r--r--   0 runner    (1001) docker     (116)     3399 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/analysis/modal_split.py
--rw-r--r--   0 runner    (1001) docker     (116)     8761 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/analysis/tracking_quality.py
--rw-r--r--   0 runner    (1001) docker     (116)      299 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/core.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-06 23:24:56.878225 trackintel-1.1.9/trackintel/geogr/
--rw-r--r--   0 runner    (1001) docker     (116)       98 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/geogr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8975 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/geogr/distances.py
--rw-r--r--   0 runner    (1001) docker     (116)     1546 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/geogr/point_distances.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-06 23:24:56.878225 trackintel-1.1.9/trackintel/io/
--rw-r--r--   0 runner    (1001) docker     (116)     1351 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    13972 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/io/dataset_reader.py
--rw-r--r--   0 runner    (1001) docker     (116)    20170 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/io/file.py
--rw-r--r--   0 runner    (1001) docker     (116)    13340 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/io/from_geopandas.py
--rw-r--r--   0 runner    (1001) docker     (116)    24262 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/io/postgis.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-06 23:24:56.878225 trackintel-1.1.9/trackintel/model/
--rw-r--r--   0 runner    (1001) docker     (116)      238 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3275 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/model/locations.py
--rw-r--r--   0 runner    (1001) docker     (116)     5508 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/model/positionfixes.py
--rw-r--r--   0 runner    (1001) docker     (116)     6098 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/model/staypoints.py
--rw-r--r--   0 runner    (1001) docker     (116)     2755 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/model/tours.py
--rw-r--r--   0 runner    (1001) docker     (116)     7092 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/model/triplegs.py
--rw-r--r--   0 runner    (1001) docker     (116)     5293 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/model/trips.py
--rw-r--r--   0 runner    (1001) docker     (116)     4480 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/model/util.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-06 23:24:56.878225 trackintel-1.1.9/trackintel/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (116)      404 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2911 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/preprocessing/filter.py
--rw-r--r--   0 runner    (1001) docker     (116)    21449 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/preprocessing/positionfixes.py
--rw-r--r--   0 runner    (1001) docker     (116)    15474 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/preprocessing/staypoints.py
--rw-r--r--   0 runner    (1001) docker     (116)    13353 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/preprocessing/triplegs.py
--rw-r--r--   0 runner    (1001) docker     (116)    17114 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/preprocessing/trips.py
--rw-r--r--   0 runner    (1001) docker     (116)     2986 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/preprocessing/util.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-06 23:24:56.878225 trackintel-1.1.9/trackintel/visualization/
--rw-r--r--   0 runner    (1001) docker     (116)      392 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2966 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/visualization/locations.py
--rw-r--r--   0 runner    (1001) docker     (116)     3805 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/visualization/modal_split.py
--rw-r--r--   0 runner    (1001) docker     (116)     1489 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/visualization/osm.py
--rw-r--r--   0 runner    (1001) docker     (116)     1809 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/visualization/positionfixes.py
--rw-r--r--   0 runner    (1001) docker     (116)     2743 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/visualization/staypoints.py
--rw-r--r--   0 runner    (1001) docker     (116)     2611 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/visualization/triplegs.py
--rw-r--r--   0 runner    (1001) docker     (116)     3600 2022-06-06 23:24:46.000000 trackintel-1.1.9/trackintel/visualization/util.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-06 23:24:56.878225 trackintel-1.1.9/trackintel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     7309 2022-06-06 23:24:56.000000 trackintel-1.1.9/trackintel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2681 2022-06-06 23:24:56.000000 trackintel-1.1.9/trackintel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-06-06 23:24:56.000000 trackintel-1.1.9/trackintel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      133 2022-06-06 23:24:56.000000 trackintel-1.1.9/trackintel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-06-06 23:24:56.000000 trackintel-1.1.9/trackintel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.770783 trackintel-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-20 14:25:08.000000 trackintel-1.2.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-20 14:25:08.000000 trackintel-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-04-20 14:25:16.770783 trackintel-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-04-20 14:25:08.000000 trackintel-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.742782 trackintel-1.2.1/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:08.000000 trackintel-1.2.1/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-04-20 14:25:08.000000 trackintel-1.2.1/benchmarks/preprocessing_benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 14:25:16.770783 trackintel-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-20 14:25:08.000000 trackintel-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.742782 trackintel-1.2.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.746782 trackintel-1.2.1/tests/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/analysis/test_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20437 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/analysis/test_location_identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/analysis/test_modal_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19336 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/analysis/test_tracking_quality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.746782 trackintel-1.2.1/tests/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/examples/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/examples/test_tutorial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.746782 trackintel-1.2.1/tests/geogr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/geogr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/geogr/test_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/geogr/test_point_distances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.750782 trackintel-1.2.1/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/io/test_dataset_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/io/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15670 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/io/test_from_geopandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28897 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/io/test_postgis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.750782 trackintel-1.2.1/tests/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/model/test_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/model/test_positionfixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/model/test_staypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/model/test_triplegs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/model/test_trips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/model/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.754783 trackintel-1.2.1/tests/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/preprocessing/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25185 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/preprocessing/test_positionfixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25722 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/preprocessing/test_staypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31836 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/preprocessing/test_triplegs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/preprocessing/test_trips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/preprocessing/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.754783 trackintel-1.2.1/tests/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/visualization/test_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/visualization/test_modal_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/visualization/test_positionfixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/visualization/test_staypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/visualization/test_triplegs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/visualization/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.758782 trackintel-1.2.1/trackintel/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.758782 trackintel-1.2.1/trackintel/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/analysis/labelling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/analysis/location_identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/analysis/modal_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/analysis/tracking_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.762783 trackintel-1.2.1/trackintel/geogr/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/geogr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/geogr/distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/geogr/point_distances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.762783 trackintel-1.2.1/trackintel/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27617 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/io/dataset_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20115 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/io/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13340 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/io/from_geopandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24080 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/io/postgis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.766783 trackintel-1.2.1/trackintel/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/model/locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/model/positionfixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/model/staypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/model/tours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/model/triplegs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/model/trips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/model/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.766783 trackintel-1.2.1/trackintel/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/preprocessing/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21266 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/preprocessing/positionfixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14528 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/preprocessing/staypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14341 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/preprocessing/triplegs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17114 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/preprocessing/trips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/preprocessing/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.770783 trackintel-1.2.1/trackintel/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/visualization/locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/visualization/modal_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/visualization/osm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/visualization/positionfixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/visualization/staypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/visualization/triplegs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/visualization/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.758782 trackintel-1.2.1/trackintel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-04-20 14:25:16.000000 trackintel-1.2.1/trackintel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-20 14:25:16.000000 trackintel-1.2.1/trackintel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:25:16.000000 trackintel-1.2.1/trackintel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-20 14:25:16.000000 trackintel-1.2.1/trackintel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-20 14:25:16.000000 trackintel-1.2.1/trackintel.egg-info/top_level.txt
```

### Comparing `trackintel-1.1.9/AUTHORS.md` & `trackintel-1.2.1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/LICENSE` & `trackintel-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/PKG-INFO` & `trackintel-1.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trackintel
-Version: 1.1.9
+Version: 1.2.1
 Summary: Human mobility and movement analysis framework.
 Home-page: https://github.com/mie-lab/trackintel
 Author: Dominik Bucher, Henry Martin, Ye Hong
 Author-email: dobucher@ethz.ch, martinhe@ethz.ch
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -12,30 +12,34 @@
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 
-# The trackintel Framework
+# The trackintel framework
 
 
 [![PyPI version](https://badge.fury.io/py/trackintel.svg)](https://badge.fury.io/py/trackintel)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/trackintel.svg)](https://anaconda.org/conda-forge/trackintel)
 [![Actions Status](https://github.com/mie-lab/trackintel/workflows/Tests/badge.svg)](https://github.com/mie-lab/trackintel/actions?query=workflow%3ATests)
 [![Documentation Status](https://readthedocs.org/projects/trackintel/badge/?version=latest)](https://trackintel.readthedocs.io/en/latest/?badge=latest)
 [![codecov.io](https://codecov.io/gh/mie-lab/trackintel/coverage.svg?branch=master)](https://codecov.io/gh/mie-lab/trackintel)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![asv](http://img.shields.io/badge/benchmarked%20by-asv-green.svg?style=flat)](https://mie-lab.github.io/trackintel/)
 
-*trackintel* is a library for the analysis of spatio-temporal tracking data with a focus on human mobility. The core of *trackintel* is the hierachical data model for movement data that is used in GIS, transport planning and related fields [[1]](#1). We provide functionalities for the full life-cycle of human mobility data analysis: import and export of tracking data of different types (e.g, trackpoints, check-ins, trajectories), preprocessing, data quality assessment, semantic enrichment, quantitative analysis and mining tasks, and visualization of data and results.
-Trackintel is based on [Pandas](https://pandas.pydata.org/) and [GeoPandas](https://geopandas.org/#)
+*trackintel* is a library for the analysis of spatio-temporal tracking data with a focus on human mobility. The core of *trackintel* is the hierachical data model for movement data that is used in GIS, transport planning and related fields. We provide functionalities for the full life-cycle of human mobility data analysis: import and export of tracking data of different types (e.g, trackpoints, check-ins, trajectories), preprocessing, data quality assessment, semantic enrichment, quantitative analysis and mining tasks, and visualization of data and results.
+Trackintel is based on [Pandas](https://pandas.pydata.org/) and [GeoPandas](https://geopandas.org/#). 
 
-You can find the documentation on the [trackintel documentation page](https://trackintel.readthedocs.io/en/latest).
+You can find the documentation on the [trackintel documentation page](https://trackintel.readthedocs.io/en/latest). 
 
 Try *trackintel* online in a MyBinder notebook: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mie-lab/trackintel/HEAD?filepath=%2Fexamples%2Ftrackintel_basic_tutorial.ipynb)
 
+Please star this repo and [cite](#citelink) our paper if you find our work is helpful for you.
+
 ## Data model
 
 An overview of the data model of *trackintel*:
 * **positionfixes** (Raw tracking points, e.g., GPS recordings or check-ins)
 * **staypoints** (Locations where a user spent time without moving, e.g., aggregations of positionfixes or check-ins). Staypoints can be classified into the following categories:
   * **activity** staypoints. Staypoints with a purpose and a semantic label, e.g., stopping at a cafe to meet with friends or staying at the workplace.
   * non-activity staypoints. Staypoints without an explicit purpose, e.g., waiting for a bus or stopping in a traffic jam.
@@ -106,15 +110,20 @@
 
 For example, the plot below shows the generated staypoints and triplegs from the imported raw positionfix data.
 <p align="center">
   <img width="595" height="500" src="https://github.com/mie-lab/trackintel/blob/master/docs/_static/example_triplegs.png?raw=true">
 </p>
 
 ## Installation and Usage
-*trackintel* is on [pypi.org](https://pypi.org/project/trackintel/), you can install it in a `GeoPandas` available environment using: 
+*trackintel* is on [pypi.org](https://pypi.org/project/trackintel/) and [conda-forge](https://anaconda.org/conda-forge/trackintel). We recommend installing trackintel via conda-forge:
+```{python}
+conda install -c conda-forge trackintel
+```
+
+Alternatively, you can install it with pip in a `GeoPandas` available environment using: 
 ```{python}
 pip install trackintel
 ```
 
 You should then be able to run the examples in the `examples` folder or import trackintel using:
 ```{python}
 import trackintel as ti
@@ -140,11 +149,22 @@
 You can find the development roadmap under `ROADMAP.md` and further development guidelines under `CONTRIBUTING.md`.
 
 ## Contributors
 
 *trackintel* is primarily maintained by the Mobility Information Engineering Lab at ETH Zurich ([mie-lab.ethz.ch](http://mie-lab.ethz.ch)).
 If you want to contribute, send a pull request and put yourself in the `AUTHORS.md` file.
 
-## References
-<a id="1">[1]</a>
-[Axhausen, K. W. (2007). Definition Of Movement and Activity For Transport Modelling. In Handbook of Transport Modelling. Emerald Group Publishing Limited.](
-https://www.researchgate.net/publication/251791517_Definition_of_movement_and_activity_for_transport_modelling)
+## <span id="citelink">Citation</span>
+
+If you find this code useful for your work or use it in your project, please consider citing:
+```
+@article{Martin_2023_trackintel,
+  doi = {10.1016/j.compenvurbsys.2023.101938},
+  volume = {101},
+  pages = {101938},
+  author = {Henry Martin and Ye Hong and Nina Wiedemann and Dominik Bucher and Martin Raubal},
+  keywords = {Human mobility analysis, Open-source software, Transport planning, Data mining, Python, Tracking studies},
+  title = {Trackintel: An open-source Python library for human mobility analysis},
+  journal = {Computers, Environment and Urban Systems},
+  year = {2023},
+}
+```
```

### Comparing `trackintel-1.1.9/README.md` & `trackintel-1.2.1/trackintel.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,45 @@
-# The trackintel Framework
+Metadata-Version: 2.1
+Name: trackintel
+Version: 1.2.1
+Summary: Human mobility and movement analysis framework.
+Home-page: https://github.com/mie-lab/trackintel
+Author: Dominik Bucher, Henry Martin, Ye Hong
+Author-email: dobucher@ethz.ch, martinhe@ethz.ch
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Requires-Python: >=3.6.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.md
+
+
+# The trackintel framework
 
 
 [![PyPI version](https://badge.fury.io/py/trackintel.svg)](https://badge.fury.io/py/trackintel)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/trackintel.svg)](https://anaconda.org/conda-forge/trackintel)
 [![Actions Status](https://github.com/mie-lab/trackintel/workflows/Tests/badge.svg)](https://github.com/mie-lab/trackintel/actions?query=workflow%3ATests)
 [![Documentation Status](https://readthedocs.org/projects/trackintel/badge/?version=latest)](https://trackintel.readthedocs.io/en/latest/?badge=latest)
 [![codecov.io](https://codecov.io/gh/mie-lab/trackintel/coverage.svg?branch=master)](https://codecov.io/gh/mie-lab/trackintel)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![asv](http://img.shields.io/badge/benchmarked%20by-asv-green.svg?style=flat)](https://mie-lab.github.io/trackintel/)
 
-*trackintel* is a library for the analysis of spatio-temporal tracking data with a focus on human mobility. The core of *trackintel* is the hierachical data model for movement data that is used in GIS, transport planning and related fields [[1]](#1). We provide functionalities for the full life-cycle of human mobility data analysis: import and export of tracking data of different types (e.g, trackpoints, check-ins, trajectories), preprocessing, data quality assessment, semantic enrichment, quantitative analysis and mining tasks, and visualization of data and results.
-Trackintel is based on [Pandas](https://pandas.pydata.org/) and [GeoPandas](https://geopandas.org/#)
+*trackintel* is a library for the analysis of spatio-temporal tracking data with a focus on human mobility. The core of *trackintel* is the hierachical data model for movement data that is used in GIS, transport planning and related fields. We provide functionalities for the full life-cycle of human mobility data analysis: import and export of tracking data of different types (e.g, trackpoints, check-ins, trajectories), preprocessing, data quality assessment, semantic enrichment, quantitative analysis and mining tasks, and visualization of data and results.
+Trackintel is based on [Pandas](https://pandas.pydata.org/) and [GeoPandas](https://geopandas.org/#). 
 
-You can find the documentation on the [trackintel documentation page](https://trackintel.readthedocs.io/en/latest).
+You can find the documentation on the [trackintel documentation page](https://trackintel.readthedocs.io/en/latest). 
 
 Try *trackintel* online in a MyBinder notebook: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mie-lab/trackintel/HEAD?filepath=%2Fexamples%2Ftrackintel_basic_tutorial.ipynb)
 
+Please star this repo and [cite](#citelink) our paper if you find our work is helpful for you.
+
 ## Data model
 
 An overview of the data model of *trackintel*:
 * **positionfixes** (Raw tracking points, e.g., GPS recordings or check-ins)
 * **staypoints** (Locations where a user spent time without moving, e.g., aggregations of positionfixes or check-ins). Staypoints can be classified into the following categories:
   * **activity** staypoints. Staypoints with a purpose and a semantic label, e.g., stopping at a cafe to meet with friends or staying at the workplace.
   * non-activity staypoints. Staypoints without an explicit purpose, e.g., waiting for a bus or stopping in a traffic jam.
@@ -88,15 +110,20 @@
 
 For example, the plot below shows the generated staypoints and triplegs from the imported raw positionfix data.
 <p align="center">
   <img width="595" height="500" src="https://github.com/mie-lab/trackintel/blob/master/docs/_static/example_triplegs.png?raw=true">
 </p>
 
 ## Installation and Usage
-*trackintel* is on [pypi.org](https://pypi.org/project/trackintel/), you can install it in a `GeoPandas` available environment using: 
+*trackintel* is on [pypi.org](https://pypi.org/project/trackintel/) and [conda-forge](https://anaconda.org/conda-forge/trackintel). We recommend installing trackintel via conda-forge:
+```{python}
+conda install -c conda-forge trackintel
+```
+
+Alternatively, you can install it with pip in a `GeoPandas` available environment using: 
 ```{python}
 pip install trackintel
 ```
 
 You should then be able to run the examples in the `examples` folder or import trackintel using:
 ```{python}
 import trackintel as ti
@@ -122,11 +149,22 @@
 You can find the development roadmap under `ROADMAP.md` and further development guidelines under `CONTRIBUTING.md`.
 
 ## Contributors
 
 *trackintel* is primarily maintained by the Mobility Information Engineering Lab at ETH Zurich ([mie-lab.ethz.ch](http://mie-lab.ethz.ch)).
 If you want to contribute, send a pull request and put yourself in the `AUTHORS.md` file.
 
-## References
-<a id="1">[1]</a>
-[Axhausen, K. W. (2007). Definition Of Movement and Activity For Transport Modelling. In Handbook of Transport Modelling. Emerald Group Publishing Limited.](
-https://www.researchgate.net/publication/251791517_Definition_of_movement_and_activity_for_transport_modelling)
+## <span id="citelink">Citation</span>
+
+If you find this code useful for your work or use it in your project, please consider citing:
+```
+@article{Martin_2023_trackintel,
+  doi = {10.1016/j.compenvurbsys.2023.101938},
+  volume = {101},
+  pages = {101938},
+  author = {Henry Martin and Ye Hong and Nina Wiedemann and Dominik Bucher and Martin Raubal},
+  keywords = {Human mobility analysis, Open-source software, Transport planning, Data mining, Python, Tracking studies},
+  title = {Trackintel: An open-source Python library for human mobility analysis},
+  journal = {Computers, Environment and Urban Systems},
+  year = {2023},
+}
+```
```

### Comparing `trackintel-1.1.9/setup.py` & `trackintel-1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,21 +37,21 @@
 ]
 
 install_requires = [
     "pandas",
     "matplotlib",
     "numpy",
     "pint",
-    "shapely",
+    "shapely<=1.8.5",
     "networkx",
     "geoalchemy2",
     "osmnx",
     "scikit-learn",
     "tqdm",
-    "geopandas>=0.9.0",
+    "geopandas>=0.10.0",
     "similaritymeasures",
     "pygeos>=0.10.0",
 ]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
```

### Comparing `trackintel-1.1.9/tests/analysis/test_label.py` & `trackintel-1.2.1/tests/analysis/test_label.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/tests/analysis/test_location_identification.py` & `trackintel-1.2.1/tests/analysis/test_location_identification.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/tests/analysis/test_modal_split.py` & `trackintel-1.2.1/tests/analysis/test_modal_split.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/tests/analysis/test_tracking_quality.py` & `trackintel-1.2.1/tests/analysis/test_tracking_quality.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
         # read positionfixes and feed to temporal_tracking_quality()
         pfs, _ = ti.io.dataset_reader.read_geolife(os.path.join("tests", "data", "geolife_long"))
         with pytest.raises(KeyError):
             ti.analysis.tracking_quality.temporal_tracking_quality(pfs)
 
         # generate locations and feed to temporal_tracking_quality()
         sp_file = os.path.join("tests", "data", "geolife", "geolife_staypoints.csv")
-        sp = ti.read_staypoints_csv(sp_file, tz="utc", index_col="id")
+        sp = ti.read_staypoints_csv(sp_file, tz="utc", index_col="id", crs="epsg:4326")
         _, locs = sp.as_staypoints.generate_locations(
             method="dbscan", epsilon=10, num_samples=1, distance_metric="haversine", agg_level="dataset"
         )
         with pytest.raises(KeyError):
             ti.analysis.tracking_quality.temporal_tracking_quality(locs)
 
     def test_tracking_quality_user_error(self, testdata_sp_tpls_geolife_long):
```

### Comparing `trackintel-1.1.9/tests/examples/test_tutorial.py` & `trackintel-1.2.1/tests/examples/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/tests/geogr/test_distances.py` & `trackintel-1.2.1/tests/geogr/test_distances.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     return gdf
 
 
 @pytest.fixture
 def single_linestring():
     """Construct LineString that has ~1024 m in QGIS."""
     return wkt.loads(
-        """LineString(13.47671401745228259 
+        """LineString(13.47671401745228259
     48.57364142178052901, 13.47510901146785933
     48.5734004715611789, 13.47343656825720082
     48.57335585102421049, 13.47172366271079369
     48.57318629262447018, 13.4697275208142031
     48.57325768570418489, 13.4680415901582915
     48.57348971251707326, 13.46604544826169914
     48.57348971251707326, 13.46473716607271243
@@ -191,36 +191,36 @@
         assert_geodataframe_equal(pfs, pfs_4326, check_less_precise=True)
 
     def test_crs_warning(self):
         """Check if warning is raised for data without crs."""
         file = os.path.join("tests", "data", "positionfixes.csv")
         pfs = ti.read_positionfixes_csv(file, sep=";", crs=None, index_col=None)
         with pytest.warns(UserWarning):
-            assert check_gdf_planar(pfs) == False
+            assert check_gdf_planar(pfs) is False
 
     def test_if_planer(self):
         """Check if planer crs is successfully checked."""
         p1 = Point(8.5067847, 47.4)
         t1 = pd.Timestamp("1971-01-01 00:00:00", tz="utc")
 
         list_dict = [
             {"user_id": 0, "started_at": t1, "finished_at": t1, "geom": p1},
         ]
         # a geographic crs different than wgs1984
         sp = gpd.GeoDataFrame(data=list_dict, geometry="geom", crs="EPSG:4610")
-        assert check_gdf_planar(sp) == False
+        assert check_gdf_planar(sp) is False
 
         # wgs1984
         sp = gpd.GeoDataFrame(data=list_dict, geometry="geom", crs="EPSG:4326")
-        assert check_gdf_planar(sp) == False
+        assert check_gdf_planar(sp) is False
 
         # wgs1984 to swiss planer
         sp = gpd.GeoDataFrame(data=list_dict, geometry="geom", crs="EPSG:4326")
         sp = sp.to_crs("EPSG:2056")
-        assert check_gdf_planar(sp) == True
+        assert check_gdf_planar(sp) is True
 
     def test_none_crs_transform(self):
         """Check if crs gets set to WGS84."""
         file = os.path.join("tests", "data", "positionfixes.csv")
         pfs = ti.read_positionfixes_csv(file, sep=";", crs=None, index_col=None)
         bool, pfs_4326 = check_gdf_planar(pfs, transform=True)
         assert not bool
```

### Comparing `trackintel-1.1.9/tests/geogr/test_point_distances.py` & `trackintel-1.2.1/tests/geogr/test_point_distances.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,18 +54,17 @@
         # their distance
         x_rad = np.asarray([radians(_) for _ in x])
         y_rad = np.asarray([radians(_) for _ in y])
         yx = np.concatenate((y_rad.reshape(-1, 1), x_rad.reshape(-1, 1)), axis=1)
 
         D_theirs = haversine_distances(yx, yx) * 6371000
         d_theirs = D_theirs[ix_1, ix_2]
-        assert np.sum(np.abs(d_ours - d_theirs)) < 0.01  #  1cm for 58 should be good enough
+        assert np.sum(np.abs(d_ours - d_theirs)) < 0.01  # 1cm for 58 should be good enough
 
     def test_example_from_sklean(self):
-
         bsas = [-34.83333, -58.5166646]
         paris = [49.0083899664, 2.53844117956]
         bsas_in_radians = [radians(_) for _ in bsas]
         paris_in_radians = [radians(_) for _ in paris]
         d_theirs = haversine_distances([bsas_in_radians, paris_in_radians]) * 6371000
 
         d_ours = haversine_dist(bsas[1], bsas[0], paris[1], paris[0])
```

### Comparing `trackintel-1.1.9/tests/io/test_dataset_reader.py` & `trackintel-1.2.1/tests/io/test_dataset_reader.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/tests/io/test_file.py` & `trackintel-1.2.1/tests/io/test_file.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/tests/io/test_from_geopandas.py` & `trackintel-1.2.1/tests/io/test_from_geopandas.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/tests/io/test_postgis.py` & `trackintel-1.2.1/tests/io/test_postgis.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 import geopandas as gpd
 from geopandas.testing import assert_geodataframe_equal
 import pandas as pd
 from pandas.testing import assert_frame_equal
 import pytest
 import sqlalchemy
+from sqlalchemy import create_engine
+
 from shapely.geometry import LineString, MultiPoint, Point, Polygon
 
 import trackintel as ti
 
 
 @pytest.fixture()
 def conn_postgis():
@@ -21,15 +23,15 @@
     -------
     conn_string, con
     """
     psycopg2 = pytest.importorskip("psycopg2")
 
     dbname = "test_geopandas"
     user = os.environ.get("PGUSER")
-    password = os.environ.get("PGPASSWORD")
+    password = "postgres"
     host = os.environ.get("PGHOST")
     port = os.environ.get("PGPORT")
     conn_string = f"postgresql://{user}:{password}@{host}:{port}/{dbname}"
 
     try:
         con = psycopg2.connect(conn_string)
     except psycopg2.OperationalError:
@@ -267,32 +269,36 @@
         conn_string, conn = conn_postgis
         table = "positionfixes"
         sql = f"SELECT * FROM {table}"
         geom_col = pfs.geometry.name
 
         try:
             pfs.as_positionfixes.to_postgis(table, conn_string)
-            pfs_db = ti.io.read_positionfixes_postgis(sql, conn_string, geom_col)
+            with pytest.warns(UserWarning):
+                pfs_db = ti.io.read_positionfixes_postgis(sql, conn, geom_col)
             pfs_db = pfs_db.set_index("id")
             print(pfs_db)
             assert_geodataframe_equal(pfs, pfs_db)
         finally:
             del_table(conn, table)
 
     def test_no_crs(self, example_positionfixes, conn_postgis):
         """Test if writing reading to postgis also works correctly without CRS."""
         pfs = example_positionfixes.copy()
         conn_string, conn = conn_postgis
         table = "positionfixes"
         sql = f"SELECT * FROM {table}"
         geom_col = pfs.geometry.name
         pfs.crs = None
+        no_crs_warning = "Could not parse CRS from the GeoDataFrame. Inserting data without defined CRS."
         try:
-            pfs.as_positionfixes.to_postgis(table, conn_string)
-            pfs_db = ti.io.read_positionfixes_postgis(sql, conn_string, geom_col)
+            with pytest.warns(UserWarning, match=no_crs_warning):
+                pfs.as_positionfixes.to_postgis(table, conn_string)
+            with pytest.warns(UserWarning):
+                pfs_db = ti.io.read_positionfixes_postgis(sql, conn, geom_col)
             pfs_db = pfs_db.set_index("id")
             assert_geodataframe_equal(pfs, pfs_db)
         finally:
             del_table(conn, table)
 
     def test_non_standard_column_names(self, example_positionfixes, conn_postgis):
         """Test renaming handled by read_positionfixes_gpd()."""
@@ -301,15 +307,16 @@
         table = "positionfixes"
         sql = f"SELECT * FROM {table}"
         geom_col = pfs.geometry.name
         rename_dict = {"user_id": "USER", "tracked_at": "time"}
         pfs.rename(rename_dict, inplace=True)
         try:
             pfs.as_positionfixes.to_postgis(table, conn_string)
-            pfs_db = ti.io.read_positionfixes_postgis(sql, conn_string, geom_col, index_col="id", **rename_dict)
+            with pytest.warns(UserWarning):
+                pfs_db = ti.io.read_positionfixes_postgis(sql, conn, geom_col, index_col="id", **rename_dict)
             assert_geodataframe_equal(example_positionfixes, pfs_db)
         finally:
             del_table(conn, table)
 
     def test_daylight_saving_tz(self, example_positionfixes, conn_postgis):
         """Test if function can handle different tz informations in one column.
 
@@ -323,15 +330,16 @@
         t1 = pd.Timestamp("2021-08-01 16:00:00", tz="utc")  # summer time
         t2 = pd.Timestamp("2021-08-01 15:00:00", tz="utc")  # summer time
         t3 = pd.Timestamp("2021-02-01 14:00:00", tz="utc")  # winter time
         pfs["tracked_at"] = [t1, t2, t3]
         geom_col = pfs.geometry.name
         try:
             pfs.as_positionfixes.to_postgis(table, conn_string)
-            pfs_db = ti.io.read_positionfixes_postgis(sql, conn_string, geom_col, index_col="id")
+            with pytest.warns(UserWarning):
+                pfs_db = ti.io.read_positionfixes_postgis(sql, conn, geom_col, index_col="id")
             assert_geodataframe_equal(pfs, pfs_db)
         finally:
             del_table(conn, table)
 
 
 class TestTriplegs:
     def test_write(self, example_triplegs, conn_postgis):
@@ -357,31 +365,35 @@
         conn_string, conn = conn_postgis
         table = "triplegs"
         sql = f"SELECT * FROM {table}"
         geom_col = tpls.geometry.name
 
         try:
             tpls.as_triplegs.to_postgis(table, conn_string)
-            tpls_db = ti.io.read_triplegs_postgis(sql, conn_string, geom_col, index_col="id")
+            with pytest.warns(UserWarning):
+                tpls_db = ti.io.read_triplegs_postgis(sql, conn, geom_col, index_col="id")
             assert_geodataframe_equal(tpls, tpls_db)
         finally:
             del_table(conn, table)
 
     def test_no_crs(self, example_triplegs, conn_postgis):
         """Test if writing reading to postgis also works correctly without CRS."""
         tpls = example_triplegs.copy()
         conn_string, conn = conn_postgis
         table = "triplegs"
         sql = f"SELECT * FROM {table}"
         geom_col = tpls.geometry.name
         tpls.crs = None
 
+        no_crs_warning = "Could not parse CRS from the GeoDataFrame. Inserting data without defined CRS."
         try:
-            tpls.as_triplegs.to_postgis(table, conn_string)
-            tpls_db = ti.io.read_triplegs_postgis(sql, conn_string, geom_col, index_col="id")
+            with pytest.warns(UserWarning, match=no_crs_warning):
+                tpls.as_triplegs.to_postgis(table, conn_string)
+            with pytest.warns(UserWarning):
+                tpls_db = ti.io.read_triplegs_postgis(sql, conn, geom_col, index_col="id")
             assert_geodataframe_equal(tpls, tpls_db)
         finally:
             del_table(conn, table)
 
     def test_non_standard_column_names(self, example_triplegs, conn_postgis):
         """Test renaming handled by read_triplegs_gpd()."""
         tpls = example_triplegs.copy()
@@ -389,15 +401,16 @@
         table = "triplegs"
         sql = f"SELECT * FROM {table}"
         geom_col = tpls.geometry.name
         rename_dict = {"user_id": "USER", "started_at": "start_time", "finished_at": "end_time"}
         tpls.rename(rename_dict, inplace=True)
         try:
             tpls.as_triplegs.to_postgis(table, conn_string)
-            tpls_db = ti.io.read_triplegs_postgis(sql, conn_string, geom_col, index_col="id", **rename_dict)
+            with pytest.warns(UserWarning):
+                tpls_db = ti.io.read_triplegs_postgis(sql, conn, geom_col, index_col="id", **rename_dict)
             assert_geodataframe_equal(example_triplegs, tpls_db)
         finally:
             del_table(conn, table)
 
 
 class TestStaypoints:
     def test_write(self, example_staypoints, conn_postgis):
@@ -423,30 +436,35 @@
         conn_string, conn = conn_postgis
         table = "staypoints"
         sql = f"SELECT * FROM {table}"
         geom_col = sp.geometry.name
 
         try:
             sp.as_staypoints.to_postgis(table, conn_string)
-            sp_db = ti.io.read_staypoints_postgis(sql, conn_string, geom_col, index_col="id")
+            with pytest.warns(UserWarning):
+                sp_db = ti.io.read_staypoints_postgis(sql, conn, geom_col, index_col="id")
             assert_geodataframe_equal(sp, sp_db)
         finally:
             del_table(conn, table)
 
     def test_no_crs(self, example_staypoints, conn_postgis):
         """Test if writing reading to postgis also works correctly without CRS."""
         sp = example_staypoints
         conn_string, conn = conn_postgis
         table = "staypoints"
         sql = f"SELECT * FROM {table}"
         geom_col = example_staypoints.geometry.name
         sp.crs = None
+
+        no_crs_warning = "Could not parse CRS from the GeoDataFrame. Inserting data without defined CRS."
         try:
-            sp.as_staypoints.to_postgis(table, conn_string)
-            sp_db = ti.io.read_staypoints_postgis(sql, conn_string, geom_col, index_col="id")
+            with pytest.warns(UserWarning, match=no_crs_warning):
+                sp.as_staypoints.to_postgis(table, conn_string)
+            with pytest.warns(UserWarning):
+                sp_db = ti.io.read_staypoints_postgis(sql, conn, geom_col, index_col="id")
             assert_geodataframe_equal(sp, sp_db)
         finally:
             del_table(conn, table)
 
 
 class TestLocations:
     def test_write(self, example_locations, conn_postgis):
@@ -472,30 +490,35 @@
         conn_string, conn = conn_postgis
         table = "locations"
         sql = f"SELECT * FROM {table}"
         geom_col = locs.geometry.name
 
         try:
             locs.as_locations.to_postgis(table, conn_string)
-            locs_db = ti.io.read_locations_postgis(sql, conn_string, geom_col, index_col="id")
+            with pytest.warns(UserWarning):
+                locs_db = ti.io.read_locations_postgis(sql, conn, geom_col, index_col="id")
             assert_geodataframe_equal(locs, locs_db)
         finally:
             del_table(conn, table)
 
     def test_no_crs(self, example_locations, conn_postgis):
         """Test if writing reading to postgis also works correctly without CRS."""
         locs = example_locations.copy()
         conn_string, conn = conn_postgis
         table = "locations"
         sql = f"SELECT * FROM {table}"
         geom_col = locs.geometry.name
         locs.crs = None
+
+        no_crs_warning = "Could not parse CRS from the GeoDataFrame. Inserting data without defined CRS."
         try:
-            locs.as_locations.to_postgis(table, conn_string)
-            locs_db = ti.io.read_locations_postgis(sql, conn_string, geom_col, index_col="id")
+            with pytest.warns(UserWarning, match=no_crs_warning):
+                locs.as_locations.to_postgis(table, conn_string)
+            with pytest.warns(UserWarning):
+                locs_db = ti.io.read_locations_postgis(sql, conn, geom_col, index_col="id")
             assert_geodataframe_equal(locs, locs_db)
         finally:
             del_table(conn, table)
 
     def test_write_extent(self, example_locations, conn_postgis):
         """Test if extent geometry is handled correctly."""
         conn_string, conn = conn_postgis
@@ -525,15 +548,16 @@
         sql = f"SELECT * FROM {table}"
         coords = [[8.45, 47.6], [8.45, 47.4], [8.55, 47.4], [8.55, 47.6], [8.45, 47.6]]
         extent = Polygon(coords)
         example_locations["extent"] = extent  # broadcasting
         example_locations["extent"] = gpd.GeoSeries(example_locations["extent"])  # dtype
         try:
             example_locations.as_locations.to_postgis(table, conn_string)
-            locs_db = ti.io.read_locations_postgis(sql, conn_string, extent="extent", index_col="id")
+            with pytest.warns(UserWarning):
+                locs_db = ti.io.read_locations_postgis(sql, conn, extent="extent", index_col="id")
             assert_geodataframe_equal(example_locations, locs_db)
         finally:
             del_table(conn, table)
 
     def test_non_standard_column_names(self, example_locations, conn_postgis):
         """Test renaming handled by read_locations_gpd()."""
         locs = example_locations.copy()
@@ -542,45 +566,47 @@
         sql = f"SELECT * FROM {table}"
         rename_dict = {"user_id": "USER", "center": "geom"}
         locs.rename(rename_dict, inplace=True)
         del rename_dict["center"]
         geom_col = locs.geometry.name
         try:
             locs.as_locations.to_postgis(table, conn_string)
-            tpls_db = ti.io.read_locations_postgis(sql, conn_string, geom_col, index_col="id", **rename_dict)
+            with pytest.warns(UserWarning):
+                tpls_db = ti.io.read_locations_postgis(sql, conn, geom_col, index_col="id", **rename_dict)
             assert_geodataframe_equal(example_locations, tpls_db)
         finally:
             del_table(conn, table)
 
 
 class TestTrips:
     def test_write(self, example_trips, conn_postgis):
         """Test if write of locations create correct schema in database."""
         trips = example_trips.copy()
         conn_string, conn = conn_postgis
         table = "trips"
         try:
-            trips.as_trips.to_postgis(table, conn_string)
-            columns_db, dtypes = get_table_schema(conn, table)
+            trips.as_trips.to_postgis(table, create_engine(conn_string))
+            columns_db, _ = get_table_schema(conn, table)
             columns = trips.columns.tolist() + [trips.index.name]
             assert len(columns_db) == len(columns)
             assert set(columns_db) == set(columns)
         finally:
             del_table(conn, table)
 
     def test_read(self, example_trips, conn_postgis):
         """Test if trips written to and read back from database are the same."""
         trips = example_trips.copy()
         conn_string, conn = conn_postgis
         table = "trips"
         sql = f"SELECT * FROM {table}"
 
         try:
-            trips.as_trips.to_postgis(table, conn_string)
-            trips_db = ti.io.read_trips_postgis(sql, conn_string, index_col="id")
+            trips.as_trips.to_postgis(table, create_engine(conn_string))
+            with pytest.warns(UserWarning):
+                trips_db = ti.io.read_trips_postgis(sql, conn, index_col="id")
             assert_frame_equal(trips, trips_db)
         finally:
             del_table(conn, table)
 
     def test_non_standard_column_names(self, example_trips, conn_postgis):
         """Test renaming handled by read_trips_gpd()."""
         trips = example_trips.copy()
@@ -592,16 +618,17 @@
             "finished_at": "end_time",
             "user_id": "USER",
             "origin_staypoint_id": "ORIGIN",
             "destination_staypoint_id": "DEST",
         }
         trips.rename(rename_dict, inplace=True)
         try:
-            trips.as_trips.to_postgis(table, conn_string)
-            tpls_db = ti.io.read_trips_postgis(sql, conn_string, index_col="id", **rename_dict)
+            trips.as_trips.to_postgis(table, create_engine(conn_string))
+            with pytest.warns(UserWarning):
+                tpls_db = ti.io.read_trips_postgis(sql, conn, index_col="id", **rename_dict)
             assert_frame_equal(example_trips, tpls_db)
         finally:
             del_table(conn, table)
 
     def test_write_with_geometry(self, example_trips, conn_postgis):
         """Test if write of trips with geometry creates correct schema in database."""
         mp1 = MultiPoint([(0.0, 0.0), (1.0, 1.0)])
@@ -628,61 +655,67 @@
         trips = gpd.GeoDataFrame(example_trips, copy=True, geometry=[mp1, mp2, mp2], crs="EPSG:4326")
         conn_string, conn = conn_postgis
         table = "trips"
         sql = f"SELECT * FROM {table}"
         geom_col = trips.geometry.name
 
         try:
-            trips.as_trips.to_postgis(table, conn_string)
-            locs_db = ti.io.read_trips_postgis(sql, conn_string, geom_col=geom_col, index_col="id")
+            trips.as_trips.to_postgis(table, create_engine(conn_string))
+            with pytest.warns(UserWarning):
+                locs_db = ti.io.read_trips_postgis(sql, conn, geom_col=geom_col, index_col="id")
             assert_geodataframe_equal(trips, locs_db)
         finally:
             del_table(conn, table)
 
 
 class TestTours:
     """Test of postgis functions for tours."""
 
     def test_write(self, example_tours, conn_postgis):
         """Test if write of tours create correct schema in database."""
         tours = example_tours
         conn_string, conn = conn_postgis
         table = "tours"
         try:
-            tours.as_tours.to_postgis(table, conn_string)
-            columns_db, dtypes = get_table_schema(conn, table)
+            tours.as_tours.to_postgis(table, create_engine(conn_string))
+            columns_db, _ = get_table_schema(conn, table)
             columns = tours.columns.tolist() + [tours.index.name]
             assert len(columns_db) == len(columns)
             assert set(columns_db) == set(columns)
         finally:
             del_table(conn, table)
 
     def test_read(self, example_tours, conn_postgis):
         """Test if tours written to and read back from database are the same."""
         tours = example_tours
         conn_string, conn = conn_postgis
         table = "tours"
         sql = f"SELECT * FROM {table}"
 
+        engine = create_engine(conn_string)
         try:
-            tours.as_tours.to_postgis(table, conn_string)
-            tours_db = ti.io.read_tours_postgis(sql, conn_string, index_col="id")
+            tours.as_tours.to_postgis(table, engine)
+            with pytest.warns(UserWarning):
+                tours_db = ti.io.read_tours_postgis(sql, conn, index_col="id")
             assert_frame_equal(tours, tours_db)
         finally:
             del_table(conn, table)
 
     def test_no_crs(self, example_tours, conn_postgis):
         """Test if writing reading to postgis also works correctly without CRS."""
         tours = example_tours
         conn_string, conn = conn_postgis
         table = "tours"
         sql = f"SELECT * FROM {table}"
+
+        engine = create_engine(conn_string)
         try:
-            tours.as_tours.to_postgis(table, conn_string)
-            tours_db = ti.io.read_tours_postgis(sql, conn_string, index_col="id")
+            tours.as_tours.to_postgis(table, engine)
+            with pytest.warns(UserWarning):
+                tours_db = ti.io.read_tours_postgis(sql, conn, index_col="id")
             assert_frame_equal(tours, tours_db)
         finally:
             del_table(conn, table)
 
 
 class TestGetSrid:
     def test_srid(self, example_positionfixes):
```

### Comparing `trackintel-1.1.9/tests/model/test_locations.py` & `trackintel-1.2.1/tests/model/test_locations.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import trackintel as ti
 
 
 @pytest.fixture
 def testdata_locs():
     """Read location test data from files."""
     sp_file = os.path.join("tests", "data", "geolife", "geolife_staypoints.csv")
-    sp = ti.read_staypoints_csv(sp_file, tz="utc", index_col="id")
+    sp = ti.read_staypoints_csv(sp_file, tz="utc", index_col="id", crs="epsg:4326")
     sp, locs = sp.as_staypoints.generate_locations(
         method="dbscan", epsilon=10, num_samples=1, distance_metric="haversine", agg_level="dataset"
     )
     return locs
 
 
 class TestLocations:
```

### Comparing `trackintel-1.1.9/tests/model/test_positionfixes.py` & `trackintel-1.2.1/tests/model/test_positionfixes.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             pfs.drop(["user_id"], axis=1).as_positionfixes
 
     def test_accessor_geometry(self, testdata_geolife):
         """Test if the as_positionfixes accessor requires geometry column."""
         pfs = testdata_geolife.copy()
 
         # check geometry
-        with pytest.raises(AttributeError, match="No geometry data set yet"):
+        with pytest.raises(AttributeError):
             pfs.drop(["geom"], axis=1).as_positionfixes
 
     def test_accessor_geometry_type(self, testdata_geolife):
         """Test if the as_positionfixes accessor requires Point geometry."""
         pfs = testdata_geolife.copy()
 
         # check geometry type
```

### Comparing `trackintel-1.1.9/tests/model/test_staypoints.py` & `trackintel-1.2.1/tests/model/test_staypoints.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             sp.drop(["user_id"], axis=1).as_staypoints
 
     def test_accessor_geometry(self, testdata_sp):
         """Test if the as_staypoints accessor requires geometry column."""
         sp = testdata_sp.copy()
 
         # geometery
-        with pytest.raises(AttributeError, match="No geometry data set yet"):
+        with pytest.raises(AttributeError):
             sp.drop(["geom"], axis=1).as_staypoints
 
     def test_accessor_geometry_type(self, testdata_sp):
         """Test if the as_staypoints accessor requires Point geometry."""
         sp = testdata_sp.copy()
 
         # check geometry type
```

### Comparing `trackintel-1.1.9/tests/model/test_triplegs.py` & `trackintel-1.2.1/tests/model/test_triplegs.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             tpls.drop(["user_id"], axis=1).as_triplegs
 
     def test_accessor_geometry(self, testdata_tpls):
         """Test if the as_triplegs accessor requires geometry column."""
         tpls = testdata_tpls.copy()
 
         # check geometry
-        with pytest.raises(AttributeError, match="No geometry data set yet"):
+        with pytest.raises(AttributeError):
             tpls.drop(["geom"], axis=1).as_triplegs
 
     def test_accessor_geometry_type(self, testdata_tpls):
         """Test if the as_triplegs accessor requires LineString geometry."""
         tpls = testdata_tpls.copy()
 
         # check geometry type
```

### Comparing `trackintel-1.1.9/tests/model/test_trips.py` & `trackintel-1.2.1/tests/model/test_trips.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/tests/model/test_util.py` & `trackintel-1.2.1/tests/model/test_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,22 +135,22 @@
     def test_accessor(self, example_triplegs):
         """Test whether the accessor yields the same output as the function"""
         pfs, tpls = example_triplegs
         tpls_speed_acc = tpls.as_triplegs.get_speed(pfs, method="pfs_mean_speed")
         tpls_speed_normal = ti.model.util.get_speed_triplegs(tpls, pfs, method="pfs_mean_speed")
         assert_geodataframe_equal(tpls_speed_acc, tpls_speed_normal)
 
-    def test_pfs_exist_assertion(self, example_triplegs):
+    def test_pfs_input_assertion(self, example_triplegs):
         """Test whether an AttributeError is raised if no positionfixes are provided as input"""
         error_msg = 'Method "pfs_mean_speed" requires positionfixes as input.'
         _, tpls = example_triplegs
         with pytest.raises(AttributeError, match=error_msg):
             ti.model.util.get_speed_triplegs(tpls, None, method="pfs_mean_speed")
 
-    def test_tripleg_id_assertion(self, example_triplegs):
+    def test_pfs_tripleg_id_assertion(self, example_triplegs):
         """Test whether an AttributeError is raised if positionfixes do not provide column "tripleg_id"."""
         error_msg = 'Positionfixes must include column "tripleg_id".'
         pfs, tpls = example_triplegs
         pfs.drop(columns=["tripleg_id"], inplace=True)
         with pytest.raises(AttributeError, match=error_msg):
             ti.model.util.get_speed_triplegs(tpls, pfs, method="pfs_mean_speed")
```

### Comparing `trackintel-1.1.9/tests/preprocessing/test_filter.py` & `trackintel-1.2.1/tests/preprocessing/test_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 @pytest.fixture
 def locs_from_geolife():
     """Create locations from geolife staypoints."""
     # read staypoints
     sp_file = os.path.join("tests", "data", "geolife", "geolife_staypoints.csv")
-    sp = ti.read_staypoints_csv(sp_file, tz="utc", index_col="id")
+    sp = ti.read_staypoints_csv(sp_file, tz="utc", index_col="id", crs="epsg:4326")
 
     # cluster staypoints to locations
     _, locs = sp.as_staypoints.generate_locations(
         method="dbscan", epsilon=10, num_samples=1, distance_metric="haversine", agg_level="dataset"
     )
 
     # the projection needs to be defined: WGS84
@@ -26,19 +26,18 @@
 class TestSpatial_filter:
     """Tests for the spatial_filter function."""
 
     def test_filter_staypoints(self):
         """Test if spatial_filter works for staypoints."""
         # read staypoints and area file
         sp_file = os.path.join("tests", "data", "geolife", "geolife_staypoints.csv")
-        sp = ti.read_staypoints_csv(sp_file, tz="utc", index_col="id")
+        sp = ti.read_staypoints_csv(sp_file, tz="utc", index_col="id", crs="epsg:4326")
         extent = gpd.read_file(os.path.join("tests", "data", "area", "tsinghua.geojson"))
 
         # the projection needs to be defined: WGS84
-        sp.crs = "epsg:4326"
         within_sp = sp.as_staypoints.spatial_filter(areas=extent, method="within", re_project=True)
         intersects_sp = sp.as_staypoints.spatial_filter(areas=extent, method="intersects", re_project=True)
         crosses_sp = sp.as_staypoints.spatial_filter(areas=extent, method="crosses", re_project=True)
 
         # the result obtained from ArcGIS
         gis_within_num = 13
 
@@ -50,19 +49,18 @@
         # For staypoints the result of within and intersects should be the same
         assert_geodataframe_equal(within_sp, intersects_sp, check_less_precise=True)
 
     def test_filter_triplegs(self):
         """Test if spatial_filter works for triplegs."""
         # read triplegs and area file
         tpls_file = os.path.join("tests", "data", "geolife", "geolife_triplegs.csv")
-        tpls = ti.read_triplegs_csv(tpls_file, tz="utc", index_col="id")
+        tpls = ti.read_triplegs_csv(tpls_file, tz="utc", index_col="id", crs="epsg:4326")
         extent = gpd.read_file(os.path.join("tests", "data", "area", "tsinghua.geojson"))
 
         # the projection needs to be defined: WGS84
-        tpls.crs = "epsg:4326"
         within_tl = tpls.as_triplegs.spatial_filter(areas=extent, method="within", re_project=True)
         intersects_tl = tpls.as_triplegs.spatial_filter(areas=extent, method="intersects", re_project=True)
         crosses_tl = tpls.as_triplegs.spatial_filter(areas=extent, method="crosses", re_project=True)
 
         # the result obtained from ArcGIS
         gis_within_num = 9
         gis_intersects_num = 20
@@ -77,15 +75,15 @@
             "The crosses tripleg number"
             + "should equal the number of intersect triplegs minus the number of within triplegs"
         )
 
     def test_filter_locations(self, locs_from_geolife):
         """Test if spatial_filter works for locations."""
         locs = locs_from_geolife
-        extent = gpd.read_file(os.path.join("tests", "data", "area", "tsinghua.geojson"))
+        extent = gpd.read_file(os.path.join("tests", "data", "area", "tsinghua.geojson"), crs="epsg:4326")
 
         # filter locations with the area
         within_loc = locs.as_locations.spatial_filter(areas=extent, method="within", re_project=True)
         intersects_loc = locs.as_locations.spatial_filter(areas=extent, method="intersects", re_project=True)
         crosses_loc = locs.as_locations.spatial_filter(areas=extent, method="crosses", re_project=True)
 
         # the result obtained from ArcGIS
```

### Comparing `trackintel-1.1.9/tests/preprocessing/test_positionfixes.py` & `trackintel-1.2.1/tests/preprocessing/test_positionfixes.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,44 +170,46 @@
         )
         assert len(sp) == len(pfs)
 
     def test_sliding_max(self):
         """Test if using large thresholds, stp extraction yield no pfs."""
         pfs, _ = ti.io.dataset_reader.read_geolife(os.path.join("tests", "data", "geolife"))
         warn_string = "No staypoints can be generated, returning empty sp."
+        max_time = pd.Timedelta.max.total_seconds() // 60
         with pytest.warns(UserWarning, match=warn_string):
             _, sp = pfs.as_positionfixes.generate_staypoints(
-                method="sliding", dist_threshold=sys.maxsize, time_threshold=sys.maxsize
+                method="sliding", dist_threshold=sys.maxsize, time_threshold=max_time
             )
         assert len(sp) == 0
 
     def test_missing_link(self):
         """Test nan is assigned for missing link between pfs and sp."""
         pfs, _ = ti.io.dataset_reader.read_geolife(os.path.join("tests", "data", "geolife"))
         warn_string = "No staypoints can be generated, returning empty sp."
+        max_time = pd.Timedelta.max.total_seconds() // 60
         with pytest.warns(UserWarning, match=warn_string):
             pfs, _ = pfs.as_positionfixes.generate_staypoints(
-                method="sliding", dist_threshold=sys.maxsize, time_threshold=sys.maxsize
+                method="sliding", dist_threshold=sys.maxsize, time_threshold=max_time
             )
 
-        assert pd.isna(pfs["staypoint_id"]).any()
+        assert pd.isna(pfs["staypoint_id"]).all()
 
     def test_dtype_consistent(self, geolife_pfs_sp_long):
         """Test the dtypes for the generated columns."""
         pfs, sp = geolife_pfs_sp_long
 
         assert pfs["user_id"].dtype == sp["user_id"].dtype
         assert pfs["staypoint_id"].dtype == "Int64"
         assert sp.index.dtype == "int64"
 
     def test_index_start(self, geolife_pfs_sp_long):
         """Test the generated index start from 0 for different methods."""
         _, sp = geolife_pfs_sp_long
 
-        assert (sp.index == np.arange(len(sp))).any()
+        assert (sp.index == np.arange(len(sp))).all()
 
     def test_include_last(self):
         """Test if the include_last arguement will include the last pfs as stp."""
         pfs, _ = ti.io.dataset_reader.read_geolife(os.path.join("tests", "data", "geolife"))
 
         pfs_wo, sp_wo = pfs.as_positionfixes.generate_staypoints(
             method="sliding", dist_threshold=100, time_threshold=5.0, include_last=False
@@ -274,28 +276,57 @@
                 "latitude": 39.975818526,
                 "longitude": 116.331600228,
                 "tracked_at": Timestamp("2011-08-03 09:12:52+0000", tz="UTC"),
                 "user_id": 55,
             },
         ]
         df = pd.DataFrame(pfs_dict)
-        pfs = gpd.GeoDataFrame(df, geometry=gpd.points_from_xy(df.longitude, df.latitude))
+        pfs = gpd.GeoDataFrame(df, geometry=gpd.points_from_xy(df.longitude, df.latitude), crs="epsg:4326")
         pfs.as_positionfixes
 
         # using the default gap_threshold will generate no sp
         warn_string = "No staypoints can be generated, returning empty sp."
         with pytest.warns(UserWarning, match=warn_string):
             _, sp = pfs.as_positionfixes.generate_staypoints(include_last=True)
             assert len(sp) == 0
 
         # using large gap_threshold one sp will be generated
         _, sp = pfs.as_positionfixes.generate_staypoints(gap_threshold=1e8, include_last=True)
         assert len(sp) == 1
 
 
+class Test_Generate_staypoints_sliding_user:
+    """Test for _generate_staypoints_sliding_user."""
+
+    def test_unknown_distance_metric(self, example_positionfixes):
+        """Test if the distance metric is unknown, an AttributeError will be raised."""
+        with pytest.raises(AttributeError):
+            example_positionfixes.as_positionfixes.generate_staypoints(
+                method="sliding", dist_threshold=100, time_threshold=5, distance_metric="unknown"
+            )
+
+
+class Test__create_new_staypoints:
+    """Test __create_new_staypoints."""
+
+    def test_planar_crs(self, geolife_pfs_sp_long):
+        """Test if planar crs are handled as well"""
+        pfs, _ = geolife_pfs_sp_long
+        _, sp_wgs84 = pfs.as_positionfixes.generate_staypoints(
+            method="sliding", dist_threshold=100, time_threshold=5.0, include_last=True
+        )
+        pfs = pfs.set_crs(2056, allow_override=True)
+        _, sp_lv95 = pfs.as_positionfixes.generate_staypoints(
+            method="sliding", dist_threshold=100, time_threshold=5.0, include_last=True
+        )
+        sp_lv95.set_crs(4326, allow_override=True, inplace=True)
+        # planar and non-planar differ only if we experience a wrap in coords like [+180, -180]
+        assert_geodataframe_equal(sp_wgs84, sp_lv95, check_less_precise=True)
+
+
 class TestGenerate_triplegs:
     """Tests for generate_triplegs() method."""
 
     def test_empty_generation(self, example_positionfixes_isolated):
         """The function should run without error if the generation result is empty (no tripleg could be generated)."""
         pfs = example_positionfixes_isolated
```

### Comparing `trackintel-1.1.9/tests/preprocessing/test_staypoints.py` & `trackintel-1.2.1/tests/preprocessing/test_staypoints.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 import pytest
 from shapely.geometry import Point
 from sklearn.cluster import DBSCAN
-from geopandas.testing import assert_geodataframe_equal
+from geopandas.testing import assert_geodataframe_equal, assert_geoseries_equal
 
 import trackintel as ti
 from trackintel.geogr.distances import calculate_distance_matrix
 
 
 @pytest.fixture
 def example_staypoints():
@@ -34,15 +34,14 @@
 
     t1 = pd.Timestamp("1971-01-01 00:00:00", tz="utc")
     t2 = pd.Timestamp("1971-01-01 05:00:00", tz="utc")
     t3 = pd.Timestamp("1971-01-02 07:00:00", tz="utc")
     t4 = pd.Timestamp("1971-01-02 08:00:00", tz="utc")
     t5 = pd.Timestamp("1971-01-02 09:00:00", tz="utc")
     t6 = pd.Timestamp("1971-01-02 10:00:00", tz="utc")
-    one_hour = datetime.timedelta(hours=1)
 
     list_dict = [
         {"id": 1, "user_id": 0, "started_at": t1, "finished_at": t2, "geom": p1},
         {"id": 5, "user_id": 0, "started_at": t2, "finished_at": t3, "geom": p2},
         {"id": 2, "user_id": 0, "started_at": t3, "finished_at": t4, "geom": p3},
         {"id": 6, "user_id": 0, "started_at": t4, "finished_at": t5, "geom": p2},
         {"id": 15, "user_id": 0, "started_at": t5, "finished_at": t6, "geom": p1},
@@ -70,15 +69,14 @@
     t1 = pd.Timestamp("1971-01-01 00:00:00", tz="utc")
     t2 = pd.Timestamp("1971-01-02 05:00:00", tz="utc")
     t3 = pd.Timestamp("1971-01-02 06:45:00", tz="utc")
     t4 = pd.Timestamp("1971-01-02 08:55:00", tz="utc")
     t45 = pd.Timestamp("1971-01-02 08:57:00", tz="utc")
     t5 = pd.Timestamp("1971-01-02 09:00:00", tz="utc")
     t6 = pd.Timestamp("1971-01-02 09:20:00", tz="utc")
-    one_hour = datetime.timedelta(hours=1)
 
     list_dict = [
         {"id": 1, "user_id": 0, "started_at": t1, "finished_at": t2, "geom": p1, "location_id": 1},
         {"id": 5, "user_id": 0, "started_at": t2, "finished_at": t2, "geom": p1, "location_id": 2},
         {"id": 2, "user_id": 0, "started_at": t3, "finished_at": t4, "geom": p1, "location_id": 2},
         {"id": 6, "user_id": 0, "started_at": t4, "finished_at": t45, "geom": p1, "location_id": 2},
         {"id": 15, "user_id": 0, "started_at": t5, "finished_at": t6, "geom": p1, "location_id": 2},
@@ -86,16 +84,16 @@
         {"id": 80, "user_id": 1, "started_at": t45, "finished_at": t5, "geom": p1, "location_id": 2},
         {"id": 3, "user_id": 1, "started_at": t5, "finished_at": t6, "geom": p1, "location_id": 4},
     ]
     sp = gpd.GeoDataFrame(data=list_dict, geometry="geom", crs="EPSG:4326")
     sp = sp.set_index("id")
     assert sp.as_staypoints
 
-    # generate example triplegs for the merge function
-    tpls = gpd.GeoDataFrame(columns=["user_id", "started_at", "finished_at"])
+    # generate empty triplegs for the merge function
+    tpls = pd.DataFrame([], columns=["user_id", "started_at", "finished_at"])
     return sp, tpls
 
 
 @pytest.fixture
 def example_triplegs_merge(example_staypoints_merge):
     """Example triplegs for merge operation
     If tripleg is between two staypoint, we don't merge those staypoints
@@ -111,15 +109,15 @@
     t45 = pd.Timestamp("1971-01-02 08:57:00", tz="utc")
     t5 = pd.Timestamp("1971-01-02 09:00:00", tz="utc")
     list_dict = [
         {"id": 0, "user_id": 0, "started_at": t45, "finished_at": t5},
         {"id": 1, "user_id": 0, "started_at": t21, "finished_at": t22},
     ]
     # geometry is not required for the merge operation, so we leave it away
-    tpls = gpd.GeoDataFrame(data=list_dict)
+    tpls = pd.DataFrame(data=list_dict)
     tpls = tpls.set_index("id")
     return sp, tpls
 
 
 class TestGenerate_locations:
     """Tests for generate_locations() method."""
 
@@ -153,15 +151,15 @@
         # the result of parallel computing should be identical
         assert_geodataframe_equal(locs_ori, locs_para)
         assert_geodataframe_equal(sp_ori, sp_para)
 
     def test_dbscan_hav_euc(self):
         """Test if using haversine and euclidean distances will generate the same location result."""
         sp_file = os.path.join("tests", "data", "geolife", "geolife_staypoints.csv")
-        sp = ti.read_staypoints_csv(sp_file, tz="utc", index_col="id")
+        sp = ti.read_staypoints_csv(sp_file, tz="utc", index_col="id", crs="epsg:4326")
 
         # haversine calculation
         _, loc_har = sp.as_staypoints.generate_locations(
             method="dbscan", epsilon=100, num_samples=1, distance_metric="haversine", agg_level="dataset"
         )
         # WGS_1984
         sp.crs = "epsg:4326"
@@ -174,15 +172,15 @@
         )
 
         assert len(loc_har) == len(loc_eu)
 
     def test_dbscan_haversine(self):
         """Test haversine dbscan location result with manually calling the DBSCAN method."""
         sp_file = os.path.join("tests", "data", "geolife", "geolife_staypoints.csv")
-        sp = ti.read_staypoints_csv(sp_file, tz="utc", index_col="id")
+        sp = ti.read_staypoints_csv(sp_file, tz="utc", index_col="id", crs="epsg:4326")
 
         # haversine calculation using sklearn.metrics.pairwise_distances
         sp, locs = sp.as_staypoints.generate_locations(
             method="dbscan", epsilon=10, num_samples=1, distance_metric="haversine", agg_level="dataset"
         )
 
         # calculate pairwise haversine matrix and fed to dbscan
@@ -191,15 +189,15 @@
         labels = db.fit_predict(sp_distance_matrix)
 
         assert len(set(locs.index)) == len(set(labels))
 
     def test_dbscan_loc(self):
         """Test haversine dbscan location result with manually grouping the locations method."""
         sp_file = os.path.join("tests", "data", "geolife", "geolife_staypoints.csv")
-        sp = ti.read_staypoints_csv(sp_file, tz="utc", index_col="id")
+        sp = ti.read_staypoints_csv(sp_file, tz="utc", index_col="id", crs="epsg:4326")
         sp, locs = sp.as_staypoints.generate_locations(
             method="dbscan", epsilon=10, num_samples=1, distance_metric="haversine", agg_level="dataset"
         )
 
         # create locations as grouped staypoints, another way to create locations
         other_locs = []
         grouped_df = sp.groupby(["user_id", "location_id"])
@@ -215,21 +213,20 @@
                 # point geometry of place
                 temp_loc["center"] = Point(group.geometry.x.mean(), group.geometry.y.mean())
                 other_locs.append(temp_loc)
 
         other_locs = gpd.GeoDataFrame(other_locs, columns=["user_id", "id", "center"], geometry="center", crs=sp.crs)
         other_locs.set_index("id", inplace=True)
 
-        assert all(other_locs["center"] == locs["center"])
-        assert all(other_locs.index == locs.index)
+        assert_geoseries_equal(other_locs["center"], locs["center"], check_less_precise=True)
 
     def test_dbscan_user_dataset(self):
         """Test user and dataset location generation."""
         sp_file = os.path.join("tests", "data", "geolife", "geolife_staypoints.csv")
-        sp = ti.read_staypoints_csv(sp_file, tz="utc", index_col="id")
+        sp = ti.read_staypoints_csv(sp_file, tz="utc", index_col="id", crs="epsg:4326")
         # take the first row and duplicate once
         sp = sp.head(1)
         sp = pd.concat([sp, sp], ignore_index=True)
         # assign a different user_id to the second row
         sp.iloc[1, 4] = 1
 
         # duplicate for a certain number
@@ -241,18 +238,24 @@
             method="dbscan", epsilon=10, num_samples=1, distance_metric="haversine", agg_level="user"
         )
         loc_dataset_num = len(locs_ds.index.unique())
         loc_user_num = len(locs_us.index.unique())
         assert loc_dataset_num == 1
         assert loc_user_num == 2
 
+    def test_crs(self, example_staypoints):
+        """Test whether the crs of the output locations is set correctly."""
+        sp = example_staypoints
+        sp, locs = sp.as_staypoints.generate_locations(method="dbscan", epsilon=20, num_samples=1)
+        assert locs.crs == sp.crs
+
     def test_dbscan_min(self):
         """Test with small epsilon parameter."""
         pfs_file = os.path.join("tests", "data", "positionfixes.csv")
-        pfs = ti.read_positionfixes_csv(pfs_file, sep=";", tz="utc", index_col="id")
+        pfs = ti.read_positionfixes_csv(pfs_file, sep=";", tz="utc", index_col="id", crs="epsg:4326")
         _, sp = pfs.as_positionfixes.generate_staypoints(
             method="sliding", gap_threshold=1e6, dist_threshold=0, time_threshold=0
         )
         _, locs_user = sp.as_staypoints.generate_locations(
             method="dbscan", epsilon=1e-18, num_samples=1, agg_level="user"
         )
         _, locs_data = sp.as_staypoints.generate_locations(
@@ -261,15 +264,15 @@
         # With small hyperparameters, clustering should not reduce the number
         assert len(locs_user) == len(sp)
         assert len(locs_data) == len(sp)
 
     def test_dbscan_max(self):
         """Test with large epsilon parameter."""
         pfs_file = os.path.join("tests", "data", "positionfixes.csv")
-        pfs = ti.read_positionfixes_csv(pfs_file, sep=";", tz="utc", index_col="id")
+        pfs = ti.read_positionfixes_csv(pfs_file, sep=";", tz="utc", index_col="id", crs="epsg:4326")
         _, sp = pfs.as_positionfixes.generate_staypoints(
             method="sliding", gap_threshold=1e6, dist_threshold=0, time_threshold=0
         )
         warn_string = "No locations can be generated, returning empty locs."
         with pytest.warns(UserWarning, match=warn_string):
             _, locs_user = sp.as_staypoints.generate_locations(
                 method="dbscan", epsilon=1e18, num_samples=1000, agg_level="user"
@@ -280,30 +283,30 @@
         # "With large epsilon, every user location is an outlier"
         assert len(locs_user) == 0
         assert len(locs_data) == 0
 
     def test_missing_link(self):
         """Test nan is assigned for missing link between sp and locs."""
         pfs_file = os.path.join("tests", "data", "positionfixes.csv")
-        pfs = ti.read_positionfixes_csv(pfs_file, sep=";", tz="utc", index_col="id")
+        pfs = ti.read_positionfixes_csv(pfs_file, sep=";", tz="utc", index_col="id", crs="epsg:4326")
         _, sp = pfs.as_positionfixes.generate_staypoints(
             method="sliding", gap_threshold=1e6, dist_threshold=0, time_threshold=0
         )
         warn_string = "No locations can be generated, returning empty locs."
         with pytest.warns(UserWarning, match=warn_string):
             sp, _ = sp.as_staypoints.generate_locations(
                 method="dbscan", epsilon=1e18, num_samples=1000, agg_level="user"
             )
 
         assert pd.isna(sp["location_id"]).any()
 
     def test_num_samples_high(self):
         """Test higher values of num_samples for generate_locations."""
         sp_file = os.path.join("tests", "data", "geolife", "geolife_staypoints.csv")
-        sp = ti.read_staypoints_csv(sp_file, tz="utc", index_col="id")
+        sp = ti.read_staypoints_csv(sp_file, tz="utc", index_col="id", crs="epsg:4326")
         sp_ns_5, _ = sp.as_staypoints.generate_locations(
             epsilon=50, distance_metric="haversine", agg_level="user", num_samples=2
         )
         non_noise_sp = sp_ns_5[sp_ns_5["location_id"] != -1]
 
         # group_by_user_id and check that no two different user ids share a common location id
         grouped = list(non_noise_sp.groupby(["user_id"])["location_id"].unique())
@@ -311,18 +314,51 @@
         for loc_list in grouped:
             loc_set.append(set(loc_list))
 
         # we assert that the count of overlaps is equal to the count of users
         # (each user has overlap with the same user)
         assert sum([int(len(p & q) > 0) for p in loc_set for q in loc_set]) == len(loc_set)
 
+    def test_num_samples_3(self):
+        """Test with num_samples=3 to check if fully false pointLine_idx causes no error."""
+        sp_file = os.path.join("tests", "data", "geolife", "geolife_staypoints.csv")
+        sp = ti.read_staypoints_csv(sp_file, tz="utc", index_col="id", crs="epsg:4326")
+        # generate locations with num_samples=1 and num_samples=3 creates the same locations
+        # but locations with only one or two staypoint are filtered out in the second run
+        sp1, locs1 = sp.as_staypoints.generate_locations(
+            num_samples=1, distance_metric="haversine", agg_level="dataset"
+        )
+        sp3, locs3 = sp.as_staypoints.generate_locations(
+            num_samples=3, distance_metric="haversine", agg_level="dataset"
+        )
+        # get all location_ids with less than 3 staypoints
+        f = sp1["location_id"].value_counts(dropna=False) < 3
+        f = f[f].index  # get set of locations with less than 3 staypoints
+        locs1 = locs1.iloc[locs1.index.difference(f)]  # drop locations with less than 3 staypoints
+        locs1 = locs1.reset_index(drop=True)  # reset index to remove offset
+        locs1.index.name = "id"  # reset index name
+        assert_geodataframe_equal(locs1, locs3)
+        map_dict = {}
+        next_loc_id = 0
+        for i, row in sp1.iterrows():
+            val = row["location_id"]
+            if val in f:  # means we have less than 3 staypoints
+                sp1.at[i, "location_id"] = np.nan
+            else:
+                # remove offset we have in counting more locations
+                if val not in map_dict:
+                    map_dict[val] = next_loc_id
+                    next_loc_id += 1
+                sp1.at[i, "location_id"] = map_dict[val]
+        assert_geodataframe_equal(sp1, sp3)
+
     def test_dtype_consistent(self):
         """Test the dtypes for the generated columns."""
         sp_file = os.path.join("tests", "data", "geolife", "geolife_staypoints.csv")
-        sp = ti.read_staypoints_csv(sp_file, tz="utc", index_col="id")
+        sp = ti.read_staypoints_csv(sp_file, tz="utc", index_col="id", crs="epsg:4326")
         #
         sp, locs = sp.as_staypoints.generate_locations(
             method="dbscan", epsilon=10, num_samples=1, distance_metric="haversine", agg_level="dataset"
         )
         assert sp["user_id"].dtype == locs["user_id"].dtype
         assert sp["location_id"].dtype == "Int64"
         assert locs.index.dtype == "int64"
@@ -334,29 +370,32 @@
         assert sp["user_id"].dtype == locs["user_id"].dtype
         assert sp["location_id"].dtype == "Int64"
         assert locs.index.dtype == "int64"
 
     def test_index_start(self):
         """Test the generated index start from 0 for different methods."""
         sp_file = os.path.join("tests", "data", "geolife", "geolife_staypoints.csv")
-        sp = ti.read_staypoints_csv(sp_file, tz="utc", index_col="id")
+        sp = ti.read_staypoints_csv(sp_file, tz="utc", index_col="id", crs="epsg:4326")
+
+        # reproject to WGS_1984_UTM_Zone_49N
+        sp = sp.to_crs("epsg:32649")
 
         distance_metric_ls = ["haversine", "euclidean"]
         agg_level_ls = ["dataset", "user"]
         for distance_metric in distance_metric_ls:
             for agg_level in agg_level_ls:
                 _, locations = sp.as_staypoints.generate_locations(
                     method="dbscan", epsilon=10, num_samples=1, distance_metric=distance_metric, agg_level=agg_level
                 )
                 assert (locations.index == np.arange(len(locations))).any()
 
     def test_print_progress_flag(self, capsys):
         """Test if the print_progress bar controls the printing behavior."""
         file = os.path.join("tests", "data", "geolife", "geolife_staypoints.csv")
-        staypoints = ti.read_staypoints_csv(file, tz="utc", index_col="id")
+        staypoints = ti.read_staypoints_csv(file, tz="utc", index_col="id", crs="epsg:4326")
 
         staypoints.as_staypoints.generate_locations(print_progress=True)
         captured_print = capsys.readouterr()
         assert captured_print.err != ""
 
         staypoints.as_staypoints.generate_locations(print_progress=False)
         captured_print = capsys.readouterr()
@@ -395,14 +434,30 @@
 
         assert (sp2.loc[[5, 6, 80, 3], "location_id"] == sp2.loc[5, "location_id"]).all()
         assert sp2.loc[1, "location_id"] == sp2.loc[15, "location_id"]
         assert sp2.loc[1, "location_id"] != sp2.loc[5, "location_id"]
 
         assert sp2.loc[[2, 7], "location_id"].isnull().all()
 
+    def test_agg_level_error(self, example_staypoints):
+        """Test if unknown "agg_level" raises AttributeError"""
+        agg_level = "unknown"
+        error_msg = f"agg_level '{agg_level}' is unknown. Supported values are ['user', 'dataset']."
+        with pytest.raises(AttributeError) as e:
+            example_staypoints.as_staypoints.generate_locations(method="dbscan", agg_level="unkown")
+            assert error_msg == str(e.value)
+
+    def test_method_error(self, example_staypoints):
+        """Test if unknown "method" raises AttributeError"""
+        method = "unknown"
+        error_msg = f"method '{method}' is unknown. Supported values are ['dbscan']."
+        with pytest.raises(AttributeError) as e:
+            example_staypoints.as_staypoints.generate_locations(method="unknown")
+            assert error_msg == str(e.value)
+
 
 class TestMergeStaypoints:
     def test_merge_staypoints(self, example_staypoints_merge):
         """Test staypoint merging."""
         sp, tpls = example_staypoints_merge
         # first test with empty tpls
         merged_sp = sp.as_staypoints.merge_staypoints(tpls, agg={"geom": "first"})
@@ -443,15 +498,15 @@
         assert sp.loc[5, "started_at"] == merged_sp.loc[5, "started_at"]
         assert sp.loc[15, "finished_at"] == merged_sp.loc[5, "finished_at"]
 
     def test_merge_staypoints_time_gap_error(self, example_staypoints_merge):
         sp, tpls = example_staypoints_merge
         # check that an int as max time gap raises a TypeError
         with pytest.raises(Exception) as e_info:
-            merged_sp = sp.as_staypoints.merge_staypoints(tpls, max_time_gap=2)
+            sp.as_staypoints.merge_staypoints(tpls, max_time_gap=2)
             assert e_info == "Parameter max_time_gap must be either of type String or pd.Timedelta!"
         # check that an timedelta as max time gap works
         _ = sp.as_staypoints.merge_staypoints(tpls, max_time_gap=pd.to_timedelta("1h"))
 
     def test_merge_staypoints_agg(self, example_staypoints_merge):
         """Test whether the user can specify the aggregation mode"""
         aggregation_dict = {"geom": "first", "finished_at": "first"}
```

### Comparing `trackintel-1.1.9/tests/preprocessing/test_triplegs.py` & `trackintel-1.2.1/tests/preprocessing/test_triplegs.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,26 +56,26 @@
         assert set(tpls_run_1.columns) == set(tpls_run_2.columns)
         assert set(sp_run_1.columns) == set(sp_run_2.columns)
 
     def test_generate_trips(self, example_triplegs_higher_gap_threshold):
         """Test if we can generate the example trips based on example data."""
         # load pregenerated trips
         path = os.path.join("tests", "data", "geolife_long", "trips.csv")
-        trips_loaded = ti.read_trips_csv(path, index_col="id", geom_col="geom", crs=None)
+        trips_loaded = ti.read_trips_csv(path, index_col="id", geom_col="geom", crs="EPSG:4326")
 
         # create trips from geolife (based on positionfixes) - with gap_threshold 1e6
         sp, tpls = example_triplegs_higher_gap_threshold
 
         # generate trips and a joint staypoint/triplegs dataframe
         sp, tpls, trips = generate_trips(sp, tpls, gap_threshold=15)
         trips = trips[
             ["user_id", "started_at", "finished_at", "origin_staypoint_id", "destination_staypoint_id", "geom"]
         ]
         # test if generated trips are equal
-        assert_geodataframe_equal(trips_loaded, trips)
+        assert_geodataframe_equal(trips_loaded, trips, check_less_precise=True)
 
     def test_trip_wo_geom(self, example_triplegs_higher_gap_threshold):
         """Test if the add_geometry parameter shows correct behavior"""
         sp, tpls = example_triplegs_higher_gap_threshold
 
         # generate trips dataframe with geometry
         _, _, trips = generate_trips(sp, tpls, gap_threshold=15)
@@ -222,27 +222,25 @@
 
         # load data and add dummy geometry
         sp_in = pd.read_csv(
             os.path.join("tests", "data", "trips", "staypoints_gaps.csv"),
             sep=";",
             index_col="id",
             parse_dates=[0, 1],
-            infer_datetime_format=True,
             dayfirst=True,
         )
         sp_in["geom"] = Point(1, 1)
         sp_in = gpd.GeoDataFrame(sp_in, geometry="geom")
         sp_in = ti.io.read_staypoints_gpd(sp_in, tz="utc")
 
         tpls_in = pd.read_csv(
             os.path.join("tests", "data", "trips", "triplegs_gaps.csv"),
             sep=";",
             index_col="id",
             parse_dates=[0, 1],
-            infer_datetime_format=True,
             dayfirst=True,
         )
         tpls_in["geom"] = LineString([[1, 1], [2, 2]])
         tpls_in = gpd.GeoDataFrame(tpls_in, geometry="geom")
         tpls_in = ti.io.read_triplegs_gpd(tpls_in, tz="utc")
 
         # load ground truth data
@@ -369,26 +367,55 @@
         """Tests is AttributeError is raised on missing "is_activity" column of staypoints."""
         sp, tpls = example_triplegs
         sp.drop(columns="is_activity", inplace=True)
         error_msg = "staypoints need the column 'is_activity' to be able to generate trips"
         with pytest.raises(AttributeError, match=error_msg):
             generate_trips(sp, tpls)
 
+    def test_crs(self, example_triplegs):
+        """Test that the resulting GeoDataFrame has the correct crs or a warning or error is thrown if not set"""
+        sp, tpls = example_triplegs
+        # Case 1: sp crs None --> throw warning and set to tpls crs
+        sp.crs = None
+        with pytest.warns(UserWarning):
+            _, _, trips = generate_trips(sp, tpls)
+            assert trips.crs == tpls.crs
+        # Case 2: Both crs None --> warn and set to None
+        tpls.crs = None
+        with pytest.warns(UserWarning):
+            _, _, trips = generate_trips(sp, tpls)
+            assert trips.crs is None
+        # Case 3: tpls crs is None --> throw warning and set to sp crs
+        sp.crs = "EPSG:4326"
+        with pytest.warns(UserWarning):
+            _, _, trips = generate_trips(sp, tpls)
+            assert trips.crs == "EPSG:4326"
+        # Case 4: Both crs set and correspond
+        tpls.crs = "EPSG:2056"
+        sp.crs = "EPSG:2056"
+        _, _, trips = generate_trips(sp, tpls)
+        assert trips.crs == "EPSG:2056"
+        # Case 5: Both crs set but differ --> throw error
+        sp.crs = "EPSG:4326"
+        error_msg = "CRS of staypoints and triplegs differ. Geometry cannot be joined safely."
+        with pytest.raises(AssertionError, match=error_msg):
+            generate_trips(sp, tpls)
+
 
 def _create_debug_sp_tpls_data(sp, tpls, gap_threshold):
     """Preprocess sp and tpls for "test_generate_trips_*."""
     # create table with relevant information from triplegs and staypoints.
     tpls["type"] = "tripleg"
     sp["type"] = "staypoint"
     cols_sp = ["started_at", "finished_at", "user_id", "type", "is_activity", "trip_id", "prev_trip_id", "next_trip_id"]
     cols_tpls = ["started_at", "finished_at", "user_id", "type", "trip_id"]
     sp_tpls = pd.concat((sp[cols_sp], tpls[cols_tpls]))
 
     # transform nan to bool
-    sp_tpls["is_activity"] = sp_tpls["is_activity"] == True
+    sp_tpls["is_activity"] = sp_tpls["is_activity"].__eq__(True)
     sp_tpls.sort_values(by=["user_id", "started_at"], inplace=True)
     sp_tpls["started_at_next"] = sp_tpls["started_at"].shift(-1)
     sp_tpls["activity_next"] = sp_tpls["is_activity"].shift(-1)
 
     sp_tpls["gap"] = (sp_tpls["started_at_next"] - sp_tpls["finished_at"]).dt.seconds / 60 > gap_threshold
 
     return sp_tpls
@@ -464,15 +491,15 @@
         ]
     )
 
     # create ID field from index
     sp_tpls["id"] = sp_tpls.index
 
     # transform nan to bool
-    sp_tpls["is_activity"] = sp_tpls["is_activity"] == True
+    sp_tpls["is_activity"] = sp_tpls["is_activity"].__eq__(True)
 
     sp_tpls.sort_values(by=["user_id", "started_at"], inplace=True)
     sp_tpls["started_at_next"] = sp_tpls["started_at"].shift(-1)
     sp_tpls["is_activity_next"] = sp_tpls["is_activity"].shift(-1)
 
     if print_progress:
         tqdm.pandas(desc="User trip generation")
@@ -553,15 +580,14 @@
     unknown_activity = {"user_id": user_id, "is_activity": True, "id": np.nan}
     origin_activity = unknown_activity
     temp_trip_stack = []
     in_trip = False
     trip_ls = []
 
     for _, row in df.iterrows():
-
         # check if we can start a new trip
         # (we make sure that we start the trip with the most recent activity)
         if in_trip is False:
             # If there are several activities in a row, we skip until the last one
             if row["is_activity"] and row["activity_next"]:
                 continue
 
@@ -577,15 +603,14 @@
 
         if in_trip is True:
             # during trip generation/recording
 
             # check if trip ends regularly
             is_gap = row["started_at_next"] - row["finished_at"] > datetime.timedelta(minutes=gap_threshold)
             if row["is_activity"] is True:
-
                 # if there are no triplegs in the trip, set the current activity as origin and start over
                 if not _check_trip_stack_has_tripleg(temp_trip_stack):
                     origin_activity = row
                     temp_trip_stack = list()
                     in_trip = True
 
                 else:
@@ -700,17 +725,17 @@
     first_trip_element = temp_trip_stack[0]
     last_trip_element = temp_trip_stack[-1]
 
     # all data has to be from the same user
     assert origin_activity["user_id"] == last_trip_element["user_id"]
 
     # double check if trip requirements are fulfilled
-    assert origin_activity["is_activity"] == True
-    assert destination_activity["is_activity"] == True
-    assert first_trip_element["is_activity"] == False
+    assert origin_activity["is_activity"] is True
+    assert destination_activity["is_activity"] is True
+    assert first_trip_element["is_activity"] is False
 
     trip_dict_entry = {
         "user_id": origin_activity["user_id"],
         "started_at": first_trip_element["started_at"],
         "finished_at": last_trip_element["finished_at"],
         "origin_staypoint_id": origin_activity["id"],
         "destination_staypoint_id": destination_activity["id"],
```

### Comparing `trackintel-1.1.9/tests/preprocessing/test_trips.py` & `trackintel-1.2.1/tests/preprocessing/test_trips.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,14 +130,15 @@
     start_time_subtour = pd.Timestamp("1971-01-02 08:45:00", tz="utc")
     middle_time = pd.Timestamp("1971-01-02 08:55:00", tz="utc")
     trips.loc[6, "finished_at"] = start_time_subtour
     # trip 6 starts at 8:45 at sp 5, then at 8:45 the user goes to 7 and back to 5
     trips.loc[100] = [0, start_time_subtour, middle_time, 5, 7, first_trip_subtour]
     trips.loc[200] = [0, middle_time, trips.loc[15, "started_at"], 7, 5, second_trip_subtour]
     trips.sort_values(by=["user_id", "started_at", "origin_staypoint_id", "destination_staypoint_id"], inplace=True)
+    trips.set_geometry("geom", crs=4326, inplace=True)
     return trips
 
 
 class TestGenerate_tours:
     """Tests for generate_tours() method."""
 
     def test_generate_tours(self, example_trip_data):
```

### Comparing `trackintel-1.1.9/tests/visualization/test_locations.py` & `trackintel-1.2.1/tests/visualization/test_locations.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/tests/visualization/test_modal_split.py` & `trackintel-1.2.1/tests/visualization/test_modal_split.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/tests/visualization/test_positionfixes.py` & `trackintel-1.2.1/tests/visualization/test_positionfixes.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/tests/visualization/test_staypoints.py` & `trackintel-1.2.1/tests/visualization/test_staypoints.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/tests/visualization/test_triplegs.py` & `trackintel-1.2.1/tests/visualization/test_triplegs.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/tests/visualization/test_util.py` & `trackintel-1.2.1/tests/visualization/test_util.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/trackintel/analysis/__init__.py` & `trackintel-1.2.1/trackintel/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/trackintel/analysis/labelling.py` & `trackintel-1.2.1/trackintel/analysis/labelling.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/trackintel/analysis/location_identification.py` & `trackintel-1.2.1/trackintel/analysis/location_identification.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/trackintel/analysis/modal_split.py` & `trackintel-1.2.1/trackintel/analysis/modal_split.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/trackintel/analysis/tracking_quality.py` & `trackintel-1.2.1/trackintel/analysis/tracking_quality.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     df.reset_index(inplace=True)
 
     # filter out records with duration <= 0
     df["duration"] = (df["finished_at"] - df["started_at"]).dt.total_seconds()
     df = df.loc[df["duration"] > 0].copy()
     # ensure proper handle of empty dataframes
     if len(df) == 0:
-        warnings.warn(f"The input dataframe does not contain any record with positive duration. Please check.")
+        warnings.warn("The input dataframe does not contain any record with positive duration. Please check.")
         return None
 
     if granularity == "all":
         quality = df.groupby("user_id", as_index=False).apply(_get_tracking_quality_user, granularity)
         return quality
 
     # split records that span several days
```

### Comparing `trackintel-1.1.9/trackintel/geogr/distances.py` & `trackintel-1.2.1/trackintel/geogr/distances.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,14 @@
                 D = cdist(xy1, xy2, metric=dist_metric, **kwds)
             else:
                 D = pairwise_distances(xy1, metric=dist_metric, n_jobs=n_jobs)
 
         return D
 
     elif geom_type == "LineString":
-
         if dist_metric in ["dtw", "frechet"]:
             # these are the preparation steps for all distance functions based only on coordinates
 
             if dist_metric == "dtw":
                 d_fun = partial(similaritymeasures.dtw, **kwds)
             else:
                 d_fun = partial(similaritymeasures.frechet_dist, **kwds)
```

### Comparing `trackintel-1.1.9/trackintel/geogr/point_distances.py` & `trackintel-1.2.1/trackintel/geogr/point_distances.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
+import math
 
 
-def haversine_dist(lon_1, lat_1, lon_2, lat_2, r=6371000):
+def haversine_dist(lon_1, lat_1, lon_2, lat_2, r=6371000, float_flag=False):
     """
     Compute the great circle or haversine distance between two coordinates in WGS84.
 
     Serialized version of the haversine distance.
 
     Parameters
     ----------
@@ -21,29 +22,45 @@
     lat_2 : float or numpy.array of shape (-1,)
         The latitude of the second point.
 
     r     : float
         Radius of the reference sphere for the calculation.
         The average Earth radius is 6'371'000 m.
 
+    float_flag : bool, default False
+        Optimization flag. Set to True if you are sure that you are only using floats as args.
+
     Returns
     -------
-    float
+    float or numpy.array
         An approximation of the distance between two points in WGS84 given in meters.
 
     Examples
     --------
     >>> haversine_dist(8.5, 47.3, 8.7, 47.2)
     18749.056277719905
 
     References
     ----------
     https://en.wikipedia.org/wiki/Haversine_formula
     https://stackoverflow.com/questions/19413259/efficient-way-to-calculate-distance-matrix-given-latitude-and-longitude-data-in
     """
+    if float_flag:
+        lon_1 = math.radians(lon_1)
+        lat_1 = math.radians(lat_1)
+        lon_2 = math.radians(lon_2)
+        lat_2 = math.radians(lat_2)
+
+        cos_lat2 = math.cos(lat_2)
+        cos_lat1 = math.cos(lat_1)
+        cos_lat_d = math.cos(lat_1 - lat_2)
+        cos_lon_d = math.cos(lon_1 - lon_2)
+
+        return r * math.acos(cos_lat_d - cos_lat1 * cos_lat2 * (1 - cos_lon_d))
+
     lon_1 = np.deg2rad(lon_1).ravel()
     lat_1 = np.deg2rad(lat_1).ravel()
     lon_2 = np.deg2rad(lon_2).ravel()
     lat_2 = np.deg2rad(lat_2).ravel()
 
     cos_lat1 = np.cos(lat_1)
     cos_lat2 = np.cos(lat_2)
```

### Comparing `trackintel-1.1.9/trackintel/io/__init__.py` & `trackintel-1.2.1/trackintel/io/__init__.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/trackintel/io/file.py` & `trackintel-1.2.1/trackintel/io/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -465,16 +465,16 @@
     --------
     >>> trackintel.read_trips_csv('data.csv')
     >>> trackintel.read_trips_csv('data.csv', columns={'start_time':'started_at', 'User':'user_id'})
         user_id                started_at               finished_at  origin_staypoint_id  destination_staypoint_id\
     id
     0         1 2015-11-27 08:00:00+00:00 2015-11-27 08:15:00+00:00                    2                         5
     1         1 2015-11-27 08:20:22+00:00 2015-11-27 08:35:22+00:00                    5                         3
-                                geom  
-    id                                                     
+                                geom
+    id
     0   MULTIPOINT (116.31842 39.98470, 116.29873 39.999729)
     1   MULTIPOINT (116.29873 39.98402, 116.32480 40.009269)
     """
     columns = {} if columns is None else columns
     trips = pd.read_csv(*args, index_col=index_col, **kwargs)
     trips.rename(columns=columns, inplace=True)
```

### Comparing `trackintel-1.1.9/trackintel/io/from_geopandas.py` & `trackintel-1.2.1/trackintel/io/from_geopandas.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/trackintel/io/postgis.py` & `trackintel-1.2.1/trackintel/io/postgis.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,16 +55,16 @@
     """Reads positionfixes from a PostGIS database.
 
     Parameters
     ----------
     sql : str
         SQL query e.g. "SELECT * FROM positionfixes"
 
-    con : str, sqlalchemy.engine.Connection or sqlalchemy.engine.Engine
-        Connection string or active connection to PostGIS database.
+    con : sqlalchemy.engine.Connection or sqlalchemy.engine.Engine
+        active connection to PostGIS database.
 
     geom_col : str, default 'geom'
         The geometry column of the table.
 
     crs : optional
         Coordinate reference system to use for the returned GeoDataFrame
 
@@ -154,16 +154,16 @@
     """Reads triplegs from a PostGIS database.
 
     Parameters
     ----------
     sql : str
         SQL query e.g. "SELECT * FROM triplegs"
 
-    con : str, sqlalchemy.engine.Connection or sqlalchemy.engine.Engine
-        Connection string or active connection to PostGIS database.
+    con : sqlalchemy.engine.Connection or sqlalchemy.engine.Engine
+        active connection to PostGIS database.
 
     geom_col : str, default 'geom'
         The geometry column of the table.
 
     crs : optional
         Coordinate reference system to use for the returned GeoDataFrame
 
@@ -253,16 +253,16 @@
     """Read staypoints from a PostGIS database.
 
     Parameters
     ----------
     sql : str
         SQL query e.g. "SELECT * FROM staypoints"
 
-    con : str, sqlalchemy.engine.Connection or sqlalchemy.engine.Engine
-        Connection string or active connection to PostGIS database.
+    con : sqlalchemy.engine.Connection or sqlalchemy.engine.Engine
+        active connection to PostGIS database.
 
     geom_col : str, default 'geom'
         The geometry column of the table.
 
     crs : optional
         Coordinate reference system to use for the returned GeoDataFrame
 
@@ -354,16 +354,16 @@
     """Reads locations from a PostGIS database.
 
     Parameters
     ----------
     sql : str
         SQL query e.g. "SELECT * FROM locations"
 
-    con : str, sqlalchemy.engine.Connection or sqlalchemy.engine.Engine
-        Connection string or active connection to PostGIS database.
+    con : sqlalchemy.engine.Connection or sqlalchemy.engine.Engine
+        active connection to PostGIS database.
 
     center : str, default 'center'
         The geometry column of the table. For the center of the location.
 
     crs : optional
         Coordinate reference system to use for the returned GeoDataFrame
 
@@ -471,16 +471,16 @@
     """Read trips from a PostGIS database.
 
     Parameters
     ----------
     sql : str
         SQL query e.g. "SELECT * FROM trips"
 
-    con : str, sqlalchemy.engine.Connection or sqlalchemy.engine.Engine
-        Connection string or active connection to PostGIS database.
+    con : sqlalchemy.engine.Connection or sqlalchemy.engine.Engine
+        active connection to PostGIS database.
 
     geom_col : str, optional
         The geometry column of the table (if exists). Start and endpoint of the trip.
 
     crs : optional
         Coordinate reference system if table has geometry.
 
@@ -597,16 +597,16 @@
     """Read tours from a PostGIS database.
 
     Parameters
     ----------
     sql : str
         SQL query e.g. "SELECT * FROM tours"
 
-    con : str, sqlalchemy.engine.Connection or sqlalchemy.engine.Engine
-        Connection string or active connection to PostGIS database.
+    con : sqlalchemy.engine.Connection or sqlalchemy.engine.Engine
+        Active connection to PostGIS database.
 
     geom_col : str, optional
         The geometry column of the table (if exists).
 
     crs : optional
         Coordinate reference system if table has geometry.
 
@@ -701,16 +701,16 @@
     ----------
     {long} : GeoDataFrame (as trackintel {long})
         The {long} to store to the database.
 
     name : str
         The name of the table to write to.
 
-    con : str, sqlalchemy.engine.Connection or sqlalchemy.engine.Engine
-        Connection string or active connection to PostGIS database.
+    con : sqlalchemy.engine.Connection or sqlalchemy.engine.Engine
+        active connection to PostGIS database.
 
     schema : str, optional
         The schema (if the database supports this) where the table resides.
 
     if_exists : str, {{'fail', 'replace', 'append'}}, default 'fail'
         How to behave if the table already exists.
```

### Comparing `trackintel-1.1.9/trackintel/model/locations.py` & `trackintel-1.2.1/trackintel/model/locations.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/trackintel/model/positionfixes.py` & `trackintel-1.2.1/trackintel/model/positionfixes.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/trackintel/model/staypoints.py` & `trackintel-1.2.1/trackintel/model/staypoints.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/trackintel/model/tours.py` & `trackintel-1.2.1/trackintel/model/tours.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/trackintel/model/triplegs.py` & `trackintel-1.2.1/trackintel/model/triplegs.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/trackintel/model/trips.py` & `trackintel-1.2.1/trackintel/model/trips.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/trackintel/model/util.py` & `trackintel-1.2.1/trackintel/model/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from functools import partial, update_wrapper
 import trackintel as ti
 import numpy as np
 import pandas as pd
+import warnings
+
 from trackintel.geogr.distances import calculate_haversine_length, check_gdf_planar
 from trackintel.geogr.point_distances import haversine_dist
 
 
 def get_speed_positionfixes(positionfixes):
     """
     Compute speed per positionfix (in m/s)
@@ -27,15 +29,18 @@
     """
     pfs = positionfixes.copy()
     is_planar_crs = ti.geogr.distances.check_gdf_planar(pfs)
 
     g = pfs.geometry
     # get distance and time difference
     if is_planar_crs:
-        dist = g.distance(g.shift(1)).to_numpy()
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", message="CRS not set for some of the concatenation inputs.*")
+
+            dist = g.distance(g.shift(1)).to_numpy()
     else:
         x = g.x.to_numpy()
         y = g.y.to_numpy()
         dist = np.zeros(len(pfs), dtype=np.float64)
         dist[1:] = haversine_dist(x[:-1], y[:-1], x[1:], y[1:])
 
     time_delta = (pfs["tracked_at"] - pfs["tracked_at"].shift(1)).dt.total_seconds().to_numpy()
@@ -85,15 +90,15 @@
         if positionfixes is None:
             raise AttributeError('Method "pfs_mean_speed" requires positionfixes as input.')
         if "tripleg_id" not in positionfixes:
             raise AttributeError('Positionfixes must include column "tripleg_id".')
         # group positionfixes by triplegs and compute average speed for each collection of positionfixes
         grouped_pfs = positionfixes.groupby("tripleg_id").apply(_single_tripleg_mean_speed)
         # add the speed values to the triplegs column
-        tpls = pd.merge(triplegs, grouped_pfs.rename("speed"), left_index=True, right_index=True)
+        tpls = pd.merge(triplegs, grouped_pfs.rename("speed"), how="left", left_index=True, right_index=True)
         tpls.index = tpls.index.astype("int64")
         return tpls
 
     else:
         raise AttributeError(f"Method {method} not known for speed computation.")
```

### Comparing `trackintel-1.1.9/trackintel/preprocessing/filter.py` & `trackintel-1.2.1/trackintel/preprocessing/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,40 +4,40 @@
 def spatial_filter(source, areas, method="within", re_project=False):
     """
     Filter staypoints, locations or triplegs with a geo extent.
 
     Parameters
     ----------
     source : GeoDataFrame (as trackintel datamodels)
-        The source feature to perform the spatial filtering 
+        The source feature to perform the spatial filtering
 
     areas : GeoDataFrame
-        The areas used to perform the spatial filtering. Note, you can have multiple Polygons 
+        The areas used to perform the spatial filtering. Note, you can have multiple Polygons
         and it will return all the features intersect with ANY of those geometries.
 
     method : {'within', 'intersects', 'crosses'}
         The method to filter the 'source' GeoDataFrame
-        
+
         - 'within'    : return instances in 'source' where no points of these instances lies in the \
             exterior of the 'areas' and at least one point of the interior of these instances lies \
             in the interior of 'areas'.
         - 'intersects': return instances in 'source' where the boundary or interior of these instances \
             intersect in any way with those of the 'areas'
         - 'crosses'   : return instances in 'source' where the interior of these instances intersects \
             the interior of the 'areas' but does not contain it, and the dimension of the intersection \
             is less than the dimension of the one of the 'areas'.
-            
+
     re_project : bool, default False
-        If this is set to True, the 'source' will be projected to the coordinate reference system of 'areas' 
-    
+        If this is set to True, the 'source' will be projected to the coordinate reference system of 'areas'
+
     Returns
     -------
     ret_gdf: GeoDataFrame (as trackintel datamodels)
         A new GeoDataFrame containing the features after the spatial filtering.
-        
+
     Examples
     --------
     >>> sp.as_staypoints.spatial_filter(areas, method="within", re_project=False)
     """
     gdf = source.copy()
 
     if re_project:
```

### Comparing `trackintel-1.1.9/trackintel/preprocessing/positionfixes.py` & `trackintel-1.2.1/trackintel/preprocessing/positionfixes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import datetime
 import warnings
 
 import geopandas as gpd
 import numpy as np
 import pandas as pd
-from shapely.geometry import LineString, Point
+from shapely.geometry import LineString
 
-from trackintel.geogr.distances import haversine_dist
-from trackintel.preprocessing.util import applyParallel, _explode_agg
+from trackintel.geogr.distances import check_gdf_planar, haversine_dist
+from trackintel.preprocessing.util import _explode_agg, angle_centroid_multipoints, applyParallel
 
 
 def generate_staypoints(
     positionfixes,
     method="sliding",
     distance_metric="haversine",
     dist_threshold=100,
@@ -223,15 +223,14 @@
     if "tripleg_id" in pfs:
         pfs.drop(columns="tripleg_id", inplace=True)
 
     # we need to ensure pfs is properly ordered
     pfs.sort_values(by=["user_id", "tracked_at"], inplace=True)
 
     if method == "between_staypoints":
-
         # get case:
         # Case 1: pfs have a column 'staypoint_id'
         # Case 2: pfs do not have a column 'staypoint_id' but staypoint are provided
 
         if "staypoint_id" not in pfs.columns:
             case = 2
         else:
@@ -388,63 +387,54 @@
     else:
         raise AttributeError(f"Method unknown. We only support 'between_staypoints'. You passed {method}")
 
 
 def _generate_staypoints_sliding_user(
     df, geo_col, elevation_flag, dist_threshold, time_threshold, gap_threshold, distance_metric, include_last=False
 ):
-    """User level staypoint geenration using sliding method, see generate_staypoints() function for parameter meaning."""
+    """User level staypoint generation using sliding method, see generate_staypoints() function for parameter meaning."""
     if distance_metric == "haversine":
         dist_func = haversine_dist
     else:
         raise AttributeError("distance_metric unknown. We only support ['haversine']. " f"You passed {distance_metric}")
 
     df = df.sort_index(kind="stable").sort_values(by=["tracked_at"], kind="stable")
 
-    # precalulate variables to not do that in for loop
-    last_curr = len(df.index) - 1
-
     # transform times to pandas Timedelta to simplify comparisons
     gap_threshold = pd.Timedelta(gap_threshold, unit="minutes")
-    # to numpy as access time of numpy numpy is faster than pandas array
-    gap_times = pd.eval("((df.tracked_at - df.tracked_at.shift(1)) > gap_threshold)").to_numpy()
+    time_threshold = pd.Timedelta(time_threshold, unit="minutes")
+    # to numpy as access time of numpy array is faster than pandas Series
+    gap_times = ((df.tracked_at - df.tracked_at.shift(1)) > gap_threshold).to_numpy()
 
     # put x and y into numpy arrays to speed up the access in the for loop (shapely is slow)
     x = df[geo_col].x.to_numpy()
     y = df[geo_col].y.to_numpy()
 
     ret_sp = []
-    start = 0
+    curr = start = 0
     for curr in range(1, len(df)):
-
         # the gap of two consecutive positionfixes should not be too long
         if gap_times[curr]:
             start = curr
             continue
 
-        delta_dist = dist_func(x[start], y[start], x[curr], y[curr])
+        delta_dist = dist_func(x[start], y[start], x[curr], y[curr], float_flag=True)
         if delta_dist >= dist_threshold:
-            # the total duration (minutes) of the staypoints
-            delta_t = (df["tracked_at"].iloc[curr] - df["tracked_at"].iloc[start]).total_seconds() // 60
-
-            # we want the staypoint to have long duration
-            if delta_t >= time_threshold:
-                # add new staypoint
+            # we want the staypoint to have long enough duration
+            if (df["tracked_at"].iloc[curr] - df["tracked_at"].iloc[start]) >= time_threshold:
                 ret_sp.append(__create_new_staypoints(start, curr, df, elevation_flag, geo_col))
             # distance large enough but time is too short -> not a staypoint
             # also initializer when new sp is added
             start = curr
 
-        # if we arrive at the last positionfix, and want to include the last staypoint
-        if include_last and curr == last_curr:
-            # additional control: we want to create staypoints with duration larger than time_threshold
-            delta_t = (df["tracked_at"].iloc[curr] - df["tracked_at"].iloc[start]).total_seconds() // 60
-            if delta_t >= time_threshold:
-                new_sp = __create_new_staypoints(start, curr, df, elevation_flag, geo_col, last_flag=True)
-                ret_sp.append(new_sp)
+    if include_last:  # aggregate remaining positionfixes
+        # additional control: we aggregate only if duration longer than time_threshold
+        if (df["tracked_at"].iloc[curr] - df["tracked_at"].iloc[start]) >= time_threshold:
+            new_sp = __create_new_staypoints(start, curr, df, elevation_flag, geo_col, last_flag=True)
+            ret_sp.append(new_sp)
 
     ret_sp = pd.DataFrame(ret_sp)
     ret_sp["user_id"] = df["user_id"].unique()[0]
     return ret_sp
 
 
 def __create_new_staypoints(start, end, pfs, elevation_flag, geo_col, last_flag=False):
@@ -455,16 +445,20 @@
     # pfs[end - 1] for stp geometry and pfs linkage.
     new_sp["started_at"] = pfs["tracked_at"].iloc[start]
     new_sp["finished_at"] = pfs["tracked_at"].iloc[end]
 
     # if end is the last pfs, we want to include the info from it as well
     if last_flag:
         end = len(pfs)
+    points = pfs[geo_col].iloc[start:end].unary_union
+    if check_gdf_planar(pfs):
+        new_sp[geo_col] = points.centroid
+    else:
+        new_sp[geo_col] = angle_centroid_multipoints(points)[0]
 
-    new_sp[geo_col] = Point(pfs[geo_col].iloc[start:end].x.median(), pfs[geo_col].iloc[start:end].y.median())
     if elevation_flag:
         new_sp["elevation"] = pfs["elevation"].iloc[start:end].median()
     new_sp["pfs_id"] = pfs.index[start:end].to_list()
 
     return new_sp
```

### Comparing `trackintel-1.1.9/trackintel/preprocessing/staypoints.py` & `trackintel-1.2.1/trackintel/preprocessing/staypoints.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-from math import radians
-
 import numpy as np
 import geopandas as gpd
 import pandas as pd
-from shapely.geometry import Point
 from sklearn.cluster import DBSCAN
 import warnings
 
-from trackintel.geogr.distances import meters_to_decimal_degrees
-from trackintel.preprocessing.util import applyParallel
+from trackintel.geogr.distances import meters_to_decimal_degrees, check_gdf_planar
+from trackintel.preprocessing.util import applyParallel, angle_centroid_multipoints
 
 
 def generate_locations(
     staypoints,
     method="dbscan",
     epsilon=100,
     num_samples=1,
@@ -68,41 +65,35 @@
         The generated locations.
 
     Examples
     --------
     >>> sp.as_staypoints.generate_locations(method='dbscan', epsilon=100, num_samples=1)
     """
     if agg_level not in ["user", "dataset"]:
-        raise AttributeError("The parameter agg_level must be one of ['user', 'dataset'].")
+        raise AttributeError(f"agg_level '{agg_level}' is unknown. Supported values are ['user', 'dataset'].")
     if method not in ["dbscan"]:
-        raise AttributeError("The parameter method must be one of ['dbscan'].")
+        raise AttributeError(f"method '{method}' is unknown. Supported value is ['dbscan'].")
 
     # initialize the return GeoDataFrames
     sp = staypoints.copy()
     sp = sp.sort_values(["user_id", "started_at"])
     geo_col = sp.geometry.name
 
     if method == "dbscan":
-
-        if distance_metric == "haversine":
-            # The input and output of sklearn's harvarsine metrix are both in radians,
-            # see https://scikit-learn.org/stable/modules/generated/sklearn.metrics.pairwise.haversine_distances.html
-            # here the 'epsilon' is directly applied to the metric's output.
-            # convert to radius
-            db = DBSCAN(eps=epsilon / 6371000, min_samples=num_samples, algorithm="ball_tree", metric=distance_metric)
-        else:
-            db = DBSCAN(eps=epsilon, min_samples=num_samples, algorithm="ball_tree", metric=distance_metric)
+        eps = epsilon / 6371000 if distance_metric == "haversine" else epsilon
+        # scikit haversine_dist wants radian. (We assume that this is good enough)
+        # https://scikit-learn.org/stable/modules/generated/sklearn.metrics.pairwise.haversine_distances.html
+        db = DBSCAN(eps=eps, min_samples=num_samples, algorithm="ball_tree", metric=distance_metric)
 
         if agg_level == "user":
             sp = applyParallel(
                 sp.groupby("user_id", as_index=False),
-                _generate_locations_per_user,
+                _gen_locs_dbscan,
                 n_jobs=n_jobs,
                 print_progress=print_progress,
-                geo_col=geo_col,
                 distance_metric=distance_metric,
                 db=db,
             )
 
             # keeping track of noise labels
             sp_non_noise_labels = sp[sp["location_id"] != -1]
             sp_noise_labels = sp[sp["location_id"] == -1]
@@ -122,112 +113,99 @@
             loc_id_offset = loc_id_offset.fillna(0).cumsum()
 
             sp_non_noise_labels["location_id"] = sp_non_noise_labels["location_id"] + loc_id_offset
             sp = gpd.GeoDataFrame(pd.concat([sp_non_noise_labels, sp_noise_labels]), geometry=geo_col)
             sp.sort_values(["user_id", "started_at"], inplace=True)
 
         else:
-            if distance_metric == "haversine":
-                # the input is converted to list of (lat, lon) tuples in radians unit
-                p = np.array([[radians(g.y), radians(g.x)] for g in sp.geometry])
-            else:
-                p = np.array([[g.x, g.y] for g in sp.geometry])
-            labels = db.fit_predict(p)
-
-            sp["location_id"] = labels
+            _gen_locs_dbscan(sp, db=db, distance_metric=distance_metric)
 
         ### create locations as grouped staypoints
         temp_sp = sp[["user_id", "location_id", sp.geometry.name]]
         if agg_level == "user":
             # directly dissolve by 'user_id' and 'location_id'
             locs = temp_sp.dissolve(by=["user_id", "location_id"], as_index=False)
         else:
             ## generate user-location pairs with same geometries across users
             # get user-location pairs
-            locs = temp_sp.dissolve(by=["user_id", "location_id"], as_index=False).drop(columns={temp_sp.geometry.name})
+            locs = temp_sp[["user_id", "location_id"]].drop_duplicates(ignore_index=True)
             # get location geometries
-            geom_df = temp_sp.dissolve(by=["location_id"], as_index=False).drop(columns={"user_id"})
+            geom_gdf = temp_sp.dissolve(by=["location_id"], as_index=False).drop(columns={"user_id"})
             # merge pairs with location geometries
-            locs = locs.merge(geom_df, on="location_id", how="left")
+            locs = geom_gdf.merge(locs, on="location_id", how="right")
 
         # filter staypoints not belonging to locations
         locs = locs.loc[locs["location_id"] != -1]
 
-        locs["center"] = None  # initialize
-        # locations with only one staypoints is of type "Point"
-        point_idx = locs.geom_type == "Point"
-        if not locs.loc[point_idx].empty:
-            locs.loc[point_idx, "center"] = locs.loc[point_idx, locs.geometry.name]
-        # locations with multiple staypoints is of type "MultiPoint"
-        if not locs.loc[~point_idx].empty:
-            locs.loc[~point_idx, "center"] = locs.loc[~point_idx, locs.geometry.name].apply(
-                lambda p: Point(np.array(p)[:, 0].mean(), np.array(p)[:, 1].mean())
-            )
+        if check_gdf_planar(locs):
+            locs["center"] = locs.geometry.centroid
+        else:
+            # error of wrapping e.g. mean([-180, +180]) -> own function needed
+            locs["center"] = angle_centroid_multipoints(locs.geometry)
 
         # extent is the convex hull of the geometry
-        locs["extent"] = None  # initialize
-        if not locs.empty:
-            locs["extent"] = locs[locs.geometry.name].apply(lambda p: p.convex_hull)
-            # convex_hull of one point would be a Point and two points a Linestring,
-            # we change them into Polygon by creating a buffer of epsilon around them.
-            pointLine_idx = (locs["extent"].geom_type == "LineString") | (locs["extent"].geom_type == "Point")
-
-            if not locs.loc[pointLine_idx].empty:
-                # Perform meter to decimal conversion if the distance metric is haversine
-                if distance_metric == "haversine":
-                    locs.loc[pointLine_idx, "extent"] = locs.loc[pointLine_idx].apply(
-                        lambda p: p["extent"].buffer(meters_to_decimal_degrees(epsilon, p["center"].y)), axis=1
-                    )
-                else:
-                    locs.loc[pointLine_idx, "extent"] = locs.loc[pointLine_idx].apply(
-                        lambda p: p["extent"].buffer(epsilon), axis=1
-                    )
+        locs["extent"] = locs.geometry.convex_hull
+        # convex_hull of Point is Point, and MultiPoint with two Points is a LineString
+        # we change them into Polygon by creating a buffer of epsilon around them.
+        pointLine_idx = (locs["extent"].geom_type == "LineString") | (locs["extent"].geom_type == "Point")
+
+        # Perform meter to decimal conversion if the distance metric is haversine
+        if distance_metric == "haversine":
+            locs.loc[pointLine_idx, "extent"] = locs.loc[pointLine_idx].apply(
+                lambda p: p["extent"].buffer(meters_to_decimal_degrees(epsilon, p["center"].y)), axis=1
+            )
+        else:
+            locs.loc[pointLine_idx, "extent"] = locs.loc[pointLine_idx, "extent"].buffer(epsilon)
 
-        locs = locs.set_geometry("center")
+        locs = locs.set_geometry("center", crs=sp.crs)
         locs = locs[["user_id", "location_id", "center", "extent"]]
 
         # index management
         locs.rename(columns={"location_id": "id"}, inplace=True)
         locs.set_index("id", inplace=True)
 
-    # staypoints not linked to a location receive np.nan in 'location_id'
-    sp.loc[sp["location_id"] == -1, "location_id"] = np.nan
+        # staypoints not linked to a location receive np.nan in 'location_id'
+        sp.loc[sp["location_id"] == -1, "location_id"] = np.nan
 
     if len(locs) > 0:
-        locs.as_locations
+        locs.as_locations  # empty location is not valid
     else:
         warnings.warn("No locations can be generated, returning empty locs.")
 
     ## dtype consistency
     # locs id (generated by this function) should be int64
     locs.index = locs.index.astype("int64")
     # location_id of staypoints can only be in Int64 (missing values)
     sp["location_id"] = sp["location_id"].astype("Int64")
     # user_id of locs should be the same as sp
     locs["user_id"] = locs["user_id"].astype(sp["user_id"].dtype)
 
     return sp, locs
 
 
-def _generate_locations_per_user(user_staypoints, distance_metric, db, geo_col):
-    """function called after groupby: should only contain records of one user;
-    see generate_locations() function for parameter meaning."""
+def _gen_locs_dbscan(sp, distance_metric, db):
+    """Small helper function that takes staypoints and apply them to DBSCAN.
 
+    Parameters
+    ----------
+    sp : GeoDataFrame (as trackintel staypoints)
+    distance_metric : str
+    db : sklearn.cluster.DBSCAN
+
+    Returns
+    -------
+    sp : GeoDataFrame (as trackintel staypoints)
+        Staypoints with new column "location_id"
+    """
+    p = np.array([sp.geometry.x, sp.geometry.y]).transpose()
     if distance_metric == "haversine":
-        # the input is converted to list of (lat, lon) tuples in radians unit
-        p = np.array([[radians(q.y), radians(q.x)] for q in (user_staypoints[geo_col])])
-    else:
-        p = np.array([[q.x, q.y] for q in (user_staypoints[geo_col])])
+        p = np.deg2rad(p)  # haversine distance metric assumes input is in rad
     labels = db.fit_predict(p)
-
-    # add staypoint - location matching to original staypoints
-    user_staypoints["location_id"] = labels
-    user_staypoints = gpd.GeoDataFrame(user_staypoints, geometry=geo_col)
-
-    return user_staypoints
+    sp["location_id"] = labels
+    return sp
 
 
 def merge_staypoints(staypoints, triplegs, max_time_gap="10min", agg={}):
     """
     Aggregate staypoints horizontally via time threshold.
 
     Parameters
@@ -288,15 +266,20 @@
     tpls_merge["type"] = "tripleg"
     sp_merge["type"] = "staypoint"
     # convert datatypes in order to preserve the datatypes (especially ints) despite of NaNs during concat
     sp_merge = sp_merge.convert_dtypes()
 
     # a joined dataframe sp_tpls is constructed to add the columns 'type' and 'next_type' to the 'sp_merge' table
     # concat and sort by time
-    sp_tpls = pd.concat([sp_merge, tpls_merge]).sort_values(by=["user_id", "started_at"])
+    with warnings.catch_warnings():
+        warnings.filterwarnings("ignore", message="CRS not set for some of the concatenation inputs.*")
+
+        # TODO: the warning relates to how we process when no triplegs is provided. In future versions,
+        # we want to seperate the two scenarios. See issue #463.
+        sp_tpls = pd.concat([sp_merge, tpls_merge]).sort_values(by=["user_id", "started_at"])
     sp_tpls.index.rename(index_name, inplace=True)
     # get information whether the there is a tripleg after a staypoint
     sp_tpls["next_type"] = sp_tpls["type"].shift(-1)
     # get only staypoints, but with next type information
     sp_merge = sp_tpls[sp_tpls["type"] == "staypoint"]
 
     # reset index and make temporary index
```

### Comparing `trackintel-1.1.9/trackintel/preprocessing/triplegs.py` & `trackintel-1.2.1/trackintel/preprocessing/triplegs.py`

 * *Files 9% similar despite different names*

```diff
@@ -128,26 +128,34 @@
     user_change["started_at"] = sp_tpls.loc[condition_new_user, "started_at"] - gap_threshold / 2
     user_change[["type", "is_activity"]] = ["user_change", True]  # nicer for debugging
 
     # merge trips with (filler) activities
     trips.drop(columns=["type", "sp_tpls_id"], inplace=True)  # make space so no overlap with activity "sp_tpls_id"
     # Inserting `gaps` and `user_change` into the dataframe creates buffers that catch shifted
     # "staypoint_id" and "trip_id" from corrupting staypoints/trips.
-    trips_with_act = pd.concat((trips, sp_tpls_only_act, gaps, user_change), axis=0, ignore_index=True)
+    with warnings.catch_warnings():
+        warnings.filterwarnings("ignore", message="CRS not set for some of the concatenation inputs.*")
+
+        # TODO: the warning might be caused from process within geopandas. Remember to check
+        # if the warning persists in later versions.
+        trips_with_act = pd.concat((trips, sp_tpls_only_act, gaps, user_change), axis=0, ignore_index=True)
     trips_with_act.sort_values(["user_id", "started_at"], inplace=True)
 
     # ID assignment #
     # add origin/destination ids by shifting
     trips_with_act["origin_staypoint_id"] = trips_with_act["sp_tpls_id"].shift(1)
     trips_with_act["destination_staypoint_id"] = trips_with_act["sp_tpls_id"].shift(-1)
 
     # add geometry for start and end points
     if add_geometry:
-        trips_with_act["origin_geom"] = trips_with_act["geom"].shift(1)
-        trips_with_act["destination_geom"] = trips_with_act["geom"].shift(-1)
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", message="CRS not set for some of the concatenation inputs.*")
+
+            trips_with_act["origin_geom"] = trips_with_act["geom"].shift(1)
+            trips_with_act["destination_geom"] = trips_with_act["geom"].shift(-1)
 
     # add prev_trip_id and next_trip_id for is_activity staypoints
     trips_with_act["prev_trip_id"] = trips_with_act["trip_id"].shift(1)
     trips_with_act["next_trip_id"] = trips_with_act["trip_id"].shift(-1)
 
     # transform column to binary
     trips_with_act["is_activity"].fillna(False, inplace=True)
@@ -194,17 +202,18 @@
         )
         # fill geometry for destionations staypoints that are NaN
         destination_nan_rows = trips[pd.isna(trips["destination_staypoint_id"])].copy()
         trips.loc[pd.isna(trips["destination_staypoint_id"]), "destination_geom"] = destination_nan_rows.tpls.map(
             # from tpls table, get the last point of the last tripleg on the trip
             lambda x: Point(tpls.loc[x[-1], tpls.geometry.name].coords[-1])
         )
-        # convert to GeoDataFrame with MultiPoint column
+        # convert to GeoDataFrame with MultiPoint column and crs (not-None if possible)
         trips["geom"] = [MultiPoint([x, y]) for x, y in zip(trips.origin_geom, trips.destination_geom)]
-        trips = gpd.GeoDataFrame(trips, geometry="geom")
+        crs_trips = sp.crs if sp.crs else tpls.crs
+        trips = gpd.GeoDataFrame(trips, geometry="geom", crs=crs_trips)
         # cleanup
         trips.drop(["origin_geom", "destination_geom"], inplace=True, axis=1)
 
     # final cleaning
     trips.drop(columns=["tpls", "sp", "trip_id"], inplace=True)
 
     # dtype consistency
@@ -248,15 +257,15 @@
         raise AttributeError("staypoints need the column 'is_activity' to be able to generate trips")
     # Copy the input because we add temporary column "type"
     tpls = triplegs.copy()
     sp = staypoints.copy()
 
     # write warnings for columns that we replace
     if "trip_id" in tpls:
-        warnings.warn(f"Override column 'trip_id' in copy of triplegs.")
+        warnings.warn("Override column 'trip_id' in copy of triplegs.")
 
     intersection = sp.columns.intersection(["trip_id", "prev_trip_id", "next_trip_id"])
     if len(intersection):
         warnings.warn(f"Override column(s) {intersection} in copy of staypoints.")
 
     tpls["is_activity"] = False  # in case "is_activity" is already a column of tpls
     tpls["type"] = "tripleg"
@@ -265,14 +274,22 @@
     # create table with relevant information from triplegs and staypoints.
     sp_cols = ["started_at", "finished_at", "user_id", "type", "is_activity"]
     tpls_cols = ["started_at", "finished_at", "user_id", "type"]
     sp_tpls = pd.concat([sp[sp_cols], tpls[tpls_cols]])
     sp_tpls["is_activity"].fillna(False, inplace=True)
     sp_tpls["sp_tpls_id"] = sp_tpls.index  # store id for later reassignment
     if add_geometry:
+        # Check if crs is set. Warn if None
+        if sp.crs is None:
+            warnings.warn("Staypoint crs is not set. Assuming same as for triplegs.")
+        if tpls.crs is None:
+            warnings.warn("Tripleg crs is not set. Assuming same as for staypoints.")
+        assert (
+            sp.crs == tpls.crs or sp.crs is None or tpls.crs is None
+        ), "CRS of staypoints and triplegs differ. Geometry cannot be joined safely."
         sp_tpls["geom"] = pd.concat([sp.geometry, tpls.geometry])
 
     sp_tpls.sort_values(by=["user_id", "started_at"], inplace=True)
     return sp_tpls
 
 
 def _get_activity_masks(df):
```

### Comparing `trackintel-1.1.9/trackintel/preprocessing/trips.py` & `trackintel-1.2.1/trackintel/preprocessing/trips.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         "max_nr_gaps": max_nr_gaps,
         "max_time": max_time,
         "staypoints": staypoints,
         "geom_col": geom_col,
         "crs_is_projected": crs_is_projected,
     }
     if print_progress:
-        tqdm.pandas(desc="User trip generation")
+        tqdm.pandas(desc="User tour generation")
         tours = (
             trips_input.groupby(["user_id"], group_keys=False, as_index=False)
             .progress_apply(_generate_tours_user, **kwargs)
             .reset_index(drop=True)
         )
     else:
         tours = (
```

### Comparing `trackintel-1.1.9/trackintel/visualization/locations.py` & `trackintel-1.2.1/trackintel/visualization/locations.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/trackintel/visualization/modal_split.py` & `trackintel-1.2.1/trackintel/visualization/modal_split.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     y_label=None,
     x_pad=10,
     y_pad=10,
     title_pad=1.02,
     skip_xticks=0,
     n_col_legend=5,
     borderaxespad=0.5,
+    bar_kws=None,
 ):
     """
     Plot modal split as returned by `trackintel.analysis.modal_split.calculate_modal_split`
 
     Parameters
     ----------
     df_modal_split : DataFrame
@@ -44,15 +45,18 @@
     title_pad : float, default: 1.02
         Passed on to `matplotlib.pyplot.title`
     skip_xticks : int, default: 1
         Every nth x-tick label is kept.
     n_col_legend : int
         Passed on as `ncol` to matplotlib.pyplot.legend()
     borderaxespad : float
+        The pad between the axes and legend border, in font-size units.
         Passed on to matplotlib.pyplot.legend()
+    bar_kws : dict
+        Parameters that control the bar-plot visualization, passed to DataFrame.plot.bar()
 
     Returns
     -------
     fig : Matplotlib figure handle
     ax : Matplotlib axis handle
 
     Examples
@@ -80,15 +84,15 @@
             "Index of modal split has to be a datetime type. This problem can be solved if the 'freq' "
             "keyword of 'calculate_modal_split is not None'"
         )
     # set date formatter
     df_modal_split.index = df_modal_split.index.map(lambda s: s.strftime(date_fmt_x_axis))
 
     # plotting
-    df_modal_split.plot.bar(stacked=True, ax=ax)
+    df_modal_split.plot.bar(stacked=True, ax=ax, **(bar_kws or {}))
 
     # skip ticks for X axis
     if skip_xticks > 0:
         for i, tick in enumerate(ax.xaxis.get_major_ticks()):
             if i % skip_xticks != 0:
                 tick.set_visible(False)
```

### Comparing `trackintel-1.1.9/trackintel/visualization/osm.py` & `trackintel-1.2.1/trackintel/visualization/osm.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/trackintel/visualization/positionfixes.py` & `trackintel-1.2.1/trackintel/visualization/positionfixes.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/trackintel/visualization/staypoints.py` & `trackintel-1.2.1/trackintel/visualization/staypoints.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/trackintel/visualization/triplegs.py` & `trackintel-1.2.1/trackintel/visualization/triplegs.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/trackintel/visualization/util.py` & `trackintel-1.2.1/trackintel/visualization/util.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.1.9/trackintel.egg-info/PKG-INFO` & `trackintel-1.2.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,27 @@
-Metadata-Version: 2.1
-Name: trackintel
-Version: 1.1.9
-Summary: Human mobility and movement analysis framework.
-Home-page: https://github.com/mie-lab/trackintel
-Author: Dominik Bucher, Henry Martin, Ye Hong
-Author-email: dobucher@ethz.ch, martinhe@ethz.ch
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS.md
-
-
-# The trackintel Framework
+# The trackintel framework
 
 
 [![PyPI version](https://badge.fury.io/py/trackintel.svg)](https://badge.fury.io/py/trackintel)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/trackintel.svg)](https://anaconda.org/conda-forge/trackintel)
 [![Actions Status](https://github.com/mie-lab/trackintel/workflows/Tests/badge.svg)](https://github.com/mie-lab/trackintel/actions?query=workflow%3ATests)
 [![Documentation Status](https://readthedocs.org/projects/trackintel/badge/?version=latest)](https://trackintel.readthedocs.io/en/latest/?badge=latest)
 [![codecov.io](https://codecov.io/gh/mie-lab/trackintel/coverage.svg?branch=master)](https://codecov.io/gh/mie-lab/trackintel)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![asv](http://img.shields.io/badge/benchmarked%20by-asv-green.svg?style=flat)](https://mie-lab.github.io/trackintel/)
 
-*trackintel* is a library for the analysis of spatio-temporal tracking data with a focus on human mobility. The core of *trackintel* is the hierachical data model for movement data that is used in GIS, transport planning and related fields [[1]](#1). We provide functionalities for the full life-cycle of human mobility data analysis: import and export of tracking data of different types (e.g, trackpoints, check-ins, trajectories), preprocessing, data quality assessment, semantic enrichment, quantitative analysis and mining tasks, and visualization of data and results.
-Trackintel is based on [Pandas](https://pandas.pydata.org/) and [GeoPandas](https://geopandas.org/#)
+*trackintel* is a library for the analysis of spatio-temporal tracking data with a focus on human mobility. The core of *trackintel* is the hierachical data model for movement data that is used in GIS, transport planning and related fields. We provide functionalities for the full life-cycle of human mobility data analysis: import and export of tracking data of different types (e.g, trackpoints, check-ins, trajectories), preprocessing, data quality assessment, semantic enrichment, quantitative analysis and mining tasks, and visualization of data and results.
+Trackintel is based on [Pandas](https://pandas.pydata.org/) and [GeoPandas](https://geopandas.org/#). 
 
-You can find the documentation on the [trackintel documentation page](https://trackintel.readthedocs.io/en/latest).
+You can find the documentation on the [trackintel documentation page](https://trackintel.readthedocs.io/en/latest). 
 
 Try *trackintel* online in a MyBinder notebook: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mie-lab/trackintel/HEAD?filepath=%2Fexamples%2Ftrackintel_basic_tutorial.ipynb)
 
+Please star this repo and [cite](#citelink) our paper if you find our work is helpful for you.
+
 ## Data model
 
 An overview of the data model of *trackintel*:
 * **positionfixes** (Raw tracking points, e.g., GPS recordings or check-ins)
 * **staypoints** (Locations where a user spent time without moving, e.g., aggregations of positionfixes or check-ins). Staypoints can be classified into the following categories:
   * **activity** staypoints. Staypoints with a purpose and a semantic label, e.g., stopping at a cafe to meet with friends or staying at the workplace.
   * non-activity staypoints. Staypoints without an explicit purpose, e.g., waiting for a bus or stopping in a traffic jam.
@@ -106,15 +92,20 @@
 
 For example, the plot below shows the generated staypoints and triplegs from the imported raw positionfix data.
 <p align="center">
   <img width="595" height="500" src="https://github.com/mie-lab/trackintel/blob/master/docs/_static/example_triplegs.png?raw=true">
 </p>
 
 ## Installation and Usage
-*trackintel* is on [pypi.org](https://pypi.org/project/trackintel/), you can install it in a `GeoPandas` available environment using: 
+*trackintel* is on [pypi.org](https://pypi.org/project/trackintel/) and [conda-forge](https://anaconda.org/conda-forge/trackintel). We recommend installing trackintel via conda-forge:
+```{python}
+conda install -c conda-forge trackintel
+```
+
+Alternatively, you can install it with pip in a `GeoPandas` available environment using: 
 ```{python}
 pip install trackintel
 ```
 
 You should then be able to run the examples in the `examples` folder or import trackintel using:
 ```{python}
 import trackintel as ti
@@ -140,11 +131,22 @@
 You can find the development roadmap under `ROADMAP.md` and further development guidelines under `CONTRIBUTING.md`.
 
 ## Contributors
 
 *trackintel* is primarily maintained by the Mobility Information Engineering Lab at ETH Zurich ([mie-lab.ethz.ch](http://mie-lab.ethz.ch)).
 If you want to contribute, send a pull request and put yourself in the `AUTHORS.md` file.
 
-## References
-<a id="1">[1]</a>
-[Axhausen, K. W. (2007). Definition Of Movement and Activity For Transport Modelling. In Handbook of Transport Modelling. Emerald Group Publishing Limited.](
-https://www.researchgate.net/publication/251791517_Definition_of_movement_and_activity_for_transport_modelling)
+## <span id="citelink">Citation</span>
+
+If you find this code useful for your work or use it in your project, please consider citing:
+```
+@article{Martin_2023_trackintel,
+  doi = {10.1016/j.compenvurbsys.2023.101938},
+  volume = {101},
+  pages = {101938},
+  author = {Henry Martin and Ye Hong and Nina Wiedemann and Dominik Bucher and Martin Raubal},
+  keywords = {Human mobility analysis, Open-source software, Transport planning, Data mining, Python, Tracking studies},
+  title = {Trackintel: An open-source Python library for human mobility analysis},
+  journal = {Computers, Environment and Urban Systems},
+  year = {2023},
+}
+```
```

### Comparing `trackintel-1.1.9/trackintel.egg-info/SOURCES.txt` & `trackintel-1.2.1/trackintel.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 AUTHORS.md
 LICENSE
 README.md
 setup.py
+benchmarks/__init__.py
+benchmarks/preprocessing_benchmarks.py
+tests/test_core.py
 tests/analysis/__init__.py
 tests/analysis/test_label.py
 tests/analysis/test_location_identification.py
 tests/analysis/test_modal_split.py
 tests/analysis/test_tracking_quality.py
 tests/examples/__init__.py
 tests/examples/test_examples.py
```

