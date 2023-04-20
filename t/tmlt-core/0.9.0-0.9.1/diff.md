# Comparing `tmp/tmlt_core-0.9.0.tar.gz` & `tmp/tmlt_core-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmlt_core-0.9.0.tar", max compression
+gzip compressed data, was "tmlt_core-0.9.1.tar", max compression
```

## Comparing `tmlt_core-0.9.0.tar` & `tmlt_core-0.9.1.tar`

### file list

```diff
@@ -1,186 +1,186 @@
--rw-r--r--   0        0        0    10069 2023-04-14 16:44:30.148892 tmlt_core-0.9.0/CHANGELOG.rst
--rw-r--r--   0        0        0    11358 2023-04-14 16:44:30.148892 tmlt_core-0.9.0/LICENSE
--rw-r--r--   0        0        0    20138 2023-04-14 16:44:30.148892 tmlt_core-0.9.0/LICENSE.docs
--rw-r--r--   0        0        0      116 2023-04-14 16:44:30.148892 tmlt_core-0.9.0/NOTICE
--rw-r--r--   0        0        0     1868 2023-04-14 16:44:30.148892 tmlt_core-0.9.0/README.md
--rw-r--r--   0        0        0    11481 2023-04-14 16:44:30.148892 tmlt_core-0.9.0/benchmark/benchmark_count_sum.py
--rw-r--r--   0        0        0     3838 2023-04-14 16:44:30.148892 tmlt_core-0.9.0/benchmark/benchmark_noise_mechanism.py
--rw-r--r--   0        0        0     8652 2023-04-14 16:44:30.149892 tmlt_core-0.9.0/benchmark/benchmark_private_join.py
--rw-r--r--   0        0        0    15676 2023-04-14 16:44:30.149892 tmlt_core-0.9.0/benchmark/benchmark_public_join.py
--rw-r--r--   0        0        0     8873 2023-04-14 16:44:30.149892 tmlt_core-0.9.0/benchmark/benchmark_quantile.py
--rw-r--r--   0        0        0    10207 2023-04-14 16:44:30.149892 tmlt_core-0.9.0/benchmark/benchmark_sparkflatmap.py
--rw-r--r--   0        0        0     9446 2023-04-14 16:44:30.149892 tmlt_core-0.9.0/benchmark/benchmark_sparkmap.py
--rw-r--r--   0        0        0      731 2023-04-14 16:44:30.149892 tmlt_core-0.9.0/benchmark/benchmarking_utils.py
--rw-r--r--   0        0        0      951 2023-04-14 16:44:30.149892 tmlt_core-0.9.0/doc/_static/css/custom.css
--rw-r--r--   0        0        0    12470 2023-04-14 16:44:30.149892 tmlt_core-0.9.0/doc/_static/favicon.ico
--rw-r--r--   0        0        0     1001 2023-04-14 16:44:30.149892 tmlt_core-0.9.0/doc/_static/js/version-banner.js
--rw-r--r--   0        0        0    30903 2023-04-14 16:44:30.149892 tmlt_core-0.9.0/doc/_static/logo.png
--rw-r--r--   0        0        0       50 2023-04-14 16:44:30.149892 tmlt_core-0.9.0/doc/_templates/build-info.html
--rw-r--r--   0        0        0      408 2023-04-14 16:44:30.149892 tmlt_core-0.9.0/doc/_templates/layout.html
--rw-r--r--   0        0        0       23 2023-04-14 16:44:30.149892 tmlt_core-0.9.0/doc/_templates/package-name.html
--rw-r--r--   0        0        0      210 2023-04-14 16:44:30.150892 tmlt_core-0.9.0/doc/additional-resources/index.rst
--rw-r--r--   0        0        0      660 2023-04-14 16:44:30.150892 tmlt_core-0.9.0/doc/additional-resources/license.rst
--rw-r--r--   0        0        0     3159 2023-04-14 16:44:30.150892 tmlt_core-0.9.0/doc/additional-resources/privacy_policy.rst
--rw-r--r--   0        0        0     6889 2023-04-14 16:44:30.150892 tmlt_core-0.9.0/doc/conf.py
--rw-r--r--   0        0        0     1836 2023-04-14 16:44:30.150892 tmlt_core-0.9.0/doc/images/index_api.svg
--rw-r--r--   0        0        0     1186 2023-04-14 16:44:30.150892 tmlt_core-0.9.0/doc/images/index_more.svg
--rw-r--r--   0        0        0      596 2023-04-14 16:44:30.150892 tmlt_core-0.9.0/doc/images/index_topic_guides.svg
--rw-r--r--   0        0        0     1363 2023-04-14 16:44:30.150892 tmlt_core-0.9.0/doc/images/index_tutorials.svg
--rw-r--r--   0        0        0    30903 2023-04-14 16:44:30.150892 tmlt_core-0.9.0/doc/images/logo.png
--rw-r--r--   0        0        0     3186 2023-04-14 16:44:30.150892 tmlt_core-0.9.0/doc/index.rst
--rw-r--r--   0        0        0     4541 2023-04-14 16:44:30.150892 tmlt_core-0.9.0/doc/installation.rst
--rw-r--r--   0        0        0     6510 2023-04-14 16:44:30.150892 tmlt_core-0.9.0/doc/ref.bib
--rw-r--r--   0        0        0     2006 2023-04-14 16:44:30.150892 tmlt_core-0.9.0/doc/templates/python/class.rst
--rw-r--r--   0        0        0     3244 2023-04-14 16:44:30.150892 tmlt_core-0.9.0/doc/templates/python/module.rst
--rw-r--r--   0        0        0    16713 2023-04-14 16:44:30.151892 tmlt_core-0.9.0/doc/topic-guides/architecture.rst
--rw-r--r--   0        0        0      345 2023-04-14 16:44:30.151892 tmlt_core-0.9.0/doc/topic-guides/index.rst
--rw-r--r--   0        0        0     1424 2023-04-14 16:44:30.151892 tmlt_core-0.9.0/doc/topic-guides/known-vulnerabilities.rst
--rw-r--r--   0        0        0     6510 2023-04-14 16:44:30.151892 tmlt_core-0.9.0/doc/topic-guides/privacy-guarantee.rst
--rw-r--r--   0        0        0     2289 2023-04-14 16:44:30.151892 tmlt_core-0.9.0/doc/topic-guides/real-numbers.rst
--rw-r--r--   0        0        0     6151 2023-04-14 16:44:30.151892 tmlt_core-0.9.0/doc/topic-guides/spark.rst
--rw-r--r--   0        0        0     8100 2023-04-14 16:44:30.151892 tmlt_core-0.9.0/doc/topic-guides/special-values.rst
--rw-r--r--   0        0        0     7334 2023-04-14 16:44:30.151892 tmlt_core-0.9.0/doc/tutorials/first-tutorial.rst
--rw-r--r--   0        0        0      231 2023-04-14 16:44:30.151892 tmlt_core-0.9.0/doc/tutorials/index.rst
--rw-r--r--   0        0        0       88 2023-04-14 16:44:30.151892 tmlt_core-0.9.0/doc/zcitations.rst
--rw-r--r--   0        0        0      363 2023-04-14 16:44:30.151892 tmlt_core-0.9.0/ext/build.py
--rw-r--r--   0        0        0     3175 2023-04-14 16:44:30.151892 tmlt_core-0.9.0/ext/build.sh
--rw-r--r--   0        0        0      150 2023-04-14 16:44:30.151892 tmlt_core-0.9.0/ext/dependency_versions.sh
--rw-r--r--   0        0        0     4909 2023-04-14 16:45:17.001831 tmlt_core-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      103 2023-04-14 16:44:30.152892 tmlt_core-0.9.0/test/__init__.py
--rw-r--r--   0        0        0      110 2023-04-14 16:44:30.152892 tmlt_core-0.9.0/test/system/__init__.py
--rw-r--r--   0        0        0     3889 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/system/measurements/test_interactive_measurements.py
--rw-r--r--   0        0        0      654 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/system/noise_distribution_tests/__init__.py
--rw-r--r--   0        0        0     5468 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/system/noise_distribution_tests/test_average.py
--rw-r--r--   0        0        0    11426 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/system/noise_distribution_tests/test_base_mechanisms.py
--rw-r--r--   0        0        0     4671 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/system/noise_distribution_tests/test_count.py
--rw-r--r--   0        0        0     4849 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/system/noise_distribution_tests/test_count_distinct.py
--rw-r--r--   0        0        0     5670 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/system/noise_distribution_tests/test_quantile.py
--rw-r--r--   0        0        0      844 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/system/noise_distribution_tests/test_samplers.py
--rw-r--r--   0        0        0     6706 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/system/noise_distribution_tests/test_standard_deviation.py
--rw-r--r--   0        0        0     5197 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/system/noise_distribution_tests/test_sum.py
--rw-r--r--   0        0        0     7067 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/system/noise_distribution_tests/test_variance.py
--rw-r--r--   0        0        0      108 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/unit/__init__.py
--rw-r--r--   0        0        0      116 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/unit/domains/__init__.py
--rw-r--r--   0        0        0     1176 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/unit/domains/test_base.py
--rw-r--r--   0        0        0     6558 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/unit/domains/test_collections.py
--rw-r--r--   0        0        0     8866 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/unit/domains/test_numpy_domains.py
--rw-r--r--   0        0        0     9857 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/unit/domains/test_pandas_domains.py
--rw-r--r--   0        0        0    26425 2023-04-14 16:44:30.154892 tmlt_core-0.9.0/test/unit/domains/test_spark_domains.py
--rw-r--r--   0        0        0      121 2023-04-14 16:44:30.154892 tmlt_core-0.9.0/test/unit/measurements/__init__.py
--rw-r--r--   0        0        0      141 2023-04-14 16:44:30.154892 tmlt_core-0.9.0/test/unit/measurements/pandas_measurements/__init__.py
--rw-r--r--   0        0        0    13818 2023-04-14 16:44:30.154892 tmlt_core-0.9.0/test/unit/measurements/pandas_measurements/test_dataframe.py
--rw-r--r--   0        0        0    10203 2023-04-14 16:44:30.154892 tmlt_core-0.9.0/test/unit/measurements/pandas_measurements/test_series.py
--rw-r--r--   0        0        0    42343 2023-04-14 16:44:30.154892 tmlt_core-0.9.0/test/unit/measurements/test_aggregations.py
--rw-r--r--   0        0        0     7429 2023-04-14 16:44:30.154892 tmlt_core-0.9.0/test/unit/measurements/test_chaining.py
--rw-r--r--   0        0        0    17787 2023-04-14 16:44:30.154892 tmlt_core-0.9.0/test/unit/measurements/test_composition.py
--rw-r--r--   0        0        0     8003 2023-04-14 16:44:30.154892 tmlt_core-0.9.0/test/unit/measurements/test_converters.py
--rw-r--r--   0        0        0    80698 2023-04-14 16:44:30.155892 tmlt_core-0.9.0/test/unit/measurements/test_interactive_measurements.py
--rw-r--r--   0        0        0    13139 2023-04-14 16:44:30.155892 tmlt_core-0.9.0/test/unit/measurements/test_noise_mechanisms.py
--rw-r--r--   0        0        0     9458 2023-04-14 16:44:30.155892 tmlt_core-0.9.0/test/unit/measurements/test_postprocess.py
--rw-r--r--   0        0        0    17510 2023-04-14 16:44:30.155892 tmlt_core-0.9.0/test/unit/measurements/test_spark_measurements.py
--rw-r--r--   0        0        0      115 2023-04-14 16:44:30.155892 tmlt_core-0.9.0/test/unit/random/__init__.py
--rw-r--r--   0        0        0     1833 2023-04-14 16:44:30.155892 tmlt_core-0.9.0/test/unit/random/test_continuous_gaussian.py
--rw-r--r--   0        0        0     1235 2023-04-14 16:44:30.155892 tmlt_core-0.9.0/test/unit/random/test_discrete_gaussian.py
--rw-r--r--   0        0        0      707 2023-04-14 16:44:30.155892 tmlt_core-0.9.0/test/unit/random/test_inverse_cdf.py
--rw-r--r--   0        0        0     1957 2023-04-14 16:44:30.155892 tmlt_core-0.9.0/test/unit/random/test_laplace.py
--rw-r--r--   0        0        0     1590 2023-04-14 16:44:30.155892 tmlt_core-0.9.0/test/unit/random/test_rng.py
--rw-r--r--   0        0        0      753 2023-04-14 16:44:30.155892 tmlt_core-0.9.0/test/unit/random/test_uniform.py
--rw-r--r--   0        0        0    15212 2023-04-14 16:44:30.155892 tmlt_core-0.9.0/test/unit/test_measures.py
--rw-r--r--   0        0        0    91233 2023-04-14 16:44:30.155892 tmlt_core-0.9.0/test/unit/test_metrics.py
--rw-r--r--   0        0        0      124 2023-04-14 16:44:30.155892 tmlt_core-0.9.0/test/unit/transformations/__init__.py
--rw-r--r--   0        0        0      146 2023-04-14 16:44:30.155892 tmlt_core-0.9.0/test/unit/transformations/spark_transformations/__init__.py
--rw-r--r--   0        0        0    22382 2023-04-14 16:44:30.156892 tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_add_remove_keys.py
--rw-r--r--   0        0        0    37109 2023-04-14 16:44:30.156892 tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_agg.py
--rw-r--r--   0        0        0     4748 2023-04-14 16:44:30.156892 tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_filter.py
--rw-r--r--   0        0        0    16386 2023-04-14 16:44:30.156892 tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_groupby.py
--rw-r--r--   0        0        0     6832 2023-04-14 16:44:30.156892 tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_id.py
--rw-r--r--   0        0        0    50620 2023-04-14 16:44:30.156892 tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_join.py
--rw-r--r--   0        0        0    27295 2023-04-14 16:44:30.156892 tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_map.py
--rw-r--r--   0        0        0    34292 2023-04-14 16:44:30.156892 tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_nan.py
--rw-r--r--   0        0        0    12670 2023-04-14 16:44:30.156892 tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_partition.py
--rw-r--r--   0        0        0     3331 2023-04-14 16:44:30.156892 tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_persist.py
--rw-r--r--   0        0        0     6053 2023-04-14 16:44:30.157892 tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_rename.py
--rw-r--r--   0        0        0     4811 2023-04-14 16:44:30.157892 tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_select.py
--rw-r--r--   0        0        0    17751 2023-04-14 16:44:30.157892 tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_truncation.py
--rw-r--r--   0        0        0     8000 2023-04-14 16:44:30.157892 tmlt_core-0.9.0/test/unit/transformations/test_chaining.py
--rw-r--r--   0        0        0     3922 2023-04-14 16:44:30.157892 tmlt_core-0.9.0/test/unit/transformations/test_converters.py
--rw-r--r--   0        0        0    39837 2023-04-14 16:44:30.157892 tmlt_core-0.9.0/test/unit/transformations/test_dictionary.py
--rw-r--r--   0        0        0     1936 2023-04-14 16:44:30.157892 tmlt_core-0.9.0/test/unit/transformations/test_identity.py
--rw-r--r--   0        0        0      114 2023-04-14 16:44:30.157892 tmlt_core-0.9.0/test/unit/utils/__init__.py
--rw-r--r--   0        0        0     8396 2023-04-14 16:44:30.157892 tmlt_core-0.9.0/test/unit/utils/test_arb.py
--rw-r--r--   0        0        0     5700 2023-04-14 16:44:30.157892 tmlt_core-0.9.0/test/unit/utils/test_cleanup.py
--rw-r--r--   0        0        0    10005 2023-04-14 16:44:30.157892 tmlt_core-0.9.0/test/unit/utils/test_configuration.py
--rw-r--r--   0        0        0     8733 2023-04-14 16:44:30.157892 tmlt_core-0.9.0/test/unit/utils/test_distributions.py
--rw-r--r--   0        0        0     6032 2023-04-14 16:44:30.157892 tmlt_core-0.9.0/test/unit/utils/test_exact_number.py
--rw-r--r--   0        0        0    13458 2023-04-14 16:44:30.157892 tmlt_core-0.9.0/test/unit/utils/test_grouped_dataframe.py
--rw-r--r--   0        0        0    37873 2023-04-14 16:44:30.158892 tmlt_core-0.9.0/test/unit/utils/test_join.py
--rw-r--r--   0        0        0     2424 2023-04-14 16:44:30.158892 tmlt_core-0.9.0/test/unit/utils/test_misc.py
--rw-r--r--   0        0        0     1054 2023-04-14 16:44:30.158892 tmlt_core-0.9.0/test/unit/utils/test_testing.py
--rw-r--r--   0        0        0     4466 2023-04-14 16:44:30.158892 tmlt_core-0.9.0/test/unit/utils/test_truncation.py
--rw-r--r--   0        0        0     1837 2023-04-14 16:44:30.158892 tmlt_core-0.9.0/test/unit/utils/test_type_utils.py
--rw-r--r--   0        0        0       37 2023-04-14 16:44:30.158892 tmlt_core-0.9.0/test_requirements.txt
--rw-r--r--   0        0        0      376 2023-04-14 16:44:30.158892 tmlt_core-0.9.0/tmlt/core/__init__.py
--rw-r--r--   0        0        0       83 2023-04-14 16:44:30.158892 tmlt_core-0.9.0/tmlt/core/domains/__init__.py
--rw-r--r--   0        0        0      992 2023-04-14 16:44:30.158892 tmlt_core-0.9.0/tmlt/core/domains/base.py
--rw-r--r--   0        0        0     3425 2023-04-14 16:44:30.158892 tmlt_core-0.9.0/tmlt/core/domains/collections.py
--rw-r--r--   0        0        0     3926 2023-04-14 16:44:30.158892 tmlt_core-0.9.0/tmlt/core/domains/numpy_domains.py
--rw-r--r--   0        0        0     4489 2023-04-14 16:44:30.158892 tmlt_core-0.9.0/tmlt/core/domains/pandas_domains.py
--rw-r--r--   0        0        0    25759 2023-04-14 16:44:30.158892 tmlt_core-0.9.0/tmlt/core/domains/spark_domains.py
--rw-r--r--   0        0        0       88 2023-04-14 16:44:30.158892 tmlt_core-0.9.0/tmlt/core/measurements/__init__.py
--rw-r--r--   0        0        0    83528 2023-04-14 16:44:30.159892 tmlt_core-0.9.0/tmlt/core/measurements/aggregations.py
--rw-r--r--   0        0        0     2931 2023-04-14 16:44:30.159892 tmlt_core-0.9.0/tmlt/core/measurements/base.py
--rw-r--r--   0        0        0     5020 2023-04-14 16:44:30.159892 tmlt_core-0.9.0/tmlt/core/measurements/chaining.py
--rw-r--r--   0        0        0     6728 2023-04-14 16:44:30.159892 tmlt_core-0.9.0/tmlt/core/measurements/composition.py
--rw-r--r--   0        0        0     8463 2023-04-14 16:44:30.159892 tmlt_core-0.9.0/tmlt/core/measurements/converters.py
--rw-r--r--   0        0        0    73838 2023-04-14 16:44:30.159892 tmlt_core-0.9.0/tmlt/core/measurements/interactive_measurements.py
--rw-r--r--   0        0        0    17009 2023-04-14 16:44:30.159892 tmlt_core-0.9.0/tmlt/core/measurements/noise_mechanisms.py
--rw-r--r--   0        0        0      120 2023-04-14 16:44:30.159892 tmlt_core-0.9.0/tmlt/core/measurements/pandas_measurements/__init__.py
--rw-r--r--   0        0        0    10135 2023-04-14 16:44:30.159892 tmlt_core-0.9.0/tmlt/core/measurements/pandas_measurements/dataframe.py
--rw-r--r--   0        0        0    15934 2023-04-14 16:44:30.159892 tmlt_core-0.9.0/tmlt/core/measurements/pandas_measurements/series.py
--rw-r--r--   0        0        0     7411 2023-04-14 16:44:30.159892 tmlt_core-0.9.0/tmlt/core/measurements/postprocess.py
--rw-r--r--   0        0        0    22812 2023-04-14 16:44:30.160892 tmlt_core-0.9.0/tmlt/core/measurements/spark_measurements.py
--rw-r--r--   0        0        0    13254 2023-04-14 16:44:30.160892 tmlt_core-0.9.0/tmlt/core/measures.py
--rw-r--r--   0        0        0    54917 2023-04-14 16:44:30.160892 tmlt_core-0.9.0/tmlt/core/metrics.py
--rw-r--r--   0        0        0        0 2023-04-14 16:44:30.160892 tmlt_core-0.9.0/tmlt/core/py.typed
--rw-r--r--   0        0        0      119 2023-04-14 16:44:30.160892 tmlt_core-0.9.0/tmlt/core/random/__init__.py
--rw-r--r--   0        0        0     2551 2023-04-14 16:44:30.160892 tmlt_core-0.9.0/tmlt/core/random/continuous_gaussian.py
--rw-r--r--   0        0        0    16941 2023-04-14 16:44:30.160892 tmlt_core-0.9.0/tmlt/core/random/discrete_gaussian.py
--rw-r--r--   0        0        0     1497 2023-04-14 16:44:30.160892 tmlt_core-0.9.0/tmlt/core/random/inverse_cdf.py
--rw-r--r--   0        0        0     2132 2023-04-14 16:44:30.160892 tmlt_core-0.9.0/tmlt/core/random/laplace.py
--rw-r--r--   0        0        0      619 2023-04-14 16:44:30.160892 tmlt_core-0.9.0/tmlt/core/random/rng.py
--rw-r--r--   0        0        0     1673 2023-04-14 16:44:30.160892 tmlt_core-0.9.0/tmlt/core/random/uniform.py
--rw-r--r--   0        0        0       91 2023-04-14 16:44:30.160892 tmlt_core-0.9.0/tmlt/core/transformations/__init__.py
--rw-r--r--   0        0        0     4029 2023-04-14 16:44:30.160892 tmlt_core-0.9.0/tmlt/core/transformations/base.py
--rw-r--r--   0        0        0     4653 2023-04-14 16:44:30.160892 tmlt_core-0.9.0/tmlt/core/transformations/chaining.py
--rw-r--r--   0        0        0     3277 2023-04-14 16:44:30.161892 tmlt_core-0.9.0/tmlt/core/transformations/converters.py
--rw-r--r--   0        0        0    27820 2023-04-14 16:44:30.161892 tmlt_core-0.9.0/tmlt/core/transformations/dictionary.py
--rw-r--r--   0        0        0     1160 2023-04-14 16:44:30.161892 tmlt_core-0.9.0/tmlt/core/transformations/identity.py
--rw-r--r--   0        0        0      125 2023-04-14 16:44:30.161892 tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/__init__.py
--rw-r--r--   0        0        0    34915 2023-04-14 16:44:30.161892 tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/add_remove_keys.py
--rw-r--r--   0        0        0    44303 2023-04-14 16:44:30.161892 tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/agg.py
--rw-r--r--   0        0        0     5860 2023-04-14 16:44:30.161892 tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/filter.py
--rw-r--r--   0        0        0    16865 2023-04-14 16:44:30.161892 tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/groupby.py
--rw-r--r--   0        0        0     5680 2023-04-14 16:44:30.161892 tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/id.py
--rw-r--r--   0        0        0    39943 2023-04-14 16:44:30.162892 tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/join.py
--rw-r--r--   0        0        0    40011 2023-04-14 16:44:30.162892 tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/map.py
--rw-r--r--   0        0        0    40713 2023-04-14 16:44:30.162892 tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/nan.py
--rw-r--r--   0        0        0     9724 2023-04-14 16:44:30.162892 tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/partition.py
--rw-r--r--   0        0        0     3862 2023-04-14 16:44:30.162892 tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/persist.py
--rw-r--r--   0        0        0     6769 2023-04-14 16:44:30.162892 tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/rename.py
--rw-r--r--   0        0        0     5800 2023-04-14 16:44:30.162892 tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/select.py
--rw-r--r--   0        0        0    22134 2023-04-14 16:44:30.162892 tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/truncation.py
--rw-r--r--   0        0        0       85 2023-04-14 16:44:30.162892 tmlt_core-0.9.0/tmlt/core/utils/__init__.py
--rw-r--r--   0        0        0    16349 2023-04-14 16:44:30.163892 tmlt_core-0.9.0/tmlt/core/utils/arb.py
--rw-r--r--   0        0        0     1181 2023-04-14 16:44:30.163892 tmlt_core-0.9.0/tmlt/core/utils/cleanup.py
--rw-r--r--   0        0        0     6030 2023-04-14 16:44:30.163892 tmlt_core-0.9.0/tmlt/core/utils/configuration.py
--rw-r--r--   0        0        0     9303 2023-04-14 16:44:30.163892 tmlt_core-0.9.0/tmlt/core/utils/distributions.py
--rw-r--r--   0        0        0    15026 2023-04-14 16:44:30.163892 tmlt_core-0.9.0/tmlt/core/utils/exact_number.py
--rw-r--r--   0        0        0     9403 2023-04-14 16:44:30.163892 tmlt_core-0.9.0/tmlt/core/utils/grouped_dataframe.py
--rw-r--r--   0        0        0    20371 2023-04-14 16:44:30.163892 tmlt_core-0.9.0/tmlt/core/utils/join.py
--rw-r--r--   0        0        0     3190 2023-04-14 16:44:30.163892 tmlt_core-0.9.0/tmlt/core/utils/misc.py
--rw-r--r--   0        0        0     3551 2023-04-14 16:44:30.163892 tmlt_core-0.9.0/tmlt/core/utils/parameters.py
--rw-r--r--   0        0        0    32413 2023-04-14 16:44:30.163892 tmlt_core-0.9.0/tmlt/core/utils/testing.py
--rw-r--r--   0        0        0     7707 2023-04-14 16:44:30.163892 tmlt_core-0.9.0/tmlt/core/utils/truncation.py
--rw-r--r--   0        0        0     2796 2023-04-14 16:44:30.163892 tmlt_core-0.9.0/tmlt/core/utils/type_utils.py
--rw-r--r--   0        0        0     6215 2023-04-14 16:44:30.163892 tmlt_core-0.9.0/tmlt/core/utils/validation.py
--rw-r--r--   0        0        0     3195 1970-01-01 00:00:00.000000 tmlt_core-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    10213 2023-04-20 16:47:33.903353 tmlt_core-0.9.1/CHANGELOG.rst
+-rw-r--r--   0        0        0    11358 2023-04-20 16:47:33.903353 tmlt_core-0.9.1/LICENSE
+-rw-r--r--   0        0        0    20138 2023-04-20 16:47:33.903353 tmlt_core-0.9.1/LICENSE.docs
+-rw-r--r--   0        0        0      116 2023-04-20 16:47:33.903353 tmlt_core-0.9.1/NOTICE
+-rw-r--r--   0        0        0     1868 2023-04-20 16:47:33.903353 tmlt_core-0.9.1/README.md
+-rw-r--r--   0        0        0    11481 2023-04-20 16:47:33.903353 tmlt_core-0.9.1/benchmark/benchmark_count_sum.py
+-rw-r--r--   0        0        0     3838 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/benchmark/benchmark_noise_mechanism.py
+-rw-r--r--   0        0        0     8652 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/benchmark/benchmark_private_join.py
+-rw-r--r--   0        0        0    15676 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/benchmark/benchmark_public_join.py
+-rw-r--r--   0        0        0     8873 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/benchmark/benchmark_quantile.py
+-rw-r--r--   0        0        0    10207 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/benchmark/benchmark_sparkflatmap.py
+-rw-r--r--   0        0        0     9446 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/benchmark/benchmark_sparkmap.py
+-rw-r--r--   0        0        0      731 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/benchmark/benchmarking_utils.py
+-rw-r--r--   0        0        0      951 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/doc/_static/css/custom.css
+-rw-r--r--   0        0        0    12470 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/doc/_static/favicon.ico
+-rw-r--r--   0        0        0     1001 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/doc/_static/js/version-banner.js
+-rw-r--r--   0        0        0    30903 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/doc/_static/logo.png
+-rw-r--r--   0        0        0       50 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/doc/_templates/build-info.html
+-rw-r--r--   0        0        0      408 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/doc/_templates/layout.html
+-rw-r--r--   0        0        0       23 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/doc/_templates/package-name.html
+-rw-r--r--   0        0        0      210 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/doc/additional-resources/index.rst
+-rw-r--r--   0        0        0      660 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/doc/additional-resources/license.rst
+-rw-r--r--   0        0        0     3159 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/doc/additional-resources/privacy_policy.rst
+-rw-r--r--   0        0        0     6889 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/conf.py
+-rw-r--r--   0        0        0     1836 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/images/index_api.svg
+-rw-r--r--   0        0        0     1186 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/images/index_more.svg
+-rw-r--r--   0        0        0      596 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/images/index_topic_guides.svg
+-rw-r--r--   0        0        0     1363 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/images/index_tutorials.svg
+-rw-r--r--   0        0        0    30903 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/images/logo.png
+-rw-r--r--   0        0        0     3186 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/index.rst
+-rw-r--r--   0        0        0     4541 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/installation.rst
+-rw-r--r--   0        0        0     8472 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/ref.bib
+-rw-r--r--   0        0        0     2006 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/templates/python/class.rst
+-rw-r--r--   0        0        0     3244 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/templates/python/module.rst
+-rw-r--r--   0        0        0    16713 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/topic-guides/architecture.rst
+-rw-r--r--   0        0        0      345 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/topic-guides/index.rst
+-rw-r--r--   0        0        0     1424 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/topic-guides/known-vulnerabilities.rst
+-rw-r--r--   0        0        0     6510 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/topic-guides/privacy-guarantee.rst
+-rw-r--r--   0        0        0     2289 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/topic-guides/real-numbers.rst
+-rw-r--r--   0        0        0     6151 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/topic-guides/spark.rst
+-rw-r--r--   0        0        0     8100 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/topic-guides/special-values.rst
+-rw-r--r--   0        0        0     7334 2023-04-20 16:47:33.906353 tmlt_core-0.9.1/doc/tutorials/first-tutorial.rst
+-rw-r--r--   0        0        0      231 2023-04-20 16:47:33.906353 tmlt_core-0.9.1/doc/tutorials/index.rst
+-rw-r--r--   0        0        0       88 2023-04-20 16:47:33.906353 tmlt_core-0.9.1/doc/zcitations.rst
+-rw-r--r--   0        0        0      363 2023-04-20 16:47:33.906353 tmlt_core-0.9.1/ext/build.py
+-rw-r--r--   0        0        0     3175 2023-04-20 16:47:33.906353 tmlt_core-0.9.1/ext/build.sh
+-rw-r--r--   0        0        0      150 2023-04-20 16:47:33.906353 tmlt_core-0.9.1/ext/dependency_versions.sh
+-rw-r--r--   0        0        0     4909 2023-04-20 16:48:10.329370 tmlt_core-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      103 2023-04-20 16:47:33.906353 tmlt_core-0.9.1/test/__init__.py
+-rw-r--r--   0        0        0      110 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/system/__init__.py
+-rw-r--r--   0        0        0     3889 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/system/measurements/test_interactive_measurements.py
+-rw-r--r--   0        0        0      654 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/system/noise_distribution_tests/__init__.py
+-rw-r--r--   0        0        0     5468 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/system/noise_distribution_tests/test_average.py
+-rw-r--r--   0        0        0    11426 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/system/noise_distribution_tests/test_base_mechanisms.py
+-rw-r--r--   0        0        0     4671 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/system/noise_distribution_tests/test_count.py
+-rw-r--r--   0        0        0     4849 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/system/noise_distribution_tests/test_count_distinct.py
+-rw-r--r--   0        0        0     5670 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/system/noise_distribution_tests/test_quantile.py
+-rw-r--r--   0        0        0      844 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/system/noise_distribution_tests/test_samplers.py
+-rw-r--r--   0        0        0     6706 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/system/noise_distribution_tests/test_standard_deviation.py
+-rw-r--r--   0        0        0     5197 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/system/noise_distribution_tests/test_sum.py
+-rw-r--r--   0        0        0     7067 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/system/noise_distribution_tests/test_variance.py
+-rw-r--r--   0        0        0      108 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/unit/__init__.py
+-rw-r--r--   0        0        0      116 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/unit/domains/__init__.py
+-rw-r--r--   0        0        0     1176 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/unit/domains/test_base.py
+-rw-r--r--   0        0        0     6558 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/unit/domains/test_collections.py
+-rw-r--r--   0        0        0     8866 2023-04-20 16:47:33.908353 tmlt_core-0.9.1/test/unit/domains/test_numpy_domains.py
+-rw-r--r--   0        0        0     9857 2023-04-20 16:47:33.908353 tmlt_core-0.9.1/test/unit/domains/test_pandas_domains.py
+-rw-r--r--   0        0        0    26425 2023-04-20 16:47:33.908353 tmlt_core-0.9.1/test/unit/domains/test_spark_domains.py
+-rw-r--r--   0        0        0      121 2023-04-20 16:47:33.908353 tmlt_core-0.9.1/test/unit/measurements/__init__.py
+-rw-r--r--   0        0        0      141 2023-04-20 16:47:33.908353 tmlt_core-0.9.1/test/unit/measurements/pandas_measurements/__init__.py
+-rw-r--r--   0        0        0    13818 2023-04-20 16:47:33.908353 tmlt_core-0.9.1/test/unit/measurements/pandas_measurements/test_dataframe.py
+-rw-r--r--   0        0        0    10203 2023-04-20 16:47:33.908353 tmlt_core-0.9.1/test/unit/measurements/pandas_measurements/test_series.py
+-rw-r--r--   0        0        0    42343 2023-04-20 16:47:33.908353 tmlt_core-0.9.1/test/unit/measurements/test_aggregations.py
+-rw-r--r--   0        0        0     7429 2023-04-20 16:47:33.908353 tmlt_core-0.9.1/test/unit/measurements/test_chaining.py
+-rw-r--r--   0        0        0    17787 2023-04-20 16:47:33.908353 tmlt_core-0.9.1/test/unit/measurements/test_composition.py
+-rw-r--r--   0        0        0     8003 2023-04-20 16:47:33.908353 tmlt_core-0.9.1/test/unit/measurements/test_converters.py
+-rw-r--r--   0        0        0    80698 2023-04-20 16:47:33.908353 tmlt_core-0.9.1/test/unit/measurements/test_interactive_measurements.py
+-rw-r--r--   0        0        0    13139 2023-04-20 16:47:33.908353 tmlt_core-0.9.1/test/unit/measurements/test_noise_mechanisms.py
+-rw-r--r--   0        0        0     9458 2023-04-20 16:47:33.908353 tmlt_core-0.9.1/test/unit/measurements/test_postprocess.py
+-rw-r--r--   0        0        0    17510 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/measurements/test_spark_measurements.py
+-rw-r--r--   0        0        0      115 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/random/__init__.py
+-rw-r--r--   0        0        0     1833 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/random/test_continuous_gaussian.py
+-rw-r--r--   0        0        0     1235 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/random/test_discrete_gaussian.py
+-rw-r--r--   0        0        0      707 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/random/test_inverse_cdf.py
+-rw-r--r--   0        0        0     1957 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/random/test_laplace.py
+-rw-r--r--   0        0        0     1590 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/random/test_rng.py
+-rw-r--r--   0        0        0      753 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/random/test_uniform.py
+-rw-r--r--   0        0        0    15212 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/test_measures.py
+-rw-r--r--   0        0        0    91233 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/test_metrics.py
+-rw-r--r--   0        0        0      124 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/transformations/__init__.py
+-rw-r--r--   0        0        0      146 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/transformations/spark_transformations/__init__.py
+-rw-r--r--   0        0        0    22382 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_add_remove_keys.py
+-rw-r--r--   0        0        0    37109 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_agg.py
+-rw-r--r--   0        0        0     4748 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_filter.py
+-rw-r--r--   0        0        0    16386 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_groupby.py
+-rw-r--r--   0        0        0     6832 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_id.py
+-rw-r--r--   0        0        0    50620 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_join.py
+-rw-r--r--   0        0        0    27295 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_map.py
+-rw-r--r--   0        0        0    34292 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_nan.py
+-rw-r--r--   0        0        0    12670 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_partition.py
+-rw-r--r--   0        0        0     3331 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_persist.py
+-rw-r--r--   0        0        0     6053 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_rename.py
+-rw-r--r--   0        0        0     4811 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_select.py
+-rw-r--r--   0        0        0    17751 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_truncation.py
+-rw-r--r--   0        0        0     8000 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/transformations/test_chaining.py
+-rw-r--r--   0        0        0     3922 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/transformations/test_converters.py
+-rw-r--r--   0        0        0    39837 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/transformations/test_dictionary.py
+-rw-r--r--   0        0        0     1936 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/transformations/test_identity.py
+-rw-r--r--   0        0        0      114 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/utils/__init__.py
+-rw-r--r--   0        0        0     8396 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/utils/test_arb.py
+-rw-r--r--   0        0        0     5700 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/utils/test_cleanup.py
+-rw-r--r--   0        0        0    10005 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/utils/test_configuration.py
+-rw-r--r--   0        0        0     8733 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/test/unit/utils/test_distributions.py
+-rw-r--r--   0        0        0     6032 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/test/unit/utils/test_exact_number.py
+-rw-r--r--   0        0        0    13458 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/test/unit/utils/test_grouped_dataframe.py
+-rw-r--r--   0        0        0    37873 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/test/unit/utils/test_join.py
+-rw-r--r--   0        0        0     2424 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/test/unit/utils/test_misc.py
+-rw-r--r--   0        0        0     1054 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/test/unit/utils/test_testing.py
+-rw-r--r--   0        0        0     4466 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/test/unit/utils/test_truncation.py
+-rw-r--r--   0        0        0     1837 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/test/unit/utils/test_type_utils.py
+-rw-r--r--   0        0        0       37 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/test_requirements.txt
+-rw-r--r--   0        0        0      376 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/tmlt/core/__init__.py
+-rw-r--r--   0        0        0       83 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/tmlt/core/domains/__init__.py
+-rw-r--r--   0        0        0      992 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/tmlt/core/domains/base.py
+-rw-r--r--   0        0        0     3425 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/tmlt/core/domains/collections.py
+-rw-r--r--   0        0        0     3926 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/tmlt/core/domains/numpy_domains.py
+-rw-r--r--   0        0        0     4489 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/tmlt/core/domains/pandas_domains.py
+-rw-r--r--   0        0        0    25759 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/tmlt/core/domains/spark_domains.py
+-rw-r--r--   0        0        0       88 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/tmlt/core/measurements/__init__.py
+-rw-r--r--   0        0        0    83528 2023-04-20 16:47:33.912353 tmlt_core-0.9.1/tmlt/core/measurements/aggregations.py
+-rw-r--r--   0        0        0     2931 2023-04-20 16:47:33.912353 tmlt_core-0.9.1/tmlt/core/measurements/base.py
+-rw-r--r--   0        0        0     5020 2023-04-20 16:47:33.912353 tmlt_core-0.9.1/tmlt/core/measurements/chaining.py
+-rw-r--r--   0        0        0     6728 2023-04-20 16:47:33.912353 tmlt_core-0.9.1/tmlt/core/measurements/composition.py
+-rw-r--r--   0        0        0     8463 2023-04-20 16:47:33.912353 tmlt_core-0.9.1/tmlt/core/measurements/converters.py
+-rw-r--r--   0        0        0    73838 2023-04-20 16:47:33.912353 tmlt_core-0.9.1/tmlt/core/measurements/interactive_measurements.py
+-rw-r--r--   0        0        0    17009 2023-04-20 16:47:33.912353 tmlt_core-0.9.1/tmlt/core/measurements/noise_mechanisms.py
+-rw-r--r--   0        0        0      120 2023-04-20 16:47:33.912353 tmlt_core-0.9.1/tmlt/core/measurements/pandas_measurements/__init__.py
+-rw-r--r--   0        0        0    10135 2023-04-20 16:47:33.912353 tmlt_core-0.9.1/tmlt/core/measurements/pandas_measurements/dataframe.py
+-rw-r--r--   0        0        0    15934 2023-04-20 16:47:33.912353 tmlt_core-0.9.1/tmlt/core/measurements/pandas_measurements/series.py
+-rw-r--r--   0        0        0     7411 2023-04-20 16:47:33.912353 tmlt_core-0.9.1/tmlt/core/measurements/postprocess.py
+-rw-r--r--   0        0        0    22812 2023-04-20 16:47:33.912353 tmlt_core-0.9.1/tmlt/core/measurements/spark_measurements.py
+-rw-r--r--   0        0        0    14858 2023-04-20 16:47:33.912353 tmlt_core-0.9.1/tmlt/core/measures.py
+-rw-r--r--   0        0        0    54917 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/metrics.py
+-rw-r--r--   0        0        0        0 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/py.typed
+-rw-r--r--   0        0        0      119 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/random/__init__.py
+-rw-r--r--   0        0        0     2551 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/random/continuous_gaussian.py
+-rw-r--r--   0        0        0    16941 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/random/discrete_gaussian.py
+-rw-r--r--   0        0        0     1497 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/random/inverse_cdf.py
+-rw-r--r--   0        0        0     2132 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/random/laplace.py
+-rw-r--r--   0        0        0      619 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/random/rng.py
+-rw-r--r--   0        0        0     1673 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/random/uniform.py
+-rw-r--r--   0        0        0       91 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/transformations/__init__.py
+-rw-r--r--   0        0        0     4029 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/transformations/base.py
+-rw-r--r--   0        0        0     4653 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/transformations/chaining.py
+-rw-r--r--   0        0        0     3277 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/transformations/converters.py
+-rw-r--r--   0        0        0    27820 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/transformations/dictionary.py
+-rw-r--r--   0        0        0     1160 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/transformations/identity.py
+-rw-r--r--   0        0        0      125 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/__init__.py
+-rw-r--r--   0        0        0    34915 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/add_remove_keys.py
+-rw-r--r--   0        0        0    44303 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/agg.py
+-rw-r--r--   0        0        0     5860 2023-04-20 16:47:33.914353 tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/filter.py
+-rw-r--r--   0        0        0    16865 2023-04-20 16:47:33.914353 tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/groupby.py
+-rw-r--r--   0        0        0     5680 2023-04-20 16:47:33.914353 tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/id.py
+-rw-r--r--   0        0        0    39943 2023-04-20 16:47:33.914353 tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/join.py
+-rw-r--r--   0        0        0    40011 2023-04-20 16:47:33.914353 tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/map.py
+-rw-r--r--   0        0        0    40713 2023-04-20 16:47:33.914353 tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/nan.py
+-rw-r--r--   0        0        0     9724 2023-04-20 16:47:33.914353 tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/partition.py
+-rw-r--r--   0        0        0     3862 2023-04-20 16:47:33.914353 tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/persist.py
+-rw-r--r--   0        0        0     6769 2023-04-20 16:47:33.914353 tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/rename.py
+-rw-r--r--   0        0        0     5800 2023-04-20 16:47:33.914353 tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/select.py
+-rw-r--r--   0        0        0    22134 2023-04-20 16:47:33.914353 tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/truncation.py
+-rw-r--r--   0        0        0       85 2023-04-20 16:47:33.914353 tmlt_core-0.9.1/tmlt/core/utils/__init__.py
+-rw-r--r--   0        0        0    16349 2023-04-20 16:47:33.915353 tmlt_core-0.9.1/tmlt/core/utils/arb.py
+-rw-r--r--   0        0        0     1181 2023-04-20 16:47:33.915353 tmlt_core-0.9.1/tmlt/core/utils/cleanup.py
+-rw-r--r--   0        0        0     6030 2023-04-20 16:47:33.915353 tmlt_core-0.9.1/tmlt/core/utils/configuration.py
+-rw-r--r--   0        0        0     9303 2023-04-20 16:47:33.915353 tmlt_core-0.9.1/tmlt/core/utils/distributions.py
+-rw-r--r--   0        0        0    15026 2023-04-20 16:47:33.915353 tmlt_core-0.9.1/tmlt/core/utils/exact_number.py
+-rw-r--r--   0        0        0     9403 2023-04-20 16:47:33.915353 tmlt_core-0.9.1/tmlt/core/utils/grouped_dataframe.py
+-rw-r--r--   0        0        0    20371 2023-04-20 16:47:33.915353 tmlt_core-0.9.1/tmlt/core/utils/join.py
+-rw-r--r--   0        0        0     3190 2023-04-20 16:47:33.915353 tmlt_core-0.9.1/tmlt/core/utils/misc.py
+-rw-r--r--   0        0        0     3551 2023-04-20 16:47:33.915353 tmlt_core-0.9.1/tmlt/core/utils/parameters.py
+-rw-r--r--   0        0        0    32413 2023-04-20 16:47:33.915353 tmlt_core-0.9.1/tmlt/core/utils/testing.py
+-rw-r--r--   0        0        0     7707 2023-04-20 16:47:33.915353 tmlt_core-0.9.1/tmlt/core/utils/truncation.py
+-rw-r--r--   0        0        0     2796 2023-04-20 16:47:33.915353 tmlt_core-0.9.1/tmlt/core/utils/type_utils.py
+-rw-r--r--   0        0        0     6215 2023-04-20 16:47:33.915353 tmlt_core-0.9.1/tmlt/core/utils/validation.py
+-rw-r--r--   0        0        0     3195 1970-01-01 00:00:00.000000 tmlt_core-0.9.1/PKG-INFO
```

### Comparing `tmlt_core-0.9.0/CHANGELOG.rst` & `tmlt_core-0.9.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 .. _core-changelog:
 
 Changelog
 =========
 
