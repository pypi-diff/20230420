# Comparing `tmp/sig-decomp-0.0.2.tar.gz` & `tmp/sig-decomp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sig-decomp-0.0.2.tar", last modified: Thu Mar 23 16:50:15 2023, max compression
+gzip compressed data, was "sig-decomp-0.1.1.tar", last modified: Thu Apr 20 21:41:11 2023, max compression
```

## Comparing `sig-decomp-0.0.2.tar` & `sig-decomp-0.1.1.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 16:50:15.314451 sig-decomp-0.0.2/
--rw-r--r--   0 root         (0) root         (0)     1521 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2790 2023-03-23 16:50:15.314451 sig-decomp-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2521 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 16:50:15.302451 sig-decomp-0.0.2/gfosd/
--rw-r--r--   0 root         (0) root         (0)       33 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/gfosd/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 16:50:15.302451 sig-decomp-0.0.2/gfosd/components/
--rw-r--r--   0 root         (0) root         (0)      714 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/gfosd/components/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3183 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/gfosd/components/aggregate.py
--rw-r--r--   0 root         (0) root         (0)     4673 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/gfosd/components/base_graph_class.py
--rw-r--r--   0 root         (0) root         (0)     1876 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/gfosd/components/basis_constraints.py
--rw-r--r--   0 root         (0) root         (0)     4069 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/gfosd/components/equality_constraints.py
--rw-r--r--   0 root         (0) root         (0)      676 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/gfosd/components/finite_set.py
--rw-r--r--   0 root         (0) root         (0)     1147 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/gfosd/components/inequality_constraints.py
--rw-r--r--   0 root         (0) root         (0)     1568 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/gfosd/components/sums.py
--rw-r--r--   0 root         (0) root         (0)    10794 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/gfosd/problem.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 16:50:15.302451 sig-decomp-0.0.2/osd/
--rw-r--r--   0 root         (0) root         (0)       31 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 16:50:15.310451 sig-decomp-0.0.2/osd/classes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 16:50:15.310451 sig-decomp-0.0.2/osd/classes/C/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/classes/C/__init__.py
--rw-r--r--   0 root         (0) root         (0)      694 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/classes/C/make_l1_trend_module.py
--rw-r--r--   0 root         (0) root         (0)      964 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/classes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1541 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/classes/approx_periodic.py
--rw-r--r--   0 root         (0) root         (0)     1908 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/classes/asymmetric_noise.py
--rw-r--r--   0 root         (0) root         (0)     5415 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/classes/base_graph_class.py
--rw-r--r--   0 root         (0) root         (0)      527 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/classes/blank.py
--rw-r--r--   0 root         (0) root         (0)      890 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/classes/boolean.py
--rw-r--r--   0 root         (0) root         (0)     4788 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/classes/component.py
--rw-r--r--   0 root         (0) root         (0)     3089 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/classes/constant.py
--rw-r--r--   0 root         (0) root         (0)     1822 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/classes/frozen.py
--rw-r--r--   0 root         (0) root         (0)     1631 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/classes/linear_trend.py
--rw-r--r--   0 root         (0) root         (0)     3012 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/classes/markov.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/classes/mean_square_small.py
--rw-r--r--   0 root         (0) root         (0)     4107 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/classes/norm1_first.py
--rw-r--r--   0 root         (0) root         (0)     7772 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/classes/norm1_second.py
--rw-r--r--   0 root         (0) root         (0)     4946 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/classes/one_jump.py
--rw-r--r--   0 root         (0) root         (0)     4547 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/classes/piecewise_constant.py
--rw-r--r--   0 root         (0) root         (0)     4085 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/classes/quad_lin.py
--rw-r--r--   0 root         (0) root         (0)      981 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/classes/quadlin_utilities.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/classes/smooth_first.py
--rw-r--r--   0 root         (0) root         (0)     5360 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/classes/smooth_second.py
--rw-r--r--   0 root         (0) root         (0)     5208 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/classes/sparse.py
--rw-r--r--   0 root         (0) root         (0)    12828 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/classes/time_smooth_entry_close.py
--rw-r--r--   0 root         (0) root         (0)     2696 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/classes/wrappers.py
--rw-r--r--   0 root         (0) root         (0)     3257 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/generators.py
--rw-r--r--   0 root         (0) root         (0)     2731 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/masking.py
--rw-r--r--   0 root         (0) root         (0)     1025 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/polish.py
--rw-r--r--   0 root         (0) root         (0)    14616 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/problem.py
--rw-r--r--   0 root         (0) root         (0)     4894 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/signal_decomp_admm.py
--rw-r--r--   0 root         (0) root         (0)     2687 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/signal_decomp_bcd.py
--rw-r--r--   0 root         (0) root         (0)     4100 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/utilities.py
--rw-r--r--   0 root         (0) root         (0)     2110 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/osd/validation.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-23 16:50:15.314451 sig-decomp-0.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      619 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 16:50:15.310451 sig-decomp-0.0.2/sig_decomp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2790 2023-03-23 16:50:15.000000 sig-decomp-0.0.2/sig_decomp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1586 2023-03-23 16:50:15.000000 sig-decomp-0.0.2/sig_decomp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-23 16:50:15.000000 sig-decomp-0.0.2/sig_decomp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-03-23 16:50:15.000000 sig-decomp-0.0.2/sig_decomp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-03-23 16:50:15.000000 sig-decomp-0.0.2/sig_decomp.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 16:50:15.310451 sig-decomp-0.0.2/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 16:50:15.310451 sig-decomp-0.0.2/tests/osd/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/tests/osd/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4595 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/tests/osd/test_cols_equal.py
--rw-r--r--   0 root         (0) root         (0)     3812 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/tests/osd/test_masking_operators.py
--rw-r--r--   0 root         (0) root         (0)     6002 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/tests/osd/test_sine_square.py
--rw-r--r--   0 root         (0) root         (0)     2874 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/tests/osd/test_vector_periodic_problem.py
--rw-r--r--   0 root         (0) root         (0)     4403 2023-03-23 16:49:58.000000 sig-decomp-0.0.2/tests/osd/test_vector_problem.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 21:41:11.129964 sig-decomp-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)     1521 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2790 2023-04-20 21:41:11.129964 sig-decomp-0.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2521 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 21:41:11.125964 sig-decomp-0.1.1/gfosd/
+-rw-r--r--   0 root         (0) root         (0)       33 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/gfosd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 21:41:11.125964 sig-decomp-0.1.1/gfosd/components/
+-rw-r--r--   0 root         (0) root         (0)      779 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/gfosd/components/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3183 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/gfosd/components/aggregate.py
+-rw-r--r--   0 root         (0) root         (0)     4673 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/gfosd/components/base_graph_class.py
+-rw-r--r--   0 root         (0) root         (0)     1876 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/gfosd/components/basis_constraints.py
+-rw-r--r--   0 root         (0) root         (0)     4873 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/gfosd/components/equality_constraints.py
+-rw-r--r--   0 root         (0) root         (0)      676 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/gfosd/components/finite_set.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/gfosd/components/inequality_constraints.py
+-rw-r--r--   0 root         (0) root         (0)     1568 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/gfosd/components/sums.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/gfosd/data_generators.py
+-rw-r--r--   0 root         (0) root         (0)    11024 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/gfosd/problem.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 21:41:11.125964 sig-decomp-0.1.1/osd/
+-rw-r--r--   0 root         (0) root         (0)       31 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 21:41:11.125964 sig-decomp-0.1.1/osd/classes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 21:41:11.129964 sig-decomp-0.1.1/osd/classes/C/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/classes/C/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      694 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/classes/C/make_l1_trend_module.py
+-rw-r--r--   0 root         (0) root         (0)      964 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/classes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1541 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/classes/approx_periodic.py
+-rw-r--r--   0 root         (0) root         (0)     1908 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/classes/asymmetric_noise.py
+-rw-r--r--   0 root         (0) root         (0)     5415 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/classes/base_graph_class.py
+-rw-r--r--   0 root         (0) root         (0)      527 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/classes/blank.py
+-rw-r--r--   0 root         (0) root         (0)      890 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/classes/boolean.py
+-rw-r--r--   0 root         (0) root         (0)     4788 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/classes/component.py
+-rw-r--r--   0 root         (0) root         (0)     3089 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/classes/constant.py
+-rw-r--r--   0 root         (0) root         (0)     1822 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/classes/frozen.py
+-rw-r--r--   0 root         (0) root         (0)     1631 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/classes/linear_trend.py
+-rw-r--r--   0 root         (0) root         (0)     3012 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/classes/markov.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/classes/mean_square_small.py
+-rw-r--r--   0 root         (0) root         (0)     4107 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/classes/norm1_first.py
+-rw-r--r--   0 root         (0) root         (0)     7772 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/classes/norm1_second.py
+-rw-r--r--   0 root         (0) root         (0)     4946 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/classes/one_jump.py
+-rw-r--r--   0 root         (0) root         (0)     4547 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/classes/piecewise_constant.py
+-rw-r--r--   0 root         (0) root         (0)     4085 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/classes/quad_lin.py
+-rw-r--r--   0 root         (0) root         (0)      981 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/classes/quadlin_utilities.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/classes/smooth_first.py
+-rw-r--r--   0 root         (0) root         (0)     5360 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/classes/smooth_second.py
+-rw-r--r--   0 root         (0) root         (0)     5208 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/classes/sparse.py
+-rw-r--r--   0 root         (0) root         (0)    12828 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/classes/time_smooth_entry_close.py
+-rw-r--r--   0 root         (0) root         (0)     2696 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/classes/wrappers.py
+-rw-r--r--   0 root         (0) root         (0)     3257 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/generators.py
+-rw-r--r--   0 root         (0) root         (0)     2731 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/masking.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/polish.py
+-rw-r--r--   0 root         (0) root         (0)    14616 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/problem.py
+-rw-r--r--   0 root         (0) root         (0)     4894 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/signal_decomp_admm.py
+-rw-r--r--   0 root         (0) root         (0)     2687 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/signal_decomp_bcd.py
+-rw-r--r--   0 root         (0) root         (0)     4100 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/osd/validation.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 21:41:11.129964 sig-decomp-0.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      619 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 21:41:11.129964 sig-decomp-0.1.1/sig_decomp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2790 2023-04-20 21:41:11.000000 sig-decomp-0.1.1/sig_decomp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-04-20 21:41:11.000000 sig-decomp-0.1.1/sig_decomp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 21:41:11.000000 sig-decomp-0.1.1/sig_decomp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-04-20 21:41:11.000000 sig-decomp-0.1.1/sig_decomp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-20 21:41:11.000000 sig-decomp-0.1.1/sig_decomp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 21:41:11.129964 sig-decomp-0.1.1/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 21:41:11.129964 sig-decomp-0.1.1/tests/osd/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/tests/osd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4595 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/tests/osd/test_cols_equal.py
+-rw-r--r--   0 root         (0) root         (0)     3812 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/tests/osd/test_masking_operators.py
+-rw-r--r--   0 root         (0) root         (0)     6002 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/tests/osd/test_sine_square.py
+-rw-r--r--   0 root         (0) root         (0)     2874 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/tests/osd/test_vector_periodic_problem.py
+-rw-r--r--   0 root         (0) root         (0)     4403 2023-04-20 21:40:58.000000 sig-decomp-0.1.1/tests/osd/test_vector_problem.py
```

### Comparing `sig-decomp-0.0.2/LICENSE` & `sig-decomp-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/PKG-INFO` & `sig-decomp-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sig-decomp
-Version: 0.0.2
+Version: 0.1.1
 Summary: Optimzation-based signal decomposition
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sig-decomp-0.0.2/README.md` & `sig-decomp-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/gfosd/components/__init__.py` & `sig-decomp-0.1.1/gfosd/components/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,10 +4,11 @@
                                    SumQuantile,
                                    SumCard)
 from gfosd.components.inequality_constraints import Inequality
 from gfosd.components.basis_constraints import Basis, Periodic
 from gfosd.components.finite_set import FiniteSet, Boolean
 from gfosd.components.aggregate import Aggregate
 from gfosd.components.equality_constraints import (FirstValEqual,
+                                                   LastValEqual,
                                                    AverageEqual,
                                                    NoCurvature,
                                                    NoSlope)
