# Comparing `tmp/espm-0.1.4.tar.gz` & `tmp/espm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "espm-0.1.4.tar", last modified: Thu Feb 23 15:09:09 2023, max compression
+gzip compressed data, was "espm-0.2.0.tar", last modified: Thu Apr 20 14:38:31 2023, max compression
```

## Comparing `espm-0.1.4.tar` & `espm-0.2.0.tar`

### file list

```diff
@@ -1,143 +1,114 @@
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-02-23 15:09:09.365387 espm-0.1.4/
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-02-23 15:09:09.333058 espm-0.1.4/.github/
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-02-23 15:09:09.336865 espm-0.1.4/.github/workflows/
--rw-r--r--   0 nati       (501) staff       (20)     1119 2023-02-23 15:04:13.000000 espm-0.1.4/.github/workflows/python.yml
--rw-r--r--   0 nati       (501) staff       (20)      178 2023-02-21 16:38:53.000000 espm-0.1.4/.readthedocs.yml
--rw-r--r--   0 nati       (501) staff       (20)      404 2023-02-21 14:45:32.000000 espm-0.1.4/CHANGELOG.rst
--rw-r--r--   0 nati       (501) staff       (20)     3993 2023-02-22 09:05:19.000000 espm-0.1.4/CONTRIBUTING.rst
--rw-r--r--   0 nati       (501) staff       (20)     1083 2022-12-06 13:16:22.000000 espm-0.1.4/Licence.txt
--rw-r--r--   0 nati       (501) staff       (20)      408 2023-02-22 10:49:09.000000 espm-0.1.4/MANIFEST.in
--rw-r--r--   0 nati       (501) staff       (20)     3867 2023-02-23 15:09:09.365226 espm-0.1.4/PKG-INFO
--rw-r--r--   0 nati       (501) staff       (20)     2830 2023-02-23 14:48:12.000000 espm-0.1.4/README.rst
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-02-23 15:09:09.340797 espm-0.1.4/doc/
--rw-r--r--   0 nati       (501) staff       (20)       30 2020-12-17 09:02:04.000000 espm-0.1.4/doc/changelog.rst
--rw-r--r--   0 nati       (501) staff       (20)     1994 2023-02-23 09:58:20.000000 espm-0.1.4/doc/conf.py
--rw-r--r--   0 nati       (501) staff       (20)       33 2019-04-30 16:36:26.000000 espm-0.1.4/doc/contributing.rst
--rw-r--r--   0 nati       (501) staff       (20)      213 2023-02-23 09:10:02.000000 espm-0.1.4/doc/index.rst
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-02-23 15:09:09.340920 espm-0.1.4/doc/introduction/
--rw-r--r--   0 nati       (501) staff       (20)     4460 2023-02-23 15:04:47.000000 espm-0.1.4/doc/introduction/index.rst
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-02-23 15:09:09.341781 espm-0.1.4/doc/reference/
--rw-r--r--   0 nati       (501) staff       (20)      203 2023-02-23 09:35:43.000000 espm-0.1.4/doc/reference/datasets.rst
--rw-r--r--   0 nati       (501) staff       (20)      202 2023-02-21 16:38:50.000000 espm-0.1.4/doc/reference/estimators.rst
--rw-r--r--   0 nati       (501) staff       (20)      141 2023-02-23 09:35:25.000000 espm-0.1.4/doc/reference/index.rst
--rw-r--r--   0 nati       (501) staff       (20)       58 2023-02-21 16:38:50.000000 espm-0.1.4/doc/reference/measures.rst
--rw-r--r--   0 nati       (501) staff       (20)      206 2023-02-23 09:21:51.000000 espm-0.1.4/doc/reference/models.rst
--rw-r--r--   0 nati       (501) staff       (20)       45 2023-02-21 16:38:50.000000 espm-0.1.4/doc/reference/utils.rst
--rw-r--r--   0 nati       (501) staff       (20)       53 2023-02-22 16:28:40.000000 espm-0.1.4/doc/reference/weights.rst
--rw-r--r--   0 nati       (501) staff       (20)       95 2019-04-30 16:36:26.000000 espm-0.1.4/doc/references.rst
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-02-23 15:09:09.341891 espm-0.1.4/doc/styles/
--rw-r--r--   0 nati       (501) staff       (20)      332 2023-02-20 15:43:46.000000 espm-0.1.4/doc/styles/sg_gallery.css
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-02-23 15:09:09.346638 espm-0.1.4/espm/
--rw-r--r--   0 nati       (501) staff       (20)       21 2023-02-23 15:07:12.000000 espm-0.1.4/espm/__init__.py
--rw-r--r--   0 nati       (501) staff       (20)     1899 2023-02-23 09:58:20.000000 espm-0.1.4/espm/conf.py
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-02-23 15:09:09.349778 espm-0.1.4/espm/datasets/
--rw-r--r--   0 nati       (501) staff       (20)      187 2023-02-23 09:58:20.000000 espm-0.1.4/espm/datasets/__init__.py
--rw-r--r--   0 nati       (501) staff       (20)     6635 2023-02-23 09:58:20.000000 espm-0.1.4/espm/datasets/base.py
--rw-r--r--   0 nati       (501) staff       (20)     3909 2023-02-23 09:58:20.000000 espm-0.1.4/espm/datasets/built_in_datasets.py
--rw-r--r--   0 nati       (501) staff       (20)     3894 2023-02-23 09:58:20.000000 espm-0.1.4/espm/datasets/generate_EDXS_phases.py
--rw-r--r--   0 nati       (501) staff       (20)     7180 2023-02-23 09:58:20.000000 espm-0.1.4/espm/datasets/generate_weights.py
--rw-r--r--   0 nati       (501) staff       (20)     3211 2023-02-23 12:13:33.000000 espm-0.1.4/espm/datasets/samples.py
--rw-r--r--   0 nati       (501) staff       (20)     9139 2023-02-23 09:58:20.000000 espm-0.1.4/espm/datasets/spim.py
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-02-23 15:09:09.350047 espm-0.1.4/espm/datasets/toy-problem/
--rw-r--r--   0 nati       (501) staff       (20)     4316 2023-02-21 16:38:50.000000 espm-0.1.4/espm/datasets/toy-problem/phase1.png
--rw-r--r--   0 nati       (501) staff       (20)     6798 2023-02-21 16:38:50.000000 espm-0.1.4/espm/datasets/toy-problem/phase2.png
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-02-23 15:09:09.352443 espm-0.1.4/espm/estimators/
--rw-r--r--   0 nati       (501) staff       (20)      529 2023-02-23 09:58:20.000000 espm-0.1.4/espm/estimators/__init__.py
--rw-r--r--   0 nati       (501) staff       (20)    19415 2023-02-23 13:48:32.000000 espm-0.1.4/espm/estimators/base.py
--rw-r--r--   0 nati       (501) staff       (20)     6026 2023-02-23 09:58:20.000000 espm-0.1.4/espm/estimators/dicotomy.py
--rw-r--r--   0 nati       (501) staff       (20)    10252 2023-02-23 14:37:13.000000 espm-0.1.4/espm/estimators/smooth_nmf.py
--rw-r--r--   0 nati       (501) staff       (20)     5700 2023-02-23 09:58:20.000000 espm-0.1.4/espm/estimators/surrogates.py
--rw-r--r--   0 nati       (501) staff       (20)    11222 2023-02-23 09:58:20.000000 espm-0.1.4/espm/estimators/updates.py
--rwxr-xr-x   0 nati       (501) staff       (20)      139 2023-02-21 16:38:50.000000 espm-0.1.4/espm/hyperspy_extension.yaml
--rw-r--r--   0 nati       (501) staff       (20)    19689 2023-02-23 15:06:34.000000 espm-0.1.4/espm/measures.py
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-02-23 15:09:09.353124 espm-0.1.4/espm/models/
--rw-r--r--   0 nati       (501) staff       (20)    12821 2023-02-23 09:58:20.000000 espm-0.1.4/espm/models/EDXS_function.py
--rw-r--r--   0 nati       (501) staff       (20)      377 2023-02-23 09:58:20.000000 espm-0.1.4/espm/models/__init__.py
--rw-r--r--   0 nati       (501) staff       (20)     8845 2023-02-23 09:58:20.000000 espm-0.1.4/espm/models/absorption_edxs.py
--rw-r--r--   0 nati       (501) staff       (20)     5600 2023-02-23 09:58:20.000000 espm-0.1.4/espm/models/base.py
--rw-r--r--   0 nati       (501) staff       (20)    15257 2023-02-23 09:58:20.000000 espm-0.1.4/espm/models/edxs.py
--rw-r--r--   0 nati       (501) staff       (20)     3130 2023-02-23 09:58:20.000000 espm-0.1.4/espm/spectrum_fitting.py
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-02-23 15:09:09.355830 espm-0.1.4/espm/tables/
--rw-r--r--   0 nati       (501) staff       (20)   299008 2023-02-21 16:38:50.000000 espm-0.1.4/espm/tables/100keV_xrays.json
--rw-r--r--   0 nati       (501) staff       (20)   288577 2023-02-21 16:38:50.000000 espm-0.1.4/espm/tables/200keV_xrays.json
--rw-r--r--   0 nati       (501) staff       (20)   282569 2023-02-21 16:38:50.000000 espm-0.1.4/espm/tables/300keV_xrays.json
--rw-r--r--   0 nati       (501) staff       (20)     6242 2023-02-21 16:38:50.000000 espm-0.1.4/espm/tables/SDD_efficiency.txt
--rw-r--r--   0 nati       (501) staff       (20)        0 2023-02-21 16:38:50.000000 espm-0.1.4/espm/tables/__init__.py
--rw-r--r--   0 nati       (501) staff       (20)   166571 2023-02-21 16:38:50.000000 espm-0.1.4/espm/tables/default_xrays.json
--rw-r--r--   0 nati       (501) staff       (20)    11811 2023-02-21 16:38:50.000000 espm-0.1.4/espm/tables/periodic_table_number.json
--rw-r--r--   0 nati       (501) staff       (20)    11616 2023-02-21 16:38:50.000000 espm-0.1.4/espm/tables/periodic_table_symbols.json
--rw-r--r--   0 nati       (501) staff       (20)      779 2023-02-21 16:38:50.000000 espm-0.1.4/espm/tables/siegbahn_to_iupac.json
--rw-r--r--   0 nati       (501) staff       (20)     4584 2023-02-23 09:58:20.000000 espm-0.1.4/espm/tables_utils.py
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-02-23 15:09:09.356991 espm-0.1.4/espm/tests/
--rw-r--r--   0 nati       (501) staff       (20)        0 2023-02-21 16:38:50.000000 espm-0.1.4/espm/tests/__init__.py
--rw-r--r--   0 nati       (501) staff       (20)     5003 2023-02-23 09:58:20.000000 espm-0.1.4/espm/tests/test_EDXS.py
--rw-r--r--   0 nati       (501) staff       (20)    10007 2023-02-23 09:58:20.000000 espm-0.1.4/espm/tests/test_datasets.py
--rw-r--r--   0 nati       (501) staff       (20)     1073 2023-02-23 09:58:20.000000 espm-0.1.4/espm/tests/test_docstring.py
--rw-r--r--   0 nati       (501) staff       (20)    10438 2023-02-23 09:58:20.000000 espm-0.1.4/espm/tests/test_estimators.py
--rw-r--r--   0 nati       (501) staff       (20)     1263 2023-02-23 09:58:20.000000 espm-0.1.4/espm/tests/test_laplacian.py
--rw-r--r--   0 nati       (501) staff       (20)     7634 2023-02-23 09:58:20.000000 espm-0.1.4/espm/tests/test_measures.py
--rw-r--r--   0 nati       (501) staff       (20)    29130 2023-02-23 09:58:20.000000 espm-0.1.4/espm/tests/test_updates.py
--rw-r--r--   0 nati       (501) staff       (20)     3652 2023-02-23 09:58:20.000000 espm-0.1.4/espm/tests/test_utils.py
--rw-r--r--   0 nati       (501) staff       (20)    11653 2023-02-23 14:13:29.000000 espm-0.1.4/espm/utils.py
--rw-r--r--   0 nati       (501) staff       (20)     3536 2023-02-23 13:21:05.000000 espm-0.1.4/espm/weights.py
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-02-23 15:09:09.347685 espm-0.1.4/espm.egg-info/
--rw-r--r--   0 nati       (501) staff       (20)     3867 2023-02-23 15:09:09.000000 espm-0.1.4/espm.egg-info/PKG-INFO
--rw-r--r--   0 nati       (501) staff       (20)     3305 2023-02-23 15:09:09.000000 espm-0.1.4/espm.egg-info/SOURCES.txt
--rw-r--r--   0 nati       (501) staff       (20)        1 2023-02-23 15:09:09.000000 espm-0.1.4/espm.egg-info/dependency_links.txt
--rw-r--r--   0 nati       (501) staff       (20)       34 2023-02-23 15:09:09.000000 espm-0.1.4/espm.egg-info/entry_points.txt
--rw-r--r--   0 nati       (501) staff       (20)        1 2023-02-23 15:09:09.000000 espm-0.1.4/espm.egg-info/not-zip-safe
--rw-r--r--   0 nati       (501) staff       (20)      207 2023-02-23 15:09:09.000000 espm-0.1.4/espm.egg-info/requires.txt
--rw-r--r--   0 nati       (501) staff       (20)        5 2023-02-23 15:09:09.000000 espm-0.1.4/espm.egg-info/top_level.txt
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-02-23 15:09:09.360170 espm-0.1.4/experiments/
--rw-r--r--   0 nati       (501) staff       (20)      763 2023-02-23 09:58:20.000000 espm-0.1.4/experiments/HPC_batch_experiment.py
--rw-r--r--   0 nati       (501) staff       (20)      833 2023-02-23 09:58:20.000000 espm-0.1.4/experiments/HPC_single_experiment.py
--rw-r--r--   0 nati       (501) staff       (20)     2549 2023-02-23 09:58:20.000000 espm-0.1.4/experiments/ICA_script.py
--rw-r--r--   0 nati       (501) staff       (20)     2705 2023-02-23 09:58:20.000000 espm-0.1.4/experiments/NMF_script.py
--rw-r--r--   0 nati       (501) staff       (20)     4963 2023-02-23 09:58:20.000000 espm-0.1.4/experiments/VCA.py
--rw-r--r--   0 nati       (501) staff       (20)     2240 2023-02-23 09:58:20.000000 espm-0.1.4/experiments/VCA_script.py
--rw-r--r--   0 nati       (501) staff       (20)     2796 2023-02-23 09:58:20.000000 espm-0.1.4/experiments/complex_data_paper.py
--rw-r--r--   0 nati       (501) staff       (20)     4291 2023-02-23 09:58:20.000000 espm-0.1.4/experiments/conf.py
--rw-r--r--   0 nati       (501) staff       (20)     4311 2023-02-23 09:58:20.000000 espm-0.1.4/experiments/data_paper.py
--rw-r--r--   0 nati       (501) staff       (20)    10377 2023-02-23 09:58:20.000000 espm-0.1.4/experiments/experiments.py
--rw-r--r--   0 nati       (501) staff       (20)      104 2023-02-21 16:38:50.000000 espm-0.1.4/experiments/generate_synthetic_dataset.py
--rwxr-xr-x   0 nati       (501) staff       (20)    17083 2023-02-23 09:58:20.000000 espm-0.1.4/experiments/mcrllm.py
--rw-r--r--   0 nati       (501) staff       (20)     2149 2023-02-23 09:58:20.000000 espm-0.1.4/experiments/mcrllm_batch.py
--rw-r--r--   0 nati       (501) staff       (20)      711 2023-02-23 09:58:20.000000 espm-0.1.4/experiments/mcrllm_script.py
--rw-r--r--   0 nati       (501) staff       (20)     1105 2023-02-23 09:58:20.000000 espm-0.1.4/experiments/mcrllm_wrapper.py
--rw-r--r--   0 nati       (501) staff       (20)      910 2023-02-23 09:58:20.000000 espm-0.1.4/experiments/quick_NMF_script.py
--rw-r--r--   0 nati       (501) staff       (20)    13889 2023-02-23 09:58:20.000000 espm-0.1.4/experiments/sunsal.py
--rw-r--r--   0 nati       (501) staff       (20)     6086 2023-02-23 09:58:20.000000 espm-0.1.4/experiments/test_experiments.py
--rwxr-xr-x   0 nati       (501) staff       (20)      139 2023-02-21 16:38:50.000000 espm-0.1.4/hyperspy_extension.yaml
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-02-23 15:09:09.363107 espm-0.1.4/notebooks/
--rw-r--r--   0 nati       (501) staff       (20)     4963 2023-02-23 09:58:20.000000 espm-0.1.4/notebooks/VCA.py
--rw-r--r--   0 nati       (501) staff       (20)     5497 2023-02-23 15:09:07.000000 espm-0.1.4/notebooks/api.ipynb
--rw-r--r--   0 nati       (501) staff       (20)    17775 2023-02-23 15:09:07.000000 espm-0.1.4/notebooks/background_fit.ipynb
--rw-r--r--   0 nati       (501) staff       (20)    13661 2023-02-23 15:09:07.000000 espm-0.1.4/notebooks/convergence-speed.ipynb
--rw-r--r--   0 nati       (501) staff       (20)     9110 2023-02-23 15:09:07.000000 espm-0.1.4/notebooks/generate_data.ipynb
--rw-r--r--   0 nati       (501) staff       (20)     2189 2023-02-23 15:09:07.000000 espm-0.1.4/notebooks/make-plots.ipynb
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-02-23 15:09:09.364930 espm-0.1.4/notebooks/old/
--rw-r--r--   0 nati       (501) staff       (20)   147612 2021-12-06 12:41:07.000000 espm-0.1.4/notebooks/old/AT_testing.ipynb
--rw-r--r--   0 nati       (501) staff       (20)     6289 2022-02-25 16:24:57.000000 espm-0.1.4/notebooks/old/algo-with-negative-variable.ipynb
--rw-r--r--   0 nati       (501) staff       (20)     8904 2021-07-13 12:59:52.000000 espm-0.1.4/notebooks/old/analyse_one_method.ipynb
--rw-r--r--   0 nati       (501) staff       (20)    20377 2021-03-23 20:35:55.000000 espm-0.1.4/notebooks/old/analyze_data.ipynb
--rw-r--r--   0 nati       (501) staff       (20)    15972 2021-03-23 20:35:55.000000 espm-0.1.4/notebooks/old/analyze_data_v2.ipynb
--rw-r--r--   0 nati       (501) staff       (20)    14011 2021-07-13 12:59:52.000000 espm-0.1.4/notebooks/old/bremstrahlung.ipynb
--rw-r--r--   0 nati       (501) staff       (20)     1878 2021-07-06 13:02:57.000000 espm-0.1.4/notebooks/old/dicho_test.ipynb
--rw-r--r--   0 nati       (501) staff       (20)    10348 2021-03-23 20:35:55.000000 espm-0.1.4/notebooks/old/generate_artificial_data.ipynb
--rw-r--r--   0 nati       (501) staff       (20)    20324 2021-05-06 13:47:57.000000 espm-0.1.4/notebooks/old/spectrum_fit.ipynb
--rw-r--r--   0 nati       (501) staff       (20)     6476 2021-07-06 13:02:57.000000 espm-0.1.4/notebooks/old/speedtest.ipynb
--rw-r--r--   0 nati       (501) staff       (20)     6820 2023-02-23 15:09:08.000000 espm-0.1.4/notebooks/other_algorithms.ipynb
--rw-r--r--   0 nati       (501) staff       (20)    17002 2023-02-23 15:09:08.000000 espm-0.1.4/notebooks/preprocess_dataset.ipynb
--rw-r--r--   0 nati       (501) staff       (20)   592095 2023-02-21 16:38:50.000000 espm-0.1.4/notebooks/read_HPC_data _TEMP.ipynb
--rw-r--r--   0 nati       (501) staff       (20)    11905 2023-02-23 15:09:08.000000 espm-0.1.4/notebooks/read_HPC_data.ipynb
--rw-r--r--   0 nati       (501) staff       (20)     4531 2023-02-23 15:09:08.000000 espm-0.1.4/notebooks/select_spectrum.ipynb
--rw-r--r--   0 nati       (501) staff       (20)    14791 2023-02-23 15:09:08.000000 espm-0.1.4/notebooks/simple-test-regularisation.ipynb
--rw-r--r--   0 nati       (501) staff       (20)    31459 2023-02-23 15:09:08.000000 espm-0.1.4/notebooks/spectrum_fit.ipynb
--rw-r--r--   0 nati       (501) staff       (20)    13889 2023-02-23 09:58:20.000000 espm-0.1.4/notebooks/sunsal.py
--rw-r--r--   0 nati       (501) staff       (20)     7554 2023-02-23 15:09:08.000000 espm-0.1.4/notebooks/surrogate-vs-bregmann.ipynb
--rw-r--r--   0 nati       (501) staff       (20)    17972 2023-02-23 15:09:08.000000 espm-0.1.4/notebooks/toy-ML.ipynb
--rw-r--r--   0 nati       (501) staff       (20)      178 2022-12-06 17:40:13.000000 espm-0.1.4/readthedoc.yml
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-02-23 15:09:09.365046 espm-0.1.4/scripts/
--rw-r--r--   0 nati       (501) staff       (20)        0 2021-07-26 13:02:08.000000 espm-0.1.4/scripts/toy_experiment.py
--rw-r--r--   0 nati       (501) staff       (20)       38 2023-02-23 15:09:09.365428 espm-0.1.4/setup.cfg
--rw-r--r--   0 nati       (501) staff       (20)     1800 2023-02-23 15:07:01.000000 espm-0.1.4/setup.py
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.807454 espm-0.2.0/
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.792374 espm-0.2.0/.github/
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.795137 espm-0.2.0/.github/workflows/
+-rw-r--r--   0 nati       (501) staff       (20)     1119 2023-02-23 15:04:13.000000 espm-0.2.0/.github/workflows/python.yml
+-rw-r--r--   0 nati       (501) staff       (20)      178 2023-02-21 16:38:53.000000 espm-0.2.0/.readthedocs.yml
+-rw-r--r--   0 nati       (501) staff       (20)      583 2023-04-20 13:32:32.000000 espm-0.2.0/CHANGELOG.rst
+-rw-r--r--   0 nati       (501) staff       (20)     3993 2023-02-22 09:05:19.000000 espm-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 nati       (501) staff       (20)     1083 2022-12-06 13:16:22.000000 espm-0.2.0/Licence.txt
+-rw-r--r--   0 nati       (501) staff       (20)      372 2023-04-18 07:43:05.000000 espm-0.2.0/MANIFEST.in
+-rw-r--r--   0 nati       (501) staff       (20)     2804 2023-04-20 14:38:31.807301 espm-0.2.0/PKG-INFO
+-rw-r--r--   0 nati       (501) staff       (20)     1767 2023-04-20 13:26:45.000000 espm-0.2.0/README.rst
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.795785 espm-0.2.0/doc/
+-rw-r--r--   0 nati       (501) staff       (20)       30 2020-12-17 09:02:04.000000 espm-0.2.0/doc/changelog.rst
+-rw-r--r--   0 nati       (501) staff       (20)     1994 2023-02-23 09:58:20.000000 espm-0.2.0/doc/conf.py
+-rw-r--r--   0 nati       (501) staff       (20)       33 2019-04-30 16:36:26.000000 espm-0.2.0/doc/contributing.rst
+-rw-r--r--   0 nati       (501) staff       (20)      213 2023-02-23 09:10:02.000000 espm-0.2.0/doc/index.rst
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.795923 espm-0.2.0/doc/introduction/
+-rw-r--r--   0 nati       (501) staff       (20)     4486 2023-04-20 12:54:03.000000 espm-0.2.0/doc/introduction/index.rst
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.797084 espm-0.2.0/doc/reference/
+-rw-r--r--   0 nati       (501) staff       (20)      220 2023-04-20 12:35:31.000000 espm-0.2.0/doc/reference/datasets.rst
+-rw-r--r--   0 nati       (501) staff       (20)      202 2023-02-21 16:38:50.000000 espm-0.2.0/doc/reference/estimators.rst
+-rw-r--r--   0 nati       (501) staff       (20)      156 2023-04-20 12:35:31.000000 espm-0.2.0/doc/reference/index.rst
+-rw-r--r--   0 nati       (501) staff       (20)       58 2023-02-21 16:38:50.000000 espm-0.2.0/doc/reference/measures.rst
+-rw-r--r--   0 nati       (501) staff       (20)      257 2023-04-20 12:35:31.000000 espm-0.2.0/doc/reference/models.rst
+-rw-r--r--   0 nati       (501) staff       (20)       70 2023-04-20 12:35:31.000000 espm-0.2.0/doc/reference/table_utils.rst
+-rw-r--r--   0 nati       (501) staff       (20)       45 2023-02-21 16:38:50.000000 espm-0.2.0/doc/reference/utils.rst
+-rw-r--r--   0 nati       (501) staff       (20)      140 2023-04-20 12:35:31.000000 espm-0.2.0/doc/reference/weights.rst
+-rw-r--r--   0 nati       (501) staff       (20)       95 2019-04-30 16:36:26.000000 espm-0.2.0/doc/references.rst
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.797235 espm-0.2.0/doc/styles/
+-rw-r--r--   0 nati       (501) staff       (20)      332 2023-02-20 15:43:46.000000 espm-0.2.0/doc/styles/sg_gallery.css
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.798332 espm-0.2.0/espm/
+-rw-r--r--   0 nati       (501) staff       (20)       21 2023-04-20 13:29:50.000000 espm-0.2.0/espm/__init__.py
+-rw-r--r--   0 nati       (501) staff       (20)     1385 2023-04-20 12:35:31.000000 espm-0.2.0/espm/conf.py
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.799758 espm-0.2.0/espm/datasets/
+-rw-r--r--   0 nati       (501) staff       (20)     1026 2023-04-20 12:35:31.000000 espm-0.2.0/espm/datasets/__init__.py
+-rw-r--r--   0 nati       (501) staff       (20)     9637 2023-04-20 13:46:14.000000 espm-0.2.0/espm/datasets/base.py
+-rw-r--r--   0 nati       (501) staff       (20)     5738 2023-04-20 12:53:51.000000 espm-0.2.0/espm/datasets/built_in_EDXS_datasets.py
+-rw-r--r--   0 nati       (501) staff       (20)    17812 2023-04-20 12:53:51.000000 espm-0.2.0/espm/datasets/eds_spim.py
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.800038 espm-0.2.0/espm/datasets/toy-problem/
+-rw-r--r--   0 nati       (501) staff       (20)     4316 2023-02-21 16:38:50.000000 espm-0.2.0/espm/datasets/toy-problem/phase1.png
+-rw-r--r--   0 nati       (501) staff       (20)     6798 2023-02-21 16:38:50.000000 espm-0.2.0/espm/datasets/toy-problem/phase2.png
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.800972 espm-0.2.0/espm/estimators/
+-rw-r--r--   0 nati       (501) staff       (20)      529 2023-02-23 09:58:20.000000 espm-0.2.0/espm/estimators/__init__.py
+-rw-r--r--   0 nati       (501) staff       (20)    19415 2023-02-23 13:48:32.000000 espm-0.2.0/espm/estimators/base.py
+-rw-r--r--   0 nati       (501) staff       (20)     6026 2023-02-23 09:58:20.000000 espm-0.2.0/espm/estimators/dicotomy.py
+-rw-r--r--   0 nati       (501) staff       (20)    10252 2023-02-23 14:37:13.000000 espm-0.2.0/espm/estimators/smooth_nmf.py
+-rw-r--r--   0 nati       (501) staff       (20)     5700 2023-02-23 09:58:20.000000 espm-0.2.0/espm/estimators/surrogates.py
+-rw-r--r--   0 nati       (501) staff       (20)    11222 2023-02-23 09:58:20.000000 espm-0.2.0/espm/estimators/updates.py
+-rwxr-xr-x   0 nati       (501) staff       (20)      143 2023-04-18 07:43:05.000000 espm-0.2.0/espm/hyperspy_extension.yaml
+-rw-r--r--   0 nati       (501) staff       (20)    20639 2023-04-20 13:24:00.000000 espm-0.2.0/espm/measures.py
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.801816 espm-0.2.0/espm/models/
+-rw-r--r--   0 nati       (501) staff       (20)    13015 2023-04-20 12:35:31.000000 espm-0.2.0/espm/models/EDXS_function.py
+-rw-r--r--   0 nati       (501) staff       (20)      500 2023-04-20 12:35:31.000000 espm-0.2.0/espm/models/__init__.py
+-rw-r--r--   0 nati       (501) staff       (20)    10090 2023-04-20 12:35:31.000000 espm-0.2.0/espm/models/absorption_edxs.py
+-rw-r--r--   0 nati       (501) staff       (20)     5682 2023-04-20 13:36:07.000000 espm-0.2.0/espm/models/base.py
+-rw-r--r--   0 nati       (501) staff       (20)    17112 2023-04-20 12:53:51.000000 espm-0.2.0/espm/models/edxs.py
+-rw-r--r--   0 nati       (501) staff       (20)     6598 2023-04-20 13:17:58.000000 espm-0.2.0/espm/models/generate_EDXS_phases.py
+-rw-r--r--   0 nati       (501) staff       (20)     3130 2023-02-23 09:58:20.000000 espm-0.2.0/espm/spectrum_fitting.py
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.803629 espm-0.2.0/espm/tables/
+-rw-r--r--   0 nati       (501) staff       (20)   299008 2023-02-21 16:38:50.000000 espm-0.2.0/espm/tables/100keV_xrays.json
+-rw-r--r--   0 nati       (501) staff       (20)   288577 2023-02-21 16:38:50.000000 espm-0.2.0/espm/tables/200keV_xrays.json
+-rw-r--r--   0 nati       (501) staff       (20)   282569 2023-02-21 16:38:50.000000 espm-0.2.0/espm/tables/300keV_xrays.json
+-rw-r--r--   0 nati       (501) staff       (20)     6242 2023-02-21 16:38:50.000000 espm-0.2.0/espm/tables/SDD_efficiency.txt
+-rw-r--r--   0 nati       (501) staff       (20)        0 2023-02-21 16:38:50.000000 espm-0.2.0/espm/tables/__init__.py
+-rw-r--r--   0 nati       (501) staff       (20)   166571 2023-02-21 16:38:50.000000 espm-0.2.0/espm/tables/default_xrays.json
+-rw-r--r--   0 nati       (501) staff       (20)    11811 2023-02-21 16:38:50.000000 espm-0.2.0/espm/tables/periodic_table_number.json
+-rw-r--r--   0 nati       (501) staff       (20)    11616 2023-02-21 16:38:50.000000 espm-0.2.0/espm/tables/periodic_table_symbols.json
+-rw-r--r--   0 nati       (501) staff       (20)      779 2023-02-21 16:38:50.000000 espm-0.2.0/espm/tables/siegbahn_to_iupac.json
+-rw-r--r--   0 nati       (501) staff       (20)     7514 2023-04-20 12:53:51.000000 espm-0.2.0/espm/tables_utils.py
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.804759 espm-0.2.0/espm/tests/
+-rw-r--r--   0 nati       (501) staff       (20)        0 2023-02-21 16:38:50.000000 espm-0.2.0/espm/tests/__init__.py
+-rw-r--r--   0 nati       (501) staff       (20)     4910 2023-04-18 07:43:05.000000 espm-0.2.0/espm/tests/test_EDXS.py
+-rw-r--r--   0 nati       (501) staff       (20)    11339 2023-04-18 07:43:05.000000 espm-0.2.0/espm/tests/test_datasets.py
+-rw-r--r--   0 nati       (501) staff       (20)     1073 2023-02-23 09:58:20.000000 espm-0.2.0/espm/tests/test_docstring.py
+-rw-r--r--   0 nati       (501) staff       (20)     9587 2023-04-18 07:43:05.000000 espm-0.2.0/espm/tests/test_estimators.py
+-rw-r--r--   0 nati       (501) staff       (20)     1263 2023-02-23 09:58:20.000000 espm-0.2.0/espm/tests/test_laplacian.py
+-rw-r--r--   0 nati       (501) staff       (20)     7634 2023-02-23 09:58:20.000000 espm-0.2.0/espm/tests/test_measures.py
+-rw-r--r--   0 nati       (501) staff       (20)    29130 2023-02-23 09:58:20.000000 espm-0.2.0/espm/tests/test_updates.py
+-rw-r--r--   0 nati       (501) staff       (20)     3652 2023-02-23 09:58:20.000000 espm-0.2.0/espm/tests/test_utils.py
+-rw-r--r--   0 nati       (501) staff       (20)    11669 2023-04-20 12:53:51.000000 espm-0.2.0/espm/utils.py
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.805166 espm-0.2.0/espm/weights/
+-rw-r--r--   0 nati       (501) staff       (20)      258 2023-04-20 12:53:51.000000 espm-0.2.0/espm/weights/__init__.py
+-rw-r--r--   0 nati       (501) staff       (20)    16957 2023-04-20 13:14:42.000000 espm-0.2.0/espm/weights/abundance.py
+-rw-r--r--   0 nati       (501) staff       (20)    11055 2023-04-20 12:53:51.000000 espm-0.2.0/espm/weights/generate_weights.py
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.799248 espm-0.2.0/espm.egg-info/
+-rw-r--r--   0 nati       (501) staff       (20)     2804 2023-04-20 14:38:31.000000 espm-0.2.0/espm.egg-info/PKG-INFO
+-rw-r--r--   0 nati       (501) staff       (20)     2441 2023-04-20 14:38:31.000000 espm-0.2.0/espm.egg-info/SOURCES.txt
+-rw-r--r--   0 nati       (501) staff       (20)        1 2023-04-20 14:38:31.000000 espm-0.2.0/espm.egg-info/dependency_links.txt
+-rw-r--r--   0 nati       (501) staff       (20)       34 2023-04-20 14:38:31.000000 espm-0.2.0/espm.egg-info/entry_points.txt
+-rw-r--r--   0 nati       (501) staff       (20)        1 2023-04-20 14:38:31.000000 espm-0.2.0/espm.egg-info/not-zip-safe
+-rw-r--r--   0 nati       (501) staff       (20)      207 2023-04-20 14:38:31.000000 espm-0.2.0/espm.egg-info/requires.txt
+-rw-r--r--   0 nati       (501) staff       (20)        5 2023-04-20 14:38:31.000000 espm-0.2.0/espm.egg-info/top_level.txt
+-rwxr-xr-x   0 nati       (501) staff       (20)      143 2023-04-18 07:43:05.000000 espm-0.2.0/hyperspy_extension.yaml
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.806980 espm-0.2.0/notebooks/
+-rw-r--r--   0 nati       (501) staff       (20)     4963 2023-02-23 09:58:20.000000 espm-0.2.0/notebooks/VCA.py
+-rw-r--r--   0 nati       (501) staff       (20)     5381 2023-04-20 14:38:30.000000 espm-0.2.0/notebooks/api.ipynb
+-rw-r--r--   0 nati       (501) staff       (20)    17775 2023-04-20 14:38:30.000000 espm-0.2.0/notebooks/background_fit.ipynb
+-rw-r--r--   0 nati       (501) staff       (20)    13661 2023-04-20 14:38:30.000000 espm-0.2.0/notebooks/convergence-speed.ipynb
+-rw-r--r--   0 nati       (501) staff       (20)     8875 2023-04-20 14:38:30.000000 espm-0.2.0/notebooks/generate_data.ipynb
+-rw-r--r--   0 nati       (501) staff       (20)     3204 2023-04-20 14:38:30.000000 espm-0.2.0/notebooks/make-plots.ipynb
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.807119 espm-0.2.0/notebooks/old/
+-rw-r--r--   0 nati       (501) staff       (20)     6289 2022-02-25 16:24:57.000000 espm-0.2.0/notebooks/old/algo-with-negative-variable.ipynb
+-rw-r--r--   0 nati       (501) staff       (20)     6820 2023-04-20 14:38:30.000000 espm-0.2.0/notebooks/other_algorithms.ipynb
+-rw-r--r--   0 nati       (501) staff       (20)    17002 2023-04-20 14:38:30.000000 espm-0.2.0/notebooks/preprocess_dataset.ipynb
+-rw-r--r--   0 nati       (501) staff       (20)     4531 2023-04-20 14:38:30.000000 espm-0.2.0/notebooks/select_spectrum.ipynb
+-rw-r--r--   0 nati       (501) staff       (20)    14791 2023-04-20 14:38:31.000000 espm-0.2.0/notebooks/simple-test-regularisation.ipynb
+-rw-r--r--   0 nati       (501) staff       (20)    31459 2023-04-20 14:38:31.000000 espm-0.2.0/notebooks/spectrum_fit.ipynb
+-rw-r--r--   0 nati       (501) staff       (20)    13889 2023-02-23 09:58:20.000000 espm-0.2.0/notebooks/sunsal.py
+-rw-r--r--   0 nati       (501) staff       (20)     7554 2023-04-20 14:38:31.000000 espm-0.2.0/notebooks/surrogate-vs-bregmann.ipynb
+-rw-r--r--   0 nati       (501) staff       (20)    18735 2023-04-20 14:38:31.000000 espm-0.2.0/notebooks/toy-ML.ipynb
+-rw-r--r--   0 nati       (501) staff       (20)      178 2022-12-06 17:40:13.000000 espm-0.2.0/readthedoc.yml
+-rw-r--r--   0 nati       (501) staff       (20)       38 2023-04-20 14:38:31.807492 espm-0.2.0/setup.cfg
+-rw-r--r--   0 nati       (501) staff       (20)     1800 2023-04-20 13:28:26.000000 espm-0.2.0/setup.py
+-rw-r--r--   0 nati       (501) staff       (20)     1120 2023-04-20 13:27:14.000000 espm-0.2.0/todo.md
```

### Comparing `espm-0.1.4/.github/workflows/python.yml` & `espm-0.2.0/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/CONTRIBUTING.rst` & `espm-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/Licence.txt` & `espm-0.2.0/Licence.txt`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/doc/conf.py` & `espm-0.2.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/doc/introduction/index.rst` & `espm-0.2.0/doc/introduction/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -42,32 +42,31 @@
 >>> ds.generate_built_in_datasets(base_path="generated_samples", seeds_range=1)
 
 Here the object `spim` is of the :class:`hyperspy._signals.signal1d.Signal1D`.
 This object has different useful attributes and methods. For example, 
 @ADRIEN --- summarize here some of them
 
 .. note::
-    Please see the review article `espm : a Python library for the simulation 
-    of STEM-EDXS datasets` for an overview of
+    Please see the review article :cite:p:`teurtrie2023espm`. 
+    `espm : a Python library for the simulation of STEM-EDXS datasets` for an overview of
     the simulation methods this package leverages.
 
-
 Factorization
 -------------
 
 Taking the non-negative matrix factorization (NMF) is done with the following:
 
 .. plot::
     :context: close-figs
     
     >>> out = spim.decomposition(3)
     >>> spim.plot_decomposition_loadings(3)
     >>> spim.plot_decomposition_factors(3)
 
-BIt will use the algorithms developped in this `contribution`_.
+It will use the algorithms developped in this `contribution`_.
 
 .. _contribution: https://link-to-the-paper.com
 
 These algorithms are an important part of this package. They are specialized to solve regularized Poisson NMF problems. Mathematically, they can be expressed as:
 
 .. math::
```

