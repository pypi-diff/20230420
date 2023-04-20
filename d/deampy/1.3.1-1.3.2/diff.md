# Comparing `tmp/deampy-1.3.1.tar.gz` & `tmp/deampy-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deampy-1.3.1.tar", last modified: Tue Apr 18 15:35:25 2023, max compression
+gzip compressed data, was "deampy-1.3.2.tar", last modified: Thu Apr 20 02:16:43 2023, max compression
```

## Comparing `deampy-1.3.1.tar` & `deampy-1.3.2.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 15:35:25.137259 deampy-1.3.1/
--rw-rw-rw-   0        0        0     3148 2022-11-29 13:37:07.000000 deampy-1.3.1/.gitignore
--rw-rw-rw-   0        0        0     1108 2022-05-23 18:31:32.000000 deampy-1.3.1/LICENSE
--rw-rw-rw-   0        0        0      244 2022-04-15 15:14:46.000000 deampy-1.3.1/Notes
--rw-rw-rw-   0        0        0      349 2023-04-18 15:35:25.135257 deampy-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0       59 2022-05-23 18:48:59.000000 deampy-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 15:35:24.637263 deampy-1.3.1/deampy/
--rw-rw-rw-   0        0        0      262 2022-05-25 20:47:50.000000 deampy-1.3.1/deampy/__init__.py
--rw-rw-rw-   0        0        0    22678 2022-05-23 19:01:57.000000 deampy-1.3.1/deampy/data_structure.py
--rw-rw-rw-   0        0        0     9513 2021-06-09 12:57:51.000000 deampy-1.3.1/deampy/decision_tree.py
--rw-rw-rw-   0        0        0     2096 2023-02-05 22:50:41.000000 deampy-1.3.1/deampy/discrete_event_sim.py
--rw-rw-rw-   0        0        0   134398 2023-04-17 21:56:38.000000 deampy-1.3.1/deampy/econ_eval.py
--rw-rw-rw-   0        0        0     5053 2022-05-23 19:18:47.000000 deampy-1.3.1/deampy/format_functions.py
--rw-rw-rw-   0        0        0     9183 2022-07-01 21:58:31.000000 deampy-1.3.1/deampy/in_out_functions.py
--rw-rw-rw-   0        0        0     9265 2023-04-11 20:11:27.000000 deampy-1.3.1/deampy/markov.py
--rw-rw-rw-   0        0        0     1907 2022-05-23 19:27:16.000000 deampy-1.3.1/deampy/models.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:35:24.695268 deampy-1.3.1/deampy/optimization/
--rw-rw-rw-   0        0        0        0 2021-06-09 12:57:51.000000 deampy-1.3.1/deampy/optimization/__init__.py
--rw-rw-rw-   0        0        0    26223 2022-05-25 23:12:36.000000 deampy-1.3.1/deampy/optimization/appx_policy_itr.py
--rw-rw-rw-   0        0        0     1079 2021-06-09 12:57:51.000000 deampy-1.3.1/deampy/optimization/learning_exploring_rules.py
--rw-rw-rw-   0        0        0      298 2021-06-09 12:57:51.000000 deampy-1.3.1/deampy/optimization/opt_support.py
--rw-rw-rw-   0        0        0     8766 2021-06-09 12:57:51.000000 deampy-1.3.1/deampy/optimization/stoch_approx.py
--rw-rw-rw-   0        0        0    21553 2023-03-03 22:43:06.000000 deampy-1.3.1/deampy/parameter_estimation.py
--rw-rw-rw-   0        0        0    23903 2023-03-03 22:43:06.000000 deampy-1.3.1/deampy/parameters.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:35:24.746280 deampy-1.3.1/deampy/plots/
--rw-rw-rw-   0        0        0        0 2021-06-09 12:57:51.000000 deampy-1.3.1/deampy/plots/__init__.py
--rw-rw-rw-   0        0        0     6234 2022-11-29 13:37:07.000000 deampy-1.3.1/deampy/plots/econ_eval_plots.py
--rw-rw-rw-   0        0        0     1368 2022-05-23 19:45:56.000000 deampy-1.3.1/deampy/plots/eff_sample_size.py
--rw-rw-rw-   0        0        0     7109 2023-03-03 22:43:06.000000 deampy-1.3.1/deampy/plots/histogram.py
--rw-rw-rw-   0        0        0     2487 2023-01-18 19:18:23.000000 deampy-1.3.1/deampy/plots/plot_support.py
--rw-rw-rw-   0        0        0     6492 2021-06-09 12:57:51.000000 deampy-1.3.1/deampy/plots/pop_pyramids.py
--rw-rw-rw-   0        0        0    26162 2023-01-20 00:02:18.000000 deampy-1.3.1/deampy/plots/prob_dists.py
--rw-rw-rw-   0        0        0     9795 2023-01-18 19:18:23.000000 deampy-1.3.1/deampy/plots/sample_paths.py
--rw-rw-rw-   0        0        0    42000 2022-11-29 13:37:07.000000 deampy-1.3.1/deampy/random_variates.py
--rw-rw-rw-   0        0        0    16282 2021-06-09 12:57:51.000000 deampy-1.3.1/deampy/regression_models.py
--rw-rw-rw-   0        0        0     9436 2022-05-23 19:40:18.000000 deampy-1.3.1/deampy/sample_path.py
--rw-rw-rw-   0        0        0     6676 2022-05-23 19:45:56.000000 deampy-1.3.1/deampy/sensitivity_analysis.py
--rw-rw-rw-   0        0        0    43258 2023-04-17 21:56:38.000000 deampy-1.3.1/deampy/statistics.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:35:24.776257 deampy-1.3.1/deampy/support/
--rw-rw-rw-   0        0        0        0 2021-06-09 12:57:51.000000 deampy-1.3.1/deampy/support/__init__.py
--rw-rw-rw-   0        0        0    10009 2023-04-11 20:11:27.000000 deampy-1.3.1/deampy/support/econ_eval_support.py
--rw-rw-rw-   0        0        0      659 2021-06-09 12:57:51.000000 deampy-1.3.1/deampy/support/misc_classes.py
--rw-rw-rw-   0        0        0     7094 2023-03-10 04:56:08.000000 deampy-1.3.1/deampy/support/misc_functions.py
--rw-rw-rw-   0        0        0     6635 2022-05-23 19:45:56.000000 deampy-1.3.1/deampy/support/simulation.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:35:24.667279 deampy-1.3.1/deampy.egg-info/
--rw-rw-rw-   0        0        0      349 2023-04-18 15:35:24.000000 deampy-1.3.1/deampy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3251 2023-04-18 15:35:24.000000 deampy-1.3.1/deampy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 15:35:24.000000 deampy-1.3.1/deampy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-04-18 15:35:24.000000 deampy-1.3.1/deampy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-18 15:35:24.000000 deampy-1.3.1/deampy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 15:35:25.138260 deampy-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      701 2023-04-18 15:35:07.000000 deampy-1.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:35:24.486265 deampy-1.3.1/tests/
-drwxrwxrwx   0        0        0        0 2023-04-18 15:35:24.806260 deampy-1.3.1/tests/approx_policy_itr/
--rw-rw-rw-   0        0        0     2063 2022-05-23 19:03:35.000000 deampy-1.3.1/tests/approx_policy_itr/compare.py
--rw-rw-rw-   0        0        0     3574 2022-05-23 18:57:17.000000 deampy-1.3.1/tests/approx_policy_itr/model.py
--rw-rw-rw-   0        0        0     1340 2022-05-23 19:03:35.000000 deampy-1.3.1/tests/approx_policy_itr/optimize_many.py
--rw-rw-rw-   0        0        0      986 2022-05-23 19:03:35.000000 deampy-1.3.1/tests/approx_policy_itr/optimize_one.py
--rw-rw-rw-   0        0        0      154 2022-05-23 18:57:17.000000 deampy-1.3.1/tests/approx_policy_itr/test_support.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:35:24.816257 deampy-1.3.1/tests/cython/
--rw-rw-rw-   0        0        0      494 2021-06-09 12:57:51.000000 deampy-1.3.1/tests/cython/fibo.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:35:24.853259 deampy-1.3.1/tests/data_structures/
--rw-rw-rw-   0        0        0     1727 2022-05-23 19:01:48.000000 deampy-1.3.1/tests/data_structures/test_multi_dim.py
--rw-rw-rw-   0        0        0      956 2022-05-23 19:02:08.000000 deampy-1.3.1/tests/data_structures/test_multi_dim_with_exp_dist.py
--rw-rw-rw-   0        0        0     1400 2022-05-23 19:02:21.000000 deampy-1.3.1/tests/data_structures/test_one_dim.py
--rw-rw-rw-   0        0        0     2566 2022-05-23 19:02:34.000000 deampy-1.3.1/tests/data_structures/test_prob_dist_2dim.py
--rw-rw-rw-   0        0        0     1283 2022-05-23 19:02:45.000000 deampy-1.3.1/tests/data_structures/test_prob_dist_3dim.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:35:24.879271 deampy-1.3.1/tests/decision_tree/
--rw-rw-rw-   0        0        0  1829766 2021-06-09 12:57:51.000000 deampy-1.3.1/tests/decision_tree/Migraine Model.tif
--rw-rw-rw-   0        0        0     1902 2022-05-23 19:04:03.000000 deampy-1.3.1/tests/decision_tree/use_decision_tree.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:35:24.886259 deampy-1.3.1/tests/discrete_even_sim/
--rw-rw-rw-   0        0        0     1027 2022-05-23 19:06:54.000000 deampy-1.3.1/tests/discrete_even_sim/test_discrete_event_classes.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:35:24.954258 deampy-1.3.1/tests/econ_eval/
--rw-rw-rw-   0        0        0      641 2022-05-23 19:07:28.000000 deampy-1.3.1/tests/econ_eval/play_ground.py
--rw-rw-rw-   0        0        0     2765 2022-05-23 19:09:33.000000 deampy-1.3.1/tests/econ_eval/test_cea.py
--rw-rw-rw-   0        0        0     1339 2022-05-23 19:10:52.000000 deampy-1.3.1/tests/econ_eval/test_cea_interval.py
--rw-rw-rw-   0        0        0      717 2022-05-23 19:11:10.000000 deampy-1.3.1/tests/econ_eval/test_cea_simple.py
--rw-rw-rw-   0        0        0     1210 2022-05-23 19:11:24.000000 deampy-1.3.1/tests/econ_eval/test_discounting.py
--rw-rw-rw-   0        0        0     2091 2023-04-11 20:11:27.000000 deampy-1.3.1/tests/econ_eval/test_icer_nmb_for_disutility.py
--rw-rw-rw-   0        0        0     3110 2023-04-11 20:11:27.000000 deampy-1.3.1/tests/econ_eval/test_icer_nmb_for_utility.py
--rw-rw-rw-   0        0        0     1044 2022-05-23 19:15:04.000000 deampy-1.3.1/tests/econ_eval/test_new_cea_simple.py
--rw-rw-rw-   0        0        0     1830 2022-05-23 19:15:17.000000 deampy-1.3.1/tests/econ_eval/test_new_cea_with_clouds.py
--rw-rw-rw-   0        0        0     1889 2023-04-11 20:11:27.000000 deampy-1.3.1/tests/econ_eval/test_nmb_graph.py
--rw-rw-rw-   0        0        0      202 2022-05-23 19:15:57.000000 deampy-1.3.1/tests/econ_eval/test_utilities.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:35:24.970258 deampy-1.3.1/tests/input_output/
--rw-rw-rw-   0        0        0      912 2022-05-23 19:16:27.000000 deampy-1.3.1/tests/input_output/test_csv_reader.py
--rw-rw-rw-   0        0        0      334 2022-05-23 19:19:05.000000 deampy-1.3.1/tests/input_output/test_csv_writter.py
--rw-rw-rw-   0        0        0     1125 2022-05-23 19:18:47.000000 deampy-1.3.1/tests/input_output/test_format_functions.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:35:24.981300 deampy-1.3.1/tests/markov/
--rw-rw-rw-   0        0        0      407 2022-05-23 19:45:56.000000 deampy-1.3.1/tests/markov/test_gillespie.py
--rw-rw-rw-   0        0        0      593 2022-05-23 19:20:02.000000 deampy-1.3.1/tests/markov/test_markov.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:35:24.991270 deampy-1.3.1/tests/misc/
--rw-rw-rw-   0        0        0      211 2022-05-23 19:43:39.000000 deampy-1.3.1/tests/misc/test_eff_sample_size.py
--rw-rw-rw-   0        0        0      269 2021-06-09 12:57:51.000000 deampy-1.3.1/tests/misc/test_sorting.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:35:24.996269 deampy-1.3.1/tests/models/
--rw-rw-rw-   0        0        0     1037 2022-05-23 19:27:04.000000 deampy-1.3.1/tests/models/mortality_model.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:35:25.017261 deampy-1.3.1/tests/optimization/
--rw-rw-rw-   0        0        0      678 2022-05-23 19:30:59.000000 deampy-1.3.1/tests/optimization/test_opt_constrained.py
--rw-rw-rw-   0        0        0      736 2022-05-23 19:31:41.000000 deampy-1.3.1/tests/optimization/test_opt_unconstrained.py
--rw-rw-rw-   0        0        0      185 2022-05-23 19:33:02.000000 deampy-1.3.1/tests/optimization/test_plot_ste_sizes.py
--rw-rw-rw-   0        0        0     1771 2022-05-23 19:29:30.000000 deampy-1.3.1/tests/optimization/toy_model.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:35:25.023260 deampy-1.3.1/tests/parameters/
--rw-rw-rw-   0        0        0      493 2022-05-23 19:42:02.000000 deampy-1.3.1/tests/parameters/parameters.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:35:25.040260 deampy-1.3.1/tests/plots/
--rw-rw-rw-   0        0        0     2069 2022-05-23 19:35:00.000000 deampy-1.3.1/tests/plots/plot_pyramids.py
--rw-rw-rw-   0        0        0      686 2022-05-23 19:45:56.000000 deampy-1.3.1/tests/plots/test_histograms.py
--rw-rw-rw-   0        0        0      410 2022-05-23 19:45:56.000000 deampy-1.3.1/tests/plots/test_moving_average.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:35:25.064281 deampy-1.3.1/tests/prob_dists/
--rw-rw-rw-   0        0        0    13584 2022-05-23 19:45:56.000000 deampy-1.3.1/tests/prob_dists/fit_dist_tests.py
--rw-rw-rw-   0        0        0    11841 2022-05-23 19:45:56.000000 deampy-1.3.1/tests/prob_dists/rvg_tests.py
--rw-rw-rw-   0        0        0      565 2022-05-23 19:36:34.000000 deampy-1.3.1/tests/prob_dists/test_fitting_prob_dists.py
--rw-rw-rw-   0        0        0     1315 2022-05-23 19:36:54.000000 deampy-1.3.1/tests/prob_dists/test_rvgs.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:35:25.099261 deampy-1.3.1/tests/regression/
--rw-rw-rw-   0        0        0     1658 2022-05-23 19:45:56.000000 deampy-1.3.1/tests/regression/test_exp_reg.py
--rw-rw-rw-   0        0        0     1614 2022-05-23 19:45:56.000000 deampy-1.3.1/tests/regression/test_poly_ref_with_interval.py
--rw-rw-rw-   0        0        0      550 2022-05-23 19:45:56.000000 deampy-1.3.1/tests/regression/test_poly_reg.py
--rw-rw-rw-   0        0        0     2967 2022-05-23 19:39:01.000000 deampy-1.3.1/tests/regression/test_polynomial_q.py
--rw-rw-rw-   0        0        0      476 2022-05-23 19:39:01.000000 deampy-1.3.1/tests/regression/test_power_reg.py
--rw-rw-rw-   0        0        0     1948 2022-05-23 19:39:01.000000 deampy-1.3.1/tests/regression/test_regression.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:35:25.116260 deampy-1.3.1/tests/sample_paths/
--rw-rw-rw-   0        0        0     1061 2023-01-18 19:18:23.000000 deampy-1.3.1/tests/sample_paths/test_incidence.py
--rw-rw-rw-   0        0        0     2130 2022-05-23 19:40:32.000000 deampy-1.3.1/tests/sample_paths/test_prev_pyramid.py
--rw-rw-rw-   0        0        0     2078 2023-01-18 19:18:23.000000 deampy-1.3.1/tests/sample_paths/test_prevalence.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:35:25.128261 deampy-1.3.1/tests/senstivity_analysis/
--rw-rw-rw-   0        0        0      512 2022-05-23 19:45:56.000000 deampy-1.3.1/tests/senstivity_analysis/test_rank_corr.py
--rw-rw-rw-   0        0        0      868 2022-05-23 19:41:14.000000 deampy-1.3.1/tests/senstivity_analysis/test_sa.py
+drwxrwxrwx   0        0        0        0 2023-04-20 02:16:43.669595 deampy-1.3.2/
+-rw-rw-rw-   0        0        0     3148 2022-11-29 13:37:07.000000 deampy-1.3.2/.gitignore
+-rw-rw-rw-   0        0        0     1108 2022-05-23 18:31:32.000000 deampy-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0      244 2022-04-15 15:14:46.000000 deampy-1.3.2/Notes
+-rw-rw-rw-   0        0        0      349 2023-04-20 02:16:43.668595 deampy-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0       59 2022-05-23 18:48:59.000000 deampy-1.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 02:16:43.149602 deampy-1.3.2/deampy/
+-rw-rw-rw-   0        0        0      262 2022-05-25 20:47:50.000000 deampy-1.3.2/deampy/__init__.py
+-rw-rw-rw-   0        0        0    22678 2022-05-23 19:01:57.000000 deampy-1.3.2/deampy/data_structure.py
+-rw-rw-rw-   0        0        0     9513 2021-06-09 12:57:51.000000 deampy-1.3.2/deampy/decision_tree.py
+-rw-rw-rw-   0        0        0     2096 2023-02-05 22:50:41.000000 deampy-1.3.2/deampy/discrete_event_sim.py
+-rw-rw-rw-   0        0        0   134398 2023-04-17 21:56:38.000000 deampy-1.3.2/deampy/econ_eval.py
+-rw-rw-rw-   0        0        0     5053 2022-05-23 19:18:47.000000 deampy-1.3.2/deampy/format_functions.py
+-rw-rw-rw-   0        0        0     9183 2022-07-01 21:58:31.000000 deampy-1.3.2/deampy/in_out_functions.py
+-rw-rw-rw-   0        0        0     9265 2023-04-11 20:11:27.000000 deampy-1.3.2/deampy/markov.py
+-rw-rw-rw-   0        0        0     1907 2022-05-23 19:27:16.000000 deampy-1.3.2/deampy/models.py
+drwxrwxrwx   0        0        0        0 2023-04-20 02:16:43.214593 deampy-1.3.2/deampy/optimization/
+-rw-rw-rw-   0        0        0        0 2021-06-09 12:57:51.000000 deampy-1.3.2/deampy/optimization/__init__.py
+-rw-rw-rw-   0        0        0    26223 2022-05-25 23:12:36.000000 deampy-1.3.2/deampy/optimization/appx_policy_itr.py
+-rw-rw-rw-   0        0        0     1079 2021-06-09 12:57:51.000000 deampy-1.3.2/deampy/optimization/learning_exploring_rules.py
+-rw-rw-rw-   0        0        0      298 2021-06-09 12:57:51.000000 deampy-1.3.2/deampy/optimization/opt_support.py
+-rw-rw-rw-   0        0        0     8766 2021-06-09 12:57:51.000000 deampy-1.3.2/deampy/optimization/stoch_approx.py
+-rw-rw-rw-   0        0        0    21553 2023-03-03 22:43:06.000000 deampy-1.3.2/deampy/parameter_estimation.py
+-rw-rw-rw-   0        0        0    23903 2023-03-03 22:43:06.000000 deampy-1.3.2/deampy/parameters.py
+drwxrwxrwx   0        0        0        0 2023-04-20 02:16:43.273594 deampy-1.3.2/deampy/plots/
+-rw-rw-rw-   0        0        0        0 2021-06-09 12:57:51.000000 deampy-1.3.2/deampy/plots/__init__.py
+-rw-rw-rw-   0        0        0     6234 2022-11-29 13:37:07.000000 deampy-1.3.2/deampy/plots/econ_eval_plots.py
+-rw-rw-rw-   0        0        0     1368 2022-05-23 19:45:56.000000 deampy-1.3.2/deampy/plots/eff_sample_size.py
+-rw-rw-rw-   0        0        0     7109 2023-03-03 22:43:06.000000 deampy-1.3.2/deampy/plots/histogram.py
+-rw-rw-rw-   0        0        0     2487 2023-01-18 19:18:23.000000 deampy-1.3.2/deampy/plots/plot_support.py
+-rw-rw-rw-   0        0        0     6492 2021-06-09 12:57:51.000000 deampy-1.3.2/deampy/plots/pop_pyramids.py
+-rw-rw-rw-   0        0        0    26140 2023-04-18 16:07:27.000000 deampy-1.3.2/deampy/plots/prob_dists.py
+-rw-rw-rw-   0        0        0     9795 2023-01-18 19:18:23.000000 deampy-1.3.2/deampy/plots/sample_paths.py
+-rw-rw-rw-   0        0        0    42000 2022-11-29 13:37:07.000000 deampy-1.3.2/deampy/random_variates.py
+-rw-rw-rw-   0        0        0    16282 2021-06-09 12:57:51.000000 deampy-1.3.2/deampy/regression_models.py
+-rw-rw-rw-   0        0        0     9436 2022-05-23 19:40:18.000000 deampy-1.3.2/deampy/sample_path.py
+-rw-rw-rw-   0        0        0     6676 2022-05-23 19:45:56.000000 deampy-1.3.2/deampy/sensitivity_analysis.py
+-rw-rw-rw-   0        0        0    43258 2023-04-17 21:56:38.000000 deampy-1.3.2/deampy/statistics.py
+drwxrwxrwx   0        0        0        0 2023-04-20 02:16:43.305591 deampy-1.3.2/deampy/support/
+-rw-rw-rw-   0        0        0        0 2021-06-09 12:57:51.000000 deampy-1.3.2/deampy/support/__init__.py
+-rw-rw-rw-   0        0        0    10009 2023-04-11 20:11:27.000000 deampy-1.3.2/deampy/support/econ_eval_support.py
+-rw-rw-rw-   0        0        0      659 2021-06-09 12:57:51.000000 deampy-1.3.2/deampy/support/misc_classes.py
+-rw-rw-rw-   0        0        0     7094 2023-03-10 04:56:08.000000 deampy-1.3.2/deampy/support/misc_functions.py
+-rw-rw-rw-   0        0        0     6635 2022-05-23 19:45:56.000000 deampy-1.3.2/deampy/support/simulation.py
+drwxrwxrwx   0        0        0        0 2023-04-20 02:16:43.180594 deampy-1.3.2/deampy.egg-info/
+-rw-rw-rw-   0        0        0      349 2023-04-20 02:16:42.000000 deampy-1.3.2/deampy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3251 2023-04-20 02:16:42.000000 deampy-1.3.2/deampy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 02:16:42.000000 deampy-1.3.2/deampy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-04-20 02:16:42.000000 deampy-1.3.2/deampy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-20 02:16:42.000000 deampy-1.3.2/deampy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 02:16:43.670596 deampy-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      701 2023-04-20 02:16:23.000000 deampy-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 02:16:42.993593 deampy-1.3.2/tests/
+drwxrwxrwx   0        0        0        0 2023-04-20 02:16:43.339594 deampy-1.3.2/tests/approx_policy_itr/
+-rw-rw-rw-   0        0        0     2063 2022-05-23 19:03:35.000000 deampy-1.3.2/tests/approx_policy_itr/compare.py
+-rw-rw-rw-   0        0        0     3574 2022-05-23 18:57:17.000000 deampy-1.3.2/tests/approx_policy_itr/model.py
+-rw-rw-rw-   0        0        0     1340 2022-05-23 19:03:35.000000 deampy-1.3.2/tests/approx_policy_itr/optimize_many.py
+-rw-rw-rw-   0        0        0      986 2022-05-23 19:03:35.000000 deampy-1.3.2/tests/approx_policy_itr/optimize_one.py
+-rw-rw-rw-   0        0        0      154 2022-05-23 18:57:17.000000 deampy-1.3.2/tests/approx_policy_itr/test_support.py
+drwxrwxrwx   0        0        0        0 2023-04-20 02:16:43.344595 deampy-1.3.2/tests/cython/
+-rw-rw-rw-   0        0        0      494 2021-06-09 12:57:51.000000 deampy-1.3.2/tests/cython/fibo.py
+drwxrwxrwx   0        0        0        0 2023-04-20 02:16:43.375595 deampy-1.3.2/tests/data_structures/
+-rw-rw-rw-   0        0        0     1727 2022-05-23 19:01:48.000000 deampy-1.3.2/tests/data_structures/test_multi_dim.py
+-rw-rw-rw-   0        0        0      956 2022-05-23 19:02:08.000000 deampy-1.3.2/tests/data_structures/test_multi_dim_with_exp_dist.py
+-rw-rw-rw-   0        0        0     1400 2022-05-23 19:02:21.000000 deampy-1.3.2/tests/data_structures/test_one_dim.py
+-rw-rw-rw-   0        0        0     2566 2022-05-23 19:02:34.000000 deampy-1.3.2/tests/data_structures/test_prob_dist_2dim.py
+-rw-rw-rw-   0        0        0     1283 2022-05-23 19:02:45.000000 deampy-1.3.2/tests/data_structures/test_prob_dist_3dim.py
+drwxrwxrwx   0        0        0        0 2023-04-20 02:16:43.396595 deampy-1.3.2/tests/decision_tree/
+-rw-rw-rw-   0        0        0  1829766 2021-06-09 12:57:51.000000 deampy-1.3.2/tests/decision_tree/Migraine Model.tif
+-rw-rw-rw-   0        0        0     1902 2022-05-23 19:04:03.000000 deampy-1.3.2/tests/decision_tree/use_decision_tree.py
+drwxrwxrwx   0        0        0        0 2023-04-20 02:16:43.402594 deampy-1.3.2/tests/discrete_even_sim/
+-rw-rw-rw-   0        0        0     1027 2022-05-23 19:06:54.000000 deampy-1.3.2/tests/discrete_even_sim/test_discrete_event_classes.py
+drwxrwxrwx   0        0        0        0 2023-04-20 02:16:43.470594 deampy-1.3.2/tests/econ_eval/
+-rw-rw-rw-   0        0        0      641 2022-05-23 19:07:28.000000 deampy-1.3.2/tests/econ_eval/play_ground.py
+-rw-rw-rw-   0        0        0     2765 2022-05-23 19:09:33.000000 deampy-1.3.2/tests/econ_eval/test_cea.py
+-rw-rw-rw-   0        0        0     1339 2022-05-23 19:10:52.000000 deampy-1.3.2/tests/econ_eval/test_cea_interval.py
+-rw-rw-rw-   0        0        0      717 2022-05-23 19:11:10.000000 deampy-1.3.2/tests/econ_eval/test_cea_simple.py
+-rw-rw-rw-   0        0        0     1210 2022-05-23 19:11:24.000000 deampy-1.3.2/tests/econ_eval/test_discounting.py
+-rw-rw-rw-   0        0        0     2091 2023-04-11 20:11:27.000000 deampy-1.3.2/tests/econ_eval/test_icer_nmb_for_disutility.py
+-rw-rw-rw-   0        0        0     3110 2023-04-11 20:11:27.000000 deampy-1.3.2/tests/econ_eval/test_icer_nmb_for_utility.py
+-rw-rw-rw-   0        0        0     1044 2022-05-23 19:15:04.000000 deampy-1.3.2/tests/econ_eval/test_new_cea_simple.py
+-rw-rw-rw-   0        0        0     1830 2022-05-23 19:15:17.000000 deampy-1.3.2/tests/econ_eval/test_new_cea_with_clouds.py
+-rw-rw-rw-   0        0        0     1889 2023-04-11 20:11:27.000000 deampy-1.3.2/tests/econ_eval/test_nmb_graph.py
+-rw-rw-rw-   0        0        0      202 2022-05-23 19:15:57.000000 deampy-1.3.2/tests/econ_eval/test_utilities.py
+drwxrwxrwx   0        0        0        0 2023-04-20 02:16:43.487595 deampy-1.3.2/tests/input_output/
+-rw-rw-rw-   0        0        0      912 2022-05-23 19:16:27.000000 deampy-1.3.2/tests/input_output/test_csv_reader.py
+-rw-rw-rw-   0        0        0      334 2022-05-23 19:19:05.000000 deampy-1.3.2/tests/input_output/test_csv_writter.py
+-rw-rw-rw-   0        0        0     1125 2022-05-23 19:18:47.000000 deampy-1.3.2/tests/input_output/test_format_functions.py
+drwxrwxrwx   0        0        0        0 2023-04-20 02:16:43.497594 deampy-1.3.2/tests/markov/
+-rw-rw-rw-   0        0        0      407 2022-05-23 19:45:56.000000 deampy-1.3.2/tests/markov/test_gillespie.py
+-rw-rw-rw-   0        0        0      593 2022-05-23 19:20:02.000000 deampy-1.3.2/tests/markov/test_markov.py
+drwxrwxrwx   0        0        0        0 2023-04-20 02:16:43.508595 deampy-1.3.2/tests/misc/
+-rw-rw-rw-   0        0        0      211 2022-05-23 19:43:39.000000 deampy-1.3.2/tests/misc/test_eff_sample_size.py
+-rw-rw-rw-   0        0        0      269 2021-06-09 12:57:51.000000 deampy-1.3.2/tests/misc/test_sorting.py
+drwxrwxrwx   0        0        0        0 2023-04-20 02:16:43.514595 deampy-1.3.2/tests/models/
+-rw-rw-rw-   0        0        0     1037 2022-05-23 19:27:04.000000 deampy-1.3.2/tests/models/mortality_model.py
+drwxrwxrwx   0        0        0        0 2023-04-20 02:16:43.538596 deampy-1.3.2/tests/optimization/
+-rw-rw-rw-   0        0        0      678 2022-05-23 19:30:59.000000 deampy-1.3.2/tests/optimization/test_opt_constrained.py
+-rw-rw-rw-   0        0        0      736 2022-05-23 19:31:41.000000 deampy-1.3.2/tests/optimization/test_opt_unconstrained.py
+-rw-rw-rw-   0        0        0      185 2022-05-23 19:33:02.000000 deampy-1.3.2/tests/optimization/test_plot_ste_sizes.py
+-rw-rw-rw-   0        0        0     1771 2022-05-23 19:29:30.000000 deampy-1.3.2/tests/optimization/toy_model.py
+drwxrwxrwx   0        0        0        0 2023-04-20 02:16:43.545593 deampy-1.3.2/tests/parameters/
+-rw-rw-rw-   0        0        0      493 2022-05-23 19:42:02.000000 deampy-1.3.2/tests/parameters/parameters.py
+drwxrwxrwx   0        0        0        0 2023-04-20 02:16:43.563594 deampy-1.3.2/tests/plots/
+-rw-rw-rw-   0        0        0     2069 2022-05-23 19:35:00.000000 deampy-1.3.2/tests/plots/plot_pyramids.py
+-rw-rw-rw-   0        0        0      686 2022-05-23 19:45:56.000000 deampy-1.3.2/tests/plots/test_histograms.py
+-rw-rw-rw-   0        0        0      410 2022-05-23 19:45:56.000000 deampy-1.3.2/tests/plots/test_moving_average.py
+drwxrwxrwx   0        0        0        0 2023-04-20 02:16:43.590596 deampy-1.3.2/tests/prob_dists/
+-rw-rw-rw-   0        0        0    13584 2022-05-23 19:45:56.000000 deampy-1.3.2/tests/prob_dists/fit_dist_tests.py
+-rw-rw-rw-   0        0        0    11841 2022-05-23 19:45:56.000000 deampy-1.3.2/tests/prob_dists/rvg_tests.py
+-rw-rw-rw-   0        0        0      565 2022-05-23 19:36:34.000000 deampy-1.3.2/tests/prob_dists/test_fitting_prob_dists.py
+-rw-rw-rw-   0        0        0     1315 2022-05-23 19:36:54.000000 deampy-1.3.2/tests/prob_dists/test_rvgs.py
+drwxrwxrwx   0        0        0        0 2023-04-20 02:16:43.628595 deampy-1.3.2/tests/regression/
+-rw-rw-rw-   0        0        0     1658 2022-05-23 19:45:56.000000 deampy-1.3.2/tests/regression/test_exp_reg.py
+-rw-rw-rw-   0        0        0     1614 2022-05-23 19:45:56.000000 deampy-1.3.2/tests/regression/test_poly_ref_with_interval.py
+-rw-rw-rw-   0        0        0      550 2022-05-23 19:45:56.000000 deampy-1.3.2/tests/regression/test_poly_reg.py
+-rw-rw-rw-   0        0        0     2967 2022-05-23 19:39:01.000000 deampy-1.3.2/tests/regression/test_polynomial_q.py
+-rw-rw-rw-   0        0        0      476 2022-05-23 19:39:01.000000 deampy-1.3.2/tests/regression/test_power_reg.py
+-rw-rw-rw-   0        0        0     1948 2022-05-23 19:39:01.000000 deampy-1.3.2/tests/regression/test_regression.py
+drwxrwxrwx   0        0        0        0 2023-04-20 02:16:43.648596 deampy-1.3.2/tests/sample_paths/
+-rw-rw-rw-   0        0        0     1061 2023-01-18 19:18:23.000000 deampy-1.3.2/tests/sample_paths/test_incidence.py
+-rw-rw-rw-   0        0        0     2130 2022-05-23 19:40:32.000000 deampy-1.3.2/tests/sample_paths/test_prev_pyramid.py
+-rw-rw-rw-   0        0        0     2078 2023-01-18 19:18:23.000000 deampy-1.3.2/tests/sample_paths/test_prevalence.py
+drwxrwxrwx   0        0        0        0 2023-04-20 02:16:43.661596 deampy-1.3.2/tests/senstivity_analysis/
+-rw-rw-rw-   0        0        0      512 2022-05-23 19:45:56.000000 deampy-1.3.2/tests/senstivity_analysis/test_rank_corr.py
+-rw-rw-rw-   0        0        0      868 2022-05-23 19:41:14.000000 deampy-1.3.2/tests/senstivity_analysis/test_sa.py
```

### Comparing `deampy-1.3.1/.gitignore` & `deampy-1.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/LICENSE` & `deampy-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/deampy/data_structure.py` & `deampy-1.3.2/deampy/data_structure.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/deampy/decision_tree.py` & `deampy-1.3.2/deampy/decision_tree.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/deampy/discrete_event_sim.py` & `deampy-1.3.2/deampy/discrete_event_sim.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/deampy/econ_eval.py` & `deampy-1.3.2/deampy/econ_eval.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/deampy/format_functions.py` & `deampy-1.3.2/deampy/format_functions.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/deampy/in_out_functions.py` & `deampy-1.3.2/deampy/in_out_functions.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/deampy/markov.py` & `deampy-1.3.2/deampy/markov.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/deampy/models.py` & `deampy-1.3.2/deampy/models.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/deampy/optimization/appx_policy_itr.py` & `deampy-1.3.2/deampy/optimization/appx_policy_itr.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/deampy/optimization/learning_exploring_rules.py` & `deampy-1.3.2/deampy/optimization/learning_exploring_rules.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/deampy/optimization/stoch_approx.py` & `deampy-1.3.2/deampy/optimization/stoch_approx.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/deampy/parameter_estimation.py` & `deampy-1.3.2/deampy/parameter_estimation.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/deampy/parameters.py` & `deampy-1.3.2/deampy/parameters.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/deampy/plots/econ_eval_plots.py` & `deampy-1.3.2/deampy/plots/econ_eval_plots.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/deampy/plots/eff_sample_size.py` & `deampy-1.3.2/deampy/plots/eff_sample_size.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/deampy/plots/histogram.py` & `deampy-1.3.2/deampy/plots/histogram.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/deampy/plots/plot_support.py` & `deampy-1.3.2/deampy/plots/plot_support.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/deampy/plots/pop_pyramids.py` & `deampy-1.3.2/deampy/plots/pop_pyramids.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/deampy/plots/prob_dists.py` & `deampy-1.3.2/deampy/plots/prob_dists.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,16 +87,15 @@
     if data is not None:
         add_hist(ax, data, bin_width)
 
     # format axis
     format_fig(ax=ax, title=title, x_label=x_label, x_range=x_range, y_range=y_range)
     ax.legend(fontsize=LEGEND_FONT_SIZE)
 