```

### Comparing `sig-decomp-0.0.2/gfosd/components/aggregate.py` & `sig-decomp-0.1.1/gfosd/components/aggregate.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/gfosd/components/base_graph_class.py` & `sig-decomp-0.1.1/gfosd/components/base_graph_class.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/gfosd/components/basis_constraints.py` & `sig-decomp-0.1.1/gfosd/components/basis_constraints.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/gfosd/components/equality_constraints.py` & `sig-decomp-0.1.1/gfosd/components/equality_constraints.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,41 @@
             [self._B.tocsr()[0]],
             [sp.coo_matrix(([1], ([0], [0])), shape=(1, self._B.shape[1]))]
         ])
 
     def _make_c(self):
         self._c = np.concatenate([np.atleast_1d(self._c[0]),
                                   [self._first_val]])
+        
+class LastValEqual(GraphComponent):
+    def __init__(self, value=0, *args, **kwargs):
+        self._last_val = value
+        super().__init__(*args, **kwargs)
+        # always retain helper variable
+        self._has_helpers = True
+
+    def _make_A(self):
+        super()._make_A()
+        super()._make_B()
+        super()._make_c()
+        self._A = sp.bmat([
+           [self._A.tocsr()[-1]],
+            [sp.dok_matrix((1, self._A.shape[1]))]
+        ])
 