+0.9.1 - 2023-04-20
+------------------
+
+Added
+~~~~~
+- Subclasses of :class:`~.Measure` now have equations defining the distance they represent.
+
 0.9.0 - 2023-04-14
 ------------------
 
 Added
 ~~~~~
 
 - :mod:`~.utils.join`, which contains utilities for validating join parameters, propogating domains through joins, and joining dataframes.
```

### Comparing `tmlt_core-0.9.0/LICENSE` & `tmlt_core-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/LICENSE.docs` & `tmlt_core-0.9.1/LICENSE.docs`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/README.md` & `tmlt_core-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/benchmark/benchmark_count_sum.py` & `tmlt_core-0.9.1/benchmark/benchmark_count_sum.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/benchmark/benchmark_noise_mechanism.py` & `tmlt_core-0.9.1/benchmark/benchmark_noise_mechanism.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/benchmark/benchmark_private_join.py` & `tmlt_core-0.9.1/benchmark/benchmark_private_join.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/benchmark/benchmark_public_join.py` & `tmlt_core-0.9.1/benchmark/benchmark_public_join.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/benchmark/benchmark_quantile.py` & `tmlt_core-0.9.1/benchmark/benchmark_quantile.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/benchmark/benchmark_sparkflatmap.py` & `tmlt_core-0.9.1/benchmark/benchmark_sparkflatmap.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/benchmark/benchmark_sparkmap.py` & `tmlt_core-0.9.1/benchmark/benchmark_sparkmap.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/benchmark/benchmarking_utils.py` & `tmlt_core-0.9.1/benchmark/benchmarking_utils.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/doc/_static/css/custom.css` & `tmlt_core-0.9.1/doc/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/doc/_static/favicon.ico` & `tmlt_core-0.9.1/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/doc/_static/js/version-banner.js` & `tmlt_core-0.9.1/doc/_static/js/version-banner.js`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/doc/_static/logo.png` & `tmlt_core-0.9.1/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/doc/additional-resources/license.rst` & `tmlt_core-0.9.1/doc/additional-resources/license.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/doc/additional-resources/privacy_policy.rst` & `tmlt_core-0.9.1/doc/additional-resources/privacy_policy.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/doc/conf.py` & `tmlt_core-0.9.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/doc/images/index_api.svg` & `tmlt_core-0.9.1/doc/images/index_api.svg`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/doc/images/index_more.svg` & `tmlt_core-0.9.1/doc/images/index_more.svg`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/doc/images/index_topic_guides.svg` & `tmlt_core-0.9.1/doc/images/index_topic_guides.svg`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/doc/images/index_tutorials.svg` & `tmlt_core-0.9.1/doc/images/index_tutorials.svg`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/doc/images/logo.png` & `tmlt_core-0.9.1/doc/images/logo.png`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/doc/index.rst` & `tmlt_core-0.9.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/doc/installation.rst` & `tmlt_core-0.9.1/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/doc/ref.bib` & `tmlt_core-0.9.1/doc/ref.bib`

 * *Files 15% similar despite different names*

