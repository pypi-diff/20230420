# Comparing `tmp/tsml-0.0.6.tar.gz` & `tmp/tsml-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsml-0.0.6.tar", last modified: Mon Apr 17 23:08:33 2023, max compression
+gzip compressed data, was "tsml-0.0.7.tar", last modified: Thu Apr 20 11:47:38 2023, max compression
```

## Comparing `tsml-0.0.6.tar` & `tsml-0.0.7.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.908886 tsml-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-17 23:08:24.000000 tsml-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-17 23:08:24.000000 tsml-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-17 23:08:33.908886 tsml-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-17 23:08:24.000000 tsml-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-17 23:08:24.000000 tsml-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 23:08:33.908886 tsml-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.896886 tsml-0.0.6/tsml/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.900886 tsml-0.0.6/tsml/convolution_based/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/convolution_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.900886 tsml-0.0.6/tsml/datasets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.900886 tsml-0.0.6/tsml/datasets/EqualMinimalJapaneseVowels/
--rw-r--r--   0 runner    (1001) docker     (123)   120661 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (123)   120799 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TRAIN.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.900886 tsml-0.0.6/tsml/datasets/MinimalChinatown/
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/datasets/MinimalChinatown/MinimalChinatown_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/datasets/MinimalChinatown/MinimalChinatown_TRAIN.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.900886 tsml-0.0.6/tsml/datasets/MinimalGasPrices/
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TRAIN.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.900886 tsml-0.0.6/tsml/datasets/MinimalJapaneseVowels/
--rw-r--r--   0 runner    (1001) docker     (123)    36247 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (123)    38758 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TRAIN.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.900886 tsml-0.0.6/tsml/datasets/UnequalMinimalChinatown/
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TRAIN.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.900886 tsml-0.0.6/tsml/datasets/UnequalMinimalGasPrices/
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TRAIN.ts
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24759 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/datasets/_data_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.900886 tsml-0.0.6/tsml/deep_learning/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/deep_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/deep_learning/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.900886 tsml-0.0.6/tsml/dictionary_based/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/dictionary_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.900886 tsml-0.0.6/tsml/distance_based/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/distance_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.900886 tsml-0.0.6/tsml/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/dummy/_dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.900886 tsml-0.0.6/tsml/feature_based/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/feature_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/feature_based/_catch22.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.904886 tsml-0.0.6/tsml/interval_based/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/interval_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45975 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/interval_based/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14260 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/interval_based/_cif.py
--rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/interval_based/_interval_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)    21635 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/interval_based/_interval_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/interval_based/_rise.py
--rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/interval_based/_stsf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/interval_based/_tsf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.904886 tsml-0.0.6/tsml/shapelet_based/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/shapelet_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/shapelet_based/_stc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.904886 tsml-0.0.6/tsml/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    81519 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/tests/_sklearn_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/tests/estimator_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/tests/test_all_estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/tests/test_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.904886 tsml-0.0.6/tsml/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/transformations/_ar_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)    46093 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/transformations/_catch22.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/transformations/_function_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    34766 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/transformations/_interval_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/transformations/_periodogram.py
--rw-r--r--   0 runner    (1001) docker     (123)    41527 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/transformations/_sfa.py
--rw-r--r--   0 runner    (1001) docker     (123)    23960 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/transformations/_shapelet_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/transformations/_summary_features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.908886 tsml-0.0.6/tsml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/utils/_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/utils/discovery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.908886 tsml-0.0.6/tsml/utils/numba_functions/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/utils/numba_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/utils/numba_functions/general.py
--rw-r--r--   0 runner    (1001) docker     (123)    19873 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/utils/numba_functions/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     7782 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/utils/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.908886 tsml-0.0.6/tsml/vector/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15951 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/vector/_cit.py
--rw-r--r--   0 runner    (1001) docker     (123)    18576 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/vector/_rotation_forest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.908886 tsml-0.0.6/tsml/vector/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/vector/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/vector/tests/test_rotation_forest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.900886 tsml-0.0.6/tsml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-17 23:08:33.000000 tsml-0.0.6/tsml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-04-17 23:08:33.000000 tsml-0.0.6/tsml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 23:08:33.000000 tsml-0.0.6/tsml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-17 23:08:33.000000 tsml-0.0.6/tsml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-17 23:08:33.000000 tsml-0.0.6/tsml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.603603 tsml-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-20 11:47:27.000000 tsml-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-20 11:47:27.000000 tsml-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-20 11:47:38.603603 tsml-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-20 11:47:27.000000 tsml-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-20 11:47:27.000000 tsml-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 11:47:38.603603 tsml-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.595602 tsml-0.0.7/tsml/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.595602 tsml-0.0.7/tsml/convolution_based/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/convolution_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.595602 tsml-0.0.7/tsml/datasets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.595602 tsml-0.0.7/tsml/datasets/EqualMinimalJapaneseVowels/
+-rw-r--r--   0 runner    (1001) docker     (123)   120661 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (123)   120799 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TRAIN.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.595602 tsml-0.0.7/tsml/datasets/MinimalChinatown/
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/datasets/MinimalChinatown/MinimalChinatown_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/datasets/MinimalChinatown/MinimalChinatown_TRAIN.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.595602 tsml-0.0.7/tsml/datasets/MinimalGasPrices/
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TRAIN.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.595602 tsml-0.0.7/tsml/datasets/MinimalJapaneseVowels/
+-rw-r--r--   0 runner    (1001) docker     (123)    36247 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    38758 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TRAIN.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.599603 tsml-0.0.7/tsml/datasets/UnequalMinimalChinatown/
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TRAIN.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.599603 tsml-0.0.7/tsml/datasets/UnequalMinimalGasPrices/
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TRAIN.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24759 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/datasets/_data_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.599603 tsml-0.0.7/tsml/deep_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/deep_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/deep_learning/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.599603 tsml-0.0.7/tsml/dictionary_based/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/dictionary_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.599603 tsml-0.0.7/tsml/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/distance_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.599603 tsml-0.0.7/tsml/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12171 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/dummy/_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.599603 tsml-0.0.7/tsml/feature_based/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/feature_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/feature_based/_catch22.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.599603 tsml-0.0.7/tsml/interval_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/interval_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46207 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/interval_based/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14260 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/interval_based/_cif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/interval_based/_interval_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21883 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/interval_based/_interval_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/interval_based/_rise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/interval_based/_stsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/interval_based/_tsf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.599603 tsml-0.0.7/tsml/shapelet_based/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/shapelet_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/shapelet_based/_stc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.599603 tsml-0.0.7/tsml/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47450 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/tests/_sklearn_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/tests/estimator_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/tests/test_all_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/tests/test_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.603603 tsml-0.0.7/tsml/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/transformations/_ar_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46014 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/transformations/_catch22.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/transformations/_function_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34766 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/transformations/_interval_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/transformations/_periodogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41527 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/transformations/_sfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24022 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/transformations/_shapelet_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/transformations/_summary_features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.603603 tsml-0.0.7/tsml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/utils/_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/utils/discovery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.603603 tsml-0.0.7/tsml/utils/numba_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/utils/numba_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/utils/numba_functions/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19873 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/utils/numba_functions/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/utils/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.603603 tsml-0.0.7/tsml/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15951 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/vector/_cit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18576 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/vector/_rotation_forest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.603603 tsml-0.0.7/tsml/vector/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/vector/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/vector/tests/test_rotation_forest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.595602 tsml-0.0.7/tsml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-20 11:47:38.000000 tsml-0.0.7/tsml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-04-20 11:47:38.000000 tsml-0.0.7/tsml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 11:47:38.000000 tsml-0.0.7/tsml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-20 11:47:38.000000 tsml-0.0.7/tsml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-20 11:47:38.000000 tsml-0.0.7/tsml.egg-info/top_level.txt
```

### Comparing `tsml-0.0.6/LICENSE` & `tsml-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/PKG-INFO` & `tsml-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsml
-Version: 0.0.6
+Version: 0.0.7
 Summary: A toolkit for time series machine learning algorithms.
 Author-email: Matthew Middlehurst <m.middlehurst@uea.ac.uk>, Tony Bagnall <ajb@uea.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) The Time Series Machine Learning (tsml) developers.
         All rights reserved.