+    def _make_B(self):
+        self._B = sp.bmat([
+           [self._B.tocsr()[-1]],
+            [sp.coo_matrix(([1], ([0], [self._B.shape[1]-1])), shape=(1, self._B.shape[1]))]
+        ])
+
+    def _make_c(self):
+        self._c = np.concatenate([np.atleast_1d(self._c[-1]),
+                                  [self._last_val]])
+        
 class AverageEqual(GraphComponent):
     def __init__(self, value=0, period=None, *args, **kwargs):
         self._avg_val = value
         self._period = period
         super().__init__(*args, **kwargs)
         # always retain helper variable, i.e. don't allow the Aggregate class
         # to try to remove variables.
```

### Comparing `sig-decomp-0.0.2/gfosd/components/finite_set.py` & `sig-decomp-0.1.1/gfosd/components/finite_set.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/gfosd/components/inequality_constraints.py` & `sig-decomp-0.1.1/gfosd/components/inequality_constraints.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/gfosd/components/sums.py` & `sig-decomp-0.1.1/gfosd/components/sums.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/gfosd/problem.py` & `sig-decomp-0.1.1/gfosd/problem.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,21 @@
         self.decompose(solver=solver, make_feasible=make_feasible, **kwargs)
         residual = (self.data[hold_set]
                     - np.sum(self.decomposition, axis=0)[hold_set])
         self.mask = self.__old_mask
         return residual, test_ixs
 
     def _solve_qss(self, data, **solver_kwargs):