```diff
@@ -153,7 +153,52 @@
   pages     = {1921--1929},
   year      = {2016},
   url       = {https://proceedings.neurips.cc/paper/2016/hash/58c54802a9fb9526cd0923353a34a7ae-Abstract.html},
   timestamp = {Mon, 16 May 2022 15:41:51 +0200},
   biburl    = {https://dblp.org/rec/conf/nips/RogersVRU16.bib},
   bibsource = {dblp computer science bibliography, https://dblp.org}
 }
+
+@inproceedings{DworkKMMN06,
+  author       = {Cynthia Dwork and
+                  Krishnaram Kenthapadi and
+                  Frank McSherry and
+                  Ilya Mironov and
+                  Moni Naor},
+  editor       = {Serge Vaudenay},
+  title        = {Our Data, Ourselves: Privacy Via Distributed Noise Generation},
+  booktitle    = {Advances in Cryptology - {EUROCRYPT} 2006, 25th Annual International
+                  Conference on the Theory and Applications of Cryptographic Techniques,
+                  St. Petersburg, Russia, May 28 - June 1, 2006, Proceedings},
+  series       = {Lecture Notes in Computer Science},
+  volume       = {4004},
+  pages        = {486--503},
+  publisher    = {Springer},
+  year         = {2006},
+  url          = {https://doi.org/10.1007/11761679_29},
+  doi          = {10.1007/11761679_29},
+  timestamp    = {Tue, 14 May 2019 10:00:53 +0200},
+  biburl       = {https://dblp.org/rec/conf/eurocrypt/DworkKMMN06.bib},
+  bibsource    = {dblp computer science bibliography, https://dblp.org}
+}
+
+@inproceedings{DworkMNS06,
+  author       = {Cynthia Dwork and
+                  Frank McSherry and
+                  Kobbi Nissim and
+                  Adam D. Smith},
+  editor       = {Shai Halevi and
+                  Tal Rabin},
+  title        = {Calibrating Noise to Sensitivity in Private Data Analysis},
+  booktitle    = {Theory of Cryptography, Third Theory of Cryptography Conference, {TCC}
+                  2006, New York, NY, USA, March 4-7, 2006, Proceedings},
+  series       = {Lecture Notes in Computer Science},
+  volume       = {3876},
+  pages        = {265--284},
+  publisher    = {Springer},
+  year         = {2006},
+  url          = {https://doi.org/10.1007/11681878_14},
+  doi          = {10.1007/11681878_14},
+  timestamp    = {Tue, 14 May 2019 10:00:47 +0200},
+  biburl       = {https://dblp.org/rec/conf/tcc/DworkMNS06.bib},
+  bibsource    = {dblp computer science bibliography, https://dblp.org}
+}
```