-    if filename:
-        Fig.output_figure(plt=plt, filename=filename, dpi=300)
+    Fig.output_figure(plt=plt, filename=filename, dpi=300)
 
 
 def plot_continuous_dists(data, dists, labels, colors, title=None, x_label=None, x_range=None, y_range=None,
                           fig_size=(6, 5), bin_width=None, filename=None):
 
     # plot histogram
     fig, ax = plt.subplots(1, 1, figsize=fig_size)
```

### Comparing `deampy-1.3.1/deampy/plots/sample_paths.py` & `deampy-1.3.2/deampy/plots/sample_paths.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/deampy/random_variates.py` & `deampy-1.3.2/deampy/random_variates.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/deampy/regression_models.py` & `deampy-1.3.2/deampy/regression_models.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/deampy/sample_path.py` & `deampy-1.3.2/deampy/sample_path.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/deampy/sensitivity_analysis.py` & `deampy-1.3.2/deampy/sensitivity_analysis.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/deampy/statistics.py` & `deampy-1.3.2/deampy/statistics.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/deampy/support/econ_eval_support.py` & `deampy-1.3.2/deampy/support/econ_eval_support.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/deampy/support/misc_classes.py` & `deampy-1.3.2/deampy/support/misc_classes.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/deampy/support/misc_functions.py` & `deampy-1.3.2/deampy/support/misc_functions.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/deampy/support/simulation.py` & `deampy-1.3.2/deampy/support/simulation.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/deampy.egg-info/SOURCES.txt` & `deampy-1.3.2/deampy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/setup.py` & `deampy-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # read the contents of your README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='deampy',
-    version='1.3.1',
+    version='1.3.2',
     install_requires=['numpy', 'matplotlib', 'scipy', 'statsmodels', 'sklearn'],
     packages=['deampy', 'deampy.optimization', 'deampy.plots', 'deampy.support'],
     url='https://github.com/modeling-health-care-decisions/deampy',
     license='MIT License',
     author='Reza Yaesoubi',
     author_email='reza.yaesoubi@yale.edu',
     description='Decision analysis in medicine and public health',