### Comparing `espm-0.1.4/espm/conf.py` & `espm-0.2.0/espm/conf.py`

 * *Files 27% similar despite different names*

```diff
@@ -19,54 +19,40 @@
 DATASETS_PATH = BASE_PATH.parent / Path("generated_datasets")
 # Ensure that the folder DATASETS_PATH exists
 DATASETS_PATH.mkdir(exist_ok=True, parents=True)
 
 
 HSPY_MAC = macs.ffast_mac # Tabulated absorption coefficient in Hyperspy
 
-DEFAULT_EDXS_PARAMS = {
-    "Det" : DEFAULT_SDD_EFF,
-    "Abs" : {
-            "thickness" : 100.0e-7,
-            "toa" : 22,
-            "density" : None,
-            "atomic_fraction" : False
-    }
+DEFAULT_MISC_PARAMS = {
+    "data_folder" : "default_synth_data",
+    "shape_2d" : (80,80),
+    "N" : 100,
+    "densities" : [2.33,19.3],
+    "model" : "EDXS",
+    "seed" : 0
 }
 
-DEFAULT_PHASE_PARAMS = [{"b0" : 1e-9 , "b1" : 1e-7, "elements_dict" :  {"14": 1.0},"scale" : 1.0},{"b0" : 7e-8 , "b1" : 3e-8, "elements_dict" :  {"79": 1.0},"scale" : 0.5}]
-
-DEFAULT_SYNTHETIC_DATA_DICT = {
-    "data_folder" : "default_synth_data",
-    "model_parameters" : {
+DEFAULT_EDXS_PARAMS = {
     "e_offset" : 0.200,
     "e_size" : 1980,
     "e_scale" : 0.01,
     "width_slope" : 0.01,
     "width_intercept" : 0.065,
-    "db_name" : "default_xrays.json",
+    "db_name" : "200keV_xrays.json",
     "E0" : 200,
     "params_dict" : {
+        "Det" : DEFAULT_SDD_EFF,
         "Abs" : {
             "thickness" : 100.0e-7,
             "toa" : 22,
             "density" : None,
             "atomic_fraction" : False
-            },
-    "Det" : DEFAULT_SDD_EFF,
-        }
-    },
-    "phases_parameters" : DEFAULT_PHASE_PARAMS,
-    "shape_2d" : (80,80),
-    "weight_type" : "sphere",
-    "weights_params" : {"radius" : 2.0},
-    "N" : 100,
-    "densities" : [2.33,19.3],
-    "model" : "EDXS",
-    "seed" : 0
+            }
+    }
 }
 
 log_shift = 1e-14
 dicotomy_tol = 1e-5
 seed_max = 4294967295
 sigmaL = 8
 maxit_dichotomy = 100
```

### Comparing `espm-0.1.4/espm/datasets/toy-problem/phase1.png` & `espm-0.2.0/espm/datasets/toy-problem/phase1.png`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/espm/datasets/toy-problem/phase2.png` & `espm-0.2.0/espm/datasets/toy-problem/phase2.png`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/espm/estimators/__init__.py` & `espm-0.2.0/espm/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/espm/estimators/base.py` & `espm-0.2.0/espm/estimators/base.py`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/espm/estimators/dicotomy.py` & `espm-0.2.0/espm/estimators/dicotomy.py`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/espm/estimators/smooth_nmf.py` & `espm-0.2.0/espm/estimators/smooth_nmf.py`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/espm/estimators/surrogates.py` & `espm-0.2.0/espm/estimators/surrogates.py`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/espm/estimators/updates.py` & `espm-0.2.0/espm/estimators/updates.py`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/espm/measures.py` & `espm-0.2.0/espm/measures.py`

 * *Files 3% similar despite different names*

```diff
@@ -215,15 +215,27 @@
 #         mins.append(np.min(vec))
 #         ind_min = np.argmin(vec)
 #         ind_mins.append(ind_min)
 #         matr[:,ind_min] = np.inf * np.ones(matr.shape[0])
 
 #     return mins, ind_mins
 
-def find_min_config(true_maps,true_spectra, algo_maps, algo_spectra,angles = True) : 
+def find_min_config(true_maps,true_spectra, algo_maps, algo_spectra,angles = True) :
+    r'''
+    Determines the best match between the true and the NMF spectra and maps by finding the configuration that minimizes either the sum of angles or the sum of MSE.
+    The function returns a warning (boolean) if the MSE and the angles disagree on the best configuration.
+
+    :param np.array 2D true_maps: true maps with shape (number of phases, number of pixels)
+    :param np.array 2D true_spectra: true spectra with shape (number of phases, number of energy channels)
+    :param np.array 2D algo_maps: NMF maps with shape (number of phases, number of pixels)
+    :param np.array 2D algo_spectra: NMF spectra with shape (number of phases, number of energy channels)
+    :param boolean angles: If True, the function will minimize the sum of angles between true and NMF spectra. If False, it will minimize the sum of MSE between true and NMF maps.
+
+    :returns: list of angles, list of MSE, configuration of the best match, warning
+    ''' 
     min_MSE_config = find_min_MSE(true_maps,algo_maps,get_ind=True,unique=True)[1]
     min_angle_config = find_min_angle(true_spectra,algo_spectra,get_ind=True,unique=True)[1]
     warning = False
 
     if min_MSE_config != min_angle_config : 
         print("WARNING : angles and mse disagree there's probably an issue")
         warning = True
```

### Comparing `espm-0.1.4/espm/models/EDXS_function.py` & `espm-0.2.0/espm/models/EDXS_function.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,19 @@
 from espm.conf import SYMBOLS_PERIODIC_TABLE
 import json
 
 from espm.utils import number_to_symbol_list
     
 def gaussian(x, mu, sigma):
     r"""
-    Calculate the gaussian function.
+    Calculate the gaussian function according to the following formula:
+
+    .. math::
+
+        f(x) = \frac{1}{\sigma \sqrt{2 \pi}} e^{-\frac{(x-\mu)^2}{2 \sigma^2}}
 
     Parameters
     ----------
     x : np.array 1D
         Energy scale.
     mu : float
         Mean of the gaussian.
@@ -106,23 +110,31 @@
     Returns
     -------
     bremsstrahlung : 
         :np.array 1D: Bremsstrahlung model
 
     Notes
     -----
-    For details see Chapman et al. Journal of Microscopy, 136, pp. 179-191, (1984)
+    For details see :cite:p:`chapman1984understanding`
     """
     return b0 / x + b1 + b2 * x
     
 def lifshin_bremsstrahlung(x, b0, b1, E0 = 200):
     r"""
     Calculate the custom parametrized bremsstrahlung inspired by the model of L.Lifshin.
 
-    The model is designed to be linear and positive in b0 and b1.
+    The model is designed to have the same definition set as the original model of L.Lifshin with :math:`b_0 > 0` and :math:`b_1 > 0`.
+
+    The model is defined as follows:
+
+    .. math::
+
+        f(\varepsilon) = b_0 \frac{\varepsilon_0 - \varepsilon}{\varepsilon_0 \varepsilon} \left(1 - \frac{\varepsilon_0 - \varepsilon}{\varepsilon_0}\right) + b_1 \frac{\left( \varepsilon_0 - \varepsilon \right) ^2}{\varepsilon_0^2 \varepsilon}
+
+    where :math:`\varepsilon_0` is the energy of the incident beam, :math:`\varepsilon` is the energy of the emitted photon and :math:`b_0` and :math:`b_1` are the parameters of the model.    
     
     Parameters
     ----------
     x : 
         :np.array 1D: Energy scale.
     b0 : 
         :float: First parameter.
@@ -175,15 +187,15 @@
     Returns
     -------
     shelf : 
         :np.array 1D: SDD shelf model.
         
     Notes
     -----
-    For details see Scholze, F. and Procop, M., X-Ray Spectrom., 38: 312-321. (2009)
+    For details see :cite:p:`scholze2009modelling`
     """
     return height * erfc(x - length)
 
 def continuum_xrays(x,params_dict={},b0= 0, b1 = 0, E0 = 200,*,elements_dict = {"Si" : 1.0} ):
     r"""
     Computes the continuum X-rays, i.e. the bremsstrahlung multiplied by the absorption and the detection efficiency.
 
@@ -310,51 +322,14 @@
     with open(SYMBOLS_PERIODIC_TABLE,"r") as f : 
         SPT = json.load(f)["table"]
     for i,elt in enumerate(elements) :
         elements_dict[elt] = norm_P[i] # * SPT[elt]["atomic_mass"]
     factor =  sum(elements_dict.values())
     return {key:elements_dict[key]/factor for key in elements_dict}
 
-@number_to_symbol_list
-def print_concentrations_from_W (part_W, *, elements = []) : 
-    r"""
-    Print a report of the chemical concentrations from a fitted W.
-
-    Parameters
-    ----------
-    part_W : 
-        :np.array 2D: W matrix output from the NMF calculation. It only makes sense when the NMF decomposition if performed with G.
-    elements : 
-        :list: List of elements as atomic number or symbol.
-
-    Returns
-    -------
-    None :
-        :None: None.
-
-    Notes
-    -----
-    This function should maybe move to another part of espm.
-    """
-    norm_W = part_W / part_W.sum(axis = 0)
-    print("Concentrations report")
-    title_string = ""
-
-    for i in range(norm_W.shape[1]) : 
-        title_string += "{:>7}".format("p" + str(i))
-    print(title_string)
-    
-    for i,j in enumerate(elements) : 
-        main_string = ""
-        main_string += "{:2}".format(j) + " : "
-        for k in range(norm_W.shape[1]) :
-            main_string += "{:05.4f} ".format(norm_W[i,k])
-        print(main_string)
-
-
 def elts_dict_from_dict_list (dict_list) : 
     r"""
     Create a single dictionnary of the elemental concentration from a list of dictionnary containing chemical compositions. The new dictionnary corresponds to the average chemical composition of the list.
 
     Parameters
     ----------
     dict_list : 
@@ -379,46 +354,64 @@
     """
     unique_elts_dict = sum((Counter(x) for x in dict_list),Counter())
     sum_elts = sum(unique_elts_dict.values())
     for e in unique_elts_dict : 
         unique_elts_dict[e] /= sum_elts
     return unique_elts_dict
 
-def update_bremsstrahlung (G,part_W,model_parameters,elements_list, norm = True) : 
+def elts_list_from_dict_list (dict_list) :
+    r"""
+    Create a list of elements from a list of dictionnary containing chemical compositions. The list contains all the elements contained in the input.
+
+    Parameters
+    ----------
+    dict_list :
+        :list [dict]: list of chemical composition dictionnary
+
+    Returns
+    -------
+    elements_list :
+        :list: List of elements as atomic number or symbol.
+
+    Examples
+    --------
+    >>> import numpy as np
+    >>> from espm.models.EDXS_function import elts_list_from_dict_list
+    >>> dicts = [{"Si" : 1.0, "C" : 0.5, "O" : 0.5},{"Ca" : 1.0, "K" : 2.0},{"O" : 1.0, "Si" : 0.5},{"C" : 1.0}] 
+    >>> elts_list_from_dict_list(dicts)
+        ["Si","Ca","O","C","K"]
+    """ 
+    unique_elts_dict = sum((Counter(x) for x in dict_list),Counter())
+    return list(unique_elts_dict.keys())
+
+def update_bremsstrahlung (G,part_W,model,elements_list) : 
     r"""
     Update the continuum X-rays part of the G matrix with the current average chemical composition.
 
     Parameters
     ----------
     G : 
         :np.array 2D: EDXS modelling matrix.
     part_W : 
         :np.array 2D: Learned chemical concentrations.
-    model_parameters : 
-        :dict: Parameters of the EDXS model.
+    model : 
+        :espm.models.EDXS: EDXS model.
     elements_list :
         :list: List of elements as atomic number or symbol.
-    norm : 
-        :bool: work in progress
     
     Returns
     -------
     new_G : 
         :np.array 2D: New G matrix with updated continuum X-rays models.
 
     Notes
     -----
     This function should maybe move to another part of espm.
     """
     elts = elts_dict_from_W(part_W,elements = elements_list)
-    model = e.EDXS(**model_parameters)
     B = G_bremsstrahlung(model.x,model.E0,model.params_dict,elements_dict=elts)
     new_G = G.copy()
-    new_G[:,-2:] = B
-    if norm : 
-        norms = np.sqrt(np.sum(new_G**2, axis=0, keepdims=True))
-        norms[0][:-2] = np.mean(norms[0][:-2])
-        new_G = new_G / norms
+    new_G[:,-2:] = B/model.norm[0][-2:]
     return new_G
```

### Comparing `espm-0.1.4/espm/models/absorption_edxs.py` & `espm-0.2.0/espm/models/absorption_edxs.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     Returns
     -------
     mass-absorption coefficient
         :np.array 1D: Calculated value of the mass-absorption coefficient on all the energy range.
 
     Notes
     -----
-    The mass-absorption coefficients are calculated using the database of hyperspy
+    The mass-absorption coefficients are calculated using the database of hyperspy :cite:p:`francisco_de_la_pena_2022_7263263`.
     """
     mu = np.zeros_like(x)
     if atomic_fraction : 
         elements_dict = atomic_to_weight_dict(elements_dict = elements_dict)
 
     sum_elts = sum(elements_dict.values())
     
@@ -52,14 +52,21 @@
         mu = 1 / np.power(x,3)
 
     return mu
 
 def absorption_correction (x,thickness = 100e-7,toa = 90,density = None,atomic_fraction = False,*,elements_dict = {"Si" : 1.0},**kwargs) : 
     r"""
     Calculate the contribution of the absorption on the EDX spectrum for a thin slab of material with a given composition at a certain energy or over a certain energy range.
+    The absorption correction is calculated using the following formula :
+    
+    .. math::
+      
+        \frac{1 - \exp(-\chi)}{\chi} 
+      
+    where :math:`\chi = \mu \rho t / \sin(\theta)`, :math:`\mu` is the mass-absorption coefficient, :math:`\rho` is the density of the material, :math:`t` is the thickness of the sample and :math:`\theta` is the average take-off angle of the x-rays travelling from the sample to the x-ray detectors.
 
     Parameters
     ----------
     x :
         :np.array 1D: Energy value or energy scale over which the mass-absorption coefficient is calculated.
     thickness : 
         :float: Thickness of the material slab in meter. If the thickness is set to 0.0, the function will return 1.0.
@@ -174,15 +181,23 @@
     mu = absorption_coefficient(x,atomic_fraction,elements_dict=elements_dict)
     if density is None : 
         density = approx_density(atomic_fraction,elements_dict = elements_dict)
     return mu*thickness*density
 
 def det_efficiency (x,det_dict) :
     r"""
-    Simulate the detection efficiency of an EDX detector.
+    Simulate the detection efficiency of an EDX detector. The absorption wihtin one layer of the detector is calculated according to the following equation, corresponding to the Beer-Lambert law:
+
+    .. math::
+
+        d_k = \exp\left( - \mu(\varepsilon_k)\rho t \right)
+
+    where :math:`d_k` is the detection efficiency at the energy :math:`\varepsilon_k`, :math:`\mu(\varepsilon_k)` is the mass-absorption coefficient at the energy :math:`\varepsilon_k`, :math:`\rho` is the density of the material, and :math:`t` is the thickness of the material.
+
+    In a detection layer of the detector, an absobed photon counts as a detected photon so that the detection efficiency is equal to 1 minus the absorption. The detection efficiency is calculated as the product of the absorption of each layer of the detector.
 
     Parameters
     ----------
     x :
         :np.array 1D: Energy value or energy scale over which the mass-absorption coefficient is calculated.
     det_dict :
         :dict: See Examples for an example of the structure of the dict. One of the layer of the input dictionnary should be named "detection" to model a active layer of the detector.
