# Comparing `tmp/causalnex-0.9.1.tar.gz` & `tmp/causalnex-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/causalnex-0.9.1.tar", last modified: Wed Jan  6 22:10:05 2021, max compression
+gzip compressed data, was "dist/causalnex-0.9.2.tar", last modified: Thu Mar 11 19:11:01 2021, max compression
```

## Comparing `causalnex-0.9.1.tar` & `causalnex-0.9.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-06 22:10:05.000000 causalnex-0.9.1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7311 2021-01-06 22:10:05.000000 causalnex-0.9.1/PKG-INFO
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-06 22:10:05.000000 causalnex-0.9.1/causalnex/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-06 22:10:05.000000 causalnex-0.9.1/causalnex/structure/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19900 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/structure/dynotears.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12280 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/structure/transformers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1751 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/structure/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-06 22:10:05.000000 causalnex-0.9.1/causalnex/structure/data_generators/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    27145 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/structure/data_generators/wrappers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    31583 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/structure/data_generators/core.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2304 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/structure/data_generators/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11924 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/structure/categorical_variable_mapper.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-06 22:10:05.000000 causalnex-0.9.1/causalnex/structure/pytorch/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19349 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/structure/pytorch/core.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-06 22:10:05.000000 causalnex-0.9.1/causalnex/structure/pytorch/dist_type/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3017 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/structure/pytorch/dist_type/binary.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2059 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/structure/pytorch/dist_type/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9874 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/structure/pytorch/dist_type/_base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3687 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/structure/pytorch/dist_type/poisson.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10461 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/structure/pytorch/dist_type/categorical.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2651 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/structure/pytorch/dist_type/continuous.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6462 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/structure/pytorch/dist_type/ordinal.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3994 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/structure/pytorch/nonlinear.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1751 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/structure/pytorch/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-06 22:10:05.000000 causalnex-0.9.1/causalnex/structure/pytorch/sklearn/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8197 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/structure/pytorch/sklearn/clf.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1635 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/structure/pytorch/sklearn/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15071 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/structure/pytorch/sklearn/_base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3198 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/structure/pytorch/sklearn/reg.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14911 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/structure/pytorch/notears.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    20098 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/structure/notears.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12532 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/structure/structuremodel.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-06 22:10:05.000000 causalnex-0.9.1/causalnex/contrib/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1431 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/contrib/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-06 22:10:05.000000 causalnex-0.9.1/causalnex/evaluation/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8235 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/evaluation/evaluation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1642 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/evaluation/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-06 22:10:05.000000 causalnex-0.9.1/causalnex/plots/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3654 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/plots/display.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9686 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/plots/plots.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1867 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/plots/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-06 22:10:05.000000 causalnex-0.9.1/causalnex/ebaybbn/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2573 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/ebaybbn/graph.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3425 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/ebaybbn/utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2904 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/ebaybbn/exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1783 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/ebaybbn/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    37019 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/ebaybbn/bbn.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-06 22:10:05.000000 causalnex-0.9.1/causalnex/inference/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13074 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/inference/inference.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1618 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/inference/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1621 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-06 22:10:05.000000 causalnex-0.9.1/causalnex/discretiser/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1574 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/discretiser/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8852 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/discretiser/discretiser.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-06 22:10:05.000000 causalnex-0.9.1/causalnex/network/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    23375 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/network/network.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1607 2021-01-06 21:43:12.000000 causalnex-0.9.1/causalnex/network/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-06 22:10:05.000000 causalnex-0.9.1/causalnex.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-01-06 22:10:05.000000 causalnex-0.9.1/causalnex.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1772 2021-01-06 22:10:05.000000 causalnex-0.9.1/causalnex.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7311 2021-01-06 22:10:05.000000 causalnex-0.9.1/causalnex.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2021-01-06 22:10:05.000000 causalnex-0.9.1/causalnex.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      245 2021-01-06 22:10:05.000000 causalnex-0.9.1/causalnex.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3441 2021-01-06 21:43:12.000000 causalnex-0.9.1/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5862 2021-01-06 21:43:12.000000 causalnex-0.9.1/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      157 2021-01-06 22:10:05.000000 causalnex-0.9.1/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-03-11 19:11:01.000000 causalnex-0.9.2/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-03-11 19:11:01.000000 causalnex-0.9.2/causalnex/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-03-11 19:11:01.000000 causalnex-0.9.2/causalnex/contrib/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1431 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/contrib/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-03-11 19:11:01.000000 causalnex-0.9.2/causalnex/discretiser/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1574 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/discretiser/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8852 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/discretiser/discretiser.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-03-11 19:11:01.000000 causalnex-0.9.2/causalnex/ebaybbn/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1783 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/ebaybbn/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    37019 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/ebaybbn/bbn.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2904 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/ebaybbn/exceptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2573 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/ebaybbn/graph.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3425 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/ebaybbn/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-03-11 19:11:01.000000 causalnex-0.9.2/causalnex/evaluation/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1642 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/evaluation/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8235 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/evaluation/evaluation.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-03-11 19:11:01.000000 causalnex-0.9.2/causalnex/inference/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1618 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/inference/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13036 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/inference/inference.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-03-11 19:11:01.000000 causalnex-0.9.2/causalnex/network/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1607 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/network/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    23371 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/network/network.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-03-11 19:11:01.000000 causalnex-0.9.2/causalnex/plots/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1867 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/plots/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3654 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/plots/display.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9686 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/plots/plots.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-03-11 19:11:01.000000 causalnex-0.9.2/causalnex/structure/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-03-11 19:11:01.000000 causalnex-0.9.2/causalnex/structure/data_generators/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2304 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/structure/data_generators/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    31583 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/structure/data_generators/core.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    27145 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/structure/data_generators/wrappers.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-03-11 19:11:01.000000 causalnex-0.9.2/causalnex/structure/pytorch/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-03-11 19:11:01.000000 causalnex-0.9.2/causalnex/structure/pytorch/dist_type/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2059 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/structure/pytorch/dist_type/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9874 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/structure/pytorch/dist_type/_base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3017 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/structure/pytorch/dist_type/binary.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10461 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/structure/pytorch/dist_type/categorical.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2651 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/structure/pytorch/dist_type/continuous.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6462 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/structure/pytorch/dist_type/ordinal.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3687 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/structure/pytorch/dist_type/poisson.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-03-11 19:11:01.000000 causalnex-0.9.2/causalnex/structure/pytorch/sklearn/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1635 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/structure/pytorch/sklearn/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15071 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/structure/pytorch/sklearn/_base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8197 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/structure/pytorch/sklearn/clf.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3198 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/structure/pytorch/sklearn/reg.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1751 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/structure/pytorch/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19315 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/structure/pytorch/core.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3960 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/structure/pytorch/nonlinear.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14911 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/structure/pytorch/notears.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1751 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/structure/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11924 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/structure/categorical_variable_mapper.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19900 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/structure/dynotears.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    20098 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/structure/notears.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12532 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/structure/structuremodel.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12280 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/structure/transformers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1621 2021-03-11 19:01:00.000000 causalnex-0.9.2/causalnex/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-03-11 19:11:01.000000 causalnex-0.9.2/causalnex.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7311 2021-03-11 19:11:01.000000 causalnex-0.9.2/causalnex.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1772 2021-03-11 19:11:01.000000 causalnex-0.9.2/causalnex.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-03-11 19:11:01.000000 causalnex-0.9.2/causalnex.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      245 2021-03-11 19:11:01.000000 causalnex-0.9.2/causalnex.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2021-03-11 19:11:01.000000 causalnex-0.9.2/causalnex.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5862 2021-03-11 19:01:00.000000 causalnex-0.9.2/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      157 2021-03-11 19:11:01.000000 causalnex-0.9.2/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3441 2021-03-11 19:01:00.000000 causalnex-0.9.2/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7311 2021-03-11 19:11:01.000000 causalnex-0.9.2/PKG-INFO
```

### Comparing `causalnex-0.9.1/PKG-INFO` & `causalnex-0.9.2/causalnex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causalnex
-Version: 0.9.1
+Version: 0.9.2
 Summary: Toolkit for causal reasoning (Bayesian Networks / Inference)
 Home-page: https://github.com/quantumblacklabs/causalnex
 Author: QuantumBlack Labs
 Author-email: causalnex@quantumblack.com
 License: Apache Software License (Apache 2.0)
 Description: ![CausalNex](https://raw.githubusercontent.com/quantumblacklabs/causalnex/master/docs/source/causalnex_banner.png)
```

### Comparing `causalnex-0.9.1/causalnex/structure/dynotears.py` & `causalnex-0.9.2/causalnex/structure/dynotears.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/structure/transformers.py` & `causalnex-0.9.2/causalnex/structure/transformers.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/structure/__init__.py` & `causalnex-0.9.2/causalnex/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/structure/data_generators/wrappers.py` & `causalnex-0.9.2/causalnex/structure/data_generators/wrappers.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/structure/data_generators/core.py` & `causalnex-0.9.2/causalnex/structure/data_generators/core.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/structure/data_generators/__init__.py` & `causalnex-0.9.2/causalnex/structure/data_generators/__init__.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/structure/categorical_variable_mapper.py` & `causalnex-0.9.2/causalnex/structure/categorical_variable_mapper.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/structure/pytorch/core.py` & `causalnex-0.9.2/causalnex/structure/pytorch/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 from sklearn.base import BaseEstimator
 
 from causalnex.structure.pytorch.dist_type._base import DistTypeBase
 from causalnex.structure.pytorch.nonlinear import LocallyConnected
 
 
 # Problem in pytorch 1.6 (_forward_unimplemented), fixed in next release:
-# pylint: disable=abstract-method
 class NotearsMLP(nn.Module, BaseEstimator):
     """
     Class for NOTEARS MLP (Multi-layer Perceptron) model.
     The model weights consist of dag_layer and loc_lin_layer weights respectively.
     dag_layer weight is the weight of the first fully connected layer which determines the causal structure.
     loc_lin_layer weights are the weight of hidden layers after the first fully connected layer
     """
```

### Comparing `causalnex-0.9.1/causalnex/structure/pytorch/dist_type/binary.py` & `causalnex-0.9.2/causalnex/structure/pytorch/dist_type/binary.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/structure/pytorch/dist_type/__init__.py` & `causalnex-0.9.2/causalnex/structure/pytorch/dist_type/__init__.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/structure/pytorch/dist_type/_base.py` & `causalnex-0.9.2/causalnex/structure/pytorch/dist_type/_base.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/structure/pytorch/dist_type/poisson.py` & `causalnex-0.9.2/causalnex/structure/pytorch/dist_type/poisson.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/structure/pytorch/dist_type/categorical.py` & `causalnex-0.9.2/causalnex/structure/pytorch/dist_type/categorical.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/structure/pytorch/dist_type/continuous.py` & `causalnex-0.9.2/causalnex/structure/pytorch/dist_type/continuous.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/structure/pytorch/dist_type/ordinal.py` & `causalnex-0.9.2/causalnex/structure/pytorch/dist_type/ordinal.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/structure/pytorch/nonlinear.py` & `causalnex-0.9.2/causalnex/structure/pytorch/nonlinear.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 import math
 
 import torch
 import torch.nn as nn
 
 
 # Problem in pytorch 1.6 (_forward_unimplemented), fixed in next release:
-# pylint: disable=abstract-method
 class LocallyConnected(nn.Module):
     """
     Local linear layer, i.e. Conv1dLocal() with filter size 1.
     """
 
     def __init__(
         self,
```

### Comparing `causalnex-0.9.1/causalnex/structure/pytorch/__init__.py` & `causalnex-0.9.2/causalnex/structure/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/structure/pytorch/sklearn/clf.py` & `causalnex-0.9.2/causalnex/structure/pytorch/sklearn/clf.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/structure/pytorch/sklearn/__init__.py` & `causalnex-0.9.2/causalnex/structure/pytorch/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/structure/pytorch/sklearn/_base.py` & `causalnex-0.9.2/causalnex/structure/pytorch/sklearn/_base.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/structure/pytorch/sklearn/reg.py` & `causalnex-0.9.2/causalnex/structure/pytorch/sklearn/reg.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/structure/pytorch/notears.py` & `causalnex-0.9.2/causalnex/structure/pytorch/notears.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/structure/notears.py` & `causalnex-0.9.2/causalnex/structure/notears.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/structure/structuremodel.py` & `causalnex-0.9.2/causalnex/structure/structuremodel.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/contrib/__init__.py` & `causalnex-0.9.2/causalnex/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/evaluation/evaluation.py` & `causalnex-0.9.2/causalnex/evaluation/evaluation.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/evaluation/__init__.py` & `causalnex-0.9.2/causalnex/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/plots/display.py` & `causalnex-0.9.2/causalnex/plots/display.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/plots/plots.py` & `causalnex-0.9.2/causalnex/plots/plots.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/plots/__init__.py` & `causalnex-0.9.2/causalnex/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/ebaybbn/graph.py` & `causalnex-0.9.2/causalnex/ebaybbn/graph.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/ebaybbn/utils.py` & `causalnex-0.9.2/causalnex/ebaybbn/utils.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/ebaybbn/exceptions.py` & `causalnex-0.9.2/causalnex/ebaybbn/exceptions.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/ebaybbn/__init__.py` & `causalnex-0.9.2/causalnex/ebaybbn/__init__.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/ebaybbn/bbn.py` & `causalnex-0.9.2/causalnex/ebaybbn/bbn.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/inference/inference.py` & `causalnex-0.9.2/causalnex/inference/inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,18 +194,16 @@
                 - if Hashable: the intervention updates the state to 1, and all other states to 0;
                 - if Dict[Hashable, float]: update states to all state -> probabilitiy in the dict.
 
         Raises:
             ValueError: if performing intervention would create an isolated node.
         """
         if not any(
-            [
-                node in inspect.getargs(f.__code__)[0][1:]
-                for _, f in self._node_functions.items()
-            ]
+            node in inspect.getargs(f.__code__)[0][1:]
+            for _, f in self._node_functions.items()
         ):
             raise ValueError(
                 "Do calculus cannot be applied because it would result in an isolate"
             )
 
         if isinstance(state, int):
             state = {s: float(s == state) for s in self._cpds[node]}
@@ -285,15 +283,15 @@
             # getargvalues was "inadvertently marked as deprecated in Python 3.5"
             # https://docs.python.org/3/library/inspect.html#inspect.getfullargspec
             arg_spec = inspect.getargvalues(inspect.currentframe())
 
             return self._cpds[arg_spec.args[0]][  # target name
                 arg_spec.locals[arg_spec.args[0]]
             ][  # target state
-                tuple([(arg, arg_spec.locals[arg]) for arg in arg_spec.args[1:]])
+                tuple((arg, arg_spec.locals[arg]) for arg in arg_spec.args[1:])
             ]  # conditions
 
         code = template.__code__
         pos_count = (
             [code.co_posonlyargcount] if hasattr(code, "co_posonlyargcount") else []
         )
         template.__code__ = types.CodeType(
```

### Comparing `causalnex-0.9.1/causalnex/inference/__init__.py` & `causalnex-0.9.2/causalnex/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/__init__.py` & `causalnex-0.9.2/causalnex/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,10 +26,10 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 causalnex toolkit for causal reasoning (Bayesian Networks / Inference)
 """
 
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 
 __all__ = ["structure", "discretiser", "evaluation", "inference", "network", "plots"]
```

### Comparing `causalnex-0.9.1/causalnex/discretiser/__init__.py` & `causalnex-0.9.2/causalnex/discretiser/__init__.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/discretiser/discretiser.py` & `causalnex-0.9.2/causalnex/discretiser/discretiser.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex/network/network.py` & `causalnex-0.9.2/causalnex/network/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -446,15 +446,15 @@
 
         parents = sorted(self._model.get_parents(node))
         cpd = self.cpds[node]
 
         transformed_data[
             "{node}_prediction".format(node=node)
         ] = transformed_data.apply(
-            lambda row: cpd[tuple([row[parent] for parent in parents])].idxmax()
+            lambda row: cpd[tuple(row[parent] for parent in parents)].idxmax()
             if parents
             else cpd[""].idxmax(),
             axis=1,
         )
         return transformed_data[[node + "_prediction"]]
 
     def _predict_from_incomplete_data(
@@ -524,15 +524,15 @@
 
         parents = sorted(self._model.get_parents(node))
         cpd = self.cpds[node]
 
         def lookup_probability(row, s):
             """Retrieve probability from CPD"""
             if parents:
-                return cpd[tuple([row[parent] for parent in parents])].loc[s]
+                return cpd[tuple(row[parent] for parent in parents)].loc[s]
             return cpd.at[s, ""]
 
         for state in self.node_states[node]:
             transformed_data[
                 "{n}_{s}".format(n=node, s=state)
             ] = transformed_data.apply(
                 lambda row, st=state: lookup_probability(row, st), axis=1
```

### Comparing `causalnex-0.9.1/causalnex/network/__init__.py` & `causalnex-0.9.2/causalnex/network/__init__.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex.egg-info/SOURCES.txt` & `causalnex-0.9.2/causalnex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/causalnex.egg-info/PKG-INFO` & `causalnex-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causalnex
-Version: 0.9.1
+Version: 0.9.2
 Summary: Toolkit for causal reasoning (Bayesian Networks / Inference)
 Home-page: https://github.com/quantumblacklabs/causalnex
 Author: QuantumBlack Labs
 Author-email: causalnex@quantumblack.com
 License: Apache Software License (Apache 2.0)
 Description: ![CausalNex](https://raw.githubusercontent.com/quantumblacklabs/causalnex/master/docs/source/causalnex_banner.png)
```

### Comparing `causalnex-0.9.1/setup.py` & `causalnex-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `causalnex-0.9.1/README.md` & `causalnex-0.9.2/README.md`

 * *Files identical despite different names*