```

### Comparing `tsml-0.0.6/pyproject.toml` & `tsml-0.0.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tsml"
-version = "0.0.6"
+version = "0.0.7"
 description = "A toolkit for time series machine learning algorithms."
 authors = [
     {name = "Matthew Middlehurst", email = "m.middlehurst@uea.ac.uk"},
     {name = "Tony Bagnall", email = "ajb@uea.ac.uk"},
 ]
 readme = "README.md"
 requires-python = ">=3.8,<3.11"
@@ -34,14 +34,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     "numba>=0.55",
     "numpy>=1.21.0",
     "scikit-learn>=1.0.2",
+    "pandas",
 ]
 
 [project.optional-dependencies]
 extras = [
     "pycatch22>=0.4.2",
     "pyfftw>=0.12.0",
     "statsmodels>=0.12.1",
```

### Comparing `tsml-0.0.6/tsml/base.py` & `tsml-0.0.7/tsml/base.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TEST.ts` & `tsml-0.0.7/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TRAIN.ts` & `tsml-0.0.7/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/datasets/MinimalChinatown/MinimalChinatown_TEST.ts` & `tsml-0.0.7/tsml/datasets/MinimalChinatown/MinimalChinatown_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/datasets/MinimalChinatown/MinimalChinatown_TRAIN.ts` & `tsml-0.0.7/tsml/datasets/MinimalChinatown/MinimalChinatown_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TEST.ts` & `tsml-0.0.7/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TRAIN.ts` & `tsml-0.0.7/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TEST.ts` & `tsml-0.0.7/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TRAIN.ts` & `tsml-0.0.7/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TEST.ts` & `tsml-0.0.7/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TRAIN.ts` & `tsml-0.0.7/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TEST.ts` & `tsml-0.0.7/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TRAIN.ts` & `tsml-0.0.7/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/datasets/__init__.py` & `tsml-0.0.7/tsml/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/datasets/_data_io.py` & `tsml-0.0.7/tsml/datasets/_data_io.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/dummy/_dummy.py` & `tsml-0.0.7/tsml/dummy/_dummy.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import numpy as np
 from sklearn.base import ClassifierMixin, ClusterMixin, RegressorMixin
 from sklearn.dummy import DummyClassifier as SklearnDummyClassifier
 from sklearn.dummy import DummyRegressor as SklearnDummyRegressor
 from sklearn.utils import check_random_state
 from sklearn.utils.multiclass import check_classification_targets
-from sklearn.utils.validation import check_is_fitted
+from sklearn.utils.validation import _num_samples, check_is_fitted
 
 from tsml.base import BaseTimeSeriesEstimator
 
 
 class DummyClassifier(ClassifierMixin, BaseTimeSeriesEstimator):
     """DummyClassifier makes predictions that ignore the input features.
 
@@ -81,73 +81,85 @@
     >>> clf = DummyClassifier(strategy="most_frequent")
     >>> clf.fit(X_train, y_train)
     DummyClassifier(strategy='most_frequent')
     >>> clf.score(X_test, y_test)
     0.5
     """
 
-    def __init__(self, strategy="prior", random_state=None, constant=None):
+    def __init__(
+        self, strategy="prior", validate=False, random_state=None, constant=None
+    ):
         self.strategy = strategy
+        self.validate = validate
         self.random_state = random_state
         self.constant = constant
 
         super(DummyClassifier, self).__init__()
 
     def fit(self, X, y):
         """"""
-        X, y = self._validate_data(X=X, y=y, ensure_min_series_length=1)
+        if self.validate:
+            X, y = self._validate_data(X=X, y=y, ensure_min_series_length=1)
 
-        check_classification_targets(y)
+            check_classification_targets(y)
 
-        self.classes_ = np.unique(y)
-        self.n_classes_ = self.classes_.shape[0]
-        self.class_dictionary_ = {}
-        for index, classVal in enumerate(self.classes_):
-            self.class_dictionary_[classVal] = index
+        self.classes_ = np.unique(np.asarray(y))
 
-        if self.n_classes_ == 1:
-            return self
+        if self.validate:
+            self.n_classes_ = self.classes_.shape[0]
+            self.class_dictionary_ = {}
+            for index, classVal in enumerate(self.classes_):
+                self.class_dictionary_[classVal] = index
 
-        self._clf = SklearnDummyClassifier(
+            if self.n_classes_ == 1:
+                return self
+
+        self.clf_ = SklearnDummyClassifier(
             strategy=self.strategy,
             random_state=self.random_state,
             constant=self.constant,
         )
-        self._clf.fit(None, y)
+        self.clf_.fit(None, y)
 
         return self
 
     def predict(self, X) -> np.ndarray:
         """"""
         check_is_fitted(self)
 
-        X = self._validate_data(X=X, reset=False, ensure_min_series_length=1)
+        if self.validate:
+            # treat case of single class seen in fit
+            if self.n_classes_ == 1:
+                return np.repeat(
+                    list(self.class_dictionary_.keys()), X.shape[0], axis=0
+                )
 
-        # treat case of single class seen in fit
-        if self.n_classes_ == 1:
-            return np.repeat(list(self.class_dictionary_.keys()), X.shape[0], axis=0)
+            X = self._validate_data(X=X, reset=False, ensure_min_series_length=1)
 
-        return self._clf.predict(np.zeros(X.shape))
+        return self.clf_.predict(np.zeros((_num_samples(X), 2)))
 
     def predict_proba(self, X) -> np.ndarray:
         """"""
         check_is_fitted(self)
 
-        # treat case of single class seen in fit
-        if self.n_classes_ == 1:
-            return np.repeat([[1]], X.shape[0], axis=0)
+        if self.validate:
+            # treat case of single class seen in fit
+            if self.n_classes_ == 1:
+                return np.repeat([[1]], X.shape[0], axis=0)
 
-        X = self._validate_data(X=X, reset=False, ensure_min_series_length=1)
+            X = self._validate_data(X=X, reset=False, ensure_min_series_length=1)
 
-        return self._clf.predict_proba(np.zeros(X.shape))
+        return self.clf_.predict_proba(np.zeros((_num_samples(X), 2)))
 
     def _more_tags(self):
         return {
             "X_types": ["3darray", "2darray", "np_list"],
             "equal_length_only": False,
+            "no_validation": not self.validate,
+            "allow_nan": True,
         }
 
 
 class DummyRegressor(RegressorMixin, BaseTimeSeriesEstimator):
     """DummyRegressor makes predictions that ignore the input features.
 
     This regressor is useful as a simple baseline to compare with other
@@ -195,44 +207,49 @@
     >>> reg = DummyRegressor()
     >>> reg.fit(X_train, y_train)
     DummyRegressor()
     >>> reg.score(X_test, y_test)
     -0.07184048625633688
     """
 
-    def __init__(self, strategy="mean", constant=None, quantile=None):
+    def __init__(self, strategy="mean", validate=False, constant=None, quantile=None):
         self.strategy = strategy
+        self.validate = validate
         self.constant = constant
         self.quantile = quantile
 
         super(DummyRegressor, self).__init__()
 
     def fit(self, X, y):
         """"""
-        _, y = self._validate_data(X=X, y=y, ensure_min_series_length=1)
+        if self.validate:
+            _, y = self._validate_data(X=X, y=y, ensure_min_series_length=1)
 
-        self._reg = SklearnDummyRegressor(
+        self.reg_ = SklearnDummyRegressor(
             strategy=self.strategy, constant=self.constant, quantile=self.quantile
         )
-        self._reg.fit(None, y)
+        self.reg_.fit(None, y)
 
         return self
 
     def predict(self, X):
         """"""
         check_is_fitted(self)
 
-        X = self._validate_data(X=X, reset=False, ensure_min_series_length=1)
+        if self.validate:
+            X = self._validate_data(X=X, reset=False, ensure_min_series_length=1)
 
-        return self._reg.predict(np.zeros(X.shape))
+        return self.reg_.predict(np.zeros((_num_samples(X), 2)))
 
     def _more_tags(self):
         return {
             "X_types": ["3darray", "2darray", "np_list"],
             "equal_length_only": False,
+            "no_validation": not self.validate,
+            "allow_nan": True,
         }
 
 
 class DummyClusterer(ClusterMixin, BaseTimeSeriesEstimator):
     """DummyRegressor makes predictions that ignore the input features.
 
     This cluster makes no effort to form reasonable clusters, and is primarily used
@@ -253,24 +270,28 @@
     DummyClusterer(random_state=0, strategy='random')
     >>> adjusted_rand_score(clu.labels_, y_train)
     0.2087729039422543
     >>> adjusted_rand_score(clu.predict(X_test), y_test)
     0.2087729039422543
     """
 
-    def __init__(self, strategy="single", n_clusters=2, random_state=None):
+    def __init__(
+        self, strategy="single", validate=False, n_clusters=2, random_state=None
+    ):
         self.strategy = strategy
+        self.validate = validate
         self.n_clusters = n_clusters
         self.random_state = random_state
 
         super(DummyClusterer, self).__init__()
 
     def fit(self, X, y=None):
         """"""
-        X = self._validate_data(X=X, ensure_min_series_length=1)
+        if self.validate:
+            X = self._validate_data(X=X, ensure_min_series_length=1)
 
         if self.strategy == "single":
             self.labels_ = np.zeros(len(X), dtype=np.int32)
         elif self.strategy == "unique":
             self.labels_ = np.arange(len(X), dtype=np.int32)
         elif self.strategy == "random":
             rng = check_random_state(self.random_state)
@@ -280,24 +301,27 @@
 
         return self
 
     def predict(self, X):
         """"""
         check_is_fitted(self)
 
-        X = self._validate_data(X=X, reset=False, ensure_min_series_length=1)
+        if self.validate:
+            X = self._validate_data(X=X, reset=False, ensure_min_series_length=1)
 
         if self.strategy == "single":
-            return np.zeros(len(X), dtype=np.int32)
+            return np.zeros(_num_samples(X), dtype=np.int32)
         elif self.strategy == "unique":
-            return np.arange(len(X), dtype=np.int32)
+            return np.arange(_num_samples(X), dtype=np.int32)
         elif self.strategy == "random":
             rng = check_random_state(self.random_state)
-            return rng.randint(self.n_clusters, size=len(X), dtype=np.int32)
+            return rng.randint(self.n_clusters, size=_num_samples(X), dtype=np.int32)
         else:
             raise ValueError(f"Unknown strategy {self.strategy}")
 
     def _more_tags(self):
         return {
             "X_types": ["3darray", "2darray", "np_list"],
             "equal_length_only": False,
+            "no_validation": not self.validate,
+            "allow_nan": True,
         }
```

### Comparing `tsml-0.0.6/tsml/feature_based/_catch22.py` & `tsml-0.0.7/tsml/feature_based/_catch22.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/interval_based/__init__.py` & `tsml-0.0.7/tsml/interval_based/__init__.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/interval_based/_base.py` & `tsml-0.0.7/tsml/interval_based/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,14 +210,16 @@
     # be able to skip transforming features in predict
     transformer_feature_skip = ["transform_features_", "_transform_features"]
 
     def fit(self, X, y):
         X, y = self._validate_data(X=X, y=y, ensure_min_samples=2)
         X = self._convert_X(X)
 
+        rng = check_random_state(self.random_state)
+
         self.n_instances_, self.n_dims_, self.series_length_ = X.shape
         if is_classifier(self):
             check_classification_targets(y)
 
             self.classes_ = np.unique(y)
             self.n_classes_ = self.classes_.shape[0]
             self.class_dictionary_ = {}
@@ -256,31 +258,29 @@
 
         # use the base series if series_transformers is None
         if self.series_transformers is None or self.series_transformers == []:
             Xt = [X]
             self._series_transformers = [None]
         # clone series_transformers if it is a transformer and transform the input data
         elif is_transformer(self.series_transformers):
-            t = _clone_estimator(
-                self.series_transformers, random_state=self.random_state
-            )
+            t = _clone_estimator(self.series_transformers, random_state=rng)
             Xt = [t.fit_transform(X, y)]
             self._series_transformers = [t]
         # clone each series_transformers transformer and include the base series if None
         # is in the list
         elif isinstance(self.series_transformers, (list, tuple)):
             Xt = []
             self._series_transformers = []
 
             for transformer in self.series_transformers:
                 if transformer is None:
                     Xt.append(X)
                     self._series_transformers.append(None)
                 elif is_transformer(transformer):
-                    t = _clone_estimator(transformer, random_state=self.random_state)
+                    t = _clone_estimator(transformer, random_state=rng)
                     Xt.append(t.fit_transform(X, y))
                     self._series_transformers.append(t)
                 else:
                     raise ValueError()  # todo error for invalid self.series_transformers
         # other inputs are invalid
         else:
             raise ValueError()  # todo error for invalid self.series_transformers
@@ -454,15 +454,16 @@
         # we store whether each series_transformer contains a transformer and/or
         # function in its interval_features
         self._interval_transformer = [False] * len(Xt)
         self._interval_function = [False] * len(Xt)
         # single transformer or function for all series_transformers
         if is_transformer(self.interval_features):
             self._interval_transformer = [True] * len(Xt)
-            self._interval_features = [[self.interval_features]] * len(Xt)
+            transformer = _clone_estimator(self.interval_features, random_state=rng)
+            self._interval_features = [[transformer]] * len(Xt)
         elif callable(self.interval_features):
             self._interval_function = [True] * len(Xt)
             self._interval_features = [[self.interval_features]] * len(Xt)
         elif isinstance(self.interval_features, (list, tuple)):
             # if input is a list and only contains transformers or functions, use the
             # list for all series in Xt
             if all(
@@ -487,26 +488,28 @@
             else:
                 self._interval_features = []
                 for i, feature in enumerate(self.interval_features):
                     if isinstance(feature, (list, tuple)):
                         for method in feature:
                             if is_transformer(method):
                                 self._interval_transformer[i] = True
+                                feature = _clone_estimator(feature, random_state=rng)
                             elif callable(method):
                                 self._interval_function[i] = True
                             else:
                                 raise ValueError(
                                     "Individual items in a interval_features list or "
                                     "tuple must be a transformer or function. Input "
                                     f"{feature} does not contain only transformers and "
                                     f"functions."
                                 )
                         self._interval_features.append(feature)
                     elif is_transformer(feature):
                         self._interval_transformer[i] = True
+                        feature = _clone_estimator(feature, random_state=rng)
                         self._interval_features.append([feature])
                     elif callable(feature):
                         self._interval_function[i] = True
                         self._interval_features.append([feature])
                     else:
                         raise ValueError(
                             "Individual items in a interval_features list or tuple "
@@ -1026,8 +1029,7 @@
                 self.replace_nan,
             )
 
         if predict_proba:
             return estimator.predict_proba(interval_features)
         else:
             return estimator.predict(interval_features)
-
```

### Comparing `tsml-0.0.6/tsml/interval_based/_cif.py` & `tsml-0.0.7/tsml/interval_based/_cif.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/interval_based/_interval_forest.py` & `tsml-0.0.7/tsml/interval_based/_interval_forest.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/interval_based/_interval_pipelines.py` & `tsml-0.0.7/tsml/interval_based/_interval_pipelines.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,15 @@
         -----
         Changes state by creating a fitted model that updates attributes
         ending in "_" and sets is_fitted flag to True.
         """
         X, y = self._validate_data(
             X=X, y=y, ensure_min_samples=2, ensure_min_series_length=3
         )
+        X = self._convert_X(X)
 
         self.n_instances_, self.n_dims_, self.series_length_ = X.shape
         self.classes_ = np.unique(y)
         self.n_classes_ = self.classes_.shape[0]
         self.class_dictionary_ = {}
         for index, classVal in enumerate(self.classes_):
             self.class_dictionary_[classVal] = index
@@ -148,14 +149,15 @@
         -------
         y : array-like, shape = [n_instances]
             Predicted class labels.
         """
         check_is_fitted(self)
 
         X = self._validate_data(X=X, reset=False, ensure_min_series_length=3)
+        X = self._convert_X(X)
 
         return self._estimator.predict(self._transformer.transform(X))
 
     def predict_proba(self, X) -> np.ndarray:
         """Predict class probabilities for n instances in X.
 
         Parameters
@@ -167,14 +169,15 @@
         -------
         y : array-like, shape = [n_instances, n_classes_]
             Predicted probabilities using the ordering in classes_.
         """
         check_is_fitted(self)
 
         X = self._validate_data(X=X, reset=False, ensure_min_series_length=3)
+        X = self._convert_X(X)
 
         m = getattr(self._estimator, "predict_proba", None)
         if callable(m):
             return self._estimator.predict_proba(self._transformer.transform(X))
         else:
             dists = np.zeros((X.shape[0], self.n_classes_))
             preds = self._estimator.predict(self._transformer.transform(X))
@@ -307,14 +310,15 @@
         -----
         Changes state by creating a fitted model that updates attributes
         ending in "_" and sets is_fitted flag to True.
         """
         X, y = self._validate_data(
             X=X, y=y, ensure_min_samples=2, ensure_min_series_length=3
         )
+        X = self._convert_X(X)
 
         self.n_instances_, self.n_dims_, self.series_length_ = X.shape
 
         self._n_jobs = check_n_jobs(self.n_jobs)
 
         interval_transformers = (
             Catch22Transformer(catch24=True, outlier_norm=True, replace_nans=True)
@@ -355,14 +359,15 @@
         -------
         y : array-like, shape = [n_instances]
             Predicted class labels.
         """
         check_is_fitted(self)
 
         X = self._validate_data(X=X, reset=False, ensure_min_series_length=3)
+        X = self._convert_X(X)
 
         return self._estimator.predict(self._transformer.transform(X))
 
     @classmethod
     def get_test_params(cls, parameter_set="default"):
         """Return testing parameter settings for the estimator.
 
@@ -485,14 +490,15 @@
         -----
         Changes state by creating a fitted model that updates attributes
         ending in "_" and sets is_fitted flag to True.
         """
         X, y = self._validate_data(
             X=X, y=y, ensure_min_samples=2, ensure_min_series_length=7
         )
+        X = self._convert_X(X)
 
         self.n_instances_, self.n_dims_, self.series_length_ = X.shape
         self.classes_ = np.unique(y)
         self.n_classes_ = self.classes_.shape[0]
         self.class_dictionary_ = {}
         for index, classVal in enumerate(self.classes_):
             self.class_dictionary_[classVal] = index
@@ -538,14 +544,15 @@
         -------
         y : array-like, shape = [n_instances]
             Predicted class labels.
         """
         check_is_fitted(self)
 
         X = self._validate_data(X=X, reset=False, ensure_min_series_length=7)
+        X = self._convert_X(X)
 
         return self._estimator.predict(self._transformer.transform(X))
 
     def predict_proba(self, X) -> np.ndarray:
         """Predict class probabilities for n instances in X.
 
         Parameters
@@ -557,14 +564,15 @@
         -------
         y : array-like, shape = [n_instances, n_classes_]
             Predicted probabilities using the ordering in classes_.
         """
         check_is_fitted(self)
 
         X = self._validate_data(X=X, reset=False, ensure_min_series_length=7)
+        X = self._convert_X(X)
 
         m = getattr(self._estimator, "predict_proba", None)
         if callable(m):
             return self._estimator.predict_proba(self._transformer.transform(X))
         else:
             dists = np.zeros((X.shape[0], self.n_classes_))
             preds = self._estimator.predict(self._transformer.transform(X))
```

### Comparing `tsml-0.0.6/tsml/interval_based/_rise.py` & `tsml-0.0.7/tsml/interval_based/_rise.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/interval_based/_stsf.py` & `tsml-0.0.7/tsml/interval_based/_stsf.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/interval_based/_tsf.py` & `tsml-0.0.7/tsml/interval_based/_tsf.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/shapelet_based/_stc.py` & `tsml-0.0.7/tsml/shapelet_based/_stc.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/tests/test_interface.py` & `tsml-0.0.7/tsml/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/transformations/__init__.py` & `tsml-0.0.7/tsml/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/transformations/_ar_coefficient.py` & `tsml-0.0.7/tsml/transformations/_ar_coefficient.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,8 +46,8 @@
 
         if self.replace_nan:
             Xt[np.isnan(Xt)] = 0
 
         return Xt
 
     def _more_tags(self):
-        return {"stateless": True, "optional_dependency": True}
+        return {"requires_fit": False, "optional_dependency": True}
```

### Comparing `tsml-0.0.6/tsml/transformations/_catch22.py` & `tsml-0.0.7/tsml/transformations/_catch22.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 import numpy as np
 from joblib import Parallel
 from numba import njit
 from sklearn.base import TransformerMixin
 from sklearn.utils.fixes import delayed
 
 from tsml.base import BaseTimeSeriesEstimator
+from tsml.utils.numba_functions.general import (
+    z_normalise_series,
+    z_normalise_series_with_mean,
+)
+from tsml.utils.numba_functions.stats import mean, numba_max, numba_min
 from tsml.utils.validation import _check_optional_dependency, check_n_jobs
 
 feature_names = [
     "DN_HistogramMode_5",
     "DN_HistogramMode_10",
     "SB_BinaryStats_diff_longstretch0",
     "DN_OutlierInclude_p_001_mdrmd",
@@ -238,54 +243,54 @@
                 if not transform_feature[f_count]:
                     continue
 
                 args = [series]
 
                 if feature == 0 or feature == 1 or feature == 11:
                     if smin is None:
-                        smin = np.min(series)
+                        smin = numba_min(series)
                     if smax is None:
-                        smax = np.max(series)
+                        smax = numba_max(series)
                     args = [series, smin, smax]
                 elif feature == 2 or feature == 22:
                     if smean is None:
-                        smean = np.mean(series)
+                        smean = mean(series)
                     args = [series, smean]
                 elif feature == 3 or feature == 4:
                     if self.outlier_norm:
                         if smean is None:
-                            smean = np.mean(series)
+                            smean = mean(series)
                         if outlier_series is None:
-                            outlier_series = _normalise_series(series, smean)
+                            outlier_series = z_normalise_series_with_mean(series, smean)
                         args = [outlier_series]
                     else:
                         args = [series]
                 elif feature == 7 or feature == 8:
                     if smean is None:
-                        smean = np.mean(series)
+                        smean = mean(series)
                     if fft is None:
                         nfft = int(
                             np.power(2, np.ceil(np.log(len(series)) / np.log(2)))
                         )
                         fft = np.fft.fft(series - smean, n=nfft)
                     args = [series, fft]
                 elif feature == 5 or feature == 6 or feature == 12:
                     if smean is None:
-                        smean = np.mean(series)
+                        smean = mean(series)
                     if fft is None:
                         nfft = int(
                             np.power(2, np.ceil(np.log(len(series)) / np.log(2)))
                         )
                         fft = np.fft.fft(series - smean, n=nfft)
                     if ac is None:
                         ac = _autocorr(series, fft)
                     args = [ac]
                 elif feature == 16 or feature == 17 or feature == 20:
                     if smean is None:
-                        smean = np.mean(series)
+                        smean = mean(series)
                     if fft is None:
                         nfft = int(
                             np.power(2, np.ceil(np.log(len(series)) / np.log(2)))
                         )
                         fft = np.fft.fft(series - smean, n=nfft)
                     if ac is None:
                         ac = _autocorr(series, fft)
@@ -299,15 +304,15 @@
                     c22[dim + n] = np.std(series)
                 else:
                     c22[dim + n] = features[feature](*args)
 
         return c22
 
     def _more_tags(self):
-        return {"X_types": ["np_list", "3darray"], "stateless": True}
+        return {"X_types": ["np_list", "3darray"], "requires_fit": False}
 
     @staticmethod
     def _DN_HistogramMode_5(X, smin, smax):
         # Mode of z-scored distribution (5-bin histogram).
         return _histogram_mode(X, 5, smin, smax)
 
     @staticmethod
@@ -1168,22 +1173,14 @@
             y_out[j] = (
                 y_out[j] * (j - breaks[1] * second_half) + coeffs_spline[second_half][i]
             )
 
     return y_out
 
 
-@njit(fastmath=True, cache=True)
-def _normalise_series(X, mean):
-    std = np.std(X)
-    if std > 0:
-        return (X - mean) / std
-    return X
-
-
 def _verify_features(features, catch24):
     if isinstance(features, str):
         if features == "all":
             f_idx = [i for i in range(22)]
             if catch24:
                 f_idx += [22, 23]
         elif features in feature_names:
@@ -1413,18 +1410,15 @@
 
         f_count = -1
         for i in range(len(X)):
             dim = i * len(f_idx)
             series = list(X[i])
 
             if self.outlier_norm and (3 in f_idx or 4 in f_idx):
-                outlier_series = np.array(series)
-                outlier_series = list(
-                    _normalise_series(outlier_series, np.mean(outlier_series))
-                )
+                outlier_series = list(z_normalise_series(X[i]))
 
             for n, feature in enumerate(f_idx):
                 f_count += 1
                 if not transform_feature[f_count]:
                     continue
 
                 if self.outlier_norm and feature in [3, 4]:
@@ -1437,10 +1431,10 @@
                     c22[dim + n] = features[feature](series)
 
         return c22
 
     def _more_tags(self):
         return {
             "X_types": ["np_list", "3darray"],
-            "stateless": True,
+            "requires_fit": False,
             "optional_dependency": True,
         }
```

### Comparing `tsml-0.0.6/tsml/transformations/_function_transformer.py` & `tsml-0.0.7/tsml/transformations/_function_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,10 +98,10 @@
         func = self.func if self.func is not None else _identity
 
         return func(X, **(self.kw_args if self.kw_args else {}))
 
     def _more_tags(self):
         return {
             "no_validation": not self.validate,
-            "stateless": True,
+            "requires_fit": False,
             "X_types": ["3darray", "2darray", "np_list"],
         }
```

### Comparing `tsml-0.0.6/tsml/transformations/_interval_extraction.py` & `tsml-0.0.7/tsml/transformations/_interval_extraction.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/transformations/_periodogram.py` & `tsml-0.0.7/tsml/transformations/_periodogram.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,8 +60,8 @@
             pyfftw.config.NUM_THREADS = old_threads
         else:
             Xt = np.abs(np.fft.fft(X)[:, :, : int(X.shape[2] / 2)])
 
         return Xt
 
     def _more_tags(self):
-        return {"stateless": True, "optional_dependency": True}
+        return {"requires_fit": False, "optional_dependency": True}
```

### Comparing `tsml-0.0.6/tsml/transformations/_sfa.py` & `tsml-0.0.7/tsml/transformations/_sfa.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/transformations/_shapelet_transform.py` & `tsml-0.0.7/tsml/transformations/_shapelet_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,14 +179,15 @@
 
         Returns
         -------
         self : RandomShapeletTransformer
             This estimator.
         """
         X, y = self._validate_data(X=X, y=y, ensure_min_samples=2)
+        X = self._convert_X(X)
 
         self.n_instances_, self.n_dims_, self.series_length_ = X.shape
         self.classes_, self._class_counts = np.unique(y, return_counts=True)
         self.n_classes_ = self.classes_.shape[0]
         self.class_dictionary_ = {}
         for index, classVal in enumerate(self.classes_):
             self.class_dictionary_[classVal] = index
@@ -331,14 +332,15 @@
         -------
         output : pandas DataFrame
             The transformed dataframe in tabular format.
         """
         check_is_fitted(self)
 
         X = self._validate_data(X=X, reset=True)
+        X = self._convert_X(X)
 
         output = np.zeros((len(X), len(self.shapelets_)))
 
         for i, series in enumerate(X):
             dists = Parallel(
                 n_jobs=self._n_jobs, backend=self.parallel_backend, prefer="threads"
             )(
```

### Comparing `tsml-0.0.6/tsml/transformations/_summary_features.py` & `tsml-0.0.7/tsml/transformations/_summary_features.py`

 * *Files 11% similar despite different names*

```diff
@@ -83,8 +83,8 @@
                     Xt[i, idx : idx + n_dims] = row_quantile(X[i], f)
                 else:
                     Xt[i, idx : idx + n_dims] = f(X[i])
 
         return Xt
 
     def _more_tags(self):
-        return {"stateless": True}
+        return {"requires_fit": False}
```

### Comparing `tsml-0.0.6/tsml/utils/_tags.py` & `tsml-0.0.7/tsml/utils/_tags.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,31 +7,22 @@
 
 import numpy as np
 from sklearn.base import BaseEstimator
 
 _DEFAULT_TAGS = {
     # sklearn tags
     "non_deterministic": False,
-    "requires_positive_X": False,
-    "requires_positive_y": False,
     "X_types": ["3darray"],
-    "poor_score": False,
     "no_validation": False,
-    "multioutput": False,
     "allow_nan": False,
-    "stateless": False,
-    "multilabel": False,
-    "_skip_test": False,
-    "_xfail_checks": False,
-    "multioutput_only": False,
-    "binary_only": False,
-    "requires_fit": True,
     "preserves_dtype": [np.float64],
+    "requires_fit": True,
     "requires_y": False,
-    "pairwise": False,
+    "_skip_test": False,
+    "_xfail_checks": False,
     # tsml tags
     "optional_dependency": False,
     "univariate_only": False,
     "equal_length_only": True,
 }
```

### Comparing `tsml-0.0.6/tsml/utils/discovery.py` & `tsml-0.0.7/tsml/utils/discovery.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/utils/numba_functions/general.py` & `tsml-0.0.7/tsml/utils/numba_functions/general.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,14 +132,46 @@
     >>> X = np.array([[[1, 2, 2, 3, 3, 3, 4, 4, 4, 4], [5, 6, 6, 7, 7, 7, 8, 8, 8, 8]]])
     >>> diff = first_order_differences_3d(X)
     """
     return X[:, :, 1:] - X[:, :, :-1]
 
 
 @njit(fastmath=True, cache=True)
+def z_normalise_series_with_mean(X: np.ndarray, series_mean: float) -> np.ndarray:
+    """Numba series normalization function for a 1d numpy array with mean.
+
+    Parameters
+    ----------
+    X : 1d numpy array
+        A 1d numpy array of values
+    series_mean : float
+        The mean of the series
+
+    Returns
+    -------
+    arr : 1d numpy array
+        The normalised series
+
+    Examples
+    --------
+    >>> import numpy as np
+    >>> from tsml.utils.numba_functions.general import z_normalise_series_with_mean
+    >>> from tsml.utils.numba_functions.stats import mean
+    >>> X = np.array([1, 2, 2, 3, 3, 3, 4, 4, 4, 4])
+    >>> X_norm = z_normalise_series_with_mean(X, mean(X))
+    """
+    s = stats.std(X)
+    if s > 0:
+        arr = (X - series_mean) / s
+    else:
+        arr = X - series_mean
+    return arr
+
+
+@njit(fastmath=True, cache=True)
 def z_normalise_series(X: np.ndarray) -> np.ndarray:
     """Numba series normalization function for a 1d numpy array.
 
     Parameters
     ----------
     X : 1d numpy array
         A 1d numpy array of values
```

### Comparing `tsml-0.0.6/tsml/utils/numba_functions/stats.py` & `tsml-0.0.7/tsml/utils/numba_functions/stats.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/utils/testing.py` & `tsml-0.0.7/tsml/utils/testing.py`

 * *Files 5% similar despite different names*

```diff
@@ -109,14 +109,15 @@
 
 
 def generate_3d_test_data(
     n_samples: int = 10,
     n_channels: int = 1,
     series_length: int = 12,
     n_labels: int = 2,
+    regression_target: bool = False,
     random_state: Union[int, None] = None,
 ) -> Tuple[np.ndarray, np.ndarray]:
     """Randomly generate 3D data for testing.
 
     Will ensure there is at least one sample per label.
 
     Parameters
@@ -125,14 +126,16 @@
         The number of samples to generate.
     n_channels : int
         The number of series channels to generate.
     series_length : int
         The number of features/series length to generate.
     n_labels : int
         The number of unique labels to generate.
+    regression_target : bool
+        If True, the target will be a float, otherwise an int.
     random_state : int or None
         Seed for random number generation.
 
     Returns
     -------
     X : np.ndarray
         Randomly generated 3D data.
@@ -148,40 +151,49 @@
     ...     series_length=10,
     ...     n_labels=3,
     ... )
     """
     rng = np.random.RandomState(random_state)
     X = n_labels * rng.uniform(size=(n_samples, n_channels, series_length))
     y = X[:, 0, 0].astype(int)
+
     for i in range(n_labels):
         if len(y) > i:
             X[i, 0, 0] = i
             y[i] = i
     X = X * (y[:, None, None] + 1)
+
+    if regression_target:
+        y = y.astype(np.float32)
+        y += rng.uniform(size=y.shape)
+
     return X, y
 
 
 def generate_2d_test_data(
     n_samples: int = 10,
     series_length: int = 8,
     n_labels: int = 2,
+    regression_target: bool = False,
     random_state: Union[int, None] = None,
 ) -> Tuple[np.ndarray, np.ndarray]:
     """Randomly generate 2D data for testing.
 
     Will ensure there is at least one sample per label.
 
     Parameters
     ----------
     n_samples : int
         The number of samples to generate.
     series_length : int
         The number of features/series length to generate.
     n_labels : int
         The number of unique labels to generate.
+    regression_target : bool
+        If True, the target will be a float, otherwise an int.
     random_state : int or None
         Seed for random number generation.
 
     Returns
     -------
     X : np.ndarray
         Randomly generated 2D data.
@@ -196,28 +208,35 @@
     ...     series_length=10,
     ...     n_labels=3,
     ... )
     """
     rng = np.random.RandomState(random_state)
     X = n_labels * rng.uniform(size=(n_samples, series_length))
     y = X[:, 0].astype(int)
+
     for i in range(n_labels):
         if len(y) > i:
             X[i, 0] = i
             y[i] = i
     X = X * (y[:, None] + 1)
+
+    if regression_target:
+        y = y.astype(np.float32)
+        y += rng.uniform(size=y.shape)
+
     return X, y
 
 
 def generate_unequal_test_data(
     n_samples: int = 10,
     n_channels: int = 1,
     min_series_length: int = 6,
     max_series_length: int = 8,
     n_labels: int = 2,
+    regression_target: bool = False,
     random_state: Union[int, None] = None,
 ) -> Tuple[List[np.ndarray], np.ndarray]:
     """Randomly generate unequal length 3D data for testing.
 
     Will ensure there is at least one sample per label.
 
     Parameters
@@ -228,14 +247,16 @@
         The number of series channels to generate.
     min_series_length : int
         The minimum number of features/series length to generate for invidiaul series.
     max_series_length : int
         The maximum number of features/series length to generate for invidiaul series.
     n_labels : int
         The number of unique labels to generate.
+    regression_target : bool
+        If True, the target will be a float, otherwise an int.
     random_state : int or None
         Seed for random number generation.
 
     Returns
     -------
     X : list of np.ndarray
         Randomly generated unequal length 3D data.
@@ -251,22 +272,26 @@
     ...     min_series_length=8,
     ...     max_series_length=12,
     ...     n_labels=3,
     ... )
     """
     rng = np.random.RandomState(random_state)
     X = []
-    y = np.zeros(n_samples)
+    y = np.zeros(n_samples, dtype=np.int32)
 
     for i in range(n_samples):
         series_length = rng.randint(min_series_length, max_series_length + 1)
         x = n_labels * rng.uniform(size=(n_channels, series_length))
         label = x[0, 0].astype(int)
         if i < n_labels and n_samples > i:
             x[0, 0] = i
             label = i
         x = x * (label + 1)
 
         X.append(x)
         y[i] = label
 
+    if regression_target:
+        y = y.astype(np.float32)
+        y += rng.uniform(size=y.shape)
+
     return X, y
```

### Comparing `tsml-0.0.6/tsml/utils/validation.py` & `tsml-0.0.7/tsml/utils/validation.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/vector/_cit.py` & `tsml-0.0.7/tsml/vector/_cit.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/vector/_rotation_forest.py` & `tsml-0.0.7/tsml/vector/_rotation_forest.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml/vector/tests/test_rotation_forest.py` & `tsml-0.0.7/tsml/vector/tests/test_rotation_forest.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.6/tsml.egg-info/PKG-INFO` & `tsml-0.0.7/tsml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsml
-Version: 0.0.6
+Version: 0.0.7
 Summary: A toolkit for time series machine learning algorithms.
 Author-email: Matthew Middlehurst <m.middlehurst@uea.ac.uk>, Tony Bagnall <ajb@uea.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) The Time Series Machine Learning (tsml) developers.
         All rights reserved.
```

### Comparing `tsml-0.0.6/tsml.egg-info/SOURCES.txt` & `tsml-0.0.7/tsml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