### Comparing `tmlt_core-0.9.0/doc/templates/python/class.rst` & `tmlt_core-0.9.1/doc/templates/python/class.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/doc/templates/python/module.rst` & `tmlt_core-0.9.1/doc/templates/python/module.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/doc/topic-guides/architecture.rst` & `tmlt_core-0.9.1/doc/topic-guides/architecture.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/doc/topic-guides/known-vulnerabilities.rst` & `tmlt_core-0.9.1/doc/topic-guides/known-vulnerabilities.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/doc/topic-guides/privacy-guarantee.rst` & `tmlt_core-0.9.1/doc/topic-guides/privacy-guarantee.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/doc/topic-guides/real-numbers.rst` & `tmlt_core-0.9.1/doc/topic-guides/real-numbers.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/doc/topic-guides/spark.rst` & `tmlt_core-0.9.1/doc/topic-guides/spark.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/doc/topic-guides/special-values.rst` & `tmlt_core-0.9.1/doc/topic-guides/special-values.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/doc/tutorials/first-tutorial.rst` & `tmlt_core-0.9.1/doc/tutorials/first-tutorial.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/ext/build.sh` & `tmlt_core-0.9.1/ext/build.sh`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/pyproject.toml` & `tmlt_core-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "Tumult's differential privacy primitives"
 readme = "README.md"
 authors = []
 license = "Apache-2.0"
 repository = "https://gitlab.com/tumult-labs/core"
 documentation = "https://docs.tmlt.dev/core/latest"
 # The version field is required in this file format, even though it's ignored because of poetry-dynamic-versioning.