```

### Comparing `espm-0.1.4/espm/models/base.py` & `espm-0.2.0/espm/models/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 r"""
-Models abstract class
----------------------
+Models base classes
+-------------------
 
-Its main purpose is to read databases and set energy parameters. 
+The PhysicalModel is the abstract class from which the EDX model inherits. 
+The ToyModel can be used for testing data analysis algorithms.
 """
 
 from abc import ABC, abstractmethod
 from pathlib import Path
 import json
 import espm.conf as conf
 import numpy as np
 from typing import Optional
 
 class Model(ABC):
-    """Abstract class for models."""
+    r"""Abstract class for models."""
     def __init__(self):
         super().__init__()
 
     @abstractmethod
     def generate_g_matr (self, g_parameters) :
         pass
 
@@ -71,15 +72,15 @@
         self.C = C
         self.K = K
         self.seed = seed
         self.G = None
         self.phases = None
     
     def generate_g_matr (self, *args, **kwargs) -> None:
-        """Generate G matrix.
+        r"""Generate G matrix.
 
         Parameters
         ----------
         args : ignored
         kwargs : ignored
 
         Returns
@@ -108,15 +109,15 @@
             inds = np.random.choice(n_el, size=[c] , replace=False)
             for ind in inds:
                 w = 0.1+0.9*np.random.rand()
                 G[:,i] += w * gauss(l, mu_gauss[ind], sigma_gauss[ind])
         self.G = G
 
     def generate_phases (self, *args, **kwargs) -> None:
-        """Generate phases.
+        r"""Generate phases.
 
         Parameters
         ----------
         args : ignored
         kwargs : ignored
 
         Returns
@@ -128,18 +129,19 @@
         if self.phases is not None :
             return
         Wdot = np.abs(np.random.laplace(size=[self.C, self.K]))
         self.Wdot = Wdot / np.mean(Wdot)/self.L
 
         self.generate_g_matr()
         self.phases = self.G @ self.Wdot
+        
     
 
 class PhysicalModel(Model) :
-    """Abstract class of the models"""
+    r"""Abstract class of the models"""
     def __init__(self, e_offset, e_size, e_scale, params_dict,db_name="default_xrays.json", E0 = 200, **kwargs) :
         super().__init__()
         self.x = self.build_energy_scale(e_offset, e_size, e_scale)
         self.params_dict = params_dict
         if db_name is None :
             self.db_dict = {}
             self.db_mdata = {}
```

### Comparing `espm-0.1.4/espm/models/edxs.py` & `espm-0.2.0/espm/models/edxs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 r"""
 EDXS model
 ----------
 
 The :mod:`espm.models.edxs` module implements the creation of the G matrix that contains a modelisation of the characteristic and continuous X-rays.
 
+**This module is a key component of the EDXS data simulation and the EDXS data analysis.**
+
 """
 
 import numpy as np
 from espm.models import PhysicalModel
 from espm.models.EDXS_function import G_bremsstrahlung, continuum_xrays, gaussian, read_lines_db, read_compact_db, update_bremsstrahlung, elts_dict_from_dict_list
 from espm.conf import DEFAULT_EDXS_PARAMS
 from espm.utils import arg_helper, symbol_to_number_dict, symbol_to_number_list
@@ -19,69 +21,89 @@
     def __init__(
         self, 
         *args, 
         width_slope=0.01,
         width_intercept=0.065,
         **kwargs
     ):
-        """
+        r"""
         :database_path: file path to a database of x-ray data (energy and intensity ratios of the peaks)
         :abs_db_path: file path to a database of attenuation coefficients (Useful for artificial data only for the moment)
         :brstlg_pars: dictionary of parameters for the continuum X-rays. Only a part of the parameters can be used without issues.
         :e_offset: energy offset of the energy axis (float)
         :e_size: number of energy channels (int)
         :e_scale: ev/channel calibration of the energy axis (float)
         :width_slope: The FWHM of the detector increases with energy which is modeled with an affine function. This is the slope of this affine function (float).
         :width_intercept: The FWHM of the detector increases with energy which is modeled with an affine function. This is the intercept of this affine function (float).
         """
         super().__init__(*args,**kwargs)
         self.width_slope = width_slope
         self.width_intercept = width_intercept
-
-        default_params = DEFAULT_EDXS_PARAMS
-        self.params_dict = arg_helper(self.params_dict,default_params)
         
         self.lines = self.db_mdata["lines"]
         self.norm = 1.0
+        self.model_elts = []
 
 
     @symbol_to_number_list
-    def generate_g_matr(self, g_type="bremsstrahlung", norm = True, reference_elt = {},*,elements=[], **kwargs):
+    def generate_g_matr(self, g_type="bremsstrahlung",reference_elt = {},*,elements=[], **kwargs):
         r"""
         Generate the G matrix. With a complete model the matrix is (e_size,n+2). The first n columns correspond to the sum of X-ray characteristic peaks associated to each shell of the elements. The last 2 columns correspond to a bremsstrahlung model. 
         
+        The first n columns of G (noted :math:`\kappa`), corresponding to the characteristic X-rays, can be calculated using the following formula:
+        
+        .. math::
+
+            \kappa_{k,Z} = \sum_{ij} x_{ij}(Z) \frac{1}{\Delta(\varepsilon_k) \sqrt{2\pi} } e{^{-\frac{1}{2} {\left( \frac{\varepsilon_k - \varepsilon^{ij}(Z)}{\Delta(\varepsilon_k)} \right)}^2}}
+        
+        where :math:`\varepsilon_k` is the energy of the kth energy channel, :math:`\varepsilon^{ij}(Z)` is the energy of the ijth line of the Zth element, :math:`\Delta(\varepsilon_k)` is the FWHM of the detector at the energy :math:`\varepsilon_k` and :math:`x_{ij}(Z)` is the intensity ratio of the ijth line of the Zth element. The last term of the equation is a gaussian function centered at :math:`\varepsilon^{ij}(Z)` and with a FWHM of :math:`\Delta(\varepsilon_k)`.
+
+        The last two columns of G (noted :math:`\beta`), corresponding to the bremsstrahlung model, can be calculated using the following formula:
+
+        .. math::
+
+            \beta_{k,n+1} = \frac{\varepsilon_0 - \varepsilon_k}{\varepsilon_0 \varepsilon_k} \times \frac{1 - (\varepsilon_0 - \varepsilon_k)}{\varepsilon_0}
+
+            \beta_{k,n+2} = \frac{(\varepsilon_0 - \varepsilon_k)^2}{\varepsilon^2_0 \varepsilon_k}
+
+        Note that there is no parameter for the bremsstrahlung since it is supposed to be learned with the W matrix (see espm.estimators).
+        
         Parameters
         ----------
         g_type : 
             :string: Options of the edxs model to include in the G matrix. The three possibilities are "identity", "no_brstlg" and "bremsstrahlung". G is going to be the identity matrix, only characteristic X-ray peaks or characteristic X-rays plus bremsstrahlung model, respectively.
-        norm : 
-            :boolean: Norms the columns of G for computation purposes. That feature will be removed, for a better solution.
         reference_elt : 
             :dict: The keys are chemical elements (atomic number) and the values are cut-off energies. This argument is used to split some of the columns of G into 2 columns. The first column corresponds to characteristic X-rays before the cut-off and second one corresponds to characteristic X-rays before the cut-off. This feature is implemented to enable more accurate absorption correction.
         elements : 
             :list: List of modeled chemical elements. The list can be populated either with atomic numbers or chemical symbols, e.g. "Fe" or 26.
 
         Returns
         -------
         g matrix :
             :np.array 2D: matrix of the edx model. 
 
         Notes
         -----
-        See our paper about the espm package for more information about the equations of this model.
+        See our paper about the espm package :cite:p:`teurtrie2023espm` for more information about the equations of this model.
         """
-        # Diagonal g_matr
+        
+        # Reset the internally stored elements list
+        self.model_elts = []
+        
         if g_type == "bremsstrahlung" : 
             self.bkgd_in_G = True
+        else : 
+            self.bkgd_in_G = False
 
+        # None is a default value for the G matrix and thus G will be considered to be the identity matrix in most of espm functions.
         if len(elements) == 0:
-            return None
+            self.G = None
 
         elif g_type == "identity" : 
-            return None
+            self.G = None
         # model based on elements_list
         elif (g_type == "bremsstrahlung") or (g_type == "no_brstlg"):
             
             # The number of shells depend on the element, it is then not straightforward to pre-determine the size of g_matr
             self.G = np.zeros((self.x.shape[0], 0))
             # For each element we unpack all shells and then unpack all lines of each shell.
             for elt in elements:
@@ -140,45 +162,49 @@
                                 * gaussian(self.x, energy, width / 2.3548)[
                                     np.newaxis
                                 ].T
                             )*D*A
                 
                 if np.max(peaks) > 0.0:
                     self.G = np.concatenate((self.G, peaks), axis=1)
+                    if str(elt) in reference_elt : 
+                        self.model_elts.append(str(elt))
+                        self.model_elts.append(str(elt))
+                    else : 
+                        self.model_elts.append(str(elt))
                 else : 
                     print("No peak is present in the energy range for element : {}".format(elt))
             
             # Appends a pure continuum spectrum is needed
             if self.bkgd_in_G:
                 approx_elts = {key : 1.0/len(elements) for key in elements}
                 brstlg_spectrum = G_bremsstrahlung(self.x,self.E0,self.params_dict,elements_dict=approx_elts)
                 if np.max(brstlg_spectrum) > 0.0 : 
                     self.G = np.concatenate((self.G, brstlg_spectrum), axis=1)
                 else : 
                     print("Bremsstrahlung parameters were not provided, bkgd not added in G")
                     self.bkgd_in_G = False
 
-            if norm : 
-                norms = np.sqrt(np.sum(self.G**2, axis=0, keepdims=True))
-                if g_type == "bremsstrahlung" : 
-                    norms[0][:-2] = np.mean(norms[0][:-2])
-                else : 
-                    norms[0] = np.mean(norms[0])
-                self.norm = norms
-                self.G /= self.norm
+            norms = np.sqrt(np.sum(self.G**2, axis=0, keepdims=True))
+            if g_type == "bremsstrahlung" : 
+                norms[0][:-2] = np.mean(norms[0][:-2])
+            else : 
+                norms[0] = np.mean(norms[0])
+            self.norm = norms
+            self.G /= self.norm
         else : 
             print("g_type has to be one of those : \"bremsstrahlung\", \"no_brstlg\" or \"identity\". G will be None, corresponding to \"identity\". ")
 
             
 
    
 
     def generate_phases(self, phases_parameters) : 
         r"""
-        Generate a series of spectra from list of phase parameters
+        Generate a series of spectra from list of phase parameters. 
 
         Parameters
         ----------
         phases_parameters : 
             :list: List of dicts containing the phase parameters.
         
         Returns
@@ -197,15 +223,15 @@
             self.phases.append(self.generate_spectrum(**p,abs_elts_dict = unique_elts))
         self.phases = np.array(self.phases)
         self.phases /= self.phases.sum(axis = 1)[:,np.newaxis]
 
     @symbol_to_number_dict
     def generate_spectrum(self, b0=0, b1 = 0, scale = 1.0,abs_elts_dict = {},*,elements_dict = {}):
         r"""
-        Generate a spectrum from bremsstrahlung parameters and a chemical composition.
+        Generate a spectrum from bremsstrahlung parameters and a chemical composition. The modelling is done using the same formula as for the generate_g_matr function.
 
         Parameters
         ----------
         b0 : 
             :float: First bremsstrahlung parameter. 
         b1 : 
             :float: Second bremsstrahlung parameter.
@@ -218,22 +244,26 @@
         Returns
         -------
         spectrum : 
             :np.array 1D: Output edx spectrum corresponding to the input chemical composition.
 
         Examples
         --------
-        >>> import matplotlib.pyplot as plt
-        >>> from espm.models.edxs import EDXS
-        >>> from espm.conf import DEFAULT_SYNTHETIC_DATA_DICT
-        >>> b0, b1 = 5.5367e-5, 0.00192181
-        >>> elts_dict = {"Si" : 1.0,"Ca" : 1.0,"O" : 3.0,"C" : 0.3}
-        >>> model = EDXS(**DEFAULT_SYNTHETIC_DATA_DICT['model_parameters'])
-        >>> spectrum = model.generate_spectrum(b0,b1, elements_dict = elts_dict)
-        >>> plt.plot(spectrum)
+
+        .. plot::
+            :context: close-figs
+
+            >>> import matplotlib.pyplot as plt
+            >>> from espm.models.edxs import EDXS
+            >>> from espm.conf import DEFAULT_EDXS_PARAMS
+            >>> b0, b1 = 5.5367e-5, 0.00192181
+            >>> elts_dict = {"Si" : 1.0,"Ca" : 1.0,"O" : 3.0,"C" : 0.3}
+            >>> model = EDXS(**DEFAULT_EDXS_PARAMS)
+            >>> spectrum = model.generate_spectrum(b0,b1, elements_dict = elts_dict)
+            >>> plt.plot(spectrum)
 
         Notes
         -----
         Check EDXS_function for details about the bremsstrahlung model.
         """
         temp = np.zeros_like(self.x)
         for elt in elements_dict.keys():
@@ -280,15 +310,15 @@
     #                     elements_dict[elt]
     #                     * cs[i]
     #                     * gaussian(self.x, energy, width / 2.3548)[:,np.newaxis]
     #                 )*((A.reshape(-1)[:,np.newaxis]).T)
     #     temp += absorption_mass_thickness(self.x, mass_thickness=mass_thickness,**self.params_dict["Abs"],elements_dict = elements_dict)
         
 
-def G_EDXS (model_params, g_params, part_W = None, G = None) : 
+def G_EDXS (model, g_params, part_W = None, G = None) : 
     r"""
     Update the bremsstrahlung part of the G matrix. This function is used for the NMF decomposition so that the absorption correction is updated in between each step.
 
     Parameters
     ----------
     model_params : 
         :dict: Parameters of the edxs model. Check espm.conf.DEFAULT_EDXS_PARAMS for an example. 
@@ -301,16 +331,15 @@
 
     Returns
     -------
     updated G : 
         :np.array 2D: Updated G matrix with a new absorption correction.
     """
     if G is None : 
-        model = EDXS(**model_params)
         model.generate_g_matr(**g_params)
         G = model.G
 
     if part_W is None : 
         return G
     else : 
-        new_G = update_bremsstrahlung(G,part_W,model_params,g_params["elements"])
+        new_G = update_bremsstrahlung(G,part_W,model,g_params["elements"])
         return new_G
```

### Comparing `espm-0.1.4/espm/spectrum_fitting.py` & `espm-0.2.0/espm/spectrum_fitting.py`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/espm/tables/100keV_xrays.json` & `espm-0.2.0/espm/tables/100keV_xrays.json`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/espm/tables/200keV_xrays.json` & `espm-0.2.0/espm/tables/200keV_xrays.json`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/espm/tables/300keV_xrays.json` & `espm-0.2.0/espm/tables/300keV_xrays.json`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/espm/tables/SDD_efficiency.txt` & `espm-0.2.0/espm/tables/SDD_efficiency.txt`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/espm/tables/default_xrays.json` & `espm-0.2.0/espm/tables/default_xrays.json`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/espm/tables/periodic_table_number.json` & `espm-0.2.0/espm/tables/periodic_table_number.json`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/espm/tables/periodic_table_symbols.json` & `espm-0.2.0/espm/tables/periodic_table_symbols.json`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/espm/tables/siegbahn_to_iupac.json` & `espm-0.2.0/espm/tables/siegbahn_to_iupac.json`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/espm/tests/test_EDXS.py` & `espm-0.2.0/espm/tests/test_EDXS.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from espm.models.absorption_edxs import det_efficiency, absorption_correction
-from espm.datasets.generate_EDXS_phases import generate_elts_dict
+from espm.models.generate_EDXS_phases import generate_elts_dict
 import numpy as np
 import espm.models.EDXS_function as ef
 from espm.models import EDXS
 from espm.models.EDXS_function import lifshin_bremsstrahlung, lifshin_bremsstrahlung_b0, lifshin_bremsstrahlung_b1
 
 x = np.linspace(0.2,19,num = 2000)
 det_dict = {
@@ -98,15 +98,15 @@
 
 def test_update_bremsstrahlung () : 
     elts_list = ["Si", "Co", "Cu","O"]
     part_P = np.ones((4,1))/4
     model = EDXS(**model_parameters)
     model.generate_g_matr(elements=elts_list)
     G = model.G
-    new_G = ef.update_bremsstrahlung(G, part_P, model_parameters, elts_list)
+    new_G = ef.update_bremsstrahlung(G, part_P, model, elts_list)
 
     assert G.shape == new_G.shape
     np.testing.assert_allclose(G[:,:-2],new_G[:,:-2])
 
 def test_generate_g_matr () : 
     model1 = EDXS(**model_parameters)
     model2 = EDXS(**model_parameters)
@@ -117,22 +117,20 @@
     G_brem = model1.G
     model2.generate_g_matr(g_type = "identity", elements = elts_list)
     G_id = model2.G
     model3.generate_g_matr(g_type = "no_brstlg", elements = elts_list)
     G_no_brstlg = model3.G
 
     assert G_brem.shape == (size, 6)
-    assert G_id.shape == (size, size)
     assert G_no_brstlg.shape == (size, 4)
 
-    np.testing.assert_allclose(G_id, np.diag(np.ones((size,))
-    ))
+    assert G_id is None
     np.testing.assert_allclose(G_brem[:,:-2], G_no_brstlg)
 
-    np.testing.assert_array_less(-1e-30, G_id)
+    # np.testing.assert_array_less(-1e-30, G_id)
     np.testing.assert_array_less(-1e-30, G_brem)
     np.testing.assert_array_less(-1e-30, G_no_brstlg)
 
 def test_G_bremsstrahlung() : 
     model = EDXS(**model_parameters)
     size = model_parameters["e_size"]
     elts_dict = {"V" : 0.3, "Ti" : 0.1, "Hf" : 0.05, "Pb" : 0.55 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `espm-0.1.4/espm/tests/test_datasets.py` & `espm-0.2.0/espm/tests/test_datasets.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,126 +1,123 @@
-from espm.datasets.spim import get_metadata
+from espm.datasets.eds_spim import get_metadata
 import numpy as np
-from espm.datasets.base import generate_dataset, generate_spim, save_generated_spim
+from espm.datasets.base import generate_dataset, generate_spim_sample, sample_to_EDS_espm, generate_spim
 from espm.models import EDXS
-from espm.datasets.generate_weights import generate_weights, random_weights, laplacian_weights, spheres_weights, gaussian_ripple_weights
-from espm.datasets.generate_EDXS_phases import generate_brem_params, generate_random_phases, unique_elts
+from espm.models.generate_EDXS_phases import generate_brem_params, generate_random_phases, unique_elts
 import os
 import hyperspy.api as hs
 import shutil
-from espm.conf import DATASETS_PATH, DEFAULT_SYNTHETIC_DATA_DICT
+from espm.conf import DATASETS_PATH
 from pathlib import Path
 from hyperspy.misc.eds.utils import take_off_angle
+import espm.weights.generate_weights as wts
+from espm.weights.generate_weights import generate_weights
+from espm.models.EDXS_function import elts_list_from_dict_list
+from espm.models.generate_EDXS_phases import generate_modular_phases
+
+elts_dicts = [{"Fe" : 0.54860348,
+               "Pt" : 0.38286879,
+               "Mo" : 0.03166235,
+               "O" : 0.03686538},
+               {"Ca" : 0.54860348,
+                "Si" : 0.38286879,
+                "O" : 0.15166235},
+                {"Cu" : 0.34,
+                 "Mo" : 0.12,
+                 "Au" : 0.54}]
+
+brstlg_pars = [{"b0" : 5e-3,
+                  "b1" : 3e-2},
+                 {"b0" : 7e-3,
+                    "b1" : 5e-2},
+                    {"b0" : 3e-3,
+                    "b1" : 5e-2}]
+
+scales = [0.05, 0.05, 0.05]
+
+model_params = {"e_offset" : 0.2,
+                "e_size" : 1900,
+                "e_scale" : 0.01,
+                "width_slope" : 0.01,
+                "width_intercept" : 0.065,
+                "db_name" : "default_xrays.json",
+                "E0" : 200,
+                "params_dict" : {
+                    "Abs" : {
+                        "thickness" : 100.0e-7,
+                        "toa" : 35,
+                        "density" : 5
+                    },
+                    "Det" : "SDD_efficiency.txt"
+                }}  
+
+misc_params = {"N" : 40,
+                "densities" : [1.3,1.6,1.9],
+                "data_folder" : "test_gen_data",
+                "seed" : 42,
+                "shape_2d" : (100,120),
+                "model" : "EDXS"}
 
-DATA_DICT = {
-    "model_parameters" : {
-        "e_offset" : 0.2,
-        "e_size" : 1900,
-        "e_scale" : 0.01,
-        "width_slope" : 0.01,
-        "width_intercept" : 0.065,
-        "db_name" : "default_xrays.json",
-        "E0" : 200,
-        "params_dict" : {
-            "Abs" : {
-                "thickness" : 100.0e-7,
-                "toa" : 35,
-                "density" : 5
-            },
-            "Det" : "SDD_efficiency.txt"
-        }
-    },
-    "N" : 40,
-    "densities" : [1.3,1.6,1.9],
-    "data_folder" : "test_gen_data",
-    "seed" : 42,
-    "weight_type" : "sphere",
-    "shape_2d" : (100,120),
-    "weights_params" : {
-        "radius" : 1.5
-    },
-    "model" : "EDXS",
-    "phases_parameters" : [{"b0" : 5e-3,
-                            "b1" : 3e-2,
-                            "scale" : 0.05,
-                            "elements_dict" : {"Fe" : 0.54860348,
-                                      "Pt" : 0.38286879,
-                                      "Mo" : 0.03166235,
-                                      "O" : 0.03686538}},
-                            {"b0" : 7e-3,
-                            "b1" : 5e-2,
-                            "scale" : 0.05,
-                            "elements_dict" : {"Ca" : 0.54860348,
-                                      "Si" : 0.38286879,
-                                      "O" : 0.15166235}},
-                            {"b0" : 3e-3,
-                            "b1" : 5e-2,
-                            "scale" : 0.05,
-                            "elements_dict" : {
-                                "Cu" : 0.34,
-                                "Mo" : 0.12,
-                                "Au" : 0.54
-                            }}]
-}
-
-MISC_DICT = {"N" : 40,
-    "densities" : [1.3,1.6,1.9],
-    "data_folder" : "test_gen_data",
-    "seed" : 42,
-    "weight_type" : "sphere",
-    "shape_2d" : (100,120),
-    "weights_params" : {
-        "radius" : 1.5
-    },
-    "model" : "EDXS"}
+elements = elts_list_from_dict_list(elts_dicts)
 
 def test_generate():
 
     # Generate the phases
-    model = EDXS(**DATA_DICT["model_parameters"])
-    model.generate_g_matr(g_type = "bremsstrahlung", elements=["Fe", "Pt", "O", "Si", "Ca", "Au", "Mo", "Cu"])
-    model.generate_phases(DATA_DICT["phases_parameters"])
-    phases1 = model.phases
+    model = EDXS(**model_params)
+    model.generate_g_matr(g_type = "bremsstrahlung", elements=elements)
+    phases1 = generate_modular_phases(elts_dicts = elts_dicts, brstlg_pars =  brstlg_pars, scales = scales, model_params = model_params)
     G = model.G
-    n_phases = len(DATA_DICT["phases_parameters"])
-    maps = generate_weights(weight_type=DATA_DICT["weight_type"], shape_2d= DATA_DICT["shape_2d"], n_phases=n_phases, seed=DATA_DICT["seed"], **DATA_DICT["weights_params"])
-    densities = np.array([1.3, 1.6, 1.9])
-    spim = generate_spim(phases1, maps, densities, DATA_DICT["N"], seed=DATA_DICT["seed"],continuous = False)
-    cont_spim = generate_spim(phases1, maps, densities, DATA_DICT["N"], seed=DATA_DICT["seed"],continuous = True)
-    Xdot = DATA_DICT["N"]* maps @ np.diag(densities)@ phases1
+    n_phases = len(elts_dicts)
+    maps = generate_weights(weight_type='sphere', shape_2d= misc_params["shape_2d"], n_phases=n_phases, seed=misc_params["seed"], radius = 15)
+    densities = np.array(misc_params["densities"])
+    spim_sample = generate_spim_sample(phases1,maps,model_params=model_params, misc_params=misc_params)
+    spim = spim_sample["X"]
+    cont_spim = spim_sample["Xdot"]
+    Xdot = misc_params["N"]* maps @ np.diag(densities)@ phases1
     W = np.abs(np.linalg.lstsq(G,spim.sum(axis = (0,1)),rcond = None)[0])
     
     assert phases1.shape == (3, 1900)
     assert maps.shape == (100,120,3)
     assert spim.shape == (100,120,1900)
     np.testing.assert_allclose(np.sum(phases1, axis=1), np.ones([3]))
     np.testing.assert_allclose( Xdot, cont_spim)
     np.testing.assert_allclose( Xdot.sum(axis=(0,1)), G@W, rtol = 0.1 )
 
+    if os.path.exists("test.hspy"):
+        os.remove("test.hspy")
     filename = "test.hspy"
-    save_generated_spim(filename, spim, DATA_DICT['N']*np.diag(densities)@phases1, maps, **DATA_DICT)
+    hspy_spim = sample_to_EDS_espm(spim_sample,elements=elements)
+    hspy_spim.save(filename)
     si = hs.load(filename)
-    si.set_signal_type("EDS_espm")
-    G = si.build_G(problem_type = "bremsstrahlung")
-    G = G()
+    si.build_G(problem_type = "bremsstrahlung")
+    G = si.G()
     phases, maps = si.phases, si.maps_2d
     # weights = weights.reshape((100,120,n_phases))
     X = si.data
     W = np.linalg.lstsq(G,X.sum(axis = (0,1)),rcond = None)[0]
     
     assert phases.shape == (1900, 3)
     assert maps.shape == (100,120,3)
     assert si.data.shape == (100,120,1900)
     np.testing.assert_allclose( Xdot, maps @ phases.T)
     np.testing.assert_allclose( Xdot.sum(axis=(0,1)), G@W, rtol = 0.2 )
 
     os.remove(filename)
 
-    generate_dataset(seeds_range=1,**DATA_DICT)
-    gen_folder = DATASETS_PATH / Path(DATA_DICT["data_folder"])
+    if os.path.exists(str(DATASETS_PATH / Path(misc_params["data_folder"]))):
+        shutil.rmtree(str(DATASETS_PATH / Path(misc_params["data_folder"])))
+    
+    generate_dataset(base_seed=misc_params['seed'],
+                    sample_number=2,
+                    model_params = model_params,
+                    misc_params = misc_params,
+                    phases = phases1,
+                    weights = maps,
+                    elements = elements)
+    gen_folder = DATASETS_PATH / Path(misc_params["data_folder"])
     gen_si = hs.load(gen_folder / Path("sample_0.hspy"))
     
     np.testing.assert_allclose(X,gen_si.data)
 
     shutil.rmtree(str(gen_folder))
     
 def test_generate_spim():