-        solver = qss.QSS(data)
+        if self._qss_obj is not None and 'warm_start' in solver_kwargs:
+            if solver_kwargs['warm_start']:
+                solver = self._qss_obj
+            else:
+                solver = qss.QSS(data)
+        else:
+            solver = qss.QSS(data)
         objval, soln = solver.solve(**solver_kwargs)
         self._qss_soln = soln
         self.objective_value = objval
         self._qss_obj = solver
         # print(soln.T @ data['P'] @ soln)
         return soln
```

### Comparing `sig-decomp-0.0.2/osd/classes/C/make_l1_trend_module.py` & `sig-decomp-0.1.1/osd/classes/C/make_l1_trend_module.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/osd/classes/__init__.py` & `sig-decomp-0.1.1/osd/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/osd/classes/approx_periodic.py` & `sig-decomp-0.1.1/osd/classes/approx_periodic.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/osd/classes/asymmetric_noise.py` & `sig-decomp-0.1.1/osd/classes/asymmetric_noise.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/osd/classes/base_graph_class.py` & `sig-decomp-0.1.1/osd/classes/base_graph_class.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/osd/classes/blank.py` & `sig-decomp-0.1.1/osd/classes/blank.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/osd/classes/boolean.py` & `sig-decomp-0.1.1/osd/classes/boolean.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/osd/classes/component.py` & `sig-decomp-0.1.1/osd/classes/component.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/osd/classes/constant.py` & `sig-decomp-0.1.1/osd/classes/constant.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/osd/classes/frozen.py` & `sig-decomp-0.1.1/osd/classes/frozen.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/osd/classes/linear_trend.py` & `sig-decomp-0.1.1/osd/classes/linear_trend.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/osd/classes/markov.py` & `sig-decomp-0.1.1/osd/classes/markov.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/osd/classes/mean_square_small.py` & `sig-decomp-0.1.1/osd/classes/mean_square_small.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/osd/classes/norm1_first.py` & `sig-decomp-0.1.1/osd/classes/norm1_first.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/osd/classes/norm1_second.py` & `sig-decomp-0.1.1/osd/classes/norm1_second.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/osd/classes/one_jump.py` & `sig-decomp-0.1.1/osd/classes/one_jump.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/osd/classes/piecewise_constant.py` & `sig-decomp-0.1.1/osd/classes/piecewise_constant.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/osd/classes/quad_lin.py` & `sig-decomp-0.1.1/osd/classes/quad_lin.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/osd/classes/quadlin_utilities.py` & `sig-decomp-0.1.1/osd/classes/quadlin_utilities.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/osd/classes/smooth_first.py` & `sig-decomp-0.1.1/osd/classes/smooth_first.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/osd/classes/smooth_second.py` & `sig-decomp-0.1.1/osd/classes/smooth_second.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/osd/classes/sparse.py` & `sig-decomp-0.1.1/osd/classes/sparse.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/osd/classes/time_smooth_entry_close.py` & `sig-decomp-0.1.1/osd/classes/time_smooth_entry_close.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/osd/classes/wrappers.py` & `sig-decomp-0.1.1/osd/classes/wrappers.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/osd/generators.py` & `sig-decomp-0.1.1/osd/generators.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/osd/masking.py` & `sig-decomp-0.1.1/osd/masking.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/osd/polish.py` & `sig-decomp-0.1.1/osd/polish.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/osd/problem.py` & `sig-decomp-0.1.1/osd/problem.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/osd/signal_decomp_admm.py` & `sig-decomp-0.1.1/osd/signal_decomp_admm.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/osd/signal_decomp_bcd.py` & `sig-decomp-0.1.1/osd/signal_decomp_bcd.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/osd/utilities.py` & `sig-decomp-0.1.1/osd/utilities.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/osd/validation.py` & `sig-decomp-0.1.1/osd/validation.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/sig_decomp.egg-info/PKG-INFO` & `sig-decomp-0.1.1/sig_decomp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sig-decomp
-Version: 0.0.2
+Version: 0.1.1
 Summary: Optimzation-based signal decomposition
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sig-decomp-0.0.2/sig_decomp.egg-info/SOURCES.txt` & `sig-decomp-0.1.1/sig_decomp.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 gfosd/__init__.py
+gfosd/data_generators.py
 gfosd/problem.py
 gfosd/components/__init__.py
 gfosd/components/aggregate.py
 gfosd/components/base_graph_class.py
 gfosd/components/basis_constraints.py
 gfosd/components/equality_constraints.py
 gfosd/components/finite_set.py
```

### Comparing `sig-decomp-0.0.2/tests/osd/test_cols_equal.py` & `sig-decomp-0.1.1/tests/osd/test_cols_equal.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/tests/osd/test_masking_operators.py` & `sig-decomp-0.1.1/tests/osd/test_masking_operators.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/tests/osd/test_sine_square.py` & `sig-decomp-0.1.1/tests/osd/test_sine_square.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/tests/osd/test_vector_periodic_problem.py` & `sig-decomp-0.1.1/tests/osd/test_vector_periodic_problem.py`

 * *Files identical despite different names*

### Comparing `sig-decomp-0.0.2/tests/osd/test_vector_problem.py` & `sig-decomp-0.1.1/tests/osd/test_vector_problem.py`

 * *Files identical despite different names*