```

### Comparing `deampy-1.3.1/tests/approx_policy_itr/compare.py` & `deampy-1.3.2/tests/approx_policy_itr/compare.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/approx_policy_itr/model.py` & `deampy-1.3.2/tests/approx_policy_itr/model.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/approx_policy_itr/optimize_many.py` & `deampy-1.3.2/tests/approx_policy_itr/optimize_many.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/approx_policy_itr/optimize_one.py` & `deampy-1.3.2/tests/approx_policy_itr/optimize_one.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/data_structures/test_multi_dim.py` & `deampy-1.3.2/tests/data_structures/test_multi_dim.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/data_structures/test_multi_dim_with_exp_dist.py` & `deampy-1.3.2/tests/data_structures/test_multi_dim_with_exp_dist.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/data_structures/test_one_dim.py` & `deampy-1.3.2/tests/data_structures/test_one_dim.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/data_structures/test_prob_dist_2dim.py` & `deampy-1.3.2/tests/data_structures/test_prob_dist_2dim.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/data_structures/test_prob_dist_3dim.py` & `deampy-1.3.2/tests/data_structures/test_prob_dist_3dim.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/decision_tree/Migraine Model.tif` & `deampy-1.3.2/tests/decision_tree/Migraine Model.tif`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/decision_tree/use_decision_tree.py` & `deampy-1.3.2/tests/decision_tree/use_decision_tree.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/discrete_even_sim/test_discrete_event_classes.py` & `deampy-1.3.2/tests/discrete_even_sim/test_discrete_event_classes.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/econ_eval/play_ground.py` & `deampy-1.3.2/tests/econ_eval/play_ground.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/econ_eval/test_cea.py` & `deampy-1.3.2/tests/econ_eval/test_cea.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/econ_eval/test_cea_interval.py` & `deampy-1.3.2/tests/econ_eval/test_cea_interval.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/econ_eval/test_cea_simple.py` & `deampy-1.3.2/tests/econ_eval/test_cea_simple.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/econ_eval/test_discounting.py` & `deampy-1.3.2/tests/econ_eval/test_discounting.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/econ_eval/test_icer_nmb_for_disutility.py` & `deampy-1.3.2/tests/econ_eval/test_icer_nmb_for_disutility.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/econ_eval/test_icer_nmb_for_utility.py` & `deampy-1.3.2/tests/econ_eval/test_icer_nmb_for_utility.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/econ_eval/test_new_cea_simple.py` & `deampy-1.3.2/tests/econ_eval/test_new_cea_simple.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/econ_eval/test_new_cea_with_clouds.py` & `deampy-1.3.2/tests/econ_eval/test_new_cea_with_clouds.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/econ_eval/test_nmb_graph.py` & `deampy-1.3.2/tests/econ_eval/test_nmb_graph.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/input_output/test_csv_reader.py` & `deampy-1.3.2/tests/input_output/test_csv_reader.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/input_output/test_format_functions.py` & `deampy-1.3.2/tests/input_output/test_format_functions.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/markov/test_markov.py` & `deampy-1.3.2/tests/markov/test_markov.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/models/mortality_model.py` & `deampy-1.3.2/tests/models/mortality_model.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/optimization/test_opt_constrained.py` & `deampy-1.3.2/tests/optimization/test_opt_constrained.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/optimization/test_opt_unconstrained.py` & `deampy-1.3.2/tests/optimization/test_opt_unconstrained.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/optimization/toy_model.py` & `deampy-1.3.2/tests/optimization/toy_model.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/plots/plot_pyramids.py` & `deampy-1.3.2/tests/plots/plot_pyramids.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/plots/test_histograms.py` & `deampy-1.3.2/tests/plots/test_histograms.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/prob_dists/fit_dist_tests.py` & `deampy-1.3.2/tests/prob_dists/fit_dist_tests.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/prob_dists/rvg_tests.py` & `deampy-1.3.2/tests/prob_dists/rvg_tests.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/prob_dists/test_fitting_prob_dists.py` & `deampy-1.3.2/tests/prob_dists/test_fitting_prob_dists.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/prob_dists/test_rvgs.py` & `deampy-1.3.2/tests/prob_dists/test_rvgs.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/regression/test_exp_reg.py` & `deampy-1.3.2/tests/regression/test_exp_reg.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/regression/test_poly_ref_with_interval.py` & `deampy-1.3.2/tests/regression/test_poly_ref_with_interval.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/regression/test_poly_reg.py` & `deampy-1.3.2/tests/regression/test_poly_reg.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/regression/test_polynomial_q.py` & `deampy-1.3.2/tests/regression/test_polynomial_q.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/regression/test_regression.py` & `deampy-1.3.2/tests/regression/test_regression.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/sample_paths/test_incidence.py` & `deampy-1.3.2/tests/sample_paths/test_incidence.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/sample_paths/test_prev_pyramid.py` & `deampy-1.3.2/tests/sample_paths/test_prev_pyramid.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/sample_paths/test_prevalence.py` & `deampy-1.3.2/tests/sample_paths/test_prevalence.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/senstivity_analysis/test_rank_corr.py` & `deampy-1.3.2/tests/senstivity_analysis/test_rank_corr.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.1/tests/senstivity_analysis/test_sa.py` & `deampy-1.3.2/tests/senstivity_analysis/test_sa.py`

 * *Files identical despite different names*