@@ -145,109 +142,137 @@
     #     X2 = np.random.poisson(N * Xdot) / N
 
     #     vals.append(np.mean(np.abs(X - Xdot)))
     #     vals2.append(np.mean(np.abs(X2 - Xdot)))
         
     # plt.plot(Ns, vals)
     # plt.plot(Ns, vals2)
-
     N = 10000
+    X3 = np.zeros([*shape_2d, ell])
+    for k, w in enumerate(densities):
+        # generating the spectroscopic events
+        for i in range(shape_2d[0]):
+            for j in range(shape_2d[1]):
+                # Draw a local_N based on the local density
+                local_N = np.random.poisson(N * w * weights[i, j, k])
+                # draw local_N events from the ideal spectrum
+                counts = np.random.choice(
+                    ell, local_N, p=phases[k]/np.sum(phases[k])
+                )
+                # Generate the spectrum based on the drawn events
+                hist = np.bincount(counts, minlength=ell)
+                X3[i, j] += hist
+
+    
     Xdot = generate_spim(phases, weights, densities, N, seed=seed,continuous = True)/N
     X = generate_spim(phases, weights, densities, N, seed=seed,continuous = False)/N
-    X2 = np.random.poisson(N * Xdot) / N
+    # X2 = np.random.poisson(N * Xdot) / N
 
+    X3 /= N
     assert ( np.mean(np.abs(X - Xdot)) < 0.005)
+    assert ( np.mean(np.abs(X3 - Xdot)) < 0.005)
+    assert ( np.mean(np.abs(X - X3)) < 0.006)
 
 
 
 def test_generate_random_weights():
     shape_2d = [28, 36]
     n_phases = 5
     
-    w = random_weights(shape_2d=shape_2d, n_phases=n_phases)
+    w = wts.random_weights(shape_2d=shape_2d, n_phases=n_phases)
     
     assert(w.shape == (*shape_2d, n_phases))
     np.testing.assert_array_less(-1e-30, w)
     np.testing.assert_array_almost_equal(np.sum(w, axis=2), 1)
 
 def test_generate_laplacian_weights():
     shape_2d = [28, 36]
     n_phases = 5
     
-    w = laplacian_weights(shape_2d=shape_2d, n_phases=n_phases)
+    w = wts.laplacian_weights(shape_2d=shape_2d, n_phases=n_phases)
     
     assert(w.shape == (*shape_2d, n_phases))
     np.testing.assert_array_less(-1e-30, w)
     np.testing.assert_array_almost_equal(np.sum(w, axis=2), 1)
     
 def test_generate_two_sphere():
     shape_2d = [80, 80]
     n_phases = 3
     radius = 2
     
-    w = spheres_weights(shape_2d=shape_2d, n_phases=n_phases, radius= radius)
+    w = wts.spheres_weights(shape_2d=shape_2d, n_phases=n_phases, radius= radius)
     
     assert(w.shape == (80, 80, 3))
     np.testing.assert_array_less(-1e-30, w)
     np.testing.assert_array_almost_equal(np.sum(w, axis=2), 1)
 
 def test_generate_gaussian_ripple() : 
     shape_2d = [100,40]
     width = 10
     
-    w = gaussian_ripple_weights(shape_2d, width = width)
+    w = wts.gaussian_ripple_weights(shape_2d, width = width)
 
     assert(w.shape == (100,40,2))
     np.testing.assert_array_less(-1e-30,w)
     np.testing.assert_array_almost_equal(np.sum(w,axis = 2), 1)
 
-def test_gen_EDXS () : 
+# def test_gen_EDXS () : 
     
-    b_dict = generate_brem_params(42)
-    assert b_dict["b0"] <= 1.0 
-    assert b_dict["b1"] <= 1.0
-
-    phases, dicts = generate_random_phases(n_phases=3,seed = 42)
-    np.testing.assert_array_less(-1e-30, phases)
-    model = EDXS(**DEFAULT_SYNTHETIC_DATA_DICT["model_parameters"])
-    model.generate_phases(dicts)
-    np.testing.assert_almost_equal(model.phases,phases)
+#     b_dict = generate_brem_params(42)
+#     assert b_dict["b0"] <= 1.0 
+#     assert b_dict["b1"] <= 1.0
+
+#     phases, dicts = generate_random_phases(n_phases=3,seed = 42)
+#     np.testing.assert_array_less(-1e-30, phases)
+#     model = EDXS(**DEFAULT_SYNTHETIC_DATA_DICT["model_parameters"])
+#     model.generate_phases(dicts)
+#     np.testing.assert_almost_equal(model.phases,phases)
 
-    unique_list = unique_elts(dicts)
-    assert len(unique_list) == len(set(unique_list))
+#     unique_list = unique_elts(dicts)
+#     assert len(unique_list) == len(set(unique_list))
 
 def test_spim () : 
 
-    generate_dataset(seeds_range=1,**DATA_DICT)
-    gen_folder = DATASETS_PATH / Path(DATA_DICT["data_folder"])
+    if os.path.exists(str(DATASETS_PATH / Path(misc_params["data_folder"]))):
+        shutil.rmtree(str(DATASETS_PATH / Path(misc_params["data_folder"])))
+    phases1 = generate_modular_phases(elts_dicts = elts_dicts, brstlg_pars =  brstlg_pars, scales = scales, model_params = model_params)
+    maps = generate_weights(weight_type='sphere', shape_2d= misc_params["shape_2d"], n_phases=len(elts_dicts), seed=misc_params["seed"], radius = 15)
+    generate_dataset(base_seed=misc_params['seed'],
+                    sample_number=2,
+                    model_params = model_params,
+                    misc_params = misc_params,
+                    phases = phases1,
+                    weights = maps,
+                    elements = elements)
+    gen_folder = DATASETS_PATH / Path(misc_params["data_folder"])
     gen_si = hs.load(gen_folder / Path("sample_0.hspy"))
 
     assert gen_si.metadata.Signal.signal_type == "EDS_espm"
 
     mod_pars = get_metadata(gen_si)
-    mod_pars["params_dict"]["Abs"]["atomic_fraction"] = False
+    # mod_pars["params_dict"]["Abs"]["atomic_fraction"] = False
 
-    assert DATA_DICT["model_parameters"] == mod_pars
+    assert model_params == mod_pars
 
     shape = gen_si.shape_2d
-    G1 = gen_si.build_G(problem_type = "identity")
-    G2 = gen_si.build_G(problem_type = "no_brstlg",reference_elt = {})
-    G3 = gen_si.build_G(problem_type = "bremsstrahlung",reference_elt = {})
+    gen_si.build_G(problem_type = "identity")
+    assert shape == (100,120)
+    assert gen_si.G is None
+    gen_si.build_G(problem_type = "no_brstlg",reference_elt = {})
+    assert gen_si.G.shape == (1900, 8)
+    gen_si.build_G(problem_type = "bremsstrahlung",reference_elt = {})
+    assert callable(gen_si.G)
+    assert gen_si.G().shape == (1900, 10)
     Xflat = gen_si.X
-    print(gen_si.metadata.Sample.elements)
+    
 