-version = "0.9.0"
+version = "0.9.1"
 
 classifiers = [
    "Development Status :: 4 - Beta",
    "Intended Audience :: Developers",
    "Intended Audience :: Science/Research",
    "Natural Language :: English",
    "Topic :: Software Development :: Libraries",
```

### Comparing `tmlt_core-0.9.0/test/system/measurements/test_interactive_measurements.py` & `tmlt_core-0.9.1/test/system/measurements/test_interactive_measurements.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/system/noise_distribution_tests/__init__.py` & `tmlt_core-0.9.1/test/system/noise_distribution_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/system/noise_distribution_tests/test_average.py` & `tmlt_core-0.9.1/test/system/noise_distribution_tests/test_average.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/system/noise_distribution_tests/test_base_mechanisms.py` & `tmlt_core-0.9.1/test/system/noise_distribution_tests/test_base_mechanisms.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/system/noise_distribution_tests/test_count.py` & `tmlt_core-0.9.1/test/system/noise_distribution_tests/test_count.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/system/noise_distribution_tests/test_count_distinct.py` & `tmlt_core-0.9.1/test/system/noise_distribution_tests/test_count_distinct.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/system/noise_distribution_tests/test_quantile.py` & `tmlt_core-0.9.1/test/system/noise_distribution_tests/test_quantile.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/system/noise_distribution_tests/test_samplers.py` & `tmlt_core-0.9.1/test/system/noise_distribution_tests/test_samplers.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/system/noise_distribution_tests/test_standard_deviation.py` & `tmlt_core-0.9.1/test/system/noise_distribution_tests/test_standard_deviation.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/system/noise_distribution_tests/test_sum.py` & `tmlt_core-0.9.1/test/system/noise_distribution_tests/test_sum.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/system/noise_distribution_tests/test_variance.py` & `tmlt_core-0.9.1/test/system/noise_distribution_tests/test_variance.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/domains/test_base.py` & `tmlt_core-0.9.1/test/unit/domains/test_base.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/domains/test_collections.py` & `tmlt_core-0.9.1/test/unit/domains/test_collections.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/domains/test_numpy_domains.py` & `tmlt_core-0.9.1/test/unit/domains/test_numpy_domains.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/domains/test_pandas_domains.py` & `tmlt_core-0.9.1/test/unit/domains/test_pandas_domains.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/domains/test_spark_domains.py` & `tmlt_core-0.9.1/test/unit/domains/test_spark_domains.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/measurements/pandas_measurements/test_dataframe.py` & `tmlt_core-0.9.1/test/unit/measurements/pandas_measurements/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/measurements/pandas_measurements/test_series.py` & `tmlt_core-0.9.1/test/unit/measurements/pandas_measurements/test_series.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/measurements/test_aggregations.py` & `tmlt_core-0.9.1/test/unit/measurements/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/measurements/test_chaining.py` & `tmlt_core-0.9.1/test/unit/measurements/test_chaining.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/measurements/test_composition.py` & `tmlt_core-0.9.1/test/unit/measurements/test_composition.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/measurements/test_converters.py` & `tmlt_core-0.9.1/test/unit/measurements/test_converters.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/measurements/test_interactive_measurements.py` & `tmlt_core-0.9.1/test/unit/measurements/test_interactive_measurements.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/measurements/test_noise_mechanisms.py` & `tmlt_core-0.9.1/test/unit/measurements/test_noise_mechanisms.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/measurements/test_postprocess.py` & `tmlt_core-0.9.1/test/unit/measurements/test_postprocess.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/measurements/test_spark_measurements.py` & `tmlt_core-0.9.1/test/unit/measurements/test_spark_measurements.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/random/test_continuous_gaussian.py` & `tmlt_core-0.9.1/test/unit/random/test_continuous_gaussian.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/random/test_discrete_gaussian.py` & `tmlt_core-0.9.1/test/unit/random/test_discrete_gaussian.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/random/test_inverse_cdf.py` & `tmlt_core-0.9.1/test/unit/random/test_inverse_cdf.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/random/test_laplace.py` & `tmlt_core-0.9.1/test/unit/random/test_laplace.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/random/test_rng.py` & `tmlt_core-0.9.1/test/unit/random/test_rng.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/random/test_uniform.py` & `tmlt_core-0.9.1/test/unit/random/test_uniform.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/test_measures.py` & `tmlt_core-0.9.1/test/unit/test_measures.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/test_metrics.py` & `tmlt_core-0.9.1/test/unit/test_metrics.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_add_remove_keys.py` & `tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_add_remove_keys.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_agg.py` & `tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_agg.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_filter.py` & `tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_filter.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_groupby.py` & `tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_groupby.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_id.py` & `tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_id.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_join.py` & `tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_join.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_map.py` & `tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_map.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_nan.py` & `tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_nan.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_partition.py` & `tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_partition.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_persist.py` & `tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_persist.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_rename.py` & `tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_rename.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_select.py` & `tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_select.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_truncation.py` & `tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_truncation.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/transformations/test_chaining.py` & `tmlt_core-0.9.1/test/unit/transformations/test_chaining.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/transformations/test_converters.py` & `tmlt_core-0.9.1/test/unit/transformations/test_converters.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/transformations/test_dictionary.py` & `tmlt_core-0.9.1/test/unit/transformations/test_dictionary.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/transformations/test_identity.py` & `tmlt_core-0.9.1/test/unit/transformations/test_identity.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/utils/test_arb.py` & `tmlt_core-0.9.1/test/unit/utils/test_arb.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/utils/test_cleanup.py` & `tmlt_core-0.9.1/test/unit/utils/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/utils/test_configuration.py` & `tmlt_core-0.9.1/test/unit/utils/test_configuration.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/utils/test_distributions.py` & `tmlt_core-0.9.1/test/unit/utils/test_distributions.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/utils/test_exact_number.py` & `tmlt_core-0.9.1/test/unit/utils/test_exact_number.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/utils/test_grouped_dataframe.py` & `tmlt_core-0.9.1/test/unit/utils/test_grouped_dataframe.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/utils/test_join.py` & `tmlt_core-0.9.1/test/unit/utils/test_join.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/utils/test_misc.py` & `tmlt_core-0.9.1/test/unit/utils/test_misc.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/utils/test_testing.py` & `tmlt_core-0.9.1/test/unit/utils/test_testing.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/utils/test_truncation.py` & `tmlt_core-0.9.1/test/unit/utils/test_truncation.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/test/unit/utils/test_type_utils.py` & `tmlt_core-0.9.1/test/unit/utils/test_type_utils.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/domains/base.py` & `tmlt_core-0.9.1/tmlt/core/domains/base.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/domains/collections.py` & `tmlt_core-0.9.1/tmlt/core/domains/collections.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/domains/numpy_domains.py` & `tmlt_core-0.9.1/tmlt/core/domains/numpy_domains.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/domains/pandas_domains.py` & `tmlt_core-0.9.1/tmlt/core/domains/pandas_domains.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/domains/spark_domains.py` & `tmlt_core-0.9.1/tmlt/core/domains/spark_domains.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/measurements/aggregations.py` & `tmlt_core-0.9.1/tmlt/core/measurements/aggregations.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/measurements/base.py` & `tmlt_core-0.9.1/tmlt/core/measurements/base.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/measurements/chaining.py` & `tmlt_core-0.9.1/tmlt/core/measurements/chaining.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/measurements/composition.py` & `tmlt_core-0.9.1/tmlt/core/measurements/composition.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/measurements/converters.py` & `tmlt_core-0.9.1/tmlt/core/measurements/converters.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/measurements/interactive_measurements.py` & `tmlt_core-0.9.1/tmlt/core/measurements/interactive_measurements.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/measurements/noise_mechanisms.py` & `tmlt_core-0.9.1/tmlt/core/measurements/noise_mechanisms.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/measurements/pandas_measurements/dataframe.py` & `tmlt_core-0.9.1/tmlt/core/measurements/pandas_measurements/dataframe.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/measurements/pandas_measurements/series.py` & `tmlt_core-0.9.1/tmlt/core/measurements/pandas_measurements/series.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/measurements/postprocess.py` & `tmlt_core-0.9.1/tmlt/core/measurements/postprocess.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/measurements/spark_measurements.py` & `tmlt_core-0.9.1/tmlt/core/measurements/spark_measurements.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/measures.py` & `tmlt_core-0.9.1/tmlt/core/measures.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,20 @@
 from tmlt.core.utils.validation import validate_exact_number
 
 PrivacyBudgetInput = Union[ExactNumberInput, Tuple[ExactNumberInput, ExactNumberInput]]
 PrivacyBudgetValue = Union[ExactNumber, Tuple[ExactNumber, ExactNumber]]
 
 
 class Measure(ABC):
-    """Base class for output measures."""
+    """Base class for output measures.
+
+    Each measure defines a way of measuring "distance" between two distributions
+    that corresponds to a te guarantees of a variant of differential privacy. Note
+    that these "distances" are not metrics.
+    """
 
     def __eq__(self, other: Any) -> bool:
         """Return True if both measures are equal."""
         return self.__class__ is other.__class__
 
     @abstractmethod
     def validate(self, value: Any):
@@ -36,15 +41,28 @@
 
     def __repr__(self) -> str:
         """Returns string representation."""
         return f"{self.__class__.__name__}()"
 
 
 class PureDP(Measure):
-    """Pure DP measure."""
+    r"""The distance between distributions in "pure" differential privacy.
+
+    As in Definition 1 of :cite:`DworkMNS06`.
+
+    In particular, under this measure the distance :math:`\epsilon` between two
+    distributions :math:`X` and :math:`Y` with the same range is:
+
+    .. math::
+
+        \epsilon = max_{S \subseteq Range(X)}\left(max\left(
+            ln\left(\frac{Pr[X \in S]}{Pr[Y \in S]}\right),
+            ln\left(\frac{Pr[Y \in S]}{Pr[X \in S]}\right)\right)\right)
+
+    """
 
     def validate(self, value: ExactNumberInput):
         """Raises an error if `value` not a valid distance.
 
         * `value` must be a nonnegative real or infinity
 
         Args:
@@ -64,15 +82,29 @@
         """Returns True if `value1` is less than or equal to `value2`."""
         self.validate(value1)
         self.validate(value2)
         return ExactNumber(value1) <= ExactNumber(value2)
 
 
 class ApproxDP(Measure):
-    """Approximate DP measure."""
+    r"""The distance between distributions in approximate differential privacy.
+
+    As introduced in :cite:`DworkKMMN06`.
+
+    In particular, under this measure valid distances :math:`(\epsilon, \delta)`
+    between two distributions :math:`X` and :math:`Y` with the same range are those
+    :math:`(\epsilon, \delta)` satisfying:
+
+    .. math::
+
+        \epsilon = max_{S \subseteq Range(X)}\left(max\left(
+            ln\left(\frac{Pr[X \in S] - \delta}{Pr[Y \in S]}\right),
+            ln\left(\frac{Pr[Y \in S] - \delta}{Pr[X \in S]}\right)\right)\right)
+
+    """
 
     def validate(self, value: Tuple[ExactNumberInput, ExactNumberInput]):
         """Raises an error if `value` not a valid distance.
 
         * `value` must be a tuple with two values: (epsilon, delta)
         * epsilon must be a nonnegative real or infinity
         * delta must be a real between 0 and 1 (inclusive)
@@ -115,18 +147,27 @@
         epsilon2 = ExactNumber(value2[0])
         delta2 = ExactNumber(value2[1])
         value2_is_infinite = not epsilon2.is_finite or delta2 == 1
         return value2_is_infinite or epsilon1 <= epsilon2 and delta1 <= delta2
 
 
 class RhoZCDP(Measure):
-    """ρ-zCDP measure.
+    r"""The distance between distributions in ρ-Zero Concentrated Differential Privacy.
+
+    As in Definition 1.1 of :cite:`BunS16`.
+
+    In particular, under this measure the distance :math:`\rho`
+    between two distributions :math:`X` and :math:`Y` with the same range is:
+
+    .. math::
+        \rho = max_{\alpha \in (1, \infty)}\left(max\left(
+            \frac{D_{\alpha}(X||Y)}{\alpha},
+            \frac{D_{\alpha}(Y||X)}{\alpha}\right)\right)
 
-    See the definition of ρ-zCDP in `this <https://arxiv.org/pdf/1605.02065.pdf>`_ paper
-    under Definition 1.1.
+    where :math:`D_{\alpha}(X||Y)` is the α-Rényi divergence between X and Y.
     """
 
     def validate(self, value: ExactNumberInput):
         """Raises an error if `value` not a valid distance.
 
         * `value` must be a nonnegative real or infinity
```

### Comparing `tmlt_core-0.9.0/tmlt/core/metrics.py` & `tmlt_core-0.9.1/tmlt/core/metrics.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/random/continuous_gaussian.py` & `tmlt_core-0.9.1/tmlt/core/random/continuous_gaussian.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/random/discrete_gaussian.py` & `tmlt_core-0.9.1/tmlt/core/random/discrete_gaussian.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/random/inverse_cdf.py` & `tmlt_core-0.9.1/tmlt/core/random/inverse_cdf.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/random/laplace.py` & `tmlt_core-0.9.1/tmlt/core/random/laplace.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/random/rng.py` & `tmlt_core-0.9.1/tmlt/core/random/rng.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/random/uniform.py` & `tmlt_core-0.9.1/tmlt/core/random/uniform.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/transformations/base.py` & `tmlt_core-0.9.1/tmlt/core/transformations/base.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/transformations/chaining.py` & `tmlt_core-0.9.1/tmlt/core/transformations/chaining.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/transformations/converters.py` & `tmlt_core-0.9.1/tmlt/core/transformations/converters.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/transformations/dictionary.py` & `tmlt_core-0.9.1/tmlt/core/transformations/dictionary.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/transformations/identity.py` & `tmlt_core-0.9.1/tmlt/core/transformations/identity.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/add_remove_keys.py` & `tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/add_remove_keys.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/agg.py` & `tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/agg.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/filter.py` & `tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/filter.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/groupby.py` & `tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/groupby.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/id.py` & `tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/id.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/join.py` & `tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/join.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/map.py` & `tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/map.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/nan.py` & `tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/nan.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/partition.py` & `tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/partition.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/persist.py` & `tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/persist.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/rename.py` & `tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/rename.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/select.py` & `tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/select.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/truncation.py` & `tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/truncation.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/utils/arb.py` & `tmlt_core-0.9.1/tmlt/core/utils/arb.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/utils/cleanup.py` & `tmlt_core-0.9.1/tmlt/core/utils/cleanup.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/utils/configuration.py` & `tmlt_core-0.9.1/tmlt/core/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/utils/distributions.py` & `tmlt_core-0.9.1/tmlt/core/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/utils/exact_number.py` & `tmlt_core-0.9.1/tmlt/core/utils/exact_number.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/utils/grouped_dataframe.py` & `tmlt_core-0.9.1/tmlt/core/utils/grouped_dataframe.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/utils/join.py` & `tmlt_core-0.9.1/tmlt/core/utils/join.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/utils/misc.py` & `tmlt_core-0.9.1/tmlt/core/utils/misc.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/utils/parameters.py` & `tmlt_core-0.9.1/tmlt/core/utils/parameters.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/utils/testing.py` & `tmlt_core-0.9.1/tmlt/core/utils/testing.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/utils/truncation.py` & `tmlt_core-0.9.1/tmlt/core/utils/truncation.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/utils/type_utils.py` & `tmlt_core-0.9.1/tmlt/core/utils/type_utils.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/tmlt/core/utils/validation.py` & `tmlt_core-0.9.1/tmlt/core/utils/validation.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.0/PKG-INFO` & `tmlt_core-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmlt-core
-Version: 0.9.0
+Version: 0.9.1
 Summary: Tumult's differential privacy primitives
 Home-page: https://gitlab.com/tumult-labs/core
 License: Apache-2.0
 Requires-Python: >=3.7.1,<3.10
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

