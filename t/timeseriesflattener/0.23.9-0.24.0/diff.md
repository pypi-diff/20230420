# Comparing `tmp/timeseriesflattener-0.23.9.tar.gz` & `tmp/timeseriesflattener-0.24.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeseriesflattener-0.23.9.tar", last modified: Tue Mar 28 12:12:58 2023, max compression
+gzip compressed data, was "timeseriesflattener-0.24.0.tar", last modified: Thu Apr 20 09:05:05 2023, max compression
```

## Comparing `timeseriesflattener-0.23.9.tar` & `timeseriesflattener-0.24.0.tar`

### file list

```diff
@@ -1,123 +1,130 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 12:12:58.053123 timeseriesflattener-0.23.9/
--rw-r--r--   0 root         (0) root         (0)      140 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/.codespellrc
--rw-r--r--   0 root         (0) root         (0)      123 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/.flake8
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 12:12:58.029122 timeseriesflattener-0.23.9/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 12:12:58.025123 timeseriesflattener-0.23.9/.github/actions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 12:12:58.029122 timeseriesflattener-0.23.9/.github/actions/test/
--rw-r--r--   0 root         (0) root         (0)     1044 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/.github/actions/test/action.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 12:12:58.029122 timeseriesflattener-0.23.9/.github/actions/test_tutorials/
--rw-r--r--   0 root         (0) root         (0)      994 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/.github/actions/test_tutorials/action.yml
--rw-r--r--   0 root         (0) root         (0)      722 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/.github/dependabot.yml
--rw-r--r--   0 root         (0) root         (0)      252 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/.github/pull_request_template.md
--rw-r--r--   0 root         (0) root         (0)      465 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/.github/setup_ci.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 12:12:58.029122 timeseriesflattener-0.23.9/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      849 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)     1148 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)      727 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/.github/workflows/generate_paper_pdf.yml
--rw-r--r--   0 root         (0) root         (0)     2446 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/.github/workflows/main_test_and_release.yml
--rw-r--r--   0 root         (0) root         (0)      463 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/.github/workflows/pre-commit.yml
--rw-r--r--   0 root         (0) root         (0)     2859 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/.gitignore
--rw-r--r--   0 root         (0) root         (0)      664 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)     1286 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/.zenodo.json
--rw-r--r--   0 root         (0) root         (0)    50991 2023-03-28 12:12:48.000000 timeseriesflattener-0.23.9/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     5238 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     4474 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     1087 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)    10062 2023-03-28 12:12:58.053123 timeseriesflattener-0.23.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9185 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/README.md
--rw-r--r--   0 root         (0) root         (0)      658 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/citation.cff
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 12:12:58.029122 timeseriesflattener-0.23.9/docs/
--rw-r--r--   0 root         (0) root         (0)      633 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 12:12:58.029122 timeseriesflattener-0.23.9/docs/_static/
--rw-r--r--   0 root         (0) root         (0)    15406 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/docs/_static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    49714 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)    49714 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/docs/_static/icon_dark.png
--rw-r--r--   0 root         (0) root         (0)   811066 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/docs/_static/terminology_figure.png
--rw-r--r--   0 root         (0) root         (0)     4211 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     2056 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)      320 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/docs/feature_specifications.rst
--rw-r--r--   0 root         (0) root         (0)     5280 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      299 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)      312 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/docs/timeseriesflattener.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 12:12:58.033123 timeseriesflattener-0.23.9/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)   130812 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/docs/tutorials/01_basic.ipynb
--rw-r--r--   0 root         (0) root         (0)    59662 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/docs/tutorials/02_advanced.ipynb
--rw-r--r--   0 root         (0) root         (0)    77800 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/docs/tutorials/03_text.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 12:12:58.033123 timeseriesflattener-0.23.9/docs/tutorials/img/
--rw-r--r--   0 root         (0) root         (0)    78953 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/docs/tutorials/img/term_a.png
--rw-r--r--   0 root         (0) root         (0)   109486 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/docs/tutorials/img/term_b.png
--rw-r--r--   0 root         (0) root         (0)   107613 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/docs/tutorials/img/term_c.png
--rw-r--r--   0 root         (0) root         (0)   250306 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/docs/tutorials/img/term_d.png
--rw-r--r--   0 root         (0) root         (0)      370 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/docs/tutorials.rst
--rw-r--r--   0 root         (0) root         (0)    49714 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 12:12:58.033123 timeseriesflattener-0.23.9/paper/
--rw-r--r--   0 root         (0) root         (0)    14392 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/paper/paper.bib
--rw-r--r--   0 root         (0) root         (0)     9434 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/paper/paper.md
--rw-r--r--   0 root         (0) root         (0)     3584 2023-03-28 12:12:48.000000 timeseriesflattener-0.23.9/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-28 12:12:58.057123 timeseriesflattener-0.23.9/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 12:12:58.025123 timeseriesflattener-0.23.9/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 12:12:58.037123 timeseriesflattener-0.23.9/src/timeseriesflattener/
--rw-r--r--   0 root         (0) root         (0)      226 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/src/timeseriesflattener/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5138 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/src/timeseriesflattener/column_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 12:12:58.037123 timeseriesflattener-0.23.9/src/timeseriesflattener/feature_cache/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/src/timeseriesflattener/feature_cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1971 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/src/timeseriesflattener/feature_cache/abstract_feature_cache.py
--rw-r--r--   0 root         (0) root         (0)     6097 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/src/timeseriesflattener/feature_cache/cache_to_disk.py
--rw-r--r--   0 root         (0) root         (0)    39388 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/src/timeseriesflattener/feature_spec_objects.py
--rw-r--r--   0 root         (0) root         (0)    36824 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/src/timeseriesflattener/flattened_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2266 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/src/timeseriesflattener/flattened_ds_validator.py
--rw-r--r--   0 root         (0) root         (0)     2160 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/src/timeseriesflattener/logger.py
--rw-r--r--   0 root         (0) root         (0)     3698 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/src/timeseriesflattener/resolve_multiple_functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 12:12:58.037123 timeseriesflattener-0.23.9/src/timeseriesflattener/testing/
--rw-r--r--   0 root         (0) root         (0)     3168 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/src/timeseriesflattener/testing/load_synth_data.py
--rw-r--r--   0 root         (0) root         (0)     1416 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/src/timeseriesflattener/testing/text_embedding_functions.py
--rw-r--r--   0 root         (0) root         (0)     5291 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/src/timeseriesflattener/testing/utils_for_testing.py
--rw-r--r--   0 root         (0) root         (0)     2342 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/src/timeseriesflattener/text_embedding_functions.py
--rw-r--r--   0 root         (0) root         (0)     7710 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/src/timeseriesflattener/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 12:12:58.037123 timeseriesflattener-0.23.9/src/timeseriesflattener.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10062 2023-03-28 12:12:57.000000 timeseriesflattener-0.23.9/src/timeseriesflattener.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3659 2023-03-28 12:12:58.000000 timeseriesflattener-0.23.9/src/timeseriesflattener.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-28 12:12:57.000000 timeseriesflattener-0.23.9/src/timeseriesflattener.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      747 2023-03-28 12:12:57.000000 timeseriesflattener-0.23.9/src/timeseriesflattener.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-03-28 12:12:57.000000 timeseriesflattener-0.23.9/src/timeseriesflattener.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 12:12:58.037123 timeseriesflattener-0.23.9/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 12:12:58.025123 timeseriesflattener-0.23.9/tests/test_data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 12:12:58.025123 timeseriesflattener-0.23.9/tests/test_data/flattened/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 12:12:58.037123 timeseriesflattener-0.23.9/tests/test_data/flattened/generated_with_outcome/
--rw-r--r--   0 root         (0) root         (0)     1477 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
--rw-r--r--   0 root         (0) root         (0)   864795 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 12:12:58.041123 timeseriesflattener-0.23.9/tests/test_data/models/
--rw-r--r--   0 root         (0) root         (0)     1905 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/test_data/models/create_bow_and_pca_model.py
--rw-r--r--   0 root         (0) root         (0)    25543 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/test_data/models/synth_bow_model.pkl
--rw-r--r--   0 root         (0) root         (0)     1015 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/test_data/models/synth_pca_model.pkl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 12:12:58.053123 timeseriesflattener-0.23.9/tests/test_data/raw/
--rw-r--r--   0 root         (0) root         (0)      779 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/test_data/raw/create_synth_prediction_times.py
--rw-r--r--   0 root         (0) root         (0)     1003 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/test_data/raw/create_synth_raw_binary.py
--rw-r--r--   0 root         (0) root         (0)      975 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/test_data/raw/create_synth_raw_float.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/test_data/raw/create_synth_sex.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/test_data/raw/create_synth_txt_data.py
--rw-r--r--   0 root         (0) root         (0)   248865 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/test_data/raw/synth_prediction_times.csv
--rw-r--r--   0 root         (0) root         (0)   268962 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/test_data/raw/synth_raw_binary_1.csv
--rw-r--r--   0 root         (0) root         (0)   268904 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/test_data/raw/synth_raw_binary_2.csv
--rw-r--r--   0 root         (0) root         (0)  4316151 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/test_data/raw/synth_raw_float_1.csv
--rw-r--r--   0 root         (0) root         (0)  4315816 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/test_data/raw/synth_raw_float_2.csv
--rw-r--r--   0 root         (0) root         (0)    68900 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/test_data/raw/synth_sex.csv
--rw-r--r--   0 root         (0) root         (0)    84570 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/test_data/raw/synth_text_data.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 12:12:58.053123 timeseriesflattener-0.23.9/tests/test_feature_cache/
--rw-r--r--   0 root         (0) root         (0)     3488 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/test_feature_cache/test_cache_to_disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 12:12:58.053123 timeseriesflattener-0.23.9/tests/test_timeseriesflattener/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/test_timeseriesflattener/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/test_timeseriesflattener/test_embedding_functions.py
--rw-r--r--   0 root         (0) root         (0)     7407 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/test_timeseriesflattener/test_feature_spec_objects.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 12:12:58.053123 timeseriesflattener-0.23.9/tests/test_timeseriesflattener/test_flattened_dataset/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18380 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
--rw-r--r--   0 root         (0) root         (0)     2391 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
--rw-r--r--   0 root         (0) root         (0)     2347 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
--rw-r--r--   0 root         (0) root         (0)     2326 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
--rw-r--r--   0 root         (0) root         (0)     6566 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2428 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
--rw-r--r--   0 root         (0) root         (0)    15053 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/test_timeseriesflattener/test_resolve_multiple.py
--rw-r--r--   0 root         (0) root         (0)      982 2023-03-28 12:12:47.000000 timeseriesflattener-0.23.9/tests/test_timeseriesflattener/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.119045 timeseriesflattener-0.24.0/
+-rw-r--r--   0 root         (0) root         (0)      489 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.cookiecutter.json
+-rw-r--r--   0 root         (0) root         (0)      738 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.cruft.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.083044 timeseriesflattener-0.24.0/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.079044 timeseriesflattener-0.24.0/.github/actions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.083044 timeseriesflattener-0.24.0/.github/actions/test/
+-rw-r--r--   0 root         (0) root         (0)      950 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.github/actions/test/action.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.087044 timeseriesflattener-0.24.0/.github/actions/test_tutorials/
+-rw-r--r--   0 root         (0) root         (0)      994 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.github/actions/test_tutorials/action.yml
+-rw-r--r--   0 root         (0) root         (0)      529 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.github/dependabot.yml
+-rw-r--r--   0 root         (0) root         (0)      252 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.github/pull_request_template.md
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.github/recommended_repo_setup.md
+-rw-r--r--   0 root         (0) root         (0)      465 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.github/setup_ci.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.087044 timeseriesflattener-0.24.0/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      720 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.github/workflows/check_for_rej.yml
+-rw-r--r--   0 root         (0) root         (0)     2083 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.github/workflows/cruft.yml
+-rw-r--r--   0 root         (0) root         (0)      849 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)      877 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)      727 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.github/workflows/generate_paper_pdf.yml
+-rw-r--r--   0 root         (0) root         (0)     2446 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.github/workflows/main_test_and_release.yml
+-rw-r--r--   0 root         (0) root         (0)     2891 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.github/workflows/stalebot.yml
+-rw-r--r--   0 root         (0) root         (0)     3027 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.github/workflows/static_type_checks.yml
+-rw-r--r--   0 root         (0) root         (0)     2871 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      644 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.zenodo.json
+-rw-r--r--   0 root         (0) root         (0)    53313 2023-04-20 09:04:52.000000 timeseriesflattener-0.24.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     5238 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     4474 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     1087 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      262 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/Makefile
+-rw-r--r--   0 root         (0) root         (0)    11584 2023-04-20 09:05:05.119045 timeseriesflattener-0.24.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9185 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      658 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/citation.cff
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.091044 timeseriesflattener-0.24.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      633 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.091044 timeseriesflattener-0.24.0/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)    15406 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/_static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    49714 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)    49714 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/_static/icon_dark.png
+-rw-r--r--   0 root         (0) root         (0)   811066 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/_static/terminology_figure.png
+-rw-r--r--   0 root         (0) root         (0)     4211 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/faq.rst
+-rw-r--r--   0 root         (0) root         (0)      320 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/feature_specifications.rst
+-rw-r--r--   0 root         (0) root         (0)     5280 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      299 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)      312 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/timeseriesflattener.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.091044 timeseriesflattener-0.24.0/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)   130812 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/tutorials/01_basic.ipynb
+-rw-r--r--   0 root         (0) root         (0)    68248 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/tutorials/02_advanced.ipynb
+-rw-r--r--   0 root         (0) root         (0)    77800 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/tutorials/03_text.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.095044 timeseriesflattener-0.24.0/docs/tutorials/img/
+-rw-r--r--   0 root         (0) root         (0)    78953 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/tutorials/img/term_a.png
+-rw-r--r--   0 root         (0) root         (0)   109486 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/tutorials/img/term_b.png
+-rw-r--r--   0 root         (0) root         (0)   107613 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/tutorials/img/term_c.png
+-rw-r--r--   0 root         (0) root         (0)   250306 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/tutorials/img/term_d.png
+-rw-r--r--   0 root         (0) root         (0)      370 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/tutorials.rst
+-rw-r--r--   0 root         (0) root         (0)    49714 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.095044 timeseriesflattener-0.24.0/paper/
+-rw-r--r--   0 root         (0) root         (0)    14392 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/paper/paper.bib
+-rw-r--r--   0 root         (0) root         (0)     9344 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/paper/paper.md
+-rw-r--r--   0 root         (0) root         (0)     4418 2023-04-20 09:04:52.000000 timeseriesflattener-0.24.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 09:05:05.119045 timeseriesflattener-0.24.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.079044 timeseriesflattener-0.24.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.095044 timeseriesflattener-0.24.0/src/timeseriesflattener/
+-rw-r--r--   0 root         (0) root         (0)      226 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/src/timeseriesflattener/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5170 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/src/timeseriesflattener/column_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.099044 timeseriesflattener-0.24.0/src/timeseriesflattener/feature_cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/src/timeseriesflattener/feature_cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1971 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/src/timeseriesflattener/feature_cache/abstract_feature_cache.py
+-rw-r--r--   0 root         (0) root         (0)     6145 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/src/timeseriesflattener/feature_cache/cache_to_disk.py
+-rw-r--r--   0 root         (0) root         (0)    40328 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/src/timeseriesflattener/feature_spec_objects.py
+-rw-r--r--   0 root         (0) root         (0)    36771 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/src/timeseriesflattener/flattened_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2266 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/src/timeseriesflattener/flattened_ds_validator.py
+-rw-r--r--   0 root         (0) root         (0)     2234 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/src/timeseriesflattener/logger.py
+-rw-r--r--   0 root         (0) root         (0)     3661 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/src/timeseriesflattener/resolve_multiple_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.099044 timeseriesflattener-0.24.0/src/timeseriesflattener/testing/
+-rw-r--r--   0 root         (0) root         (0)     3168 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/src/timeseriesflattener/testing/load_synth_data.py
+-rw-r--r--   0 root         (0) root         (0)     1416 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/src/timeseriesflattener/testing/text_embedding_functions.py
+-rw-r--r--   0 root         (0) root         (0)     5271 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/src/timeseriesflattener/testing/utils_for_testing.py
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/src/timeseriesflattener/text_embedding_functions.py
+-rw-r--r--   0 root         (0) root         (0)     7704 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/src/timeseriesflattener/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.099044 timeseriesflattener-0.24.0/src/timeseriesflattener.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11584 2023-04-20 09:05:04.000000 timeseriesflattener-0.24.0/src/timeseriesflattener.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3857 2023-04-20 09:05:05.000000 timeseriesflattener-0.24.0/src/timeseriesflattener.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 09:05:04.000000 timeseriesflattener-0.24.0/src/timeseriesflattener.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      820 2023-04-20 09:05:04.000000 timeseriesflattener-0.24.0/src/timeseriesflattener.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-04-20 09:05:04.000000 timeseriesflattener-0.24.0/src/timeseriesflattener.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     9157 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.099044 timeseriesflattener-0.24.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.079044 timeseriesflattener-0.24.0/tests/test_data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.079044 timeseriesflattener-0.24.0/tests/test_data/flattened/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.099044 timeseriesflattener-0.24.0/tests/test_data/flattened/generated_with_outcome/
+-rw-r--r--   0 root         (0) root         (0)     1477 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tests/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
+-rw-r--r--   0 root         (0) root         (0)   864795 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tests/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.103044 timeseriesflattener-0.24.0/tests/test_data/models/
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tests/test_data/models/create_bow_and_pca_model.py
+-rw-r--r--   0 root         (0) root         (0)    25543 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tests/test_data/models/synth_bow_model.pkl
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tests/test_data/models/synth_pca_model.pkl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.115044 timeseriesflattener-0.24.0/tests/test_data/raw/
+-rw-r--r--   0 root         (0) root         (0)      779 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tests/test_data/raw/create_synth_prediction_times.py
+-rw-r--r--   0 root         (0) root         (0)     1003 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tests/test_data/raw/create_synth_raw_binary.py
+-rw-r--r--   0 root         (0) root         (0)      975 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tests/test_data/raw/create_synth_raw_float.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tests/test_data/raw/create_synth_sex.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tests/test_data/raw/create_synth_txt_data.py
+-rw-r--r--   0 root         (0) root         (0)   248865 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tests/test_data/raw/synth_prediction_times.csv
+-rw-r--r--   0 root         (0) root         (0)   268962 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tests/test_data/raw/synth_raw_binary_1.csv
+-rw-r--r--   0 root         (0) root         (0)   268904 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tests/test_data/raw/synth_raw_binary_2.csv
+-rw-r--r--   0 root         (0) root         (0)  4316151 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_data/raw/synth_raw_float_1.csv
+-rw-r--r--   0 root         (0) root         (0)  4315816 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_data/raw/synth_raw_float_2.csv
+-rw-r--r--   0 root         (0) root         (0)    68900 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_data/raw/synth_sex.csv
+-rw-r--r--   0 root         (0) root         (0)    84570 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_data/raw/synth_text_data.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.115044 timeseriesflattener-0.24.0/tests/test_feature_cache/
+-rw-r--r--   0 root         (0) root         (0)     3490 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_feature_cache/test_cache_to_disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.119045 timeseriesflattener-0.24.0/tests/test_timeseriesflattener/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_timeseriesflattener/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_embedding_functions.py
+-rw-r--r--   0 root         (0) root         (0)     7778 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_feature_spec_objects.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.119045 timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_flattened_dataset/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18335 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
+-rw-r--r--   0 root         (0) root         (0)     6598 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
+-rw-r--r--   0 root         (0) root         (0)    15009 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_resolve_multiple.py
+-rw-r--r--   0 root         (0) root         (0)      998 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_utils.py
```

### Comparing `timeseriesflattener-0.23.9/.github/actions/test_tutorials/action.yml` & `timeseriesflattener-0.24.0/.github/actions/test_tutorials/action.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/.github/workflows/dependabot_automerge.yml` & `timeseriesflattener-0.24.0/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/.github/workflows/generate_paper_pdf.yml` & `timeseriesflattener-0.24.0/.github/workflows/generate_paper_pdf.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/.github/workflows/main_test_and_release.yml` & `timeseriesflattener-0.24.0/.github/workflows/main_test_and_release.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/.gitignore` & `timeseriesflattener-0.24.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -162,7 +162,9 @@
 poetry.lock
 *.html
 
 # PyCharm
 /.idea/*
 **/tmp/
 **/.tmp/
+
+*nbconvert*
```

### Comparing `timeseriesflattener-0.23.9/.pre-commit-config.yaml` & `timeseriesflattener-0.24.0/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 repos:
   - repo: https://github.com/psf/black
     rev: 22.8.0
     hooks:
       - id: black
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    # Ruff version.
     rev: v0.0.254
     hooks:
       - id: ruff
         args:
           [
             "--extend-select",
             "F401",
```

### Comparing `timeseriesflattener-0.23.9/.zenodo.json` & `timeseriesflattener-0.24.0/.zenodo.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/CHANGELOG.md` & `timeseriesflattener-0.24.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,38 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.24.0 (2023-04-20)
+### Feature
+* Modify invoke test command to take python-versions arg ([`4a9c5c2`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/4a9c5c2e672fc67bd56e57313588f09737b69f88))
+* Improve type hints ([`d53e61e`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/d53e61e0b7037064b1cb4e0a29455c5523749dba))
+
+### Fix
+* Support multiple python versions for testing ([`d929147`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/d929147cc14b59947b559501e31eec60f278f1fc))
+* Correct interval str computation ([`0cd0437`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/0cd043743617730f979e1e1b34e3adb30137d36f))
+* Change col str naming ([`f853452`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/f85345218cc0fb5dc69b748edb3555806d3bc9fe))
+* Fix interval days type hints in specs ([`e26235c`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/e26235c78c5068e17b0bce0a5c64c47c2a362ffc))
+* Rename test deps ([`471a63b`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/471a63b9147932677cbf816582ed1d228c38b9c0))
+* Type hints ([`21726f2`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/21726f2aa976c0110b6a0b7656c2bd60fd10f7ef))
+
+### Documentation
+* Align docstrings ([`8d92a25`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/8d92a2553e3909906194e661a4c58e9a5f2d5226))
+* Fix tutorial ([`f856a56`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/f856a5661cf3bed9832c0ddd3c25d2f8f3323107))
+* Update docstrings ([`b771f5b`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/b771f5b89cba1aa2f28b2c5a7dafb47b18e04991))
+* Update citation in faq ([`8fdfbc4`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/8fdfbc44d8e641e3261d4a623e209234ea8c3d66))
+
+## v0.23.11 (2023-03-28)
+### Fix
+* Doi for shamout and imrie ([`4823e1e`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/4823e1ef0b66c2438f08d8080cd1d14f62696ff2))
+
+## v0.23.10 (2023-03-28)
+### Fix
+* Force new release ([`e6522d6`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/e6522d6af0c7d302d7326a15cdbc7c3aaee1e71c))
+
 ## v0.23.9 (2023-03-28)
 ### Fix
 * Description in .zenodo.json ([`1a4e31a`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/1a4e31adfd7f3253a56e312444767cd2c4d6a15a))
 
 ## v0.23.8 (2023-03-28)
 ### Fix
 * Add .zenodo.json ([`f6bc274`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/f6bc274f79e9e84fe6c7085598eb2534e222c93c))
```

### Comparing `timeseriesflattener-0.23.9/CODE_OF_CONDUCT.md` & `timeseriesflattener-0.24.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/CONTRIBUTING.md` & `timeseriesflattener-0.24.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/LICENSE` & `timeseriesflattener-0.24.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/PKG-INFO` & `timeseriesflattener-0.24.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7469 6d65  : 2.1.Name: time
 00000020: 7365 7269 6573 666c 6174 7465 6e65 720a  seriesflattener.
-00000030: 5665 7273 696f 6e3a 2030 2e32 332e 390a  Version: 0.23.9.
+00000030: 5665 7273 696f 6e3a 2030 2e32 342e 300a  Version: 0.24.0.
 00000040: 5375 6d6d 6172 793a 2041 2070 6163 6b61  Summary: A packa
 00000050: 6765 2066 6f72 2063 6f6e 7665 7274 696e  ge for convertin
 00000060: 6720 7469 6d65 2073 6572 6965 7320 6461  g time series da
 00000070: 7461 2066 726f 6d20 652e 672e 2065 6c65  ta from e.g. ele
 00000080: 6374 726f 6e69 6320 6865 616c 7468 2072  ctronic health r
 00000090: 6563 6f72 6473 2069 6e74 6f20 7769 6465  ecords into wide
 000000a0: 2066 6f72 6d61 7420 6461 7461 2e0a 4175   format data..Au
@@ -15,615 +15,710 @@
 000000e0: 7365 6e20 3c6c 6173 7365 6830 3331 3040  sen <lasseh0310@
 000000f0: 676d 6169 6c2e 636f 6d3e 2c20 4a61 6b6f  gmail.com>, Jako
 00000100: 6220 4772 c3b8 686e 2044 616d 6761 6172  b Gr..hn Damgaar
 00000110: 6420 3c62 6f6b 616a 6764 4067 6d61 696c  d <bokajgd@gmail
 00000120: 2e63 6f6d 3e2c 204d 6172 7469 6e20 4265  .com>, Martin Be
 00000130: 726e 7374 6f72 6666 203c 6d61 7274 696e  rnstorff <martin
 00000140: 6265 726e 7374 6f72 6666 4067 6d61 696c  bernstorff@gmail
-00000150: 2e63 6f6d 3e0a 436c 6173 7369 6669 6572  .com>.Classifier
-00000160: 3a20 4f70 6572 6174 696e 6720 5379 7374  : Operating Syst
-00000170: 656d 203a 3a20 504f 5349 5820 3a3a 204c  em :: POSIX :: L
-00000180: 696e 7578 0a43 6c61 7373 6966 6965 723a  inux.Classifier:
-00000190: 204f 7065 7261 7469 6e67 2053 7973 7465   Operating Syste
-000001a0: 6d20 3a3a 204d 6163 4f53 203a 3a20 4d61  m :: MacOS :: Ma
-000001b0: 634f 5320 580a 436c 6173 7369 6669 6572  cOS X.Classifier
-000001c0: 3a20 4f70 6572 6174 696e 6720 5379 7374  : Operating Syst
-000001d0: 656d 203a 3a20 4d69 6372 6f73 6f66 7420  em :: Microsoft 
-000001e0: 3a3a 2057 696e 646f 7773 0a43 6c61 7373  :: Windows.Class
-000001f0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000200: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000210: 7974 686f 6e20 3a3a 2033 2e38 0a43 6c61  ython :: 3.8.Cla
-00000220: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00000230: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000240: 2050 7974 686f 6e20 3a3a 2033 2e39 0a43   Python :: 3.9.C
-00000250: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-00000260: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000270: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
-00000280: 300a 436c 6173 7369 6669 6572 3a20 5072  0.Classifier: Pr
-00000290: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000002a0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000002b0: 332e 3131 0a52 6571 7569 7265 732d 5079  3.11.Requires-Py
-000002c0: 7468 6f6e 3a20 3c33 2e31 322e 302c 3e3d  thon: <3.12.0,>=
-000002d0: 332e 382e 300a 4465 7363 7269 7074 696f  3.8.0.Descriptio
-000002e0: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
-000002f0: 7465 7874 2f6d 6172 6b64 6f77 6e0a 5072  text/markdown.Pr
-00000300: 6f76 6964 6573 2d45 7874 7261 3a20 6465  ovides-Extra: de
-00000310: 760a 5072 6f76 6964 6573 2d45 7874 7261  v.Provides-Extra
-00000320: 3a20 646f 6373 0a50 726f 7669 6465 732d  : docs.Provides-
-00000330: 4578 7472 613a 2074 7574 6f72 6961 6c73  Extra: tutorials
-00000340: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-00000350: 2074 6578 740a 4c69 6365 6e73 652d 4669   text.License-Fi
-00000360: 6c65 3a20 4c49 4345 4e53 450a 0a3c 6120  le: LICENSE..<a 
-00000370: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-00000380: 7468 7562 2e63 6f6d 2f41 6172 6875 732d  thub.com/Aarhus-
-00000390: 5073 7963 6869 6174 7279 2d52 6573 6561  Psychiatry-Resea
-000003a0: 7263 682f 7469 6d65 7365 7269 6573 666c  rch/timeseriesfl
-000003b0: 6174 7465 6e65 7222 3e3c 696d 6720 7372  attener"><img sr
-000003c0: 633d 2268 7474 7073 3a2f 2f67 6974 6875  c="https://githu
-000003d0: 622e 636f 6d2f 4161 7268 7573 2d50 7379  b.com/Aarhus-Psy
-000003e0: 6368 6961 7472 792d 5265 7365 6172 6368  chiatry-Research
-000003f0: 2f74 696d 6573 6572 6965 7366 6c61 7474  /timeseriesflatt
-00000400: 656e 6572 2f62 6c6f 622f 6d61 696e 2f64  ener/blob/main/d
-00000410: 6f63 732f 5f73 7461 7469 632f 6963 6f6e  ocs/_static/icon
-00000420: 2e70 6e67 3f72 6177 3d74 7275 6522 2077  .png?raw=true" w
-00000430: 6964 7468 3d22 3230 3022 2061 6c69 676e  idth="200" align
-00000440: 3d22 7269 6768 7422 2f3e 3c2f 613e 0a0a  ="right"/></a>..
-00000450: 2320 5469 6d65 7365 7269 6573 666c 6174  # Timeseriesflat
-00000460: 7465 6e65 720a 0a5b 215b 6769 7468 7562  tener..[![github
-00000470: 2061 6374 696f 6e73 2064 6f63 735d 2868   actions docs](h
-00000480: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000490: 6d2f 4161 7268 7573 2d50 7379 6368 6961  m/Aarhus-Psychia
-000004a0: 7472 792d 5265 7365 6172 6368 2f74 696d  try-Research/tim
-000004b0: 6573 6572 6965 7366 6c61 7474 656e 6572  eseriesflattener
-000004c0: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-000004d0: 7773 2f64 6f63 756d 656e 7461 7469 6f6e  ws/documentation
-000004e0: 2e79 6d6c 2f62 6164 6765 2e73 7667 295d  .yml/badge.svg)]
-000004f0: 2868 7474 7073 3a2f 2f61 6172 6875 732d  (https://aarhus-
-00000500: 7073 7963 6869 6174 7279 2d72 6573 6561  psychiatry-resea
-00000510: 7263 682e 6769 7468 7562 2e69 6f2f 7469  rch.github.io/ti
-00000520: 6d65 7365 7269 6573 666c 6174 7465 6e65  meseriesflattene
-00000530: 722f 290a 5b21 5b67 6974 6875 6220 6163  r/).[![github ac
-00000540: 7469 6f6e 7320 7079 7465 7374 5d28 6874  tions pytest](ht
-00000550: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000560: 2f41 6172 6875 732d 5073 7963 6869 6174  /Aarhus-Psychiat
-00000570: 7279 2d52 6573 6561 7263 682f 7469 6d65  ry-Research/time
-00000580: 7365 7269 6573 666c 6174 7465 6e65 722f  seriesflattener/
-00000590: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
-000005a0: 732f 6d61 696e 5f74 6573 745f 616e 645f  s/main_test_and_
-000005b0: 7265 6c65 6173 652e 796d 6c2f 6261 6467  release.yml/badg
-000005c0: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
-000005d0: 6769 7468 7562 2e63 6f6d 2f41 6172 6875  github.com/Aarhu
-000005e0: 732d 5073 7963 6869 6174 7279 2d52 6573  s-Psychiatry-Res
-000005f0: 6561 7263 682f 7469 6d65 7365 7269 6573  earch/timeseries
-00000600: 666c 6174 7465 6e65 722f 6163 7469 6f6e  flattener/action
-00000610: 7329 0a5b 215b 7079 7468 6f6e 2076 6572  s).[![python ver
-00000620: 7369 6f6e 735d 2868 7474 7073 3a2f 2f69  sions](https://i
-00000630: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-00000640: 7069 2f70 7976 6572 7369 6f6e 732f 7469  pi/pyversions/ti
-00000650: 6d65 7365 7269 6573 666c 6174 7465 6e65  meseriesflattene
-00000660: 7229 5d28 6874 7470 733a 2f2f 7079 7069  r)](https://pypi
-00000670: 2e6f 7267 2f70 726f 6a65 6374 2f74 696d  .org/project/tim
-00000680: 6573 6572 6965 7366 6c61 7474 656e 6572  eseriesflattener
-00000690: 2f29 0a5b 215b 436f 6465 2073 7479 6c65  /).[![Code style
-000006a0: 3a20 626c 6163 6b5d 2868 7474 7073 3a2f  : black](https:/
-000006b0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-000006c0: 6261 6467 652f 436f 6465 2532 3053 7479  badge/Code%20Sty
-000006d0: 6c65 2d42 6c61 636b 2d62 6c61 636b 295d  le-Black-black)]
-000006e0: 2868 7474 7073 3a2f 2f62 6c61 636b 2e72  (https://black.r
-000006f0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00000700: 2f73 7461 626c 652f 7468 655f 626c 6163  /stable/the_blac
-00000710: 6b5f 636f 6465 5f73 7479 6c65 2f63 7572  k_code_style/cur
-00000720: 7265 6e74 5f73 7479 6c65 2e68 746d 6c29  rent_style.html)
-00000730: 0a0a 5b21 5b50 7950 4920 7665 7273 696f  ..[![PyPI versio
-00000740: 6e5d 2868 7474 7073 3a2f 2f62 6164 6765  n](https://badge
-00000750: 2e66 7572 792e 696f 2f70 792f 7469 6d65  .fury.io/py/time
-00000760: 7365 7269 6573 666c 6174 7465 6e65 722e  seriesflattener.
-00000770: 7376 6729 5d28 6874 7470 733a 2f2f 7079  svg)](https://py
-00000780: 7069 2e6f 7267 2f70 726f 6a65 6374 2f74  pi.org/project/t
-00000790: 696d 6573 6572 6965 7366 6c61 7474 656e  imeseriesflatten
-000007a0: 6572 2f29 0a5b 215b 7374 6174 7573 5d28  er/).[![status](
-000007b0: 6874 7470 733a 2f2f 6a6f 7373 2e74 6865  https://joss.the
-000007c0: 6f6a 2e6f 7267 2f70 6170 6572 732f 3362  oj.org/papers/3b
-000007d0: 6265 6138 3734 3536 3638 6431 6161 3430  bea8745668d1aa40
-000007e0: 6666 3739 3663 3666 6433 6462 3837 2f73  ff796c6fd3db87/s
-000007f0: 7461 7475 732e 7376 6729 5d28 6874 7470  tatus.svg)](http
-00000800: 733a 2f2f 6a6f 7373 2e74 6865 6f6a 2e6f  s://joss.theoj.o
-00000810: 7267 2f70 6170 6572 732f 3362 6265 6138  rg/papers/3bbea8
-00000820: 3734 3536 3638 6431 6161 3430 6666 3739  745668d1aa40ff79
-00000830: 3663 3666 6433 6462 3837 290a 0a54 696d  6c6fd3db87)..Tim
-00000840: 6520 7365 7269 6573 2066 726f 6d20 652e  e series from e.
-00000850: 672e 2065 6c65 6374 726f 6e69 6320 6865  g. electronic he
-00000860: 616c 7468 2072 6563 6f72 6473 206f 6674  alth records oft
-00000870: 656e 2068 6176 6520 6120 6c61 7267 6520  en have a large 
-00000880: 6e75 6d62 6572 206f 6620 7661 7269 6162  number of variab
-00000890: 6c65 732c 2061 7265 2073 616d 706c 6564  les, are sampled
-000008a0: 2061 7420 6972 7265 6775 6c61 7220 696e   at irregular in
-000008b0: 7465 7276 616c 7320 616e 6420 7465 6e64  tervals and tend
-000008c0: 2074 6f20 6861 7665 2061 206c 6172 6765   to have a large
-000008d0: 206e 756d 6265 7220 6f66 206d 6973 7369   number of missi
-000008e0: 6e67 2076 616c 7565 732e 2042 6566 6f72  ng values. Befor
-000008f0: 6520 7468 6973 2074 7970 6520 6f66 2064  e this type of d
-00000900: 6174 6120 6361 6e20 6265 2075 7365 6420  ata can be used 
-00000910: 666f 7220 7072 6564 6963 7469 6f6e 206d  for prediction m
-00000920: 6f64 656c 6c69 6e67 2077 6974 6820 6d61  odelling with ma
-00000930: 6368 696e 6520 6c65 6172 6e69 6e67 206d  chine learning m
-00000940: 6574 686f 6473 2073 7563 6820 6173 206c  ethods such as l
-00000950: 6f67 6973 7469 6320 7265 6772 6573 7369  ogistic regressi
-00000960: 6f6e 206f 7220 5847 426f 6f73 742c 2074  on or XGBoost, t
-00000970: 6865 2064 6174 6120 6e65 6564 7320 746f  he data needs to
-00000980: 2062 6520 7265 7368 6170 6564 2e20 0a0a   be reshaped. ..
-00000990: 496e 2065 7373 656e 6365 2c20 7468 6520  In essence, the 
-000009a0: 7469 6d65 2073 6572 6965 7320 6e65 6564  time series need
-000009b0: 2074 6f20 6265 202a 666c 6174 7465 6e65   to be *flattene
-000009c0: 642a 2073 6f20 7468 6174 2065 6163 6820  d* so that each 
-000009d0: 7072 6564 6963 7469 6f6e 2074 696d 6520  prediction time 
-000009e0: 6973 2072 6570 7265 7365 6e74 6564 2062  is represented b
-000009f0: 7920 6120 7365 7420 6f66 2070 7265 6469  y a set of predi
-00000a00: 6374 6f72 2076 616c 7565 7320 616e 6420  ctor values and 
-00000a10: 616e 206f 7574 636f 6d65 2076 616c 7565  an outcome value
-00000a20: 2e20 5468 6573 6520 7072 6564 6963 746f  . These predicto
-00000a30: 7220 7661 6c75 6573 2063 616e 2062 6520  r values can be 
-00000a40: 636f 6e73 7472 7563 7465 6420 6279 2061  constructed by a
-00000a50: 6767 7265 6761 7469 6e67 2074 6865 2070  ggregating the p
-00000a60: 7265 6365 6469 6e67 2076 616c 7565 7320  receding values 
-00000a70: 696e 2074 6865 2074 696d 6520 7365 7269  in the time seri
-00000a80: 6573 2077 6974 6869 6e20 6120 6365 7274  es within a cert
-00000a90: 6169 6e20 7469 6d65 2077 696e 646f 772e  ain time window.
-00000aa0: 200a 0a60 7469 6d65 7365 7269 6573 666c   ..`timeseriesfl
-00000ab0: 6174 7465 6e65 7260 2061 696d 7320 746f  attener` aims to
-00000ac0: 2073 696d 706c 6966 7920 7468 6973 2070   simplify this p
-00000ad0: 726f 6365 7373 2062 7920 7072 6f76 6964  rocess by provid
-00000ae0: 696e 6720 616e 2065 6173 792d 746f 2d75  ing an easy-to-u
-00000af0: 7365 2061 6e64 2066 756c 6c79 2d73 7065  se and fully-spe
-00000b00: 6369 6669 6564 2070 6970 656c 696e 6520  cified pipeline 
-00000b10: 666f 7220 666c 6174 7465 6e69 6e67 2063  for flattening c
-00000b20: 6f6d 706c 6578 2074 696d 6520 7365 7269  omplex time seri
-00000b30: 6573 2e20 0a0a 2323 20f0 9f94 a720 496e  es. ..## .... In
-00000b40: 7374 616c 6c61 7469 6f6e 0a54 6f20 6765  stallation.To ge
-00000b50: 7420 7374 6172 7465 6420 7573 696e 6720  t started using 
-00000b60: 7469 6d65 7365 7269 6573 666c 6174 7465  timeseriesflatte
-00000b70: 6e65 7220 7369 6d70 6c79 2069 6e73 7461  ner simply insta
-00000b80: 6c6c 2069 7420 7573 696e 6720 7069 7020  ll it using pip 
-00000b90: 6279 2072 756e 6e69 6e67 2074 6865 2066  by running the f
-00000ba0: 6f6c 6c6f 7769 6e67 206c 696e 6520 696e  ollowing line in
-00000bb0: 2079 6f75 7220 7465 726d 696e 616c 3a0a   your terminal:.
-00000bc0: 0a60 6060 0a70 6970 2069 6e73 7461 6c6c  .```.pip install
-00000bd0: 2074 696d 6573 6572 6965 7366 6c61 7474   timeseriesflatt
-00000be0: 656e 6572 0a60 6060 0a0a 2323 20e2 9aa1  ener.```..## ...
-00000bf0: 2051 7569 636b 2073 7461 7274 0a0a 6060   Quick start..``
-00000c00: 6070 790a 696d 706f 7274 206e 756d 7079  `py.import numpy
-00000c10: 2061 7320 6e70 0a69 6d70 6f72 7420 7061   as np.import pa
-00000c20: 6e64 6173 2061 7320 7064 0a0a 6966 205f  ndas as pd..if _
-00000c30: 5f6e 616d 655f 5f20 3d3d 2022 5f5f 6d61  _name__ == "__ma
-00000c40: 696e 5f5f 223a 0a0a 2020 2020 2320 4c6f  in__":..    # Lo
-00000c50: 6164 2061 2064 6174 6166 7261 6d65 2077  ad a dataframe w
-00000c60: 6974 6820 7469 6d65 7320 796f 7520 7769  ith times you wi
-00000c70: 7368 2074 6f20 6d61 6b65 2061 2070 7265  sh to make a pre
-00000c80: 6469 6374 696f 6e0a 2020 2020 7072 6564  diction.    pred
-00000c90: 6963 7469 6f6e 5f74 696d 6573 5f64 6620  iction_times_df 
-00000ca0: 3d20 7064 2e44 6174 6146 7261 6d65 280a  = pd.DataFrame(.
-00000cb0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-00000cc0: 2020 2020 2020 2269 6422 3a20 5b31 2c20        "id": [1, 
-00000cd0: 312c 2032 5d2c 0a20 2020 2020 2020 2020  1, 2],.         
-00000ce0: 2020 2022 6461 7465 223a 205b 2232 3032     "date": ["202
-00000cf0: 302d 3031 2d30 3122 2c20 2232 3032 302d  0-01-01", "2020-
-00000d00: 3032 2d30 3122 2c20 2232 3032 302d 3032  02-01", "2020-02
-00000d10: 2d30 3122 5d2c 0a20 2020 2020 2020 207d  -01"],.        }
-00000d20: 2c0a 2020 2020 290a 2020 2020 2320 4c6f  ,.    ).    # Lo
-00000d30: 6164 2061 2064 6174 6166 7261 6d65 2077  ad a dataframe w
-00000d40: 6974 6820 7261 7720 7661 6c75 6573 2079  ith raw values y
-00000d50: 6f75 2077 6973 6820 746f 2061 6767 7265  ou wish to aggre
-00000d60: 6761 7465 2061 7320 7072 6564 6963 746f  gate as predicto
-00000d70: 7273 0a20 2020 2070 7265 6469 6374 6f72  rs.    predictor
-00000d80: 5f64 6620 3d20 7064 2e44 6174 6146 7261  _df = pd.DataFra
-00000d90: 6d65 280a 2020 2020 2020 2020 7b0a 2020  me(.        {.  
-00000da0: 2020 2020 2020 2020 2020 2269 6422 3a20            "id": 
-00000db0: 5b31 2c20 312c 2031 2c20 325d 2c0a 2020  [1, 1, 1, 2],.  
-00000dc0: 2020 2020 2020 2020 2020 2264 6174 6522            "date"
-00000dd0: 3a20 5b0a 2020 2020 2020 2020 2020 2020  : [.            
-00000de0: 2020 2020 2232 3032 302d 3031 2d31 3522      "2020-01-15"
-00000df0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000e00: 2020 2232 3031 392d 3132 2d31 3022 2c0a    "2019-12-10",.
-00000e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e20: 2232 3031 392d 3132 2d31 3522 2c0a 2020  "2019-12-15",.  
-00000e30: 2020 2020 2020 2020 2020 2020 2020 2232                "2
-00000e40: 3032 302d 3031 2d30 3222 2c0a 2020 2020  020-01-02",.    
-00000e50: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
-00000e60: 2020 2020 2020 2022 7661 6c75 6522 3a20         "value": 
-00000e70: 5b31 2c20 322c 2033 2c20 345d 2c0a 2020  [1, 2, 3, 4],.  
-00000e80: 2020 2020 2020 7d2c 0a20 2020 2029 0a20        },.    ). 
-00000e90: 2020 2023 204c 6f61 6420 6120 6461 7461     # Load a data
-00000ea0: 6672 616d 6520 7370 6563 6966 7969 6e67  frame specifying
-00000eb0: 2077 6865 6e20 7468 6520 6f75 7463 6f6d   when the outcom
-00000ec0: 6520 6f63 6375 7273 0a20 2020 206f 7574  e occurs.    out
-00000ed0: 636f 6d65 5f64 6620 3d20 7064 2e44 6174  come_df = pd.Dat
-00000ee0: 6146 7261 6d65 287b 2269 6422 3a20 5b31  aFrame({"id": [1
-00000ef0: 5d2c 2022 6461 7465 223a 205b 2232 3032  ], "date": ["202
-00000f00: 302d 3033 2d30 3122 5d2c 2022 7661 6c75  0-03-01"], "valu
-00000f10: 6522 3a20 5b31 5d7d 290a 0a20 2020 2023  e": [1]})..    #
-00000f20: 2053 7065 6369 6679 2068 6f77 2074 6f20   Specify how to 
-00000f30: 6167 6772 6567 6174 6520 7468 6520 7072  aggregate the pr
-00000f40: 6564 6963 746f 7273 2061 6e64 2064 6566  edictors and def
-00000f50: 696e 6520 7468 6520 6f75 7463 6f6d 650a  ine the outcome.
-00000f60: 2020 2020 6672 6f6d 2074 696d 6573 6572      from timeser
-00000f70: 6965 7366 6c61 7474 656e 6572 2e66 6561  iesflattener.fea
-00000f80: 7475 7265 5f73 7065 635f 6f62 6a65 6374  ture_spec_object
-00000f90: 7320 696d 706f 7274 204f 7574 636f 6d65  s import Outcome
-00000fa0: 5370 6563 2c20 5072 6564 6963 746f 7253  Spec, PredictorS
-00000fb0: 7065 630a 2020 2020 6672 6f6d 2074 696d  pec.    from tim
-00000fc0: 6573 6572 6965 7366 6c61 7474 656e 6572  eseriesflattener
-00000fd0: 2e72 6573 6f6c 7665 5f6d 756c 7469 706c  .resolve_multipl
-00000fe0: 655f 6675 6e63 7469 6f6e 7320 696d 706f  e_functions impo
-00000ff0: 7274 206d 6178 696d 756d 2c20 6d65 616e  rt maximum, mean
-00001000: 0a0a 2020 2020 7072 6564 6963 746f 725f  ..    predictor_
-00001010: 7370 6563 203d 2050 7265 6469 6374 6f72  spec = Predictor
-00001020: 5370 6563 280a 2020 2020 2020 2020 7661  Spec(.        va
-00001030: 6c75 6573 5f64 663d 7072 6564 6963 746f  lues_df=predicto
-00001040: 725f 6466 2c0a 2020 2020 2020 2020 6c6f  r_df,.        lo
-00001050: 6f6b 6265 6869 6e64 5f64 6179 733d 3330  okbehind_days=30
-00001060: 2c0a 2020 2020 2020 2020 6661 6c6c 6261  ,.        fallba
-00001070: 636b 3d6e 702e 6e61 6e2c 0a20 2020 2020  ck=np.nan,.     
-00001080: 2020 2065 6e74 6974 795f 6964 5f63 6f6c     entity_id_col
-00001090: 5f6e 616d 653d 2269 6422 2c0a 2020 2020  _name="id",.    
-000010a0: 2020 2020 7265 736f 6c76 655f 6d75 6c74      resolve_mult
-000010b0: 6970 6c65 5f66 6e3d 6d65 616e 2c0a 2020  iple_fn=mean,.  
-000010c0: 2020 2020 2020 6665 6174 7572 655f 6e61        feature_na
-000010d0: 6d65 3d22 7465 7374 5f66 6561 7475 7265  me="test_feature
-000010e0: 222c 0a20 2020 2029 0a20 2020 206f 7574  ",.    ).    out
-000010f0: 636f 6d65 5f73 7065 6320 3d20 4f75 7463  come_spec = Outc
-00001100: 6f6d 6553 7065 6328 0a20 2020 2020 2020  omeSpec(.       
-00001110: 2076 616c 7565 735f 6466 3d6f 7574 636f   values_df=outco
-00001120: 6d65 5f64 662c 0a20 2020 2020 2020 206c  me_df,.        l
-00001130: 6f6f 6b61 6865 6164 5f64 6179 733d 3331  ookahead_days=31
-00001140: 2c0a 2020 2020 2020 2020 6661 6c6c 6261  ,.        fallba
-00001150: 636b 3d30 2c0a 2020 2020 2020 2020 656e  ck=0,.        en
-00001160: 7469 7479 5f69 645f 636f 6c5f 6e61 6d65  tity_id_col_name
-00001170: 3d22 6964 222c 0a20 2020 2020 2020 2072  ="id",.        r
-00001180: 6573 6f6c 7665 5f6d 756c 7469 706c 655f  esolve_multiple_
-00001190: 666e 3d6d 6178 696d 756d 2c0a 2020 2020  fn=maximum,.    
-000011a0: 2020 2020 6665 6174 7572 655f 6e61 6d65      feature_name
-000011b0: 3d22 7465 7374 5f6f 7574 636f 6d65 222c  ="test_outcome",
-000011c0: 0a20 2020 2020 2020 2069 6e63 6964 656e  .        inciden
-000011d0: 743d 4661 6c73 652c 0a20 2020 2029 0a0a  t=False,.    )..
-000011e0: 2020 2020 2320 496e 7374 616e 7469 6174      # Instantiat
-000011f0: 6520 5469 6d65 7365 7269 6573 466c 6174  e TimeseriesFlat
-00001200: 7465 6e65 7220 616e 6420 6164 6420 7468  tener and add th
-00001210: 6520 7370 6563 6966 6963 6174 696f 6e73  e specifications
-00001220: 0a20 2020 2066 726f 6d20 7469 6d65 7365  .    from timese
-00001230: 7269 6573 666c 6174 7465 6e65 7220 696d  riesflattener im
-00001240: 706f 7274 2054 696d 6573 6572 6965 7346  port TimeseriesF
-00001250: 6c61 7474 656e 6572 0a0a 2020 2020 7473  lattener..    ts
-00001260: 5f66 6c61 7474 656e 6572 203d 2054 696d  _flattener = Tim
-00001270: 6573 6572 6965 7346 6c61 7474 656e 6572  eseriesFlattener
-00001280: 280a 2020 2020 2020 2020 7072 6564 6963  (.        predic
-00001290: 7469 6f6e 5f74 696d 6573 5f64 663d 7072  tion_times_df=pr
-000012a0: 6564 6963 7469 6f6e 5f74 696d 6573 5f64  ediction_times_d
-000012b0: 662c 0a20 2020 2020 2020 2065 6e74 6974  f,.        entit
-000012c0: 795f 6964 5f63 6f6c 5f6e 616d 653d 2269  y_id_col_name="i
-000012d0: 6422 2c0a 2020 2020 2020 2020 7469 6d65  d",.        time
-000012e0: 7374 616d 705f 636f 6c5f 6e61 6d65 3d22  stamp_col_name="
-000012f0: 6461 7465 222c 0a20 2020 2020 2020 206e  date",.        n
-00001300: 5f77 6f72 6b65 7273 3d31 2c0a 2020 2020  _workers=1,.    
-00001310: 2020 2020 6472 6f70 5f70 7265 645f 7469      drop_pred_ti
-00001320: 6d65 735f 7769 7468 5f69 6e73 7566 6669  mes_with_insuffi
-00001330: 6369 656e 745f 6c6f 6f6b 5f64 6973 7461  cient_look_dista
-00001340: 6e63 653d 4661 6c73 652c 0a20 2020 2029  nce=False,.    )
-00001350: 0a20 2020 2074 735f 666c 6174 7465 6e65  .    ts_flattene
-00001360: 722e 6164 645f 7370 6563 285b 7072 6564  r.add_spec([pred
-00001370: 6963 746f 725f 7370 6563 2c20 6f75 7463  ictor_spec, outc
-00001380: 6f6d 655f 7370 6563 5d29 0a20 2020 2064  ome_spec]).    d
-00001390: 6620 3d20 7473 5f66 6c61 7474 656e 6572  f = ts_flattener
-000013a0: 2e67 6574 5f64 6628 290a 2020 2020 6466  .get_df().    df
-000013b0: 0a60 6060 0a4f 7574 7075 743a 0a0a 7c20  .```.Output:..| 
-000013c0: 2020 2020 207c 2020 2069 6420 7c20 6461       |   id | da
-000013d0: 7465 2020 2020 2020 2020 2020 2020 2020  te              
-000013e0: 2020 7c20 7072 6564 6963 7469 6f6e 5f74    | prediction_t
-000013f0: 696d 655f 7575 6964 2020 7c20 7072 6564  ime_uuid  | pred
-00001400: 5f74 6573 745f 6665 6174 7572 655f 7769  _test_feature_wi
-00001410: 7468 696e 5f33 305f 6461 7973 5f6d 6561  thin_30_days_mea
-00001420: 6e5f 6661 6c6c 6261 636b 5f6e 616e 207c  n_fallback_nan |
-00001430: 206f 7574 635f 7465 7374 5f6f 7574 636f   outc_test_outco
-00001440: 6d65 5f77 6974 6869 6e5f 3331 5f64 6179  me_within_31_day
-00001450: 735f 6d61 7869 6d75 6d5f 6661 6c6c 6261  s_maximum_fallba
-00001460: 636b 5f30 5f64 6963 686f 746f 6d6f 7573  ck_0_dichotomous
-00001470: 207c 0a7c 202d 2d2d 3a20 7c20 2d2d 2d3a   |.| ---: | ---:
-00001480: 207c 203a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   | :------------
-00001490: 2d2d 2d2d 2d2d 207c 203a 2d2d 2d2d 2d2d  ------ | :------
-000014a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c  -------------- |
-000014b0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
-000014c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000014d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000014e0: 2d2d 3a20 7c20 2d2d 2d2d 2d2d 2d2d 2d2d  --: | ----------
-000014f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001520: 2d2d 2d2d 3a20 7c0a 7c20 2020 2030 207c  ----: |.|    0 |
-00001530: 2020 2020 3120 7c20 3230 3230 2d30 312d      1 | 2020-01-
-00001540: 3031 2030 303a 3030 3a30 3020 7c20 312d  01 00:00:00 | 1-
-00001550: 3230 3230 2d30 312d 3031 2d30 302d 3030  2020-01-01-00-00
-00001560: 2d30 3020 7c20 2020 2020 2020 2020 2020  -00 |           
-00001570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001590: 2020 2020 2032 2e35 207c 2020 2020 2020       2.5 |      
-000015a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015d0: 2020 2020 2020 2020 2030 207c 0a7c 2020           0 |.|  
-000015e0: 2020 3120 7c20 2020 2031 207c 2032 3032    1 |    1 | 202
-000015f0: 302d 3032 2d30 3120 3030 3a30 303a 3030  0-02-01 00:00:00
-00001600: 207c 2031 2d32 3032 302d 3032 2d30 312d   | 1-2020-02-01-
-00001610: 3030 2d30 302d 3030 207c 2020 2020 2020  00-00-00 |      
-00001620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001640: 2020 2020 2020 2020 2020 2020 3120 7c20              1 | 
-00001650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001680: 2020 2020 2020 2020 2020 2020 2020 3120                1 
-00001690: 7c0a 7c20 2020 2032 207c 2020 2020 3220  |.|    2 |    2 
-000016a0: 7c20 3230 3230 2d30 322d 3031 2030 303a  | 2020-02-01 00:
-000016b0: 3030 3a30 3020 7c20 322d 3230 3230 2d30  00:00 | 2-2020-0
-000016c0: 322d 3031 2d30 302d 3030 2d30 3020 7c20  2-01-00-00-00 | 
-000016d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001700: 2034 207c 2020 2020 2020 2020 2020 2020   4 |            
-00001710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001740: 2020 2030 207c 0a0a 0a23 2320 f09f 9396     0 |...## ....
-00001750: 2044 6f63 756d 656e 7461 7469 6f6e 0a0a   Documentation..
-00001760: 7c20 446f 6375 6d65 6e74 6174 696f 6e20  | Documentation 
-00001770: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00001780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017d0: 2020 7c0a 7c20 2d2d 2d2d 2d2d 2d2d 2d2d    |.| ----------
-000017e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c 202d  ------------ | -
-000017f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001800: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001810: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001820: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001830: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001840: 2d2d 2d2d 2d20 7c0a 7c20 f09f 8e93 202a  ----- |.| .... *
-00001850: 2a5b 5475 746f 7269 616c 5d2a 2a20 2020  *[Tutorial]**   
-00001860: 2020 2020 7c20 5369 6d70 6c65 2061 6e64      | Simple and
-00001870: 2061 6476 616e 6365 6420 7475 746f 7269   advanced tutori
-00001880: 616c 7320 746f 2067 6574 2079 6f75 2073  als to get you s
-00001890: 7461 7274 6564 2075 7369 6e67 2060 7469  tarted using `ti
-000018a0: 6d65 7365 7269 6573 666c 6174 7465 6e65  meseriesflattene
-000018b0: 7260 2020 2020 2020 2020 2020 207c 0a7c  r`           |.|
-000018c0: 20f0 9f8e 9b20 2a2a 5b47 656e 6572 616c   .... **[General
-000018d0: 2064 6f63 735d 2a2a 207c 2054 6865 2064   docs]** | The d
-000018e0: 6574 6169 6c65 6420 7265 6665 7265 6e63  etailed referenc
-000018f0: 6520 666f 7220 7469 6d65 7365 7269 6573  e for timeseries
-00001900: 666c 6174 7465 6e65 7227 7320 4150 492e  flattener's API.
-00001910: 207c 0a7c 20f0 9f99 8b20 2a2a 5b46 4151   |.| .... **[FAQ
-00001920: 5d2a 2a20 2020 2020 2020 2020 2020 207c  ]**            |
-00001930: 2046 7265 7175 656e 746c 7920 6173 6b65   Frequently aske
-00001940: 6420 7175 6573 7469 6f6e 2020 2020 2020  d question      
-00001950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001980: 2020 2020 2020 2020 7c0a 7c20 f09f 97ba          |.| ....
-00001990: efb8 8f20 2a2a 5b52 6f61 646d 6170 5d2a  ... **[Roadmap]*
-000019a0: 2a20 2020 2020 2020 207c 204b 616e 6261  *        | Kanba
-000019b0: 6e20 626f 6172 6420 666f 7220 7468 6520  n board for the 
-000019c0: 726f 6164 6d61 7020 666f 7220 7468 6520  roadmap for the 
-000019d0: 7072 6f6a 6563 7420 2020 2020 2020 2020  project         
-000019e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a00: 2020 7c0a 0a5b 5475 746f 7269 616c 5d3a    |..[Tutorial]:
-00001a10: 2068 7474 7073 3a2f 2f61 6172 6875 732d   https://aarhus-
-00001a20: 7073 7963 6869 6174 7279 2d72 6573 6561  psychiatry-resea
-00001a30: 7263 682e 6769 7468 7562 2e69 6f2f 7469  rch.github.io/ti
-00001a40: 6d65 7365 7269 6573 666c 6174 7465 6e65  meseriesflattene
-00001a50: 722f 7475 746f 7269 616c 732e 6874 6d6c  r/tutorials.html
-00001a60: 0a5b 4765 6e65 7261 6c20 646f 6373 5d3a  .[General docs]:
-00001a70: 2068 7474 7073 3a2f 2f41 6172 6875 732d   https://Aarhus-
-00001a80: 5073 7963 6869 6174 7279 2d52 6573 6561  Psychiatry-Resea
-00001a90: 7263 682e 6769 7468 7562 2e69 6f2f 7469  rch.github.io/ti
-00001aa0: 6d65 7365 7269 6573 666c 6174 7465 6e65  meseriesflattene
-00001ab0: 722f 0a5b 4641 515d 3a20 6874 7470 733a  r/.[FAQ]: https:
-00001ac0: 2f2f 4161 7268 7573 2d50 7379 6368 6961  //Aarhus-Psychia
-00001ad0: 7472 792d 5265 7365 6172 6368 2e67 6974  try-Research.git
-00001ae0: 6875 622e 696f 2f74 696d 6573 6572 6965  hub.io/timeserie
-00001af0: 7366 6c61 7474 656e 6572 2f66 6171 2e68  sflattener/faq.h
-00001b00: 746d 6c0a 5b52 6f61 646d 6170 5d3a 2068  tml.[Roadmap]: h
-00001b10: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001b20: 6d2f 6f72 6773 2f41 6172 6875 732d 5073  m/orgs/Aarhus-Ps
-00001b30: 7963 6869 6174 7279 2d52 6573 6561 7263  ychiatry-Researc
-00001b40: 682f 7072 6f6a 6563 7473 2f31 312f 7669  h/projects/11/vi
-00001b50: 6577 732f 310a 0a23 2320 f09f 92ac 2057  ews/1..## .... W
-00001b60: 6865 7265 2074 6f20 6173 6b20 7175 6573  here to ask ques
-00001b70: 7469 6f6e 730a 0a7c 2054 7970 6520 2020  tions..| Type   
-00001b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b90: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00000150: 2e63 6f6d 3e0a 4c69 6365 6e73 653a 204d  .com>.License: M
+00000160: 4954 204c 6963 656e 7365 0a20 2020 2020  IT License.     
+00000170: 2020 200a 2020 2020 2020 2020 436f 7079     .        Copy
+00000180: 7269 6768 7420 2863 2920 3230 3232 2050  right (c) 2022 P
+00000190: 5359 434f 5020 4772 6f75 702c 2041 6172  SYCOP Group, Aar
+000001a0: 6875 7320 556e 6976 6572 7369 7479 0a20  hus University. 
+000001b0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000001c0: 5065 726d 6973 7369 6f6e 2069 7320 6865  Permission is he
+000001d0: 7265 6279 2067 7261 6e74 6564 2c20 6672  reby granted, fr
+000001e0: 6565 206f 6620 6368 6172 6765 2c20 746f  ee of charge, to
+000001f0: 2061 6e79 2070 6572 736f 6e20 6f62 7461   any person obta
+00000200: 696e 696e 6720 6120 636f 7079 0a20 2020  ining a copy.   
+00000210: 2020 2020 206f 6620 7468 6973 2073 6f66       of this sof
+00000220: 7477 6172 6520 616e 6420 6173 736f 6369  tware and associ
+00000230: 6174 6564 2064 6f63 756d 656e 7461 7469  ated documentati
+00000240: 6f6e 2066 696c 6573 2028 7468 6520 2253  on files (the "S
+00000250: 6f66 7477 6172 6522 292c 2074 6f20 6465  oftware"), to de
+00000260: 616c 0a20 2020 2020 2020 2069 6e20 7468  al.        in th
+00000270: 6520 536f 6674 7761 7265 2077 6974 686f  e Software witho
+00000280: 7574 2072 6573 7472 6963 7469 6f6e 2c20  ut restriction, 
+00000290: 696e 636c 7564 696e 6720 7769 7468 6f75  including withou
+000002a0: 7420 6c69 6d69 7461 7469 6f6e 2074 6865  t limitation the
+000002b0: 2072 6967 6874 730a 2020 2020 2020 2020   rights.        
+000002c0: 746f 2075 7365 2c20 636f 7079 2c20 6d6f  to use, copy, mo
+000002d0: 6469 6679 2c20 6d65 7267 652c 2070 7562  dify, merge, pub
+000002e0: 6c69 7368 2c20 6469 7374 7269 6275 7465  lish, distribute
+000002f0: 2c20 7375 626c 6963 656e 7365 2c20 616e  , sublicense, an
+00000300: 642f 6f72 2073 656c 6c0a 2020 2020 2020  d/or sell.      
+00000310: 2020 636f 7069 6573 206f 6620 7468 6520    copies of the 
+00000320: 536f 6674 7761 7265 2c20 616e 6420 746f  Software, and to
+00000330: 2070 6572 6d69 7420 7065 7273 6f6e 7320   permit persons 
+00000340: 746f 2077 686f 6d20 7468 6520 536f 6674  to whom the Soft
+00000350: 7761 7265 2069 730a 2020 2020 2020 2020  ware is.        
+00000360: 6675 726e 6973 6865 6420 746f 2064 6f20  furnished to do 
+00000370: 736f 2c20 7375 626a 6563 7420 746f 2074  so, subject to t
+00000380: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6e  he following con
+00000390: 6469 7469 6f6e 733a 0a20 2020 2020 2020  ditions:.       
+000003a0: 200a 2020 2020 2020 2020 5468 6520 6162   .        The ab
+000003b0: 6f76 6520 636f 7079 7269 6768 7420 6e6f  ove copyright no
+000003c0: 7469 6365 2061 6e64 2074 6869 7320 7065  tice and this pe
+000003d0: 726d 6973 7369 6f6e 206e 6f74 6963 6520  rmission notice 
+000003e0: 7368 616c 6c20 6265 2069 6e63 6c75 6465  shall be include
+000003f0: 6420 696e 2061 6c6c 0a20 2020 2020 2020  d in all.       
+00000400: 2063 6f70 6965 7320 6f72 2073 7562 7374   copies or subst
+00000410: 616e 7469 616c 2070 6f72 7469 6f6e 7320  antial portions 
+00000420: 6f66 2074 6865 2053 6f66 7477 6172 652e  of the Software.
+00000430: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00000440: 2020 5448 4520 534f 4654 5741 5245 2049    THE SOFTWARE I
+00000450: 5320 5052 4f56 4944 4544 2022 4153 2049  S PROVIDED "AS I
+00000460: 5322 2c20 5749 5448 4f55 5420 5741 5252  S", WITHOUT WARR
+00000470: 414e 5459 204f 4620 414e 5920 4b49 4e44  ANTY OF ANY KIND
+00000480: 2c20 4558 5052 4553 5320 4f52 0a20 2020  , EXPRESS OR.   
+00000490: 2020 2020 2049 4d50 4c49 4544 2c20 494e       IMPLIED, IN
+000004a0: 434c 5544 494e 4720 4255 5420 4e4f 5420  CLUDING BUT NOT 
+000004b0: 4c49 4d49 5445 4420 544f 2054 4845 2057  LIMITED TO THE W
+000004c0: 4152 5241 4e54 4945 5320 4f46 204d 4552  ARRANTIES OF MER
+000004d0: 4348 414e 5441 4249 4c49 5459 2c0a 2020  CHANTABILITY,.  
+000004e0: 2020 2020 2020 4649 544e 4553 5320 464f        FITNESS FO
+000004f0: 5220 4120 5041 5254 4943 554c 4152 2050  R A PARTICULAR P
+00000500: 5552 504f 5345 2041 4e44 204e 4f4e 494e  URPOSE AND NONIN
+00000510: 4652 494e 4745 4d45 4e54 2e20 494e 204e  FRINGEMENT. IN N
+00000520: 4f20 4556 454e 5420 5348 414c 4c20 5448  O EVENT SHALL TH
+00000530: 450a 2020 2020 2020 2020 4155 5448 4f52  E.        AUTHOR
+00000540: 5320 4f52 2043 4f50 5952 4947 4854 2048  S OR COPYRIGHT H
+00000550: 4f4c 4445 5253 2042 4520 4c49 4142 4c45  OLDERS BE LIABLE
+00000560: 2046 4f52 2041 4e59 2043 4c41 494d 2c20   FOR ANY CLAIM, 
+00000570: 4441 4d41 4745 5320 4f52 204f 5448 4552  DAMAGES OR OTHER
+00000580: 0a20 2020 2020 2020 204c 4941 4249 4c49  .        LIABILI
+00000590: 5459 2c20 5748 4554 4845 5220 494e 2041  TY, WHETHER IN A
+000005a0: 4e20 4143 5449 4f4e 204f 4620 434f 4e54  N ACTION OF CONT
+000005b0: 5241 4354 2c20 544f 5254 204f 5220 4f54  RACT, TORT OR OT
+000005c0: 4845 5257 4953 452c 2041 5249 5349 4e47  HERWISE, ARISING
+000005d0: 2046 524f 4d2c 0a20 2020 2020 2020 204f   FROM,.        O
+000005e0: 5554 204f 4620 4f52 2049 4e20 434f 4e4e  UT OF OR IN CONN
+000005f0: 4543 5449 4f4e 2057 4954 4820 5448 4520  ECTION WITH THE 
+00000600: 534f 4654 5741 5245 204f 5220 5448 4520  SOFTWARE OR THE 
+00000610: 5553 4520 4f52 204f 5448 4552 2044 4541  USE OR OTHER DEA
+00000620: 4c49 4e47 5320 494e 2054 4845 0a20 2020  LINGS IN THE.   
+00000630: 2020 2020 2053 4f46 5457 4152 452e 0a50       SOFTWARE..P
+00000640: 726f 6a65 6374 2d55 524c 3a20 686f 6d65  roject-URL: home
+00000650: 7061 6765 2c20 6874 7470 733a 2f2f 6769  page, https://gi
+00000660: 7468 7562 2e63 6f6d 2f4d 6172 7469 6e42  thub.com/MartinB
+00000670: 6572 6e73 746f 7266 662f 7469 6d65 7365  ernstorff/timese
+00000680: 7269 6573 666c 6174 7465 6e65 720a 5072  riesflattener.Pr
+00000690: 6f6a 6563 742d 5552 4c3a 2072 6570 6f73  oject-URL: repos
+000006a0: 6974 6f72 792c 2068 7474 7073 3a2f 2f67  itory, https://g
+000006b0: 6974 6875 622e 636f 6d2f 4d61 7274 696e  ithub.com/Martin
+000006c0: 4265 726e 7374 6f72 6666 2f74 696d 6573  Bernstorff/times
+000006d0: 6572 6965 7366 6c61 7474 656e 6572 0a50  eriesflattener.P
+000006e0: 726f 6a65 6374 2d55 524c 3a20 646f 6375  roject-URL: docu
+000006f0: 6d65 6e74 6174 696f 6e2c 2068 7474 7073  mentation, https
+00000700: 3a2f 2f4d 6172 7469 6e42 6572 6e73 746f  ://MartinBernsto
+00000710: 7266 662e 6769 7468 7562 2e69 6f2f 7469  rff.github.io/ti
+00000720: 6d65 7365 7269 6573 666c 6174 7465 6e65  meseriesflattene
+00000730: 722f 0a43 6c61 7373 6966 6965 723a 204f  r/.Classifier: O
+00000740: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+00000750: 3a3a 2050 4f53 4958 203a 3a20 4c69 6e75  :: POSIX :: Linu
+00000760: 780a 436c 6173 7369 6669 6572 3a20 4f70  x.Classifier: Op
+00000770: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
+00000780: 3a20 4d61 634f 5320 3a3a 204d 6163 4f53  : MacOS :: MacOS
+00000790: 2058 0a43 6c61 7373 6966 6965 723a 204f   X.Classifier: O
+000007a0: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+000007b0: 3a3a 204d 6963 726f 736f 6674 203a 3a20  :: Microsoft :: 
+000007c0: 5769 6e64 6f77 730a 436c 6173 7369 6669  Windows.Classifi
+000007d0: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+000007e0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000007f0: 6f6e 203a 3a20 332e 380a 436c 6173 7369  on :: 3.8.Classi
+00000800: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+00000810: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000820: 7468 6f6e 203a 3a20 332e 390a 436c 6173  thon :: 3.9.Clas
+00000830: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00000840: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000850: 5079 7468 6f6e 203a 3a20 332e 3130 0a43  Python :: 3.10.C
+00000860: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+00000870: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000880: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
+00000890: 310a 5265 7175 6972 6573 2d50 7974 686f  1.Requires-Pytho
+000008a0: 6e3a 203c 332e 3132 2e30 2c3e 3d33 2e38  n: <3.12.0,>=3.8
+000008b0: 2e30 0a44 6573 6372 6970 7469 6f6e 2d43  .0.Description-C
+000008c0: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
+000008d0: 742f 6d61 726b 646f 776e 0a50 726f 7669  t/markdown.Provi
+000008e0: 6465 732d 4578 7472 613a 2064 6576 0a50  des-Extra: dev.P
+000008f0: 726f 7669 6465 732d 4578 7472 613a 2074  rovides-Extra: t
+00000900: 6573 740a 5072 6f76 6964 6573 2d45 7874  est.Provides-Ext
+00000910: 7261 3a20 646f 6373 0a50 726f 7669 6465  ra: docs.Provide
+00000920: 732d 4578 7472 613a 2074 7574 6f72 6961  s-Extra: tutoria
+00000930: 6c73 0a50 726f 7669 6465 732d 4578 7472  ls.Provides-Extr
+00000940: 613a 2074 6578 740a 4c69 6365 6e73 652d  a: text.License-
+00000950: 4669 6c65 3a20 4c49 4345 4e53 450a 0a3c  File: LICENSE..<
+00000960: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000970: 6769 7468 7562 2e63 6f6d 2f41 6172 6875  github.com/Aarhu
+00000980: 732d 5073 7963 6869 6174 7279 2d52 6573  s-Psychiatry-Res
+00000990: 6561 7263 682f 7469 6d65 7365 7269 6573  earch/timeseries
+000009a0: 666c 6174 7465 6e65 7222 3e3c 696d 6720  flattener"><img 
+000009b0: 7372 633d 2268 7474 7073 3a2f 2f67 6974  src="https://git
+000009c0: 6875 622e 636f 6d2f 4161 7268 7573 2d50  hub.com/Aarhus-P
+000009d0: 7379 6368 6961 7472 792d 5265 7365 6172  sychiatry-Resear
+000009e0: 6368 2f74 696d 6573 6572 6965 7366 6c61  ch/timeseriesfla
+000009f0: 7474 656e 6572 2f62 6c6f 622f 6d61 696e  ttener/blob/main
+00000a00: 2f64 6f63 732f 5f73 7461 7469 632f 6963  /docs/_static/ic
+00000a10: 6f6e 2e70 6e67 3f72 6177 3d74 7275 6522  on.png?raw=true"
+00000a20: 2077 6964 7468 3d22 3230 3022 2061 6c69   width="200" ali
+00000a30: 676e 3d22 7269 6768 7422 2f3e 3c2f 613e  gn="right"/></a>
+00000a40: 0a0a 2320 5469 6d65 7365 7269 6573 666c  ..# Timeseriesfl
+00000a50: 6174 7465 6e65 720a 0a5b 215b 6769 7468  attener..[![gith
+00000a60: 7562 2061 6374 696f 6e73 2064 6f63 735d  ub actions docs]
+00000a70: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000a80: 636f 6d2f 4161 7268 7573 2d50 7379 6368  com/Aarhus-Psych
+00000a90: 6961 7472 792d 5265 7365 6172 6368 2f74  iatry-Research/t
+00000aa0: 696d 6573 6572 6965 7366 6c61 7474 656e  imeseriesflatten
+00000ab0: 6572 2f61 6374 696f 6e73 2f77 6f72 6b66  er/actions/workf
+00000ac0: 6c6f 7773 2f64 6f63 756d 656e 7461 7469  lows/documentati
+00000ad0: 6f6e 2e79 6d6c 2f62 6164 6765 2e73 7667  on.yml/badge.svg
+00000ae0: 295d 2868 7474 7073 3a2f 2f61 6172 6875  )](https://aarhu
+00000af0: 732d 7073 7963 6869 6174 7279 2d72 6573  s-psychiatry-res
+00000b00: 6561 7263 682e 6769 7468 7562 2e69 6f2f  earch.github.io/
+00000b10: 7469 6d65 7365 7269 6573 666c 6174 7465  timeseriesflatte
+00000b20: 6e65 722f 290a 5b21 5b67 6974 6875 6220  ner/).[![github 
+00000b30: 6163 7469 6f6e 7320 7079 7465 7374 5d28  actions pytest](
+00000b40: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000b50: 6f6d 2f41 6172 6875 732d 5073 7963 6869  om/Aarhus-Psychi
+00000b60: 6174 7279 2d52 6573 6561 7263 682f 7469  atry-Research/ti
+00000b70: 6d65 7365 7269 6573 666c 6174 7465 6e65  meseriesflattene
+00000b80: 722f 6163 7469 6f6e 732f 776f 726b 666c  r/actions/workfl
+00000b90: 6f77 732f 6d61 696e 5f74 6573 745f 616e  ows/main_test_an
+00000ba0: 645f 7265 6c65 6173 652e 796d 6c2f 6261  d_release.yml/ba
+00000bb0: 6467 652e 7376 6729 5d28 6874 7470 733a  dge.svg)](https:
+00000bc0: 2f2f 6769 7468 7562 2e63 6f6d 2f41 6172  //github.com/Aar
+00000bd0: 6875 732d 5073 7963 6869 6174 7279 2d52  hus-Psychiatry-R
+00000be0: 6573 6561 7263 682f 7469 6d65 7365 7269  esearch/timeseri
+00000bf0: 6573 666c 6174 7465 6e65 722f 6163 7469  esflattener/acti
+00000c00: 6f6e 7329 0a5b 215b 7079 7468 6f6e 2076  ons).[![python v
+00000c10: 6572 7369 6f6e 735d 2868 7474 7073 3a2f  ersions](https:/
+00000c20: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000c30: 7079 7069 2f70 7976 6572 7369 6f6e 732f  pypi/pyversions/
+00000c40: 7469 6d65 7365 7269 6573 666c 6174 7465  timeseriesflatte
+00000c50: 6e65 7229 5d28 6874 7470 733a 2f2f 7079  ner)](https://py
+00000c60: 7069 2e6f 7267 2f70 726f 6a65 6374 2f74  pi.org/project/t
+00000c70: 696d 6573 6572 6965 7366 6c61 7474 656e  imeseriesflatten
+00000c80: 6572 2f29 0a5b 215b 436f 6465 2073 7479  er/).[![Code sty
+00000c90: 6c65 3a20 626c 6163 6b5d 2868 7474 7073  le: black](https
+00000ca0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000cb0: 6f2f 6261 6467 652f 436f 6465 2532 3053  o/badge/Code%20S
+00000cc0: 7479 6c65 2d42 6c61 636b 2d62 6c61 636b  tyle-Black-black
+00000cd0: 295d 2868 7474 7073 3a2f 2f62 6c61 636b  )](https://black
+00000ce0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00000cf0: 656e 2f73 7461 626c 652f 7468 655f 626c  en/stable/the_bl
+00000d00: 6163 6b5f 636f 6465 5f73 7479 6c65 2f63  ack_code_style/c
+00000d10: 7572 7265 6e74 5f73 7479 6c65 2e68 746d  urrent_style.htm
+00000d20: 6c29 0a0a 5b21 5b50 7950 4920 7665 7273  l)..[![PyPI vers
+00000d30: 696f 6e5d 2868 7474 7073 3a2f 2f62 6164  ion](https://bad
+00000d40: 6765 2e66 7572 792e 696f 2f70 792f 7469  ge.fury.io/py/ti
+00000d50: 6d65 7365 7269 6573 666c 6174 7465 6e65  meseriesflattene
+00000d60: 722e 7376 6729 5d28 6874 7470 733a 2f2f  r.svg)](https://
+00000d70: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+00000d80: 2f74 696d 6573 6572 6965 7366 6c61 7474  /timeseriesflatt
+00000d90: 656e 6572 2f29 0a5b 215b 7374 6174 7573  ener/).[![status
+00000da0: 5d28 6874 7470 733a 2f2f 6a6f 7373 2e74  ](https://joss.t
+00000db0: 6865 6f6a 2e6f 7267 2f70 6170 6572 732f  heoj.org/papers/
+00000dc0: 3362 6265 6138 3734 3536 3638 6431 6161  3bbea8745668d1aa
+00000dd0: 3430 6666 3739 3663 3666 6433 6462 3837  40ff796c6fd3db87
+00000de0: 2f73 7461 7475 732e 7376 6729 5d28 6874  /status.svg)](ht
+00000df0: 7470 733a 2f2f 6a6f 7373 2e74 6865 6f6a  tps://joss.theoj
+00000e00: 2e6f 7267 2f70 6170 6572 732f 3362 6265  .org/papers/3bbe
+00000e10: 6138 3734 3536 3638 6431 6161 3430 6666  a8745668d1aa40ff
+00000e20: 3739 3663 3666 6433 6462 3837 290a 0a54  796c6fd3db87)..T
+00000e30: 696d 6520 7365 7269 6573 2066 726f 6d20  ime series from 
+00000e40: 652e 672e 2065 6c65 6374 726f 6e69 6320  e.g. electronic 
+00000e50: 6865 616c 7468 2072 6563 6f72 6473 206f  health records o
+00000e60: 6674 656e 2068 6176 6520 6120 6c61 7267  ften have a larg
+00000e70: 6520 6e75 6d62 6572 206f 6620 7661 7269  e number of vari
+00000e80: 6162 6c65 732c 2061 7265 2073 616d 706c  ables, are sampl
+00000e90: 6564 2061 7420 6972 7265 6775 6c61 7220  ed at irregular 
+00000ea0: 696e 7465 7276 616c 7320 616e 6420 7465  intervals and te
+00000eb0: 6e64 2074 6f20 6861 7665 2061 206c 6172  nd to have a lar
+00000ec0: 6765 206e 756d 6265 7220 6f66 206d 6973  ge number of mis
+00000ed0: 7369 6e67 2076 616c 7565 732e 2042 6566  sing values. Bef
+00000ee0: 6f72 6520 7468 6973 2074 7970 6520 6f66  ore this type of
+00000ef0: 2064 6174 6120 6361 6e20 6265 2075 7365   data can be use
+00000f00: 6420 666f 7220 7072 6564 6963 7469 6f6e  d for prediction
+00000f10: 206d 6f64 656c 6c69 6e67 2077 6974 6820   modelling with 
+00000f20: 6d61 6368 696e 6520 6c65 6172 6e69 6e67  machine learning
+00000f30: 206d 6574 686f 6473 2073 7563 6820 6173   methods such as
+00000f40: 206c 6f67 6973 7469 6320 7265 6772 6573   logistic regres
+00000f50: 7369 6f6e 206f 7220 5847 426f 6f73 742c  sion or XGBoost,
+00000f60: 2074 6865 2064 6174 6120 6e65 6564 7320   the data needs 
+00000f70: 746f 2062 6520 7265 7368 6170 6564 2e20  to be reshaped. 
+00000f80: 0a0a 496e 2065 7373 656e 6365 2c20 7468  ..In essence, th
+00000f90: 6520 7469 6d65 2073 6572 6965 7320 6e65  e time series ne
+00000fa0: 6564 2074 6f20 6265 202a 666c 6174 7465  ed to be *flatte
+00000fb0: 6e65 642a 2073 6f20 7468 6174 2065 6163  ned* so that eac
+00000fc0: 6820 7072 6564 6963 7469 6f6e 2074 696d  h prediction tim
+00000fd0: 6520 6973 2072 6570 7265 7365 6e74 6564  e is represented
+00000fe0: 2062 7920 6120 7365 7420 6f66 2070 7265   by a set of pre
+00000ff0: 6469 6374 6f72 2076 616c 7565 7320 616e  dictor values an
+00001000: 6420 616e 206f 7574 636f 6d65 2076 616c  d an outcome val
+00001010: 7565 2e20 5468 6573 6520 7072 6564 6963  ue. These predic
+00001020: 746f 7220 7661 6c75 6573 2063 616e 2062  tor values can b
+00001030: 6520 636f 6e73 7472 7563 7465 6420 6279  e constructed by
+00001040: 2061 6767 7265 6761 7469 6e67 2074 6865   aggregating the
+00001050: 2070 7265 6365 6469 6e67 2076 616c 7565   preceding value
+00001060: 7320 696e 2074 6865 2074 696d 6520 7365  s in the time se
+00001070: 7269 6573 2077 6974 6869 6e20 6120 6365  ries within a ce
+00001080: 7274 6169 6e20 7469 6d65 2077 696e 646f  rtain time windo
+00001090: 772e 200a 0a60 7469 6d65 7365 7269 6573  w. ..`timeseries
+000010a0: 666c 6174 7465 6e65 7260 2061 696d 7320  flattener` aims 
+000010b0: 746f 2073 696d 706c 6966 7920 7468 6973  to simplify this
+000010c0: 2070 726f 6365 7373 2062 7920 7072 6f76   process by prov
+000010d0: 6964 696e 6720 616e 2065 6173 792d 746f  iding an easy-to
+000010e0: 2d75 7365 2061 6e64 2066 756c 6c79 2d73  -use and fully-s
+000010f0: 7065 6369 6669 6564 2070 6970 656c 696e  pecified pipelin
+00001100: 6520 666f 7220 666c 6174 7465 6e69 6e67  e for flattening
+00001110: 2063 6f6d 706c 6578 2074 696d 6520 7365   complex time se
+00001120: 7269 6573 2e20 0a0a 2323 20f0 9f94 a720  ries. ..## .... 
+00001130: 496e 7374 616c 6c61 7469 6f6e 0a54 6f20  Installation.To 
+00001140: 6765 7420 7374 6172 7465 6420 7573 696e  get started usin
+00001150: 6720 7469 6d65 7365 7269 6573 666c 6174  g timeseriesflat
+00001160: 7465 6e65 7220 7369 6d70 6c79 2069 6e73  tener simply ins
+00001170: 7461 6c6c 2069 7420 7573 696e 6720 7069  tall it using pi
+00001180: 7020 6279 2072 756e 6e69 6e67 2074 6865  p by running the
+00001190: 2066 6f6c 6c6f 7769 6e67 206c 696e 6520   following line 
+000011a0: 696e 2079 6f75 7220 7465 726d 696e 616c  in your terminal
+000011b0: 3a0a 0a60 6060 0a70 6970 2069 6e73 7461  :..```.pip insta
+000011c0: 6c6c 2074 696d 6573 6572 6965 7366 6c61  ll timeseriesfla
+000011d0: 7474 656e 6572 0a60 6060 0a0a 2323 20e2  ttener.```..## .
+000011e0: 9aa1 2051 7569 636b 2073 7461 7274 0a0a  .. Quick start..
+000011f0: 6060 6070 790a 696d 706f 7274 206e 756d  ```py.import num
+00001200: 7079 2061 7320 6e70 0a69 6d70 6f72 7420  py as np.import 
+00001210: 7061 6e64 6173 2061 7320 7064 0a0a 6966  pandas as pd..if
+00001220: 205f 5f6e 616d 655f 5f20 3d3d 2022 5f5f   __name__ == "__
+00001230: 6d61 696e 5f5f 223a 0a0a 2020 2020 2320  main__":..    # 
+00001240: 4c6f 6164 2061 2064 6174 6166 7261 6d65  Load a dataframe
+00001250: 2077 6974 6820 7469 6d65 7320 796f 7520   with times you 
+00001260: 7769 7368 2074 6f20 6d61 6b65 2061 2070  wish to make a p
+00001270: 7265 6469 6374 696f 6e0a 2020 2020 7072  rediction.    pr
+00001280: 6564 6963 7469 6f6e 5f74 696d 6573 5f64  ediction_times_d
+00001290: 6620 3d20 7064 2e44 6174 6146 7261 6d65  f = pd.DataFrame
+000012a0: 280a 2020 2020 2020 2020 7b0a 2020 2020  (.        {.    
+000012b0: 2020 2020 2020 2020 2269 6422 3a20 5b31          "id": [1
+000012c0: 2c20 312c 2032 5d2c 0a20 2020 2020 2020  , 1, 2],.       
+000012d0: 2020 2020 2022 6461 7465 223a 205b 2232       "date": ["2
+000012e0: 3032 302d 3031 2d30 3122 2c20 2232 3032  020-01-01", "202
+000012f0: 302d 3032 2d30 3122 2c20 2232 3032 302d  0-02-01", "2020-
+00001300: 3032 2d30 3122 5d2c 0a20 2020 2020 2020  02-01"],.       
+00001310: 207d 2c0a 2020 2020 290a 2020 2020 2320   },.    ).    # 
+00001320: 4c6f 6164 2061 2064 6174 6166 7261 6d65  Load a dataframe
+00001330: 2077 6974 6820 7261 7720 7661 6c75 6573   with raw values
+00001340: 2079 6f75 2077 6973 6820 746f 2061 6767   you wish to agg
+00001350: 7265 6761 7465 2061 7320 7072 6564 6963  regate as predic
+00001360: 746f 7273 0a20 2020 2070 7265 6469 6374  tors.    predict
+00001370: 6f72 5f64 6620 3d20 7064 2e44 6174 6146  or_df = pd.DataF
+00001380: 7261 6d65 280a 2020 2020 2020 2020 7b0a  rame(.        {.
+00001390: 2020 2020 2020 2020 2020 2020 2269 6422              "id"
+000013a0: 3a20 5b31 2c20 312c 2031 2c20 325d 2c0a  : [1, 1, 1, 2],.
+000013b0: 2020 2020 2020 2020 2020 2020 2264 6174              "dat
+000013c0: 6522 3a20 5b0a 2020 2020 2020 2020 2020  e": [.          
+000013d0: 2020 2020 2020 2232 3032 302d 3031 2d31        "2020-01-1
+000013e0: 3522 2c0a 2020 2020 2020 2020 2020 2020  5",.            
+000013f0: 2020 2020 2232 3031 392d 3132 2d31 3022      "2019-12-10"
+00001400: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001410: 2020 2232 3031 392d 3132 2d31 3522 2c0a    "2019-12-15",.
+00001420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001430: 2232 3032 302d 3031 2d30 3222 2c0a 2020  "2020-01-02",.  
+00001440: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
+00001450: 2020 2020 2020 2020 2022 7661 6c75 6522           "value"
+00001460: 3a20 5b31 2c20 322c 2033 2c20 345d 2c0a  : [1, 2, 3, 4],.
+00001470: 2020 2020 2020 2020 7d2c 0a20 2020 2029          },.    )
+00001480: 0a20 2020 2023 204c 6f61 6420 6120 6461  .    # Load a da
+00001490: 7461 6672 616d 6520 7370 6563 6966 7969  taframe specifyi
+000014a0: 6e67 2077 6865 6e20 7468 6520 6f75 7463  ng when the outc
+000014b0: 6f6d 6520 6f63 6375 7273 0a20 2020 206f  ome occurs.    o
+000014c0: 7574 636f 6d65 5f64 6620 3d20 7064 2e44  utcome_df = pd.D
+000014d0: 6174 6146 7261 6d65 287b 2269 6422 3a20  ataFrame({"id": 
+000014e0: 5b31 5d2c 2022 6461 7465 223a 205b 2232  [1], "date": ["2
+000014f0: 3032 302d 3033 2d30 3122 5d2c 2022 7661  020-03-01"], "va
+00001500: 6c75 6522 3a20 5b31 5d7d 290a 0a20 2020  lue": [1]})..   
+00001510: 2023 2053 7065 6369 6679 2068 6f77 2074   # Specify how t
+00001520: 6f20 6167 6772 6567 6174 6520 7468 6520  o aggregate the 
+00001530: 7072 6564 6963 746f 7273 2061 6e64 2064  predictors and d
+00001540: 6566 696e 6520 7468 6520 6f75 7463 6f6d  efine the outcom
+00001550: 650a 2020 2020 6672 6f6d 2074 696d 6573  e.    from times
+00001560: 6572 6965 7366 6c61 7474 656e 6572 2e66  eriesflattener.f
+00001570: 6561 7475 7265 5f73 7065 635f 6f62 6a65  eature_spec_obje
+00001580: 6374 7320 696d 706f 7274 204f 7574 636f  cts import Outco
+00001590: 6d65 5370 6563 2c20 5072 6564 6963 746f  meSpec, Predicto
+000015a0: 7253 7065 630a 2020 2020 6672 6f6d 2074  rSpec.    from t
+000015b0: 696d 6573 6572 6965 7366 6c61 7474 656e  imeseriesflatten
+000015c0: 6572 2e72 6573 6f6c 7665 5f6d 756c 7469  er.resolve_multi
+000015d0: 706c 655f 6675 6e63 7469 6f6e 7320 696d  ple_functions im
+000015e0: 706f 7274 206d 6178 696d 756d 2c20 6d65  port maximum, me
+000015f0: 616e 0a0a 2020 2020 7072 6564 6963 746f  an..    predicto
+00001600: 725f 7370 6563 203d 2050 7265 6469 6374  r_spec = Predict
+00001610: 6f72 5370 6563 280a 2020 2020 2020 2020  orSpec(.        
+00001620: 7661 6c75 6573 5f64 663d 7072 6564 6963  values_df=predic
+00001630: 746f 725f 6466 2c0a 2020 2020 2020 2020  tor_df,.        
+00001640: 6c6f 6f6b 6265 6869 6e64 5f64 6179 733d  lookbehind_days=
+00001650: 3330 2c0a 2020 2020 2020 2020 6661 6c6c  30,.        fall
+00001660: 6261 636b 3d6e 702e 6e61 6e2c 0a20 2020  back=np.nan,.   
+00001670: 2020 2020 2065 6e74 6974 795f 6964 5f63       entity_id_c
+00001680: 6f6c 5f6e 616d 653d 2269 6422 2c0a 2020  ol_name="id",.  
+00001690: 2020 2020 2020 7265 736f 6c76 655f 6d75        resolve_mu
+000016a0: 6c74 6970 6c65 5f66 6e3d 6d65 616e 2c0a  ltiple_fn=mean,.
+000016b0: 2020 2020 2020 2020 6665 6174 7572 655f          feature_
+000016c0: 6e61 6d65 3d22 7465 7374 5f66 6561 7475  name="test_featu
+000016d0: 7265 222c 0a20 2020 2029 0a20 2020 206f  re",.    ).    o
+000016e0: 7574 636f 6d65 5f73 7065 6320 3d20 4f75  utcome_spec = Ou
+000016f0: 7463 6f6d 6553 7065 6328 0a20 2020 2020  tcomeSpec(.     
+00001700: 2020 2076 616c 7565 735f 6466 3d6f 7574     values_df=out
+00001710: 636f 6d65 5f64 662c 0a20 2020 2020 2020  come_df,.       
+00001720: 206c 6f6f 6b61 6865 6164 5f64 6179 733d   lookahead_days=
+00001730: 3331 2c0a 2020 2020 2020 2020 6661 6c6c  31,.        fall
+00001740: 6261 636b 3d30 2c0a 2020 2020 2020 2020  back=0,.        
+00001750: 656e 7469 7479 5f69 645f 636f 6c5f 6e61  entity_id_col_na
+00001760: 6d65 3d22 6964 222c 0a20 2020 2020 2020  me="id",.       
+00001770: 2072 6573 6f6c 7665 5f6d 756c 7469 706c   resolve_multipl
+00001780: 655f 666e 3d6d 6178 696d 756d 2c0a 2020  e_fn=maximum,.  
+00001790: 2020 2020 2020 6665 6174 7572 655f 6e61        feature_na
+000017a0: 6d65 3d22 7465 7374 5f6f 7574 636f 6d65  me="test_outcome
+000017b0: 222c 0a20 2020 2020 2020 2069 6e63 6964  ",.        incid
+000017c0: 656e 743d 4661 6c73 652c 0a20 2020 2029  ent=False,.    )
+000017d0: 0a0a 2020 2020 2320 496e 7374 616e 7469  ..    # Instanti
+000017e0: 6174 6520 5469 6d65 7365 7269 6573 466c  ate TimeseriesFl
+000017f0: 6174 7465 6e65 7220 616e 6420 6164 6420  attener and add 
+00001800: 7468 6520 7370 6563 6966 6963 6174 696f  the specificatio
+00001810: 6e73 0a20 2020 2066 726f 6d20 7469 6d65  ns.    from time
+00001820: 7365 7269 6573 666c 6174 7465 6e65 7220  seriesflattener 
+00001830: 696d 706f 7274 2054 696d 6573 6572 6965  import Timeserie
+00001840: 7346 6c61 7474 656e 6572 0a0a 2020 2020  sFlattener..    
+00001850: 7473 5f66 6c61 7474 656e 6572 203d 2054  ts_flattener = T
+00001860: 696d 6573 6572 6965 7346 6c61 7474 656e  imeseriesFlatten
+00001870: 6572 280a 2020 2020 2020 2020 7072 6564  er(.        pred
+00001880: 6963 7469 6f6e 5f74 696d 6573 5f64 663d  iction_times_df=
+00001890: 7072 6564 6963 7469 6f6e 5f74 696d 6573  prediction_times
+000018a0: 5f64 662c 0a20 2020 2020 2020 2065 6e74  _df,.        ent
+000018b0: 6974 795f 6964 5f63 6f6c 5f6e 616d 653d  ity_id_col_name=
+000018c0: 2269 6422 2c0a 2020 2020 2020 2020 7469  "id",.        ti
+000018d0: 6d65 7374 616d 705f 636f 6c5f 6e61 6d65  mestamp_col_name
+000018e0: 3d22 6461 7465 222c 0a20 2020 2020 2020  ="date",.       
+000018f0: 206e 5f77 6f72 6b65 7273 3d31 2c0a 2020   n_workers=1,.  
+00001900: 2020 2020 2020 6472 6f70 5f70 7265 645f        drop_pred_
+00001910: 7469 6d65 735f 7769 7468 5f69 6e73 7566  times_with_insuf
+00001920: 6669 6369 656e 745f 6c6f 6f6b 5f64 6973  ficient_look_dis
+00001930: 7461 6e63 653d 4661 6c73 652c 0a20 2020  tance=False,.   
+00001940: 2029 0a20 2020 2074 735f 666c 6174 7465   ).    ts_flatte
+00001950: 6e65 722e 6164 645f 7370 6563 285b 7072  ner.add_spec([pr
+00001960: 6564 6963 746f 725f 7370 6563 2c20 6f75  edictor_spec, ou
+00001970: 7463 6f6d 655f 7370 6563 5d29 0a20 2020  tcome_spec]).   
+00001980: 2064 6620 3d20 7473 5f66 6c61 7474 656e   df = ts_flatten
+00001990: 6572 2e67 6574 5f64 6628 290a 2020 2020  er.get_df().    
+000019a0: 6466 0a60 6060 0a4f 7574 7075 743a 0a0a  df.```.Output:..
+000019b0: 7c20 2020 2020 207c 2020 2069 6420 7c20  |      |   id | 
+000019c0: 6461 7465 2020 2020 2020 2020 2020 2020  date            
+000019d0: 2020 2020 7c20 7072 6564 6963 7469 6f6e      | prediction
+000019e0: 5f74 696d 655f 7575 6964 2020 7c20 7072  _time_uuid  | pr
+000019f0: 6564 5f74 6573 745f 6665 6174 7572 655f  ed_test_feature_
+00001a00: 7769 7468 696e 5f33 305f 6461 7973 5f6d  within_30_days_m
+00001a10: 6561 6e5f 6661 6c6c 6261 636b 5f6e 616e  ean_fallback_nan
+00001a20: 207c 206f 7574 635f 7465 7374 5f6f 7574   | outc_test_out
+00001a30: 636f 6d65 5f77 6974 6869 6e5f 3331 5f64  come_within_31_d
+00001a40: 6179 735f 6d61 7869 6d75 6d5f 6661 6c6c  ays_maximum_fall
+00001a50: 6261 636b 5f30 5f64 6963 686f 746f 6d6f  back_0_dichotomo
+00001a60: 7573 207c 0a7c 202d 2d2d 3a20 7c20 2d2d  us |.| ---: | --
+00001a70: 2d3a 207c 203a 2d2d 2d2d 2d2d 2d2d 2d2d  -: | :----------
+00001a80: 2d2d 2d2d 2d2d 2d2d 207c 203a 2d2d 2d2d  -------- | :----
+00001a90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001aa0: 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   | -------------
+00001ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001ac0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001ad0: 2d2d 2d2d 3a20 7c20 2d2d 2d2d 2d2d 2d2d  ----: | --------
+00001ae0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001af0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001b00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001b10: 2d2d 2d2d 2d2d 3a20 7c0a 7c20 2020 2030  ------: |.|    0
+00001b20: 207c 2020 2020 3120 7c20 3230 3230 2d30   |    1 | 2020-0
+00001b30: 312d 3031 2030 303a 3030 3a30 3020 7c20  1-01 00:00:00 | 
+00001b40: 312d 3230 3230 2d30 312d 3031 2d30 302d  1-2020-01-01-00-
+00001b50: 3030 2d30 3020 7c20 2020 2020 2020 2020  00-00 |         
+00001b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b80: 2020 2020 2020 2032 2e35 207c 2020 2020         2.5 |    
+00001b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bb0: 207c 0a7c 202d 2d2d 2d2d 2d2d 2d2d 2d2d   |.| -----------
-00001bc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001bd0: 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d2d  --- | ----------
-00001be0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c 0a7c  ------------ |.|
-00001bf0: 20f0 9f9a a820 2a2a 4275 6720 5265 706f   .... **Bug Repo
-00001c00: 7274 732a 2a20 2020 2020 2020 2020 2020  rts**           
-00001c10: 2020 207c 205b 4769 7448 7562 2049 7373     | [GitHub Iss
-00001c20: 7565 2054 7261 636b 6572 5d20 7c0a 7c20  ue Tracker] |.| 
-00001c30: f09f 8e81 202a 2a46 6561 7475 7265 2052  .... **Feature R
-00001c40: 6571 7565 7374 7320 2620 4964 6561 732a  equests & Ideas*
-00001c50: 2a20 7c20 5b47 6974 4875 6220 4973 7375  * | [GitHub Issu
-00001c60: 6520 5472 6163 6b65 725d 207c 0a7c 20f0  e Tracker] |.| .
-00001c70: 9f91 a9e2 808d f09f 92bb 202a 2a55 7361  .......... **Usa
-00001c80: 6765 2051 7565 7374 696f 6e73 2a2a 2020  ge Questions**  
-00001c90: 2020 2020 2020 2020 7c20 5b47 6974 4875          | [GitHu
-00001ca0: 6220 4469 7363 7573 7369 6f6e 735d 2020  b Discussions]  
-00001cb0: 207c 0a7c 20f0 9f97 af20 2a2a 4765 6e65   |.| .... **Gene
-00001cc0: 7261 6c20 4469 7363 7573 7369 6f6e 2a2a  ral Discussion**
-00001cd0: 2020 2020 2020 207c 205b 4769 7448 7562         | [GitHub
-00001ce0: 2044 6973 6375 7373 696f 6e73 5d20 2020   Discussions]   
-00001cf0: 7c0a 0a5b 6769 7468 7562 2069 7373 7565  |..[github issue
-00001d00: 2074 7261 636b 6572 5d3a 2068 7474 7073   tracker]: https
-00001d10: 3a2f 2f67 6974 6875 622e 636f 6d2f 4161  ://github.com/Aa
-00001d20: 7268 7573 2d50 7379 6368 6961 7472 792d  rhus-Psychiatry-
-00001d30: 5265 7365 6172 6368 2f74 696d 6573 6572  Research/timeser
-00001d40: 6965 7366 6c61 7474 656e 6572 2f69 7373  iesflattener/iss
-00001d50: 7565 730a 5b67 6974 6875 6220 6469 7363  ues.[github disc
-00001d60: 7573 7369 6f6e 735d 3a20 6874 7470 733a  ussions]: https:
-00001d70: 2f2f 6769 7468 7562 2e63 6f6d 2f41 6172  //github.com/Aar
-00001d80: 6875 732d 5073 7963 6869 6174 7279 2d52  hus-Psychiatry-R
-00001d90: 6573 6561 7263 682f 7469 6d65 7365 7269  esearch/timeseri
-00001da0: 6573 666c 6174 7465 6e65 722f 6469 7363  esflattener/disc
-00001db0: 7573 7369 6f6e 730a 0a0a 2323 20f0 9f8e  ussions...## ...
-00001dc0: 9320 5072 6f6a 6563 7473 0a50 5359 434f  . Projects.PSYCO
-00001dd0: 5020 7072 6f6a 6563 7473 2077 6869 6368  P projects which
-00001de0: 2075 7365 2060 7469 6d65 7365 7269 6573   use `timeseries
-00001df0: 666c 6174 7465 6e65 7260 2e20 4e6f 7465  flattener`. Note
-00001e00: 2074 6861 7420 736f 6d65 206f 6620 7468   that some of th
-00001e10: 6573 6520 7072 6f6a 6563 7473 2068 6176  ese projects hav
-00001e20: 6520 7965 7420 746f 2062 6520 7075 626c  e yet to be publ
-00001e30: 6973 6865 6420 616e 6420 6172 6520 7468  ished and are th
-00001e40: 7573 2070 7269 7661 7465 2e0a 0a7c 2050  us private...| P
-00001e50: 726f 6a65 6374 2020 2020 2020 2020 2020  roject          
-00001e60: 2020 2020 2020 207c 2050 7562 6c69 6361         | Publica
-00001e70: 7469 6f6e 7320 7c20 2020 2020 2020 2020  tions |         
-00001e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001bc0: 2020 2020 2020 2020 2020 2030 207c 0a7c             0 |.|
+00001bd0: 2020 2020 3120 7c20 2020 2031 207c 2032      1 |    1 | 2
+00001be0: 3032 302d 3032 2d30 3120 3030 3a30 303a  020-02-01 00:00:
+00001bf0: 3030 207c 2031 2d32 3032 302d 3032 2d30  00 | 1-2020-02-0
+00001c00: 312d 3030 2d30 302d 3030 207c 2020 2020  1-00-00-00 |    
+00001c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c30: 2020 2020 2020 2020 2020 2020 2020 3120                1 
+00001c40: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+00001c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c80: 3120 7c0a 7c20 2020 2032 207c 2020 2020  1 |.|    2 |    
+00001c90: 3220 7c20 3230 3230 2d30 322d 3031 2030  2 | 2020-02-01 0
+00001ca0: 303a 3030 3a30 3020 7c20 322d 3230 3230  0:00:00 | 2-2020
+00001cb0: 2d30 322d 3031 2d30 302d 3030 2d30 3020  -02-01-00-00-00 
+00001cc0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+00001cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cf0: 2020 2034 207c 2020 2020 2020 2020 2020     4 |          
+00001d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d30: 2020 2020 2030 207c 0a0a 0a23 2320 f09f       0 |...## ..
+00001d40: 9396 2044 6f63 756d 656e 7461 7469 6f6e  .. Documentation
+00001d50: 0a0a 7c20 446f 6375 6d65 6e74 6174 696f  ..| Documentatio
+00001d60: 6e20 2020 2020 2020 2020 207c 2020 2020  n          |    
+00001d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001dc0: 2020 2020 7c0a 7c20 2d2d 2d2d 2d2d 2d2d      |.| --------
+00001dd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c  -------------- |
+00001de0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+00001df0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001e00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001e10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001e20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001e30: 2d2d 2d2d 2d2d 2d20 7c0a 7c20 f09f 8e93  ------- |.| ....
+00001e40: 202a 2a5b 5475 746f 7269 616c 5d2a 2a20   **[Tutorial]** 
+00001e50: 2020 2020 2020 7c20 5369 6d70 6c65 2061        | Simple a
+00001e60: 6e64 2061 6476 616e 6365 6420 7475 746f  nd advanced tuto
+00001e70: 7269 616c 7320 746f 2067 6574 2079 6f75  rials to get you
+00001e80: 2073 7461 7274 6564 2075 7369 6e67 2060   started using `
+00001e90: 7469 6d65 7365 7269 6573 666c 6174 7465  timeseriesflatte
+00001ea0: 6e65 7260 2020 2020 2020 2020 2020 207c  ner`           |
+00001eb0: 0a7c 20f0 9f8e 9b20 2a2a 5b47 656e 6572  .| .... **[Gener
+00001ec0: 616c 2064 6f63 735d 2a2a 207c 2054 6865  al docs]** | The
+00001ed0: 2064 6574 6169 6c65 6420 7265 6665 7265   detailed refere
+00001ee0: 6e63 6520 666f 7220 7469 6d65 7365 7269  nce for timeseri
+00001ef0: 6573 666c 6174 7465 6e65 7227 7320 4150  esflattener's AP
+00001f00: 492e 207c 0a7c 20f0 9f99 8b20 2a2a 5b46  I. |.| .... **[F
+00001f10: 4151 5d2a 2a20 2020 2020 2020 2020 2020  AQ]**           
+00001f20: 207c 2046 7265 7175 656e 746c 7920 6173   | Frequently as
+00001f30: 6b65 6420 7175 6573 7469 6f6e 2020 2020  ked question    
 00001f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f50: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00001f60: 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  | --------------
-00001f70: 2d2d 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d  --------- | ----
-00001f80: 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d  -------- | -----
-00001f90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001fa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001fb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001fc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001fd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001fe0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001ff0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002000: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002020: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002030: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002040: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002050: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002060: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002070: 207c 0a7c 202a 2a5b 5479 7065 2032 2044   |.| **[Type 2 D
-00002080: 6961 6265 7465 735d 2a2a 2020 207c 2020  iabetes]**   |  
-00002090: 2020 2020 2020 2020 2020 2020 7c20 5072              | Pr
-000020a0: 6564 6963 7469 6f6e 206f 6620 7479 7065  ediction of type
-000020b0: 2032 2064 6961 6265 7465 7320 616d 6f6e   2 diabetes amon
-000020c0: 6720 7061 7469 656e 7473 2077 6974 6820  g patients with 
-000020d0: 7669 7369 7473 2074 6f20 7073 7963 6869  visits to psychi
-000020e0: 6174 7269 6320 686f 7370 6974 616c 2064  atric hospital d
-000020f0: 6570 6172 746d 656e 7473 2020 2020 2020  epartments      
-00002100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f70: 2020 2020 2020 2020 2020 7c0a 7c20 f09f            |.| ..
+00001f80: 97ba efb8 8f20 2a2a 5b52 6f61 646d 6170  ..... **[Roadmap
+00001f90: 5d2a 2a20 2020 2020 2020 207c 204b 616e  ]**        | Kan
+00001fa0: 6261 6e20 626f 6172 6420 666f 7220 7468  ban board for th
+00001fb0: 6520 726f 6164 6d61 7020 666f 7220 7468  e roadmap for th
+00001fc0: 6520 7072 6f6a 6563 7420 2020 2020 2020  e project       
+00001fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ff0: 2020 2020 7c0a 0a5b 5475 746f 7269 616c      |..[Tutorial
+00002000: 5d3a 2068 7474 7073 3a2f 2f61 6172 6875  ]: https://aarhu
+00002010: 732d 7073 7963 6869 6174 7279 2d72 6573  s-psychiatry-res
+00002020: 6561 7263 682e 6769 7468 7562 2e69 6f2f  earch.github.io/
+00002030: 7469 6d65 7365 7269 6573 666c 6174 7465  timeseriesflatte
+00002040: 6e65 722f 7475 746f 7269 616c 732e 6874  ner/tutorials.ht
+00002050: 6d6c 0a5b 4765 6e65 7261 6c20 646f 6373  ml.[General docs
+00002060: 5d3a 2068 7474 7073 3a2f 2f41 6172 6875  ]: https://Aarhu
+00002070: 732d 5073 7963 6869 6174 7279 2d52 6573  s-Psychiatry-Res
+00002080: 6561 7263 682e 6769 7468 7562 2e69 6f2f  earch.github.io/
+00002090: 7469 6d65 7365 7269 6573 666c 6174 7465  timeseriesflatte
+000020a0: 6e65 722f 0a5b 4641 515d 3a20 6874 7470  ner/.[FAQ]: http
+000020b0: 733a 2f2f 4161 7268 7573 2d50 7379 6368  s://Aarhus-Psych
+000020c0: 6961 7472 792d 5265 7365 6172 6368 2e67  iatry-Research.g
+000020d0: 6974 6875 622e 696f 2f74 696d 6573 6572  ithub.io/timeser
+000020e0: 6965 7366 6c61 7474 656e 6572 2f66 6171  iesflattener/faq
+000020f0: 2e68 746d 6c0a 5b52 6f61 646d 6170 5d3a  .html.[Roadmap]:
+00002100: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00002110: 636f 6d2f 6f72 6773 2f41 6172 6875 732d  com/orgs/Aarhus-
+00002120: 5073 7963 6869 6174 7279 2d52 6573 6561  Psychiatry-Resea
+00002130: 7263 682f 7072 6f6a 6563 7473 2f31 312f  rch/projects/11/
+00002140: 7669 6577 732f 310a 0a23 2320 f09f 92ac  views/1..## ....
+00002150: 2057 6865 7265 2074 6f20 6173 6b20 7175   Where to ask qu
+00002160: 6573 7469 6f6e 730a 0a7c 2054 7970 6520  estions..| Type 
 00002170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002180: 2020 2020 7c0a 7c20 2a2a 5b43 616e 6365      |.| **[Cance
-00002190: 725d 2a2a 2020 2020 2020 2020 2020 2020  r]**            
-000021a0: 7c20 2020 2020 2020 2020 2020 2020 207c  |              |
-000021b0: 2050 7265 6469 6374 696f 6e20 6f66 2043   Prediction of C
-000021c0: 616e 6365 7220 616d 6f6e 6720 7061 7469  ancer among pati
-000021d0: 656e 7473 2077 6974 6820 7669 7369 7473  ents with visits
-000021e0: 2074 6f20 7073 7963 6869 6174 7269 6320   to psychiatric 
-000021f0: 686f 7370 6974 616c 2064 6570 6172 746d  hospital departm
-00002200: 656e 7473 2020 2020 2020 2020 2020 2020  ents            
-00002210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002290: 2020 2020 2020 207c 0a7c 202a 2a5b 434f         |.| **[CO
-000022a0: 5044 5d2a 2a20 2020 2020 2020 2020 2020  PD]**           
-000022b0: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-000022c0: 2020 7c20 5072 6564 6963 7469 6f6e 206f    | Prediction o
-000022d0: 6620 4368 726f 6e69 6320 6f62 7374 7275  f Chronic obstru
-000022e0: 6374 6976 6520 7075 6c6d 6f6e 6172 7920  ctive pulmonary 
-000022f0: 6469 7365 6173 6520 2843 4f50 4429 2061  disease (COPD) a
-00002300: 6d6f 6e67 2070 6174 6965 6e74 7320 7769  mong patients wi
-00002310: 7468 2076 6973 6974 7320 746f 2070 7379  th visits to psy
-00002320: 6368 6961 7472 6963 2068 6f73 7069 7461  chiatric hospita
-00002330: 6c20 6465 7061 7274 6d65 6e74 7320 2020  l departments   
-00002340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023a0: 2020 2020 2020 2020 2020 7c0a 7c20 2a2a            |.| **
-000023b0: 5b46 6f72 6365 6420 6164 6d69 7373 696f  [Forced admissio
-000023c0: 6e73 5d2a 2a20 7c20 2020 2020 2020 2020  ns]** |         
-000023d0: 2020 2020 207c 2050 7265 6469 6374 696f       | Predictio
-000023e0: 6e20 6f66 2066 6f72 6365 6420 6164 6d69  n of forced admi
-000023f0: 7373 696f 6e73 206f 6620 7061 7469 656e  ssions of patien
-00002400: 7473 2074 6f20 7468 6520 7073 7963 6869  ts to the psychi
-00002410: 6174 7269 6320 686f 7370 6974 616c 2064  atric hospital d
-00002420: 6570 6172 746d 656e 7473 2e20 456e 636f  epartments. Enco
-00002430: 6d70 6173 7365 7320 7477 6f20 7365 7061  mpasses two sepa
-00002440: 7261 7465 2070 726f 6a65 6374 733a 2031  rate projects: 1
-00002450: 2e20 5072 6564 6963 6974 696e 6720 6174  . Prediciting at
-00002460: 2074 696d 6520 6f66 2064 6973 6368 6172   time of dischar
-00002470: 6765 2066 6f72 2069 6e70 6174 6965 6e74  ge for inpatient
-00002480: 2061 646d 6973 7369 6f6e 732e 2032 2e20   admissions. 2. 
-00002490: 5072 6564 6963 7469 6e67 2064 6179 2062  Predicting day b
-000024a0: 6566 6f72 6520 6f75 7470 6174 6965 6e74  efore outpatient
-000024b0: 2061 646d 6973 7369 6f6e 732e 207c 0a7c   admissions. |.|
-000024c0: 202a 2a5b 436f 6572 6369 6f6e 5d2a 2a20   **[Coercion]** 
-000024d0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-000024e0: 2020 2020 2020 2020 7c20 5072 6564 6963          | Predic
-000024f0: 7469 6f6e 206f 6620 636f 6572 6369 6f6e  tion of coercion
-00002500: 2061 6d6f 6e67 2070 6174 6965 6e74 7320   among patients 
-00002510: 6164 6d69 7474 6965 6420 746f 2074 6865  admittied to the
-00002520: 2068 6f73 7069 7461 6c20 7073 7963 6869   hospital psychi
-00002530: 6174 7269 6320 6465 7061 7274 6d65 6e74  atric department
-00002540: 2e20 456e 636f 6d70 6173 7365 7320 7072  . Encompasses pr
-00002550: 6564 6963 7469 6e67 206d 6563 6861 6e69  edicting mechani
-00002560: 6361 6c20 7265 7374 7261 696e 742c 2073  cal restraint, s
-00002570: 6564 6174 6976 6520 6d65 6469 6361 7469  edative medicati
-00002580: 6f6e 2061 6e64 206d 616e 7561 6c20 7265  on and manual re
-00002590: 7374 7261 696e 7420 3438 2068 6f75 7273  straint 48 hours
-000025a0: 2062 6566 6f72 6520 636f 6572 6369 6f6e   before coercion
-000025b0: 206f 6363 7572 732e 2020 2020 2020 2020   occurs.        
-000025c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025d0: 7c0a 0a0a 5b54 7970 6520 3220 6469 6162  |...[Type 2 diab
-000025e0: 6574 6573 5d3a 2068 7474 7073 3a2f 2f67  etes]: https://g
-000025f0: 6974 6875 622e 636f 6d2f 4161 7268 7573  ithub.com/Aarhus
-00002600: 2d50 7379 6368 6961 7472 792d 5265 7365  -Psychiatry-Rese
-00002610: 6172 6368 2f70 7379 636f 702d 7432 640a  arch/psycop-t2d.
-00002620: 5b43 616e 6365 725d 3a20 6874 7470 733a  [Cancer]: https:
-00002630: 2f2f 6769 7468 7562 2e63 6f6d 2f41 6172  //github.com/Aar
-00002640: 6875 732d 5073 7963 6869 6174 7279 2d52  hus-Psychiatry-R
-00002650: 6573 6561 7263 682f 7073 7963 6f70 2d63  esearch/psycop-c
-00002660: 616e 6365 720a 5b43 4f50 445d 3a20 6874  ancer.[COPD]: ht
-00002670: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00002680: 2f41 6172 6875 732d 5073 7963 6869 6174  /Aarhus-Psychiat
-00002690: 7279 2d52 6573 6561 7263 682f 7073 7963  ry-Research/psyc
-000026a0: 6f70 2d63 6f70 640a 5b46 6f72 6365 6420  op-copd.[Forced 
-000026b0: 6164 6d69 7373 696f 6e73 5d3a 2068 7474  admissions]: htt
-000026c0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000026d0: 4161 7268 7573 2d50 7379 6368 6961 7472  Aarhus-Psychiatr
-000026e0: 792d 5265 7365 6172 6368 2f70 7379 636f  y-Research/psyco
-000026f0: 702d 666f 7263 6564 2d61 646d 6973 7369  p-forced-admissi
-00002700: 6f6e 730a 5b43 6f65 7263 696f 6e5d 3a20  ons.[Coercion]: 
-00002710: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00002720: 6f6d 2f41 6172 6875 732d 5073 7963 6869  om/Aarhus-Psychi
-00002730: 6174 7279 2d52 6573 6561 7263 682f 7079  atry-Research/py
-00002740: 7363 6f70 2d63 6f65 7263 696f 6e0a       scop-coercion.
+00002180: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
+00002190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021a0: 2020 207c 0a7c 202d 2d2d 2d2d 2d2d 2d2d     |.| ---------
+000021b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000021c0: 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d  ----- | --------
+000021d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c  -------------- |
+000021e0: 0a7c 20f0 9f9a a820 2a2a 4275 6720 5265  .| .... **Bug Re
+000021f0: 706f 7274 732a 2a20 2020 2020 2020 2020  ports**         
+00002200: 2020 2020 207c 205b 4769 7448 7562 2049       | [GitHub I
+00002210: 7373 7565 2054 7261 636b 6572 5d20 7c0a  ssue Tracker] |.
+00002220: 7c20 f09f 8e81 202a 2a46 6561 7475 7265  | .... **Feature
+00002230: 2052 6571 7565 7374 7320 2620 4964 6561   Requests & Idea
+00002240: 732a 2a20 7c20 5b47 6974 4875 6220 4973  s** | [GitHub Is
+00002250: 7375 6520 5472 6163 6b65 725d 207c 0a7c  sue Tracker] |.|
+00002260: 20f0 9f91 a9e2 808d f09f 92bb 202a 2a55   ........... **U
+00002270: 7361 6765 2051 7565 7374 696f 6e73 2a2a  sage Questions**
+00002280: 2020 2020 2020 2020 2020 7c20 5b47 6974            | [Git
+00002290: 4875 6220 4469 7363 7573 7369 6f6e 735d  Hub Discussions]
+000022a0: 2020 207c 0a7c 20f0 9f97 af20 2a2a 4765     |.| .... **Ge
+000022b0: 6e65 7261 6c20 4469 7363 7573 7369 6f6e  neral Discussion
+000022c0: 2a2a 2020 2020 2020 207c 205b 4769 7448  **       | [GitH
+000022d0: 7562 2044 6973 6375 7373 696f 6e73 5d20  ub Discussions] 
+000022e0: 2020 7c0a 0a5b 6769 7468 7562 2069 7373    |..[github iss
+000022f0: 7565 2074 7261 636b 6572 5d3a 2068 7474  ue tracker]: htt
+00002300: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00002310: 4161 7268 7573 2d50 7379 6368 6961 7472  Aarhus-Psychiatr
+00002320: 792d 5265 7365 6172 6368 2f74 696d 6573  y-Research/times
+00002330: 6572 6965 7366 6c61 7474 656e 6572 2f69  eriesflattener/i
+00002340: 7373 7565 730a 5b67 6974 6875 6220 6469  ssues.[github di
+00002350: 7363 7573 7369 6f6e 735d 3a20 6874 7470  scussions]: http
+00002360: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f41  s://github.com/A
+00002370: 6172 6875 732d 5073 7963 6869 6174 7279  arhus-Psychiatry
+00002380: 2d52 6573 6561 7263 682f 7469 6d65 7365  -Research/timese
+00002390: 7269 6573 666c 6174 7465 6e65 722f 6469  riesflattener/di
+000023a0: 7363 7573 7369 6f6e 730a 0a0a 2323 20f0  scussions...## .
+000023b0: 9f8e 9320 5072 6f6a 6563 7473 0a50 5359  ... Projects.PSY
+000023c0: 434f 5020 7072 6f6a 6563 7473 2077 6869  COP projects whi
+000023d0: 6368 2075 7365 2060 7469 6d65 7365 7269  ch use `timeseri
+000023e0: 6573 666c 6174 7465 6e65 7260 2e20 4e6f  esflattener`. No
+000023f0: 7465 2074 6861 7420 736f 6d65 206f 6620  te that some of 
+00002400: 7468 6573 6520 7072 6f6a 6563 7473 2068  these projects h
+00002410: 6176 6520 7965 7420 746f 2062 6520 7075  ave yet to be pu
+00002420: 626c 6973 6865 6420 616e 6420 6172 6520  blished and are 
+00002430: 7468 7573 2070 7269 7661 7465 2e0a 0a7c  thus private...|
+00002440: 2050 726f 6a65 6374 2020 2020 2020 2020   Project        
+00002450: 2020 2020 2020 2020 207c 2050 7562 6c69           | Publi
+00002460: 6361 7469 6f6e 7320 7c20 2020 2020 2020  cations |       
+00002470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002550: 7c0a 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |.| ------------
+00002560: 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c20 2d2d  ----------- | --
+00002570: 2d2d 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d  ---------- | ---
+00002580: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002590: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000025a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000025b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000025c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000025d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000025e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000025f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002600: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002610: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002620: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002630: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002640: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002650: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002660: 2d2d 207c 0a7c 202a 2a5b 5479 7065 2032  -- |.| **[Type 2
+00002670: 2044 6961 6265 7465 735d 2a2a 2020 207c   Diabetes]**   |
+00002680: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00002690: 5072 6564 6963 7469 6f6e 206f 6620 7479  Prediction of ty
+000026a0: 7065 2032 2064 6961 6265 7465 7320 616d  pe 2 diabetes am
+000026b0: 6f6e 6720 7061 7469 656e 7473 2077 6974  ong patients wit
+000026c0: 6820 7669 7369 7473 2074 6f20 7073 7963  h visits to psyc
+000026d0: 6869 6174 7269 6320 686f 7370 6974 616c  hiatric hospital
+000026e0: 2064 6570 6172 746d 656e 7473 2020 2020   departments    
+000026f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002770: 2020 2020 2020 7c0a 7c20 2a2a 5b43 616e        |.| **[Can
+00002780: 6365 725d 2a2a 2020 2020 2020 2020 2020  cer]**          
+00002790: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
+000027a0: 207c 2050 7265 6469 6374 696f 6e20 6f66   | Prediction of
+000027b0: 2043 616e 6365 7220 616d 6f6e 6720 7061   Cancer among pa
+000027c0: 7469 656e 7473 2077 6974 6820 7669 7369  tients with visi
+000027d0: 7473 2074 6f20 7073 7963 6869 6174 7269  ts to psychiatri
+000027e0: 6320 686f 7370 6974 616c 2064 6570 6172  c hospital depar
+000027f0: 746d 656e 7473 2020 2020 2020 2020 2020  tments          
+00002800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002880: 2020 2020 2020 2020 207c 0a7c 202a 2a5b           |.| **[
+00002890: 434f 5044 5d2a 2a20 2020 2020 2020 2020  COPD]**         
+000028a0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+000028b0: 2020 2020 7c20 5072 6564 6963 7469 6f6e      | Prediction
+000028c0: 206f 6620 4368 726f 6e69 6320 6f62 7374   of Chronic obst
+000028d0: 7275 6374 6976 6520 7075 6c6d 6f6e 6172  ructive pulmonar
+000028e0: 7920 6469 7365 6173 6520 2843 4f50 4429  y disease (COPD)
+000028f0: 2061 6d6f 6e67 2070 6174 6965 6e74 7320   among patients 
+00002900: 7769 7468 2076 6973 6974 7320 746f 2070  with visits to p
+00002910: 7379 6368 6961 7472 6963 2068 6f73 7069  sychiatric hospi
+00002920: 7461 6c20 6465 7061 7274 6d65 6e74 7320  tal departments 
+00002930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002990: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+000029a0: 2a2a 5b46 6f72 6365 6420 6164 6d69 7373  **[Forced admiss
+000029b0: 696f 6e73 5d2a 2a20 7c20 2020 2020 2020  ions]** |       
+000029c0: 2020 2020 2020 207c 2050 7265 6469 6374         | Predict
+000029d0: 696f 6e20 6f66 2066 6f72 6365 6420 6164  ion of forced ad
+000029e0: 6d69 7373 696f 6e73 206f 6620 7061 7469  missions of pati
+000029f0: 656e 7473 2074 6f20 7468 6520 7073 7963  ents to the psyc
+00002a00: 6869 6174 7269 6320 686f 7370 6974 616c  hiatric hospital
+00002a10: 2064 6570 6172 746d 656e 7473 2e20 456e   departments. En
+00002a20: 636f 6d70 6173 7365 7320 7477 6f20 7365  compasses two se
+00002a30: 7061 7261 7465 2070 726f 6a65 6374 733a  parate projects:
+00002a40: 2031 2e20 5072 6564 6963 6974 696e 6720   1. Prediciting 
+00002a50: 6174 2074 696d 6520 6f66 2064 6973 6368  at time of disch
+00002a60: 6172 6765 2066 6f72 2069 6e70 6174 6965  arge for inpatie
+00002a70: 6e74 2061 646d 6973 7369 6f6e 732e 2032  nt admissions. 2
+00002a80: 2e20 5072 6564 6963 7469 6e67 2064 6179  . Predicting day
+00002a90: 2062 6566 6f72 6520 6f75 7470 6174 6965   before outpatie
+00002aa0: 6e74 2061 646d 6973 7369 6f6e 732e 207c  nt admissions. |
+00002ab0: 0a7c 202a 2a5b 436f 6572 6369 6f6e 5d2a  .| **[Coercion]*
+00002ac0: 2a20 2020 2020 2020 2020 207c 2020 2020  *          |    
+00002ad0: 2020 2020 2020 2020 2020 7c20 5072 6564            | Pred
+00002ae0: 6963 7469 6f6e 206f 6620 636f 6572 6369  iction of coerci
+00002af0: 6f6e 2061 6d6f 6e67 2070 6174 6965 6e74  on among patient
+00002b00: 7320 6164 6d69 7474 6965 6420 746f 2074  s admittied to t
+00002b10: 6865 2068 6f73 7069 7461 6c20 7073 7963  he hospital psyc
+00002b20: 6869 6174 7269 6320 6465 7061 7274 6d65  hiatric departme
+00002b30: 6e74 2e20 456e 636f 6d70 6173 7365 7320  nt. Encompasses 
+00002b40: 7072 6564 6963 7469 6e67 206d 6563 6861  predicting mecha
+00002b50: 6e69 6361 6c20 7265 7374 7261 696e 742c  nical restraint,
+00002b60: 2073 6564 6174 6976 6520 6d65 6469 6361   sedative medica
+00002b70: 7469 6f6e 2061 6e64 206d 616e 7561 6c20  tion and manual 
+00002b80: 7265 7374 7261 696e 7420 3438 2068 6f75  restraint 48 hou
+00002b90: 7273 2062 6566 6f72 6520 636f 6572 6369  rs before coerci
+00002ba0: 6f6e 206f 6363 7572 732e 2020 2020 2020  on occurs.      
+00002bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bc0: 2020 7c0a 0a0a 5b54 7970 6520 3220 6469    |...[Type 2 di
+00002bd0: 6162 6574 6573 5d3a 2068 7474 7073 3a2f  abetes]: https:/
+00002be0: 2f67 6974 6875 622e 636f 6d2f 4161 7268  /github.com/Aarh
+00002bf0: 7573 2d50 7379 6368 6961 7472 792d 5265  us-Psychiatry-Re
+00002c00: 7365 6172 6368 2f70 7379 636f 702d 7432  search/psycop-t2
+00002c10: 640a 5b43 616e 6365 725d 3a20 6874 7470  d.[Cancer]: http
+00002c20: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f41  s://github.com/A
+00002c30: 6172 6875 732d 5073 7963 6869 6174 7279  arhus-Psychiatry
+00002c40: 2d52 6573 6561 7263 682f 7073 7963 6f70  -Research/psycop
+00002c50: 2d63 616e 6365 720a 5b43 4f50 445d 3a20  -cancer.[COPD]: 
+00002c60: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00002c70: 6f6d 2f41 6172 6875 732d 5073 7963 6869  om/Aarhus-Psychi
+00002c80: 6174 7279 2d52 6573 6561 7263 682f 7073  atry-Research/ps
+00002c90: 7963 6f70 2d63 6f70 640a 5b46 6f72 6365  ycop-copd.[Force
+00002ca0: 6420 6164 6d69 7373 696f 6e73 5d3a 2068  d admissions]: h
+00002cb0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00002cc0: 6d2f 4161 7268 7573 2d50 7379 6368 6961  m/Aarhus-Psychia
+00002cd0: 7472 792d 5265 7365 6172 6368 2f70 7379  try-Research/psy
+00002ce0: 636f 702d 666f 7263 6564 2d61 646d 6973  cop-forced-admis
+00002cf0: 7369 6f6e 730a 5b43 6f65 7263 696f 6e5d  sions.[Coercion]
+00002d00: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+00002d10: 2e63 6f6d 2f41 6172 6875 732d 5073 7963  .com/Aarhus-Psyc
+00002d20: 6869 6174 7279 2d52 6573 6561 7263 682f  hiatry-Research/
+00002d30: 7079 7363 6f70 2d63 6f65 7263 696f 6e0a  pyscop-coercion.
```

### Comparing `timeseriesflattener-0.23.9/README.md` & `timeseriesflattener-0.24.0/README.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/citation.cff` & `timeseriesflattener-0.24.0/citation.cff`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/docs/Makefile` & `timeseriesflattener-0.24.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/docs/_static/favicon.ico` & `timeseriesflattener-0.24.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/docs/_static/icon.png` & `timeseriesflattener-0.24.0/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/docs/_static/icon_dark.png` & `timeseriesflattener-0.24.0/docs/_static/icon_dark.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/docs/_static/terminology_figure.png` & `timeseriesflattener-0.24.0/docs/_static/terminology_figure.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/docs/conf.py` & `timeseriesflattener-0.24.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/docs/faq.rst` & `timeseriesflattener-0.24.0/docs/faq.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 Frequently Asked Questions
 ================================
 
 
 Citing this package
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-If you wish to use this library in your research, please cite it using (Changing the version if relevant):
+If you wish to use this library in your research, please cite the `JOSS paper <https://joss.theoj.org/papers/10.21105/joss.05197.pdf>`__:
 
-.. TODO: the following need to be corrected:
 .. code-block::
 
-   @software{Bernstorff_timeseriesflattener_2022,
-      author = {Bernstorff, Martin and Enevoldsen, Kenneth and Damgaard, Jakob Grøhn and Hæstrup, Frida and Hansen, Lasse},
-      doi = {10.5281/zenodo.7389672},
-      month = {11},
-      title = {{timeseriesflattener}},
-      url = {https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener},
-      year = {2022}
-   }
+   @article{bernstorff2023timeseriesflattener,
+  title={timeseriesflattener: A Python package for summarizing features from (medical) time series},
+  author={Bernstorff, Martin and Enevoldsen, Kenneth and Damgaard, Jakob and Danielsen, Andreas and Hansen, Lasse},
+  journal={Journal of Open Source Software},
+  volume={8},
+  number={83},
+  pages={5197},
+  year={2023}
+}
 
 
 Or if you prefer APA:
 
 .. code-block:: 
 
-   Bernstorff, M., Enevoldsen, K., Damgaard, J. G., Hæstrup, F., & Hansen, L. (2022). timeseriesflattener [Computer software]. https://doi.org/10.5281/zenodo.7389672
+   Bernstorff, M., Enevoldsen, K., Damgaard, J., Danielsen, A., & Hansen, L. (2023). timeseriesflattener: A Python package for summarizing features from (medical) time series. Journal of Open Source Software, 8(83), 5197.
 
 
 
 How do I test the code and run the test suite?
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 This package comes with an extensive test suite. In order to run the tests,
 you'll usually want to clone the repository and build the package from the
 source. This will also install the required development dependencies
 and test utilities defined in the `pyproject.toml <https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/blob/main/pyproject.toml>`__.
 
 
 .. code-block:: bash
 
-   poetry install
+   pip install -e ."[dev]"
 
    python -m pytest
 
 
 which will run all the test in the `tests` folder.
 
 Specific tests can be run using:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `timeseriesflattener-0.23.9/docs/index.rst` & `timeseriesflattener-0.24.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/docs/tutorials/01_basic.ipynb` & `timeseriesflattener-0.24.0/docs/tutorials/01_basic.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/docs/tutorials/02_advanced.ipynb` & `timeseriesflattener-0.24.0/docs/tutorials/02_advanced.ipynb`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9923394097222222%*

 * *Differences: {"'cells'": "{3: {'execution_count': 3}, 4: {'execution_count': 4, 'outputs': {0: "*

 * *            "{'execution_count': 4}}}, 10: {'execution_count': 5}, 11: {'execution_count': 6}, 13: "*

 * *            "{'execution_count': 7}, 17: {'execution_count': 8}, 18: {'execution_count': 9, "*

 * *            "'source': {insert: [(5, '    cache=DiskCache(\\n'), (6, '        "*

 * *            'feature_cache_dir=Path(".tmp") / "feature_cache",\\n\'), (7, \'    ),\\n\'), (9, '*

 * *            "')\\n')], delete: [7, 5]}}, 20: {'execution_ […]*

```diff
@@ -34,29 +34,29 @@
                 "This function is then called when you initialise a feature specification.\n",
                 "\n",
                 "This loader is specified in the values_loader key like so:\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from skimpy import skim\n",
                 "from timeseriesflattener.testing.load_synth_data import load_synth_predictor_float\n",
                 "from timeseriesflattener.resolve_multiple_functions import mean\n",
                 "from timeseriesflattener.feature_spec_objects import PredictorSpec\n",
                 "from pprint import pprint\n",
                 "import numpy as np"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -166,15 +166,15 @@
                             "99997       8168 1969-07-30 01:45:00  0.929738\n",
                             "99998       9328 1965-12-22 10:53:00  5.124424\n",
                             "99999       6582 1965-02-10 09:52:00  7.414466\n",
                             "\n",
                             "[100000 rows x 3 columns]"
                         ]
                     },
-                    "execution_count": 2,
+                    "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "pred_spec_batch = PredictorSpec(\n",
                 "    values_loader=load_synth_predictor_float,\n",
@@ -246,25 +246,25 @@
                 "Manually specifying a handful of features one at a time is rather straightforward, but what if you want to generate hundreds of features? Or want to have multiple different lookbehind windows, e.g. a month, 6 months and a year? Then the amount of code you'll have to write will grow quite substantially and becomes time consuming and hard to navigate.\n",
                 "\n",
                 "To solve this problem, we implemented feature group specifications. They allow you to combinatorially create features. Let's look at an example:\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from timeseriesflattener.feature_spec_objects import PredictorGroupSpec\n",
                 "from timeseriesflattener.resolve_multiple_functions import maximum"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [],
             "source": [
                 "pred_spec_batch = PredictorGroupSpec(\n",
                 "    values_loader=[\"synth_predictor_float\"],\n",
                 "    lookbehind_days=[365, 730],\n",
                 "    fallback=[np.nan],\n",
@@ -283,15 +283,15 @@
                 "2. We require values_loaders to be strings that can be resolved from the registry. This string is also used when creating the column names - otherwise we wouldn't know what to call the columns.\n",
                 "\n",
                 "Let's check that the results look good."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "\u2013\u2013\u2013\u2013\u2013\u2013\u2013\u2013\u2013 We created 4 combinations of predictors. \u2013\u2013\u2013\u2013\u2013\u2013\u2013\u2013\u2013\u2013\n",
@@ -348,39 +348,41 @@
             "metadata": {},
             "source": [
                 "Timeseriesflattener ships with a class that allows for caching to disk. Let's look at an example of that:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from skimpy import skim\n",
                 "from timeseriesflattener.testing.load_synth_data import load_synth_prediction_times\n",
                 "from timeseriesflattener.feature_cache.cache_to_disk import DiskCache\n",
                 "from timeseriesflattener.flattened_dataset import TimeseriesFlattener\n",
                 "from pathlib import Path"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [],
             "source": [
                 "ts_flattener = TimeseriesFlattener(\n",
                 "    prediction_times_df=load_synth_prediction_times(),\n",
                 "    entity_id_col_name=\"entity_id\",\n",
                 "    timestamp_col_name=\"timestamp\",\n",
                 "    n_workers=4,\n",
-                "    cache=DiskCache(feature_cache_dir=Path(\".tmp\") / \"feature_cache\"),\n",
+                "    cache=DiskCache(\n",
+                "        feature_cache_dir=Path(\".tmp\") / \"feature_cache\",\n",
+                "    ),\n",
                 "    drop_pred_times_with_insufficient_look_distance=True,\n",
-                ")"
+                ")\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -389,46 +391,64 @@
                 "The first time we create features, this will just save them to disk and won't make any difference to performance. But say we want to add two more features - then it'll load the features that it has already computed from disk, and then only compute the two new features.\n",
                 "\n",
                 "Note that DiskCache is an instance of the abstract class FeatureCache. If you want to implement your own cache, for example using REDIS or SQL, all you'll need is to implement the 3 methods in that class. Now, let's compute a dataframe to check that everything works."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [],
             "source": [
                 "ts_flattener.add_spec(pred_spec_batch)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "2022-12-09 11:44:44 [INFO] There were unprocessed specs, computing...\n",
-                        "2022-12-09 11:44:44 [INFO] _drop_pred_time_if_insufficient_look_distance: Dropped 4038 (40.38%) rows\n",
-                        "100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 4/4 [00:01<00:00,  2.91it/s]\n",
-                        "2022-12-09 11:44:46 [INFO] Starting concatenation. Will take some time on performant systems, e.g. 30s for 100 features. This is normal.\n",
-                        "2022-12-09 11:44:46 [INFO] Concatenation took 0.019 seconds\n",
-                        "2022-12-09 11:44:46 [INFO] Merging with original df\n"
+                        "2023-04-19 15:30:57 [INFO] There were unprocessed specs, computing...\n",
+                        "2023-04-19 15:30:57 [INFO] _drop_pred_time_if_insufficient_look_distance: Dropped 4038 (40.38%) rows\n",
+                        "2023-04-19 15:30:57 [INFO] Processing 4 temporal features in parallel with 4 workers. Chunksize is 1. If this is above 1, it may take some time for the progress bar to move, as processing is batched. However, this makes for much faster total performance.\n",
+                        "  0%|          | 0/4 [00:01<?, ?it/s]\n"
+                    ]
+                },
+                {
+                    "ename": "KeyError",
+                    "evalue": "'prediction_time_uuid'",
+                    "output_type": "error",
+                    "traceback": [
+                        "\u001b[0;31m---------------------------------------------------------------------------\u001b[0m",
+                        "\u001b[0;31mRemoteTraceback\u001b[0m                           Traceback (most recent call last)",
+                        "\u001b[0;31mRemoteTraceback\u001b[0m: \n\"\"\"\nTraceback (most recent call last):\n  File \"/Users/au484925/Desktop/Git/timeseriesflattener/.venv39/lib/python3.9/site-packages/pandas/core/indexes/base.py\", line 3802, in get_loc\n    return self._engine.get_loc(casted_key)\n  File \"pandas/_libs/index.pyx\", line 138, in pandas._libs.index.IndexEngine.get_loc\n  File \"pandas/_libs/index.pyx\", line 165, in pandas._libs.index.IndexEngine.get_loc\n  File \"pandas/_libs/hashtable_class_helper.pxi\", line 5745, in pandas._libs.hashtable.PyObjectHashTable.get_item\n  File \"pandas/_libs/hashtable_class_helper.pxi\", line 5753, in pandas._libs.hashtable.PyObjectHashTable.get_item\nKeyError: 'prediction_time_uuid'\n\nThe above exception was the direct cause of the following exception:\n\nTraceback (most recent call last):\n  File \"/opt/homebrew/Cellar/python@3.9/3.9.16/Frameworks/Python.framework/Versions/3.9/lib/python3.9/multiprocessing/pool.py\", line 125, in worker\n    result = (True, func(*args, **kwds))\n  File \"/Users/au484925/Desktop/Git/timeseriesflattener/src/timeseriesflattener/flattened_dataset.py\", line 452, in _get_temporal_feature\n    df = self.cache.read_feature(feature_spec=feature_spec)\n  File \"/Users/au484925/Desktop/Git/timeseriesflattener/src/timeseriesflattener/feature_cache/cache_to_disk.py\", line 124, in read_feature\n    left=self.prediction_times_df[self.pred_time_uuid_col_name],\n  File \"/Users/au484925/Desktop/Git/timeseriesflattener/.venv39/lib/python3.9/site-packages/pandas/core/frame.py\", line 3807, in __getitem__\n    indexer = self.columns.get_loc(key)\n  File \"/Users/au484925/Desktop/Git/timeseriesflattener/.venv39/lib/python3.9/site-packages/pandas/core/indexes/base.py\", line 3804, in get_loc\n    raise KeyError(key) from err\nKeyError: 'prediction_time_uuid'\n\"\"\"",
+                        "\nThe above exception was the direct cause of the following exception:\n",
+                        "\u001b[0;31mKeyError\u001b[0m                                  Traceback (most recent call last)",
+                        "Cell \u001b[0;32mIn[11], line 1\u001b[0m\n\u001b[0;32m----> 1\u001b[0m df \u001b[39m=\u001b[39m ts_flattener\u001b[39m.\u001b[39;49mget_df()\n",
+                        "File \u001b[0;32m~/Desktop/Git/timeseriesflattener/src/timeseriesflattener/flattened_dataset.py:940\u001b[0m, in \u001b[0;36mTimeseriesFlattener.get_df\u001b[0;34m(self)\u001b[0m\n\u001b[1;32m    938\u001b[0m \u001b[39mif\u001b[39;00m \u001b[39mlen\u001b[39m(\u001b[39mself\u001b[39m\u001b[39m.\u001b[39munprocessed_specs) \u001b[39m>\u001b[39m \u001b[39m0\u001b[39m:\n\u001b[1;32m    939\u001b[0m     log\u001b[39m.\u001b[39minfo(\u001b[39m\"\u001b[39m\u001b[39mThere were unprocessed specs, computing...\u001b[39m\u001b[39m\"\u001b[39m)\n\u001b[0;32m--> 940\u001b[0m     \u001b[39mself\u001b[39;49m\u001b[39m.\u001b[39;49mcompute()\n\u001b[1;32m    942\u001b[0m \u001b[39m# Process\u001b[39;00m\n\u001b[1;32m    943\u001b[0m \u001b[39mreturn\u001b[39;00m \u001b[39mself\u001b[39m\u001b[39m.\u001b[39m_df\n",
+                        "File \u001b[0;32m~/Desktop/Git/timeseriesflattener/src/timeseriesflattener/flattened_dataset.py:929\u001b[0m, in \u001b[0;36mTimeseriesFlattener.compute\u001b[0;34m(self)\u001b[0m\n\u001b[1;32m    926\u001b[0m     log\u001b[39m.\u001b[39mwarning(\u001b[39m\"\u001b[39m\u001b[39mNo unprocessed specs, skipping\u001b[39m\u001b[39m\"\u001b[39m)\n\u001b[1;32m    927\u001b[0m     \u001b[39mreturn\u001b[39;00m\n\u001b[0;32m--> 929\u001b[0m \u001b[39mself\u001b[39;49m\u001b[39m.\u001b[39;49m_process_temporal_specs()\n\u001b[1;32m    930\u001b[0m \u001b[39mself\u001b[39m\u001b[39m.\u001b[39m_process_static_specs()\n",
+                        "File \u001b[0;32m~/Desktop/Git/timeseriesflattener/src/timeseriesflattener/flattened_dataset.py:788\u001b[0m, in \u001b[0;36mTimeseriesFlattener._process_temporal_specs\u001b[0;34m(self)\u001b[0m\n\u001b[1;32m    785\u001b[0m     \u001b[39mself\u001b[39m\u001b[39m.\u001b[39m_df \u001b[39m=\u001b[39m \u001b[39mself\u001b[39m\u001b[39m.\u001b[39m_drop_pred_time_if_insufficient_look_distance(df\u001b[39m=\u001b[39m\u001b[39mself\u001b[39m\u001b[39m.\u001b[39m_df)\n\u001b[1;32m    787\u001b[0m \u001b[39mif\u001b[39;00m \u001b[39mlen\u001b[39m(temporal_batch) \u001b[39m>\u001b[39m \u001b[39m0\u001b[39m:\n\u001b[0;32m--> 788\u001b[0m     \u001b[39mself\u001b[39;49m\u001b[39m.\u001b[39;49m_add_temporal_batch(temporal_batch\u001b[39m=\u001b[39;49mtemporal_batch)\n\u001b[1;32m    790\u001b[0m \u001b[39m# Remove the processed specs\u001b[39;00m\n\u001b[1;32m    791\u001b[0m \u001b[39mself\u001b[39m\u001b[39m.\u001b[39munprocessed_specs\u001b[39m.\u001b[39moutcome_specs \u001b[39m=\u001b[39m []\n",
+                        "File \u001b[0;32m~/Desktop/Git/timeseriesflattener/src/timeseriesflattener/flattened_dataset.py:574\u001b[0m, in \u001b[0;36mTimeseriesFlattener._add_temporal_batch\u001b[0;34m(self, temporal_batch)\u001b[0m\n\u001b[1;32m    569\u001b[0m log\u001b[39m.\u001b[39minfo(\n\u001b[1;32m    570\u001b[0m     \u001b[39mf\u001b[39m\u001b[39m\"\u001b[39m\u001b[39mProcessing \u001b[39m\u001b[39m{\u001b[39;00m\u001b[39mlen\u001b[39m(temporal_batch)\u001b[39m}\u001b[39;00m\u001b[39m temporal features in parallel with \u001b[39m\u001b[39m{\u001b[39;00mn_workers\u001b[39m}\u001b[39;00m\u001b[39m workers. Chunksize is \u001b[39m\u001b[39m{\u001b[39;00mchunksize\u001b[39m}\u001b[39;00m\u001b[39m. If this is above 1, it may take some time for the progress bar to move, as processing is batched. However, this makes for much faster total performance.\u001b[39m\u001b[39m\"\u001b[39m,\n\u001b[1;32m    571\u001b[0m )\n\u001b[1;32m    573\u001b[0m \u001b[39mwith\u001b[39;00m Pool(n_workers) \u001b[39mas\u001b[39;00m p:\n\u001b[0;32m--> 574\u001b[0m     flattened_predictor_dfs \u001b[39m=\u001b[39m \u001b[39mlist\u001b[39;49m(\n\u001b[1;32m    575\u001b[0m         tqdm\u001b[39m.\u001b[39;49mtqdm(\n\u001b[1;32m    576\u001b[0m             p\u001b[39m.\u001b[39;49mimap(\n\u001b[1;32m    577\u001b[0m                 func\u001b[39m=\u001b[39;49m\u001b[39mself\u001b[39;49m\u001b[39m.\u001b[39;49m_get_temporal_feature,\n\u001b[1;32m    578\u001b[0m                 iterable\u001b[39m=\u001b[39;49mtemporal_batch,\n\u001b[1;32m    579\u001b[0m                 chunksize\u001b[39m=\u001b[39;49mchunksize,\n\u001b[1;32m    580\u001b[0m             ),\n\u001b[1;32m    581\u001b[0m             total\u001b[39m=\u001b[39;49m\u001b[39mlen\u001b[39;49m(temporal_batch),\n\u001b[1;32m    582\u001b[0m         ),\n\u001b[1;32m    583\u001b[0m     )\n\u001b[1;32m    585\u001b[0m \u001b[39mself\u001b[39m\u001b[39m.\u001b[39m_concatenate_flattened_timeseries(\n\u001b[1;32m    586\u001b[0m     flattened_predictor_dfs\u001b[39m=\u001b[39mflattened_predictor_dfs,\n\u001b[1;32m    587\u001b[0m )\n",
+                        "File \u001b[0;32m~/Desktop/Git/timeseriesflattener/.venv39/lib/python3.9/site-packages/tqdm/std.py:1178\u001b[0m, in \u001b[0;36mtqdm.__iter__\u001b[0;34m(self)\u001b[0m\n\u001b[1;32m   1175\u001b[0m time \u001b[39m=\u001b[39m \u001b[39mself\u001b[39m\u001b[39m.\u001b[39m_time\n\u001b[1;32m   1177\u001b[0m \u001b[39mtry\u001b[39;00m:\n\u001b[0;32m-> 1178\u001b[0m     \u001b[39mfor\u001b[39;00m obj \u001b[39min\u001b[39;00m iterable:\n\u001b[1;32m   1179\u001b[0m         \u001b[39myield\u001b[39;00m obj\n\u001b[1;32m   1180\u001b[0m         \u001b[39m# Update and possibly print the progressbar.\u001b[39;00m\n\u001b[1;32m   1181\u001b[0m         \u001b[39m# Note: does not call self.update(1) for speed optimisation.\u001b[39;00m\n",
+                        "File \u001b[0;32m/opt/homebrew/Cellar/python@3.9/3.9.16/Frameworks/Python.framework/Versions/3.9/lib/python3.9/multiprocessing/pool.py:870\u001b[0m, in \u001b[0;36mIMapIterator.next\u001b[0;34m(self, timeout)\u001b[0m\n\u001b[1;32m    868\u001b[0m \u001b[39mif\u001b[39;00m success:\n\u001b[1;32m    869\u001b[0m     \u001b[39mreturn\u001b[39;00m value\n\u001b[0;32m--> 870\u001b[0m \u001b[39mraise\u001b[39;00m value\n",
+                        "\u001b[0;31mKeyError\u001b[0m: 'prediction_time_uuid'"
                     ]
                 }
             ],
             "source": [
                 "df = ts_flattener.get_df()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<pre style=\"white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace\">\u256d\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500 skimpy summary \u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u256e\n",
                             "\u2502 <span style=\"font-style: italic\">         Data Summary         </span> <span style=\"font-style: italic\">      Data Types       </span>                                                          \u2502\n",
@@ -525,15 +545,15 @@
                 "skim(df)\n",
                 "\n",
                 "list(df.columns)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<style type=\"text/css\">\n",
                             "</style>\n",
@@ -669,16 +689,17 @@
                 "rename_dict = {c: f\"pred_{i+1}\" for i, c in enumerate(pred_cols)}\n",
                 "df_renamed = df.rename(rename_dict, axis=1)\n",
                 "\n",
                 "# Print a dataframe\n",
                 "base_cols = [\"entity_id\", \"timestamp\", \"prediction_time_uuid\"]\n",
                 "renamed_cols = list(rename_dict.values())\n",
                 "\n",
-                "df_renamed[0:10][base_cols + renamed_cols].style.\\\n",
-                "    set_table_attributes('style=\"font-size: 14px\"')"
+                "df_renamed[0:10][base_cols + renamed_cols].style.set_table_attributes(\n",
+                "    'style=\"font-size: 14px\"'\n",
+                ")\n"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3.10.7 ('.venv': poetry)",
             "language": "python",
@@ -690,15 +711,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.8 (main, Oct 13 2022, 09:48:40) [Clang 14.0.0 (clang-1400.0.29.102)]"
+            "version": "3.9.16"
         },
         "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
                 "hash": "d2b49c0af2d95979144de75823f7cfbb268839811992fdd0cb17fc1bb54ce815"
             }
         }
```

### Comparing `timeseriesflattener-0.23.9/docs/tutorials/03_text.ipynb` & `timeseriesflattener-0.24.0/docs/tutorials/03_text.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/docs/tutorials/img/term_a.png` & `timeseriesflattener-0.24.0/docs/tutorials/img/term_a.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/docs/tutorials/img/term_b.png` & `timeseriesflattener-0.24.0/docs/tutorials/img/term_b.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/docs/tutorials/img/term_c.png` & `timeseriesflattener-0.24.0/docs/tutorials/img/term_c.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/docs/tutorials/img/term_d.png` & `timeseriesflattener-0.24.0/docs/tutorials/img/term_d.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/icon.png` & `timeseriesflattener-0.24.0/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/paper/paper.bib` & `timeseriesflattener-0.24.0/paper/paper.bib`

 * *Files 0% similar despite different names*

```diff
@@ -101,27 +101,27 @@
 
 @article{imrie_autoprognosis_2022,
   title        = {{AutoPrognosis} 2.0: Democratizing Diagnostic and Prognostic Modeling in Healthcare with Automated Machine Learning},
   shorttitle   = {{AutoPrognosis} 2.0},
   journaltitle = {{arXiv} preprint {arXiv}:2210.12090},
   author       = {Imrie, Fergus and Cebere, Bogdan and {McKinney}, Eoin F. and van der Schaar, Mihaela},
   date         = {2022},
+  doi          = {10.48550/arXiv.2210.12090},
   file         = {Imrie et al_2022_AutoPrognosis 2.pdf:/Users/au554730/Library/Mobile Documents/com~apple~CloudDocs/zotero_storage/Imrie et al_2022_AutoPrognosis 2.pdf:application/pdf;Snapshot:/Users/au554730/Zotero/storage/NJSFPHCH/2210.html:text/html}
 }
 
 @article{shamout_machine_2021,
   title        = {Machine learning for clinical outcome prediction},
   volume       = {14},
   pages        = {116--126},
   journaltitle = {{IEEE} reviews in Biomedical Engineering},
   author       = {Shamout, Farah and Zhu, Tingting and Clifton, David A.},
   doi          = {10.1109/RBME.2020.3007816},
   date         = {2021},
-  note         = {Publisher: {IEEE}},
-  doi          = {10.48550/arXiv.2210.12090}
+  note         = {Publisher: {IEEE}}
 }
 
 @article{johnson_mimic-iii_2016,
   title        = {{MIMIC}-{III}, a freely accessible critical care database},
   volume       = {3},
   pages        = {1--9},
   number       = {1},
```

### Comparing `timeseriesflattener-0.23.9/paper/paper.md` & `timeseriesflattener-0.24.0/paper/paper.md`

 * *Files 0% similar despite different names*

```diff
@@ -32,17 +32,16 @@
  - name: Center for Humanities Computing, Aarhus University, Aarhus, Denmark
    index: 3
  - name: Psychosis Research Unit, Aarhus University Hospital - Psychiatry, Denmark
    index: 4
 date: 2 December 2022
 bibliography: paper.bib
 ---
-# timeseriesflattener: A Python package for summarising features from (medical) time series
 
-# Summary
+# Summary 
 Time series from e.g. electronic health records often have a large number of variables that are sampled at irregular and differing intervals. Before this type of data can be used for prediction modelling with machine learning methods such as logistic regression or XGBoost [@chen_xgboost_2016], the data needs to be reshaped. In essence, the time series need to be *flattened* so that each prediction time is represented by a vector of predefined length. This vector should hold the set of predictor values and an outcome value. These predictor values can be constructed by aggregating the preceding values in the time series within a certain time window. This process of flattening the data lays the foundation for further analyses and requires handling a number of tasks such as 1) how to deal with missing values, 2) which value to use if none fall within the prediction window, 3) how to handle variables measured multiple times within the chosen time window, and 4) how to handle predictors that attempt to look further back than the start of the dataset.  
 
 `timeseriesflattener` aims to simplify this process by providing an easy-to-use and fully-specified pipeline for flattening complex time series. `timeseriesflattener` implements all the functionality required for aggregating features in specific time windows, grouped by e.g. patient IDs, in a computationally efficient manner. The package is currently used for feature extraction from electronic health records in studies based on the Psychiatric Clinical Outcome Prediction Cohort (PSYCOP) projects [@hansen_psychiatric_2021].
 
 # Statement of need
 The recent surge in machine learning capabilities has led to large efforts in using information from electronic health records and other medical time series for prediction modelling [@rajkomar_scalable_2018; @shamout_machine_2021]. These efforts have spawned important developments related to prediction modelling of clinical data such as AutoPrognosis2.0 [@imrie_autoprognosis_2022] and general-purpose autoML frameworks such as `auto-sklearn` [@feurer_efficient_2015]. However, modelling and machine learning tends to take the spotlight, with often insufficient attention being paid to data preparation and problem framing. For example, some earlier papers have generated predictions at a specific time interval before each outcome. However, this makes the problem artificially easy, and the model will not generalise to the real world [@lauritsen_framing_2021]. 
 
@@ -92,8 +91,8 @@
 The package is aimed at researchers and individuals working with irregular time series such as electronic health records or sensor data from e.g. glucose monitoring or Internet of Things devices.
 
 
 # Acknowledgements
 This work is supported by the Lundbeck Foundation (grant number: R344-2020-1073), the Danish Cancer Society (grant number: R283-A16461), the Central Denmark Region Fund for Strengthening of Health Science (grant number: 1-36-72-4-20) and the Danish Agency for Digitisation Investment Fund for New Technologies (grant number 2020-6720). 
 
 
-# References
+# References
```

### Comparing `timeseriesflattener-0.23.9/src/timeseriesflattener/column_handler.py` & `timeseriesflattener-0.24.0/src/timeseriesflattener/column_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,18 +90,18 @@
         single value column.
 
         Args:
             df (pd.DataFrame): Dataframe with value column
             output_spec (TemporalSpec): Output specification
         """
         if "value" in df.columns and isinstance(df["value"], pd.DataFrame):
-            df["value"] = df["value"].fillna(output_spec.fallback)
+            df["value"] = df["value"].fillna(output_spec.fallback)  # type: ignore
         else:
             df[output_spec.get_col_str()] = df[output_spec.get_col_str()].fillna(
-                output_spec.fallback,
+                output_spec.fallback,  # type: ignore
             )
         return df
 
     @staticmethod
     def flatten_multiindex(df: pd.DataFrame) -> pd.DataFrame:
         """Checks if dataframe has multiindex columns and flattens them if it does.
         In this case, flattening means stripping the first level of the multiindex.
```

### Comparing `timeseriesflattener-0.23.9/src/timeseriesflattener/feature_cache/abstract_feature_cache.py` & `timeseriesflattener-0.24.0/src/timeseriesflattener/feature_cache/abstract_feature_cache.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/src/timeseriesflattener/feature_cache/cache_to_disk.py` & `timeseriesflattener-0.24.0/src/timeseriesflattener/feature_cache/cache_to_disk.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             pred_time_uuid_col_name (str, optional): Name of column containing prediction time uuids. Defaults to "pred_time_uuid".
             entity_id_col_name (str, optional): Name of column containing entity ids. Defaults to "entity_id".
             timestamp_col_name (str, optional): Name of column containing timestamps. Defaults to "timestamp".
             cache_file_suffix (str, optional): File suffix for cache files. Defaults to ".parquet".
         """
 
         super().__init__(
-            prediction_times_df=prediction_times_df,
+            prediction_times_df=prediction_times_df,  # type: ignore
             pred_time_uuid_col_name=pred_time_uuid_col_name,
         )
 
         self.feature_cache_dir = feature_cache_dir
         self.feature_cache_dir.mkdir(exist_ok=True, parents=True)
 
         self.cache_file_suffix = cache_file_suffix
@@ -127,29 +127,29 @@
             how="left",
             on=self.pred_time_uuid_col_name,
             validate="m:1",
         )
 
         # Replace NaNs with fallback
         df[feature_spec.get_col_str()] = df[feature_spec.get_col_str()].fillna(
-            feature_spec.fallback,
+            feature_spec.fallback,  # type: ignore
         )
 
         return df
 
     def write_feature(
         self,
         feature_spec: TemporalSpec,
         df: pd.DataFrame,
     ):
         """Write feature to cache."""
         file_name = self._get_file_name(feature_spec=feature_spec)
 
         # Drop rows containing fallback, since it's non-informative
-        df = df[df[feature_spec.get_col_str()] != feature_spec.fallback].dropna()
+        df = df[df[feature_spec.get_col_str()] != feature_spec.fallback].dropna()  # type: ignore
 
         # Drop entity and timestamp columns if they exists
         for col in [self.entity_entity_id_col_name, self.timestamp_col_name]:
             if col in df.columns:
                 df = df.drop(columns=col)
 
         # Write df to cache
```

### Comparing `timeseriesflattener-0.23.9/src/timeseriesflattener/feature_spec_objects.py` & `timeseriesflattener-0.24.0/src/timeseriesflattener/feature_spec_objects.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,36 +11,34 @@
 from pydantic import Extra, Field
 
 from timeseriesflattener.resolve_multiple_functions import resolve_multiple_fns
 from timeseriesflattener.utils import data_loaders, split_dfs
 
 log = logging.getLogger(__name__)
 
-# pylint: disable=consider-alternative-union-syntax, trailing-whitespace, missing-class-docstring, too-few-public-methods
-
 
 @lru_cache
 def load_df_with_cache(
     loader_fn: Callable,
     kwargs: Dict[str, Any],
     feature_name: str,
 ) -> pd.DataFrame:
     """Wrapper function to cache dataframe loading."""
     start_time = time.time()
     log.info(
         f"{feature_name}: Loading values",
-    )  # pylint: disable=logging-fstring-interpolation
+    )
 
     df = loader_fn(**kwargs)
 
     end_time = time.time()
 
     log.debug(
         f"{feature_name}: Loaded in {end_time - start_time:.2f} seconds",
-    )  # pylint: disable=logging-fstring-interpolation
+    )
 
     return df
 
 
 def in_dict_and_not_none(d: dict, key: str) -> bool:
     """Check if a key is in a dictionary and its value is not None."""
     return key in d and d[key] is not None
@@ -61,15 +59,15 @@
         if callable(data["values_loader"]):
             if "loader_kwargs" not in data or data["loader_kwargs"] is None:
                 data["loader_kwargs"] = {}
 
             data["values_df"] = load_df_with_cache(
                 loader_fn=data["values_loader"],
                 kwargs=frozendict(data["loader_kwargs"]),  # type: ignore
-                feature_name=data["feature_name"],
+                feature_name=data["feature_name"],  # type: ignore
             )
 
 
 def resolve_values_df(data: Dict[str, Any]) -> Dict[str, pd.DataFrame]:
     """Resolve the values_df attribute to a dataframe."""
     if not any(key in data for key in ["values_loader", "values_name", "values_df"]):
         raise ValueError(
@@ -182,21 +180,21 @@
         raise ValueError("\n".join(errors))
 
 
 class _AnySpec(BaseModel):
     """A base class for all feature specifications.
 
     Fields:
-        values_loader (Optional[Callable]):
-            Loader for the df. Tries to resolve from the data_loaders registry,
-            then calls the function which should return a dataframe.
         values_name (Optional[str]):
             A string that maps to a key in a dictionary instantiated by
             `split_df_and_register_to_dict`. Each key corresponds to a dataframe, which
             is a subset of the df where the values_name == key.
+        values_loader (Optional[Callable]):
+            Loader for the df. Tries to resolve from the data_loaders registry,
+            then calls the function which should return a dataframe.
         loader_kwargs (Optional[Mapping[str, Any]]):
             Optional kwargs for the values_loader.
         values_df (Optional[DataFrame]):
             Dataframe with the values.
         feature_name (str):
             The name of the feature. Used for column name generation, e.g.
             <prefix>_<feature_name>.
@@ -204,39 +202,39 @@
             The prefix used for column name generation, e.g.
             <prefix>_<feature_name>.
         input_col_name_override (Optional[str]):
             An override for the input column name. If None, will  attempt
             to infer it by looking for the only column that doesn't match id_col_name
             or timestamp_col_name.
         output_col_name_override (Optional[str]):
-    Override the generated column name after flattening the time series
+            Override the generated column name after flattening the time series
     """
 
     class Doc:
         short_description = "A base class for all feature specifications."
 
-    values_loader: Optional[Callable] = Field(
-        None,
-        description="""Loader for the df. Tries to resolve from the data_loaders registry,
-            then calls the function which should return a dataframe.""",
-    )
-
     values_name: Optional[str] = Field(
         default=None,
         description="""A string that maps to a key in a dictionary instantiated by
             `split_df_and_register_to_dict`. Each key corresponds to a dataframe, which
             is a subset of the df where the values_name == key.""",
     )
 
+    values_loader: Optional[Callable] = Field(
+        None,
+        description="""Loader for the df. Tries to resolve from the data_loaders registry,
+            then calls the function which should return a dataframe.""",
+    )
+
     loader_kwargs: Optional[Dict[str, Any]] = Field(
         default=None,
         description="""Optional kwargs for the values_loader.""",
     )
 
-    values_df: Optional[pd.DataFrame] = Field(
+    values_df: Optional[pd.DataFrame] = Field(  # type: ignore
         default=None,
         description="Dataframe with the values.",
     )
 
     feature_name: str = Field(
         description="""The name of the feature. Used for column name generation, e.g.
             <prefix>_<feature_name>.""",
@@ -286,19 +284,23 @@
     def get_col_str(self, additional_feature_name: Optional[str] = None) -> str:
         """Create column name for the output column.
 
         Args:
             additional_feature_name (Optional[str]): An additional feature name
                 to append to the column name.
         """
+        if self.output_col_name_override:
+            return self.output_col_name_override
+
         feature_name = self.feature_name
+
         if additional_feature_name:
             feature_name = f"{feature_name}-{additional_feature_name}"
-        col_str = f"{self.prefix}_{feature_name}"
-        return col_str
+
+        return f"{self.prefix}_{feature_name}"
 
     def __eq__(self, other: Any) -> bool:
         """Add equality check for dataframes.
 
         Trying to run `spec in list_of_specs` works for all attributes except for df, since the truth value of a dataframe is ambiguous.
         To remedy this, we use pandas' .equals() method for comparing the dfs, and get the combined truth value.
         """
@@ -316,27 +318,32 @@
         return other_attributes_equal and dfs_equal
 
 
 class StaticSpec(_AnySpec):
     class Doc:
         short_description = """Specification for a static feature."""
 
+    def __init__(self, values_loader: Optional[Callable] = None, **kwargs: Any):
+        # Somehow, pyright cannot correctly infer the values_loader type, so we have
+        # to manually specify it
+        super().__init__(values_loader=values_loader, **kwargs)
+
 
 class TemporalSpec(_AnySpec):
     """The minimum specification required for collapsing a temporal
         feature, whether looking ahead or behind. Mostly used for inheritance below.
 
     Fields:
-        values_loader (Optional[Callable]):
-            Loader for the df. Tries to resolve from the data_loaders registry,
-            then calls the function which should return a dataframe.
         values_name (Optional[str]):
             A string that maps to a key in a dictionary instantiated by
             `split_df_and_register_to_dict`. Each key corresponds to a dataframe, which
             is a subset of the df where the values_name == key.
+        values_loader (Optional[Callable]):
+            Loader for the df. Tries to resolve from the data_loaders registry,
+            then calls the function which should return a dataframe.
         loader_kwargs (Optional[dict]):
             Optional kwargs passed onto the data loader.
         values_df (Optional[DataFrame]):
             Dataframe with the values.
         feature_name (str):
             The name of the feature. Used for column name generation, e.g.
             <prefix>_<feature_name>.
@@ -345,15 +352,15 @@
             <prefix>_<feature_name>.
         input_col_name_override (Optional[str]):
             An override for the input column name. If None, will  attempt
             to infer it by looking for the only column that doesn't match id_col_name
             or timestamp_col_name.
         output_col_name_override (Optional[str]):
             Override the generated column name after flattening the time series
-        interval_days (Union[int, float]):
+        interval_days (Optional[float]):
             How far to look in the given direction (ahead for outcomes,
             behind for predictors)
         resolve_multiple_fn (Union[Callable, str]):
             A function used for resolving multiple values within the
             interval_days.
         key_for_resolve_multiple (Optional[str]):
             Key used to lookup the resolve_multiple_fn in the
@@ -370,15 +377,15 @@
             Col name for ids in the input dataframe. Defaults to: entity_id.
     """
 
     class Doc:
         short_description = """The minimum specification required for collapsing a temporal
         feature, whether looking ahead or behind. Mostly used for inheritance below."""
 
-    interval_days: Union[int, float] = Field(
+    interval_days: Optional[float] = Field(
         description="""How far to look in the given direction (ahead for outcomes,
             behind for predictors)""",
     )
 
     resolve_multiple_fn: Union[Callable, str] = Field(
         description="""A function used for resolving multiple values within the
             interval_days.""",
@@ -433,37 +440,45 @@
 
         # override fallback strings with objects
         if self.fallback == "nan":
             self.fallback = float("nan")
 
     def get_col_str(self, additional_feature_name: Optional[str] = None) -> str:
         """Generate the column name for the output column.
+        If interval days is a float, the decimal point is changed to an underscore.
 
         Args:
             additional_feature_name (Optional[str]): additional feature name to
                 append to the column name.
         """
         feature_name = self.feature_name
         if additional_feature_name:
             feature_name = feature_name + "-" + str(additional_feature_name)
-        col_str = f"{self.prefix}_{feature_name}_within_{self.interval_days}_days_{self.key_for_resolve_multiple}_fallback_{self.fallback}"
+
+        interval_days_str = (  # This is required because pydantic coerces the int 2 to float 2.0
+            int(self.interval_days)  # type: ignore
+            if self.interval_days.is_integer()  # type: ignore
+            else str(self.interval_days).replace(".", "-")
+        )
+
+        col_str = f"{self.prefix}_{feature_name}_within_{interval_days_str}_days_{self.key_for_resolve_multiple}_fallback_{self.fallback}"
         return col_str
 
 
 class PredictorSpec(TemporalSpec):
     """Specification for a single predictor, where the df has been resolved.
 
     Fields:
-        values_loader (Optional[Callable]):
-            Loader for the df. Tries to resolve from the data_loaders registry,
-            then calls the function which should return a dataframe.
         values_name (Optional[str]):
             A string that maps to a key in a dictionary instantiated by
             `split_df_and_register_to_dict`. Each key corresponds to a dataframe, which
             is a subset of the df where the values_name == key.
+        values_loader (Optional[Callable]):
+            Loader for the df. Tries to resolve from the data_loaders registry,
+            then calls the function which should return a dataframe.
         loader_kwargs (Optional[dict]):
             Optional kwargs passed onto the data loader.
         values_df (Optional[DataFrame]):
             Dataframe with the values.
         feature_name (str):
             The name of the feature. Used for column name generation, e.g.
             <prefix>_<feature_name>.
@@ -472,15 +487,15 @@
             <prefix>_<feature_name>. Defaults to: pred.
         input_col_name_override (Optional[str]):
             An override for the input column name. If None, will  attempt
             to infer it by looking for the only column that doesn't match id_col_name
             or timestamp_col_name.
         output_col_name_override (Optional[str]):
             Override the generated column name after flattening the time series
-        interval_days (Union[int, float]):
+        interval_days (Optional[float]):
             How far to look in the given direction (ahead for outcomes,
             behind for predictors)
         resolve_multiple_fn (Union[Callable, str]):
             A function used for resolving multiple values within the
             interval_days.
         key_for_resolve_multiple (Optional[str]):
             Key used to lookup the resolve_multiple_fn in the
@@ -491,34 +506,35 @@
         fallback (Union[Callable, int, float, str]):
             Which value to use if no values are found within interval_days.
         allowed_nan_value_prop (float):
             If NaN is higher than this in the input dataframe during
             resolution, raise an error. Defaults to: 0.0.
         entity_id_col_name (str):
             Col name for ids in the input dataframe. Defaults to: entity_id.
-        lookbehind_days (Union[int, float]):
+        lookbehind_days (float):
             How far behind to look for values
     """
 
     class Doc:
         short_description = (
             """Specification for a single predictor, where the df has been resolved."""
         )
 
     prefix: str = Field(
         default="pred",
         description="""The prefix used for column name generation, e.g.
             <prefix>_<feature_name>.""",
     )
 
-    lookbehind_days: Union[int, float] = Field(
+    lookbehind_days: float = Field(
         description="""How far behind to look for values""",
     )
 
     def __init__(self, **data: Any):
+        # Unused argument to correctly type hint the interface
         if "lookbehind_days" in data:
             data["interval_days"] = data["lookbehind_days"]
 
         data["lookbehind_days"] = data["interval_days"]
 
         if not data["interval_days"] and not data["lookbehind_days"]:
             raise ValueError("lookbehind_days or interval_days must be specified.")
@@ -526,21 +542,21 @@
         super().__init__(**data)
 
 
 class TextPredictorSpec(PredictorSpec):
     """Specification for a text predictor, where the df has been resolved.
 
     Fields:
-        values_loader (Optional[Callable]):
-            Loader for the df. Tries to resolve from the data_loaders registry,
-            then calls the function which should return a dataframe.
         values_name (Optional[str]):
             A string that maps to a key in a dictionary instantiated by
             `split_df_and_register_to_dict`. Each key corresponds to a dataframe, which
             is a subset of the df where the values_name == key.
+        values_loader (Optional[Callable]):
+            Loader for the df. Tries to resolve from the data_loaders registry,
+            then calls the function which should return a dataframe.
         loader_kwargs (Optional[dict]):
             Optional kwargs passed onto the data loader.
         values_df (Optional[DataFrame]):
             Dataframe with the values.
         feature_name (str):
             The name of the feature. Used for column name generation, e.g.
             <prefix>_<feature_name>.
@@ -549,15 +565,15 @@
             <prefix>_<feature_name>. Defaults to: pred.
         input_col_name_override (Optional[str]):
             An override for the input column name. If None, will  attempt
             to infer it by looking for the only column that doesn't match id_col_name
             or timestamp_col_name.
         output_col_name_override (Optional[str]):
             Override the generated column name after flattening the time series
-        interval_days (Union[int, float]):
+        interval_days (Optional[float]):
             How far to look in the given direction (ahead for outcomes,
             behind for predictors)
         resolve_multiple_fn (Union[Callable, str]):
             A function used for resolving multiple values within the
         interval_days, i.e. how to combine texts within the lookbehind window.
         Defaults to: 'concatenate'. Other possible options are 'latest' and
         'earliest'. Defaults to: concatenate.
@@ -570,15 +586,15 @@
         fallback (Union[Callable, int, float, str]):
             Which value to use if no values are found within interval_days.
         allowed_nan_value_prop (float):
             If NaN is higher than this in the input dataframe during
             resolution, raise an error. Defaults to: 0.0.
         entity_id_col_name (str):
             Col name for ids in the input dataframe. Defaults to: entity_id.
-        lookbehind_days (Union[int, float]):
+        lookbehind_days (float):
             How far behind to look for values
         embedding_fn (Callable):
             A function used for embedding the text. Should take a
         pandas series of strings and return a pandas dataframe of embeddings.
         Defaults to: None.
         embedding_fn_kwargs (Optional[dict]):
             Optional kwargs passed onto the embedding_fn."""
@@ -601,26 +617,38 @@
         default="concatenate",
         description="""A function used for resolving multiple values within the
         interval_days, i.e. how to combine texts within the lookbehind window.
         Defaults to: 'concatenate'. Other possible options are 'latest' and
         'earliest'.""",
     )
 
+    def __init__(self, **data: Any):
+        # Unused argument to correctly type hint the interface
+        if "lookbehind_days" in data:
+            data["interval_days"] = data["lookbehind_days"]
+
+        data["lookbehind_days"] = data["interval_days"]
+
+        if not data["interval_days"] and not data["lookbehind_days"]:
+            raise ValueError("lookbehind_days or interval_days must be specified.")
+
+        super().__init__(**data)
+
 
 class OutcomeSpec(TemporalSpec):
     """Specification for a single outcome, where the df has been resolved.
 
     Fields:
-        values_loader (Optional[Callable]):
-            Loader for the df. Tries to resolve from the data_loaders registry,
-            then calls the function which should return a dataframe.
         values_name (Optional[str]):
             A string that maps to a key in a dictionary instantiated by
             `split_df_and_register_to_dict`. Each key corresponds to a dataframe, which
             is a subset of the df where the values_name == key.
+        values_loader (Optional[Callable]):
+            Loader for the df. Tries to resolve from the data_loaders registry,
+            then calls the function which should return a dataframe.
         loader_kwargs (Optional[dict]):
             Optional kwargs passed onto the data loader.
         values_df (Optional[DataFrame]):
             Dataframe with the values.
         feature_name (str):
             The name of the feature. Used for column name generation, e.g.
             <prefix>_<feature_name>.
@@ -629,15 +657,15 @@
             <prefix>_<outcome_name>. Defaults to: outc.
         input_col_name_override (Optional[str]):
             An override for the input column name. If None, will  attempt
             to infer it by looking for the only column that doesn't match id_col_name
             or timestamp_col_name.
         output_col_name_override (Optional[str]):
             Override the generated column name after flattening the time series
-        interval_days (Union[int, float]):
+        interval_days (Optional[float]):
             How far to look in the given direction (ahead for outcomes,
             behind for predictors)
         resolve_multiple_fn (Union[Callable, str]):
             A function used for resolving multiple values within the
             interval_days.
         key_for_resolve_multiple (Optional[str]):
             Key used to lookup the resolve_multiple_fn in the
@@ -653,15 +681,15 @@
         entity_id_col_name (str):
             Col name for ids in the input dataframe. Defaults to: entity_id.
         incident (bool):
             Whether the outcome is incident or not.
             I.e., incident outcomes are outcomes you can only experience once.
             For example, type 2 diabetes is incident. Incident outcomes can be handled
             in a vectorised way during resolution, which is faster than non-incident outcomes.
-        lookahead_days (Union[int, float]):
+        lookahead_days (float):
             How far ahead to look for values
     """
 
     class Doc:
         short_description = (
             """Specification for a single outcome, where the df has been resolved."""
         )
@@ -675,15 +703,15 @@
     incident: bool = Field(
         description="""Whether the outcome is incident or not.
             I.e., incident outcomes are outcomes you can only experience once.
             For example, type 2 diabetes is incident. Incident outcomes can be handled
             in a vectorised way during resolution, which is faster than non-incident outcomes.""",
     )
 
-    lookahead_days: Union[int, float] = Field(
+    lookahead_days: float = Field(
         description="""How far ahead to look for values""",
     )
 
     def __init__(self, **data: Any):
         if "lookahead_days" in data:
             data["interval_days"] = data["lookahead_days"]
 
@@ -714,15 +742,15 @@
 class _MinGroupSpec(BaseModel):
     class Doc:
         short_description = """Minimum specification for a group of features,
         whether they're looking ahead or behind.
 
         Used to generate combinations of features."""
 
-    values_loader: Optional[List[str]] = Field(
+    values_loader: Optional[Sequence[str]] = Field(
         default=None,
         description="""Loader for the df. Tries to resolve from the data_loaders
             registry, then calls the function which should return a dataframe.""",
     )
 
     values_name: Optional[List[str]] = Field(
         default=None,
@@ -747,15 +775,15 @@
     )
 
     resolve_multiple_fn: List[Union[Callable, str]] = Field(
         description="""Name of resolve multiple fn, resolved from
             resolve_multiple_functions.py""",
     )
 
-    fallback: List[Union[Callable, str]] = Field(
+    fallback: Sequence[Union[Callable, str, float]] = Field(
         description="""Which value to use if no values are found within interval_days.""",
     )
 
     allowed_nan_value_prop: List[float] = Field(
         default=[0.0],
         description="""If NaN is higher than this in the input dataframe during
             resolution, raise an error.""",
@@ -769,20 +797,20 @@
     loader_kwargs: Optional[List[Dict[str, Any]]] = Field(
         default=None,
         description="""Optional kwargs for the values_loader.""",
     )
 
     def _check_loaders_are_valid(self):
         """Check that all loaders can be resolved from the data_loaders catalogue."""
-        invalid_loaders = list(
-            set(self.values_loader) - set(data_loaders.get_all().keys()),
+        invalid_loaders: list = list(
+            set(self.values_loader) - set(data_loaders.get_all().keys()),  # type: ignore
         )
         if len(invalid_loaders) != 0:
             # New line variable as f-string can't handle backslashes
-            nl = "\n"  # pylint: disable = invalid-name
+            nl = "\n"
             available_loaders = [str(loader) for loader in data_loaders.get_all()]
 
             avail_loaders_str = nl.join(available_loaders)
 
             if len(available_loaders) == 0:
                 avail_loaders_str = "No loaders available."
 
@@ -854,15 +882,15 @@
     return [output_class(**d) for d in permuted_dicts]  # type: ignore
 
 
 class PredictorGroupSpec(_MinGroupSpec):
     """Specification for a group of predictors.
 
     Fields:
-        values_loader (Optional[List[str]]):
+        values_loader (Optional[Sequence[str]]):
             Loader for the df. Tries to resolve from the data_loaders
             registry, then calls the function which should return a dataframe.
         values_name (Optional[List[str]]):
             List of strings that corresponds to a key in a dictionary
             of multiple dataframes that correspods to a name of a type of values.
         values_df (Optional[DataFrame]):
             Dataframe with the values.
@@ -870,36 +898,36 @@
             Override for the column name to use as values in df.
         output_col_name_override (Optional[str]):
             Override for the column name to use as values in the
             output df.
         resolve_multiple_fn (List[Union[Callable, str]]):
             Name of resolve multiple fn, resolved from
             resolve_multiple_functions.py
-        fallback (List[Union[Callable, str]]):
+        fallback (Sequence[Union[Callable, str, float]]):
             Which value to use if no values are found within interval_days.
         allowed_nan_value_prop (List[float]):
             If NaN is higher than this in the input dataframe during
             resolution, raise an error. Defaults to: [0.0].
         prefix (str):
             Prefix for column name, e,g, <prefix>_<feature_name>. Defaults to: pred.
         loader_kwargs (Optional[List[Dict[str, Any]]]):
             Optional kwargs for the values_loader.
-        lookbehind_days (List[Union[int, float]]):
+        lookbehind_days (List[float]):
             How far behind to look for values
     """
 
     class Doc:
         short_description = """Specification for a group of predictors."""
 
     prefix: str = Field(
         default="pred",
         description="""Prefix for column name, e,g, <prefix>_<feature_name>.""",
     )
 
-    lookbehind_days: List[Union[int, float]] = Field(
+    lookbehind_days: List[float] = Field(
         description="""How far behind to look for values""",
     )
 
     def create_combinations(self) -> List[PredictorSpec]:
         """Create all combinations from the group spec."""
         return create_specs_from_group(  # type: ignore
             feature_group_spec=self,
@@ -907,15 +935,15 @@
         )
 
 
 class OutcomeGroupSpec(_MinGroupSpec):
     """Specification for a group of outcomes.
 
     Fields:
-    values_loader (Optional[List[str]]):
+    values_loader (Optional[Sequence[str]]):
         Loader for the df. Tries to resolve from the data_loaders
         registry, then calls the function which should return a dataframe.
     values_name (Optional[List[str]]):
         List of strings that corresponds to a key in a dictionary
         of multiple dataframes that correspods to a name of a type of values.
     values_df (Optional[DataFrame]):
         Dataframe with the values.
@@ -923,29 +951,29 @@
         Override for the column name to use as values in df.
     output_col_name_override (Optional[str]):
         Override for the column name to use as values in the
         output df.
     resolve_multiple_fn (List[Union[Callable, str]]):
         Name of resolve multiple fn, resolved from
         resolve_multiple_functions.py
-    fallback (List[Union[Callable, str]]):
+    fallback (Sequence[Union[Callable, str, float]]):
         Which value to use if no values are found within interval_days.
     allowed_nan_value_prop (List[float]):
         If NaN is higher than this in the input dataframe during
         resolution, raise an error. Defaults to: [0.0].
     prefix (str):
         Prefix for column name, e.g. <prefix>_<feature_name>. Defaults to: outc.
-    loader_kwargs (Optional[List[Dict[str, Any]]]):
+    loader_kwargs (Optional[List[Dict[str,Any]]]):
         Optional kwargs for the values_loader.
     incident (Sequence[bool]):
         Whether the outcome is incident or not, i.e. whether you
         can experience it more than once. For example, type 2 diabetes is incident.
         Incident outcomes can be handled in a vectorised way during resolution,
          which is faster than non-incident outcomes.
-    lookahead_days (List[Union[int, float]]):
+    lookahead_days (List[float]):
         How far ahead to look for values
     """
 
     class Doc:
         short_description = """Specification for a group of outcomes."""
 
     prefix: str = Field(
@@ -956,15 +984,15 @@
     incident: Sequence[bool] = Field(
         description="""Whether the outcome is incident or not, i.e. whether you
             can experience it more than once. For example, type 2 diabetes is incident.
             Incident outcomes can be handled in a vectorised way during resolution,
              which is faster than non-incident outcomes.""",
     )
 
-    lookahead_days: List[Union[int, float]] = Field(
+    lookahead_days: List[float] = Field(
         description="""How far ahead to look for values""",
     )
 
     def create_combinations(self) -> List[OutcomeSpec]:
         """Create all combinations from the group spec."""
         return create_specs_from_group(  # type: ignore
             feature_group_spec=self,
```

### Comparing `timeseriesflattener-0.23.9/src/timeseriesflattener/flattened_dataset.py` & `timeseriesflattener-0.24.0/src/timeseriesflattener/flattened_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     def __len__(self) -> int:
         """Return number of specs in collection."""
         return (
             len(self.outcome_specs) + len(self.predictor_specs) + len(self.static_specs)
         )
 
 
-class TimeseriesFlattener:  # pylint: disable=too-many-instance-attributes
+class TimeseriesFlattener:
     """Turn a set of time-series into tabular prediction-time data."""
 
     def _override_cache_attributes_with_self_attributes(
         self,
         prediction_times_df: DataFrame,
     ):
         """Make cache inherit attributes from flattened dataset.
@@ -83,15 +83,15 @@
                 and getattr(self.cache, attr) != getattr(self, attr)
             ):
                 log.info(
                     f"Overriding {attr} in cache with {attr} passed to init of flattened dataset",
                 )
                 setattr(self.cache, attr, getattr(self, attr))
 
-    def __init__(  # pylint: disable=too-many-arguments
+    def __init__(
         self,
         prediction_times_df: DataFrame,
         drop_pred_times_with_insufficient_look_distance: bool,
         cache: Optional[FeatureCache] = None,
         entity_id_col_name: str = "entity_id",
         timestamp_col_name: str = "timestamp",
         predictor_col_name_prefix: str = "pred",
@@ -237,18 +237,20 @@
             df[val_timestamp_col_name] = (
                 df[val_timestamp_col_name] - dt.datetime(1970, 1, 1)
             ).dt.total_seconds() / 86400
         except TypeError:
             log.info("All values are NaT, returning empty dataframe")
 
         # Sort by timestamp_pred in case resolve_multiple needs dates
-        df = df.sort_values(by=val_timestamp_col_name).groupby(pred_time_uuid_colname)
+        grouped_df = df.sort_values(by=val_timestamp_col_name).groupby(
+            pred_time_uuid_colname,
+        )
 
         if callable(resolve_multiple):
-            df = resolve_multiple(df).reset_index()
+            df = resolve_multiple(grouped_df).reset_index()
         else:
             raise ValueError("resolve_multiple must be or resolve to a Callable")
 
         return df
 
     @staticmethod
     def _drop_records_outside_interval_days(
@@ -272,15 +274,15 @@
         Raises:
             ValueError: If direction is neither ahead nor behind.
 
         Returns:
             DataFrame
         """
         df["time_from_pred_to_val_in_days"] = (
-            (df[timestamp_value_colname] - df[timestamp_pred_colname])
+            (df[timestamp_value_colname] - df[timestamp_pred_colname])  # type: ignore
             / (np.timedelta64(1, "s"))
             / 86_400
         )
         # Divide by 86.400 seconds/day
 
         if direction == "ahead":
             df["is_in_interval"] = (
@@ -354,15 +356,15 @@
             direction = "behind"
         else:
             raise ValueError(f"Unknown output_spec type {type(output_spec)}")
 
         df = TimeseriesFlattener._drop_records_outside_interval_days(
             df,
             direction=direction,
-            interval_days=output_spec.interval_days,
+            interval_days=output_spec.interval_days,  # type: ignore
             timestamp_pred_colname=timestamp_pred_col_name,
             timestamp_value_colname=timestamp_val_col_name,
         )
 
         df[timestamp_val_col_name].replace(
             {output_spec.fallback: pd.NaT},
             inplace=True,  # noqa
@@ -409,15 +411,17 @@
             )
 
         # Add back prediction times that don't have a value, and fill them with fallback
         df = TimeseriesFlattener._add_back_prediction_times_without_value(
             df=df,
             pred_times_with_uuid=prediction_times_with_uuid_df,
             pred_time_uuid_colname=pred_time_uuid_col_name,
-        ).fillna(output_spec.fallback)
+        ).fillna(
+            output_spec.fallback,  # type: ignore
+        )
 
         return df[[*value_col_str_name, pred_time_uuid_col_name]]
 
     @staticmethod
     def rename_input_col_to_value(
         df: pd.DataFrame,
         output_spec: TemporalSpec,
@@ -544,15 +548,15 @@
         end_time = time.time()
 
         log.info(f"Concatenation took {round(end_time - start_time, 3)} seconds")
 
         log.info("Merging with original df")
         self._df = self._df.merge(right=new_features, on=self.pred_time_uuid_col_name)
 
-    def _add_temporal_batch(  # pylint: disable=too-many-branches
+    def _add_temporal_batch(
         self,
         temporal_batch: List[TemporalSpec],
     ):
         """Add predictors to the flattened dataframe from a list."""
         # Shuffle predictor specs to avoid IO contention
         random.shuffle(temporal_batch)
 
@@ -611,18 +615,15 @@
             elif len(possible_value_cols) == 0:
                 raise ValueError(
                     "No value column found in spec.df, please check.",
                 )
         else:
             value_col_name = static_spec.input_col_name_override
 
-        if static_spec.output_col_name_override is not None:
-            output_col_name = static_spec.output_col_name_override
-        elif static_spec.feature_name:
-            output_col_name = f"{static_spec.prefix}_{static_spec.feature_name}"
+        output_col_name = static_spec.get_col_str()
 
         df = pd.DataFrame(
             {
                 self.entity_id_col_name: static_spec.values_df[self.entity_id_col_name],  # type: ignore
                 output_col_name: static_spec.values_df[value_col_name],  # type: ignore
             },
         )
@@ -669,16 +670,16 @@
             df[
                 df[outcome_timestamp_col_name] < df[prediction_timestamp_col_name]
             ].index,
         )
 
         if outcome_spec.is_dichotomous():
             outcome_is_within_lookahead = (
-                df[prediction_timestamp_col_name]
-                + timedelta(days=outcome_spec.interval_days)
+                df[prediction_timestamp_col_name]  # type: ignore
+                + timedelta(days=outcome_spec.interval_days)  # type: ignore
                 > df[outcome_timestamp_col_name]
             )
 
             df[outcome_spec.get_col_str()] = outcome_is_within_lookahead.astype(int)
 
         df = df.rename(
             {prediction_timestamp_col_name: "timestamp"},
@@ -705,15 +706,16 @@
         if isinstance(spec, PredictorSpec):
             min_val_date = spec.values_df[self.timestamp_col_name].min()  # type: ignore
             return min_val_date + pd.Timedelta(days=spec.lookbehind_days)
 
         if isinstance(spec, OutcomeSpec):
             max_val_date = spec.values_df[self.timestamp_col_name].max()  # type: ignore
             return max_val_date - pd.Timedelta(days=spec.lookahead_days)
-        return None
+
+        raise ValueError(f"Spec type {type(spec)} not recognised.")
 
     @print_df_dimensions_diff
     def _drop_pred_time_if_insufficient_look_distance(
         self,
         df: pd.DataFrame,
     ) -> pd.DataFrame:
         """Drop prediction times if there is insufficient look distance.
@@ -772,15 +774,15 @@
         # Remove processed specs. Beware of using .remove on a list of specs, as it causes errors.
         self.unprocessed_specs.outcome_specs = [
             s
             for s in self.unprocessed_specs.outcome_specs
             if hasattr(s, "incident") and not s.incident
         ]
 
-        temporal_batch = self.unprocessed_specs.outcome_specs
+        temporal_batch: List[TemporalSpec] = self.unprocessed_specs.outcome_specs  # type: ignore
         temporal_batch += self.unprocessed_specs.predictor_specs
 
         if self.drop_pred_times_with_insufficient_look_distance:
             self._df = self._drop_pred_time_if_insufficient_look_distance(df=self._df)
 
         if len(temporal_batch) > 0:
             self._add_temporal_batch(temporal_batch=temporal_batch)
@@ -890,26 +892,27 @@
             except ValueError as e:
                 raise ValueError(
                     f"Conversion of {date_of_birth_col_name} to datetime failed, doesn't match format %Y-%m-%d. Recommend converting to datetime before adding.",
                 ) from e
 
         output_age_col_name = f"{output_prefix}_age_in_years"
 
+        tmp_prefix = "tmp"
         self._add_static_info(
             static_spec=_AnySpec(
                 values_df=date_of_birth_df,
                 input_col_name_override=date_of_birth_col_name,
-                prefix="temp",
+                prefix=tmp_prefix,
                 # We typically don't want to use date of birth as a predictor,
                 # but might want to use transformations - e.g. "year of birth" or "age at prediction time".
                 feature_name=date_of_birth_col_name,
             ),
         )
 
-        tmp_date_of_birth_col_name = f"temp_{date_of_birth_col_name}"
+        tmp_date_of_birth_col_name = f"{tmp_prefix}_{date_of_birth_col_name}"
 
         self._df[output_age_col_name] = (
             (
                 self._df[self.timestamp_col_name] - self._df[tmp_date_of_birth_col_name]
             ).dt.days
             / (365.25)
         ).round(2)
```

### Comparing `timeseriesflattener-0.23.9/src/timeseriesflattener/flattened_ds_validator.py` & `timeseriesflattener-0.24.0/src/timeseriesflattener/flattened_ds_validator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/src/timeseriesflattener/logger.py` & `timeseriesflattener-0.24.0/src/timeseriesflattener/logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Example of how to setup a logger with sensible defaults."""
 
 import logging
 from pathlib import Path
+from typing import Optional, Union
 
 import coloredlogs
 
 from timeseriesflattener.utils import PROJECT_ROOT
 
 
 def setup_logger(
     name: str,
     level: int = logging.DEBUG,
-    log_file_path: str = None,
+    log_file_path: Optional[Union[str, Path]] = None,
     fmt: str = "%(asctime)s [%(levelname)s] %(message)s",
 ) -> logging.Logger:
     """
     Set up a logger with the given name and log level.
 
     Args:
         name (str): The name of the logger. Typically use __name__.
@@ -62,15 +63,15 @@
             logfile_dir.mkdir(parents=True)
 
         file_handler = logging.FileHandler(log_file_path)
 
         if level:
             file_handler.setLevel(level)
         if fmt:
-            file_handler.setFormatter(formatter)
+            file_handler.setFormatter(formatter)  # type: ignore
 
         logger.addHandler(file_handler)
 
     return logger
 
 
 if __name__ == "__main__":
```

### Comparing `timeseriesflattener-0.23.9/src/timeseriesflattener/resolve_multiple_functions.py` & `timeseriesflattener-0.24.0/src/timeseriesflattener/resolve_multiple_functions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,72 +1,71 @@
 """Functions for resolving multiple values in a time-series into a single
 value."""
 
-# pylint: disable=missing-function-docstring
 
 import catalogue
 from pandas import DataFrame, Series
 from scipy import stats
 
 resolve_multiple_fns = catalogue.create("timeseriesflattener", "resolve_strategies")
 
 
 @resolve_multiple_fns.register("latest")
-def latest(grouped_df: DataFrame) -> DataFrame:
+def latest(grouped_df: DataFrame) -> Series:
     """Get the latest value.
 
     Args:
         grouped_df (DataFrame): A dataframe sorted by descending timestamp, grouped by citizen.
 
     Returns:
         DataFrame: Dataframe with only the latest value.
     """
-    return grouped_df.last()
+    return grouped_df.last()  # type: ignore
 
 
 @resolve_multiple_fns.register("earliest")
-def earliest(grouped_df: DataFrame) -> DataFrame:
+def earliest(grouped_df: DataFrame) -> Series:
     """Get the earliest value.
 
     Args:
         grouped_df (DataFrame): A dataframe sorted by descending timestamp, grouped by citizen.
 
     Returns:
         DataFrame: Dataframe with only the earliest value in each group.
     """
-    return grouped_df.first()
+    return grouped_df.first()  # type: ignore
 
 
 @resolve_multiple_fns.register("max")
-def maximum(grouped_df: DataFrame) -> DataFrame:
+def maximum(grouped_df: DataFrame) -> Series:
     return grouped_df.max()
 
 
 @resolve_multiple_fns.register("min")
-def minimum(grouped_df: DataFrame) -> DataFrame:
+def minimum(grouped_df: DataFrame) -> Series:
     return grouped_df.min()
 
 
 @resolve_multiple_fns.register("mean")
-def mean(grouped_df: DataFrame) -> DataFrame:
+def mean(grouped_df: DataFrame) -> Series:
     return grouped_df.mean(numeric_only=True)
 
 
 @resolve_multiple_fns.register("sum")
-def summed(grouped_df: DataFrame) -> DataFrame:
+def summed(grouped_df: DataFrame) -> Series:
     return grouped_df.sum()
 
 
 @resolve_multiple_fns.register("count")
-def count(grouped_df: DataFrame) -> DataFrame:
+def count(grouped_df: DataFrame) -> Series:
     return grouped_df.count()
 
 
 @resolve_multiple_fns.register("variance")
-def variance(grouped_df: DataFrame) -> DataFrame:
+def variance(grouped_df: DataFrame) -> Series:
     return grouped_df.var()
 
 
 @resolve_multiple_fns.register("bool")
 def boolean(grouped_df: DataFrame) -> DataFrame:
     """Returns a boolean value indicating whether or not event has occurred in
     look ahead/behind window.
```

### Comparing `timeseriesflattener-0.23.9/src/timeseriesflattener/testing/load_synth_data.py` & `timeseriesflattener-0.24.0/src/timeseriesflattener/testing/load_synth_data.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/src/timeseriesflattener/testing/text_embedding_functions.py` & `timeseriesflattener-0.24.0/src/timeseriesflattener/testing/text_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/src/timeseriesflattener/testing/utils_for_testing.py` & `timeseriesflattener-0.24.0/src/timeseriesflattener/testing/utils_for_testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         convert_np_nan_to_nan (bool): Whether to convert np.nan to np.nan. Defaults to True.
         convert_str_to_float (bool): Whether to convert strings to floats. Defaults to False.
 
     Returns:
         DataFrame: A dataframe.
     """
 
-    df = pd.read_table(StringIO(string), sep=",", index_col=False)
+    df = pd.read_table(StringIO(string), sep=",", index_col=False)  # type: ignore
 
     if convert_timestamp_to_datetime:
         df = convert_cols_with_matching_colnames_to_datetime(df, "timestamp")
 
     if convert_np_nan_to_nan:
         # Convert "np.nan" str to the actual np.nan
         df = df.replace("np.nan", np.nan)
@@ -97,15 +97,15 @@
 
     flattened_ds = TimeseriesFlattener(
         prediction_times_df=prediction_times_df,
         n_workers=4,
         drop_pred_times_with_insufficient_look_distance=False,
     )
 
-    flattened_ds.add_spec(  # pylint: disable=protected-access
+    flattened_ds.add_spec(
         spec=output_spec,
     )
 
     if expected_df:
         for col in expected_df.columns:
             assert_series_equal(
                 left=flattened_ds.get_df()[col],
```

### Comparing `timeseriesflattener-0.23.9/src/timeseriesflattener/text_embedding_functions.py` & `timeseriesflattener-0.24.0/src/timeseriesflattener/text_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/src/timeseriesflattener/utils.py` & `timeseriesflattener-0.24.0/src/timeseriesflattener/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 utilities. If this file grows, consider splitting it up.
 """
 
 import functools
 import logging
 import os
 from pathlib import Path
-from typing import Any, Callable, Dict, Hashable, List, Optional
+from typing import Any, Callable, Dict, Hashable, List, Union
 
 import catalogue
 import pandas as pd
 
 data_loaders = catalogue.create("timeseriesflattener", "data_loaders")
-split_dfs: Dict[str, pd.DataFrame] = {}
+split_dfs: Dict[str, pd.DataFrame] = {}  #
 
 
 PROJECT_ROOT = Path(__file__).resolve().parents[2]
 
 
 def split_df_and_register_to_dict(
     df: pd.DataFrame,
@@ -87,15 +87,15 @@
         .replace("}", "")
         .replace(", ", "_")
     )
 
 
 def load_dataset_from_file(
     file_path: Path,
-    nrows: Optional[int] = None,
+    nrows: Union[int, None] = None,
 ) -> pd.DataFrame:
     """Load dataset from file. Handles csv and parquet files based on suffix.
 
     Args:
         file_path (str): File name.
         nrows (int): Number of rows to load.
 
@@ -190,15 +190,15 @@
 
     for d in predictor_spec_list:
         # Remove any keys with unhashable values
         # Otherwise, we get an error when using "in".
         d = {k: v for k, v in d.items() if isinstance(v, Hashable)}  # noqa
 
         d_as_tuple = tuple(d.items())
-        if d_as_tuple in seen:  # pylint: disable=R6103
+        if d_as_tuple in seen:
             duplicates.add(d_as_tuple)
         else:
             seen.add(d_as_tuple)
 
     if len(duplicates) > 0:
         raise ValueError(f"Found duplicates in list of dicts: {duplicates}")
 
@@ -249,10 +249,10 @@
                 )
 
                 log.info(f"{func.__name__}: Dropped {diff} ({percent_diff}%) {dim}")
             else:
                 if print_when_no_diff:
                     log.info(f"{func.__name__}: No {dim} dropped")
 
-        return result
+        return result  # type: ignore
 
     return wrapper
```

### Comparing `timeseriesflattener-0.23.9/src/timeseriesflattener.egg-info/PKG-INFO` & `timeseriesflattener-0.24.0/src/timeseriesflattener.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7469 6d65  : 2.1.Name: time
 00000020: 7365 7269 6573 666c 6174 7465 6e65 720a  seriesflattener.
-00000030: 5665 7273 696f 6e3a 2030 2e32 332e 390a  Version: 0.23.9.
+00000030: 5665 7273 696f 6e3a 2030 2e32 342e 300a  Version: 0.24.0.
 00000040: 5375 6d6d 6172 793a 2041 2070 6163 6b61  Summary: A packa
 00000050: 6765 2066 6f72 2063 6f6e 7665 7274 696e  ge for convertin
 00000060: 6720 7469 6d65 2073 6572 6965 7320 6461  g time series da
 00000070: 7461 2066 726f 6d20 652e 672e 2065 6c65  ta from e.g. ele
 00000080: 6374 726f 6e69 6320 6865 616c 7468 2072  ctronic health r
 00000090: 6563 6f72 6473 2069 6e74 6f20 7769 6465  ecords into wide
 000000a0: 2066 6f72 6d61 7420 6461 7461 2e0a 4175   format data..Au
@@ -15,615 +15,710 @@
 000000e0: 7365 6e20 3c6c 6173 7365 6830 3331 3040  sen <lasseh0310@
 000000f0: 676d 6169 6c2e 636f 6d3e 2c20 4a61 6b6f  gmail.com>, Jako
 00000100: 6220 4772 c3b8 686e 2044 616d 6761 6172  b Gr..hn Damgaar
 00000110: 6420 3c62 6f6b 616a 6764 4067 6d61 696c  d <bokajgd@gmail
 00000120: 2e63 6f6d 3e2c 204d 6172 7469 6e20 4265  .com>, Martin Be
 00000130: 726e 7374 6f72 6666 203c 6d61 7274 696e  rnstorff <martin
 00000140: 6265 726e 7374 6f72 6666 4067 6d61 696c  bernstorff@gmail
-00000150: 2e63 6f6d 3e0a 436c 6173 7369 6669 6572  .com>.Classifier
-00000160: 3a20 4f70 6572 6174 696e 6720 5379 7374  : Operating Syst
-00000170: 656d 203a 3a20 504f 5349 5820 3a3a 204c  em :: POSIX :: L
-00000180: 696e 7578 0a43 6c61 7373 6966 6965 723a  inux.Classifier:
-00000190: 204f 7065 7261 7469 6e67 2053 7973 7465   Operating Syste
-000001a0: 6d20 3a3a 204d 6163 4f53 203a 3a20 4d61  m :: MacOS :: Ma
-000001b0: 634f 5320 580a 436c 6173 7369 6669 6572  cOS X.Classifier
-000001c0: 3a20 4f70 6572 6174 696e 6720 5379 7374  : Operating Syst
-000001d0: 656d 203a 3a20 4d69 6372 6f73 6f66 7420  em :: Microsoft 
-000001e0: 3a3a 2057 696e 646f 7773 0a43 6c61 7373  :: Windows.Class
-000001f0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000200: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000210: 7974 686f 6e20 3a3a 2033 2e38 0a43 6c61  ython :: 3.8.Cla
-00000220: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00000230: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000240: 2050 7974 686f 6e20 3a3a 2033 2e39 0a43   Python :: 3.9.C
-00000250: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-00000260: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000270: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
-00000280: 300a 436c 6173 7369 6669 6572 3a20 5072  0.Classifier: Pr
-00000290: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000002a0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000002b0: 332e 3131 0a52 6571 7569 7265 732d 5079  3.11.Requires-Py
-000002c0: 7468 6f6e 3a20 3c33 2e31 322e 302c 3e3d  thon: <3.12.0,>=
-000002d0: 332e 382e 300a 4465 7363 7269 7074 696f  3.8.0.Descriptio
-000002e0: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
-000002f0: 7465 7874 2f6d 6172 6b64 6f77 6e0a 5072  text/markdown.Pr
-00000300: 6f76 6964 6573 2d45 7874 7261 3a20 6465  ovides-Extra: de
-00000310: 760a 5072 6f76 6964 6573 2d45 7874 7261  v.Provides-Extra
-00000320: 3a20 646f 6373 0a50 726f 7669 6465 732d  : docs.Provides-
-00000330: 4578 7472 613a 2074 7574 6f72 6961 6c73  Extra: tutorials
-00000340: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-00000350: 2074 6578 740a 4c69 6365 6e73 652d 4669   text.License-Fi
-00000360: 6c65 3a20 4c49 4345 4e53 450a 0a3c 6120  le: LICENSE..<a 
-00000370: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-00000380: 7468 7562 2e63 6f6d 2f41 6172 6875 732d  thub.com/Aarhus-
-00000390: 5073 7963 6869 6174 7279 2d52 6573 6561  Psychiatry-Resea
-000003a0: 7263 682f 7469 6d65 7365 7269 6573 666c  rch/timeseriesfl
-000003b0: 6174 7465 6e65 7222 3e3c 696d 6720 7372  attener"><img sr
-000003c0: 633d 2268 7474 7073 3a2f 2f67 6974 6875  c="https://githu
-000003d0: 622e 636f 6d2f 4161 7268 7573 2d50 7379  b.com/Aarhus-Psy
-000003e0: 6368 6961 7472 792d 5265 7365 6172 6368  chiatry-Research
-000003f0: 2f74 696d 6573 6572 6965 7366 6c61 7474  /timeseriesflatt
-00000400: 656e 6572 2f62 6c6f 622f 6d61 696e 2f64  ener/blob/main/d
-00000410: 6f63 732f 5f73 7461 7469 632f 6963 6f6e  ocs/_static/icon
-00000420: 2e70 6e67 3f72 6177 3d74 7275 6522 2077  .png?raw=true" w
-00000430: 6964 7468 3d22 3230 3022 2061 6c69 676e  idth="200" align
-00000440: 3d22 7269 6768 7422 2f3e 3c2f 613e 0a0a  ="right"/></a>..
-00000450: 2320 5469 6d65 7365 7269 6573 666c 6174  # Timeseriesflat
-00000460: 7465 6e65 720a 0a5b 215b 6769 7468 7562  tener..[![github
-00000470: 2061 6374 696f 6e73 2064 6f63 735d 2868   actions docs](h
-00000480: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000490: 6d2f 4161 7268 7573 2d50 7379 6368 6961  m/Aarhus-Psychia
-000004a0: 7472 792d 5265 7365 6172 6368 2f74 696d  try-Research/tim
-000004b0: 6573 6572 6965 7366 6c61 7474 656e 6572  eseriesflattener
-000004c0: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-000004d0: 7773 2f64 6f63 756d 656e 7461 7469 6f6e  ws/documentation
-000004e0: 2e79 6d6c 2f62 6164 6765 2e73 7667 295d  .yml/badge.svg)]
-000004f0: 2868 7474 7073 3a2f 2f61 6172 6875 732d  (https://aarhus-
-00000500: 7073 7963 6869 6174 7279 2d72 6573 6561  psychiatry-resea
-00000510: 7263 682e 6769 7468 7562 2e69 6f2f 7469  rch.github.io/ti
-00000520: 6d65 7365 7269 6573 666c 6174 7465 6e65  meseriesflattene
-00000530: 722f 290a 5b21 5b67 6974 6875 6220 6163  r/).[![github ac
-00000540: 7469 6f6e 7320 7079 7465 7374 5d28 6874  tions pytest](ht
-00000550: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000560: 2f41 6172 6875 732d 5073 7963 6869 6174  /Aarhus-Psychiat
-00000570: 7279 2d52 6573 6561 7263 682f 7469 6d65  ry-Research/time
-00000580: 7365 7269 6573 666c 6174 7465 6e65 722f  seriesflattener/
-00000590: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
-000005a0: 732f 6d61 696e 5f74 6573 745f 616e 645f  s/main_test_and_
-000005b0: 7265 6c65 6173 652e 796d 6c2f 6261 6467  release.yml/badg
-000005c0: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
-000005d0: 6769 7468 7562 2e63 6f6d 2f41 6172 6875  github.com/Aarhu
-000005e0: 732d 5073 7963 6869 6174 7279 2d52 6573  s-Psychiatry-Res
-000005f0: 6561 7263 682f 7469 6d65 7365 7269 6573  earch/timeseries
-00000600: 666c 6174 7465 6e65 722f 6163 7469 6f6e  flattener/action
-00000610: 7329 0a5b 215b 7079 7468 6f6e 2076 6572  s).[![python ver
-00000620: 7369 6f6e 735d 2868 7474 7073 3a2f 2f69  sions](https://i
-00000630: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-00000640: 7069 2f70 7976 6572 7369 6f6e 732f 7469  pi/pyversions/ti
-00000650: 6d65 7365 7269 6573 666c 6174 7465 6e65  meseriesflattene
-00000660: 7229 5d28 6874 7470 733a 2f2f 7079 7069  r)](https://pypi
-00000670: 2e6f 7267 2f70 726f 6a65 6374 2f74 696d  .org/project/tim
-00000680: 6573 6572 6965 7366 6c61 7474 656e 6572  eseriesflattener
-00000690: 2f29 0a5b 215b 436f 6465 2073 7479 6c65  /).[![Code style
-000006a0: 3a20 626c 6163 6b5d 2868 7474 7073 3a2f  : black](https:/
-000006b0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-000006c0: 6261 6467 652f 436f 6465 2532 3053 7479  badge/Code%20Sty
-000006d0: 6c65 2d42 6c61 636b 2d62 6c61 636b 295d  le-Black-black)]
-000006e0: 2868 7474 7073 3a2f 2f62 6c61 636b 2e72  (https://black.r
-000006f0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00000700: 2f73 7461 626c 652f 7468 655f 626c 6163  /stable/the_blac
-00000710: 6b5f 636f 6465 5f73 7479 6c65 2f63 7572  k_code_style/cur
-00000720: 7265 6e74 5f73 7479 6c65 2e68 746d 6c29  rent_style.html)
-00000730: 0a0a 5b21 5b50 7950 4920 7665 7273 696f  ..[![PyPI versio
-00000740: 6e5d 2868 7474 7073 3a2f 2f62 6164 6765  n](https://badge
-00000750: 2e66 7572 792e 696f 2f70 792f 7469 6d65  .fury.io/py/time
-00000760: 7365 7269 6573 666c 6174 7465 6e65 722e  seriesflattener.
-00000770: 7376 6729 5d28 6874 7470 733a 2f2f 7079  svg)](https://py
-00000780: 7069 2e6f 7267 2f70 726f 6a65 6374 2f74  pi.org/project/t
-00000790: 696d 6573 6572 6965 7366 6c61 7474 656e  imeseriesflatten
-000007a0: 6572 2f29 0a5b 215b 7374 6174 7573 5d28  er/).[![status](
-000007b0: 6874 7470 733a 2f2f 6a6f 7373 2e74 6865  https://joss.the
-000007c0: 6f6a 2e6f 7267 2f70 6170 6572 732f 3362  oj.org/papers/3b
-000007d0: 6265 6138 3734 3536 3638 6431 6161 3430  bea8745668d1aa40
-000007e0: 6666 3739 3663 3666 6433 6462 3837 2f73  ff796c6fd3db87/s
-000007f0: 7461 7475 732e 7376 6729 5d28 6874 7470  tatus.svg)](http
-00000800: 733a 2f2f 6a6f 7373 2e74 6865 6f6a 2e6f  s://joss.theoj.o
-00000810: 7267 2f70 6170 6572 732f 3362 6265 6138  rg/papers/3bbea8
-00000820: 3734 3536 3638 6431 6161 3430 6666 3739  745668d1aa40ff79
-00000830: 3663 3666 6433 6462 3837 290a 0a54 696d  6c6fd3db87)..Tim
-00000840: 6520 7365 7269 6573 2066 726f 6d20 652e  e series from e.
-00000850: 672e 2065 6c65 6374 726f 6e69 6320 6865  g. electronic he
-00000860: 616c 7468 2072 6563 6f72 6473 206f 6674  alth records oft
-00000870: 656e 2068 6176 6520 6120 6c61 7267 6520  en have a large 
-00000880: 6e75 6d62 6572 206f 6620 7661 7269 6162  number of variab
-00000890: 6c65 732c 2061 7265 2073 616d 706c 6564  les, are sampled
-000008a0: 2061 7420 6972 7265 6775 6c61 7220 696e   at irregular in
-000008b0: 7465 7276 616c 7320 616e 6420 7465 6e64  tervals and tend
-000008c0: 2074 6f20 6861 7665 2061 206c 6172 6765   to have a large
-000008d0: 206e 756d 6265 7220 6f66 206d 6973 7369   number of missi
-000008e0: 6e67 2076 616c 7565 732e 2042 6566 6f72  ng values. Befor
-000008f0: 6520 7468 6973 2074 7970 6520 6f66 2064  e this type of d
-00000900: 6174 6120 6361 6e20 6265 2075 7365 6420  ata can be used 
-00000910: 666f 7220 7072 6564 6963 7469 6f6e 206d  for prediction m
-00000920: 6f64 656c 6c69 6e67 2077 6974 6820 6d61  odelling with ma
-00000930: 6368 696e 6520 6c65 6172 6e69 6e67 206d  chine learning m
-00000940: 6574 686f 6473 2073 7563 6820 6173 206c  ethods such as l
-00000950: 6f67 6973 7469 6320 7265 6772 6573 7369  ogistic regressi
-00000960: 6f6e 206f 7220 5847 426f 6f73 742c 2074  on or XGBoost, t
-00000970: 6865 2064 6174 6120 6e65 6564 7320 746f  he data needs to
-00000980: 2062 6520 7265 7368 6170 6564 2e20 0a0a   be reshaped. ..
-00000990: 496e 2065 7373 656e 6365 2c20 7468 6520  In essence, the 
-000009a0: 7469 6d65 2073 6572 6965 7320 6e65 6564  time series need
-000009b0: 2074 6f20 6265 202a 666c 6174 7465 6e65   to be *flattene
-000009c0: 642a 2073 6f20 7468 6174 2065 6163 6820  d* so that each 
-000009d0: 7072 6564 6963 7469 6f6e 2074 696d 6520  prediction time 
-000009e0: 6973 2072 6570 7265 7365 6e74 6564 2062  is represented b
-000009f0: 7920 6120 7365 7420 6f66 2070 7265 6469  y a set of predi
-00000a00: 6374 6f72 2076 616c 7565 7320 616e 6420  ctor values and 
-00000a10: 616e 206f 7574 636f 6d65 2076 616c 7565  an outcome value
-00000a20: 2e20 5468 6573 6520 7072 6564 6963 746f  . These predicto
-00000a30: 7220 7661 6c75 6573 2063 616e 2062 6520  r values can be 
-00000a40: 636f 6e73 7472 7563 7465 6420 6279 2061  constructed by a
-00000a50: 6767 7265 6761 7469 6e67 2074 6865 2070  ggregating the p
-00000a60: 7265 6365 6469 6e67 2076 616c 7565 7320  receding values 
-00000a70: 696e 2074 6865 2074 696d 6520 7365 7269  in the time seri
-00000a80: 6573 2077 6974 6869 6e20 6120 6365 7274  es within a cert
-00000a90: 6169 6e20 7469 6d65 2077 696e 646f 772e  ain time window.
-00000aa0: 200a 0a60 7469 6d65 7365 7269 6573 666c   ..`timeseriesfl
-00000ab0: 6174 7465 6e65 7260 2061 696d 7320 746f  attener` aims to
-00000ac0: 2073 696d 706c 6966 7920 7468 6973 2070   simplify this p
-00000ad0: 726f 6365 7373 2062 7920 7072 6f76 6964  rocess by provid
-00000ae0: 696e 6720 616e 2065 6173 792d 746f 2d75  ing an easy-to-u
-00000af0: 7365 2061 6e64 2066 756c 6c79 2d73 7065  se and fully-spe
-00000b00: 6369 6669 6564 2070 6970 656c 696e 6520  cified pipeline 
-00000b10: 666f 7220 666c 6174 7465 6e69 6e67 2063  for flattening c
-00000b20: 6f6d 706c 6578 2074 696d 6520 7365 7269  omplex time seri
-00000b30: 6573 2e20 0a0a 2323 20f0 9f94 a720 496e  es. ..## .... In
-00000b40: 7374 616c 6c61 7469 6f6e 0a54 6f20 6765  stallation.To ge
-00000b50: 7420 7374 6172 7465 6420 7573 696e 6720  t started using 
-00000b60: 7469 6d65 7365 7269 6573 666c 6174 7465  timeseriesflatte
-00000b70: 6e65 7220 7369 6d70 6c79 2069 6e73 7461  ner simply insta
-00000b80: 6c6c 2069 7420 7573 696e 6720 7069 7020  ll it using pip 
-00000b90: 6279 2072 756e 6e69 6e67 2074 6865 2066  by running the f
-00000ba0: 6f6c 6c6f 7769 6e67 206c 696e 6520 696e  ollowing line in
-00000bb0: 2079 6f75 7220 7465 726d 696e 616c 3a0a   your terminal:.
-00000bc0: 0a60 6060 0a70 6970 2069 6e73 7461 6c6c  .```.pip install
-00000bd0: 2074 696d 6573 6572 6965 7366 6c61 7474   timeseriesflatt
-00000be0: 656e 6572 0a60 6060 0a0a 2323 20e2 9aa1  ener.```..## ...
-00000bf0: 2051 7569 636b 2073 7461 7274 0a0a 6060   Quick start..``
-00000c00: 6070 790a 696d 706f 7274 206e 756d 7079  `py.import numpy
-00000c10: 2061 7320 6e70 0a69 6d70 6f72 7420 7061   as np.import pa
-00000c20: 6e64 6173 2061 7320 7064 0a0a 6966 205f  ndas as pd..if _
-00000c30: 5f6e 616d 655f 5f20 3d3d 2022 5f5f 6d61  _name__ == "__ma
-00000c40: 696e 5f5f 223a 0a0a 2020 2020 2320 4c6f  in__":..    # Lo
-00000c50: 6164 2061 2064 6174 6166 7261 6d65 2077  ad a dataframe w
-00000c60: 6974 6820 7469 6d65 7320 796f 7520 7769  ith times you wi
-00000c70: 7368 2074 6f20 6d61 6b65 2061 2070 7265  sh to make a pre
-00000c80: 6469 6374 696f 6e0a 2020 2020 7072 6564  diction.    pred
-00000c90: 6963 7469 6f6e 5f74 696d 6573 5f64 6620  iction_times_df 
-00000ca0: 3d20 7064 2e44 6174 6146 7261 6d65 280a  = pd.DataFrame(.
-00000cb0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-00000cc0: 2020 2020 2020 2269 6422 3a20 5b31 2c20        "id": [1, 
-00000cd0: 312c 2032 5d2c 0a20 2020 2020 2020 2020  1, 2],.         
-00000ce0: 2020 2022 6461 7465 223a 205b 2232 3032     "date": ["202
-00000cf0: 302d 3031 2d30 3122 2c20 2232 3032 302d  0-01-01", "2020-
-00000d00: 3032 2d30 3122 2c20 2232 3032 302d 3032  02-01", "2020-02
-00000d10: 2d30 3122 5d2c 0a20 2020 2020 2020 207d  -01"],.        }
-00000d20: 2c0a 2020 2020 290a 2020 2020 2320 4c6f  ,.    ).    # Lo
-00000d30: 6164 2061 2064 6174 6166 7261 6d65 2077  ad a dataframe w
-00000d40: 6974 6820 7261 7720 7661 6c75 6573 2079  ith raw values y
-00000d50: 6f75 2077 6973 6820 746f 2061 6767 7265  ou wish to aggre
-00000d60: 6761 7465 2061 7320 7072 6564 6963 746f  gate as predicto
-00000d70: 7273 0a20 2020 2070 7265 6469 6374 6f72  rs.    predictor
-00000d80: 5f64 6620 3d20 7064 2e44 6174 6146 7261  _df = pd.DataFra
-00000d90: 6d65 280a 2020 2020 2020 2020 7b0a 2020  me(.        {.  
-00000da0: 2020 2020 2020 2020 2020 2269 6422 3a20            "id": 
-00000db0: 5b31 2c20 312c 2031 2c20 325d 2c0a 2020  [1, 1, 1, 2],.  
-00000dc0: 2020 2020 2020 2020 2020 2264 6174 6522            "date"
-00000dd0: 3a20 5b0a 2020 2020 2020 2020 2020 2020  : [.            
-00000de0: 2020 2020 2232 3032 302d 3031 2d31 3522      "2020-01-15"
-00000df0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000e00: 2020 2232 3031 392d 3132 2d31 3022 2c0a    "2019-12-10",.
-00000e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e20: 2232 3031 392d 3132 2d31 3522 2c0a 2020  "2019-12-15",.  
-00000e30: 2020 2020 2020 2020 2020 2020 2020 2232                "2
-00000e40: 3032 302d 3031 2d30 3222 2c0a 2020 2020  020-01-02",.    
-00000e50: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
-00000e60: 2020 2020 2020 2022 7661 6c75 6522 3a20         "value": 
-00000e70: 5b31 2c20 322c 2033 2c20 345d 2c0a 2020  [1, 2, 3, 4],.  
-00000e80: 2020 2020 2020 7d2c 0a20 2020 2029 0a20        },.    ). 
-00000e90: 2020 2023 204c 6f61 6420 6120 6461 7461     # Load a data
-00000ea0: 6672 616d 6520 7370 6563 6966 7969 6e67  frame specifying
-00000eb0: 2077 6865 6e20 7468 6520 6f75 7463 6f6d   when the outcom
-00000ec0: 6520 6f63 6375 7273 0a20 2020 206f 7574  e occurs.    out
-00000ed0: 636f 6d65 5f64 6620 3d20 7064 2e44 6174  come_df = pd.Dat
-00000ee0: 6146 7261 6d65 287b 2269 6422 3a20 5b31  aFrame({"id": [1
-00000ef0: 5d2c 2022 6461 7465 223a 205b 2232 3032  ], "date": ["202
-00000f00: 302d 3033 2d30 3122 5d2c 2022 7661 6c75  0-03-01"], "valu
-00000f10: 6522 3a20 5b31 5d7d 290a 0a20 2020 2023  e": [1]})..    #
-00000f20: 2053 7065 6369 6679 2068 6f77 2074 6f20   Specify how to 
-00000f30: 6167 6772 6567 6174 6520 7468 6520 7072  aggregate the pr
-00000f40: 6564 6963 746f 7273 2061 6e64 2064 6566  edictors and def
-00000f50: 696e 6520 7468 6520 6f75 7463 6f6d 650a  ine the outcome.
-00000f60: 2020 2020 6672 6f6d 2074 696d 6573 6572      from timeser
-00000f70: 6965 7366 6c61 7474 656e 6572 2e66 6561  iesflattener.fea
-00000f80: 7475 7265 5f73 7065 635f 6f62 6a65 6374  ture_spec_object
-00000f90: 7320 696d 706f 7274 204f 7574 636f 6d65  s import Outcome
-00000fa0: 5370 6563 2c20 5072 6564 6963 746f 7253  Spec, PredictorS
-00000fb0: 7065 630a 2020 2020 6672 6f6d 2074 696d  pec.    from tim
-00000fc0: 6573 6572 6965 7366 6c61 7474 656e 6572  eseriesflattener
-00000fd0: 2e72 6573 6f6c 7665 5f6d 756c 7469 706c  .resolve_multipl
-00000fe0: 655f 6675 6e63 7469 6f6e 7320 696d 706f  e_functions impo
-00000ff0: 7274 206d 6178 696d 756d 2c20 6d65 616e  rt maximum, mean
-00001000: 0a0a 2020 2020 7072 6564 6963 746f 725f  ..    predictor_
-00001010: 7370 6563 203d 2050 7265 6469 6374 6f72  spec = Predictor
-00001020: 5370 6563 280a 2020 2020 2020 2020 7661  Spec(.        va
-00001030: 6c75 6573 5f64 663d 7072 6564 6963 746f  lues_df=predicto
-00001040: 725f 6466 2c0a 2020 2020 2020 2020 6c6f  r_df,.        lo
-00001050: 6f6b 6265 6869 6e64 5f64 6179 733d 3330  okbehind_days=30
-00001060: 2c0a 2020 2020 2020 2020 6661 6c6c 6261  ,.        fallba
-00001070: 636b 3d6e 702e 6e61 6e2c 0a20 2020 2020  ck=np.nan,.     
-00001080: 2020 2065 6e74 6974 795f 6964 5f63 6f6c     entity_id_col
-00001090: 5f6e 616d 653d 2269 6422 2c0a 2020 2020  _name="id",.    
-000010a0: 2020 2020 7265 736f 6c76 655f 6d75 6c74      resolve_mult
-000010b0: 6970 6c65 5f66 6e3d 6d65 616e 2c0a 2020  iple_fn=mean,.  
-000010c0: 2020 2020 2020 6665 6174 7572 655f 6e61        feature_na
-000010d0: 6d65 3d22 7465 7374 5f66 6561 7475 7265  me="test_feature
-000010e0: 222c 0a20 2020 2029 0a20 2020 206f 7574  ",.    ).    out
-000010f0: 636f 6d65 5f73 7065 6320 3d20 4f75 7463  come_spec = Outc
-00001100: 6f6d 6553 7065 6328 0a20 2020 2020 2020  omeSpec(.       
-00001110: 2076 616c 7565 735f 6466 3d6f 7574 636f   values_df=outco
-00001120: 6d65 5f64 662c 0a20 2020 2020 2020 206c  me_df,.        l
-00001130: 6f6f 6b61 6865 6164 5f64 6179 733d 3331  ookahead_days=31
-00001140: 2c0a 2020 2020 2020 2020 6661 6c6c 6261  ,.        fallba
-00001150: 636b 3d30 2c0a 2020 2020 2020 2020 656e  ck=0,.        en
-00001160: 7469 7479 5f69 645f 636f 6c5f 6e61 6d65  tity_id_col_name
-00001170: 3d22 6964 222c 0a20 2020 2020 2020 2072  ="id",.        r
-00001180: 6573 6f6c 7665 5f6d 756c 7469 706c 655f  esolve_multiple_
-00001190: 666e 3d6d 6178 696d 756d 2c0a 2020 2020  fn=maximum,.    
-000011a0: 2020 2020 6665 6174 7572 655f 6e61 6d65      feature_name
-000011b0: 3d22 7465 7374 5f6f 7574 636f 6d65 222c  ="test_outcome",
-000011c0: 0a20 2020 2020 2020 2069 6e63 6964 656e  .        inciden
-000011d0: 743d 4661 6c73 652c 0a20 2020 2029 0a0a  t=False,.    )..
-000011e0: 2020 2020 2320 496e 7374 616e 7469 6174      # Instantiat
-000011f0: 6520 5469 6d65 7365 7269 6573 466c 6174  e TimeseriesFlat
-00001200: 7465 6e65 7220 616e 6420 6164 6420 7468  tener and add th
-00001210: 6520 7370 6563 6966 6963 6174 696f 6e73  e specifications
-00001220: 0a20 2020 2066 726f 6d20 7469 6d65 7365  .    from timese
-00001230: 7269 6573 666c 6174 7465 6e65 7220 696d  riesflattener im
-00001240: 706f 7274 2054 696d 6573 6572 6965 7346  port TimeseriesF
-00001250: 6c61 7474 656e 6572 0a0a 2020 2020 7473  lattener..    ts
-00001260: 5f66 6c61 7474 656e 6572 203d 2054 696d  _flattener = Tim
-00001270: 6573 6572 6965 7346 6c61 7474 656e 6572  eseriesFlattener
-00001280: 280a 2020 2020 2020 2020 7072 6564 6963  (.        predic
-00001290: 7469 6f6e 5f74 696d 6573 5f64 663d 7072  tion_times_df=pr
-000012a0: 6564 6963 7469 6f6e 5f74 696d 6573 5f64  ediction_times_d
-000012b0: 662c 0a20 2020 2020 2020 2065 6e74 6974  f,.        entit
-000012c0: 795f 6964 5f63 6f6c 5f6e 616d 653d 2269  y_id_col_name="i
-000012d0: 6422 2c0a 2020 2020 2020 2020 7469 6d65  d",.        time
-000012e0: 7374 616d 705f 636f 6c5f 6e61 6d65 3d22  stamp_col_name="
-000012f0: 6461 7465 222c 0a20 2020 2020 2020 206e  date",.        n
-00001300: 5f77 6f72 6b65 7273 3d31 2c0a 2020 2020  _workers=1,.    
-00001310: 2020 2020 6472 6f70 5f70 7265 645f 7469      drop_pred_ti
-00001320: 6d65 735f 7769 7468 5f69 6e73 7566 6669  mes_with_insuffi
-00001330: 6369 656e 745f 6c6f 6f6b 5f64 6973 7461  cient_look_dista
-00001340: 6e63 653d 4661 6c73 652c 0a20 2020 2029  nce=False,.    )
-00001350: 0a20 2020 2074 735f 666c 6174 7465 6e65  .    ts_flattene
-00001360: 722e 6164 645f 7370 6563 285b 7072 6564  r.add_spec([pred
-00001370: 6963 746f 725f 7370 6563 2c20 6f75 7463  ictor_spec, outc
-00001380: 6f6d 655f 7370 6563 5d29 0a20 2020 2064  ome_spec]).    d
-00001390: 6620 3d20 7473 5f66 6c61 7474 656e 6572  f = ts_flattener
-000013a0: 2e67 6574 5f64 6628 290a 2020 2020 6466  .get_df().    df
-000013b0: 0a60 6060 0a4f 7574 7075 743a 0a0a 7c20  .```.Output:..| 
-000013c0: 2020 2020 207c 2020 2069 6420 7c20 6461       |   id | da
-000013d0: 7465 2020 2020 2020 2020 2020 2020 2020  te              
-000013e0: 2020 7c20 7072 6564 6963 7469 6f6e 5f74    | prediction_t
-000013f0: 696d 655f 7575 6964 2020 7c20 7072 6564  ime_uuid  | pred
-00001400: 5f74 6573 745f 6665 6174 7572 655f 7769  _test_feature_wi
-00001410: 7468 696e 5f33 305f 6461 7973 5f6d 6561  thin_30_days_mea
-00001420: 6e5f 6661 6c6c 6261 636b 5f6e 616e 207c  n_fallback_nan |
-00001430: 206f 7574 635f 7465 7374 5f6f 7574 636f   outc_test_outco
-00001440: 6d65 5f77 6974 6869 6e5f 3331 5f64 6179  me_within_31_day
-00001450: 735f 6d61 7869 6d75 6d5f 6661 6c6c 6261  s_maximum_fallba
-00001460: 636b 5f30 5f64 6963 686f 746f 6d6f 7573  ck_0_dichotomous
-00001470: 207c 0a7c 202d 2d2d 3a20 7c20 2d2d 2d3a   |.| ---: | ---:
-00001480: 207c 203a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   | :------------
-00001490: 2d2d 2d2d 2d2d 207c 203a 2d2d 2d2d 2d2d  ------ | :------
-000014a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c  -------------- |
-000014b0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
-000014c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000014d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000014e0: 2d2d 3a20 7c20 2d2d 2d2d 2d2d 2d2d 2d2d  --: | ----------
-000014f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001520: 2d2d 2d2d 3a20 7c0a 7c20 2020 2030 207c  ----: |.|    0 |
-00001530: 2020 2020 3120 7c20 3230 3230 2d30 312d      1 | 2020-01-
-00001540: 3031 2030 303a 3030 3a30 3020 7c20 312d  01 00:00:00 | 1-
-00001550: 3230 3230 2d30 312d 3031 2d30 302d 3030  2020-01-01-00-00
-00001560: 2d30 3020 7c20 2020 2020 2020 2020 2020  -00 |           
-00001570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001590: 2020 2020 2032 2e35 207c 2020 2020 2020       2.5 |      
-000015a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015d0: 2020 2020 2020 2020 2030 207c 0a7c 2020           0 |.|  
-000015e0: 2020 3120 7c20 2020 2031 207c 2032 3032    1 |    1 | 202
-000015f0: 302d 3032 2d30 3120 3030 3a30 303a 3030  0-02-01 00:00:00
-00001600: 207c 2031 2d32 3032 302d 3032 2d30 312d   | 1-2020-02-01-
-00001610: 3030 2d30 302d 3030 207c 2020 2020 2020  00-00-00 |      
-00001620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001640: 2020 2020 2020 2020 2020 2020 3120 7c20              1 | 
-00001650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001680: 2020 2020 2020 2020 2020 2020 2020 3120                1 
-00001690: 7c0a 7c20 2020 2032 207c 2020 2020 3220  |.|    2 |    2 
-000016a0: 7c20 3230 3230 2d30 322d 3031 2030 303a  | 2020-02-01 00:
-000016b0: 3030 3a30 3020 7c20 322d 3230 3230 2d30  00:00 | 2-2020-0
-000016c0: 322d 3031 2d30 302d 3030 2d30 3020 7c20  2-01-00-00-00 | 
-000016d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001700: 2034 207c 2020 2020 2020 2020 2020 2020   4 |            
-00001710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001740: 2020 2030 207c 0a0a 0a23 2320 f09f 9396     0 |...## ....
-00001750: 2044 6f63 756d 656e 7461 7469 6f6e 0a0a   Documentation..
-00001760: 7c20 446f 6375 6d65 6e74 6174 696f 6e20  | Documentation 
-00001770: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00001780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017d0: 2020 7c0a 7c20 2d2d 2d2d 2d2d 2d2d 2d2d    |.| ----------
-000017e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c 202d  ------------ | -
-000017f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001800: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001810: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001820: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001830: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001840: 2d2d 2d2d 2d20 7c0a 7c20 f09f 8e93 202a  ----- |.| .... *
-00001850: 2a5b 5475 746f 7269 616c 5d2a 2a20 2020  *[Tutorial]**   
-00001860: 2020 2020 7c20 5369 6d70 6c65 2061 6e64      | Simple and
-00001870: 2061 6476 616e 6365 6420 7475 746f 7269   advanced tutori
-00001880: 616c 7320 746f 2067 6574 2079 6f75 2073  als to get you s
-00001890: 7461 7274 6564 2075 7369 6e67 2060 7469  tarted using `ti
-000018a0: 6d65 7365 7269 6573 666c 6174 7465 6e65  meseriesflattene
-000018b0: 7260 2020 2020 2020 2020 2020 207c 0a7c  r`           |.|
-000018c0: 20f0 9f8e 9b20 2a2a 5b47 656e 6572 616c   .... **[General
-000018d0: 2064 6f63 735d 2a2a 207c 2054 6865 2064   docs]** | The d
-000018e0: 6574 6169 6c65 6420 7265 6665 7265 6e63  etailed referenc
-000018f0: 6520 666f 7220 7469 6d65 7365 7269 6573  e for timeseries
-00001900: 666c 6174 7465 6e65 7227 7320 4150 492e  flattener's API.
-00001910: 207c 0a7c 20f0 9f99 8b20 2a2a 5b46 4151   |.| .... **[FAQ
-00001920: 5d2a 2a20 2020 2020 2020 2020 2020 207c  ]**            |
-00001930: 2046 7265 7175 656e 746c 7920 6173 6b65   Frequently aske
-00001940: 6420 7175 6573 7469 6f6e 2020 2020 2020  d question      
-00001950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001980: 2020 2020 2020 2020 7c0a 7c20 f09f 97ba          |.| ....
-00001990: efb8 8f20 2a2a 5b52 6f61 646d 6170 5d2a  ... **[Roadmap]*
-000019a0: 2a20 2020 2020 2020 207c 204b 616e 6261  *        | Kanba
-000019b0: 6e20 626f 6172 6420 666f 7220 7468 6520  n board for the 
-000019c0: 726f 6164 6d61 7020 666f 7220 7468 6520  roadmap for the 
-000019d0: 7072 6f6a 6563 7420 2020 2020 2020 2020  project         
-000019e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a00: 2020 7c0a 0a5b 5475 746f 7269 616c 5d3a    |..[Tutorial]:
-00001a10: 2068 7474 7073 3a2f 2f61 6172 6875 732d   https://aarhus-
-00001a20: 7073 7963 6869 6174 7279 2d72 6573 6561  psychiatry-resea
-00001a30: 7263 682e 6769 7468 7562 2e69 6f2f 7469  rch.github.io/ti
-00001a40: 6d65 7365 7269 6573 666c 6174 7465 6e65  meseriesflattene
-00001a50: 722f 7475 746f 7269 616c 732e 6874 6d6c  r/tutorials.html
-00001a60: 0a5b 4765 6e65 7261 6c20 646f 6373 5d3a  .[General docs]:
-00001a70: 2068 7474 7073 3a2f 2f41 6172 6875 732d   https://Aarhus-
-00001a80: 5073 7963 6869 6174 7279 2d52 6573 6561  Psychiatry-Resea
-00001a90: 7263 682e 6769 7468 7562 2e69 6f2f 7469  rch.github.io/ti
-00001aa0: 6d65 7365 7269 6573 666c 6174 7465 6e65  meseriesflattene
-00001ab0: 722f 0a5b 4641 515d 3a20 6874 7470 733a  r/.[FAQ]: https:
-00001ac0: 2f2f 4161 7268 7573 2d50 7379 6368 6961  //Aarhus-Psychia
-00001ad0: 7472 792d 5265 7365 6172 6368 2e67 6974  try-Research.git
-00001ae0: 6875 622e 696f 2f74 696d 6573 6572 6965  hub.io/timeserie
-00001af0: 7366 6c61 7474 656e 6572 2f66 6171 2e68  sflattener/faq.h
-00001b00: 746d 6c0a 5b52 6f61 646d 6170 5d3a 2068  tml.[Roadmap]: h
-00001b10: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001b20: 6d2f 6f72 6773 2f41 6172 6875 732d 5073  m/orgs/Aarhus-Ps
-00001b30: 7963 6869 6174 7279 2d52 6573 6561 7263  ychiatry-Researc
-00001b40: 682f 7072 6f6a 6563 7473 2f31 312f 7669  h/projects/11/vi
-00001b50: 6577 732f 310a 0a23 2320 f09f 92ac 2057  ews/1..## .... W
-00001b60: 6865 7265 2074 6f20 6173 6b20 7175 6573  here to ask ques
-00001b70: 7469 6f6e 730a 0a7c 2054 7970 6520 2020  tions..| Type   
-00001b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b90: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00000150: 2e63 6f6d 3e0a 4c69 6365 6e73 653a 204d  .com>.License: M
+00000160: 4954 204c 6963 656e 7365 0a20 2020 2020  IT License.     
+00000170: 2020 200a 2020 2020 2020 2020 436f 7079     .        Copy
+00000180: 7269 6768 7420 2863 2920 3230 3232 2050  right (c) 2022 P
+00000190: 5359 434f 5020 4772 6f75 702c 2041 6172  SYCOP Group, Aar
+000001a0: 6875 7320 556e 6976 6572 7369 7479 0a20  hus University. 
+000001b0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000001c0: 5065 726d 6973 7369 6f6e 2069 7320 6865  Permission is he
+000001d0: 7265 6279 2067 7261 6e74 6564 2c20 6672  reby granted, fr
+000001e0: 6565 206f 6620 6368 6172 6765 2c20 746f  ee of charge, to
+000001f0: 2061 6e79 2070 6572 736f 6e20 6f62 7461   any person obta
+00000200: 696e 696e 6720 6120 636f 7079 0a20 2020  ining a copy.   
+00000210: 2020 2020 206f 6620 7468 6973 2073 6f66       of this sof
+00000220: 7477 6172 6520 616e 6420 6173 736f 6369  tware and associ
+00000230: 6174 6564 2064 6f63 756d 656e 7461 7469  ated documentati
+00000240: 6f6e 2066 696c 6573 2028 7468 6520 2253  on files (the "S
+00000250: 6f66 7477 6172 6522 292c 2074 6f20 6465  oftware"), to de
+00000260: 616c 0a20 2020 2020 2020 2069 6e20 7468  al.        in th
+00000270: 6520 536f 6674 7761 7265 2077 6974 686f  e Software witho
+00000280: 7574 2072 6573 7472 6963 7469 6f6e 2c20  ut restriction, 
+00000290: 696e 636c 7564 696e 6720 7769 7468 6f75  including withou
+000002a0: 7420 6c69 6d69 7461 7469 6f6e 2074 6865  t limitation the
+000002b0: 2072 6967 6874 730a 2020 2020 2020 2020   rights.        
+000002c0: 746f 2075 7365 2c20 636f 7079 2c20 6d6f  to use, copy, mo
+000002d0: 6469 6679 2c20 6d65 7267 652c 2070 7562  dify, merge, pub
+000002e0: 6c69 7368 2c20 6469 7374 7269 6275 7465  lish, distribute
+000002f0: 2c20 7375 626c 6963 656e 7365 2c20 616e  , sublicense, an
+00000300: 642f 6f72 2073 656c 6c0a 2020 2020 2020  d/or sell.      
+00000310: 2020 636f 7069 6573 206f 6620 7468 6520    copies of the 
+00000320: 536f 6674 7761 7265 2c20 616e 6420 746f  Software, and to
+00000330: 2070 6572 6d69 7420 7065 7273 6f6e 7320   permit persons 
+00000340: 746f 2077 686f 6d20 7468 6520 536f 6674  to whom the Soft
+00000350: 7761 7265 2069 730a 2020 2020 2020 2020  ware is.        
+00000360: 6675 726e 6973 6865 6420 746f 2064 6f20  furnished to do 
+00000370: 736f 2c20 7375 626a 6563 7420 746f 2074  so, subject to t
+00000380: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6e  he following con
+00000390: 6469 7469 6f6e 733a 0a20 2020 2020 2020  ditions:.       
+000003a0: 200a 2020 2020 2020 2020 5468 6520 6162   .        The ab
+000003b0: 6f76 6520 636f 7079 7269 6768 7420 6e6f  ove copyright no
+000003c0: 7469 6365 2061 6e64 2074 6869 7320 7065  tice and this pe
+000003d0: 726d 6973 7369 6f6e 206e 6f74 6963 6520  rmission notice 
+000003e0: 7368 616c 6c20 6265 2069 6e63 6c75 6465  shall be include
+000003f0: 6420 696e 2061 6c6c 0a20 2020 2020 2020  d in all.       
+00000400: 2063 6f70 6965 7320 6f72 2073 7562 7374   copies or subst
+00000410: 616e 7469 616c 2070 6f72 7469 6f6e 7320  antial portions 
+00000420: 6f66 2074 6865 2053 6f66 7477 6172 652e  of the Software.
+00000430: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00000440: 2020 5448 4520 534f 4654 5741 5245 2049    THE SOFTWARE I
+00000450: 5320 5052 4f56 4944 4544 2022 4153 2049  S PROVIDED "AS I
+00000460: 5322 2c20 5749 5448 4f55 5420 5741 5252  S", WITHOUT WARR
+00000470: 414e 5459 204f 4620 414e 5920 4b49 4e44  ANTY OF ANY KIND
+00000480: 2c20 4558 5052 4553 5320 4f52 0a20 2020  , EXPRESS OR.   
+00000490: 2020 2020 2049 4d50 4c49 4544 2c20 494e       IMPLIED, IN
+000004a0: 434c 5544 494e 4720 4255 5420 4e4f 5420  CLUDING BUT NOT 
+000004b0: 4c49 4d49 5445 4420 544f 2054 4845 2057  LIMITED TO THE W
+000004c0: 4152 5241 4e54 4945 5320 4f46 204d 4552  ARRANTIES OF MER
+000004d0: 4348 414e 5441 4249 4c49 5459 2c0a 2020  CHANTABILITY,.  
+000004e0: 2020 2020 2020 4649 544e 4553 5320 464f        FITNESS FO
+000004f0: 5220 4120 5041 5254 4943 554c 4152 2050  R A PARTICULAR P
+00000500: 5552 504f 5345 2041 4e44 204e 4f4e 494e  URPOSE AND NONIN
+00000510: 4652 494e 4745 4d45 4e54 2e20 494e 204e  FRINGEMENT. IN N
+00000520: 4f20 4556 454e 5420 5348 414c 4c20 5448  O EVENT SHALL TH
+00000530: 450a 2020 2020 2020 2020 4155 5448 4f52  E.        AUTHOR
+00000540: 5320 4f52 2043 4f50 5952 4947 4854 2048  S OR COPYRIGHT H
+00000550: 4f4c 4445 5253 2042 4520 4c49 4142 4c45  OLDERS BE LIABLE
+00000560: 2046 4f52 2041 4e59 2043 4c41 494d 2c20   FOR ANY CLAIM, 
+00000570: 4441 4d41 4745 5320 4f52 204f 5448 4552  DAMAGES OR OTHER
+00000580: 0a20 2020 2020 2020 204c 4941 4249 4c49  .        LIABILI
+00000590: 5459 2c20 5748 4554 4845 5220 494e 2041  TY, WHETHER IN A
+000005a0: 4e20 4143 5449 4f4e 204f 4620 434f 4e54  N ACTION OF CONT
+000005b0: 5241 4354 2c20 544f 5254 204f 5220 4f54  RACT, TORT OR OT
+000005c0: 4845 5257 4953 452c 2041 5249 5349 4e47  HERWISE, ARISING
+000005d0: 2046 524f 4d2c 0a20 2020 2020 2020 204f   FROM,.        O
+000005e0: 5554 204f 4620 4f52 2049 4e20 434f 4e4e  UT OF OR IN CONN
+000005f0: 4543 5449 4f4e 2057 4954 4820 5448 4520  ECTION WITH THE 
+00000600: 534f 4654 5741 5245 204f 5220 5448 4520  SOFTWARE OR THE 
+00000610: 5553 4520 4f52 204f 5448 4552 2044 4541  USE OR OTHER DEA
+00000620: 4c49 4e47 5320 494e 2054 4845 0a20 2020  LINGS IN THE.   
+00000630: 2020 2020 2053 4f46 5457 4152 452e 0a50       SOFTWARE..P
+00000640: 726f 6a65 6374 2d55 524c 3a20 686f 6d65  roject-URL: home
+00000650: 7061 6765 2c20 6874 7470 733a 2f2f 6769  page, https://gi
+00000660: 7468 7562 2e63 6f6d 2f4d 6172 7469 6e42  thub.com/MartinB
+00000670: 6572 6e73 746f 7266 662f 7469 6d65 7365  ernstorff/timese
+00000680: 7269 6573 666c 6174 7465 6e65 720a 5072  riesflattener.Pr
+00000690: 6f6a 6563 742d 5552 4c3a 2072 6570 6f73  oject-URL: repos
+000006a0: 6974 6f72 792c 2068 7474 7073 3a2f 2f67  itory, https://g
+000006b0: 6974 6875 622e 636f 6d2f 4d61 7274 696e  ithub.com/Martin
+000006c0: 4265 726e 7374 6f72 6666 2f74 696d 6573  Bernstorff/times
+000006d0: 6572 6965 7366 6c61 7474 656e 6572 0a50  eriesflattener.P
+000006e0: 726f 6a65 6374 2d55 524c 3a20 646f 6375  roject-URL: docu
+000006f0: 6d65 6e74 6174 696f 6e2c 2068 7474 7073  mentation, https
+00000700: 3a2f 2f4d 6172 7469 6e42 6572 6e73 746f  ://MartinBernsto
+00000710: 7266 662e 6769 7468 7562 2e69 6f2f 7469  rff.github.io/ti
+00000720: 6d65 7365 7269 6573 666c 6174 7465 6e65  meseriesflattene
+00000730: 722f 0a43 6c61 7373 6966 6965 723a 204f  r/.Classifier: O
+00000740: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+00000750: 3a3a 2050 4f53 4958 203a 3a20 4c69 6e75  :: POSIX :: Linu
+00000760: 780a 436c 6173 7369 6669 6572 3a20 4f70  x.Classifier: Op
+00000770: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
+00000780: 3a20 4d61 634f 5320 3a3a 204d 6163 4f53  : MacOS :: MacOS
+00000790: 2058 0a43 6c61 7373 6966 6965 723a 204f   X.Classifier: O
+000007a0: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+000007b0: 3a3a 204d 6963 726f 736f 6674 203a 3a20  :: Microsoft :: 
+000007c0: 5769 6e64 6f77 730a 436c 6173 7369 6669  Windows.Classifi
+000007d0: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+000007e0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000007f0: 6f6e 203a 3a20 332e 380a 436c 6173 7369  on :: 3.8.Classi
+00000800: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+00000810: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000820: 7468 6f6e 203a 3a20 332e 390a 436c 6173  thon :: 3.9.Clas
+00000830: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00000840: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000850: 5079 7468 6f6e 203a 3a20 332e 3130 0a43  Python :: 3.10.C
+00000860: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+00000870: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000880: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
+00000890: 310a 5265 7175 6972 6573 2d50 7974 686f  1.Requires-Pytho
+000008a0: 6e3a 203c 332e 3132 2e30 2c3e 3d33 2e38  n: <3.12.0,>=3.8
+000008b0: 2e30 0a44 6573 6372 6970 7469 6f6e 2d43  .0.Description-C
+000008c0: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
+000008d0: 742f 6d61 726b 646f 776e 0a50 726f 7669  t/markdown.Provi
+000008e0: 6465 732d 4578 7472 613a 2064 6576 0a50  des-Extra: dev.P
+000008f0: 726f 7669 6465 732d 4578 7472 613a 2074  rovides-Extra: t
+00000900: 6573 740a 5072 6f76 6964 6573 2d45 7874  est.Provides-Ext
+00000910: 7261 3a20 646f 6373 0a50 726f 7669 6465  ra: docs.Provide
+00000920: 732d 4578 7472 613a 2074 7574 6f72 6961  s-Extra: tutoria
+00000930: 6c73 0a50 726f 7669 6465 732d 4578 7472  ls.Provides-Extr
+00000940: 613a 2074 6578 740a 4c69 6365 6e73 652d  a: text.License-
+00000950: 4669 6c65 3a20 4c49 4345 4e53 450a 0a3c  File: LICENSE..<
+00000960: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000970: 6769 7468 7562 2e63 6f6d 2f41 6172 6875  github.com/Aarhu
+00000980: 732d 5073 7963 6869 6174 7279 2d52 6573  s-Psychiatry-Res
+00000990: 6561 7263 682f 7469 6d65 7365 7269 6573  earch/timeseries
+000009a0: 666c 6174 7465 6e65 7222 3e3c 696d 6720  flattener"><img 
+000009b0: 7372 633d 2268 7474 7073 3a2f 2f67 6974  src="https://git
+000009c0: 6875 622e 636f 6d2f 4161 7268 7573 2d50  hub.com/Aarhus-P
+000009d0: 7379 6368 6961 7472 792d 5265 7365 6172  sychiatry-Resear
+000009e0: 6368 2f74 696d 6573 6572 6965 7366 6c61  ch/timeseriesfla
+000009f0: 7474 656e 6572 2f62 6c6f 622f 6d61 696e  ttener/blob/main
+00000a00: 2f64 6f63 732f 5f73 7461 7469 632f 6963  /docs/_static/ic
+00000a10: 6f6e 2e70 6e67 3f72 6177 3d74 7275 6522  on.png?raw=true"
+00000a20: 2077 6964 7468 3d22 3230 3022 2061 6c69   width="200" ali
+00000a30: 676e 3d22 7269 6768 7422 2f3e 3c2f 613e  gn="right"/></a>
+00000a40: 0a0a 2320 5469 6d65 7365 7269 6573 666c  ..# Timeseriesfl
+00000a50: 6174 7465 6e65 720a 0a5b 215b 6769 7468  attener..[![gith
+00000a60: 7562 2061 6374 696f 6e73 2064 6f63 735d  ub actions docs]
+00000a70: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000a80: 636f 6d2f 4161 7268 7573 2d50 7379 6368  com/Aarhus-Psych
+00000a90: 6961 7472 792d 5265 7365 6172 6368 2f74  iatry-Research/t
+00000aa0: 696d 6573 6572 6965 7366 6c61 7474 656e  imeseriesflatten
+00000ab0: 6572 2f61 6374 696f 6e73 2f77 6f72 6b66  er/actions/workf
+00000ac0: 6c6f 7773 2f64 6f63 756d 656e 7461 7469  lows/documentati
+00000ad0: 6f6e 2e79 6d6c 2f62 6164 6765 2e73 7667  on.yml/badge.svg
+00000ae0: 295d 2868 7474 7073 3a2f 2f61 6172 6875  )](https://aarhu
+00000af0: 732d 7073 7963 6869 6174 7279 2d72 6573  s-psychiatry-res
+00000b00: 6561 7263 682e 6769 7468 7562 2e69 6f2f  earch.github.io/
+00000b10: 7469 6d65 7365 7269 6573 666c 6174 7465  timeseriesflatte
+00000b20: 6e65 722f 290a 5b21 5b67 6974 6875 6220  ner/).[![github 
+00000b30: 6163 7469 6f6e 7320 7079 7465 7374 5d28  actions pytest](
+00000b40: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000b50: 6f6d 2f41 6172 6875 732d 5073 7963 6869  om/Aarhus-Psychi
+00000b60: 6174 7279 2d52 6573 6561 7263 682f 7469  atry-Research/ti
+00000b70: 6d65 7365 7269 6573 666c 6174 7465 6e65  meseriesflattene
+00000b80: 722f 6163 7469 6f6e 732f 776f 726b 666c  r/actions/workfl
+00000b90: 6f77 732f 6d61 696e 5f74 6573 745f 616e  ows/main_test_an
+00000ba0: 645f 7265 6c65 6173 652e 796d 6c2f 6261  d_release.yml/ba
+00000bb0: 6467 652e 7376 6729 5d28 6874 7470 733a  dge.svg)](https:
+00000bc0: 2f2f 6769 7468 7562 2e63 6f6d 2f41 6172  //github.com/Aar
+00000bd0: 6875 732d 5073 7963 6869 6174 7279 2d52  hus-Psychiatry-R
+00000be0: 6573 6561 7263 682f 7469 6d65 7365 7269  esearch/timeseri
+00000bf0: 6573 666c 6174 7465 6e65 722f 6163 7469  esflattener/acti
+00000c00: 6f6e 7329 0a5b 215b 7079 7468 6f6e 2076  ons).[![python v
+00000c10: 6572 7369 6f6e 735d 2868 7474 7073 3a2f  ersions](https:/
+00000c20: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000c30: 7079 7069 2f70 7976 6572 7369 6f6e 732f  pypi/pyversions/
+00000c40: 7469 6d65 7365 7269 6573 666c 6174 7465  timeseriesflatte
+00000c50: 6e65 7229 5d28 6874 7470 733a 2f2f 7079  ner)](https://py
+00000c60: 7069 2e6f 7267 2f70 726f 6a65 6374 2f74  pi.org/project/t
+00000c70: 696d 6573 6572 6965 7366 6c61 7474 656e  imeseriesflatten
+00000c80: 6572 2f29 0a5b 215b 436f 6465 2073 7479  er/).[![Code sty
+00000c90: 6c65 3a20 626c 6163 6b5d 2868 7474 7073  le: black](https
+00000ca0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000cb0: 6f2f 6261 6467 652f 436f 6465 2532 3053  o/badge/Code%20S
+00000cc0: 7479 6c65 2d42 6c61 636b 2d62 6c61 636b  tyle-Black-black
+00000cd0: 295d 2868 7474 7073 3a2f 2f62 6c61 636b  )](https://black
+00000ce0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00000cf0: 656e 2f73 7461 626c 652f 7468 655f 626c  en/stable/the_bl
+00000d00: 6163 6b5f 636f 6465 5f73 7479 6c65 2f63  ack_code_style/c
+00000d10: 7572 7265 6e74 5f73 7479 6c65 2e68 746d  urrent_style.htm
+00000d20: 6c29 0a0a 5b21 5b50 7950 4920 7665 7273  l)..[![PyPI vers
+00000d30: 696f 6e5d 2868 7474 7073 3a2f 2f62 6164  ion](https://bad
+00000d40: 6765 2e66 7572 792e 696f 2f70 792f 7469  ge.fury.io/py/ti
+00000d50: 6d65 7365 7269 6573 666c 6174 7465 6e65  meseriesflattene
+00000d60: 722e 7376 6729 5d28 6874 7470 733a 2f2f  r.svg)](https://
+00000d70: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+00000d80: 2f74 696d 6573 6572 6965 7366 6c61 7474  /timeseriesflatt
+00000d90: 656e 6572 2f29 0a5b 215b 7374 6174 7573  ener/).[![status
+00000da0: 5d28 6874 7470 733a 2f2f 6a6f 7373 2e74  ](https://joss.t
+00000db0: 6865 6f6a 2e6f 7267 2f70 6170 6572 732f  heoj.org/papers/
+00000dc0: 3362 6265 6138 3734 3536 3638 6431 6161  3bbea8745668d1aa
+00000dd0: 3430 6666 3739 3663 3666 6433 6462 3837  40ff796c6fd3db87
+00000de0: 2f73 7461 7475 732e 7376 6729 5d28 6874  /status.svg)](ht
+00000df0: 7470 733a 2f2f 6a6f 7373 2e74 6865 6f6a  tps://joss.theoj
+00000e00: 2e6f 7267 2f70 6170 6572 732f 3362 6265  .org/papers/3bbe
+00000e10: 6138 3734 3536 3638 6431 6161 3430 6666  a8745668d1aa40ff
+00000e20: 3739 3663 3666 6433 6462 3837 290a 0a54  796c6fd3db87)..T
+00000e30: 696d 6520 7365 7269 6573 2066 726f 6d20  ime series from 
+00000e40: 652e 672e 2065 6c65 6374 726f 6e69 6320  e.g. electronic 
+00000e50: 6865 616c 7468 2072 6563 6f72 6473 206f  health records o
+00000e60: 6674 656e 2068 6176 6520 6120 6c61 7267  ften have a larg
+00000e70: 6520 6e75 6d62 6572 206f 6620 7661 7269  e number of vari
+00000e80: 6162 6c65 732c 2061 7265 2073 616d 706c  ables, are sampl
+00000e90: 6564 2061 7420 6972 7265 6775 6c61 7220  ed at irregular 
+00000ea0: 696e 7465 7276 616c 7320 616e 6420 7465  intervals and te
+00000eb0: 6e64 2074 6f20 6861 7665 2061 206c 6172  nd to have a lar
+00000ec0: 6765 206e 756d 6265 7220 6f66 206d 6973  ge number of mis
+00000ed0: 7369 6e67 2076 616c 7565 732e 2042 6566  sing values. Bef
+00000ee0: 6f72 6520 7468 6973 2074 7970 6520 6f66  ore this type of
+00000ef0: 2064 6174 6120 6361 6e20 6265 2075 7365   data can be use
+00000f00: 6420 666f 7220 7072 6564 6963 7469 6f6e  d for prediction
+00000f10: 206d 6f64 656c 6c69 6e67 2077 6974 6820   modelling with 
+00000f20: 6d61 6368 696e 6520 6c65 6172 6e69 6e67  machine learning
+00000f30: 206d 6574 686f 6473 2073 7563 6820 6173   methods such as
+00000f40: 206c 6f67 6973 7469 6320 7265 6772 6573   logistic regres
+00000f50: 7369 6f6e 206f 7220 5847 426f 6f73 742c  sion or XGBoost,
+00000f60: 2074 6865 2064 6174 6120 6e65 6564 7320   the data needs 
+00000f70: 746f 2062 6520 7265 7368 6170 6564 2e20  to be reshaped. 
+00000f80: 0a0a 496e 2065 7373 656e 6365 2c20 7468  ..In essence, th
+00000f90: 6520 7469 6d65 2073 6572 6965 7320 6e65  e time series ne
+00000fa0: 6564 2074 6f20 6265 202a 666c 6174 7465  ed to be *flatte
+00000fb0: 6e65 642a 2073 6f20 7468 6174 2065 6163  ned* so that eac
+00000fc0: 6820 7072 6564 6963 7469 6f6e 2074 696d  h prediction tim
+00000fd0: 6520 6973 2072 6570 7265 7365 6e74 6564  e is represented
+00000fe0: 2062 7920 6120 7365 7420 6f66 2070 7265   by a set of pre
+00000ff0: 6469 6374 6f72 2076 616c 7565 7320 616e  dictor values an
+00001000: 6420 616e 206f 7574 636f 6d65 2076 616c  d an outcome val
+00001010: 7565 2e20 5468 6573 6520 7072 6564 6963  ue. These predic
+00001020: 746f 7220 7661 6c75 6573 2063 616e 2062  tor values can b
+00001030: 6520 636f 6e73 7472 7563 7465 6420 6279  e constructed by
+00001040: 2061 6767 7265 6761 7469 6e67 2074 6865   aggregating the
+00001050: 2070 7265 6365 6469 6e67 2076 616c 7565   preceding value
+00001060: 7320 696e 2074 6865 2074 696d 6520 7365  s in the time se
+00001070: 7269 6573 2077 6974 6869 6e20 6120 6365  ries within a ce
+00001080: 7274 6169 6e20 7469 6d65 2077 696e 646f  rtain time windo
+00001090: 772e 200a 0a60 7469 6d65 7365 7269 6573  w. ..`timeseries
+000010a0: 666c 6174 7465 6e65 7260 2061 696d 7320  flattener` aims 
+000010b0: 746f 2073 696d 706c 6966 7920 7468 6973  to simplify this
+000010c0: 2070 726f 6365 7373 2062 7920 7072 6f76   process by prov
+000010d0: 6964 696e 6720 616e 2065 6173 792d 746f  iding an easy-to
+000010e0: 2d75 7365 2061 6e64 2066 756c 6c79 2d73  -use and fully-s
+000010f0: 7065 6369 6669 6564 2070 6970 656c 696e  pecified pipelin
+00001100: 6520 666f 7220 666c 6174 7465 6e69 6e67  e for flattening
+00001110: 2063 6f6d 706c 6578 2074 696d 6520 7365   complex time se
+00001120: 7269 6573 2e20 0a0a 2323 20f0 9f94 a720  ries. ..## .... 
+00001130: 496e 7374 616c 6c61 7469 6f6e 0a54 6f20  Installation.To 
+00001140: 6765 7420 7374 6172 7465 6420 7573 696e  get started usin
+00001150: 6720 7469 6d65 7365 7269 6573 666c 6174  g timeseriesflat
+00001160: 7465 6e65 7220 7369 6d70 6c79 2069 6e73  tener simply ins
+00001170: 7461 6c6c 2069 7420 7573 696e 6720 7069  tall it using pi
+00001180: 7020 6279 2072 756e 6e69 6e67 2074 6865  p by running the
+00001190: 2066 6f6c 6c6f 7769 6e67 206c 696e 6520   following line 
+000011a0: 696e 2079 6f75 7220 7465 726d 696e 616c  in your terminal
+000011b0: 3a0a 0a60 6060 0a70 6970 2069 6e73 7461  :..```.pip insta
+000011c0: 6c6c 2074 696d 6573 6572 6965 7366 6c61  ll timeseriesfla
+000011d0: 7474 656e 6572 0a60 6060 0a0a 2323 20e2  ttener.```..## .
+000011e0: 9aa1 2051 7569 636b 2073 7461 7274 0a0a  .. Quick start..
+000011f0: 6060 6070 790a 696d 706f 7274 206e 756d  ```py.import num
+00001200: 7079 2061 7320 6e70 0a69 6d70 6f72 7420  py as np.import 
+00001210: 7061 6e64 6173 2061 7320 7064 0a0a 6966  pandas as pd..if
+00001220: 205f 5f6e 616d 655f 5f20 3d3d 2022 5f5f   __name__ == "__
+00001230: 6d61 696e 5f5f 223a 0a0a 2020 2020 2320  main__":..    # 
+00001240: 4c6f 6164 2061 2064 6174 6166 7261 6d65  Load a dataframe
+00001250: 2077 6974 6820 7469 6d65 7320 796f 7520   with times you 
+00001260: 7769 7368 2074 6f20 6d61 6b65 2061 2070  wish to make a p
+00001270: 7265 6469 6374 696f 6e0a 2020 2020 7072  rediction.    pr
+00001280: 6564 6963 7469 6f6e 5f74 696d 6573 5f64  ediction_times_d
+00001290: 6620 3d20 7064 2e44 6174 6146 7261 6d65  f = pd.DataFrame
+000012a0: 280a 2020 2020 2020 2020 7b0a 2020 2020  (.        {.    
+000012b0: 2020 2020 2020 2020 2269 6422 3a20 5b31          "id": [1
+000012c0: 2c20 312c 2032 5d2c 0a20 2020 2020 2020  , 1, 2],.       
+000012d0: 2020 2020 2022 6461 7465 223a 205b 2232       "date": ["2
+000012e0: 3032 302d 3031 2d30 3122 2c20 2232 3032  020-01-01", "202
+000012f0: 302d 3032 2d30 3122 2c20 2232 3032 302d  0-02-01", "2020-
+00001300: 3032 2d30 3122 5d2c 0a20 2020 2020 2020  02-01"],.       
+00001310: 207d 2c0a 2020 2020 290a 2020 2020 2320   },.    ).    # 
+00001320: 4c6f 6164 2061 2064 6174 6166 7261 6d65  Load a dataframe
+00001330: 2077 6974 6820 7261 7720 7661 6c75 6573   with raw values
+00001340: 2079 6f75 2077 6973 6820 746f 2061 6767   you wish to agg
+00001350: 7265 6761 7465 2061 7320 7072 6564 6963  regate as predic
+00001360: 746f 7273 0a20 2020 2070 7265 6469 6374  tors.    predict
+00001370: 6f72 5f64 6620 3d20 7064 2e44 6174 6146  or_df = pd.DataF
+00001380: 7261 6d65 280a 2020 2020 2020 2020 7b0a  rame(.        {.
+00001390: 2020 2020 2020 2020 2020 2020 2269 6422              "id"
+000013a0: 3a20 5b31 2c20 312c 2031 2c20 325d 2c0a  : [1, 1, 1, 2],.
+000013b0: 2020 2020 2020 2020 2020 2020 2264 6174              "dat
+000013c0: 6522 3a20 5b0a 2020 2020 2020 2020 2020  e": [.          
+000013d0: 2020 2020 2020 2232 3032 302d 3031 2d31        "2020-01-1
+000013e0: 3522 2c0a 2020 2020 2020 2020 2020 2020  5",.            
+000013f0: 2020 2020 2232 3031 392d 3132 2d31 3022      "2019-12-10"
+00001400: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001410: 2020 2232 3031 392d 3132 2d31 3522 2c0a    "2019-12-15",.
+00001420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001430: 2232 3032 302d 3031 2d30 3222 2c0a 2020  "2020-01-02",.  
+00001440: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
+00001450: 2020 2020 2020 2020 2022 7661 6c75 6522           "value"
+00001460: 3a20 5b31 2c20 322c 2033 2c20 345d 2c0a  : [1, 2, 3, 4],.
+00001470: 2020 2020 2020 2020 7d2c 0a20 2020 2029          },.    )
+00001480: 0a20 2020 2023 204c 6f61 6420 6120 6461  .    # Load a da
+00001490: 7461 6672 616d 6520 7370 6563 6966 7969  taframe specifyi
+000014a0: 6e67 2077 6865 6e20 7468 6520 6f75 7463  ng when the outc
+000014b0: 6f6d 6520 6f63 6375 7273 0a20 2020 206f  ome occurs.    o
+000014c0: 7574 636f 6d65 5f64 6620 3d20 7064 2e44  utcome_df = pd.D
+000014d0: 6174 6146 7261 6d65 287b 2269 6422 3a20  ataFrame({"id": 
+000014e0: 5b31 5d2c 2022 6461 7465 223a 205b 2232  [1], "date": ["2
+000014f0: 3032 302d 3033 2d30 3122 5d2c 2022 7661  020-03-01"], "va
+00001500: 6c75 6522 3a20 5b31 5d7d 290a 0a20 2020  lue": [1]})..   
+00001510: 2023 2053 7065 6369 6679 2068 6f77 2074   # Specify how t
+00001520: 6f20 6167 6772 6567 6174 6520 7468 6520  o aggregate the 
+00001530: 7072 6564 6963 746f 7273 2061 6e64 2064  predictors and d
+00001540: 6566 696e 6520 7468 6520 6f75 7463 6f6d  efine the outcom
+00001550: 650a 2020 2020 6672 6f6d 2074 696d 6573  e.    from times
+00001560: 6572 6965 7366 6c61 7474 656e 6572 2e66  eriesflattener.f
+00001570: 6561 7475 7265 5f73 7065 635f 6f62 6a65  eature_spec_obje
+00001580: 6374 7320 696d 706f 7274 204f 7574 636f  cts import Outco
+00001590: 6d65 5370 6563 2c20 5072 6564 6963 746f  meSpec, Predicto
+000015a0: 7253 7065 630a 2020 2020 6672 6f6d 2074  rSpec.    from t
+000015b0: 696d 6573 6572 6965 7366 6c61 7474 656e  imeseriesflatten
+000015c0: 6572 2e72 6573 6f6c 7665 5f6d 756c 7469  er.resolve_multi
+000015d0: 706c 655f 6675 6e63 7469 6f6e 7320 696d  ple_functions im
+000015e0: 706f 7274 206d 6178 696d 756d 2c20 6d65  port maximum, me
+000015f0: 616e 0a0a 2020 2020 7072 6564 6963 746f  an..    predicto
+00001600: 725f 7370 6563 203d 2050 7265 6469 6374  r_spec = Predict
+00001610: 6f72 5370 6563 280a 2020 2020 2020 2020  orSpec(.        
+00001620: 7661 6c75 6573 5f64 663d 7072 6564 6963  values_df=predic
+00001630: 746f 725f 6466 2c0a 2020 2020 2020 2020  tor_df,.        
+00001640: 6c6f 6f6b 6265 6869 6e64 5f64 6179 733d  lookbehind_days=
+00001650: 3330 2c0a 2020 2020 2020 2020 6661 6c6c  30,.        fall
+00001660: 6261 636b 3d6e 702e 6e61 6e2c 0a20 2020  back=np.nan,.   
+00001670: 2020 2020 2065 6e74 6974 795f 6964 5f63       entity_id_c
+00001680: 6f6c 5f6e 616d 653d 2269 6422 2c0a 2020  ol_name="id",.  
+00001690: 2020 2020 2020 7265 736f 6c76 655f 6d75        resolve_mu
+000016a0: 6c74 6970 6c65 5f66 6e3d 6d65 616e 2c0a  ltiple_fn=mean,.
+000016b0: 2020 2020 2020 2020 6665 6174 7572 655f          feature_
+000016c0: 6e61 6d65 3d22 7465 7374 5f66 6561 7475  name="test_featu
+000016d0: 7265 222c 0a20 2020 2029 0a20 2020 206f  re",.    ).    o
+000016e0: 7574 636f 6d65 5f73 7065 6320 3d20 4f75  utcome_spec = Ou
+000016f0: 7463 6f6d 6553 7065 6328 0a20 2020 2020  tcomeSpec(.     
+00001700: 2020 2076 616c 7565 735f 6466 3d6f 7574     values_df=out
+00001710: 636f 6d65 5f64 662c 0a20 2020 2020 2020  come_df,.       
+00001720: 206c 6f6f 6b61 6865 6164 5f64 6179 733d   lookahead_days=
+00001730: 3331 2c0a 2020 2020 2020 2020 6661 6c6c  31,.        fall
+00001740: 6261 636b 3d30 2c0a 2020 2020 2020 2020  back=0,.        
+00001750: 656e 7469 7479 5f69 645f 636f 6c5f 6e61  entity_id_col_na
+00001760: 6d65 3d22 6964 222c 0a20 2020 2020 2020  me="id",.       
+00001770: 2072 6573 6f6c 7665 5f6d 756c 7469 706c   resolve_multipl
+00001780: 655f 666e 3d6d 6178 696d 756d 2c0a 2020  e_fn=maximum,.  
+00001790: 2020 2020 2020 6665 6174 7572 655f 6e61        feature_na
+000017a0: 6d65 3d22 7465 7374 5f6f 7574 636f 6d65  me="test_outcome
+000017b0: 222c 0a20 2020 2020 2020 2069 6e63 6964  ",.        incid
+000017c0: 656e 743d 4661 6c73 652c 0a20 2020 2029  ent=False,.    )
+000017d0: 0a0a 2020 2020 2320 496e 7374 616e 7469  ..    # Instanti
+000017e0: 6174 6520 5469 6d65 7365 7269 6573 466c  ate TimeseriesFl
+000017f0: 6174 7465 6e65 7220 616e 6420 6164 6420  attener and add 
+00001800: 7468 6520 7370 6563 6966 6963 6174 696f  the specificatio
+00001810: 6e73 0a20 2020 2066 726f 6d20 7469 6d65  ns.    from time
+00001820: 7365 7269 6573 666c 6174 7465 6e65 7220  seriesflattener 
+00001830: 696d 706f 7274 2054 696d 6573 6572 6965  import Timeserie
+00001840: 7346 6c61 7474 656e 6572 0a0a 2020 2020  sFlattener..    
+00001850: 7473 5f66 6c61 7474 656e 6572 203d 2054  ts_flattener = T
+00001860: 696d 6573 6572 6965 7346 6c61 7474 656e  imeseriesFlatten
+00001870: 6572 280a 2020 2020 2020 2020 7072 6564  er(.        pred
+00001880: 6963 7469 6f6e 5f74 696d 6573 5f64 663d  iction_times_df=
+00001890: 7072 6564 6963 7469 6f6e 5f74 696d 6573  prediction_times
+000018a0: 5f64 662c 0a20 2020 2020 2020 2065 6e74  _df,.        ent
+000018b0: 6974 795f 6964 5f63 6f6c 5f6e 616d 653d  ity_id_col_name=
+000018c0: 2269 6422 2c0a 2020 2020 2020 2020 7469  "id",.        ti
+000018d0: 6d65 7374 616d 705f 636f 6c5f 6e61 6d65  mestamp_col_name
+000018e0: 3d22 6461 7465 222c 0a20 2020 2020 2020  ="date",.       
+000018f0: 206e 5f77 6f72 6b65 7273 3d31 2c0a 2020   n_workers=1,.  
+00001900: 2020 2020 2020 6472 6f70 5f70 7265 645f        drop_pred_
+00001910: 7469 6d65 735f 7769 7468 5f69 6e73 7566  times_with_insuf
+00001920: 6669 6369 656e 745f 6c6f 6f6b 5f64 6973  ficient_look_dis
+00001930: 7461 6e63 653d 4661 6c73 652c 0a20 2020  tance=False,.   
+00001940: 2029 0a20 2020 2074 735f 666c 6174 7465   ).    ts_flatte
+00001950: 6e65 722e 6164 645f 7370 6563 285b 7072  ner.add_spec([pr
+00001960: 6564 6963 746f 725f 7370 6563 2c20 6f75  edictor_spec, ou
+00001970: 7463 6f6d 655f 7370 6563 5d29 0a20 2020  tcome_spec]).   
+00001980: 2064 6620 3d20 7473 5f66 6c61 7474 656e   df = ts_flatten
+00001990: 6572 2e67 6574 5f64 6628 290a 2020 2020  er.get_df().    
+000019a0: 6466 0a60 6060 0a4f 7574 7075 743a 0a0a  df.```.Output:..
+000019b0: 7c20 2020 2020 207c 2020 2069 6420 7c20  |      |   id | 
+000019c0: 6461 7465 2020 2020 2020 2020 2020 2020  date            
+000019d0: 2020 2020 7c20 7072 6564 6963 7469 6f6e      | prediction
+000019e0: 5f74 696d 655f 7575 6964 2020 7c20 7072  _time_uuid  | pr
+000019f0: 6564 5f74 6573 745f 6665 6174 7572 655f  ed_test_feature_
+00001a00: 7769 7468 696e 5f33 305f 6461 7973 5f6d  within_30_days_m
+00001a10: 6561 6e5f 6661 6c6c 6261 636b 5f6e 616e  ean_fallback_nan
+00001a20: 207c 206f 7574 635f 7465 7374 5f6f 7574   | outc_test_out
+00001a30: 636f 6d65 5f77 6974 6869 6e5f 3331 5f64  come_within_31_d
+00001a40: 6179 735f 6d61 7869 6d75 6d5f 6661 6c6c  ays_maximum_fall
+00001a50: 6261 636b 5f30 5f64 6963 686f 746f 6d6f  back_0_dichotomo
+00001a60: 7573 207c 0a7c 202d 2d2d 3a20 7c20 2d2d  us |.| ---: | --
+00001a70: 2d3a 207c 203a 2d2d 2d2d 2d2d 2d2d 2d2d  -: | :----------
+00001a80: 2d2d 2d2d 2d2d 2d2d 207c 203a 2d2d 2d2d  -------- | :----
+00001a90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001aa0: 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   | -------------
+00001ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001ac0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001ad0: 2d2d 2d2d 3a20 7c20 2d2d 2d2d 2d2d 2d2d  ----: | --------
+00001ae0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001af0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001b00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001b10: 2d2d 2d2d 2d2d 3a20 7c0a 7c20 2020 2030  ------: |.|    0
+00001b20: 207c 2020 2020 3120 7c20 3230 3230 2d30   |    1 | 2020-0
+00001b30: 312d 3031 2030 303a 3030 3a30 3020 7c20  1-01 00:00:00 | 
+00001b40: 312d 3230 3230 2d30 312d 3031 2d30 302d  1-2020-01-01-00-
+00001b50: 3030 2d30 3020 7c20 2020 2020 2020 2020  00-00 |         
+00001b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b80: 2020 2020 2020 2032 2e35 207c 2020 2020         2.5 |    
+00001b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bb0: 207c 0a7c 202d 2d2d 2d2d 2d2d 2d2d 2d2d   |.| -----------
-00001bc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001bd0: 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d2d  --- | ----------
-00001be0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c 0a7c  ------------ |.|
-00001bf0: 20f0 9f9a a820 2a2a 4275 6720 5265 706f   .... **Bug Repo
-00001c00: 7274 732a 2a20 2020 2020 2020 2020 2020  rts**           
-00001c10: 2020 207c 205b 4769 7448 7562 2049 7373     | [GitHub Iss
-00001c20: 7565 2054 7261 636b 6572 5d20 7c0a 7c20  ue Tracker] |.| 
-00001c30: f09f 8e81 202a 2a46 6561 7475 7265 2052  .... **Feature R
-00001c40: 6571 7565 7374 7320 2620 4964 6561 732a  equests & Ideas*
-00001c50: 2a20 7c20 5b47 6974 4875 6220 4973 7375  * | [GitHub Issu
-00001c60: 6520 5472 6163 6b65 725d 207c 0a7c 20f0  e Tracker] |.| .
-00001c70: 9f91 a9e2 808d f09f 92bb 202a 2a55 7361  .......... **Usa
-00001c80: 6765 2051 7565 7374 696f 6e73 2a2a 2020  ge Questions**  
-00001c90: 2020 2020 2020 2020 7c20 5b47 6974 4875          | [GitHu
-00001ca0: 6220 4469 7363 7573 7369 6f6e 735d 2020  b Discussions]  
-00001cb0: 207c 0a7c 20f0 9f97 af20 2a2a 4765 6e65   |.| .... **Gene
-00001cc0: 7261 6c20 4469 7363 7573 7369 6f6e 2a2a  ral Discussion**
-00001cd0: 2020 2020 2020 207c 205b 4769 7448 7562         | [GitHub
-00001ce0: 2044 6973 6375 7373 696f 6e73 5d20 2020   Discussions]   
-00001cf0: 7c0a 0a5b 6769 7468 7562 2069 7373 7565  |..[github issue
-00001d00: 2074 7261 636b 6572 5d3a 2068 7474 7073   tracker]: https
-00001d10: 3a2f 2f67 6974 6875 622e 636f 6d2f 4161  ://github.com/Aa
-00001d20: 7268 7573 2d50 7379 6368 6961 7472 792d  rhus-Psychiatry-
-00001d30: 5265 7365 6172 6368 2f74 696d 6573 6572  Research/timeser
-00001d40: 6965 7366 6c61 7474 656e 6572 2f69 7373  iesflattener/iss
-00001d50: 7565 730a 5b67 6974 6875 6220 6469 7363  ues.[github disc
-00001d60: 7573 7369 6f6e 735d 3a20 6874 7470 733a  ussions]: https:
-00001d70: 2f2f 6769 7468 7562 2e63 6f6d 2f41 6172  //github.com/Aar
-00001d80: 6875 732d 5073 7963 6869 6174 7279 2d52  hus-Psychiatry-R
-00001d90: 6573 6561 7263 682f 7469 6d65 7365 7269  esearch/timeseri
-00001da0: 6573 666c 6174 7465 6e65 722f 6469 7363  esflattener/disc
-00001db0: 7573 7369 6f6e 730a 0a0a 2323 20f0 9f8e  ussions...## ...
-00001dc0: 9320 5072 6f6a 6563 7473 0a50 5359 434f  . Projects.PSYCO
-00001dd0: 5020 7072 6f6a 6563 7473 2077 6869 6368  P projects which
-00001de0: 2075 7365 2060 7469 6d65 7365 7269 6573   use `timeseries
-00001df0: 666c 6174 7465 6e65 7260 2e20 4e6f 7465  flattener`. Note
-00001e00: 2074 6861 7420 736f 6d65 206f 6620 7468   that some of th
-00001e10: 6573 6520 7072 6f6a 6563 7473 2068 6176  ese projects hav
-00001e20: 6520 7965 7420 746f 2062 6520 7075 626c  e yet to be publ
-00001e30: 6973 6865 6420 616e 6420 6172 6520 7468  ished and are th
-00001e40: 7573 2070 7269 7661 7465 2e0a 0a7c 2050  us private...| P
-00001e50: 726f 6a65 6374 2020 2020 2020 2020 2020  roject          
-00001e60: 2020 2020 2020 207c 2050 7562 6c69 6361         | Publica
-00001e70: 7469 6f6e 7320 7c20 2020 2020 2020 2020  tions |         
-00001e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001bc0: 2020 2020 2020 2020 2020 2030 207c 0a7c             0 |.|
+00001bd0: 2020 2020 3120 7c20 2020 2031 207c 2032      1 |    1 | 2
+00001be0: 3032 302d 3032 2d30 3120 3030 3a30 303a  020-02-01 00:00:
+00001bf0: 3030 207c 2031 2d32 3032 302d 3032 2d30  00 | 1-2020-02-0
+00001c00: 312d 3030 2d30 302d 3030 207c 2020 2020  1-00-00-00 |    
+00001c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c30: 2020 2020 2020 2020 2020 2020 2020 3120                1 
+00001c40: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+00001c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c80: 3120 7c0a 7c20 2020 2032 207c 2020 2020  1 |.|    2 |    
+00001c90: 3220 7c20 3230 3230 2d30 322d 3031 2030  2 | 2020-02-01 0
+00001ca0: 303a 3030 3a30 3020 7c20 322d 3230 3230  0:00:00 | 2-2020
+00001cb0: 2d30 322d 3031 2d30 302d 3030 2d30 3020  -02-01-00-00-00 
+00001cc0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+00001cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cf0: 2020 2034 207c 2020 2020 2020 2020 2020     4 |          
+00001d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d30: 2020 2020 2030 207c 0a0a 0a23 2320 f09f       0 |...## ..
+00001d40: 9396 2044 6f63 756d 656e 7461 7469 6f6e  .. Documentation
+00001d50: 0a0a 7c20 446f 6375 6d65 6e74 6174 696f  ..| Documentatio
+00001d60: 6e20 2020 2020 2020 2020 207c 2020 2020  n          |    
+00001d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001dc0: 2020 2020 7c0a 7c20 2d2d 2d2d 2d2d 2d2d      |.| --------
+00001dd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c  -------------- |
+00001de0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+00001df0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001e00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001e10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001e20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001e30: 2d2d 2d2d 2d2d 2d20 7c0a 7c20 f09f 8e93  ------- |.| ....
+00001e40: 202a 2a5b 5475 746f 7269 616c 5d2a 2a20   **[Tutorial]** 
+00001e50: 2020 2020 2020 7c20 5369 6d70 6c65 2061        | Simple a
+00001e60: 6e64 2061 6476 616e 6365 6420 7475 746f  nd advanced tuto
+00001e70: 7269 616c 7320 746f 2067 6574 2079 6f75  rials to get you
+00001e80: 2073 7461 7274 6564 2075 7369 6e67 2060   started using `
+00001e90: 7469 6d65 7365 7269 6573 666c 6174 7465  timeseriesflatte
+00001ea0: 6e65 7260 2020 2020 2020 2020 2020 207c  ner`           |
+00001eb0: 0a7c 20f0 9f8e 9b20 2a2a 5b47 656e 6572  .| .... **[Gener
+00001ec0: 616c 2064 6f63 735d 2a2a 207c 2054 6865  al docs]** | The
+00001ed0: 2064 6574 6169 6c65 6420 7265 6665 7265   detailed refere
+00001ee0: 6e63 6520 666f 7220 7469 6d65 7365 7269  nce for timeseri
+00001ef0: 6573 666c 6174 7465 6e65 7227 7320 4150  esflattener's AP
+00001f00: 492e 207c 0a7c 20f0 9f99 8b20 2a2a 5b46  I. |.| .... **[F
+00001f10: 4151 5d2a 2a20 2020 2020 2020 2020 2020  AQ]**           
+00001f20: 207c 2046 7265 7175 656e 746c 7920 6173   | Frequently as
+00001f30: 6b65 6420 7175 6573 7469 6f6e 2020 2020  ked question    
 00001f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f50: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00001f60: 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  | --------------
-00001f70: 2d2d 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d  --------- | ----
-00001f80: 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d  -------- | -----
-00001f90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001fa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001fb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001fc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001fd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001fe0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001ff0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002000: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002020: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002030: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002040: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002050: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002060: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002070: 207c 0a7c 202a 2a5b 5479 7065 2032 2044   |.| **[Type 2 D
-00002080: 6961 6265 7465 735d 2a2a 2020 207c 2020  iabetes]**   |  
-00002090: 2020 2020 2020 2020 2020 2020 7c20 5072              | Pr
-000020a0: 6564 6963 7469 6f6e 206f 6620 7479 7065  ediction of type
-000020b0: 2032 2064 6961 6265 7465 7320 616d 6f6e   2 diabetes amon
-000020c0: 6720 7061 7469 656e 7473 2077 6974 6820  g patients with 
-000020d0: 7669 7369 7473 2074 6f20 7073 7963 6869  visits to psychi
-000020e0: 6174 7269 6320 686f 7370 6974 616c 2064  atric hospital d
-000020f0: 6570 6172 746d 656e 7473 2020 2020 2020  epartments      
-00002100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f70: 2020 2020 2020 2020 2020 7c0a 7c20 f09f            |.| ..
+00001f80: 97ba efb8 8f20 2a2a 5b52 6f61 646d 6170  ..... **[Roadmap
+00001f90: 5d2a 2a20 2020 2020 2020 207c 204b 616e  ]**        | Kan
+00001fa0: 6261 6e20 626f 6172 6420 666f 7220 7468  ban board for th
+00001fb0: 6520 726f 6164 6d61 7020 666f 7220 7468  e roadmap for th
+00001fc0: 6520 7072 6f6a 6563 7420 2020 2020 2020  e project       
+00001fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ff0: 2020 2020 7c0a 0a5b 5475 746f 7269 616c      |..[Tutorial
+00002000: 5d3a 2068 7474 7073 3a2f 2f61 6172 6875  ]: https://aarhu
+00002010: 732d 7073 7963 6869 6174 7279 2d72 6573  s-psychiatry-res
+00002020: 6561 7263 682e 6769 7468 7562 2e69 6f2f  earch.github.io/
+00002030: 7469 6d65 7365 7269 6573 666c 6174 7465  timeseriesflatte
+00002040: 6e65 722f 7475 746f 7269 616c 732e 6874  ner/tutorials.ht
+00002050: 6d6c 0a5b 4765 6e65 7261 6c20 646f 6373  ml.[General docs
+00002060: 5d3a 2068 7474 7073 3a2f 2f41 6172 6875  ]: https://Aarhu
+00002070: 732d 5073 7963 6869 6174 7279 2d52 6573  s-Psychiatry-Res
+00002080: 6561 7263 682e 6769 7468 7562 2e69 6f2f  earch.github.io/
+00002090: 7469 6d65 7365 7269 6573 666c 6174 7465  timeseriesflatte
+000020a0: 6e65 722f 0a5b 4641 515d 3a20 6874 7470  ner/.[FAQ]: http
+000020b0: 733a 2f2f 4161 7268 7573 2d50 7379 6368  s://Aarhus-Psych
+000020c0: 6961 7472 792d 5265 7365 6172 6368 2e67  iatry-Research.g
+000020d0: 6974 6875 622e 696f 2f74 696d 6573 6572  ithub.io/timeser
+000020e0: 6965 7366 6c61 7474 656e 6572 2f66 6171  iesflattener/faq
+000020f0: 2e68 746d 6c0a 5b52 6f61 646d 6170 5d3a  .html.[Roadmap]:
+00002100: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00002110: 636f 6d2f 6f72 6773 2f41 6172 6875 732d  com/orgs/Aarhus-
+00002120: 5073 7963 6869 6174 7279 2d52 6573 6561  Psychiatry-Resea
+00002130: 7263 682f 7072 6f6a 6563 7473 2f31 312f  rch/projects/11/
+00002140: 7669 6577 732f 310a 0a23 2320 f09f 92ac  views/1..## ....
+00002150: 2057 6865 7265 2074 6f20 6173 6b20 7175   Where to ask qu
+00002160: 6573 7469 6f6e 730a 0a7c 2054 7970 6520  estions..| Type 
 00002170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002180: 2020 2020 7c0a 7c20 2a2a 5b43 616e 6365      |.| **[Cance
-00002190: 725d 2a2a 2020 2020 2020 2020 2020 2020  r]**            
-000021a0: 7c20 2020 2020 2020 2020 2020 2020 207c  |              |
-000021b0: 2050 7265 6469 6374 696f 6e20 6f66 2043   Prediction of C
-000021c0: 616e 6365 7220 616d 6f6e 6720 7061 7469  ancer among pati
-000021d0: 656e 7473 2077 6974 6820 7669 7369 7473  ents with visits
-000021e0: 2074 6f20 7073 7963 6869 6174 7269 6320   to psychiatric 
-000021f0: 686f 7370 6974 616c 2064 6570 6172 746d  hospital departm
-00002200: 656e 7473 2020 2020 2020 2020 2020 2020  ents            
-00002210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002290: 2020 2020 2020 207c 0a7c 202a 2a5b 434f         |.| **[CO
-000022a0: 5044 5d2a 2a20 2020 2020 2020 2020 2020  PD]**           
-000022b0: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-000022c0: 2020 7c20 5072 6564 6963 7469 6f6e 206f    | Prediction o
-000022d0: 6620 4368 726f 6e69 6320 6f62 7374 7275  f Chronic obstru
-000022e0: 6374 6976 6520 7075 6c6d 6f6e 6172 7920  ctive pulmonary 
-000022f0: 6469 7365 6173 6520 2843 4f50 4429 2061  disease (COPD) a
-00002300: 6d6f 6e67 2070 6174 6965 6e74 7320 7769  mong patients wi
-00002310: 7468 2076 6973 6974 7320 746f 2070 7379  th visits to psy
-00002320: 6368 6961 7472 6963 2068 6f73 7069 7461  chiatric hospita
-00002330: 6c20 6465 7061 7274 6d65 6e74 7320 2020  l departments   
-00002340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023a0: 2020 2020 2020 2020 2020 7c0a 7c20 2a2a            |.| **
-000023b0: 5b46 6f72 6365 6420 6164 6d69 7373 696f  [Forced admissio
-000023c0: 6e73 5d2a 2a20 7c20 2020 2020 2020 2020  ns]** |         
-000023d0: 2020 2020 207c 2050 7265 6469 6374 696f       | Predictio
-000023e0: 6e20 6f66 2066 6f72 6365 6420 6164 6d69  n of forced admi
-000023f0: 7373 696f 6e73 206f 6620 7061 7469 656e  ssions of patien
-00002400: 7473 2074 6f20 7468 6520 7073 7963 6869  ts to the psychi
-00002410: 6174 7269 6320 686f 7370 6974 616c 2064  atric hospital d
-00002420: 6570 6172 746d 656e 7473 2e20 456e 636f  epartments. Enco
-00002430: 6d70 6173 7365 7320 7477 6f20 7365 7061  mpasses two sepa
-00002440: 7261 7465 2070 726f 6a65 6374 733a 2031  rate projects: 1
-00002450: 2e20 5072 6564 6963 6974 696e 6720 6174  . Prediciting at
-00002460: 2074 696d 6520 6f66 2064 6973 6368 6172   time of dischar
-00002470: 6765 2066 6f72 2069 6e70 6174 6965 6e74  ge for inpatient
-00002480: 2061 646d 6973 7369 6f6e 732e 2032 2e20   admissions. 2. 
-00002490: 5072 6564 6963 7469 6e67 2064 6179 2062  Predicting day b
-000024a0: 6566 6f72 6520 6f75 7470 6174 6965 6e74  efore outpatient
-000024b0: 2061 646d 6973 7369 6f6e 732e 207c 0a7c   admissions. |.|
-000024c0: 202a 2a5b 436f 6572 6369 6f6e 5d2a 2a20   **[Coercion]** 
-000024d0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-000024e0: 2020 2020 2020 2020 7c20 5072 6564 6963          | Predic
-000024f0: 7469 6f6e 206f 6620 636f 6572 6369 6f6e  tion of coercion
-00002500: 2061 6d6f 6e67 2070 6174 6965 6e74 7320   among patients 
-00002510: 6164 6d69 7474 6965 6420 746f 2074 6865  admittied to the
-00002520: 2068 6f73 7069 7461 6c20 7073 7963 6869   hospital psychi
-00002530: 6174 7269 6320 6465 7061 7274 6d65 6e74  atric department
-00002540: 2e20 456e 636f 6d70 6173 7365 7320 7072  . Encompasses pr
-00002550: 6564 6963 7469 6e67 206d 6563 6861 6e69  edicting mechani
-00002560: 6361 6c20 7265 7374 7261 696e 742c 2073  cal restraint, s
-00002570: 6564 6174 6976 6520 6d65 6469 6361 7469  edative medicati
-00002580: 6f6e 2061 6e64 206d 616e 7561 6c20 7265  on and manual re
-00002590: 7374 7261 696e 7420 3438 2068 6f75 7273  straint 48 hours
-000025a0: 2062 6566 6f72 6520 636f 6572 6369 6f6e   before coercion
-000025b0: 206f 6363 7572 732e 2020 2020 2020 2020   occurs.        
-000025c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025d0: 7c0a 0a0a 5b54 7970 6520 3220 6469 6162  |...[Type 2 diab
-000025e0: 6574 6573 5d3a 2068 7474 7073 3a2f 2f67  etes]: https://g
-000025f0: 6974 6875 622e 636f 6d2f 4161 7268 7573  ithub.com/Aarhus
-00002600: 2d50 7379 6368 6961 7472 792d 5265 7365  -Psychiatry-Rese
-00002610: 6172 6368 2f70 7379 636f 702d 7432 640a  arch/psycop-t2d.
-00002620: 5b43 616e 6365 725d 3a20 6874 7470 733a  [Cancer]: https:
-00002630: 2f2f 6769 7468 7562 2e63 6f6d 2f41 6172  //github.com/Aar
-00002640: 6875 732d 5073 7963 6869 6174 7279 2d52  hus-Psychiatry-R
-00002650: 6573 6561 7263 682f 7073 7963 6f70 2d63  esearch/psycop-c
-00002660: 616e 6365 720a 5b43 4f50 445d 3a20 6874  ancer.[COPD]: ht
-00002670: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00002680: 2f41 6172 6875 732d 5073 7963 6869 6174  /Aarhus-Psychiat
-00002690: 7279 2d52 6573 6561 7263 682f 7073 7963  ry-Research/psyc
-000026a0: 6f70 2d63 6f70 640a 5b46 6f72 6365 6420  op-copd.[Forced 
-000026b0: 6164 6d69 7373 696f 6e73 5d3a 2068 7474  admissions]: htt
-000026c0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000026d0: 4161 7268 7573 2d50 7379 6368 6961 7472  Aarhus-Psychiatr
-000026e0: 792d 5265 7365 6172 6368 2f70 7379 636f  y-Research/psyco
-000026f0: 702d 666f 7263 6564 2d61 646d 6973 7369  p-forced-admissi
-00002700: 6f6e 730a 5b43 6f65 7263 696f 6e5d 3a20  ons.[Coercion]: 
-00002710: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00002720: 6f6d 2f41 6172 6875 732d 5073 7963 6869  om/Aarhus-Psychi
-00002730: 6174 7279 2d52 6573 6561 7263 682f 7079  atry-Research/py
-00002740: 7363 6f70 2d63 6f65 7263 696f 6e0a       scop-coercion.
+00002180: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
+00002190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021a0: 2020 207c 0a7c 202d 2d2d 2d2d 2d2d 2d2d     |.| ---------
+000021b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000021c0: 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d  ----- | --------
+000021d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c  -------------- |
+000021e0: 0a7c 20f0 9f9a a820 2a2a 4275 6720 5265  .| .... **Bug Re
+000021f0: 706f 7274 732a 2a20 2020 2020 2020 2020  ports**         
+00002200: 2020 2020 207c 205b 4769 7448 7562 2049       | [GitHub I
+00002210: 7373 7565 2054 7261 636b 6572 5d20 7c0a  ssue Tracker] |.
+00002220: 7c20 f09f 8e81 202a 2a46 6561 7475 7265  | .... **Feature
+00002230: 2052 6571 7565 7374 7320 2620 4964 6561   Requests & Idea
+00002240: 732a 2a20 7c20 5b47 6974 4875 6220 4973  s** | [GitHub Is
+00002250: 7375 6520 5472 6163 6b65 725d 207c 0a7c  sue Tracker] |.|
+00002260: 20f0 9f91 a9e2 808d f09f 92bb 202a 2a55   ........... **U
+00002270: 7361 6765 2051 7565 7374 696f 6e73 2a2a  sage Questions**
+00002280: 2020 2020 2020 2020 2020 7c20 5b47 6974            | [Git
+00002290: 4875 6220 4469 7363 7573 7369 6f6e 735d  Hub Discussions]
+000022a0: 2020 207c 0a7c 20f0 9f97 af20 2a2a 4765     |.| .... **Ge
+000022b0: 6e65 7261 6c20 4469 7363 7573 7369 6f6e  neral Discussion
+000022c0: 2a2a 2020 2020 2020 207c 205b 4769 7448  **       | [GitH
+000022d0: 7562 2044 6973 6375 7373 696f 6e73 5d20  ub Discussions] 
+000022e0: 2020 7c0a 0a5b 6769 7468 7562 2069 7373    |..[github iss
+000022f0: 7565 2074 7261 636b 6572 5d3a 2068 7474  ue tracker]: htt
+00002300: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00002310: 4161 7268 7573 2d50 7379 6368 6961 7472  Aarhus-Psychiatr
+00002320: 792d 5265 7365 6172 6368 2f74 696d 6573  y-Research/times
+00002330: 6572 6965 7366 6c61 7474 656e 6572 2f69  eriesflattener/i
+00002340: 7373 7565 730a 5b67 6974 6875 6220 6469  ssues.[github di
+00002350: 7363 7573 7369 6f6e 735d 3a20 6874 7470  scussions]: http
+00002360: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f41  s://github.com/A
+00002370: 6172 6875 732d 5073 7963 6869 6174 7279  arhus-Psychiatry
+00002380: 2d52 6573 6561 7263 682f 7469 6d65 7365  -Research/timese
+00002390: 7269 6573 666c 6174 7465 6e65 722f 6469  riesflattener/di
+000023a0: 7363 7573 7369 6f6e 730a 0a0a 2323 20f0  scussions...## .
+000023b0: 9f8e 9320 5072 6f6a 6563 7473 0a50 5359  ... Projects.PSY
+000023c0: 434f 5020 7072 6f6a 6563 7473 2077 6869  COP projects whi
+000023d0: 6368 2075 7365 2060 7469 6d65 7365 7269  ch use `timeseri
+000023e0: 6573 666c 6174 7465 6e65 7260 2e20 4e6f  esflattener`. No
+000023f0: 7465 2074 6861 7420 736f 6d65 206f 6620  te that some of 
+00002400: 7468 6573 6520 7072 6f6a 6563 7473 2068  these projects h
+00002410: 6176 6520 7965 7420 746f 2062 6520 7075  ave yet to be pu
+00002420: 626c 6973 6865 6420 616e 6420 6172 6520  blished and are 
+00002430: 7468 7573 2070 7269 7661 7465 2e0a 0a7c  thus private...|
+00002440: 2050 726f 6a65 6374 2020 2020 2020 2020   Project        
+00002450: 2020 2020 2020 2020 207c 2050 7562 6c69           | Publi
+00002460: 6361 7469 6f6e 7320 7c20 2020 2020 2020  cations |       
+00002470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002550: 7c0a 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |.| ------------
+00002560: 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c20 2d2d  ----------- | --
+00002570: 2d2d 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d  ---------- | ---
+00002580: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002590: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000025a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000025b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000025c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000025d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000025e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000025f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002600: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002610: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002620: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002630: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002640: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002650: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002660: 2d2d 207c 0a7c 202a 2a5b 5479 7065 2032  -- |.| **[Type 2
+00002670: 2044 6961 6265 7465 735d 2a2a 2020 207c   Diabetes]**   |
+00002680: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00002690: 5072 6564 6963 7469 6f6e 206f 6620 7479  Prediction of ty
+000026a0: 7065 2032 2064 6961 6265 7465 7320 616d  pe 2 diabetes am
+000026b0: 6f6e 6720 7061 7469 656e 7473 2077 6974  ong patients wit
+000026c0: 6820 7669 7369 7473 2074 6f20 7073 7963  h visits to psyc
+000026d0: 6869 6174 7269 6320 686f 7370 6974 616c  hiatric hospital
+000026e0: 2064 6570 6172 746d 656e 7473 2020 2020   departments    
+000026f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002770: 2020 2020 2020 7c0a 7c20 2a2a 5b43 616e        |.| **[Can
+00002780: 6365 725d 2a2a 2020 2020 2020 2020 2020  cer]**          
+00002790: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
+000027a0: 207c 2050 7265 6469 6374 696f 6e20 6f66   | Prediction of
+000027b0: 2043 616e 6365 7220 616d 6f6e 6720 7061   Cancer among pa
+000027c0: 7469 656e 7473 2077 6974 6820 7669 7369  tients with visi
+000027d0: 7473 2074 6f20 7073 7963 6869 6174 7269  ts to psychiatri
+000027e0: 6320 686f 7370 6974 616c 2064 6570 6172  c hospital depar
+000027f0: 746d 656e 7473 2020 2020 2020 2020 2020  tments          
+00002800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002880: 2020 2020 2020 2020 207c 0a7c 202a 2a5b           |.| **[
+00002890: 434f 5044 5d2a 2a20 2020 2020 2020 2020  COPD]**         
+000028a0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+000028b0: 2020 2020 7c20 5072 6564 6963 7469 6f6e      | Prediction
+000028c0: 206f 6620 4368 726f 6e69 6320 6f62 7374   of Chronic obst
+000028d0: 7275 6374 6976 6520 7075 6c6d 6f6e 6172  ructive pulmonar
+000028e0: 7920 6469 7365 6173 6520 2843 4f50 4429  y disease (COPD)
+000028f0: 2061 6d6f 6e67 2070 6174 6965 6e74 7320   among patients 
+00002900: 7769 7468 2076 6973 6974 7320 746f 2070  with visits to p
+00002910: 7379 6368 6961 7472 6963 2068 6f73 7069  sychiatric hospi
+00002920: 7461 6c20 6465 7061 7274 6d65 6e74 7320  tal departments 
+00002930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002990: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+000029a0: 2a2a 5b46 6f72 6365 6420 6164 6d69 7373  **[Forced admiss
+000029b0: 696f 6e73 5d2a 2a20 7c20 2020 2020 2020  ions]** |       
+000029c0: 2020 2020 2020 207c 2050 7265 6469 6374         | Predict
+000029d0: 696f 6e20 6f66 2066 6f72 6365 6420 6164  ion of forced ad
+000029e0: 6d69 7373 696f 6e73 206f 6620 7061 7469  missions of pati
+000029f0: 656e 7473 2074 6f20 7468 6520 7073 7963  ents to the psyc
+00002a00: 6869 6174 7269 6320 686f 7370 6974 616c  hiatric hospital
+00002a10: 2064 6570 6172 746d 656e 7473 2e20 456e   departments. En
+00002a20: 636f 6d70 6173 7365 7320 7477 6f20 7365  compasses two se
+00002a30: 7061 7261 7465 2070 726f 6a65 6374 733a  parate projects:
+00002a40: 2031 2e20 5072 6564 6963 6974 696e 6720   1. Prediciting 
+00002a50: 6174 2074 696d 6520 6f66 2064 6973 6368  at time of disch
+00002a60: 6172 6765 2066 6f72 2069 6e70 6174 6965  arge for inpatie
+00002a70: 6e74 2061 646d 6973 7369 6f6e 732e 2032  nt admissions. 2
+00002a80: 2e20 5072 6564 6963 7469 6e67 2064 6179  . Predicting day
+00002a90: 2062 6566 6f72 6520 6f75 7470 6174 6965   before outpatie
+00002aa0: 6e74 2061 646d 6973 7369 6f6e 732e 207c  nt admissions. |
+00002ab0: 0a7c 202a 2a5b 436f 6572 6369 6f6e 5d2a  .| **[Coercion]*
+00002ac0: 2a20 2020 2020 2020 2020 207c 2020 2020  *          |    
+00002ad0: 2020 2020 2020 2020 2020 7c20 5072 6564            | Pred
+00002ae0: 6963 7469 6f6e 206f 6620 636f 6572 6369  iction of coerci
+00002af0: 6f6e 2061 6d6f 6e67 2070 6174 6965 6e74  on among patient
+00002b00: 7320 6164 6d69 7474 6965 6420 746f 2074  s admittied to t
+00002b10: 6865 2068 6f73 7069 7461 6c20 7073 7963  he hospital psyc
+00002b20: 6869 6174 7269 6320 6465 7061 7274 6d65  hiatric departme
+00002b30: 6e74 2e20 456e 636f 6d70 6173 7365 7320  nt. Encompasses 
+00002b40: 7072 6564 6963 7469 6e67 206d 6563 6861  predicting mecha
+00002b50: 6e69 6361 6c20 7265 7374 7261 696e 742c  nical restraint,
+00002b60: 2073 6564 6174 6976 6520 6d65 6469 6361   sedative medica
+00002b70: 7469 6f6e 2061 6e64 206d 616e 7561 6c20  tion and manual 
+00002b80: 7265 7374 7261 696e 7420 3438 2068 6f75  restraint 48 hou
+00002b90: 7273 2062 6566 6f72 6520 636f 6572 6369  rs before coerci
+00002ba0: 6f6e 206f 6363 7572 732e 2020 2020 2020  on occurs.      
+00002bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bc0: 2020 7c0a 0a0a 5b54 7970 6520 3220 6469    |...[Type 2 di
+00002bd0: 6162 6574 6573 5d3a 2068 7474 7073 3a2f  abetes]: https:/
+00002be0: 2f67 6974 6875 622e 636f 6d2f 4161 7268  /github.com/Aarh
+00002bf0: 7573 2d50 7379 6368 6961 7472 792d 5265  us-Psychiatry-Re
+00002c00: 7365 6172 6368 2f70 7379 636f 702d 7432  search/psycop-t2
+00002c10: 640a 5b43 616e 6365 725d 3a20 6874 7470  d.[Cancer]: http
+00002c20: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f41  s://github.com/A
+00002c30: 6172 6875 732d 5073 7963 6869 6174 7279  arhus-Psychiatry
+00002c40: 2d52 6573 6561 7263 682f 7073 7963 6f70  -Research/psycop
+00002c50: 2d63 616e 6365 720a 5b43 4f50 445d 3a20  -cancer.[COPD]: 
+00002c60: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00002c70: 6f6d 2f41 6172 6875 732d 5073 7963 6869  om/Aarhus-Psychi
+00002c80: 6174 7279 2d52 6573 6561 7263 682f 7073  atry-Research/ps
+00002c90: 7963 6f70 2d63 6f70 640a 5b46 6f72 6365  ycop-copd.[Force
+00002ca0: 6420 6164 6d69 7373 696f 6e73 5d3a 2068  d admissions]: h
+00002cb0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00002cc0: 6d2f 4161 7268 7573 2d50 7379 6368 6961  m/Aarhus-Psychia
+00002cd0: 7472 792d 5265 7365 6172 6368 2f70 7379  try-Research/psy
+00002ce0: 636f 702d 666f 7263 6564 2d61 646d 6973  cop-forced-admis
+00002cf0: 7369 6f6e 730a 5b43 6f65 7263 696f 6e5d  sions.[Coercion]
+00002d00: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+00002d10: 2e63 6f6d 2f41 6172 6875 732d 5073 7963  .com/Aarhus-Psyc
+00002d20: 6869 6174 7279 2d52 6573 6561 7263 682f  hiatry-Research/
+00002d30: 7079 7363 6f70 2d63 6f65 7263 696f 6e0a  pyscop-coercion.
```

### Comparing `timeseriesflattener-0.23.9/src/timeseriesflattener.egg-info/SOURCES.txt` & `timeseriesflattener-0.24.0/src/timeseriesflattener.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,37 @@
-.codespellrc
-.flake8
+.cookiecutter.json
+.cruft.json
 .gitignore
 .pre-commit-config.yaml
 .zenodo.json
 CHANGELOG.md
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
+Makefile
 README.md
 citation.cff
 icon.png
 pyproject.toml
+tasks.py
 .github/dependabot.yml
 .github/pull_request_template.md
+.github/recommended_repo_setup.md
 .github/setup_ci.md
 .github/actions/test/action.yml
 .github/actions/test_tutorials/action.yml
+.github/workflows/check_for_rej.yml
+.github/workflows/cruft.yml
 .github/workflows/dependabot_automerge.yml
 .github/workflows/documentation.yml
 .github/workflows/generate_paper_pdf.yml
 .github/workflows/main_test_and_release.yml
 .github/workflows/pre-commit.yml
+.github/workflows/stalebot.yml
+.github/workflows/static_type_checks.yml
 docs/Makefile
 docs/conf.py
 docs/faq.rst
 docs/feature_specifications.rst
 docs/index.rst
 docs/installation.rst
 docs/timeseriesflattener.rst
```

### Comparing `timeseriesflattener-0.23.9/src/timeseriesflattener.egg-info/requires.txt` & `timeseriesflattener-0.24.0/src/timeseriesflattener.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,45 @@
 scipy<1.9.4,>=1.8.0
 scikit-learn<1.2.3,>=1.1.2
 pydantic<1.11.0,>=1.9.0
-pandas<1.6.0,>=1.4.0
+pandas<2.1.0,>=1.4.0
 catalogue<2.1.0,>=2.0.0
 numpy<1.24.2,>=1.23.3
 pyarrow<11.1.0,>=9.0.0
-protobuf<=3.20.3
+protobuf<=4.22.3
 frozendict<2.4.0,>=2.3.4
 coloredlogs<15.1.0,>14.0.0
 psycopmlutils<0.12.0,>=0.5.0
 
 [dev]
-black<23.1.1,>=22.8.0
-pre-commit<3.2.2,>=2.20.0
-mypy<1.2,>=0.971
-pytest<7.2.3,>=7.1.3
-pytest-cov<4.0.1,>=3.0.0
-pytest-xdist<3.2.2,>=2.4.0
+cruft
+pyright
+pre-commit<2.21.0,==2.20.0
+ruff==0.0.262
+black[jupyter]==22.8.0
+pandas-stubs
+invoke
+tox
 
 [docs]
 sphinx<6.2.0,>=5.3.0
-furo==2023.3.23
-sphinx-copybutton<0.5.2,>=0.5.1
-sphinxext-opengraph<0.8.2,>=0.7.3
+furo==2023.3.27
+sphinx-copybutton<0.5.3,>=0.5.1
+sphinxext-opengraph<0.8.3,>=0.7.3
 myst-nb<1.17.0,>=0.6.0
 sphinx_design<0.3.1,>=0.3.0
 autodoc_pydantic<1.9.0,>=1.1.0
 
+[test]
+pytest<7.3.0,>=7.1.3
+pytest-cov<3.1.0,>=3.0.0
+pytest-xdist<3.2.0,>=3.0.0
+pytest-sugar<0.10.0,>=0.9.4
+
 [text]
-transformers<4.28.0,>=4.26.0
+transformers<4.29.0,>=4.26.0
 torch<2.1.0,>=1.12.0
 sentence-transformers<2.5.0,>=1.0.0
 
 [tutorials]
 jupyter<1.1.0,>=1.0.0
 skimpy<0.1.0,>=0.0.7
```

### Comparing `timeseriesflattener-0.23.9/tests/conftest.py` & `timeseriesflattener-0.24.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/tests/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py` & `timeseriesflattener-0.24.0/tests/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/tests/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv` & `timeseriesflattener-0.24.0/tests/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/tests/test_data/models/create_bow_and_pca_model.py` & `timeseriesflattener-0.24.0/tests/test_data/models/create_bow_and_pca_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     model.fit(embedding)
     return model
 
 
 def save_model_to_test_dir(
     model: Any,
     filename: str,
-):  # pylint: disable=missing-type-doc
+):
     """
     Saves the model to a pickle file
 
     Args:
         model: The model to save
         filename: The filename to save the model to
     """
```

### Comparing `timeseriesflattener-0.23.9/tests/test_data/models/synth_bow_model.pkl` & `timeseriesflattener-0.24.0/tests/test_data/models/synth_bow_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/tests/test_data/models/synth_pca_model.pkl` & `timeseriesflattener-0.24.0/tests/test_data/models/synth_pca_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/tests/test_data/raw/create_synth_prediction_times.py` & `timeseriesflattener-0.24.0/tests/test_data/raw/create_synth_prediction_times.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/tests/test_data/raw/create_synth_raw_binary.py` & `timeseriesflattener-0.24.0/tests/test_data/raw/create_synth_raw_binary.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/tests/test_data/raw/create_synth_raw_float.py` & `timeseriesflattener-0.24.0/tests/test_data/raw/create_synth_raw_float.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/tests/test_data/raw/create_synth_sex.py` & `timeseriesflattener-0.24.0/tests/test_data/raw/create_synth_sex.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/tests/test_data/raw/synth_prediction_times.csv` & `timeseriesflattener-0.24.0/tests/test_data/raw/synth_prediction_times.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/tests/test_data/raw/synth_raw_binary_1.csv` & `timeseriesflattener-0.24.0/tests/test_data/raw/synth_raw_binary_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/tests/test_data/raw/synth_raw_binary_2.csv` & `timeseriesflattener-0.24.0/tests/test_data/raw/synth_raw_binary_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/tests/test_data/raw/synth_raw_float_1.csv` & `timeseriesflattener-0.24.0/tests/test_data/raw/synth_raw_float_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/tests/test_data/raw/synth_raw_float_2.csv` & `timeseriesflattener-0.24.0/tests/test_data/raw/synth_raw_float_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/tests/test_data/raw/synth_sex.csv` & `timeseriesflattener-0.24.0/tests/test_data/raw/synth_sex.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/tests/test_data/raw/synth_text_data.csv` & `timeseriesflattener-0.24.0/tests/test_data/raw/synth_text_data.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/tests/test_feature_cache/test_cache_to_disk.py` & `timeseriesflattener-0.24.0/tests/test_feature_cache/test_cache_to_disk.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             "timestamp": [1, 2, 3],
             "value": [1, 2, 3],
         },
     )
 
     test_spec = PredictorSpec(
         values_df=values_df,
-        interval_days=5,
+        lookbehind_days=5,
         resolve_multiple_fn=latest,
         key_for_resolve_multiple="latest",
         fallback=np.nan,
         feature_name="test_feature",
     )
 
     generated_df = pd.DataFrame(
```

### Comparing `timeseriesflattener-0.23.9/tests/test_timeseriesflattener/test_embedding_functions.py` & `timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.23.9/tests/test_timeseriesflattener/test_feature_spec_objects.py` & `timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_feature_spec_objects.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Test that feature spec objects work as intended."""
 
+
 from typing import List
 
 import numpy as np
 import pandas as pd
 import pytest
 from timeseriesflattener.feature_spec_objects import (
     BaseModel,
@@ -14,15 +15,15 @@
     TemporalSpec,
     TextPredictorSpec,
     _AnySpec,
     check_that_col_names_in_kwargs_exist_in_df,
     generate_docstring_from_attributes,
 )
 from timeseriesflattener.resolve_multiple_functions import maximum
-from timeseriesflattener.testing.load_synth_data import (  # pylint: disable=unused-import; noqa
+from timeseriesflattener.testing.load_synth_data import (
     load_synth_predictor_float,
     synth_predictor_binary,
 )
 from timeseriesflattener.utils import split_df_and_register_to_dict
 
 
 def test_anyspec_init():
@@ -140,14 +141,26 @@
         fallback=[np.nan],
         resolve_multiple_fn=[maximum],
     ).create_combinations()
 
     assert "maximum" in pred_spec_batch[0].get_col_str()
 
 
+def test_lookbehind_days_handles_floats():
+    """Test that lookbheind days does not coerce floats into ints."""
+    pred_spec_batch = PredictorGroupSpec(
+        values_loader=["synth_predictor_float"],
+        lookbehind_days=[2, 0.5],
+        fallback=[np.nan],
+        resolve_multiple_fn=[maximum],
+    ).create_combinations()
+
+    assert pred_spec_batch[1].lookbehind_days == 0.5
+
+
 def get_lines_with_diff(text1: str, text2: str) -> List[str]:
     """Find all lines in text1 which are different from text2."""
     # Remove whitespace and periods
     text_1 = text1.replace(" ", "").replace(".", "")
     text_2 = text2.replace(" ", "").replace(".", "")
 
     lines1 = text_1.splitlines()
@@ -165,15 +178,15 @@
         TextPredictorSpec,
         OutcomeSpec,
         OutcomeGroupSpec,
     ],
 )
 def test_feature_spec_docstrings(spec: BaseModel):
     """Test that docstring is generated correctly."""
-    current_docstring = spec.__doc__
+    current_docstring: str = spec.__doc__  # type: ignore
     generated_docstring = generate_docstring_from_attributes(cls=spec)
     # strip docstrings of newlines and whitespace to allow room for formatting
     current_docstring_no_whitespace = (
         current_docstring.replace(" ", "")
         .replace(
             "\n",
             "",
```

### Comparing `timeseriesflattener-0.23.9/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py` & `timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Tests for adding values to a flattened dataset."""
 
-# pylint: disable=missing-function-docstring
 
 import numpy as np
 import pandas as pd
 import pytest
 from timeseriesflattener import TimeseriesFlattener
 from timeseriesflattener.feature_spec_objects import (
     OutcomeSpec,
@@ -14,16 +13,14 @@
 )
 from timeseriesflattener.testing.text_embedding_functions import bow_test_embedding
 from timeseriesflattener.testing.utils_for_testing import (
     assert_flattened_data_as_expected,
     str_to_df,
 )
 
-# pylint: disable=import-error
-
 
 # Predictors
 def test_predictor_after_prediction_time():
     prediction_times_df = str_to_df(
         """entity_id,timestamp,
     1,2021-12-31 00:00:00
     """,
@@ -230,15 +227,15 @@
 
     dataset = TimeseriesFlattener(
         prediction_times_df=str_to_df(prediction_times_df),
         drop_pred_times_with_insufficient_look_distance=False,
     )
 
     dataset.add_spec(
-        StaticSpec(
+        StaticSpec(  # type: ignore
             values_df=str_to_df(static_predictor),
             feature_name=feature_name,
             prefix=prefix,
             input_col_name_override=feature_name,
         ),
     )
 
@@ -426,15 +423,15 @@
         incident=True,
         feature_name="value",
     )
 
     flattened_dataset.add_spec(
         spec=[
             output_spec,
-            StaticSpec(
+            StaticSpec(  # type: ignore
                 values_df=male_df,
                 feature_name="male",
                 prefix="pred",
                 input_col_name_override="male",
                 output_col_name_override="pred_male_overridden",
             ),
         ],
```

### Comparing `timeseriesflattener-0.23.9/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py` & `timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Test that cache hits."""
-# pylint: disable=unused-import, redefined-outer-name
+
 
 from pathlib import Path
 from typing import List
 
 import numpy as np
 import pandas as pd
 import pytest
@@ -45,14 +45,15 @@
     synth_prediction_times: pd.DataFrame,
 ):
     """Test that cache hits."""
 
     cache = DiskCache(
         feature_cache_dir=tmp_path,
         entity_id_col_name="entity_id",
+        prediction_times_df=synth_prediction_times,
     )
 
     # Create the cache
     first_df = create_flattened_df(
         predictor_specs=predictor_specs.copy(),
         prediction_times_df=synth_prediction_times,
         cache=cache,
```

### Comparing `timeseriesflattener-0.23.9/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py` & `timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from typing import Any, Callable, List
 
 import pandas as pd
 import pytest
 from pandas import DataFrame
 from timeseriesflattener.flattened_dataset import TimeseriesFlattener
 
-# pylint: disable=protected-access
-
 
 def benchmark(func: Callable, *args: Any, **kwargs: Any) -> float:
     """Benchmark a function."""
     start = time.perf_counter()
     func(*args, **kwargs)
     end = time.perf_counter()
     print(f"{func.__name__} took {end - start:.4f} seconds to execute.")
@@ -25,15 +23,15 @@
     """Generate a test df with a random integer column and a uuid index."""
     df = pd.DataFrame()
 
     # create a column with random integers between 1 and 1000_000
     df["random_int"] = col_values
 
     # Set index to uuids
-    df.index = uuids
+    df.index = uuids  # type: ignore
 
     # Sort df by indices
     print("Generated df")
 
     return df
```

### Comparing `timeseriesflattener-0.23.9/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py` & `timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """Tests for errors raised from flattened dataset class."""
 
 import pytest
 from timeseriesflattener.feature_spec_objects import PredictorSpec
 from timeseriesflattener.flattened_dataset import TimeseriesFlattener
 from timeseriesflattener.testing.utils_for_testing import (
-    str_to_df,  # pylint: disable=import-error
+    str_to_df,
 )
 
-# pylint: disable=missing-function-docstring
-
 
 def test_col_does_not_exist_in_prediction_times():
     prediction_times_str = """entity_id,
                             1,
                             """
 
     prediction_times_df = str_to_df(prediction_times_str)
```

### Comparing `timeseriesflattener-0.23.9/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py` & `timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     # Test adding multiple specs
     dataset.add_spec([predictor_spec, static_spec])
     assert dataset.unprocessed_specs.predictor_specs == [predictor_spec]
     assert dataset.unprocessed_specs.static_specs == [static_spec]
 
     # Test adding an invalid spec type
     with pytest.raises(ValueError):  # noqa
-        dataset.add_spec("invalid spec")
+        dataset.add_spec("invalid spec")  # type: ignore
 
 
 @pytest.mark.huggingface()
 def test_compute_specs(
     synth_prediction_times: pd.DataFrame,
     synth_outcome: pd.DataFrame,
     synth_text_data: pd.DataFrame,
@@ -85,15 +85,15 @@
         fallback=np.nan,
     )
     static_spec = StaticSpec(
         values_df=synth_outcome[["value", "entity_id"]],
         feature_name="static",
         prefix="pred",
     )
-    text_spec = TextPredictorSpec(
+    text_spec = TextPredictorSpec(  # type: ignore
         values_df=synth_text_data,
         feature_name="text",
         lookbehind_days=750,
         input_col_name_override="text",
         resolve_multiple_fn="concatenate",
         fallback=np.nan,
         embedding_fn=sentence_transformers_embedding,
```

### Comparing `timeseriesflattener-0.23.9/tests/test_timeseriesflattener/test_flattened_dataset/utils.py` & `timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_flattened_dataset/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Integration test for the flattened dataset generation."""
 
-# pylint: disable=unused-import, redefined-outer-name
 
 from typing import List, Optional
 
 import numpy as np
 import pandas as pd
 from timeseriesflattener.feature_cache.abstract_feature_cache import FeatureCache
 from timeseriesflattener.feature_spec_objects import PredictorSpec
@@ -66,11 +65,11 @@
         prediction_times_df=prediction_times_df,
         n_workers=1,
         cache=cache,
         drop_pred_times_with_insufficient_look_distance=False,
     )
 
     flat_ds.add_spec(
-        spec=predictor_specs,
+        spec=predictor_specs,  # type: ignore
     )
 
     return flat_ds.get_df()
```

### Comparing `timeseriesflattener-0.23.9/tests/test_timeseriesflattener/test_resolve_multiple.py` & `timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_resolve_multiple.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Tests of resolve_multiple strategies."""
-# pylint: disable=missing-function-docstring
+
 
 import numpy as np
 from timeseriesflattener.feature_spec_objects import OutcomeSpec, PredictorSpec
 from timeseriesflattener.testing.utils_for_testing import (
     assert_flattened_data_as_expected,
     str_to_df,
 )
```

### Comparing `timeseriesflattener-0.23.9/tests/test_timeseriesflattener/test_utils.py` & `timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 
     spec = _AnySpec(
         values_name="value_name_1",
         feature_name="test",
         prefix="test",
     )
 
-    assert len(spec.values_df) == 10000
+    assert len(spec.values_df) == 10000  # type: ignore
```