-    assert shape == (100,120)
-    np.testing.assert_array_equal(G1,np.diag(np.ones((1900,))))
-    assert G2.shape == (1900, 8)
-    assert callable(G3)
-    assert G3().shape == (1900, 10)
-    G4 = gen_si.build_G(problem_type = "no_brstlg")
-    G5 = gen_si.build_G(problem_type = "bremsstrahlung")
-    assert G4.shape == (1900, 9)
-    assert G5().shape == (1900, 11)
+    gen_si.build_G(problem_type = "no_brstlg",reference_elt = {"26" : 3.0})
+    assert gen_si.G.shape == (1900, 9)
+    gen_si.build_G(problem_type = "bremsstrahlung",reference_elt = {"26" : 3.0})
+    assert gen_si.G().shape == (1900, 11)
     assert Xflat.shape == (1900, 120*100)
 
     detector_dict = {
         "detection" : {
             "thickness" : 45,
             "elements_dict" : {
                 "Si" : 3,
```

### Comparing `espm-0.1.4/espm/tests/test_docstring.py` & `espm-0.2.0/espm/tests/test_docstring.py`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/espm/tests/test_estimators.py` & `espm-0.2.0/espm/tests/test_estimators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,95 +1,89 @@
 from sklearn.utils.estimator_checks import check_estimator
 from espm.estimators.surrogates import diff_surrogate, smooth_l2_surrogate, smooth_dgkl_surrogate
 from espm.estimators import SmoothNMF
 from espm.estimators.base import normalization_factor
 import numpy as np
 from espm.models import EDXS
-from espm.datasets.generate_weights import generate_weights
+from espm.weights import generate_weights
 from espm.datasets.base import generate_spim
 from espm.measures import trace_xtLx
 from espm.utils import create_laplacian_matrix
 from espm.models.edxs import G_EDXS
+from espm.models.generate_EDXS_phases import generate_modular_phases
+from espm.datasets.base import generate_spim_sample
 import hyperspy.api as hs
 
-def generate_one_sample():
-    model_parameters = {
-        "e_offset" : 0.2,
-        "e_size" : 2000,
-        "e_scale" : 0.01,
-        "width_slope" : 0.01,
-        "width_intercept" : 0.065,
-        "db_name" : "default_xrays.json",
-        "E0" : 200,
-        "params_dict" : {
-            "Abs" : {
-                "thickness" : 100.0e-7,
-                "toa" : 35,
-                "density" : 5
-            },
-            "Det" : "SDD_efficiency.txt"
-        }
+
+phases_dict  = {
+    'elts_dicts'  : [
+    {"Fe" : 0.54860348,
+     "Pt" : 0.38286879,
+     "Mo" : 0.03166235},
+    {"Ca" : 0.54860348,
+     "Si" : 0.38286879,
+     "O" : 0.03166235}
+    ],
+    'brstlg_pars' : [
+    {'b0': 5e-3,
+    'b1': 3e-2},
+    {'b0': 7e-3,
+      'b1': 5e-2}
+    ],
+    'scales' : [0.05,0.05],
+    'model_params': {'e_offset': 0.2,
+    'e_size': 2000,
+    'e_scale': 0.01,
+    'width_slope': 0.01,
+    'width_intercept': 0.065,
+    'db_name': '200keV_xrays.json',
+    'E0': 200,
+    'params_dict': {'Abs': {'thickness': 1e-05,
+    'toa': 35,
+    'density': 5,
+    'atomic_fraction': False},
+    'Det': 'SDD_efficiency.txt'}}
     }
 
-    misc_params = {
-    "N" : 100,
-    "densities" : [1.3,1.6],
-    "data_folder" : "test_gen_data",
-    "seed" : 42,
-    "weight_type" : "laplacian",
-    "shape_2d" : (10,20),
-    "weights_params" : {"radius" : 1.5},
-    "model" : "EDXS"}
-    
-    
-    phases_parameters = [{"b0" : 5e-3,
-                            "b1" : 3e-2,
-                            "scale" : 0.05,
-                            "elements_dict" : {"Fe" : 0.54860348,
-                                      "Pt" : 0.38286879,
-                                      "Mo" : 0.03166235}},
-                            {"b0" : 7e-3,
-                            "b1" : 5e-2,
-                            "scale" : 0.05,
-                            "elements_dict" : {"Ca" : 0.54860348,
-                                      "Si" : 0.38286879,
-                                      "O" : 0.15166235}}]
+misc_dict = {
+  'N': 100,
+  'seed' : 42,
+  'data_folder': 'built_in_particules',
+  'shape_2d': [10, 20],
+  'model': 'EDXS',
+  'densities': [1.3, 1.6]
+}
+
+def generate_one_sample():
+
 
-    N = misc_params["N"]
     
     # Generate the phases
-    model = EDXS(**model_parameters)
-    model.generate_phases(phases_parameters)
-    phases = model.phases
+    model = EDXS(**phases_dict["model_params"])
+    phases =  generate_modular_phases(**phases_dict)
     model.generate_g_matr(g_type="bremsstrahlung", elements=["Fe", "Mo", "Ca", "Si", "O", "Pt"] ,reference_elt={})
     G = model.G
 
-    weights = generate_weights(misc_params["weight_type"], misc_params["shape_2d"], n_phases=len(phases_parameters), seed=misc_params["seed"], **misc_params["weights_params"])
-
-    stoch = generate_spim(phases, weights, misc_params["densities"], misc_params["N"], seed=misc_params["seed"],continuous = False)
-    cont = generate_spim(phases, weights, misc_params["densities"], misc_params["N"], seed=misc_params["seed"],continuous = True)
-
-    spim_stoch = hs.signals.Signal1D(stoch)
-    spim_stoch.set_signal_type("EDS_espm")
+    weights = generate_weights.generate_weights("laplacian", misc_dict["shape_2d"], n_phases=len(phases_dict["elts_dicts"]), seed=misc_dict["seed"], size_x = 10, size_y = 10)
 
-    spim_cont = hs.signals.Signal1D(cont)
-    spim_cont.set_signal_type("EDS_espm")
+    sample = generate_spim_sample(phases, weights, phases_dict["model_params"],misc_dict, seed = 42,g_params = {})
 
-    X = spim_stoch.X
-    X_cont = spim_cont.X
-    
-    D = phases.T
-    H = weights.reshape((misc_params["shape_2d"][0]*misc_params["shape_2d"][1],len(phases_parameters))).T
+    X = sample["X"].reshape(-1, sample["X"].shape[-1]).T
+    X_cont = sample['Xdot'].reshape(-1, sample['Xdot'].shape[-1]).T
     
+    D = sample['GW'].T
+    H = sample["H_flat"].T
+
     W = np.abs(np.linalg.lstsq(G, D, rcond=None)[0])
     for i in range(10) : 
-        G = G_EDXS(model_parameters, {"g_type" : "bremsstrahlung", "elements" : ["Fe", "Mo", "Ca", "Si", "O", "Pt"]},W[:-2,:],G)
+        G = G_EDXS(model, {"g_type" : "bremsstrahlung", "elements" : ["Fe", "Mo", "Ca", "Si", "O", "Pt"]},W[:-2,:],G)
         W = np.abs(np.linalg.lstsq(G, D, rcond=None)[0])
 
-    w = np.array(misc_params["densities"])
+    w = np.array(misc_dict["densities"])
+    N = misc_dict["N"]
 
     return G, W, H, D, w, X, X_cont, N
 
 def gen_fixed_mat () : 
     fixed_W = -1*np.ones((8,2))
     fixed_W[0,0] = 0.0
     fixed_W[1,0] = 0.0
@@ -100,41 +94,41 @@
 
     return fixed_W, fixed_H
 
 
 def test_generate_one_sample():
     G, W, H, D, w, X, Xdot, N = generate_one_sample()
     np.testing.assert_allclose(G @ W , D, atol=1e-3)
-    np.testing.assert_allclose( N * D @ np.diag(w) @ H , Xdot)
-    np.testing.assert_allclose(N * G @ W @ np.diag(w) @ H , Xdot, atol=1e-1)
+    np.testing.assert_allclose( D @ H , Xdot)
+    np.testing.assert_allclose(G @ W @ H , Xdot, atol=1e-1)
 
 def test_NMF_scikit () : 
     estimator = SmoothNMF(n_components= 5,max_iter=200,force_simplex = True,mu = 1.0, epsilon_reg = 1.0,hspy_comp = False)
     check_estimator(estimator)
     estimator = SmoothNMF( n_components= 5,lambda_L=2,max_iter=200,force_simplex = True,mu = 1.0, epsilon_reg = 1.0,hspy_comp = False)
     check_estimator(estimator)
 
 def test_general():
     G, W, H, D, w, X, Xdot, N = generate_one_sample()
 
     estimator = SmoothNMF(G=G,n_components= 2,max_iter=200,force_simplex = True,mu = 0, epsilon_reg = 1, hspy_comp = False)
     D2 = estimator.fit_transform(H=H, X=Xdot)
-    np.testing.assert_allclose(N*D@np.diag(w), D2, atol=3e-1)
+    np.testing.assert_allclose(D, D2, atol=6e-1)
 
     estimator = SmoothNMF(n_components= 2,max_iter=200,force_simplex = True,mu = 0, epsilon_reg = 1, hspy_comp = False)
     D2 = estimator.fit_transform(H=H, X=Xdot)
-    np.testing.assert_allclose(N*D@np.diag(w), D2, atol=3e-1)
+    np.testing.assert_allclose(D, D2, atol=6e-1)
 
     estimator = SmoothNMF(G=G,n_components= 2,max_iter=200,force_simplex = False,mu = 0, epsilon_reg = 1, hspy_comp = False)
-    D2 = estimator.fit_transform( W=W@np.diag(w), X=Xdot)
-    np.testing.assert_allclose(N*D@np.diag(w), D2, atol=3e-1)
+    D2 = estimator.fit_transform( W=W, X=Xdot)
+    np.testing.assert_allclose(D, D2, atol=3e-1)
 
     estimator = SmoothNMF(G =G, n_components= 2,max_iter=200,force_simplex = True,mu = 0, epsilon_reg = 1, hspy_comp = False)
-    D2 = estimator.fit_transform(W=N*W@np.diag(w), X=Xdot)
-    np.testing.assert_allclose(N*D@np.diag(w), D2, atol=3e-1)
+    D2 = estimator.fit_transform(W=W, X=Xdot)
+    np.testing.assert_allclose(D, D2, atol=3e-1)
 
     estimator = SmoothNMF(G=G, n_components= 2,max_iter=200,force_simplex = True,mu = 0, epsilon_reg = 1, hspy_comp = False)
     estimator.fit_transform(X=Xdot)
     P2, A2 = estimator.W_, estimator.H_ 
     np.testing.assert_allclose(G @ P2 @ A2,  Xdot, atol=1)
 
     estimator = SmoothNMF(G=G, n_components= 2,max_iter=200,force_simplex = True,mu = 0, epsilon_reg = 1, hspy_comp = False)
```

### Comparing `espm-0.1.4/espm/tests/test_laplacian.py` & `espm-0.2.0/espm/tests/test_laplacian.py`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/espm/tests/test_measures.py` & `espm-0.2.0/espm/tests/test_measures.py`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/espm/tests/test_updates.py` & `espm-0.2.0/espm/tests/test_updates.py`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/espm/tests/test_utils.py` & `espm-0.2.0/espm/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/espm/utils.py` & `espm-0.2.0/espm/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""Utils for the ESPM package"""
+r"""Utils for the ESPM package"""
 
 import numpy as np
 from scipy.sparse import lil_matrix, block_diag
 from scipy.optimize import nnls
 from espm.conf import SYMBOLS_PERIODIC_TABLE, NUMBER_PERIODIC_TABLE
 import json
 from hyperspy.misc.material import atomic_to_weight, density_of_mixture
 from functools import wraps
 
 _qtg_widgets = []
 _plt_figures = []
 
 def process_losses(losses):
-    """ Process the losses to be plotted
+    r""" Process the losses to be plotted
 
     Parameters
     ----------
     losses: np.ndarray
         Array of losses (output of `espm.estimators.NMFEstimator.get_losses` method)
 
     Returns
@@ -32,15 +32,15 @@
     for data in losses:
         for i, d in enumerate(data):
             values[i].append(d)
     values = np.array(values)
     return values, names
 
 def create_laplacian_matrix(nx, ny=None):
-    """
+    r"""
     Helper method to create the laplacian matrix for the laplacian regularization
     
     Parameters
     ----------
     :param nx: height of the original image
     :param ny: width of the original image
 
@@ -72,15 +72,15 @@
     #Diagonals linking different rows
     blocks.setdiag(-1,k=ny)
     blocks.setdiag(-1,k=-ny)
     return blocks
 
 
 def rescaled_DH(D,H) :
-    """Rescale the matrices D and H such that the columns of H sums approximately to one.
+    r"""Rescale the matrices D and H such that the columns of H sums approximately to one.
 
     :param np.array 2D D: n x k matrix
     :param np.array 2D H: k x m matrix
 
     :return: D_rescale, H_rescale
     :rtype: np.array 2D, np.array 2D   
 
@@ -91,27 +91,27 @@
     if (s<=0).any():
         s = np.maximum(nnls(H.T, o)[0], 1e-10)
     D_rescale = D@np.diag(1/s)
     H_rescale = np.diag(s)@H
     return D_rescale, H_rescale
 
 def bin_spim(data,n,m):
-    """ 
+    r""" 
     
     Take a 3D array of size (x,y,k) [px, py, e]
     Returns a 3D array of size (n,m,k) [new_px, new_py, e]
     """
     # return a matrix of shape (n,m,k)
     bs = data.shape[0]//n,data.shape[1]//m  # blocksize averaged over
     k = data.shape[2]
     return np.reshape(np.array([np.sum(data[k1*bs[0]:(k1+1)*bs[0],k2*bs[1]:(k2+1)*bs[1]],axis=(0,1)) for k1 in range(n) for k2 in range(m)]),(n,m,k))
 
 
 def number_to_symbol_dict (func) : 
-    """
+    r"""
     Decorator
     Takes a dict of elements (a.k.a chemical composition) with atomic numbers as keys (e.g. 26 for Fe)
     returns a dict of elements with symbols as keys (e.g. Fe for iron)
     """
     @wraps(func)
     def inner(*args,**kwargs) : 
         elts_dict = kwargs["elements_dict"]
@@ -132,15 +132,15 @@
         
         kwargs["elements_dict"] = new_dict
         return func(*args,**kwargs)
 
     return inner
 
 def symbol_to_number_dict (func) : 
-    """
+    r"""
     Decorator
     Takes a dict of elements (a.k.a chemical composition) with symbols as keys (e.g. Fe for iron)
     returns a dict of elements with atomic numbers as keys (e.g. 26 for iron)
     """
     @wraps(func)
     def inner(*args,**kwargs) : 
         elts_dict = kwargs["elements_dict"]
@@ -159,15 +159,15 @@
                 raise ValueError("Input has to be either atomic number, either chemical symbols")
         
         kwargs["elements_dict"] = new_dict
         return func(*args,**kwargs)
     return inner
 
 def symbol_to_number_list (func) : 
-    """
+    r"""
     Decorator
     Takes a dict of elements (a.k.a chemical composition) with symbols as keys (e.g. Fe for iron)
     returns a dict of elements with atomic numbers as keys (e.g. 26 for iron)
     """
     @wraps(func)
     def inner(*args,**kwargs) : 
         elts_list = kwargs["elements"]
@@ -184,15 +184,15 @@
         
         kwargs["elements"] = new_list
         return func(*args,**kwargs)
             
     return inner
 
 def number_to_symbol_list (func) : 
-    """
+    r"""
     Decorator
     Takes a dict of elements (a.k.a chemical composition) with symbols as keys (e.g. Fe for iron)
     returns a dict of elements with atomic numbers as keys (e.g. 26 for iron)
     """
     @wraps(func)
     def inner(*args,**kwargs) : 
         elts_list = kwargs["elements"]
@@ -210,15 +210,15 @@
         kwargs["elements"] = new_list
         return func(*args,**kwargs)
             
     return inner
 
 @number_to_symbol_dict
 def atomic_to_weight_dict (*,elements_dict = {}) :
-    """
+    r"""
     Wrapper to the atomic_to_weight function of hyperspy. Takes a dict of chemical composition expressed in atomic fractions.
     Returns a dict of chemical composition expressed in atomic weight fratiom.
     """ 
     if len(elements_dict.keys()) == 0 : 
         return elements_dict
     else : 
         list_elts = []
@@ -232,15 +232,15 @@
         for i, elt in enumerate(list_elts) : 
             new_dict[elt] = list_wt[i]
         
         return new_dict
 
 @number_to_symbol_dict
 def approx_density(atomic_fraction = False,*,elements_dict = {}) :
-    """
+    r"""
     Wrapper to the density_of_mixture function of hyperspy. Takes a dict of chemical composition expressed in atomic weight fractions.
     Returns an approximated density.
     """  
     if len(elements_dict.keys()) == 0 : 
         return 1.0
     else : 
         list_elts = []
@@ -251,15 +251,15 @@
         for elt in elements_dict.keys() : 
             list_elts.append(elt)
             list_wt.append(elements_dict[elt])
         
         return density_of_mixture(list_wt,list_elts)
 
 def arg_helper(params, d_params):
-    """ Check if all parameter of d_params are in params. If not, they are added to params with the default value.
+    r""" Check if all parameter of d_params are in params. If not, they are added to params with the default value.
 
     Parameters
     ----------
     params : dict
         Dictionary of parameters to be checked.
     d_params : dict
         Dictionary of default parameters.
@@ -274,15 +274,15 @@
         params[key] = params.get(key, d_params[key])
         if isdict(params[key])  and isdict(d_params[key]):
             params[key] = arg_helper(params[key], d_params[key])
     check_keys(params, d_params)
     return params
 
 def check_keys(params, d_params, upperkeys = '',toprint = True):
-    """ Check if all parameter of d_params are in params. If not, they are added to params with the default value.
+    r""" Check if all parameter of d_params are in params. If not, they are added to params with the default value.
 
     Parameters
     ----------
     params : dict
         Dictionary of parameters to be checked.
     d_params : dict
         Dictionary of default parameters.
@@ -318,41 +318,41 @@
 #                     check_keys(params[key],d_params[key],upperkeys=upperkeys+'[\'{}\']'.format(key))
                 if isdict(d_params[key]):
                     if toprint :
                         check_keys(params[key],d_params[key],upperkeys=upperkeys+'[\'{}\']'.format(key))
     return True
 
 def isdict(p):
-    """Return True if the variable a dictionary.
+    r"""Return True if the variable a dictionary.
     
     :param p: variable to check
     :type p: any
     :return: True if p is a dictionary
     :rtype: bool
 
     """
     return type(p) is dict
 
 def is_symbol (i) :
-    """ Return True if i is a chemical symbol
+    r""" Return True if i is a chemical symbol
     
     :param i: variable to check
     :type i: any
     :return: True if i is a chemical symbol
     :rtype: bool
 
     """
     symb_list = symbol_list()
     if i in symb_list : 
         return True
     else : 
         return False
 
 def is_number (i) :
-    """ Return True if i is a number
+    r""" Return True if i is a number
 
     :param i: variable to check
     :type i: any
     :return: True if i is a number
     :rtype: bool
 
     """
```

### Comparing `espm-0.1.4/espm.egg-info/SOURCES.txt` & `espm-0.2.0/espm.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -3,64 +3,63 @@
 CONTRIBUTING.rst
 Licence.txt
 MANIFEST.in
 README.rst
 hyperspy_extension.yaml
 readthedoc.yml
 setup.py
+todo.md
 .github/workflows/python.yml
 doc/changelog.rst
 doc/conf.py
 doc/contributing.rst
 doc/index.rst
 doc/references.rst
 doc/introduction/index.rst
 doc/reference/datasets.rst
 doc/reference/estimators.rst
 doc/reference/index.rst
 doc/reference/measures.rst
 doc/reference/models.rst
+doc/reference/table_utils.rst
 doc/reference/utils.rst
 doc/reference/weights.rst
 doc/styles/sg_gallery.css
 espm/__init__.py
 espm/conf.py
 espm/hyperspy_extension.yaml
 espm/measures.py
 espm/spectrum_fitting.py
 espm/tables_utils.py
 espm/utils.py
-espm/weights.py
 espm.egg-info/PKG-INFO
 espm.egg-info/SOURCES.txt
 espm.egg-info/dependency_links.txt
 espm.egg-info/entry_points.txt
 espm.egg-info/not-zip-safe
 espm.egg-info/requires.txt
 espm.egg-info/top_level.txt
 espm/datasets/__init__.py
 espm/datasets/base.py
-espm/datasets/built_in_datasets.py
-espm/datasets/generate_EDXS_phases.py
-espm/datasets/generate_weights.py
-espm/datasets/samples.py
-espm/datasets/spim.py
+espm/datasets/built_in_EDXS_datasets.py
+espm/datasets/eds_spim.py
 espm/datasets/toy-problem/phase1.png
 espm/datasets/toy-problem/phase2.png
 espm/estimators/__init__.py
 espm/estimators/base.py
 espm/estimators/dicotomy.py
 espm/estimators/smooth_nmf.py
 espm/estimators/surrogates.py
 espm/estimators/updates.py
 espm/models/EDXS_function.py
 espm/models/__init__.py
 espm/models/absorption_edxs.py
 espm/models/base.py
 espm/models/edxs.py
+espm/models/generate_EDXS_phases.py
 espm/tables/100keV_xrays.json
 espm/tables/200keV_xrays.json
 espm/tables/300keV_xrays.json
 espm/tables/SDD_efficiency.txt
 espm/tables/__init__.py
 espm/tables/default_xrays.json
 espm/tables/periodic_table_number.json
@@ -71,52 +70,25 @@
 espm/tests/test_datasets.py
 espm/tests/test_docstring.py
 espm/tests/test_estimators.py
 espm/tests/test_laplacian.py
 espm/tests/test_measures.py
 espm/tests/test_updates.py
 espm/tests/test_utils.py
-experiments/HPC_batch_experiment.py
-experiments/HPC_single_experiment.py
-experiments/ICA_script.py
-experiments/NMF_script.py
-experiments/VCA.py
-experiments/VCA_script.py
-experiments/complex_data_paper.py
-experiments/conf.py
-experiments/data_paper.py
-experiments/experiments.py
-experiments/generate_synthetic_dataset.py
-experiments/mcrllm.py
-experiments/mcrllm_batch.py
-experiments/mcrllm_script.py
-experiments/mcrllm_wrapper.py
-experiments/quick_NMF_script.py
-experiments/sunsal.py
-experiments/test_experiments.py
+espm/weights/__init__.py
+espm/weights/abundance.py
+espm/weights/generate_weights.py
 notebooks/VCA.py
 notebooks/api.ipynb
 notebooks/background_fit.ipynb
 notebooks/convergence-speed.ipynb
 notebooks/generate_data.ipynb
 notebooks/make-plots.ipynb
 notebooks/other_algorithms.ipynb
 notebooks/preprocess_dataset.ipynb
-notebooks/read_HPC_data _TEMP.ipynb
-notebooks/read_HPC_data.ipynb
 notebooks/select_spectrum.ipynb
 notebooks/simple-test-regularisation.ipynb
 notebooks/spectrum_fit.ipynb
 notebooks/sunsal.py
 notebooks/surrogate-vs-bregmann.ipynb
 notebooks/toy-ML.ipynb
-notebooks/old/AT_testing.ipynb
-notebooks/old/algo-with-negative-variable.ipynb
-notebooks/old/analyse_one_method.ipynb
-notebooks/old/analyze_data.ipynb
-notebooks/old/analyze_data_v2.ipynb
-notebooks/old/bremstrahlung.ipynb
-notebooks/old/dicho_test.ipynb
-notebooks/old/generate_artificial_data.ipynb
-notebooks/old/spectrum_fit.ipynb
-notebooks/old/speedtest.ipynb
-scripts/toy_experiment.py
+notebooks/old/algo-with-negative-variable.ipynb
```

### Comparing `espm-0.1.4/experiments/VCA.py` & `espm-0.2.0/notebooks/VCA.py`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/experiments/sunsal.py` & `espm-0.2.0/notebooks/sunsal.py`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/notebooks/api.ipynb` & `espm-0.2.0/notebooks/api.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9898040674603175%*

 * *Differences: {"'cells'": "{2: {'source': {delete: [9]}}, 6: {'source': "*

 * *            '[\'spim.build_G("bremsstrahlung")\']}, 8: {\'source\': [\'est = SmoothNMF( '*

 * *            "n_components = 3,tol=0.000001, max_iter = 50, G = spim.G,hspy_comp = True)']}, 12: "*

 * *            "{'source': ['spim.print_concentration_report()']}}",*

 * * "'metadata'": "{'kernelspec': {'display_name': 'Python 3'}, 'language_info': {'version': "*

 * *               "'3.8.10'}, 'vscode': {'interpreter': {'hash': "*

 * *               "'e7370f93d1d0cde622a1f8e1c […]*

```diff
@@ -30,15 +30,14 @@
                 "%matplotlib inline\n",
                 "\n",
                 "# Generic imports \n",
                 "import hyperspy.api as hs\n",
                 "import numpy as np\n",
                 "\n",
                 "# espm imports\n",
-                "from espm.models.EDXS_function import print_concentrations_from_W\n",
                 "from espm.estimators import SmoothNMF\n",
                 "import espm.datasets as ds"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
@@ -77,15 +76,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "G = spim.build_G(\"bremsstrahlung\")"
+                "spim.build_G(\"bremsstrahlung\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -100,15 +99,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "est = SmoothNMF( n_components = 3,tol=0.000001, max_iter = 1000, G = G,hspy_comp = True)"
+                "est = SmoothNMF( n_components = 3,tol=0.000001, max_iter = 50, G = spim.G,hspy_comp = True)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -142,15 +141,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "print_concentrations_from_W(est.W_, elements = spim.metadata.Sample.elements)"
+                "spim.print_concentration_report()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
@@ -170,29 +169,29 @@
             "source": [
                 "spim.plot_decomposition_factors(3)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "espm",
+            "display_name": "Python 3",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.6"
+            "version": "3.8.10"
         },
         "varInspector": {
             "cols": {
                 "lenName": 16,
                 "lenType": 16,
                 "lenVar": 40
             },
@@ -217,14 +216,14 @@
                 "instance",
                 "_Feature"
             ],
             "window_display": false
         },
         "vscode": {
             "interpreter": {
-                "hash": "a7ceffc662db6c9d514927743d8d35570797b920e33613212d4f424c0416cf91"
+                "hash": "e7370f93d1d0cde622a1f8e1c04877d8463912d04d973331ad4851f04de6915a"
             }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `espm-0.1.4/notebooks/background_fit.ipynb` & `espm-0.2.0/notebooks/background_fit.ipynb`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/notebooks/convergence-speed.ipynb` & `espm-0.2.0/notebooks/convergence-speed.ipynb`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/notebooks/generate_data.ipynb` & `espm-0.2.0/notebooks/generate_data.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9837695802005013%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(6, 'from espm.weights.generate_weights import "*

 * *            "chemical_map_weights\\n'), (7, 'from espm.models.generate_EDXS_phases import "*

 * *            "generate_modular_phases\\n'), (8, 'from espm.models.EDXS_function import "*

 * *            "elts_list_from_dict_list\\n')], delete: [9, 8, 6, 5]}}, 4: {'source': {insert: [(9, "*

 * *            "'path = get_repo_path() / "*

 * *            'Path("generated_datasets/71GPa_experimental_data.hspy")\\n\'), (12, \'weights = '*

 * *           […]*

```diff
@@ -28,19 +28,18 @@
             "outputs": [],
             "source": [
                 "%load_ext autoreload\n",
                 "%autoreload 2\n",
                 "%matplotlib inline\n",
                 "\n",
                 "# espm imports\n",
-                "from espm.datasets.generate_weights import generate_weights, chemical_maps_weights\n",
-                "from espm.datasets.generate_EDXS_phases import generate_random_phases, unique_elts, generate_modular_phases\n",
                 "from espm.datasets.base import generate_dataset\n",
-                "from espm.utils import arg_helper\n",
-                "from pathlib import Path\n",
+                "from espm.weights.generate_weights import chemical_map_weights\n",
+                "from espm.models.generate_EDXS_phases import generate_modular_phases\n",
+                "from espm.models.EDXS_function import elts_list_from_dict_list\n",
                 "\n",
                 "# Generic imports \n",
                 "from pathlib import Path\n",
                 "import matplotlib.pyplot as plt\n",
                 "import numpy as np\n",
                 "import hyperspy.api as hs\n",
                 "\n"
@@ -67,18 +66,18 @@
                 "    \n",
                 "    This is a bit of a hack, but it works.\n",
                 "    \"\"\"\n",
                 "    this_path = Path.cwd() / Path(\"generate_data.ipynb\")\n",
                 "    return this_path.resolve().parent.parent\n",
                 "\n",
                 "# Path of the experimental dataset\n",
-                "path = get_repo_path() / Path(\"experiments/71GPa_experimental_data.hspy\")\n",
+                "path = get_repo_path() / Path(\"generated_datasets/71GPa_experimental_data.hspy\")\n",
                 "\n",
                 "#\u00a0Creation of the weights\n",
-                "weights = chemical_maps_weights(path,[\"Fe_Ka\",\"Ca_Ka\"],conc_max = 0.7)"
+                "weights = chemical_map_weights( file = path, line_list = [\"Fe_Ka\",\"Ca_Ka\"], conc_list = [0.5,0.5])"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -195,24 +194,23 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "phases, full_dict = generate_modular_phases(\n",
+                "phases = generate_modular_phases(\n",
                 "    elts_dicts=elts_dicts, brstlg_pars = brstlg_pars,\n",
                 "    scales = [1, 1, 1],\n",
                 "    model_params= model_params,\n",
                 "    seed = 42\n",
                 "    )\n",
                 "# scales : bremsstrahlung parameters modifiers\n",
                 "\n",
-                "# Finish building the dictionnary of the simulation\n",
-                "data_dict.update(full_dict)"
+                "elements = elts_list_from_dict_list(elts_dicts)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -227,17 +225,17 @@
             },
             "outputs": [],
             "source": [
                 "fig,axs = plt.subplots(3,1,figsize = (20,15))\n",
                 "\n",
                 "# Build the energy scale\n",
                 "x = np.linspace(\n",
-                "    full_dict[\"model_parameters\"][\"e_offset\"],\n",
-                "    full_dict[\"model_parameters\"][\"e_offset\"]+full_dict[\"model_parameters\"][\"e_scale\"]*full_dict[\"model_parameters\"][\"e_size\"],\n",
-                "    num=full_dict[\"model_parameters\"][\"e_size\"])\n",
+                "    model_params[\"e_offset\"],\n",
+                "    model_params[\"e_offset\"]+model_params[\"e_scale\"]*model_params[\"e_size\"],\n",
+                "    num=model_params[\"e_size\"])\n",
                 "\n",
                 "for j in range(axs.shape[0]) :\n",
                 "    axs[j].plot(x,phases[j])\n",
                 "    axs[j].set_title(\"Phase {}\".format(j),fontsize = 22)\n",
                 "\n",
                 "axs[-1].set_xlabel(\"Energy loss (eV)\",fontsize = 16)"
             ]
@@ -256,42 +254,32 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "generate_dataset(seeds_range=1, **data_dict, weights=weights )"
+                "generate_dataset( phases = phases,\n",
+                "                  weights = weights,\n",
+                "                  model_params = model_params,\n",
+                "                  misc_params = data_dict,\n",
+                "                  base_seed=data_dict[\"seed\"],\n",
+                "                  sample_number=1,\n",
+                "                  elements = elements)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The previous command will save the data in the `generated_datasets` folder defined in the `espm.conf.py` file.\n",
                 "\n",
                 "You can also define the path where the data will be saved using the \"base_path\" argument"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "# generate_dataset(basepath=\"generated_samples\", seeds_range=1, **data_dict, weights=weights )"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "espm",
             "language": "python",
             "name": "python3"
@@ -302,15 +290,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.6"
+            "version": "3.8.10"
         },
         "vscode": {
             "interpreter": {
                 "hash": "8d9f0750808bbb89d6238996d547b1a0ab25cae94b245e8c4572708d26b443fd"
             }
         }
     },
```

### Comparing `espm-0.1.4/notebooks/old/algo-with-negative-variable.ipynb` & `espm-0.2.0/notebooks/old/algo-with-negative-variable.ipynb`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/notebooks/old/analyse_one_method.ipynb` & `espm-0.2.0/notebooks/surrogate-vs-bregmann.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7935303853067011%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, '%matplotlib inline')], delete: [2]}}, 1: {'source': "*

 * *            "{insert: [(2, 'from matplotlib.ticker import LinearLocator\\n'), (3, '\\n')], delete: "*

 * *            "[4, 3, 2]}}, 2: {'source': ['nx = 20\\n', 'ny = nx\\n', 'lx = 2\\n', 'ly = 2\\n', "*

 * *            "'\\n', 'xt = np.array([0.5, 0.5])\\n', 'a = np.array([0.2, 0.8])\\n', '\\n', '\\n', "*

 * *            "'xt = np.expand_dims(xt, axis=[0,1])\\n', 'a = np.expand_dims(a, axis=[0,1])\\n', "*

 * *            "'\\n', ' […]*

```diff
@@ -4,311 +4,283 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "%load_ext autoreload\n",
                 "%autoreload 2\n",
-                "%matplotlib inline\n"
+                "%matplotlib inline"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
-                "from snmfem.experiments import load_samples, print_results, load_data, run_experiment\n",
-                "from snmfem.measures import KLdiv\n",
-                "import re"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "import warnings\n",
-                "warnings.simplefilter(action='ignore', category=FutureWarning)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "# Running NMF"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## Inputs"
+                "from matplotlib.ticker import LinearLocator\n",
+                "\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "dataset = \"dataset_EDXS.json\"\n",
-                "n_sample = 0"
+                "nx = 20\n",
+                "ny = nx\n",
+                "lx = 2\n",
+                "ly = 2\n",
+                "\n",
+                "xt = np.array([0.5, 0.5])\n",
+                "a = np.array([0.2, 0.8])\n",
+                "\n",
+                "\n",
+                "xt = np.expand_dims(xt, axis=[0,1])\n",
+                "a = np.expand_dims(a, axis=[0,1])\n",
+                "\n",
+                "x1 = np.arange(lx/nx, lx+lx/nx, lx/nx)\n",
+                "x2 = np.arange(ly/ny, ly+ly/ny, ly/ny)\n",
+                "X1, X2 = np.meshgrid(x1, x2)\n",
+                "X = np.array([X1, X2]).T\n",
+                "\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "samples, k = load_samples(dataset)\n",
-                "sample = samples[n_sample]"
+                "X.shape, a.shape, xt.shape"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# About initialization\n",
-                "# 'random': non-negative random matrices, scaled with: sqrt(X.mean() / n_components)\n",
-                "# 'nndsvd': Nonnegative Double Singular Value Decomposition (NNDSVD) initialization (better for sparseness)\n",
-                "# 'nndsvda': NNDSVD with zeros filled with the average of X (better when sparsity is not desired)\n",
-                "# 'nndsvdar' NNDSVD with zeros filled with small random values (generally faster, less accurate alternative to NNDSVDa for when sparsity is not desired)\n",
+                "def f(x, a):\n",
+                "    T = np.sum(a*x, axis=-1)\n",
+                "    return - np.log(T) + T\n",
                 "\n",
-                "# for me random was the best initialization...\n",
-                "default_params = {\n",
-                "    \"n_components\" : k,\n",
-                "    \"tol\" : 1e-6,\n",
-                "    \"max_iter\" : 10000,\n",
-                "    \"init\" : \"random\",\n",
-                "    \"random_state\" : 1,\n",
-                "    \"verbose\" : 1\n",
-                "    }\n",
+                "def MU_surrogate(x, a, xt):\n",
+                "    ut = a*xt\n",
+                "    ut = ut / np.sum(ut, axis=-1, keepdims=True)\n",
+                "    return np.sum( - ut * ( np.log(a*x) - np.log(ut) ) + a*x, axis=-1)\n",
                 "\n",
-                "params_snmf = {\n",
-                "    \"force_simplex\" : True,\n",
-                "    \"skip_G\" : False,\n",
-                "    \"mu\": np.array([0, 1, 1])\n",
-                "}\n",
+                "def EM_surrogate(x, a, xt):\n",
+                "    pass\n",
                 "\n",
-                "params_evalution = {\n",
-                "    \"u\" : True,\n",
-                "}\n",
+                "def Bregman_surrogate(x, a, xt):\n",
+                "    L = 1\n",
+                "    ax = np.sum(a*x, axis=-1)\n",
+                "    axt = np.sum(a*xt, axis=-1)\n",
+                "    return ax - ax / axt + np.sum(- np.log(x) + x / xt, axis=-1)\n",
                 "\n",
-                "# All parameters are contained here\n",
-                "exp = {\"name\": \"snmfem smooth 30\", \"method\": \"SmoothNMF\", \"params\": {**default_params, **params_snmf, \"lambda_L\" : 100.0}}"
+                "def Weighted_Bregman_surrogate(x, a, xt):\n",
+                "    L = 1\n",
+                "    ax = np.sum(a*x, axis=-1)\n",
+                "    axt = np.sum(a*xt, axis=-1)\n",
+                "    ut = a*xt\n",
+                "    ut = ut / np.sum(ut, axis=-1, keepdims=True)\n",
+                "    return ax - ax / axt + np.sum(- ut*np.log(x) + ut*x / xt, axis=-1)\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "Xflat, true_spectra, true_maps, G, shape_2d = load_data(sample)\n"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "# Run a single experiment and plotting results"
+                "Z = f(X,a)\n",
+                "Z_MU = MU_surrogate(X, a, xt)\n",
+                "Z_Bregman = Bregman_surrogate(X, a, xt)\n",
+                "Z_Weighted_Bregman = Weighted_Bregman_surrogate(X, a, xt)\n",
+                "\n",
+                "fxk = f(xt, a)\n",
+                "Z_Bregman = Z_Bregman-Bregman_surrogate(xt, a, xt) + fxk\n",
+                "Z_Weighted_Bregman = Z_Weighted_Bregman-Weighted_Bregman_surrogate(xt, a, xt) + fxk"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "Xflat, true_spectra, true_maps, G, shape_2d = load_data(sample)\n",
-                "\n",
-                "m, (GP, A), loss  = run_experiment(Xflat, true_spectra, true_maps, G, exp, params_evalution,shape_2d)\n"
+                "Z.shape, X1.shape"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "Xtrue = true_spectra.T @ true_maps"
+                "def subplot3d(ax, X1, X2, Z):\n",
+                "    # Plot the surface.\n",
+                "    surf = ax.plot_surface(X1, X2, Z, cmap=plt.cm.coolwarm,\n",
+                "                        linewidth=0, antialiased=False)\n",
+                "    # Customize the z axis.\n",
+                "    # ax.set_zlim(-1.01, 1.01)\n",
+                "    ax.zaxis.set_major_locator(LinearLocator(10))\n",
+                "    # A StrMethodFormatter is used automatically\n",
+                "    ax.zaxis.set_major_formatter('{x:.02f}')\n",
+                "\n",
+                "    # Add a color bar which maps values to colors.\n",
+                "    plt.colorbar(surf, shrink=0.5, aspect=5)\n",
+                "\n",
+                "plt.figure(figsize=(18, 5),)\n",
+                "\n",
+                "ax = plt.subplot(1,3,1,  projection='3d')\n",
+                "subplot3d(ax, X1, X2, Z)\n",
+                "\n",
+                "ax = plt.subplot(1,3,2,  projection='3d')\n",
+                "subplot3d(ax, X1, X2, Z_MU)\n",
+                "\n",
+                "ax = plt.subplot(1,3,3,  projection='3d')\n",
+                "subplot3d(ax, X1, X2, Z_Bregman)\n",
+                "\n",
+                "plt.show()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from snmfem.measures import KL\n",
-                "print(KL(Xflat, Xtrue, average=True))\n",
-                "print(KL(Xflat, GP @ A, average=True))\n",
-                "print(KL(Xtrue, GP @ A, average=True))\n"
+                "\n",
+                "\n",
+                "plt.figure(figsize=(8,8))\n",
+                "rstride = 2\n",
+                "cstride = 2\n",
+                "ax = plt.subplot( projection='3d')\n",
+                "\n",
+                "ax.plot_wireframe(X1, X2, Z, rstride=rstride, cstride=cstride, color=\"black\", label=\"$f(x)$\")\n",
+                "ax.plot_wireframe(X1, X2, Z_MU, rstride=rstride, cstride=cstride, color=\"green\", label=\"MU surrogate\")\n",
+                "ax.plot_wireframe(X1, X2, Z_Bregman, rstride=rstride, cstride=cstride, color=\"blue\", label=\"Bregman surrogate\")\n",
+                "ax.scatter3D(xt[:,:,0], xt[:,:,1], fxk[0], \"o\",color=\"red\", label=\"$x^t$\", linewidth=6)\n",
+                "ax.legend()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Ploting parameters\n",
-                "fontsize = 15\n",
-                "aspect_ratio = 3/4\n",
-                "scale = 20\n",
-                "cmap = plt.cm.gist_heat_r\n",
-                "vmin = 0\n",
-                "vmax = np.max(true_maps)\n",
-                "\n"
+                "nx = 500\n",
+                "lx = 2\n",
+                "y = 0.5\n",
+                "\n",
+                "xt = np.array([0.5, y])\n",
+                "a = np.array([0.2, 0.8])\n",
+                "\n",
+                "\n",
+                "xt = np.expand_dims(xt, axis=[0,1])\n",
+                "a = np.expand_dims(a, axis=[0,1])\n",
+                "\n",
+                "x1 = np.arange(lx/nx, lx+lx/nx, lx/nx)\n",
+                "x2 = np.arange(y, y+ly/ny, ly/ny)\n",
+                "X1, X2 = np.meshgrid(x1, x2)\n",
+                "X = np.array([X1, X2]).T"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "metric = np.array(m[:-1])\n",
-                "order = np.array(m[-1])\n",
-                "\n",
-                "fig, axes = plt.subplots(k,3,figsize = (scale, scale/3*k * aspect_ratio))\n",
-                "\n",
-                "\n",
-                "for j in range(k):\n",
-                "    ind = np.arange(k)[order[0,j]]\n",
-                "    axes[j, 0].plot(true_spectra[j],'bo',label='truth',linewidth=4)\n",
-                "    axes[j, 0].plot(GP[:,ind] ,'r-',label='reconstructed',markersize=3.5)\n",
-                "    axes[j, 0].set_title(\"{:.2f} deg\".format(metric[0,j]))\n",
-                "\n",
-                "for j in range(k):\n",
-                "    ind = np.arange(k)[order[1,j]]\n",
-                "    axes[j, 1].imshow(A[ind].reshape(*shape_2d), vmin=vmin, vmax=vmax, cmap=cmap)\n",
-                "    axes[j, 1].set_title(\"Mse: {:.2f}\".format(metric[1,j]))\n",
-                "    axes[j, 2].imshow(true_maps[j].reshape(*shape_2d), vmin=vmin, vmax=vmax, cmap=cmap)   \n",
-                "    \n",
-                "rows = ['Phase {}'.format(col) for col in range(k)]\n",
-                "cols = [\"Phase\", \"Map\", \"Real map\"]\n",
-                "\n",
-                "for ax, col in zip(axes[0], cols):\n",
-                "    ax.set_title(col, fontsize=fontsize)\n",
+                "z = f(X,a)\n",
+                "z_MU = MU_surrogate(X, a, xt)\n",
+                "z_Bregman = Bregman_surrogate(X, a, xt)\n",
+                "z_Weighted_Bregman = Weighted_Bregman_surrogate(X, a, xt)\n",
                 "\n",
-                "for ax, row in zip(axes[:,0], rows):\n",
-                "    ax.set_ylabel(row, rotation=90, fontsize=fontsize)\n",
-                "\n",
-                "fig.tight_layout()\n",
-                "\n",
-                "plt.show()\n"
+                "fxk = f(xt, a)\n",
+                "z_Bregman = z_Bregman-Bregman_surrogate(xt, a, xt) + fxk\n",
+                "z_Weighted_Bregman = z_Weighted_Bregman-Weighted_Bregman_surrogate(xt, a, xt) + fxk"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "# Quick and dirty way to look at the Loss"
+                "def argmin(x, z):\n",
+                "    i = np.argmin(z)\n",
+                "    return x[i], z[i]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# fig, axes = plt.subplots(1, 2, figsize=(10, 3))\n",
+                "plt.figure(figsize=(6,4))\n",
                 "\n",
-                "# names = list(loss.dtype.names)\n",
-                "# values = np.array([list(e) for e in loss])\n",
+                "plt.plot(x1, z, color=\"black\", label=\"$f(x)$\")\n",
+                "plt.plot(x1, z_MU, color=\"green\", label=\"MU surrogate\")\n",
+                "plt.plot(*argmin(x1,z_MU), \"x\", color=\"green\", label=\"MU minimum\")\n",
+                "plt.plot(x1, z_Bregman,  color=\"blue\", label=\"Bregman surrogate\")\n",
+                "plt.plot(*argmin(x1,z_Bregman), \"x\", color=\"blue\", label=\"Bregman minimum\")\n",
                 "\n",
-                "# # axes[0].plot(values[:,1:-2], markersize=3.5)\n",
-                "# axes[0].plot(values[:,1],'b',markersize=3.5)\n",
-                "# axes[0].plot(values[:,0],'r--',markersize=3.5)\n",
-                "# axes[0].set_yscale(\"log\")\n",
-                "# axes[0].set_xlabel(\"number of iterations\")\n",
-                "# # axes[0].legend(names[1:-2] + [names[0]])\n",
-                "# axes[0].legend([names[1]] + [names[0]])\n",
-                "# axes[0].set_title(\"Losses\")\n",
+                "# plt.plot(x1, z_Weighted_Bregman,  color=\"orange\", label=\"Weigthed Bregman surrogate\")\n",
+                "# plt.plot(*argmin(x1,z_Weighted_Bregman), \"x\", color=\"orange\", label=\"Weighted Bregman minimum\")\n",
                 "\n",
-                "# axes[1].plot(values[:,-2:], markersize=3.5)\n",
-                "# axes[1].legend(names[-2:])\n",
-                "# axes[1].set_xlabel(\"number of iterations\")\n",
-                "# axes[1].set_title(\"Evolution of A and P\")\n",
-                "# axes[1].set_yscale(\"log\")\n",
                 "\n",
-                "# fig.tight_layout()"
+                "plt.plot(xt[0, 0, :1], fxk, \"o\", color=\"red\", label=\"$x^t$\" )\n",
+                "plt.ylim([1,2])\n",
+                "plt.xlim([0,2])\n",
+                "plt.legend(loc=1)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
-            "source": [
-                "mark_space = 20\n",
-                "marker_list = [\"-o\",\"-s\",\"->\",\"-<\",\"-^\",\"-v\",\"-d\"]\n",
-                "\n",
-                "\n",
-                "fig, axes = plt.subplots(1, 4, figsize=(15, 3))\n",
-                "\n",
-                "names = list(loss.dtype.names)\n",
-                "for j,name in enumerate(names) :\n",
-                "    if re.match(r\".*(loss)\",name) : \n",
-                "        axes[0].plot(loss[name],marker_list[j%len(marker_list)],markersize=3.5,label = name,markevery = mark_space,linewidth = 2)\n",
-                "        axes[0].set_yscale(\"log\")\n",
-                "        axes[0].legend()\n",
-                "        axes[0].set_xlabel(\"number of iterations\")\n",
-                "    elif re.match(r\"^(rel)\",name) : \n",
-                "        axes[1].plot(loss[name],marker_list[j%len(marker_list)],markersize=3.5,label = name,markevery = mark_space,linewidth = 2)\n",
-                "        axes[1].legend()\n",
-                "        axes[1].set_xlabel(\"number of iterations\")\n",
-                "    elif re.match(r\"^(ang)\",name) :\n",
-                "        axes[2].plot(loss[name],marker_list[j%len(marker_list)],markersize=3.5,label = name,markevery = mark_space,linewidth = 2)\n",
-                "        axes[2].legend()\n",
-                "        axes[2].set_xlabel(\"number of iterations\")\n",
-                "    elif re.match(r\"^(mse)\",name) :\n",
-                "        axes[3].plot(loss[name],marker_list[j%len(marker_list)],markersize=3.5,label = name,markevery = mark_space,linewidth = 2)\n",
-                "        axes[3].legend()\n",
-                "        axes[3].set_xlabel(\"number of iterations\")\n",
-                "\n",
-                "cols = [\"Losses\", \"Evolution of A and P\",\"Angles\",\"MSE\"]\n",
-                "\n",
-                "for ax, col in zip(axes, cols):\n",
-                "    ax.set_title(col, fontsize=fontsize)\n",
-                "\n",
-                "fig.tight_layout()"
-            ]
+            "source": []
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "espm",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.6"
+            "version": "3.10.6"
+        },
+        "vscode": {
+            "interpreter": {
+                "hash": "a7ceffc662db6c9d514927743d8d35570797b920e33613212d4f424c0416cf91"
+            }
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 4
+    "nbformat_minor": 2
 }
```

### Comparing `espm-0.1.4/notebooks/old/analyze_data.ipynb` & `espm-0.2.0/notebooks/toy-ML.ipynb`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7501277884526178%*

 * *Differences: {"'cells'": '{1: {\'source\': [\'## Imports and function definition\\n\', \'\\n\', "Let\'s start '*

 * *            'by importing the necessary libraries."], \'attachments\': OrderedDict()}, 2: '*

 * *            "{'source': ['# Some useful modules for notebooks\\n', '%load_ext autoreload\\n', "*

 * *            "'%autoreload 2\\n', '%matplotlib inline']}, 3: {'source': ['import numpy as np\\n', "*

 * *            "'import matplotlib.pyplot as plt\\n', 'from espm.estimators import SmoothNMF\\n', "*

 * *            "'from espm.measu […]*

```diff
@@ -1,661 +1,607 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Imports"
+                "# Regularized Poisson NMF on a toy dataset\n",
+                "\n",
+                "This notebook is part of the ESPM package. It is available on [github](https://github.com/adriente/espm/blob/main/notebooks/toy-ML.ipynb) \n",
+                "\n",
+                "In this notebook, we show how to solve a regularized Poisson Non Negative Matrix Factorization (NMF) on a toy dataset. The general goal of this problem is to separate a matrix $X$ into two matrices $D$ and $H$ such that $X \\approx DH$. \n",
+                "We will assume that $D$ is the product of two matrices $G$ and $W$ such that $D = GW$. The matrix $G$ is assumed to be known and therefore $W$ is the matrix we want to find. In the field of electro-microscopy, the matrix $GW$ represent the phases, the matrix $H$ is the matrix of maps (or weights) and $X$ is the data matrix. The maps $H$ are 2D images.\n",
+                "Furthermore, we will assume that $W, H$ are non-negative or more generally greater than a small positive value $\\epsilon$. \n",
+                "\n",
+                "The data measured data $X$ is follow a Poisson distribution, i.e. $X_{ij} \\sim \\text{Poisson}(n_p\\dot{X}_{ij})$. In the context of electro-microscopy, $n_p$ is the number of photons per pixel. $\\dot{X} = G \\dot{W} \\dot{H}$ would correspond a noiseless measurement. \n",
+                "\n",
+                "The size of:\n",
+                "\n",
+                "* $X$ is (n, p),\n",
+                "* $W$ is (m, k),\n",
+                "* $H$ is (k, p),\n",
+                "* $G$ is (n, m).\n",
+                "\n",
+                "In general, m is assumed to be much smaller than n and $G$ is assumed to be known. The parameter `shape_2d` defines the shape of the images for the columns of $H$ and $X$, i.e. `shape_2d[0]*shape_2d[1] = p`.\n",
+                "\n",
+                "Mathematically. the problem can be formulated as:\n",
+                "$$\\dot{W}, \\dot{H} = \\arg\\min_{W\\geq\\epsilon, H\\geq\\epsilon, \\sum_i H_{ij}  = 1} D_{GKL}(X || GWH) + \\lambda tr ( H^\\top \\Delta H) + \\mu \\sum_{i,j} (\\log H_{ij} +  \\epsilon_{reg})$$\n",
+                "\n",
+                "Here $D_{GKL}$ is the fidelity term, i.e. the Generalized KL divergence \n",
+                "\n",
+                "$$D_{GKL}(X \\| Y) = \\sum_{i,j} X_{ij} \\log \\frac{X_{ij}}{Y_{ij}} - X_{ij} + Y_{ij} $$\n",
+                "\n",
+                "The loss is regularized using two terms: a Laplacian regularization on $H$ and a log regularization on $H$. \n",
+                "$\\lambda$ and $\\mu$ are the regularization parameters.\n",
+                "The Laplacian regularization is defined as:\n",
+                "\n",
+                "$$ \\lambda tr ( H^\\top \\Delta H) $$\n",
+                "\n",
+                "where $\\Delta$ is the Laplacian operator (it can be created using the function :mod:`espm.utils.create_laplacian_matrix`). **Note that the columns of the matrices $H$ and $X$ are assumed to be images.** \n",
+                "\n",
+                "The log regularization is defined as:\n",
+                "\n",
+                "$$ \\mu \\sum_{i,j} (\\log H_{ij} +  \\epsilon_{reg}) $$\n",
+                "\n",
+                "where $\\epsilon_{reg}$ is the slope of log regularization at 0. This term acts similarly to an L1 penalty but affects less larger values. \n",
+                "\n",
+                "Finally, we assume $W,H\\geq \\epsilon$ and that the lines of $H$ sum to 1: $$\\sum_i H_{ij}  = 1.$$ This is done by adding the parameter `force_simplex=True` to the class `espm.estimators.SmoothNMF`. This constraint is essential as it prevent the algorithm to find a solution where all the maps tend to 0 because of the other constraints.\n",
+                "\n",
+                "In this notebook, we will use the class `espm.estimators.SmoothNMF` to solve the problem.\n"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "%matplotlib qt\n",
-                "import matplotlib.pyplot as plt\n",
-                "import numpy as np\n",
-                "# from snmf import SNMF\n",
-                "# import EDXS_model\n",
-                "import h5py\n",
-                "# hyperspy is the commonly used library to handle spectrum images in the electron microscopy community\n",
-                "import hyperspy.api as hs\n",
-                "# import utils as u\n",
-                "import snmfem\n",
-                "from snmfem.measures import find_min_angle,find_min_MSE\n",
-                "from snmfem import EDXS_model\n",
-                "from snmfem.estimator.snmf import SNMF"
+                "## Imports and function definition\n",
+                "\n",
+                "Let's start by importing the necessary libraries."
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "# Load the data"
+                "# Some useful modules for notebooks\n",
+                "%load_ext autoreload\n",
+                "%autoreload 2\n",
+                "%matplotlib inline"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# filename=\"Data/71GPa_subsolidus\"\n",
-                "filename = \"C:/Users/teurtrie/Travail/SNMF_EDXS/snmfem/Data/aspim037_N100_2ptcls_brstlg\"\n",
-                "\n",
-                "S=hs.load(filename+\".hspy\")\n",
-                "X=S.data\n",
-                "\n",
-                "# This part of the spectrum image contains only pure spectra from phase 0\n",
-                "# This kind of area is often available in experimental datasets\n",
-                "X_part=S.inav[60:,:].data\n",
-                "\n",
-                "# Loading of ground truth\n",
-                "true_spectra=[]\n",
-                "true_maps=[]\n",
-                "true_spectra.append(np.genfromtxt(filename+\"spectrum_p0\"))\n",
-                "true_spectra.append(np.genfromtxt(filename+\"spectrum_p1\"))\n",
-                "true_spectra.append(np.genfromtxt(filename+\"spectrum_p2\"))\n",
-                "true_maps.append(np.load(filename+\"map_p0.npy\"))\n",
-                "true_maps.append(np.load(filename+\"map_p1.npy\"))\n",
-                "true_maps.append(np.load(filename+\"map_p2.npy\"))"
+                "import numpy as np\n",
+                "import matplotlib.pyplot as plt\n",
+                "from espm.estimators import SmoothNMF\n",
+                "from espm.measures import find_min_angle, ordered_mse, ordered_mae, ordered_r2\n",
+                "from espm.models import ToyModel\n",
+                "from espm.weights import generate_weights as gw\n",
+                "from espm.datasets.base import generate_spim_sample\n",
+                "from espm.utils import process_losses"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Performance assessment functions\n",
-                "\n",
-                "These functions are used to compare the endmembers determined by SNMF and the ground truth"
+                "Now we define the parameters that will be used to generate the data.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# This function will find the best matching endmember for each true spectrum. This is useful since the A and P matrice are initialized at random. \n",
                 "\n",
-                "# This function works but can probably greatly improved\n",
-                "def find_min_angle (list_true_vectors,list_algo_vectors) :\n",
-                "    # This function calculates all the possible angles between endmembers and true spectra\n",
-                "    # For each true spectrum a best matching endmember is found\n",
-                "    # The function returns the angles of the corresponding pairs\n",
-                "    copy_algo_vectors=list_algo_vectors.copy()\n",
-                "    size=list_algo_vectors[0].shape\n",
-                "    ordered_angles=[]\n",
-                "    for i in range(len(list_true_vectors)) :\n",
-                "        list_angles=[]\n",
-                "        for j in range(len(list_algo_vectors)) :\n",
-                "            list_angles.append(u.Functions.spectral_angle(list_true_vectors[i],list_algo_vectors[j]))\n",
-                "        ind_min=np.argmin(np.array(list_angles))\n",
-                "        list_algo_vectors[ind_min]=1e28*np.ones(size)\n",
-                "        ordered_angles.append(u.Functions.spectral_angle(list_true_vectors[i],copy_algo_vectors[ind_min]))\n",
-                "    return ordered_angles\n",
+                "seed = 0 # for reproducibility\n",
                 "\n",
-                "# This function works but can probably greatly improved\n",
-                "def find_min_MSE (list_true_maps,list_algo_maps) :\n",
-                "    # This function calculates all the possible MSE between abundances and true maps\n",
-                "    # For each true map a best matching abundance is found\n",
-                "    # The function returns the MSE of the corresponding pairs\n",
-                "    copy_algo_maps=list_algo_maps.copy()\n",
-                "    size=list_algo_maps[0].shape\n",
-                "    ordered_maps=[]\n",
-                "    for i in range(len(list_true_maps)) :\n",
-                "        list_maps=[]\n",
-                "        for j in range(len(list_algo_maps)) :\n",
-                "            list_maps.append(u.Functions.MSE_map(list_true_maps[i],list_algo_maps[j]))\n",
-                "        ind_min=np.argmin(np.array(list_maps))\n",
-                "        list_algo_maps[ind_min]=1e28*np.ones(size)\n",
-                "        ordered_maps.append(u.Functions.MSE_map(list_true_maps[i],copy_algo_maps[ind_min]))\n",
-                "    return ordered_maps\n",
+                "m = 15 # Number of components\n",
+                "n = 200 # Length of the phases\n",
                 "\n",
-                "# This function gives the residuals between the model determined by snmf and the data that were fitted\n",
-                "def residuals (data,model) :\n",
-                "    X_sum=data.sum(axis=0).sum(axis=0)\n",
-                "    model_sum=model.get_phase_map(0).sum()*model.get_phase_spectrum(0)+model.get_phase_map(1).sum()*model.get_phase_spectrum(1)+model.get_phase_map(2).sum()*model.get_phase_spectrum(2)\n",
-                "    return X_sum-model_sum"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "# Parameters "
+                "n_poisson = 300 # Average poisson number per pixel (this number will be splitted on the m dimension)\n",
+                "\n",
+                "densities = np.random.uniform(0.1, 2.0, 3) # Random densities\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# True bremsstrahlung parameters\n",
-                "brstlg_pars = {\"c0\" : 4.8935e-05,\"c1\" : 1464.19810, \"c2\" : 0.04216872, \"b0\" : 0.15910789, \"b1\" : -0.00773158, \"b2\" : 8.7417e-04}\n",
-                "# brstlg_pars = {\n",
-                "#                 \"c0\"  :  8.0192e-08,\n",
-                "#                 \"c1\"  :  380.523471\t,\n",
-                "#                 \"c2\"  :  2.7332e-11,\n",
-                "#                 \"b0\"  :  0.09002422,\n",
-                "#                 \"b1\"  :  -0.0162849,\n",
-                "#                 \"b2\"  :  0.00193291\n",
-                "#                 }\n",
+                "def get_toy_sample():\n",
+                "    model_params = {\"L\": n, \"C\": m, \"K\": 3, \"seed\": seed}\n",
+                "    misc_params = {\"N\": n_poisson, \"seed\": seed, 'densities' : densities, \"model\": \"ToyModel\"}\n",
                 "\n",
+                "    toy_model = ToyModel(**model_params)\n",
+                "    toy_model.generate_phases()\n",
+                "    phases = toy_model.phases.T\n",
+                "    weights = gw.generate_weights(\"toy_problem\", None)\n",
                 "\n",
-                "# SNMF parameters\n",
-                "tol = 1e-4\n",
-                "max_iter = 50000\n",
-                "b_tol = 1e-1\n",
-                "mu_sparse = 0.0\n",
-                "eps_sparse = 1.0\n",
-                "phases = 3\n",
-                "em = EDXS_model.EDXS_Model(\"C:/Users/teurtrie/Travail/SNMF_EDXS/snmfem/Data/simple_xrays_threshold.json\",brstlg_pars = brstlg_pars,e_offset=S.axes_manager[2].offset,e_scale=S.axes_manager[2].scale,e_size=S.axes_manager[2].size)\n",
-                "# em.generate_g_matr([8,13,14,12,26,29,31,72,71,62,60,92,20],brstlg = False)\n",
-                "em.generate_g_matr([12,13,14,20,26,29,31,34,40,60,62,71,92],brstlg = True)\n",
+                "    sample = generate_spim_sample(phases, weights, model_params,misc_params, seed = seed)\n",
+                "    return sample\n",
                 "\n",
+                "def to_vec(X):\n",
+                "    n = X.shape[2]    \n",
+                "    return X.transpose(2,0,1).reshape(n, -1)\n",
                 "\n",
+                "sample = get_toy_sample()\n",
                 "\n",
-                "# # If mu_sparse !=0 a good initialization of the first phase is required, it can be done using the spectrum below\n",
-                "init_matrix=np.average(X_part,axis=(0,1))"
+                "GW = sample[\"GW\"].T\n",
+                "G = sample[\"G\"]\n",
+                "H = to_vec(sample[\"H\"])\n",
+                "X = to_vec(sample[\"X\"])\n",
+                "Xdot = to_vec(sample[\"Xdot\"])\n",
+                "shape_2d = sample[\"shape_2d\"]\n",
+                "\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# SNMF"
+                "Let us look at the dimension of our problem."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Creation of an SNMF object with the parameters above\n",
-                "mdl = SNMF(max_iter = max_iter, tol = tol, b_tol = b_tol, mu_sparse=mu_sparse, eps_sparse = eps_sparse, num_phases=phases,edxs_model=em, brstlg_pars = brstlg_pars, init_spectrum = init_matrix)"
+                "print(f\"\"\"\n",
+                "- X: {X.shape}\n",
+                "- Xdot: {Xdot.shape}\n",
+                "- G: {G.shape}\n",
+                "- GW: {GW.shape}\n",
+                "- H: {H.shape}\n",
+                "- shape_2d: {shape_2d}\n",
+                "\"\"\")"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "tags": [
-                    "outputPrepend"
-                ]
-            },
-            "outputs": [],
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
             "source": [
-                "mdl.fit(X,eval_print=True)"
+                "Here `Xdot` contains the noisless data such that the ground truth `H` and `GW` satisfies:\n",
+                "$$X = GWH$$"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "\n",
-                "\n",
-                "filename = \"C:/Users/teurtrie/Travail/SNMF_EDXS/Code/Results/aspims/mask_bl_mu0.57_eps1.0_out.hdf5\"\n",
-                "\n",
-                "with h5py.File(filename, \"r\") as f:\n",
-                "    # List all groups\n",
-                "    print(\"Keys: %s\" % f.keys())\n",
-                "    a = list(f.keys())[0]\n",
-                "    b = list(f.keys())[1]\n",
-                "    g = list(f.keys())[2]\n",
-                "    p = list(f.keys())[3]\n",
-                "\n",
-                "    # Get the data\n",
-                "    loaded_a = np.array(f[a])\n",
-                "    loaded_b = np.array(f[b])\n",
-                "    loaded_g = np.array(f[g])\n",
-                "    loaded_p = np.array(f[p])\n",
-                "\n",
-                "h_spec = loaded_g@loaded_p + loaded_b\n",
-                "\n",
-                "# f_b = \"Results/0.3wt%Nd-Sm-Hf-Lu-U-A-X15-71GPa_subsolidus grains_01_Brg spectrum.hdf5\"\n",
-                "# f_c = \"Results/0.3wt%Nd-Sm-Hf-Lu-U-A-X15-71GPa_subsolidus grains_01_CaPv spectrum.hdf5\"\n",
-                "# f_f = \"Results/0.3wt%Nd-Sm-Hf-Lu-U-A-X15-71GPa_subsolidus grains_01_Fp spectrum.hdf5\"\n",
-                "\n",
-                "# with h5py.File(f_b, \"r\") as f :\n",
-                "#     brg = np.array(f[\"Experiments\"][\"EDSmap\"][\"data\"])\n",
-                "# with h5py.File(f_f, \"r\") as f :\n",
-                "#     fp = np.array(f[\"Experiments\"][\"EDSmap\"][\"data\"])\n",
-                "# with h5py.File(f_c, \"r\") as f :\n",
-                "#     capv = np.array(f[\"Experiments\"][\"EDSmap\"][\"data\"])\n",
-                "\n",
-                "# x_true = np.linspace(-0.48,-0.48+1047*0.01,num=1047)\n",
-                "# true_spectra = [brg,fp,capv]"
+                "np.testing.assert_allclose(Xdot, GW @ H)"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Let us plot the ground truth maps $H$ (sometimes also called weights). Here the variable `shape_2d` is used to reshape the columns of $H$ into images."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "filename = \"C:/Users/teurtrie/Travail/SNMF_EDXS/Code/Results/71GPa_subsolidus_mu3.0_eps1.0.hdf5\"\n",
-                "with h5py.File(filename, \"r\") as f:\n",
-                "    # List all groups\n",
-                "    print(\"Keys: %s\" % f.keys())\n",
-                "    a = list(f.keys())[0]\n",
-                "    b = list(f.keys())[1]\n",
-                "    p = list(f.keys())[2]\n",
-                "\n",
-                "    # Get the data\n",
-                "    loaded_a = np.array(f[a])\n",
-                "    loaded_b = np.array(f[b])\n",
-                "    loaded_p = np.array(f[p])\n",
                 "\n",
-                "h_spec = mdl.g_matr@loaded_p + loaded_b"
+                "vmin, vmax = 0,1\n",
+                "cmap = plt.cm.gray_r\n",
+                "plt.figure(figsize=(10, 3))\n",
+                "for i, hdot in enumerate(H):\n",
+                "    plt.subplot(1,3,i+1)\n",
+                "    plt.imshow(H[i].reshape(shape_2d), cmap=cmap, vmin=vmin, vmax=vmax)\n",
+                "    plt.axis(\"off\")\n",
+                "    plt.title(f\"GT - Map {i+1}\")"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "plt.imshow(aa)\n",
-                "plt.xticks(ticks=[])\n",
-                "plt.yticks(ticks=[])"
+                "We can also plot the phases corresponding to these maps. The phases corresponds to the matrix $GW$."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "a0 = (loaded_a[0,:]*128).astype(\"int\")\n",
-                "a1 = (loaded_a[1,:]*255000).astype(\"int\")\n",
-                "a2 = (loaded_a[2,:]*255).astype(\"int\")\n",
-                "a = np.vstack((a0,a1,a2))\n",
-                "\n"
+                "e = np.linspace(0,1, GW.shape[0])\n",
+                "plt.plot(e, GW)\n",
+                "plt.title(\"GT - Phases\")\n",
+                "plt.xlabel(\"Frequency [normalized]\")\n",
+                "plt.legend([f\"phase {i+1}\" for i in range(3)]);"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "aa = a.T.reshape(201,201,3)"
+                "The matrix $G$ is assumed to be known appriori. Here we plot the first 5 lines of $G$."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "np.sqrt(121203)"
+                "l = np.linspace(0, 1,n)\n",
+                "plt.plot(l, G[:,:5]);"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "trunc_true = x_true > em.x[0]\n",
-                "trunc_res = (em.x < x_true[-1])\n",
-                "res_spec = [h_spec[:,0][trunc_res][:-1],h_spec[:,1][trunc_res][:-1],h_spec[:,2][trunc_res][:-1]]\n",
-                "true_spectra = [brg[trunc_true],fp[trunc_true],capv[trunc_true]]\n",
-                "\n",
-                "angles=find_min_angle(true_spectra,res_spec)\n",
+                "Note that the function `create_toy_sample` did not return $W$ but only $GW$. \n",
                 "\n",
-                "print(\"Angle phase 0 :\",angles[0])\n",
-                "print(\"Angle phase 1 :\",angles[1])\n",
-                "print(\"Angle phase 2 :\",angles[2])\n"
+                "Using the ground truth $GW$, it can be computed as follows:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "angles=find_min_angle(true_spectra,[h_spec[:,0],h_spec[:,1],h_spec[:,2]])\n",
-                "\n",
-                "print(\"Angle phase 0 :\",angles[0])\n",
-                "print(\"Angle phase 1 :\",angles[1])\n",
-                "print(\"Angle phase 2 :\",angles[2])\n"
+                "W = np.linalg.lstsq(GW, G, rcond=None)[0].T\n",
+                "W.shape"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Results"
+                "## Solving the problem"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "# Returns the angles between the ground truth and the endmembers found using SNMF\n",
-                "angles=find_min_angle(true_spectra,[mdl.get_phase_spectrum(0),mdl.get_phase_spectrum(1),mdl.get_phase_spectrum(2)])\n",
-                "\n",
-                "maps=find_min_MSE(true_maps,[mdl.get_phase_map(0),mdl.get_phase_map(1),mdl.get_phase_map(2)])\n",
+                "#### Parameters\n",
                 "\n",
-                "print(\"Angle phase 0 :\",angles[0])\n",
-                "print(\"Angle phase 1 :\",angles[1])\n",
-                "print(\"Angle phase 2 :\",angles[2])\n",
-                "print(\"MSE phase 0 :\",maps[0])\n",
-                "print(\"MSE phase 1 :\",maps[1])\n",
-                "print(\"MSE phase 2 :\",maps[2])\n",
-                "\n",
-                "# RITM0165818"
+                "Let us define the different hyperparameters of the problem. Feel free to change them and see how the results change."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Visualisation of the results"
+                "Let us first define our regularisation parameters."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# switch correspond to the index of the SNMF endmember\n",
-                "# true correspond to the index of the true spectrum\n",
-                "# The 2 should be changed independantly until a match is found\n",
-                "switch = 1\n",
-                "true= 1\n",
-                "\n",
-                "plt.rcParams.update({'font.size': 22})\n",
-                "fig1 = plt.figure(figsize=(20, 12))\n",
-                "plt.subplot(121)\n",
-                "plt.plot(em.x,133*true_spectra[true]/np.sum(true_spectra[true]),'bo',label='truth',linewidth=4)\n",
-                "plt.plot(em.x, mdl.get_phase_spectrum(switch),'r-',label='reconstructed',markersize=3.5)\n",
-                "plt.legend(loc='best')\n",
-                "plt.xlim(0, 10)\n",
-                "plt.ylabel(\"Intensity\")\n",
-                "\n",
-                "plt.subplot(122)\n",
-                "plt.imshow(mdl.get_phase_map(switch), cmap=\"viridis\")\n",
-                "plt.grid(b=30)\n",
-                "plt.title(f\"Activations of first spectrum\")\n",
-                "plt.colorbar()\n",
-                "plt.clim(0, 1)\n",
-                "\n",
-                "fig1.tight_layout()"
+                "lambda_L = 1 # Smoothness of the maps\n",
+                "mu = 0.2 # Sparsity of the maps"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "# switch correspond to the index of the SNMF endmember\n",
-                "# true correspond to the index of the true spectrum\n",
-                "# The 2 should be changed independantly until a match is found\n",
-                "switch =2\n",
-                "true=1\n",
-                "\n",
-                "x = np.linspace(S.axes_manager[2].offset,S.axes_manager[2].offset+S.axes_manager[2].scale*S.axes_manager[2].size,num=S.axes_manager[2].size)\n",
-                "\n",
-                "N=[100,125,133]\n",
-                "\n",
-                "plt.rcParams.update({'font.size': 22})\n",
-                "fig1 = plt.figure(figsize=(20, 12))\n",
-                "plt.subplot(121)\n",
-                "plt.plot(x,N[true]*true_spectra[true]/np.sum(true_spectra[true]),'bo',label='truth',linewidth=4)\n",
-                "plt.plot(x, h_spec[:,switch],'r-',label='reconstructed',markersize=3.5)\n",
-                "plt.legend(loc='best')\n",
-                "plt.xlim(0, 10)\n",
-                "plt.ylabel(\"Intensity\")\n",
-                "\n",
-                "plt.subplot(122)\n",
-                "plt.imshow(loaded_a[switch].reshape(80,80), cmap=\"viridis\")\n",
-                "plt.grid(b=30)\n",
-                "plt.title(f\"Activations of first spectrum\")\n",
-                "plt.colorbar()\n",
-                "plt.clim(0, 1)\n",
-                "\n",
-                "fig1.tight_layout()"
+                "We can additionally add a simplex constraint to the problem by setting `force_simplex=True`. This will add the constraint that the line of $H$ sum to 1. This constraint should be activated for the regularizers to work!. Practically, it will prevent the algorithm from simply minimizing $W$ and increasing $H$."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "plt.imshow((loaded_a[0]>0.99).reshape(80,80))"
+                "force_simplex = True"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Finally, we can decide to specify $G$ or not. If the matrix $G$ is not specified, the algorithm will directly estimate $GW$ insead of $W$."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# switch correspond to the index of the SNMF endmember\n",
-                "# true correspond to the index of the true spectrum\n",
-                "# The 2 should be changed independantly until a match is found\n",
-                "switch = 1\n",
-                "true=2\n",
-                "\n",
-                "plt.rcParams.update({'font.size': 22})\n",
-                "fig1 = plt.figure(figsize=(20, 12))\n",
-                "plt.subplot(121)\n",
-                "#plt.plot(x_true[trunc_true],50000*true_spectra[true]/np.sum(true_spectra[true]),'bo',label='truth',linewidth=4)\n",
-                "plt.plot(em.x,h_spec[:,switch],'r-',label='reconstructed',markersize=3.5)\n",
-                "plt.legend(loc='best')\n",
-                "plt.xlim(0, 10)\n",
-                "plt.ylabel(\"Intensity\")\n",
-                "\n",
-                "plt.subplot(122)\n",
-                "plt.imshow(loaded_a[switch].reshape(201,201), cmap=\"viridis\")\n",
-                "plt.grid(b=30)\n",
-                "plt.title(f\"Activations of first spectrum\")\n",
-                "plt.colorbar()\n",
-                "#plt.clim(0, 1)\n",
-                "\n",
-                "fig1.tight_layout()"
+                "Gused = G"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Cross validation"
+                "Note that wihtout regularisation, i.e. with the parameters\n",
+                "```python\n",
+                "lambda_L = 0\n",
+                "mu = 0 \n",
+                "Gused = None\n",
+                "force_simplex=False\n",
+                "``` \n",
+                "we recover the classical Poisson/KL NMF problem. Our algorithm will apply the MU algorithm from Lee and Seung (2001)."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# En chantier"
+                "Let us define the parameters for the algorithm. Here the class `espm.estimator.SmoothNMF` heritates from sckit-learn's `NMF` class. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "init_p_matr = np.random.rand(dl.g_matr.shape[1],dl.p_)\n",
-                "init_p_matr[:,0] = (np.linalg.inv(dl.g_matr.T@dl.g_matr)@dl.g_matr.T@(true_spectra[0]-1.9*Distributions.simplified_brstlg(Gaussians().x,b0,b1,b2,c0))).clip(min=1e-5)\n",
-                "init_p_matr[:,1] = (np.linalg.inv(dl.g_matr.T@dl.g_matr)@dl.g_matr.T@(true_spectra[1]-2.0 *Distributions.simplified_brstlg(Gaussians().x,b0,b1,b2,c0))).clip(min=1e-5)\n",
-                "init_p_matr[:,2] = (np.linalg.inv(dl.g_matr.T@dl.g_matr)@dl.g_matr.T@(true_spectra[2]-1.7*Distributions.simplified_brstlg(Gaussians().x,b0,b1,b2,c0))).clip(min=1e-5)\n",
                 "\n",
-                "init_a_matr = np.random.rand(dl.p_, X.shape[0]*X.shape[1])\n",
-                "init_a_matr[0,:]= true_maps[0].reshape(6400)\n",
-                "init_a_matr[1,:]= true_maps[1].reshape(6400)\n",
-                "init_a_matr[2,:]= true_maps[2].reshape(6400)"
+                "K = len(H) # Number of components / let assume that we know it\n",
+                "params = {}\n",
+                "params[\"tol\"]=1e-6 # Tolerance for the stopping criterion.\n",
+                "params[\"max_iter\"] = 200 # Maximum number of iterations before timing out.\n",
+                "params[\"hspy_comp\"] = False # If should be set to True if hspy data format is used.\n",
+                "params[\"verbose\"] = 1 # Verbosity level.\n",
+                "params[\"eval_print\"] = 10 # Print the evaluation every eval_print iterations.\n",
+                "params[\"epsilon_reg\"] = 1 # Regularization parameter \n",
+                "params[\"linesearch\"] = False # Use linesearch to accelerate convergence\n",
+                "params[\"shape_2d\"] = shape_2d # Shape of the 2D maps\n",
+                "params[\"n_components\"] = K # Number of components\n",
+                "params[\"normalize\"] = True # Normalize the data. It helps to keep the range of the regularization parameters lambda_L and mu in a reasonable range.\n",
+                "\n",
+                "estimator = SmoothNMF(mu=mu, lambda_L=lambda_L, G = Gused, force_simplex=force_simplex, **params)"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "x_matr = np.random.rand(80*80,2000).T\n",
-                "a = loaded_a\n",
-                "mask1 = a[0,:] > 0.99\n",
-                "mask2 = a[1:,:]<0.01\n",
-                "mask = np.vstack((mask1,mask2))\n",
-                "L = adj(80)"
+                "The function `fit_transform` will solve the problem and return the matrix $GW$."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "n_mask = np.invert(mask)\n",
-                "neigh = (((mask[0,:]@L).clip(max=1)- mask[0,:].astype(\"int\")).clip(min=0)).astype(\"bool\")\n",
-                "a[0,:][neigh] = 0.8\n",
-                "a[0,:][np.logical_xor(n_mask[0,:],neigh)] = 0.1"
+                "GW_est = estimator.fit_transform(X)"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "plt.imshow(a[0,:].reshape(80,80))"
+                "We can plot the different losses to see how the algorithm converges."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "n2 = (((mask[0,:]@L).clip(max=1)- mask[0,:].astype(\"int\")).clip(min=0)).astype(\"bool\")\n"
+                "\n",
+                "losses = estimator.get_losses()\n",
+                "\n",
+                "values, names = process_losses(losses)\n",
+                "\n",
+                "plt.figure(figsize=(10, 6))\n",
+                "for name, value in zip(names[:4], values[:4]):\n",
+                "    plt.plot(value, label=name)\n",
+                "    plt.xlabel(\"iteration\")\n",
+                "plt.yscale(\"log\")\n",
+                "plt.legend()\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "a[0,:][n2] = 10000"
+                "losses[0]"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "plt.imshow(a[0,:].reshape(80,80))"
+                "We can easily recover $W$ and $H$ from the estimator."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from scipy.sparse import lil_matrix, block_diag\n",
-                "def adj(n):\n",
-                "    \"\"\"\n",
-                "    Helper method to create the laplacian matrix for the laplacian regularization\n",
-                "    :param n: width of the original image\n",
-                "    :return:the n x n laplacian matrix\n",
-                "    \"\"\"\n",
-                "    \n",
-                "    #Blocks corresponding to the corner of the image (linking row elements)\n",
-                "    top_block=lil_matrix((n,n),dtype=np.float32)\n",
-                "    #top_block.setdiag([1]+[1]*(n-2)+[1])\n",
-                "    top_block.setdiag(1,k=1)\n",
-                "    top_block.setdiag(1,k=-1)\n",
-                "    #Blocks corresponding to the middle of the image (linking row elements)\n",
-                "    mid_block=lil_matrix((n,n),dtype=np.float32)\n",
-                "    #mid_block.setdiag([1]+[1]*(n-2)+[1])\n",
-                "    mid_block.setdiag(1,k=1)\n",
-                "    mid_block.setdiag(1,k=-1)\n",
-                "    #Construction of the diagonal of blocks\n",
-                "    list_blocks=[top_block]+[mid_block]*(n-2)+[top_block]\n",
-                "    blocks=block_diag(list_blocks)\n",
-                "    #Diagonals linking different rows\n",
-                "    blocks.setdiag(1,k=n)\n",
-                "    blocks.setdiag(1,k=-n)\n",
-                "    return blocks"
+                "H_est = estimator.H_\n",
+                "W_est = estimator.W_"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "plt.imshow(adj(3).toarray())"
+                "Let us compute some metrics to evaluate the quality of the solution. We will use the metrics defined in the module `espm.metrics`.\n",
+                "\n",
+                "We first compute the angles between the phases `GW` and the estimated phases `GW_est`. The angles are computed using the function `compute_angles`. This function also return the indices to match the estimations and the ground truths. Indeed, there is no reason for them to have the same order. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "a = adj(80)\n",
-                "b = np.random.rand(6400)\n",
-                "a@b -b"
+                "angles, true_inds = find_min_angle(GW.T, GW_est.T, unique=True, get_ind=True)\n",
+                "print(\"angles : \", angles)"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Now, we can compute the Mean Squared Error (MSE) between the maps `H` and the estimated maps `H_est`. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "np.sqrt(6400)"
+                "mse = ordered_mse(H, H_est, true_inds)\n",
+                "print(\"mse : \", mse)"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Finally, let us plot the results. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "nbsphinx-thumbnail"
+                ]
+            },
             "outputs": [],
-            "source": []
+            "source": [
+                "\n",
+                "def plot_results(Ddot, D, Hdotflat, Hflat):\n",
+                "    fontsize = 30\n",
+                "    scale = 15\n",
+                "    aspect_ratio = 1.4\n",
+                "    marker_list = [\"-o\",\"-s\",\"->\",\"-<\",\"-^\",\"-v\",\"-d\"]\n",
+                "    mark_space = 20\n",
+                "    # cmap = plt.cm.hot_r    \n",
+                "    cmap = plt.cm.gray_r\n",
+                "    vmax = 1\n",
+                "    vmin = 0\n",
+                "    K = len(H)\n",
+                "    L = len(D)\n",
+                "    \n",
+                "    angles, true_inds = find_min_angle(Ddot.T, D.T, unique=True, get_ind=True)\n",
+                "    mse = ordered_mse(Hdotflat, Hflat, true_inds)\n",
+                "    mae = ordered_mae(Hdotflat, Hflat, true_inds)\n",
+                "    r2 = ordered_r2(Hdotflat, Hflat, true_inds)\n",
+                "\n",
+                "\n",
+                "    fig, axes = plt.subplots(K,3,figsize = (scale/K * 3 * aspect_ratio,scale))\n",
+                "    x = np.linspace(0,1, num = L)\n",
+                "    for i in range(K): \n",
+                "        axes[2,i].plot(x,Ddot.T[i,:],'g-',label='ground truth',linewidth=4)\n",
+                "        axes[2,i].plot(x,D[:,true_inds[i]],'r--',label='reconstructed',linewidth=4)\n",
+                "        axes[2,i].set_title(\"{:.2f} deg\".format(angles[i]),fontsize = fontsize-2)\n",
+                "        axes[2,i].set_xlim(0,1)\n",
+                "\n",
+                "        axes[1,i].imshow((Hflat[true_inds[i],:]).reshape(shape_2d),vmin = vmin, vmax = vmax , cmap=cmap)\n",
+                "        axes[1,i].set_title(\"R2: {:.2f}\".format(r2[true_inds[i]]),fontsize = fontsize-2)\n",
+                "        # axes[i,1].set_ylim(0.0,1.0)\n",
+                "        axes[1,i].tick_params(axis = \"both\",labelleft = False, labelbottom = False,left = False, bottom = False)\n",
+                "\n",
+                "        im = axes[0,i].imshow(Hdotflat[i].reshape(shape_2d),vmin = vmin, vmax = vmax, cmap=cmap)\n",
+                "        axes[0,i].set_title(\"Phase {}\".format(i),fontsize = fontsize)\n",
+                "        axes[0,i].tick_params(axis = \"both\",labelleft = False, labelbottom = False,left = False, bottom = False)\n",
+                "        axes[2,0].legend()\n",
+                "\n",
+                "    rows = [\"True maps\",\"Reconstructed maps\",\"Spectra\"]\n",
+                "\n",
+                "    for ax, row in zip(axes[:,0], rows):\n",
+                "        ax.set_ylabel(row, rotation=90, fontsize=fontsize)\n",
+                "\n",
+                "\n",
+                "    fig.subplots_adjust(right=0.84)\n",
+                "    # put colorbar at desire position\n",
+                "    cbar_ax = fig.add_axes([0.85, 0.5, 0.01, 0.3])\n",
+                "    fig.colorbar(im,cax=cbar_ax)\n",
+                "\n",
+                "    # fig.tight_layout()\n",
+                "\n",
+                "    print(\"angles : \", angles)\n",
+                "    print(\"mse : \", mse)\n",
+                "    print(\"mae : \", mae)\n",
+                "    print(\"r2 : \", r2)\n",
+                "\n",
+                "    return fig\n",
+                "\n",
+                "fig = plot_results(GW, GW_est, H, H_est)\n",
+                "plt.show()  \n"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3.7.6 64-bit ('teurtrie-Jj3N6OEN': pipenv)",
-            "metadata": {
-                "interpreter": {
-                    "hash": "f6679034cdacd370e2932d4f533870513ed60f8e3e5a021334854984182bfbf5"
-                }
-            },
+            "display_name": "espm",
+            "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.7.6"
+            "version": "3.10.6"
         },
-        "orig_nbformat": 2
+        "vscode": {
+            "interpreter": {
+                "hash": "8d9f0750808bbb89d6238996d547b1a0ab25cae94b245e8c4572708d26b443fd"
+            }
+        }
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 4
 }
```

### Comparing `espm-0.1.4/notebooks/old/analyze_data_v2.ipynb` & `espm-0.2.0/notebooks/preprocess_dataset.ipynb`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.959539573244552%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, '%matplotlib inline')], delete: [2]}}, 2: {'source': ['# "*

 * *            "Data preprocessing for the neural network\\n', '\\n', 'This notebook illustrate the "*

 * *            "data preprocessing steps to create the dataset']}, 3: {'source': ['# Input resolution "*

 * *            "of the panel\\n', 'res = 512']}, 4: {'source': ['### 1. Projection of the mesh "*

 * *            "distance onto a plane\\n', '\\n', 'Alternatively, run the script "*

 * *            "`panel_obj_to_mat.py`, w […]*

```diff
@@ -4,633 +4,642 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "%load_ext autoreload\n",
                 "%autoreload 2\n",
-                "%matplotlib qt"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "# Imports and utility functions"
+                "%matplotlib inline"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "\n",
-                "import matplotlib.pyplot as plt\n",
-                "import numpy as np\n",
-                "from snmfem.estimator.snmf import SNMF\n",
-                "from snmfem import EDXS_model\n",
-                "from snmfem.measures import find_min_angle, find_min_MSE, residuals\n",
-                "from snmfem.conf import DATASETS_PATH\n",
-                "from pathlib import Path\n",
-                "\n",
-                "# hyperspy is the commonly used library to handle spectrum images in the electron microscopy community\n",
-                "import hyperspy.api as hs\n"
+                "import logging\n",
+                "logging.basicConfig(level=logging.INFO)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Data Loading"
+                "# Data preprocessing for the neural network\n",
+                "\n",
+                "This notebook illustrate the data preprocessing steps to create the dataset"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "folder = DATASETS_PATH / Path(\"aspim037_N100_2ptcls_brstlg\")\n",
-                "sample_num = 1\n",
-                "\n",
-                "sample_filenames = list(folder.glob(\"*.npz\"))\n",
-                "print(\"Found {} samples\".format(len(sample_filenames)))\n",
-                "sample_filename = sample_filenames[sample_num]"
+                "# Input resolution of the panel\n",
+                "res = 512"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "# S=hs.load(filename+\".hspy\")\n",
-                "dat = np.load(sample_filename)\n",
-                "X = dat[\"X\"]\n",
-                "Xdot = dat[\"Xdot\"]\n",
-                "phases = dat[\"phases\"] \n",
-                "densities = dat[\"densities\"]\n",
-                "weights = dat[\"weights\"]\n",
-                "N = dat[\"N\"]\n",
-                "k = len(densities)\n",
+                "### 1. Projection of the mesh distance onto a plane\n",
                 "\n",
-                "S = hs.signals.Signal1D(X)\n",
-                "S.axes_manager[2].name=\"Energy\"\n",
-                "S.axes_manager[2].scale=0.01\n",
-                "S.axes_manager[2].offset=0.20805000000000007\n",
-                "S.axes_manager[2].unit=\"keV\"\n",
-                "\n",
-                "# # This part of the spectrum image contains only pure spectra from phase 0\n",
-                "# # This kind of area is often available in experimental datasets\n",
-                "X_part=S.inav[60:,:].data"
+                "Alternatively, run the script `panel_obj_to_mat.py`, which can execute this code in parallel."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "X.shape"
+                "import os\n",
+                "from ddad.ml.preprocess import get_panel_names, build_surface_from_name\n",
+                "from ddad.ml.path import data_path\n",
+                "import numpy as np\n",
+                "import matplotlib.pyplot as plt"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "X_part.shape"
+                "# Force the recomputation of the panel\n",
+                "rebuild = False"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
-                "plt.figure()\n",
-                "plt.imshow(np.mean(X, axis=2))\n",
-                "plt.colorbar()\n"
+                "names = get_panel_names()\n",
+                "path_data = os.path.join(data_path(\"processed\"), \"../panel_mat_{}\".format(res))\n",
+                "os.makedirs(path_data, exist_ok=True)\n",
+                "for name in names:\n",
+                "    print(\"Converting panel: {}\".format(name))\n",
+                "    try:\n",
+                "        outpath = os.path.join(path_data, name+\"_mat.npz\")\n",
+                "        if rebuild or not(os.path.exists(outpath)):\n",
+                "            if not rebuild:\n",
+                "                print(\"   Not availlable -> build\")\n",
+                "            surface = build_surface_from_name(name, res=res)\n",
+                "            if surface is not None:\n",
+                "                np.savez_compressed(outpath, surface=surface)\n",
+                "            else:\n",
+                "                print(\"Something went wrong...\")\n",
+                "        else:\n",
+                "            print(\"   Already availlable -> skip\")\n",
+                "    except Exception as _:\n",
+                "        import traceback\n",
+                "\n",
+                "        traceback.print_exc()\n",
+                "        print(\"Fail for panel {}\".format(name))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "plt.figure()\n",
-                "plt.hist(X.flatten(), 100)\n",
-                "plt.yscale(\"log\")"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "# Interactive plotting of the data"
+                "names = get_panel_names()\n",
+                "print(\"Found {} walls\".format(len(names)))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "roi=hs.roi.RectangularROI(12,12,24,24)\n",
-                "S.plot()\n",
-                "spim_ROI=roi.interactive(S)\n",
-                "    \n",
-                "sum_ROI=hs.interactive(spim_ROI.sum,\n",
-                "               event=spim_ROI.axes_manager.events.any_axis_changed,\n",
-                "               recompute_out_event=None)\n",
-                "sum_ROI.plot()"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "# Testing an NMF algorithm"
+                "path_data = os.path.join(data_path(\"processed\"), \"../panel_mat_{}\".format(res))\n",
+                "all_mat = []\n",
+                "names.sort()\n",
+                "for name in names:\n",
+                "    panel_path = os.path.join(path_data, name+\"_mat.npz\")\n",
+                "    all_mat.append(np.load(panel_path)[\"surface\"])\n",
+                "all_mat = np.array(all_mat)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "D = phases.T\n",
-                "A = weights.reshape(-1, 3).T\n",
-                "w = densities\n",
-                "W = np.diag(w)\n",
-                "Dp = N * D @ W\n",
-                "Xdot_m = Xdot.reshape(-1, 1980).T\n",
-                "X_m = X.reshape(-1, 1980).T\n",
-                "\n",
-                "np.testing.assert_allclose(Xdot_m, Dp @ A)\n",
-                "np.testing.assert_allclose(np.sum(A, axis=0), np.ones(A.shape[1]))\n"
+                "plt.hist(all_mat.flatten(),100);\n",
+                "plt.yscale(\"log\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from snmfem.estimator.nmf import NMF"
+                "from ddad.ml.plot import draw_images\n",
+                "vmax = np.max(all_mat)\n",
+                "vmin = - vmax\n",
+                "plt.figure(figsize=(30,30))\n",
+                "im = draw_images(all_mat, 15,15, cmap=plt.cm.seismic, vmin=vmin, vmax=vmax )\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from sklearn.decomposition import TruncatedSVD\n",
-                "from sklearn.decomposition import NMF\n",
-                "from sklearn.decomposition._nmf import _initialize_nmf as initialize_nmf "
+                "np.min(all_mat), np.max(all_mat)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# U,V = initialize_nmf(Xdot_m, k)"
+                "col = 13\n",
+                "line = 8\n",
+                "ind = (col-1)*15+line-1\n",
+                "vmax = np.max(all_mat)\n",
+                "vmin = - vmax\n",
+                "plt.figure(figsize=(8,8))\n",
+                "plt.imshow(all_mat[ind], cmap=plt.cm.seismic, vmin=vmin, vmax=vmax )\n",
+                "plt.title(names[ind])\n",
+                "plt.colorbar()"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "def truncated_SVD(X, k, algorithm='randomized', n_iter=5, **kwargs):\n",
-                "    \"\"\"Wrapper function to perform a truncated SVD.\n",
-                "    \n",
-                "    Returns U, V, e where X = U V and e is the explained variance ratio.\n",
-                "    \"\"\"\n",
-                "    tsvd = TruncatedSVD(n_components=k, algorithm=algorithm, n_iter=n_iter, **kwargs)\n",
-                "    U = tsvd.fit_transform(X)\n",
-                "    V = tsvd.components_\n",
-                "    e = tsvd.explained_variance_ratio_\n",
-                "    return U, V, e\n"
+                "### 2. Creating a dataset from (geometry, impulse) pairs"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "Xr = Xdot.reshape(-1, Xdot.shape[2])\n",
-                "Xr.shape"
+                "import os\n",
+                "import numpy as np\n",
+                "from ddad.ml.preprocess import build_dataset\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "U, V, e = truncated_SVD(Xr, k =k, n_iter=20)\n",
-                "np.testing.assert_allclose(np.sum(e),1)\n",
-                "np.testing.assert_allclose((U @ V), Xr)"
+                "use_time = False\n",
+                "use_chanels = True\n",
+                "plane = 0 # Select the closest plane 6x6\n",
+                "data_type=\"cummulative_energy\"\n",
+                "\n",
+                "# Name for our dataset\n",
+                "name_file = \"../data/data_{}_{}_{}_{}_{}.npz\".format(res, data_type, use_time, use_chanels, plane)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Parameters intialisation"
+                "#### Preprocess"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# True bremsstrahlung parameters\n",
-                "brstlg_pars = {\"c0\" : 4.8935e-05,\"c1\" : 1464.19810, \"c2\" : 0.04216872, \"b0\" : 0.15910789, \"b1\" : -0.00773158, \"b2\" : 8.7417e-04}\n",
+                "mats, samples, sel_names, sel_sources = build_dataset(res, data_type, use_time, use_chanels, plane)\n",
+                "np.savez_compressed(name_file, mats=mats, samples=samples, sel_names=sel_names, sel_sources=sel_sources)\n",
                 "\n",
-                "# SNMF parameters\n",
-                "tol = 1e-4\n",
-                "max_iter = 5000\n",
-                "b_tol = 1e-1\n",
-                "mu_sparse = 0.0\n",
-                "eps_sparse = 1.0\n",
-                "phases = 3\n",
-                "debug = True\n",
-                "\n",
-                "# # If mu_sparse !=0 a good initialization of the first phase is required, it can be done using the spectrum below\n",
-                "init_matrix=np.average(X_part,axis=(0,1))"
+                "del mats\n",
+                "del samples\n",
+                "del sel_names\n",
+                "del sel_sources"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "## Creating the EDXS model"
+                "# Test data loading\n",
+                "dat = np.load(name_file, allow_pickle=True)\n",
+                "samples = dat[\"samples\"]\n",
+                "mats = dat[\"mats\"]\n",
+                "sel_names = dat[\"sel_names\"]\n",
+                "sel_sources = dat[\"sel_sources\"]\n",
+                "sel_sources = [tuple(e) for e in sel_sources.tolist()]\n",
+                "\n",
+                "del dat"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "em = EDXS_model.EDXS_Model(\"Data/simple_xrays_threshold.json\",brstlg_pars = brstlg_pars,e_offset=S.axes_manager[2].offset,e_scale=S.axes_manager[2].scale,e_size=S.axes_manager[2].size)\n",
-                "em.generate_g_matr([8,13,14,12,26,29,31,72,71,62,60,92,20],brstlg = False) # If brstlg=False, it will learn the continum model, if brstlg=True it add a column in the G matrix using the parameters , "
+                "#### Preprocess for a different configuration"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "S.axes_manager[2].scale, "
+                "use_time = False\n",
+                "use_chanels = False\n",
+                "plane = 0 # Select the closest plane 6x6\n",
+                "data_type=\"cummulative_energy\"\n",
+                "\n",
+                "# Name for our dataset\n",
+                "name_file = \"../data/data_{}_{}_{}_{}_{}.npz\".format(res, data_type, use_time, use_chanels, plane)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "S.axes_manager[2].offset"
+                "mats, samples, sel_names, sel_sources = build_dataset(res, data_type, use_time, use_chanels, plane)\n",
+                "np.savez_compressed(name_file, mats=mats, samples=samples, sel_names=sel_names, sel_sources=sel_sources)\n",
+                "\n",
+                "del mats\n",
+                "del samples\n",
+                "del sel_names\n",
+                "del sel_sources"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "brstlg_pars"
+                "# Test data loading\n",
+                "dat = np.load(name_file, allow_pickle=True)\n",
+                "samples = dat[\"samples\"]\n",
+                "sel_names = dat[\"sel_names\"]\n",
+                "sel_sources = dat[\"sel_sources\"]\n",
+                "sel_sources = [tuple(e) for e in sel_sources.tolist()]\n",
+                "mats = dat[\"mats\"]\n",
+                "\n",
+                "del dat"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "em.g_matr.shape"
+                "### 3. Look at a sample"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "em.x"
+                "import matplotlib.pyplot as plt"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "## Loading the ground truth"
+                "sample = samples[0]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "true_spectra=[]\n",
-                "true_maps=[]\n",
-                "true_spectra.append(np.genfromtxt(filename+\"spectrum_p0\"))\n",
-                "true_spectra.append(np.genfromtxt(filename+\"spectrum_p1\"))\n",
-                "true_spectra.append(np.genfromtxt(filename+\"spectrum_p2\"))\n",
-                "true_maps.append(np.load(filename+\"map_p0.npy\"))\n",
-                "true_maps.append(np.load(filename+\"map_p1.npy\"))\n",
-                "true_maps.append(np.load(filename+\"map_p2.npy\"))\n",
-                "\n",
-                "true_spectra = np.array(true_spectra)\n",
-                "true_maps = np.array(true_maps)\n"
+                "# First part is the geometry input\n",
+                "plt.imshow(mats[sample[0]]);"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "true_maps.shape, true_spectra.shape"
+                "# Outputs, in this case the reflected energy\n",
+                "if use_chanels:\n",
+                "    plt.figure(figsize=(10, 6))\n",
+                "    for i in range(5):\n",
+                "        plt.subplot(2,3,i+1)\n",
+                "        plt.imshow(sample[1][:,i].reshape(6-plane, 6-plane))\n",
+                "        plt.colorbar()\n",
+                "else:\n",
+                "    plt.imshow(sample[1].reshape(6-plane, 6-plane))\n",
+                "    plt.colorbar()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "plt.figure(figsize=(10,10))\n",
-                "plt.subplot(221)\n",
-                "plt.plot(em.x, true_spectra.T);\n",
-                "plt.yscale(\"log\")\n",
-                "for i in range(3):\n",
-                "    plt.subplot(2,2,i+2)\n",
-                "    plt.imshow(true_maps[i])"
+                "# The mask used to tell which of the outputs should be used for the loss\n",
+                "plt.imshow(sample[2].reshape(6-plane, 6-plane))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
-            "source": []
+            "source": [
+                "# The mask indicating the position of the source (just the reverse of the previous element)\n",
+                "plt.imshow(sample[3].reshape(6-plane, 6-plane))"
+            ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Checking the loss of the ground truth\n",
-                "n_components = true_maps.shape[0]\n",
-                "im_size = true_maps.shape[1:]\n",
-                "\n",
-                "perfect_reconstruction = (true_maps.reshape(n_components,-1).T @ true_spectra ).reshape(*im_size, -1)\n",
-                "diff = perfect_reconstruction -X\n",
-                "np.std(diff)"
+                "sample[1].shape"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "plt.figure(figsize=(10,5))\n",
-                "plt.subplot(121)\n",
-                "plt.imshow(np.mean(perfect_reconstruction, axis=2))\n",
-                "plt.colorbar()\n",
-                "plt.subplot(122)\n",
-                "plt.imshow(np.mean(X, axis=2))\n",
-                "plt.colorbar()\n"
+                "## 4. Creating dataset for alternative problems"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# SNMF\n",
-                "\n",
-                "## Initialize the algorithm"
+                "Object classification and interpolation from IR"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "mdl = SNMF(max_iter = max_iter, tol = tol, b_tol = b_tol, mu_sparse=mu_sparse, eps_sparse = eps_sparse, num_phases=phases,edxs_model=em, brstlg_pars = brstlg_pars, init_spectrum = init_matrix, debug=debug)"
+                "from ddad.ml.preprocess import get_panel_names\n",
+                "from ddad.dataset import PanelData\n",
+                "import matplotlib.pyplot as plt\n",
+                "import numpy as np\n",
+                "from ddad.ml.path import \n",
+                "\n"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "## Running the algorithm"
+                "from ddad.grid import Grid\n",
+                "from ddad.config import GRID_FILE\n",
+                "grid = Grid.from_json(GRID_FILE)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "scrolled": true
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "mdl.fit(X,eval_print=50, flush=False)"
+                "cells_source_reciever = [grid.cells_from_index(i) for i in range(2951)]\n",
+                "cells = np.array(cells_source_reciever).reshape(-1, 3).tolist()\n",
+                "cells = set([tuple(c) for c in cells])\n",
+                "positions = np.array([np.array(grid.position(c)) for c in cells])\n",
+                "mp = np.median(positions, axis=0)\n",
+                "sp = 125\n",
+                "positions = (positions - mp) / sp\n",
+                "cells2positions = {c:p for c,p in zip(cells, positions)}\n",
+                "positions_source_reciever = np.array([ np.array([cells2positions[c1], cells2positions[c2] ]) for c1, c2 in cells_source_reciever])\n",
+                "# positions_source_reciever"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# from time import sleep\n",
-                "# for i in range(10):\n",
-                "#     print(f\"\\r {i}\", end=\"\", flush=True)\n",
-                "#     sleep(0.1)\n"
+                "# for name in get_panel_names():\n",
+                "\n",
+                "lt = 256\n",
+                "\n",
+                "name_file = os.path.join(data_path(), \"../data_classification_{}.npz\".format(lt))\n",
+                "\n",
+                "names = get_panel_names()\n",
+                "\n",
+                "samples = []\n",
+                "labels = []\n",
+                "# srs = []\n",
+                "\n",
+                "for i, name in enumerate(names):\n",
+                "\n",
+                "    p = PanelData(name)\n",
+                "    samples.append(p.matrix_after_direct_sound_removal[:,:256])\n",
+                "    labels.append(i * np.ones(2951).astype(int))\n",
+                "    srs.append(positions_source_reciever)\n",
+                "labels = np.concatenate(labels)\n",
+                "samples = np.concatenate(samples)\n",
+                "srs = np.concatenate(srs)\n",
+                "\n",
+                "np.savez(name_file, labels=labels, samples=samples, names=names)\n",
+                "\n"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "# Results\n",
-                "\n",
-                "## Comparison with ground truth"
+                "samples.shape, labels.shape, len(names)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Returns the angles between the ground truth and the endmembers found using SNMF\n",
-                "angles=find_min_angle(true_spectra,[mdl.get_phase_spectrum(0),mdl.get_phase_spectrum(1),mdl.get_phase_spectrum(2)])\n",
+                "name_file = os.path.join(data_path(), \"../data_interpolation_{}.npz\".format(lt))\n",
                 "\n",
-                "maps=find_min_MSE(true_maps,[mdl.get_phase_map(0),mdl.get_phase_map(1),mdl.get_phase_map(2)])\n",
-                "\n",
-                "print(\"Angle phase 0 :\",angles[0])\n",
-                "print(\"Angle phase 1 :\",angles[1])\n",
-                "print(\"Angle phase 2 :\",angles[2])\n",
-                "print(\"MSE phase 0 :\",maps[0])\n",
-                "print(\"MSE phase 1 :\",maps[1])\n",
-                "print(\"MSE phase 2 :\",maps[2])"
+                "np.savez(name_file, srs=srs, cells2positions=cells2positions, \n",
+                "         cells_source_reciever=cells_source_reciever, samples=samples, names=names,\n",
+                "         mp=mp, sp=sp, positions_source_reciever=positions_source_reciever)\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Visualisation of the results \n",
-                "\n",
-                "### Matching endmembers and ground truth"
+                "## 5. Check reprinted panels"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# switch is the index of the endmember (0 to 2)\n",
-                "switch = 1\n",
-                "# true is the index of the ground truth (0 to 2)\n",
-                "true=1"
+                "names = get_panel_names()\n",
+                "print(\"Found {} walls\".format(len(names)))"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "## Endmember + abundance plot"
+                "for name in names:\n",
+                "    if \"reprint\" in name:\n",
+                "        try:\n",
+                "            parts = name.split(\"reprint\")\n",
+                "            name1 = parts[0] + parts[1]        \n",
+                "            name2 = name\n",
+                "            out1 = np.array([s[1] for s  in samples[sel_names==name1]])\n",
+                "            print(name1, out1.shape)\n",
+                "            out2 = np.array([s[1] for s  in samples[sel_names==name2]])\n",
+                "            print(name2, out2.shape)\n",
+                "            print(np.linalg.norm((out1-out2).flatten())/np.linalg.norm(out1))\n",
+                "        except:\n",
+                "            pass"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "plt.rcParams.update({'font.size': 22})\n",
-                "fig1 = plt.figure(figsize=(20, 12))\n",
-                "plt.subplot(121)\n",
-                "plt.plot(em.x,100*true_spectra[true]/np.sum(true_spectra[true]),'bo',label='truth',linewidth=4)\n",
-                "plt.plot(em.x, mdl.get_phase_spectrum(switch),'r-',label='reconstructed',markersize=3.5)\n",
-                "plt.legend(loc='best')\n",
-                "plt.xlim(0, 10)\n",
-                "plt.ylim(0,1)\n",
-                "plt.ylabel(\"Intensity\")\n",
-                "\n",
-                "plt.subplot(122)\n",
-                "plt.imshow(mdl.get_phase_map(switch), cmap=\"viridis\")\n",
-                "plt.grid(b=30)\n",
-                "plt.title(f\"Activations of first spectrum\")\n",
-                "plt.colorbar()\n",
-                "plt.clim(0, 1)\n",
-                "\n",
-                "fig1.tight_layout()"
+                "for name in names:\n",
+                "    if \"reprint\" in name:\n",
+                "        try:\n",
+                "            parts = name.split(\"reprint\")\n",
+                "            name1 = parts[0] + parts[1]        \n",
+                "            name2 = name\n",
+                "            out1 = PanelData(name1).total_energy_bands_normalized.flatten()\n",
+                "            out2 = PanelData(name2).total_energy_bands_normalized.flatten()\n",
+                "            print(\"Rel error between {} and {} : {}\".format(name1, name2, np.linalg.norm((out1-out2).flatten())/np.linalg.norm(out1)))\n",
+                "        except:\n",
+                "            pass"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "## Plotting the convergence\n",
-                "\n",
-                "### Losses"
+                "for name in names:\n",
+                "    if \"reprint\" in name:\n",
+                "        try:\n",
+                "            parts = name.split(\"reprint\")\n",
+                "            name1 = parts[0] + parts[1]        \n",
+                "            name2 = name\n",
+                "            out1 = PanelData(name1).flat.total_energy_bands_normalized.flatten()\n",
+                "            out2 = PanelData(name2).flat.total_energy_bands_normalized.flatten()\n",
+                "            print(\"Rel error between flat for {} and flat for {} : {}\".format(name1, name2, np.linalg.norm((out1-out2).flatten())/np.linalg.norm(out1)))\n",
+                "        except:\n",
+                "            pass"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "fig, (ax1, ax2) = plt.subplots(2, 1)\n",
-                "ax1.plot(mdl.base_losses)\n",
-                "ax1.set_title(\"base loss\",fontsize=24)\n",
-                "ax1.set_xticks([])\n",
-                "ax2.plot(mdl.losses)\n",
-                "ax2.set_title(\"full loss\",fontsize=24)\n",
-                "ax2.set_xlabel(\"number of iterations\",fontsize=20)"
+                "from ddad.dataset import PanelData"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "### B parameters step sizes"
+                "name1 = \"panel_0003_1\"\n",
+                "name2 = \"panel_0003reprint_1\"\n",
+                "# name1 = \"panel_0002_1\"\n",
+                "# name2 = \"panel_0002reprint_1\"\n",
+                "p1 = PanelData(name1)\n",
+                "p2 = PanelData(name2)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "fig, (ax1, ax2, ax3, ax4, ax5) = plt.subplots(5, 1)\n",
-                "ax1.plot(np.array(mdl.eta_list)[:,0])\n",
-                "ax1.set_title(\"step size b1\",fontsize=18)\n",
-                "ax1.set_xticks([])\n",
-                "ax2.plot(np.array(mdl.eta_list)[:,1])\n",
-                "ax2.set_title(\"step size b2\",fontsize=18)\n",
-                "ax2.set_xticks([])\n",
-                "ax3.plot(np.array(mdl.eta_list)[:,2])\n",
-                "ax3.set_title(\"step size c0\",fontsize=18)\n",
-                "ax3.set_xticks([])\n",
-                "ax4.plot(np.array(mdl.eta_list)[:,3])\n",
-                "ax4.set_title(\"step size c1\",fontsize=18)\n",
-                "ax4.set_xticks([])\n",
-                "ax5.plot(np.array(mdl.eta_list)[:,4])\n",
-                "ax5.set_title(\"step size c2\",fontsize=18)\n",
-                "ax5.set_xlabel(\"number of iterations\",fontsize=16)"
+                "p1.print_panel_info() \n",
+                "p2.print_panel_info() "
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
+            "source": [
+                "index = 200"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
             "source": [
-                "### A, P and B norms"
+                "plt.plot(p1.matrix_after_direct_sound_removal[index], label =name1)\n",
+                "plt.plot(p2.matrix_after_direct_sound_removal[index], label =name2)\n",
+                "plt.legend()\n",
+                "# plt.xlim([20, 150])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "fig, (ax1, ax2, ax3) = plt.subplots(3, 1)\n",
-                "ax1.plot(mdl.a_norm)\n",
-                "ax1.set_title(\"A norm\",fontsize=18)\n",
-                "ax1.set_xticks([])\n",
-                "ax2.plot(mdl.p_norm)\n",
-                "ax2.set_title(\"P norm\",fontsize=18)\n",
-                "ax2.set_xticks([])\n",
-                "ax3.plot(mdl.b_norm)\n",
-                "ax3.set_title(\"B norm\",fontsize=18)\n",
-                "ax3.set_xlabel(\"number of iterations\",fontsize=16)"
+                "plt.plot(np.mean(p1.matrix_after_direct_sound_removal, axis=0), label =name1)\n",
+                "plt.plot(np.mean(p2.matrix_after_direct_sound_removal, axis=0), label =name2)\n",
+                "plt.legend()\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -649,13 +658,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.6-final"
+            "version": "3.8.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `espm-0.1.4/notebooks/old/generate_artificial_data.ipynb` & `espm-0.2.0/notebooks/other_algorithms.ipynb`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7420454545454546%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, '%matplotlib inline\\n'), (3, 'import hyperspy.api as "*

 * *            "hs\\n'), (4, 'import matplotlib.pyplot as plt\\n'), (5, 'import numpy as np\\n'), (6, "*

 * *            "'from espm.conf import DATASETS_PATH\\n'), (7, 'from pathlib import Path\\n'), (8, "*

 * *            "'from espm.measures import find_min_angle, find_min_MSE, ordered_mse\\n'), (9, 'from "*

 * *            "espm.utils import rescaled_DH')], delete: [2]}}, 1: {'source': ['dataset_path = "*

 * *            'DATASET […]*

```diff
@@ -1,374 +1,243 @@
 {
     "cells": [
         {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "# Imports"
-            ]
-        },
-        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "%load_ext autoreload\n",
                 "%autoreload 2\n",
-                "%matplotlib inline"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "# %matplotlib qt\n",
-                "import snmfem.generate_data as gd\n",
-                "from snmfem.models import EDXS\n",
-                "import numpy as np\n",
+                "%matplotlib inline\n",
                 "import hyperspy.api as hs\n",
                 "import matplotlib.pyplot as plt\n",
-                "from snmfem.conf import DB_PATH"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "# Parameters"
+                "import numpy as np\n",
+                "from espm.conf import DATASETS_PATH\n",
+                "from pathlib import Path\n",
+                "from espm.measures import find_min_angle, find_min_MSE, ordered_mse\n",
+                "from espm.utils import rescaled_DH"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# To save the dataset\n",
-                "filename = \"aspim037_N100_2ptcls_brstlg\"\n",
-                "abs_db_path = None\n",
-                "# abs_db_path = \"Data/wernisch_abs.json\"\n",
-                "abs_elt_dict = None\n",
-                "\n",
-                "# Continuum X-rays parameters\n",
-                "# They were determine by fitting experimental data from 0.6 to 18 keV. Since low energies were incorporated, the model is only effective and not quantitative. \n",
-                "brstlg_pars = {\"c0\" : 0.094, \"c1\" : 1417, \"c2\" : 1e-6, \"b0\" : 1.2, \"b1\" : -0.06, \"b2\" : 0.00683}\n",
-                "\n",
-                "# brstlg_pars = {\"c0\" : 9.3144e-04,\"c1\" : 1.23453632, \"c2\" : 4.9488e-10, \"b0\" : 0.14986191, \"b1\" : -0.00188483, \"b2\" : 2.5428e-04}\n",
-                "\n",
-                "\n",
-                "scale = 1\n",
-                "\n",
-                "# Average number of counts in one spectrum of the artificial data\n",
-                "N = 100 \n",
-                "\n",
-                "# Creation of the pure spectra of the different phases.\n",
-                "phase1 = EDXS(DB_PATH,abs_db_path,brstlg_pars)\n",
-                "#phase1.generate_abs_coeff({\"8\":1.0,\"12\" : 0.51,\"14\":0.61,\"13\":0.07,\"20\":0.04,\"62\":0.02,\"26\":0.028,\"60\":0.002,\"71\":0.003,\"72\":0.003,\"29\" : 0.02})\n",
-                "# Gaussians corresponding to elements\n",
-                "phase1.generate_spectrum({\"8\":1.0,\"12\" : 0.51,\"14\":0.61,\"13\":0.07,\"20\":0.04,\"62\":0.02,\"26\":0.028,\"60\":0.002,\"71\":0.003,\"72\":0.003,\"29\" : 0.02},scale)\n",
-                "\n",
-                "phase2 = EDXS(DB_PATH,abs_db_path,brstlg_pars)\n",
-                "#phase2.generate_abs_coeff({\"8\":0.54,\"26\":0.15,\"12\" : 1.0,\"29\":0.038,\"92\":0.0052,\"60\":0.004,\"31\":0.03,\"71\":0.003})\n",
-                "phase2.generate_spectrum({\"8\":0.54,\"26\":0.15,\"12\" : 1.0,\"29\":0.038,\"92\":0.0052,\"60\":0.004,\"31\":0.03,\"71\":0.003},scale)\n",
-                "\n",
-                "phase3 = EDXS(DB_PATH,abs_db_path,brstlg_pars)\n",
-                "#phase3.generate_abs_coeff({\"8\":1.0,\"14\":0.12,\"13\":0.18,\"20\":0.47,\"62\":0.04,\"26\":0.004,\"60\":0.008,\"72\":0.004,\"29\":0.01})\n",
-                "phase3.generate_spectrum({\"8\":1.0,\"14\":0.12,\"13\":0.18,\"20\":0.47,\"62\":0.04,\"26\":0.004,\"60\":0.008,\"72\":0.004,\"29\":0.01},scale)\n",
+                "dataset_path = DATASETS_PATH / Path(\"FpBrgCaPv_N293_paper/sample_1.hspy\")\n",
+                "true_spim = hs.load(str(dataset_path))\n",
+                "true_spectra = true_spim.phases\n",
+                "true_maps = true_spim.maps\n",
+                "k = len(true_spim.metadata.Truth.phases)\n",
+                "shape_2d = true_spim.shape_2d\n",
                 "\n",
-                "# Objects needed for the creation of data\n",
-                "# list of spectra\n",
-                "phases = np.array([phase1.spectrum,phase2.spectrum,phase3.spectrum])\n",
-                "# list of densities which will give different total number of events per spectra\n",
-                "densities = np.array([1.0,1.33,1.25])"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "phases.shape"
+                "fontsize = 30\n",
+                "scale = 15\n",
+                "aspect_ratio = 1.4\n",
+                "marker_list = [\"-o\",\"-s\",\"->\",\"-<\",\"-^\",\"-v\",\"-d\"]\n",
+                "mark_space = 20"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Artificial data creation\n",
-                "\n",
-                "Note : Each function of ArtificialSpim updates the current object and adds on top. It is usually better to re-create a new object to change the artificial data settings.\n",
-                "Spim corresponds to spectrum image."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "# Creation of an ArtificialSpim instance\n",
-                "spim=gd.AritificialSpim(phases,densities,(80,80))\n",
-                "assert(spim.phases.shape==(3, 1980))\n",
-                "assert(spim.densities.shape==(3,))"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "np.testing.assert_allclose(np.sum(spim.phases, axis=1), np.ones([3]))"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "# We add two particles belonging to two different phases to the data\n",
-                "spim.sphere((25,30),3.5,3.5,0.0,0.5,1)\n",
-                "spim.sphere((55,30),3.5,3.5,0.0,0.5,2)"
+                "# NMF"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Generates a noiseless version of the dataset\n",
-                "spim.generate_spim_deterministic()\n",
-                "assert(spim.generated_spim.shape==(80, 80, 1980))"
+                "true_spim.decomposition(False,algorithm = \"NMF\", max_iter = 200000, tol = 1e-9, solver = \"mu\", beta_loss = \"kullback-leibler\", verbose = True, output_dimension = 3, init = \"random\", random_state = 52)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "np.testing.assert_allclose(np.sum(spim.generated_spim, axis=2), np.ones([80,80]))"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "D = spim.phases.T\n",
-                "A = spim.weights.reshape(-1, 3).T\n",
-                "X = spim.generated_spim.reshape(-1, 1980).T\n",
-                "np.testing.assert_allclose(D@A, X)"
+                "factors = true_spim.get_decomposition_factors().data.T\n",
+                "loadings = true_spim.get_decomposition_loadings().data.reshape((3,16384))\n",
+                "\n",
+                "r_factors, r_loadings = rescaled_DH(factors,loadings)"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "plt.figure(figsize=(15, 4))\n",
-                "for i in range(3):\n",
-                "    plt.subplot(1,3,i+1)\n",
-                "    plt.imshow(spim.weights[:,:,i], vmin=0, vmax=1)\n",
-                "    plt.colorbar()"
+                "# ICA"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Generate noisy spectra based on a Poisson distribution with average N\n",
-                "spim.generate_spim_stochastic(N)"
+                "true_spim.decomposition(True,output_dimension = 3,random_state = 42)\n",
+                "true_spim.blind_source_separation(number_of_components=3,tol = 1e-9)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# plt.imshow(spim.density_map)\n",
-                "# plt.colorbar()"
+                "factors = true_spim.get_bss_factors().data.T\n",
+                "loadings = true_spim.get_bss_loadings().data.reshape((3,16384))\n",
+                "\n",
+                "r_factors, r_loadings = rescaled_DH(factors,loadings)"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "assert(spim.continuous_spim.shape==(80, 80, 1980))"
+                "# VCA"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "D = spim.phases.T\n",
-                "A = spim.weights.reshape(-1, 3).T\n",
-                "w = spim.densities\n",
-                "Xdot = spim.continuous_spim.reshape(-1, 1980).T\n",
-                "# n D W A\n",
-                "np.testing.assert_allclose(N*D@np.diag(w)@A, Xdot)"
+                "from VCA import vca\n",
+                "from sunsal import sunsal\n",
+                "\n",
+                "r_factors, a, b = vca(true_spim.X, 3)\n",
+                "r_loadings, c, d, e = sunsal(r_factors,true_spim.X,positivity=True, addone = True, tol = 1e-9) "
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "spim.densities"
+                "# MCRLLM"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# ns = [10, 30, 100, 300, 1000, 3000, 10000, 30000]\n",
-                "# rels = []\n",
-                "# for n in ns:\n",
-                "#     spim.generate_spim_stochastic(n)\n",
-                "#     Xhat = spim.continuous_spim\n",
-                "#     Xtilde = spim.stochastic_spim\n",
-                "#     r = np.linalg.norm((Xhat-Xtilde).flatten())/np.sqrt(np.linalg.norm(Xhat.flatten())*np.linalg.norm(Xtilde.flatten()))\n",
-                "#     print(\"For {}, the relative error is: {}\".format(n, r))\n",
-                "#     rels.append(r)"
+                "from snmfem.estimators.mcrllm_wrapper import MCRLLM\n",
+                "\n",
+                "estimator = MCRLLM(n_components=3, init=\"Kmeans\", tol = 1e-4, max_iter=20000,hspy_comp=True)\n",
+                "\n",
+                "true_spim.decomposition(algorithm=estimator,verbose=True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Generate noisy spectra based on a Poisson distribution with average N\n",
-                "spim.generate_spim_stochastic(N, old=True)\n",
-                "Xhat2 = spim.continuous_spim\n",
-                "spim.generate_spim_stochastic(N, old=False)\n",
-                "Xhat = spim.continuous_spim"
+                "factors = true_spim.get_decomposition_factors().data.T\n",
+                "loadings = true_spim.get_decomposition_loadings().data.reshape((3,16384))\n",
+                "\n",
+                "r_factors, r_loadings = rescaled_DA(factors,loadings)"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "np.linalg.norm((Xhat-Xhat2).flatten())/np.sqrt(np.linalg.norm(Xhat.flatten())*np.linalg.norm(Xhat2.flatten()))"
+                "# Results"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "spim.generate_spim_stochastic(N, old=False)\n",
-                "Xhat = spim.continuous_spim\n",
-                "# To save the data and the ground truth under similar names\n",
-                "spim.save(filename)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "# Data visualisation"
+                "angles, true_inds = find_min_angle(true_spectra.T, r_factors.T, unique=True, get_ind=True)\n",
+                "mse = ordered_mse(true_maps, r_loadings, true_inds)\n",
+                "\n",
+                "print(\"angles : \", angles)\n",
+                "print(\"mse : \", mse)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# To visualise the pure spectrum of the first phase\n",
-                "x = phase1.x\n",
-                "plt.plot(x,phases[2],\"g-\",linewidth=2)\n",
-                "plt.plot(x,phase1.continuum_xrays()*scale)\n",
-                "plt.xlabel(\"Energy [keV]\")\n",
-                "plt.ylabel(\"Intensity\")\n",
-                "plt.rcParams.update({'font.size': 22})\n",
-                "plt.tight_layout()"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## Interactive visualization of the created datacube\n",
+                "fig, axes = plt.subplots(k,3,figsize = (scale/k * 3 * aspect_ratio,scale))\n",
+                "x = np.linspace(true_spim.axes_manager[2].offset,\n",
+                "                true_spim.axes_manager[2].offset + true_spim.axes_manager[2].scale * true_spim.axes_manager[2].size,\n",
+                "                num = true_spim.axes_manager[2].size)\n",
+                "for i in range(k): \n",
+                "    axes[2,i].plot(x,true_spectra.T[i,:],'bo',label='truth',linewidth=4)\n",
+                "    axes[2,i].plot(x,r_factors[:,true_inds[i]],'r-',label='reconstructed',markersize=3.5)\n",
+                "    axes[2,i].set_title(\"{:.2f} deg\".format(angles[i]),fontsize = fontsize-2)\n",
+                "    axes[2,i].set_xlim(0,10.0)\n",
                 "\n",
-                "3 windows will pop : \n",
+                "    axes[1,i].imshow((r_loadings[true_inds[i],:]).reshape(shape_2d),vmin = 0.0, vmax = 1.0 )\n",
+                "    axes[1,i].set_title(\"{:.2f} MSE\".format(mse[true_inds[i]]),fontsize = fontsize-2)\n",
+                "    # axes[i,1].set_ylim(0.0,1.0)\n",
+                "    axes[1,i].tick_params(axis = \"both\",labelleft = False, labelbottom = False,left = False, bottom = False)\n",
                 "\n",
-                "1) Map of the sum of counts per pixel - A very tiny green square will be plotted as well at the top left\n",
+                "    im = axes[0,i].imshow(true_maps[i].reshape(shape_2d),vmin = 0.0, vmax = 1.0)\n",
+                "    axes[0,i].set_title(\"Phase {}\".format(i),fontsize = fontsize)\n",
+                "    axes[0,i].tick_params(axis = \"both\",labelleft = False, labelbottom = False,left = False, bottom = False)\n",
+                "    axes[2,0].legend()\n",
                 "\n",
-                "2) Spectrum of the top left corner pixel (hyperspy built-in)\n",
+                "rows = [\"True maps\",\"Reconstructed maps\",\"Spectra\"]\n",
                 "\n",
-                "3) Sum of spectra of the green area in 1)\n",
+                "for ax, row in zip(axes[:,0], rows):\n",
+                "    ax.set_ylabel(row, rotation=90, fontsize=fontsize)\n",
                 "\n",
-                "It possible to move and reshape the green area in 1) to explore the data"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "signal=hs.signals.Signal1D(spim.stochastic_spim)\n",
-                "roi=hs.roi.RectangularROI(12,12,24,24)\n",
-                "signal.plot()\n",
-                "spim_ROI=roi.interactive(signal)\n",
-                "    \n",
-                "sum_ROI=hs.interactive(spim_ROI.sum,\n",
-                "               event=spim_ROI.axes_manager.events.any_axis_changed,\n",
-                "               recompute_out_event=None)\n",
-                "sum_ROI.plot()"
+                "\n",
+                "fig.subplots_adjust(right=0.84)\n",
+                "# put colorbar at desire position\n",
+                "cbar_ax = fig.add_axes([0.85, 0.5, 0.01, 0.3])\n",
+                "fig.colorbar(im,cax=cbar_ax)\n",
+                "\n",
+                "# fig.tight_layout()\n",
+                "\n",
+                "plt.show()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
+        "interpreter": {
+            "hash": "af6160b2371d66f432113418f198c66756233694b27723985e6f75953dadfe90"
+        },
         "kernelspec": {
-            "display_name": "Python 3",
-            "language": "python",
+            "display_name": "Python 3.8.5 64-bit ('SNMF_EDXS--pNpjmq1': pipenv)",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.5-final"
-        },
-        "orig_nbformat": 2
+            "version": "3.8.5"
+        }
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 4
 }
```

### Comparing `espm-0.1.4/notebooks/select_spectrum.ipynb` & `espm-0.2.0/notebooks/select_spectrum.ipynb`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/notebooks/simple-test-regularisation.ipynb` & `espm-0.2.0/notebooks/simple-test-regularisation.ipynb`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/notebooks/spectrum_fit.ipynb` & `espm-0.2.0/notebooks/spectrum_fit.ipynb`

 * *Files identical despite different names*

### Comparing `espm-0.1.4/setup.py` & `espm-0.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='espm',
-    version='0.1.4',
+    version='0.2.0',
     description='Electron SPectro-Microscopy Python Library',
     url='https://github.com/adriente/espm',
     author='Adrien Teurtie, Nathanael Perraudin',
     author_email='nathanael.perraudin@sdsc.ethz.ch',
     license='MIT',
     packages=setuptools.find_packages(),
     zip_safe=False,
```

