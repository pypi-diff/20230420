# Comparing `tmp/optax-0.1.4.tar.gz` & `tmp/optax-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optax-0.1.4.tar", last modified: Mon Nov 21 13:45:06 2022, max compression
+gzip compressed data, was "optax-0.1.5.tar", last modified: Thu Apr 20 14:42:18 2023, max compression
```

## Comparing `optax-0.1.4.tar` & `optax-0.1.5.tar`

### file list

```diff
@@ -1,86 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 13:45:06.137469 optax-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-11-21 13:44:54.000000 optax-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-11-21 13:44:54.000000 optax-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    12297 2022-11-21 13:45:06.137469 optax-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11394 2022-11-21 13:44:54.000000 optax-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 13:45:06.125468 optax-0.1.4/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     8850 2022-11-21 13:44:54.000000 optax-0.1.4/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 13:45:06.125468 optax-0.1.4/docs/ext/
--rw-r--r--   0 runner    (1001) docker     (121)     2041 2022-11-21 13:44:54.000000 optax-0.1.4/docs/ext/coverage_check.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 13:45:06.129469 optax-0.1.4/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-11-21 13:44:54.000000 optax-0.1.4/examples/datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)     2947 2022-11-21 13:44:54.000000 optax-0.1.4/examples/datasets_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     6545 2022-11-21 13:44:54.000000 optax-0.1.4/examples/differentially_private_sgd.py
--rw-r--r--   0 runner    (1001) docker     (121)     3244 2022-11-21 13:44:54.000000 optax-0.1.4/examples/flax_example.py
--rw-r--r--   0 runner    (1001) docker     (121)     2680 2022-11-21 13:44:54.000000 optax-0.1.4/examples/haiku_example.py
--rw-r--r--   0 runner    (1001) docker     (121)     3304 2022-11-21 13:44:54.000000 optax-0.1.4/examples/lookahead_mnist.py
--rw-r--r--   0 runner    (1001) docker     (121)     1744 2022-11-21 13:44:54.000000 optax-0.1.4/examples/lookahead_mnist_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4299 2022-11-21 13:44:54.000000 optax-0.1.4/examples/mnist.py
--rw-r--r--   0 runner    (1001) docker     (121)     2970 2022-11-21 13:44:54.000000 optax-0.1.4/examples/mnist_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 13:45:06.129469 optax-0.1.4/optax/
--rw-r--r--   0 runner    (1001) docker     (121)    12439 2022-11-21 13:44:54.000000 optax-0.1.4/optax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 13:45:06.137469 optax-0.1.4/optax/_src/
--rw-r--r--   0 runner    (1001) docker     (121)    35001 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/alias.py
--rw-r--r--   0 runner    (1001) docker     (121)     7071 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/alias_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     8342 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4728 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/base_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     7502 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/clipping.py
--rw-r--r--   0 runner    (1001) docker     (121)     3769 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/clipping_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     5698 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/combine.py
--rw-r--r--   0 runner    (1001) docker     (121)     5263 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/combine_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3242 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/constrain.py
--rw-r--r--   0 runner    (1001) docker     (121)     4201 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/constrain_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    17504 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/control_variates.py
--rw-r--r--   0 runner    (1001) docker     (121)    21789 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/control_variates_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     5952 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/equivalence_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 13:45:06.137469 optax-0.1.4/optax/_src/experimental/
--rw-r--r--   0 runner    (1001) docker     (121)     4101 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/experimental/complex_valued.py
--rw-r--r--   0 runner    (1001) docker     (121)     2870 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/experimental/complex_valued_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     6268 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/experimental/extra_args.py
--rw-r--r--   0 runner    (1001) docker     (121)     2042 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/experimental/extra_args_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     7404 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/factorized.py
--rw-r--r--   0 runner    (1001) docker     (121)     1552 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/factorized_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3783 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/float64_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     7498 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/linear_algebra.py
--rw-r--r--   0 runner    (1001) docker     (121)     2177 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/linear_algebra_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     7447 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/lookahead.py
--rw-r--r--   0 runner    (1001) docker     (121)     5385 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/lookahead_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    20353 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/loss.py
--rw-r--r--   0 runner    (1001) docker     (121)    17621 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/loss_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4643 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/numerics.py
--rw-r--r--   0 runner    (1001) docker     (121)     4177 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/numerics_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2731 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/privacy.py
--rw-r--r--   0 runner    (1001) docker     (121)     4560 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/privacy_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    22756 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/schedule.py
--rw-r--r--   0 runner    (1001) docker     (121)    24470 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/schedule_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3593 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/second_order.py
--rw-r--r--   0 runner    (1001) docker     (121)     3060 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/second_order_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    12277 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/stochastic_gradient_estimators.py
--rw-r--r--   0 runner    (1001) docker     (121)    13766 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/stochastic_gradient_estimators_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1458 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    37727 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/transform.py
--rw-r--r--   0 runner    (1001) docker     (121)    10335 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/transform_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3692 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/update.py
--rw-r--r--   0 runner    (1001) docker     (121)     2870 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/update_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4786 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2154 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    21080 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (121)    25489 2022-11-21 13:44:54.000000 optax-0.1.4/optax/_src/wrappers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 13:45:06.137469 optax-0.1.4/optax/experimental/
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-11-21 13:44:54.000000 optax-0.1.4/optax/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      986 2022-11-21 13:44:54.000000 optax-0.1.4/optax/optax_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 13:45:06.129469 optax-0.1.4/optax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12297 2022-11-21 13:45:06.000000 optax-0.1.4/optax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2025 2022-11-21 13:45:06.000000 optax-0.1.4/optax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-21 13:45:06.000000 optax-0.1.4/optax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-21 13:45:06.000000 optax-0.1.4/optax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-11-21 13:45:06.000000 optax-0.1.4/optax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-11-21 13:45:06.000000 optax-0.1.4/optax.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 13:45:06.137469 optax-0.1.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-11-21 13:44:54.000000 optax-0.1.4/requirements/minimum-requirements-dp-accounting.txt
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-11-21 13:44:54.000000 optax-0.1.4/requirements/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-11-21 13:44:54.000000 optax-0.1.4/requirements/requirements-examples.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-11-21 13:44:54.000000 optax-0.1.4/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-11-21 13:44:54.000000 optax-0.1.4/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-21 13:45:06.137469 optax-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2811 2022-11-21 13:44:54.000000 optax-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:42:18.392917 optax-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-20 14:42:04.000000 optax-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-20 14:42:04.000000 optax-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-04-20 14:42:18.392917 optax-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-04-20 14:42:04.000000 optax-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:42:18.384917 optax-0.1.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     8850 2023-04-20 14:42:04.000000 optax-0.1.5/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:42:18.384917 optax-0.1.5/docs/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-04-20 14:42:04.000000 optax-0.1.5/docs/ext/coverage_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:42:18.384917 optax-0.1.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-20 14:42:04.000000 optax-0.1.5/examples/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-20 14:42:04.000000 optax-0.1.5/examples/datasets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-04-20 14:42:04.000000 optax-0.1.5/examples/differentially_private_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-20 14:42:04.000000 optax-0.1.5/examples/flax_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-20 14:42:04.000000 optax-0.1.5/examples/haiku_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-20 14:42:04.000000 optax-0.1.5/examples/lookahead_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-20 14:42:04.000000 optax-0.1.5/examples/lookahead_mnist_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-04-20 14:42:04.000000 optax-0.1.5/examples/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-20 14:42:04.000000 optax-0.1.5/examples/mnist_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:42:18.384917 optax-0.1.5/optax/
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-20 14:42:04.000000 optax-0.1.5/optax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:42:18.388917 optax-0.1.5/optax/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)    37367 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/alias_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11453 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/clipping_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/combine_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/constrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/constrain_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17563 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/control_variates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21789 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/control_variates_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/equivalence_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:42:18.388917 optax-0.1.5/optax/_src/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/experimental/complex_valued.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/experimental/complex_valued_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/experimental/extra_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/experimental/extra_args_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/factorized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/factorized_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/float64_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/linear_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/linear_algebra_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/lookahead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/lookahead_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22680 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19278 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/loss_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/numerics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/numerics_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/privacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/privacy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23336 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25900 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/schedule_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/second_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/second_order_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/state_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/state_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/stochastic_gradient_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13766 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/stochastic_gradient_estimators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39085 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10403 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/transform_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/update_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21653 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26244 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/wrappers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:42:18.388917 optax-0.1.5/optax/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-20 14:42:04.000000 optax-0.1.5/optax/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-20 14:42:04.000000 optax-0.1.5/optax/optax_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:42:18.384917 optax-0.1.5/optax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-04-20 14:42:18.000000 optax-0.1.5/optax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-20 14:42:18.000000 optax-0.1.5/optax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:42:18.000000 optax-0.1.5/optax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:42:18.000000 optax-0.1.5/optax.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-20 14:42:18.000000 optax-0.1.5/optax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-20 14:42:18.000000 optax-0.1.5/optax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:42:18.388917 optax-0.1.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-20 14:42:04.000000 optax-0.1.5/requirements/minimum-requirements-dp-accounting.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-20 14:42:04.000000 optax-0.1.5/requirements/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-20 14:42:04.000000 optax-0.1.5/requirements/requirements-examples.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 14:42:04.000000 optax-0.1.5/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-20 14:42:04.000000 optax-0.1.5/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 14:42:18.392917 optax-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-20 14:42:04.000000 optax-0.1.5/setup.py
```

### Comparing `optax-0.1.4/LICENSE` & `optax-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `optax-0.1.4/PKG-INFO` & `optax-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optax
-Version: 0.1.4
+Version: 0.1.5
 Summary: A gradient processing and optimisation library in JAX.
 Home-page: https://github.com/deepmind/optax
 Author: DeepMind
 Author-email: optax-dev@google.com
 License: Apache 2.0
 Keywords: reinforcement-learning python machine learning
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Optax
 
 ![CI status](https://github.com/deepmind/optax/workflows/tests/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/optax/badge/?version=latest)](http://optax.readthedocs.io)
```

### Comparing `optax-0.1.4/README.md` & `optax-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `optax-0.1.4/docs/conf.py` & `optax-0.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.4/docs/ext/coverage_check.py` & `optax-0.1.5/docs/ext/coverage_check.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.4/examples/datasets.py` & `optax-0.1.5/examples/datasets.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.4/examples/datasets_test.py` & `optax-0.1.5/examples/datasets_test.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.4/examples/differentially_private_sgd.py` & `optax-0.1.5/examples/differentially_private_sgd.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.4/examples/flax_example.py` & `optax-0.1.5/examples/flax_example.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.4/examples/haiku_example.py` & `optax-0.1.5/examples/haiku_example.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.4/examples/lookahead_mnist.py` & `optax-0.1.5/examples/lookahead_mnist.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,12 +76,12 @@
 
     # Validation is done on the slow lookahead parameters.
     eval_model = functools.partial(apply_params_fn, params.slow)
     test_acc = mnist.model_accuracy(eval_model,
                                     test_dataset.as_numpy_iterator())
     print(f'Epoch {epoch+1}: test acc: {test_acc:.2f}')
 
-  return test_acc
+  return test_acc  # pytype: disable=bad-return-type  # numpy-scalars
 
 
 if __name__ == '__main__':
   app.run(main)
```

### Comparing `optax-0.1.4/examples/lookahead_mnist_test.py` & `optax-0.1.5/examples/lookahead_mnist_test.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.4/examples/mnist.py` & `optax-0.1.5/examples/mnist.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,15 +50,15 @@
   for batch in dataset:
     # Take batch size into account in case there is a smaller remainder batch.
     batch_size = batch['image'].shape[0]
     logits = model(batch['image'])
     accuracy_sum += _single_batch_accuracy(logits, batch['label']) * batch_size
     dataset_size += batch_size
 
-  return accuracy_sum / dataset_size
+  return accuracy_sum / dataset_size  # pytype: disable=bad-return-type  # numpy-scalars  # pylint: disable=line-too-long
 
 
 # Optax is agnostic to which (if any) neural network library is used. Below we
 # provide a Haiku version.
 def build_model(layer_dims: Sequence[int]) -> hk.Transformed:
   """Simple multi-layer perceptron model for image classification."""
 
@@ -107,15 +107,15 @@
     for batch in train_dataset.as_numpy_iterator():
       params, opt_state = train_step(params, opt_state, batch)
 
     eval_model = functools.partial(apply_params_fn, params)
     test_acc = model_accuracy(eval_model, test_dataset.as_numpy_iterator())
     print(f'Epoch {epoch+1}: test acc: {test_acc:.2f}')
 
-  return test_acc
+  return test_acc  # pytype: disable=bad-return-type  # numpy-scalars
 
 
 def main(unused_argv):
   """Trains an MLP on MNIST using the adam optimizers."""
   return train_on_mnist(optax.adam(LEARNING_RATE), DEFAULT_HIDDEN_SIZES)
```

### Comparing `optax-0.1.4/examples/mnist_test.py` & `optax-0.1.5/examples/mnist_test.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.4/optax/__init__.py` & `optax-0.1.5/optax/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,36 +23,40 @@
 from optax._src.alias import adamaxw
 from optax._src.alias import adamw
 from optax._src.alias import amsgrad
 from optax._src.alias import dpsgd
 from optax._src.alias import fromage
 from optax._src.alias import lamb
 from optax._src.alias import lars
+from optax._src.alias import lion
 from optax._src.alias import MaskOrFn
 from optax._src.alias import noisy_sgd
 from optax._src.alias import novograd
 from optax._src.alias import optimistic_gradient_descent
 from optax._src.alias import radam
 from optax._src.alias import rmsprop
 from optax._src.alias import ScalarOrSchedule
 from optax._src.alias import sgd
 from optax._src.alias import sm3
 from optax._src.alias import yogi
 from optax._src.base import EmptyState
 from optax._src.base import GradientTransformation
+from optax._src.base import GradientTransformationExtraArgs
 from optax._src.base import identity
 from optax._src.base import OptState
 from optax._src.base import Params
 from optax._src.base import Schedule
 from optax._src.base import set_to_zero
 from optax._src.base import stateless
 from optax._src.base import stateless_with_tree_map
 from optax._src.base import TransformInitFn
+from optax._src.base import TransformUpdateExtraArgsFn
 from optax._src.base import TransformUpdateFn
 from optax._src.base import Updates
+from optax._src.base import with_extra_args_support
 from optax._src.clipping import adaptive_grad_clip
 from optax._src.clipping import AdaptiveGradClipState
 from optax._src.clipping import clip
 from optax._src.clipping import clip_by_block_rms
 from optax._src.clipping import clip_by_global_norm
 from optax._src.clipping import ClipByGlobalNormState
 from optax._src.clipping import ClipState
@@ -71,26 +75,29 @@
 from optax._src.factorized import scale_by_factored_rms
 from optax._src.linear_algebra import global_norm
 from optax._src.linear_algebra import matrix_inverse_pth_root
 from optax._src.linear_algebra import power_iteration
 from optax._src.lookahead import lookahead
 from optax._src.lookahead import LookaheadParams
 from optax._src.lookahead import LookaheadState
+from optax._src.loss import convex_kl_divergence
 from optax._src.loss import cosine_distance
 from optax._src.loss import cosine_similarity
 from optax._src.loss import ctc_loss
 from optax._src.loss import ctc_loss_with_forward_probs
 from optax._src.loss import hinge_loss
 from optax._src.loss import huber_loss
+from optax._src.loss import kl_divergence
 from optax._src.loss import l2_loss
 from optax._src.loss import log_cosh
 from optax._src.loss import sigmoid_binary_cross_entropy
 from optax._src.loss import smooth_labels
 from optax._src.loss import softmax_cross_entropy
 from optax._src.loss import softmax_cross_entropy_with_integer_labels
+from optax._src.loss import squared_error
 from optax._src.numerics import safe_int32_increment
 from optax._src.numerics import safe_norm
 from optax._src.numerics import safe_root_mean_squares
 from optax._src.privacy import differentially_private_aggregate
 from optax._src.privacy import DifferentiallyPrivateAggregateState
 from optax._src.schedule import constant_schedule
 from optax._src.schedule import cosine_decay_schedule
@@ -106,14 +113,15 @@
 from optax._src.schedule import polynomial_schedule
 from optax._src.schedule import sgdr_schedule
 from optax._src.schedule import warmup_cosine_decay_schedule
 from optax._src.schedule import warmup_exponential_decay_schedule
 from optax._src.second_order import fisher_diag
 from optax._src.second_order import hessian_diag
 from optax._src.second_order import hvp
+from optax._src.state_utils import tree_map_params
 from optax._src.stochastic_gradient_estimators import measure_valued_jacobians
 from optax._src.stochastic_gradient_estimators import pathwise_jacobians
 from optax._src.stochastic_gradient_estimators import score_function_jacobians
 from optax._src.transform import add_decayed_weights
 from optax._src.transform import add_noise
 from optax._src.transform import AddDecayedWeightsState
 from optax._src.transform import additive_weight_decay
@@ -126,14 +134,15 @@
 from optax._src.transform import ema
 from optax._src.transform import EmaState
 from optax._src.transform import scale
 from optax._src.transform import scale_by_adam
 from optax._src.transform import scale_by_adamax
 from optax._src.transform import scale_by_amsgrad
 from optax._src.transform import scale_by_belief
+from optax._src.transform import scale_by_lion
 from optax._src.transform import scale_by_novograd
 from optax._src.transform import scale_by_optimistic_gradient
 from optax._src.transform import scale_by_param_block_norm
 from optax._src.transform import scale_by_param_block_rms
 from optax._src.transform import scale_by_radam
 from optax._src.transform import scale_by_rms
 from optax._src.transform import scale_by_rss
@@ -141,15 +150,15 @@
 from optax._src.transform import scale_by_sm3
 from optax._src.transform import scale_by_stddev
 from optax._src.transform import scale_by_trust_ratio
 from optax._src.transform import scale_by_yogi
 from optax._src.transform import ScaleByAdamState
 from optax._src.transform import ScaleByAmsgradState
 from optax._src.transform import ScaleByBeliefState
-from optax._src.transform import ScaleByFromageState
+from optax._src.transform import ScaleByLionState
 from optax._src.transform import ScaleByNovogradState
 from optax._src.transform import ScaleByRmsState
 from optax._src.transform import ScaleByRssState
 from optax._src.transform import ScaleByRStdDevState
 from optax._src.transform import ScaleByScheduleState
 from optax._src.transform import ScaleBySM3State
 from optax._src.transform import ScaleByTrustRatioState
@@ -174,15 +183,15 @@
 from optax._src.wrappers import MaybeUpdateState
 from optax._src.wrappers import MultiSteps
 from optax._src.wrappers import MultiStepsState
 from optax._src.wrappers import ShouldSkipUpdateFunction
 from optax._src.wrappers import skip_large_updates
 from optax._src.wrappers import skip_not_finite
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
 
 __all__ = (
     "adabelief",
     "adafactor",
     "adagrad",
     "adam",
     "adamax",
@@ -210,14 +219,15 @@
     "ClipByGlobalNormState",
     "ClipState",
     "constant_schedule",
     "ctc_loss",
     "ctc_loss_with_forward_probs",
     "control_delta_method",
     "control_variates_jacobians",
+    "convex_kl_divergence",
     "cosine_decay_schedule",
     "cosine_distance",
     "cosine_onecycle_schedule",
     "cosine_similarity",
     "differentially_private_aggregate",
     "DifferentiallyPrivateAggregateState",
     "dpsgd",
@@ -227,27 +237,30 @@
     "exponential_decay",
     "FactoredState",
     "fisher_diag",
     "flatten",
     "fromage",
     "global_norm",
     "GradientTransformation",
+    "GradientTransformationExtraArgs",
     "hinge_loss",
     "hessian_diag",
     "huber_loss",
     "hvp",
     "identity",
     "incremental_update",
     "inject_hyperparams",
     "InjectHyperparamsState",
     "join_schedules",
     "keep_params_nonnegative",
+    "kl_divergence",
     "l2_loss",
     "lamb",
     "lars",
+    "lion",
     "linear_onecycle_schedule",
     "linear_schedule",
     "log_cosh",
     "lookahead",
     "LookaheadParams",
     "LookaheadState",
     "masked",
@@ -281,14 +294,15 @@
     "safe_norm",
     "safe_root_mean_squares",
     "ScalarOrSchedule",
     "scale_by_adam",
     "scale_by_adamax",
     "scale_by_amsgrad",
     "scale_by_belief",
+    "scale_by_lion",
     "scale_by_factored_rms",
     "scale_by_novograd",
     "scale_by_param_block_norm",
     "scale_by_param_block_rms",
     "scale_by_radam",
     "scale_by_rms",
     "scale_by_rss",
@@ -298,15 +312,15 @@
     "scale_by_trust_ratio",
     "scale_by_yogi",
     "scale_gradient",
     "scale",
     "ScaleByAdamState",
     "ScaleByAmsgradState",
     "ScaleByBeliefState",
-    "ScaleByFromageState",
+    "ScaleByLionState",
     "ScaleByNovogradState",
     "ScaleByRmsState",
     "ScaleByRssState",
     "ScaleByRStdDevState",
     "ScaleByScheduleState",
     "ScaleBySM3State",
     "ScaleByTrustRatioState",
@@ -319,20 +333,22 @@
     "ShouldSkipUpdateFunction",
     "sigmoid_binary_cross_entropy",
     "skip_large_updates",
     "skip_not_finite",
     "sm3",
     "smooth_labels",
     "softmax_cross_entropy",
+    "softmax_cross_entropy_with_integer_labels",
     "stateless",
     "stateless_with_tree_map",
     "trace",
     "TraceState",
     "TransformInitFn",
     "TransformUpdateFn",
+    "TransformUpdateExtraArgsFn",
     "Updates",
     "warmup_cosine_decay_schedule",
     "warmup_exponential_decay_schedule",
     "yogi",
     "zero_nans",
     "ZeroNansState",
 )
```

### Comparing `optax-0.1.4/optax/_src/alias.py` & `optax-0.1.5/optax/_src/alias.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,26 +12,27 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Aliases for popular optimizers."""
 
 from typing import Any, Callable, Optional, Union
 
+import jax
 import jax.numpy as jnp
 
 from optax._src import base
 from optax._src import clipping
 from optax._src import combine
 from optax._src import factorized
 from optax._src import privacy
 from optax._src import transform
 from optax._src import wrappers
 
 
-ScalarOrSchedule = Union[float, base.Schedule]
+ScalarOrSchedule = Union[float, jax.Array, base.Schedule]
 MaskOrFn = Optional[Union[Any, Callable[[base.Params], Any]]]
 
 
 def _scale_by_learning_rate(learning_rate: ScalarOrSchedule, flip_sign=True):
   m = -1 if flip_sign else 1
   if callable(learning_rate):
     return transform.scale_by_schedule(lambda count: m * learning_rate(count))
@@ -298,14 +299,62 @@
       transform.scale_by_adam(
           b1=b1, b2=b2, eps=eps, eps_root=eps_root, mu_dtype=mu_dtype),
       transform.add_decayed_weights(weight_decay, mask),
       _scale_by_learning_rate(learning_rate),
   )
 
 
+def lion(
+    learning_rate: ScalarOrSchedule,
+    b1: float = 0.9,
+    b2: float = 0.99,
+    mu_dtype: Optional[Any] = None,
+    weight_decay: float = 1e-3,
+    mask: Optional[Union[Any, Callable[[base.Params], Any]]] = None,
+) -> base.GradientTransformation:
+  """The Lion optimizer.
+
+  Lion is discovered by symbolic program search. Unlike most adaptive optimizers
+  such as AdamW, Lion only tracks momentum, making it more memory-efficient.
+  The update of Lion is produced through the sign operation, resulting in a
+  larger norm compared to updates produced by other optimizers such as SGD and
+  AdamW. A suitable learning rate for Lion is typically 3-10x smaller than that
+  for AdamW, the weight decay for Lion should be in turn 3-10x larger than that
+  for AdamW to maintain a similar strength (lr * wd).
+
+  References:
+    Chen et al, 2023: https://arxiv.org/abs/2302.06675
+
+  Args:
+    learning_rate: A fixed global scaling factor.
+    b1: Rate to combine the momentum and the current gradient.
+    b2: Exponential decay rate to track the momentum of past gradients.
+    mu_dtype: Optional `dtype` to be used for the first order accumulator; if
+      `None` then the `dtype` is inferred from `params` and `updates`.
+    weight_decay: Strength of the weight decay regularization. Note that this
+      weight decay is multiplied with the learning rate. This is consistent
+      with other frameworks such as PyTorch, but different from
+      (Loshchilov et al, 2019) where the weight decay is only multiplied with
+      the "schedule multiplier", but not the base learning rate.
+    mask: A tree with same structure as (or a prefix of) the params PyTree,
+      or a Callable that returns such a pytree given the params/updates.
+      The leaves should be booleans, `True` for leaves/subtrees you want to
+      apply the weight decay to, and `False` for those you want to skip. Note
+      that the Adam gradient transformations are applied to all parameters.
+
+  Returns:
+    The corresponding `GradientTransformation`.
+  """
+  return combine.chain(
+      transform.scale_by_lion(b1=b1, b2=b2, mu_dtype=mu_dtype),
+      transform.add_decayed_weights(weight_decay, mask),
+      _scale_by_learning_rate(learning_rate),
+  )
+
+
 def amsgrad(
     learning_rate: ScalarOrSchedule,
     b1: float = 0.9,
     b2: float = 0.999,
     eps: float = 1e-8,
     eps_root: float = 0.0,
     mu_dtype: Optional[Any] = None,
@@ -548,15 +597,15 @@
 
   Optimistic gradient descent is an approximation of extra-gradient methods
   which require multiple gradient calls to compute the next update. It has
   strong formal guarantees for last-iterate convergence in min-max games, for
   which standard gradient descent can oscillate or even diverge.
 
   References:
-    [Mokhtari et al, 2019](https://arxiv.org/abs/1901.08511v2)
+    Mokhtari et al, 2019: https://arxiv.org/abs/1901.08511v2
 
   Args:
     learning_rate: A fixed global scaling factor.
     alpha: Coefficient for generalized OGD.
     beta: Coefficient for generalized OGD negative momentum.
 
   Returns:
@@ -731,35 +780,37 @@
 
 def yogi(
     learning_rate: ScalarOrSchedule,
     b1: float = 0.9,
     b2: float = 0.999,
     eps: float = 1e-3,
 ) -> base.GradientTransformation:
+  # pylint: disable=line-too-long
   """The Yogi optimizer.
 
   Yogi is an adaptive optimizer, which provides control in tuning the effective
   learning rate to prevent it from increasing. By doing so, it focuses on
   addressing the issues of convergence and generalization in exponential moving
   average-based adaptive methods (such as Adam and RMSprop). Yogi is a
   modification of Adam and uses the same parameters.
 
   References:
-    Zaheer et al, 2020: http://www.sanjivk.com/yogi_nips2018.pdf
+    Zaheer et al, 2018: https://proceedings.neurips.cc/paper/2018/file/90365351ccc7437a1309dc64e4db32a3-Paper.pdf
 
   Args:
     learning_rate: A fixed global scaling factor.
     b1: Exponential decay rate to track the first moment of past gradients.
     b2: Exponential decay rate to track the second moment of past gradients.
     eps: A small constant applied to denominator outside of the square root
       (as in the Adam paper) to avoid dividing by zero when rescaling.
 
   Returns:
     The corresponding `GradientTransformation`.
   """
+  # pylint: enable=line-too-long
   return combine.chain(
       transform.scale_by_yogi(b1=b1, b2=b2, eps=eps),
       _scale_by_learning_rate(learning_rate),
   )
 
 
 def dpsgd(
```

### Comparing `optax-0.1.4/optax/_src/alias_test.py` & `optax-0.1.5/optax/_src/alias_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,47 +20,54 @@
 import chex
 import jax
 import jax.numpy as jnp
 
 from optax._src import alias
 from optax._src import numerics
 from optax._src import schedule
+from optax._src import state_utils
 from optax._src import update
 
 _OPTIMIZERS_UNDER_TEST = (
     dict(opt_name='sgd', opt_kwargs=dict(learning_rate=1e-3, momentum=0.9)),
     dict(opt_name='adafactor', opt_kwargs=dict(learning_rate=5e-3)),
     dict(opt_name='adagrad', opt_kwargs=dict(learning_rate=1.0)),
     dict(opt_name='adam', opt_kwargs=dict(learning_rate=1e-1)),
     dict(opt_name='adamw', opt_kwargs=dict(learning_rate=1e-1)),
     dict(opt_name='adamax', opt_kwargs=dict(learning_rate=1e-1)),
     dict(opt_name='adamaxw', opt_kwargs=dict(learning_rate=1e-1)),
     dict(opt_name='amsgrad', opt_kwargs=dict(learning_rate=1e-1)),
     dict(opt_name='lars', opt_kwargs=dict(learning_rate=1.0)),
     dict(opt_name='lamb', opt_kwargs=dict(learning_rate=1e-3)),
+    dict(
+        opt_name='lion', opt_kwargs=dict(learning_rate=1e-2, weight_decay=1e-4),
+    ),
     dict(opt_name='noisy_sgd', opt_kwargs=dict(learning_rate=1e-3, eta=1e-4)),
     dict(opt_name='novograd', opt_kwargs=dict(learning_rate=1e-3)),
     dict(
         opt_name='optimistic_gradient_descent',
-        opt_kwargs=dict(learning_rate=2e-3, alpha=0.7, beta=0.1)),
+        opt_kwargs=dict(learning_rate=2e-3, alpha=0.7, beta=0.1),
+    ),
     dict(opt_name='rmsprop', opt_kwargs=dict(learning_rate=5e-3)),
     dict(opt_name='rmsprop', opt_kwargs=dict(learning_rate=5e-3, momentum=0.9)),
     dict(opt_name='fromage', opt_kwargs=dict(learning_rate=5e-3)),
     dict(opt_name='adabelief', opt_kwargs=dict(learning_rate=1e-2)),
     dict(opt_name='radam', opt_kwargs=dict(learning_rate=5e-3)),
     dict(opt_name='sm3', opt_kwargs=dict(learning_rate=1.0)),
     dict(opt_name='yogi', opt_kwargs=dict(learning_rate=1e-1)),
     dict(
         opt_name='dpsgd',
         opt_kwargs=dict(
             learning_rate=1e-3,
-            l2_norm_clip=10.,
+            l2_norm_clip=10.0,
             noise_multiplier=1e-3,
             seed=0,
-            momentum=0.2)),
+            momentum=0.2,
+        ),
+    ),
 )
 
 
 def _setup_parabola(dtype):
   """Quadratic function as an optimization target."""
   initial_params = jnp.array([-1.0, 10.0, 1.0], dtype=dtype)
   final_params = jnp.array([1.0, -1.0, 1.0], dtype=dtype)
@@ -98,19 +105,24 @@
 
   @parameterized.product(
       _OPTIMIZERS_UNDER_TEST,
       target=(_setup_parabola, _setup_rosenbrock),
       dtype=(jnp.float32, jnp.complex64),
   )
   def test_optimization(self, opt_name, opt_kwargs, target, dtype):
-    if (opt_name
-        in ('fromage', 'noisy_sgd', 'sm3', 'optimistic_gradient_descent') and
-        jnp.iscomplexobj(dtype)):
+    if opt_name in (
+        'fromage',
+        'noisy_sgd',
+        'sm3',
+        'optimistic_gradient_descent',
+        'lion',
+    ) and jnp.iscomplexobj(dtype):
       raise absltest.SkipTest(
-          f'{opt_name} does not support complex parameters.')
+          f'{opt_name} does not support complex parameters.'
+      )
 
     opt = getattr(alias, opt_name)(**opt_kwargs)
     initial_params, final_params, get_updates = target(dtype)
 
     @jax.jit
     def step(params, state):
       updates = get_updates(params)
@@ -121,14 +133,17 @@
       updates = jax.tree_util.tree_map(lambda x: x.conj(), updates)
       updates, state = opt.update(updates, state, params)
       params = update.apply_updates(params, updates)
       return params, state
 
     params = initial_params
     state = opt.init(params)
+    # A no-op change, to verify that tree map works.
+    state = state_utils.tree_map_params(opt, lambda v: v, state)
+
     for _ in range(10000):
       params, state = step(params, state)
 
     chex.assert_trees_all_close(params, final_params, rtol=3e-2, atol=3e-2)
 
   @chex.all_variants
   @parameterized.product(_OPTIMIZERS_UNDER_TEST)
@@ -169,18 +184,18 @@
       ('complex64', 'complex64'),
       ('None', None),
   ])
   def test_explicit_dtype(self, dtype):
     expected_dtype = jax.dtypes.canonicalize_dtype(dtype)  # None -> float32
     tx = alias.sgd(0.1, momentum=0.9, accumulator_dtype=dtype)
     trace_state, _ = tx.init(jnp.array([0.0, 0.0]))
-    self.assertEqual(expected_dtype, trace_state.trace.dtype)
+    self.assertEqual(expected_dtype, getattr(trace_state, 'trace').dtype)
     tx = alias.adam(0.1, mu_dtype=dtype)
     adam_state, _ = tx.init(jnp.array([0.0, 0.0]))
-    self.assertEqual(expected_dtype, adam_state.mu.dtype)
+    self.assertEqual(expected_dtype, getattr(adam_state, 'mu').dtype)
     tx = alias.adamw(0.1, mu_dtype=dtype)
     adam_state, _, _ = tx.init(jnp.array([0.0, 0.0]))
-    self.assertEqual(expected_dtype, adam_state.mu.dtype)
+    self.assertEqual(expected_dtype, getattr(adam_state, 'mu').dtype)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `optax-0.1.4/optax/_src/base.py` & `optax-0.1.5/optax/_src/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,20 +10,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Base interfaces and datatypes."""
 
-from typing import Any, Callable, NamedTuple, Optional, Sequence, Tuple
+from typing import Any, Callable, NamedTuple, Optional, Protocol, Sequence, Tuple
 
 import chex
 import jax
 import jax.numpy as jnp
-import typing_extensions
 
 NO_PARAMS_MSG = (
     'You are using a transformation that requires the current value of '
     'parameters, but you are not passing `params` when calling `update`.')
 
 PyTree = Any
 Shape = Sequence[int]
@@ -31,15 +30,15 @@
 OptState = chex.ArrayTree  # States are arbitrary nests of `jnp.ndarrays`.
 Params = chex.ArrayTree  # Parameters are arbitrary nests of `jnp.ndarrays`.
 Updates = Params  # Gradient updates are of the same type as parameters.
 
 Schedule = Callable[[chex.Numeric], chex.Numeric]
 
 
-class TransformInitFn(typing_extensions.Protocol):
+class TransformInitFn(Protocol):
   """A callable type for the `init` step of a `GradientTransformation`.
 
   The `init` step takes a tree of `params` and uses these to construct an
   arbitrary structured initial `state` for the gradient transformation. This
   may hold statistics of the past updates or any other non static information.
   """
 
@@ -50,22 +49,25 @@
       params: The initial value of the parameters.
 
     Returns:
       The initial state of the gradient transformation.
     """
 
 
-class TransformUpdateFn(typing_extensions.Protocol):
+class TransformUpdateFn(Protocol):
   """A callable type for the `update` step of a `GradientTransformation`.
 
   The `update` step takes a tree of candidate parameter `updates` (e.g. their
   gradient with respect to some loss), an arbitrary structured `state`, and the
   current `params` of the model being optimised. The `params` argument is
   optional, it must however be provided when using transformations that require
   access to the current values of the parameters.
+
+  For the case where additional arguments are required, an alternative interface
+  may be used, see ``TransformUpdateExtraArgsFn`` for details.
   """
 
   def __call__(
       self,
       updates: Updates,
       state: OptState,
       params: Optional[Params] = None
@@ -78,22 +80,65 @@
       params: (Optionally) the current value of the parameters.
 
     Returns:
       The transformed updates, and the updated state.
     """
 
 
+class TransformUpdateExtraArgsFn(Protocol):
+  """An update function accepting additional keyword arguments."""
+
+  def __call__(
+      self,
+      updates: Updates,
+      state: OptState,
+      params: Optional[Params] = None,
+      **extra_args: Any,
+  ) -> Tuple[Updates, OptState]:
+    """Update function with optional extra arguments.
+
+    For example, an update function that requires an additional loss parameter
+    (which might be useful for implementing learning rate schedules that depend
+    on the current loss value) could be expressed as follows.
+
+    >>> def update(updates, state, params=None, *, loss, **extra_args):
+    >>>   del extra_args
+    >>>   # use loss value
+
+    Note that the loss value is keyword only, (it follows a `*` in the
+    signature of the function). This means users will get explicit errors if
+    they try to use this gradient transformation without providing the required
+    argument.
+
+    Args:
+      updates: The gradient updates passed to this transformation.
+      state: The state associated with this transformation
+      params: Optional params.
+      **extra_args: Additional keyword arguments passed to this transform. All
+        implementors of this interface should accept arbitrary keyword
+        arguments, ignoring those that are not needed for the current
+        transformation. Transformations that require specific extra args should
+        specify these using keyword-only arguments.
+    Returns:
+      Transformed updates, and an updated value for the state.
+    """
+
+
 class GradientTransformation(NamedTuple):
   """A pair of pure functions implementing a gradient transformation.
 
   Optax optimizers are all implemented as _gradient transformations_.
   A gradient transformation is defined to be a pair of pure functions, which
   are combined together in a `NamedTuple` so that they can be referred to by
   name.
 
+  Note that an extended API is provided for users wishing to build optimizers
+  that take additional arguments during the update step. For more details,
+  see ``GradientTransoformationExtraArgs``.
+
   Since gradient transformations do not contain any internal state, all stateful
   optimizer properties (such as the current step count when using optimizer
   scheduels, or  momemtum values) are passed through optax gradient
   transformations by using the optimizer _state_ pytree. Each time a gradient
   transformation is applied, a new state is computed and returned, ready to be
   passed to the next call to the gradient transformation.
 
@@ -113,14 +158,34 @@
       function), and optionally the current params. The update function then
       returns the computed gradient updates, and a new optimizer state.
   """
   init: TransformInitFn
   update: TransformUpdateFn
 
 
+class GradientTransformationExtraArgs(GradientTransformation):
+  """A specialization of GradientTransformation that supports extra args.
+
+  Extends the existing GradientTransformation interface by adding support for
+  passing extra arguments to the update function.
+
+  Note that if no extra args are provided, then the API of this function is
+  identical to the case of ``TransformUpdateFn``. This means that we can safely
+  wrap any gradient transformation (that does not support extra args) as one
+  that does. The new gradient transformation will accept (and ignore) any
+  extra arguments that a user might pass to it. This is the behavior implemented
+  by ``optax.with_extra_args_support()``.
+
+  Attributes:
+    update: Overrides the type signature of the update in the base type to
+      accept extra arguments.
+  """
+  update: TransformUpdateExtraArgsFn
+
+
 class EmptyState(NamedTuple):
   """An empty state for the simplest stateless transformations."""
 
 
 def identity() -> GradientTransformation:
   """Stateless identity transformation that leaves input gradients untouched.
 
@@ -227,7 +292,22 @@
     if params is not None:
       return jax.tree_util.tree_map(f, updates, params), EmptyState()
     else:
       f_ = lambda u: f(u, None)
       return jax.tree_util.tree_map(f_, updates), EmptyState()
 
   return GradientTransformation(init_fn, update_fn)
+
+
+def with_extra_args_support(
+    tx: GradientTransformation,
+) -> GradientTransformationExtraArgs:
+  """Wraps a gradient transformation, so that it ignores extra args."""
+
+  if isinstance(tx, GradientTransformationExtraArgs):
+    return tx
+
+  def update(updates, state, params=None, **extra_args):
+    del extra_args
+    return tx.update(updates, state, params)
+
+  return GradientTransformationExtraArgs(tx.init, update)
```

### Comparing `optax-0.1.4/optax/_src/base_test.py` & `optax-0.1.5/optax/_src/base_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -58,14 +58,74 @@
   @chex.all_variants(with_pmap=False)
   def test_set_to_zero_is_stateless(self):
     """Tests that the zero transform returns an empty state."""
     self.assertEqual(
         self.variant(base.set_to_zero().init)(params=None), base.EmptyState())
 
 
+class ExtraArgsTest(chex.TestCase):
+
+  def test_isinstance(self):
+    """Locks in behaviour for comparing transformations."""
+
+    def init_fn(params):
+      del params
+      return {}
+
+    def update_fn(updates, state, params=None):
+      del params
+      return updates, state
+
+    t1 = base.GradientTransformation(init_fn, update_fn)
+    self.assertIsInstance(t1, base.GradientTransformation)
+    self.assertNotIsInstance(t1, base.GradientTransformationExtraArgs)
+
+    t2 = base.with_extra_args_support(t1)
+    self.assertIsInstance(t2, base.GradientTransformation)
+    self.assertIsInstance(t2, base.GradientTransformationExtraArgs)
+
+    with self.subTest('args_correctly_ignored'):
+      state = t2.init({})
+      t2.update({}, state, ignored_arg='hi')
+
+    t3 = base.with_extra_args_support(t2)
+    self.assertIsInstance(t3, base.GradientTransformation)
+    self.assertIsInstance(t3, base.GradientTransformationExtraArgs)
+
+  def test_extra_args_with_callback(self):
+    """An example of using extra args to log the learning rate."""
+
+    def init_fn(params):
+      del params
+      return {}
+
+    def update_fn(updates, state, *, metrics_logger=None, **extra_args):
+      del extra_args
+
+      if metrics_logger:
+        metrics_logger('learning_rate', 0.3)
+      return updates, state
+
+    t = base.GradientTransformationExtraArgs(init_fn, update_fn)
+
+    @jax.jit
+    def f(params):
+      state = t.init(params)
+
+      metrics = {}
+      def metrics_logger(name, value):
+        metrics[name] = value
+
+      t.update(params, state, metrics_logger=metrics_logger)
+      return metrics
+
+    metrics = f({'a': 1})
+    self.assertEqual(metrics['learning_rate'], 0.3)
+
+
 class StatelessTest(chex.TestCase):
   """Tests for the stateless transformation."""
 
   @chex.all_variants
   def test_stateless(self):
     params = {'a': jnp.zeros((1, 2)), 'b': jnp.ones((1,))}
     updates = {'a': jnp.ones((1, 2)), 'b': jnp.full((1,), 2.0)}
@@ -84,26 +144,26 @@
   def test_stateless_no_params(self):
     updates = {'linear': jnp.full((5, 3), 3.0)}
 
     @base.stateless
     def opt(g, _):
       return jax.tree_util.tree_map(lambda g_: g_ * 2, g)
 
-    state = opt.init(None)
+    state = opt.init(None)  # pytype: disable=wrong-arg-types  # numpy-scalars
     update_fn = self.variant(opt.update)
     new_updates, _ = update_fn(updates, state)
     expected_updates = {'linear': jnp.full((5, 3), 6.0)}
     chex.assert_trees_all_close(new_updates, expected_updates)
 
   def test_init_returns_emptystate(self):
     def weight_decay(g, p):
       return jax.tree_util.tree_map(lambda g_, p_: g_ + 0.1 * p_, g, p)
 
     opt = base.stateless(weight_decay)
-    state = opt.init(None)
+    state = opt.init(None)  # pytype: disable=wrong-arg-types  # numpy-scalars
     self.assertIsInstance(state, base.EmptyState)
 
 
 class StatelessWithTreeMapTest(chex.TestCase):
   """Tests for the stateless_with_tree_map transformation."""
 
   @chex.all_variants
@@ -119,21 +179,21 @@
     chex.assert_trees_all_close(new_updates, expected_updates)
 
   @chex.all_variants
   def test_stateless_with_tree_map_no_params(self):
     updates = {'linear': jnp.full((5, 3), 3.0)}
 
     opt = base.stateless_with_tree_map(lambda g, _: g * 2.0)
-    state = opt.init(None)
+    state = opt.init(None)  # pytype: disable=wrong-arg-types  # numpy-scalars
     update_fn = self.variant(opt.update)
     new_updates, _ = update_fn(updates, state)
     expected_updates = {'linear': jnp.full((5, 3), 6.0)}
     chex.assert_trees_all_close(new_updates, expected_updates)
 
   def test_init_returns_emptystate(self):
     opt = base.stateless_with_tree_map(lambda g, p: g + 0.1 * p)
-    state = opt.init(None)
+    state = opt.init(None)  # pytype: disable=wrong-arg-types  # numpy-scalars
     self.assertIsInstance(state, base.EmptyState)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `optax-0.1.4/optax/_src/clipping.py` & `optax-0.1.5/optax/_src/clipping.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 # ==============================================================================
 """Gradient clipping transformations.
 
 Note that complex numbers are also supported, see
 https://gist.github.com/wdphy16/118aef6fb5f82c49790d7678cf87da29
 """
-from typing import Tuple
+from typing import List, Tuple
 
 import chex
 import jax
 import jax.numpy as jnp
 
 from optax._src import base
 from optax._src import linear_algebra
@@ -121,16 +121,17 @@
 
     updates = jax.tree_util.tree_map(clip_fn, updates)
     return updates, state
 
   return base.GradientTransformation(init_fn, update_fn)
 
 
-def per_example_global_norm_clip(grads: chex.Array,
-                                 l2_norm_clip: float) -> Tuple[chex.Array, int]:
+def per_example_global_norm_clip(
+    grads: List[chex.Array], l2_norm_clip: float
+) -> Tuple[List[chex.Array], jax.Array]:
   """Applies gradient clipping per-example using their global norm.
 
   References:
     [Abadi et al, 2016](https://arxiv.org/abs/1607.00133)
 
   Args:
     grads: flattened update; the function expects these to have a batch
```

### Comparing `optax-0.1.4/optax/_src/clipping_test.py` & `optax-0.1.5/optax/_src/clipping_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,45 +35,45 @@
     self.per_step_updates = (jnp.array([500., 5.]), jnp.array([300., 3.]))
 
   def test_clip(self):
     updates = self.per_step_updates
     # For a sufficiently high delta the update should not be changed.
     clipper = clipping.clip(1e6)
     clipped_updates, _ = clipper.update(updates, None)
-    chex.assert_tree_all_close(clipped_updates, clipped_updates)
+    chex.assert_trees_all_close(clipped_updates, clipped_updates)
     # Clipping at delta=1 should make all updates exactly 1.
     clipper = clipping.clip(1.)
     clipped_updates, _ = clipper.update(updates, None)
-    chex.assert_tree_all_close(
+    chex.assert_trees_all_close(
         clipped_updates, jax.tree_util.tree_map(jnp.ones_like, updates))
 
   def test_clip_by_block_rms(self):
     rmf_fn = lambda t: jnp.sqrt(jnp.mean(t**2))
     updates = self.per_step_updates
     for i in range(1, STEPS + 1):
       clipper = clipping.clip_by_block_rms(1. / i)
       # Check that the clipper actually works and block rms is <= threshold
       updates, _ = clipper.update(updates, None)
       self.assertAlmostEqual(rmf_fn(updates[0]), 1. / i)
       self.assertAlmostEqual(rmf_fn(updates[1]), 1. / i)
       # Check that continuously clipping won't cause numerical issues.
       updates_step, _ = clipper.update(self.per_step_updates, None)
-      chex.assert_tree_all_close(updates, updates_step)
+      chex.assert_trees_all_close(updates, updates_step)
 
   def test_clip_by_global_norm(self):
     updates = self.per_step_updates
     for i in range(1, STEPS + 1):
       clipper = clipping.clip_by_global_norm(1. / i)
       # Check that the clipper actually works and global norm is <= max_norm
       updates, _ = clipper.update(updates, None)
       self.assertAlmostEqual(
           linear_algebra.global_norm(updates), 1. / i, places=6)
       # Check that continuously clipping won't cause numerical issues.
       updates_step, _ = clipper.update(self.per_step_updates, None)
-      chex.assert_tree_all_close(updates, updates_step)
+      chex.assert_trees_all_close(updates, updates_step)
 
   def test_adaptive_grad_clip(self):
     updates = self.per_step_updates
     params = self.init_params
     for i in range(1, STEPS + 1):
       clip_r = 1. / i
       clipper = clipping.adaptive_grad_clip(clip_r)
@@ -85,12 +85,12 @@
       cmp = jax.tree_util.tree_map(
           lambda u, p, c=clip_r: u - c * p < 1e-6, u_norm, p_norm)
       for leaf in jax.tree_util.tree_leaves(cmp):
         self.assertTrue(leaf.all())
 
       # Check that continuously clipping won't cause numerical issues.
       updates_step, _ = clipper.update(self.per_step_updates, None, params)
-      chex.assert_tree_all_close(updates, updates_step)
+      chex.assert_trees_all_close(updates, updates_step)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `optax-0.1.4/optax/_src/combine.py` & `optax-0.1.5/optax/_src/combine.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,51 +19,61 @@
 import jax
 
 from optax._src import base
 from optax._src import wrappers
 
 
 def chain(
-    *args: base.GradientTransformation
-) -> base.GradientTransformation:
+    *args: base.GradientTransformation,
+) -> base.GradientTransformationExtraArgs:
   """Applies a list of chainable update transformations.
 
   Given a sequence of chainable transforms, `chain` returns an `init_fn`
   that constructs a `state` by concatenating the states of the individual
   transforms, and returns an `update_fn` which chains the update transformations
   feeding the appropriate state to each.
 
   Args:
     *args: a sequence of chainable (init_fn, update_fn) tuples.
 
   Returns:
-    A single (init_fn, update_fn) tuple.
+    A ``GradientTransformationExtraArgs``, created by chaining the input
+    transformations. Note that independent of the argument types, the resulting
+    transformation always supports extra args. Any extra arguments passed to the
+    returned transformation will be passed only to those transformations in the
+    chain that support extra args.
   """
 
-  init_fns, update_fns = zip(*args)
+  transforms = [base.with_extra_args_support(t) for t in args]
+  init_fns, update_fns = zip(*transforms)
 
   def init_fn(params):
     return tuple(fn(params) for fn in init_fns)
 
-  def update_fn(updates, state, params=None):
+  def update_fn(updates, state, params=None, **extra_args):
     if len(update_fns) != len(state):
       raise ValueError('The number of updates and states has to be the same in '
                        'chain! Make sure you have called init first!')
 
     new_state = []
     for s, fn in zip(state, update_fns):
-      updates, new_s = fn(updates, s, params)
+      updates, new_s = fn(updates, s, params, **extra_args)
       new_state.append(new_s)
     return updates, tuple(new_state)
 
-  return base.GradientTransformation(init_fn, update_fn)
+  # We opt to always return the GradientTransformationExtraArgs type here,
+  # instead of selecting the return type based on the arguments, since it works
+  # much better with the currently available type checkers. It also means that
+  # users will not get unexpected signature errors if they remove all of the
+  # transformations in a chain accepting extra args.
+  return base.GradientTransformationExtraArgs(init_fn, update_fn)
 
 
 class MultiTransformState(NamedTuple):
-  inner_states: Mapping[Hashable, NamedTuple]
+  inner_states: Mapping[Hashable, base.OptState]
 
 
 def multi_transform(
     transforms: Mapping[Hashable, base.GradientTransformation],
     param_labels: Union[base.PyTree, Callable[[base.PyTree], base.PyTree]]
 ) -> base.GradientTransformation:
   """Partitions params and applies a different transformation to each subset.
```

### Comparing `optax-0.1.4/optax/_src/combine_test.py` & `optax-0.1.5/optax/_src/combine_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from absl.testing import parameterized
 
 import chex
 import jax
 import jax.numpy as jnp
 
 from optax._src import alias
+from optax._src import base
 from optax._src import combine
 from optax._src import transform
 from optax._src import update
 
 
 STEPS = 50
 LR = 1e-2
@@ -69,24 +70,88 @@
       for t, s in zip(transformations, states):
         updates, state = t.update(updates, s)
         new_states.append(state)
       manual_params = update.apply_updates(manual_params, updates)
       states = new_states
 
     # Check equivalence.
-    chex.assert_tree_all_close(manual_params, chain_params, rtol=1e-4)
+    chex.assert_trees_all_close(manual_params, chain_params, rtol=1e-4)
 
 
 def _map_keys_fn(fn):
   def map_fn(nested_dict):
     return {k: (map_fn(v) if isinstance(v, dict) else fn(k, v))
             for k, v in nested_dict.items()}
   return map_fn
 
 
+class ExtraArgsTest(chex.TestCase):
+
+  def test_extra_args(self):
+    def init_fn(params):
+      del params
+      return tuple()
+
+    # Arguments required by a transformation should be keyword-only.
+    # For example, the loss argument in this transformation.
+    def update_fn(updates, state, params=None, *, loss, **extra_args):
+      # Extra args should always be accepted.
+      del extra_args, params
+      assert loss == 1
+      return updates, state
+
+    t = base.GradientTransformationExtraArgs(init_fn, update_fn)
+    result = combine.chain(alias.adam(1e-3), t)
+    self.assertIsInstance(result, base.GradientTransformationExtraArgs)
+
+    params = {'a': 1, 'b': 2}
+    state = result.init(params)
+    result.update(params, state, loss=1, ignored_kwarg='hi')
+
+  def test_extra_args_chaining(self):
+    def init_fn(params):
+      del params
+      return {}
+    def update_fn(updates, state, params=None):
+      del params
+      return updates, state
+
+    # Possible gotcha: Chaining regular gradient transformations results in
+    # a transformation that supports extra args.
+    t1 = base.GradientTransformation(init_fn, update_fn)
+    t2 = combine.chain(t1, t1)
+    self.assertIsInstance(t2, base.GradientTransformation)
+    self.assertIsInstance(t2, base.GradientTransformationExtraArgs)
+
+    t3 = base.with_extra_args_support(t2)
+    self.assertIsInstance(t3, base.GradientTransformationExtraArgs)
+
+  def test_extra_args_positional_params(self):
+    def init_fn(params):
+      del params
+      return tuple()
+
+    def update_fn(updates, state, params=None):
+      assert params is not None
+      return updates, state
+
+    def update_fn_kwargs(updates, state, params=None, **extra_args):
+      del extra_args
+      assert params is not None
+      return updates, state
+
+    t1 = base.GradientTransformation(init_fn, update_fn)
+    t2 = base.GradientTransformationExtraArgs(init_fn, update_fn_kwargs)
+    opt = combine.chain(t1, t2)
+    params = {'a': 1, 'b': 2}
+    state = opt.init(params)
+    opt.update(params, state, params, ignored_kwarg='hi')
+    opt.update(params, state, params=params, ignored_kwarg='hi')
+
+
 class MultiTransformTest(chex.TestCase):
   """Tests for the multi_transform wrapper."""
 
   @chex.all_variants
   @parameterized.parameters(True, False)
   def test_multi_transform(self, use_fn):
     params = {'a1': 1., 'b1': 2., 'z1': {'a2': 3., 'z2': {'c1': 4.}}}
@@ -103,20 +168,20 @@
     state = self.variant(tx.init)(params)
 
     correct_update_fn = _map_keys_fn(
         lambda k, v: {'a': -v, 'b': v, 'c': 2.0*v}[k[0]])
 
     updates, state = update_fn(input_updates, state, params)
     correct_updates = correct_update_fn(input_updates)
-    chex.assert_tree_all_close(updates, correct_updates)
+    chex.assert_trees_all_close(updates, correct_updates)
 
     # Check repeated application, this time with no params.
     correct_updates = correct_update_fn(correct_updates)
     updates, state = update_fn(updates, state)
-    chex.assert_tree_all_close(updates, correct_updates)
+    chex.assert_trees_all_close(updates, correct_updates)
 
   @parameterized.parameters(list, tuple, dict)
   def test_empty(self, container):
     init_fn, update_fn = combine.multi_transform(
         {0: alias.sgd(1.)}, lambda _: 0)
     updates, _ = update_fn(container(), init_fn(container()))
     self.assertEqual(updates, container())
```

### Comparing `optax-0.1.4/optax/_src/constrain.py` & `optax-0.1.5/optax/_src/constrain.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.4/optax/_src/constrain_test.py` & `optax-0.1.5/optax/_src/constrain_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,73 +43,74 @@
     opt = combine.chain(
         transform.trace(decay=0, nesterov=False), transform.scale(-LR))
     opt_state = opt.init(params)
 
     updates, _ = opt.update(grads, opt_state, params)
     new_params = update.apply_updates(params, updates)
 
-    chex.assert_tree_all_close(new_params, (jnp.array([-6., 4., -1.]),
-                                            jnp.array([-4., 6., 1.]),
-                                            jnp.array([-5., 5., 0.])))
+    chex.assert_trees_all_close(new_params, (jnp.array([-6., 4., -1.]),
+                                             jnp.array([-4., 6., 1.]),
+                                             jnp.array([-5., 5., 0.])))
 
     # sgd with keeping parameters non-negative
     opt = combine.chain(
         transform.trace(decay=0, nesterov=False), transform.scale(-LR),
         constrain.keep_params_nonnegative())
     opt_state = opt.init(params)
 
     updates, _ = opt.update(grads, opt_state, params)
     new_params = update.apply_updates(params, updates)
 
-    chex.assert_tree_all_close(new_params, (jnp.array([0., 4., 0.]),
-                                            jnp.array([0., 6., 1.]),
-                                            jnp.array([0., 5., 0.])))
+    chex.assert_trees_all_close(new_params, (jnp.array([0., 4., 0.]),
+                                             jnp.array([0., 6., 1.]),
+                                             jnp.array([0., 5., 0.])))
 
   @chex.all_variants
   def test_zero_nans(self):
     params = (jnp.zeros([3]), jnp.zeros([3]), jnp.zeros([3]))
 
     opt = constrain.zero_nans()
     opt_state = self.variant(opt.init)(params)
     update_fn = self.variant(opt.update)
 
-    chex.assert_tree_all_close(opt_state,
-                               constrain.ZeroNansState((jnp.array(False),) * 3))
+    chex.assert_trees_all_close(
+        opt_state,
+        constrain.ZeroNansState((jnp.array(False),) * 3))
 
     # Check an upate with nans
     grads_with_nans = (jnp.ones([3]),
                        jnp.array([1., float('nan'), float('nan')]),
                        jnp.array([float('nan'), 1., 1.]))
     updates, opt_state = update_fn(grads_with_nans, opt_state)
-    chex.assert_tree_all_close(
+    chex.assert_trees_all_close(
         opt_state,
         constrain.ZeroNansState(
             (jnp.array(False), jnp.array(True), jnp.array(True))))
-    chex.assert_tree_all_close(
+    chex.assert_trees_all_close(
         updates,
         (jnp.ones([3]), jnp.array([1., 0., 0.]), jnp.array([0., 1., 1.])))
 
     # Check an upate with nans and infs
     grads_with_nans_infs = (jnp.ones([3]),
                             jnp.array([1., float('nan'),
                                        float('nan')]),
                             jnp.array([float('inf'), 1., 1.]))
     updates, opt_state = update_fn(grads_with_nans_infs, opt_state)
-    chex.assert_tree_all_close(
+    chex.assert_trees_all_close(
         opt_state,
         constrain.ZeroNansState(
             (jnp.array(False), jnp.array(True), jnp.array(False))))
-    chex.assert_tree_all_close(updates, (jnp.ones([3]), jnp.array(
+    chex.assert_trees_all_close(updates, (jnp.ones([3]), jnp.array(
         [1., 0., 0.]), jnp.array([float('inf'), 1., 1.])))
 
     # Check an upate with only good values
     grads = (jnp.ones([3]), jnp.ones([3]), jnp.ones([3]))
     updates, opt_state = update_fn(grads, opt_state)
-    chex.assert_tree_all_close(
+    chex.assert_trees_all_close(
         opt_state,
         constrain.ZeroNansState(
             (jnp.array(False), jnp.array(False), jnp.array(False))))
-    chex.assert_tree_all_close(updates, grads)
+    chex.assert_trees_all_close(updates, grads)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `optax-0.1.4/optax/_src/control_variates.py` & `optax-0.1.5/optax/_src/control_variates.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 import jax
 import jax.numpy as jnp
 
 from optax._src import base
 
 
 CvState = Any
-ComputeCv = Callable[[base.Params, chex.Array, CvState], float]
+ComputeCv = Callable[[base.Params, chex.Array, CvState], chex.Array]
 CvExpectedValue = Callable[[base.Params, CvState], CvState]
 UpdateCvState = Callable[[base.Params, chex.Array, CvState], CvState]
 ControlVariate = Tuple[ComputeCv, CvExpectedValue, UpdateCvState]
 
 
 def control_delta_method(
     function: Callable[[chex.Array], float]) -> ControlVariate:
@@ -267,15 +267,15 @@
           The mean of this vector is the gradient wrt to parameters that can be
           used for learning. The entire jacobian vector can be used to assess
           estimator variance.
         * The updated CV state.
   """
   control_variate = control_variate_from_function(function)
   stochastic_cv, expected_value_cv, update_state_cv = control_variate
-  data_dim = params[0].shape[0]
+  data_dim = jax.tree_util.tree_leaves(params)[0].shape[0]
   if estimate_cv_coeffs:
     cv_coeffs = estimate_control_variate_coefficients(
         function, control_variate_from_function, grad_estimator, params,
         dist_builder, rng, estimate_cv_coeffs_num_samples,
         control_variate_state)
   else:
     cv_coeffs = [1.0] * len(params)
@@ -311,15 +311,15 @@
   cv_param_grads = jax.grad(param_fn)(params)
   # The gradients of the closed form expectation of the control variate
   # with respect to the parameters: # \nabla_{\theta} E_{p(x; \theta)}].
   expected_value_grads = jax.grad(
       lambda x: expected_value_cv(x, control_variate_state))(params)
 
   jacobians = []
-  for param_index, param in enumerate(params):
+  for param_index, param in enumerate(jax.tree_util.tree_leaves(params)):
     chex.assert_shape(function_jacobians[param_index], (num_samples, data_dim))
     chex.assert_shape(cv_jacobians[param_index], (num_samples, data_dim))
     chex.assert_shape(cv_param_grads[param_index], (data_dim,))
     chex.assert_shape(expected_value_grads[param_index], (data_dim,))
 
     cv_coeff = cv_coeffs[param_index]
     # \int \nabla_{\theta} {p(x; \theta)} (f(x) - h(x; \theta)) dx
```

### Comparing `optax-0.1.4/optax/_src/control_variates_test.py` & `optax-0.1.5/optax/_src/control_variates_test.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.4/optax/_src/equivalence_test.py` & `optax-0.1.5/optax/_src/equivalence_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
       return optax_optimizer.update(updates, state)
 
     for _ in range(STEPS):
       updates, state = step(self.per_step_updates, state)
       optax_params = update.apply_updates(optax_params, updates)
 
     # Check equivalence.
-    chex.assert_tree_all_close(jax_params, optax_params, rtol=rtol)
+    chex.assert_trees_all_close(jax_params, optax_params, rtol=rtol)
 
 
 class FlaxOptimizersEquivalenceTest(chex.TestCase):
 
   def setUp(self):
     super().setUp()
     self.init_params = (
@@ -165,12 +165,12 @@
     state = optax_optimizer.init(optax_params)
     for _ in range(STEPS):
       updates, state = optax_optimizer.update(
           self.per_step_updates, state, optax_params)
       optax_params = update.apply_updates(optax_params, updates)
 
     # Check equivalence.
-    chex.assert_tree_all_close(flax_params, optax_params, rtol=2e-4)
+    chex.assert_trees_all_close(flax_params, optax_params, rtol=2e-4)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `optax-0.1.4/optax/_src/experimental/complex_valued.py` & `optax-0.1.5/optax/_src/experimental/complex_valued.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.4/optax/_src/experimental/complex_valued_test.py` & `optax-0.1.5/optax/_src/experimental/complex_valued_test.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.4/optax/_src/experimental/extra_args.py` & `optax-0.1.5/optax/_src/experimental/extra_args.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,33 +20,32 @@
 
 We introduce `GradientTransformationWithExtraArgs` as an experimental feature.
 You can use the new `named_chain` to combine both old-style and new-style
 transformations. We will then monitor users to understand how they use it and
 gather feedback from optax users before merging this into the stable API.
 """
 
-from typing import Any, Mapping, Optional, Tuple, Union, NamedTuple
+from typing import Any, Mapping, Optional, Protocol, Tuple, Union, NamedTuple
 
 from optax._src import base
-import typing_extensions
 
 
-class InitFnWithExtraArgs(typing_extensions.Protocol):
+class InitFnWithExtraArgs(Protocol):
   """Like `TransformInitFn` but with optional `extra_args`."""
 
   def __call__(
       self,
       params: base.Params,
       *,
       extra_args: Optional[Mapping[str, Any]] = None,
   ) -> base.OptState:
     """The `init` function."""
 
 
-class UpdateFnWithExtraArgs(typing_extensions.Protocol):
+class UpdateFnWithExtraArgs(Protocol):
   """Like `TransformUpdateFn` but with optional `extra_args`."""
 
   def __call__(
       self,
       updates: base.Updates,
       state: base.OptState,
       params: Optional[base.Params] = None,
```

### Comparing `optax-0.1.4/optax/_src/experimental/extra_args_test.py` & `optax-0.1.5/optax/_src/experimental/extra_args_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,12 +54,12 @@
     extra_args = {
         'scale_by_policy_loss': {'loss': 0.01},
         'scale_by_value_loss': {'loss': 10.0}}
 
     opt_state = tx.init(params, extra_args=extra_args)
     updates, opt_state = tx.update(
         grads, opt_state, params, extra_args=extra_args)
-    chex.assert_tree_all_close(updates, {'a': jnp.ones((4,))})
+    chex.assert_trees_all_close(updates, {'a': jnp.ones((4,))})
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `optax-0.1.4/optax/_src/factorized.py` & `optax-0.1.5/optax/_src/factorized.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 from optax._src import base
 from optax._src import numerics
 from optax._src import utils
 
 # pylint:disable=no-value-for-parameter
 
 
-def _decay_rate_pow(i: int, exponent: float = 0.8) -> float:
+def _decay_rate_pow(i: int, exponent: float = 0.8) -> chex.Array:
   """Second-order moment decay schedule."""
-  t = jnp.array(i, jnp.float32) + 1.0
+  t = jnp.array(i + 1, jnp.float32)
   return 1.0 - t**(-exponent)
 
 
 def _factored_dims(
     shape: base.Shape,
     factored: bool,
     min_dim_size_to_factor: int
```

### Comparing `optax-0.1.4/optax/_src/factorized_test.py` & `optax-0.1.5/optax/_src/factorized_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Tests for `factorized.py`."""
 
+from absl.testing import absltest
 from absl.testing import parameterized
 
 import chex
 import jax.numpy as jnp
 
 from optax._src import factorized
 
@@ -39,7 +40,11 @@
 
     state = init_fn(params)
     chex.assert_tree_all_finite(state)
 
     updates, state = transform_fn(self.per_step_updates, state, params)
     chex.assert_tree_all_finite((params, updates, state))
     chex.assert_tree_all_equal_shapes(params, updates)
+
+
+if __name__ == '__main__':
+  absltest.main()
```

### Comparing `optax-0.1.4/optax/_src/float64_test.py` & `optax-0.1.5/optax/_src/float64_test.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.4/optax/_src/linear_algebra.py` & `optax-0.1.5/optax/_src/linear_algebra.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import jax.numpy as jnp
 import numpy as np
 
 from optax._src import base
 from optax._src import numerics
 
 
-def global_norm(updates: base.Updates) -> base.Updates:
+def global_norm(updates: base.PyTree) -> chex.Array:
   """Compute the global norm across a nested structure of tensors."""
   return jnp.sqrt(sum(
       jnp.sum(numerics.abs_sq(x)) for x in jax.tree_util.tree_leaves(updates)))
 
 
 def power_iteration(matrix: chex.Array,
                     num_iters: int = 100,
```

### Comparing `optax-0.1.4/optax/_src/linear_algebra_test.py` & `optax-0.1.5/optax/_src/linear_algebra_test.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.4/optax/_src/lookahead.py` & `optax-0.1.5/optax/_src/lookahead.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """A lookahead optimization wrapper."""
 
-from typing import NamedTuple, Tuple
+from typing import NamedTuple, Tuple, Union
 
 from absl import logging
 import jax
 import jax.numpy as jnp
 
 from optax._src import base
 
@@ -92,17 +92,16 @@
     passed to the update function should be calculated using the fast lookahead
     parameters only.
   """
   if sync_period < 1:
     raise ValueError('Synchronization period must be >= 1.')
 
   def init_fn(params: base.Params) -> LookaheadState:
-    try:
-      fast_params = params.fast
-    except AttributeError:
+    fast_params = getattr(params, 'fast', None)
+    if fast_params is None:
       # Allowing init_fn to be called with fast parameters reduces the
       # modifications necessary to adapt code to use lookahead in some cases.
       logging.warning(
           '`params` has no attribute `fast`. Continuing by assuming that '
           'only fast parameters were passed to lookahead init.')
       fast_params = params
 
@@ -112,15 +111,15 @@
 
   def update_fn(
       updates: base.Updates, state: LookaheadState,
       params: LookaheadParams) -> Tuple[LookaheadParams, LookaheadState]:
     updates, fast_state = fast_optimizer.update(updates, state.fast_state,
                                                 params.fast)
 
-    sync_next = (state.steps_since_sync == sync_period - 1)
+    sync_next = state.steps_since_sync == sync_period - 1
     updates = _lookahead_update(updates, sync_next, params, slow_step_size)
     if reset_state:
       # Jittable way of resetting the fast optimizer state if parameters will be
       # synchronized after this update step.
       initial_state = fast_optimizer.init(params.fast)
       fast_state = jax.tree_util.tree_map(
           lambda current, init: (1 - sync_next) * current + sync_next * init,
@@ -129,16 +128,16 @@
     steps_since_sync = (state.steps_since_sync + 1) % sync_period
     return updates, LookaheadState(fast_state, steps_since_sync)
 
   return base.GradientTransformation(init_fn, update_fn)
 
 
 def _lookahead_update(
-    updates: base.Updates, sync_next: bool, params: LookaheadParams,
-    slow_step_size: float) -> LookaheadParams:
+    updates: base.Updates, sync_next: Union[bool, jax.Array],
+    params: LookaheadParams, slow_step_size: float) -> LookaheadParams:
   """Returns the updates corresponding to one lookahead step.
 
   References:
     [Zhang et al, 2019](https://arxiv.org/pdf/1907.08610v1.pdf)
 
   Args:
     updates: Updates returned by the fast optimizer.
```

### Comparing `optax-0.1.4/optax/_src/lookahead_test.py` & `optax-0.1.5/optax/_src/lookahead_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import chex
 import jax
 import jax.numpy as jnp
 import numpy as np
 from optax._src import alias
 from optax._src import base
 from optax._src import lookahead
+from optax._src import state_utils
 from optax._src import update
 
 
 def _build_sgd():
   return alias.sgd(1.)
 
 
@@ -72,14 +73,18 @@
 
   def loop(self, optimizer, num_steps, params):
     """Performs a given number of optimizer steps."""
     init_fn, update_fn = optimizer
     # Use the chex variant to check various function versions (jit, pmap, etc).
     step = self.variant(update_fn)
     opt_state = self.variant(init_fn)(params)
+
+    # A no-op change, to verify that tree map works.
+    opt_state = state_utils.tree_map_params(init_fn, lambda v: v, opt_state)
+
     for _ in range(num_steps):
       updates, opt_state = step(self.grads, opt_state, params)
       params = update.apply_updates(params, updates)
 
     return params, opt_state
 
   @chex.all_variants
@@ -90,37 +95,41 @@
         _test_optimizer(-0.5), sync_period=sync_period, slow_step_size=1 / 3)
 
     final_params, _ = self.loop(optimizer, 2 * sync_period,
                                 self.synced_initial_params)
     # x steps must be: 3 -> 2 -> 1 -> 2 (sync) -> 1 -> 0 -> 1 (sync).
     # Similarly for y (with sign flipped).
     correct_final_params = {'x': 1, 'y': -1}
-    chex.assert_tree_all_close(final_params.slow, correct_final_params)
+    chex.assert_trees_all_close(final_params.slow, correct_final_params)
 
   @chex.all_variants
   @parameterized.parameters([False], [True])
   def test_lookahead_state_reset(self, reset_state):
     """Checks that lookahead resets the fast optimizer state correctly."""
     num_steps = sync_period = 3
     fast_optimizer = _test_optimizer(-0.5)
     optimizer = lookahead.lookahead(
         fast_optimizer,
         sync_period=sync_period,
         slow_step_size=0.5,
         reset_state=reset_state)
 
     _, opt_state = self.loop(optimizer, num_steps, self.synced_initial_params)
+
+    # A no-op change, to verify that this does not break anything
+    opt_state = state_utils.tree_map_params(optimizer, lambda v: v, opt_state)
+
     fast_state = opt_state.fast_state
     if reset_state:
       correct_state = fast_optimizer.init(self.initial_params)
     else:
       _, correct_state = self.loop(fast_optimizer, num_steps,
                                    self.initial_params)
 
-    chex.assert_tree_all_close(fast_state, correct_state)
+    chex.assert_trees_all_close(fast_state, correct_state)
 
   @chex.all_variants
   @parameterized.parameters(
       [1, 0.5, {'x': np.array(1.), 'y': np.array(-1.)}],
       [1, 0, {'x': np.array(3.), 'y': np.array(-3.)}],
       [1, 1, {'x': np.array(-1.), 'y': np.array(1.)}],
       [2, 1, {'x': np.array(-1.), 'y': np.array(1.)}])  # pyformat: disable
@@ -129,12 +138,12 @@
     """Checks special cases of the lookahed optimizer parameters."""
     # These edge cases are important to check since users might use them as
     # simple ways of disabling lookahead in experiments.
     optimizer = lookahead.lookahead(
         _test_optimizer(-1), sync_period, slow_step_size)
     final_params, _ = self.loop(
         optimizer, num_steps=2, params=self.synced_initial_params)
-    chex.assert_tree_all_close(final_params.slow, correct_result)
+    chex.assert_trees_all_close(final_params.slow, correct_result)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `optax-0.1.4/optax/_src/loss.py` & `optax-0.1.5/optax/_src/loss.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,22 +25,25 @@
 import chex
 import jax
 import jax.numpy as jnp
 
 from optax._src import utils
 
 
-def l2_loss(
+def squared_error(
     predictions: chex.Array,
     targets: Optional[chex.Array] = None,
 ) -> chex.Array:
-  """Calculates the L2 loss for a set of predictions.
+  """Calculates the squared error for a set of predictions.
 
-  Note: the 0.5 term is standard in "Pattern Recognition and Machine Learning"
-  by Bishop, but not "The Elements of Statistical Learning" by Tibshirani.
+  Mean Squared Error can be computed as squared_error(a, b).mean().
+
+  Note: l2_loss = 0.5 * squared_error, where the 0.5 term is standard in
+  "Pattern Recognition and Machine Learning" by Bishop, but not
+  "The Elements of Statistical Learning" by Tibshirani.
 
   References:
     [Chris Bishop, 2006](https://bit.ly/3eeP0ga)
 
   Args:
     predictions: a vector of arbitrary shape `[...]`.
     targets: a vector with shape broadcastable to that of `predictions`;
@@ -49,16 +52,39 @@
   Returns:
     elementwise squared differences, with same shape as `predictions`.
   """
   chex.assert_type([predictions], float)
   if targets is not None:
     # Avoid broadcasting logic for "-" operator.
     chex.assert_equal_shape((predictions, targets))
-  errors = (predictions - targets) if (targets is not None) else predictions
-  return 0.5 * (errors)**2
+  errors = predictions - targets if targets is not None else predictions
+  return errors ** 2
+
+
+def l2_loss(
+    predictions: chex.Array,
+    targets: Optional[chex.Array] = None,
+) -> chex.Array:
+  """Calculates the L2 loss for a set of predictions.
+
+  Note: the 0.5 term is standard in "Pattern Recognition and Machine Learning"
+  by Bishop, but not "The Elements of Statistical Learning" by Tibshirani.
+
+  References:
+    [Chris Bishop, 2006](https://bit.ly/3eeP0ga)
+
+  Args:
+    predictions: a vector of arbitrary shape `[...]`.
+    targets: a vector with shape broadcastable to that of `predictions`;
+      if not provided then it is assumed to be a vector of zeros.
+
+  Returns:
+    elementwise squared differences, with same shape as `predictions`.
+  """
+  return 0.5 * squared_error(predictions, targets)
 
 
 def huber_loss(
     predictions: chex.Array,
     targets: Optional[chex.Array] = None,
     delta: float = 1.) -> chex.Array:
   """Huber loss, similar to L2 loss close to zero, L1 loss away from zero.
@@ -115,33 +141,40 @@
   num_categories = labels.shape[-1]
   return (1.0 - alpha) * labels + alpha / num_categories
 
 
 def sigmoid_binary_cross_entropy(logits, labels):
   """Computes element-wise sigmoid cross entropy given logits and labels.
 
-  This can be used to measure the error in discrete classification tasks in
-  which each class is an independent binary prediction and different classes
-  are not mutually exclusive. This may be used for multilabel image
-  classification for instance a model may predict that an image contains both a
-  cat and a dog.
+  This function can be used for binary or multiclass classification (where each
+  class is an independent binary prediction and different classes are not
+  mutually exclusive e.g. predicting that an image contains both a cat
+  and a dog.)
+
+  Because this function is overloaded, please ensure your `logits` and `labels`
+  are compatible with each other. If you're passing in binary `labels` (values
+  in {0, 1}), ensure your `logits` correspond to class 1 only. If you're
+  passing in per-class target probabilities or one-hot `labels`, please ensure
+  your `logits` are also multiclass. Be particularly careful if you're relying
+  on implicit broadcasting to reshape `logits` or `labels`.
 
   References:
     [Goodfellow et al, 2016](http://www.deeplearningbook.org/contents/prob.html)
 
   Args:
     logits: Each element is the unnormalized log probability of a binary
-      prediction.
-    labels: The target probabilities, must have a shape broadcastable to that of
-      `logits`.
+      prediction. See note about compatibility with `labels` above.
+    labels: Binary labels whose values are {0,1} or multi-class target
+      probabilities. See note about compatibility with `logits` above.
 
   Returns:
     cross entropy for each binary prediction, same shape as `logits`.
   """
   chex.assert_type([logits], float)
+  labels = labels.astype(logits.dtype)
   log_p = jax.nn.log_sigmoid(logits)
   # log(1 - sigmoid(x)) = log_sigmoid(-x), the latter more numerically stable
   log_not_p = jax.nn.log_sigmoid(-logits)
   return -labels * log_p - (1. - labels) * log_not_p
 
 
 def softmax_cross_entropy(
@@ -158,15 +191,15 @@
   References:
     [Goodfellow et al, 2016](http://www.deeplearningbook.org/contents/prob.html)
 
   Args:
     logits: Unnormalized log probabilities, with shape `[..., num_classes]`.
     labels: Valid probability distributions (non-negative, sum to 1), e.g a
       one hot encoding specifying the correct class for each input;
-      must have a shape broadcastable to `[..., num_classes]``
+      must have a shape broadcastable to `[..., num_classes]`.
 
   Returns:
     cross entropy between each prediction and the corresponding target
     distributions, with shape `[...]`.
   """
   chex.assert_type([logits], float)
   return -jnp.sum(labels * jax.nn.log_softmax(logits, axis=-1), axis=-1)
@@ -457,36 +490,66 @@
   """
   per_seq_loss, _, _ = ctc_loss_with_forward_probs(
       logits, logit_paddings, labels, label_paddings,
       blank_id=blank_id, log_epsilon=log_epsilon)
   return per_seq_loss
 
 
-def kl_divergence(log_predictions: chex.Array,
-                  targets: chex.Array) -> chex.Array:
+def convex_kl_divergence(
+    log_predictions: chex.Array, targets: chex.Array
+) -> chex.Array:
+  """Computes a convex version of the Kullback-Leibler divergence loss.
+
+  Measures the information gain achieved if target probability distribution
+  would be used instead of predicted probability distribution.
+  This version is jointly convex in p (targets) and q (log_predictions).
+
+  References:
+    [Kullback, Leibler, 1951](https://www.jstor.org/stable/2236703)
+
+  Args:
+    log_predictions: Probabilities of predicted distribution with shape [...,
+      dim]. Expected to be in the log-space to avoid underflow.
+    targets: Probabilities of target distribution with shape [..., dim].
+      Expected to be strictly positive.
+
+  Returns:
+    Kullback-Leibler divergence of predicted distribution from target
+    distribution with shape [...].
+  """
+  return kl_divergence(log_predictions, targets) + jnp.sum(
+      jnp.exp(log_predictions) - targets, axis=-1
+  )
+
+
+def kl_divergence(
+    log_predictions: chex.Array, targets: chex.Array
+) -> chex.Array:
   """Computes the Kullback-Leibler divergence (relative entropy) loss.
 
   Measures the information gain achieved if target probability distribution
   would be used instead of predicted probability distribution.
 
   References:
     [Kullback, Leibler, 1951](https://www.jstor.org/stable/2236703)
 
   Args:
-    log_predictions: Probabilities of predicted distribution with shape
-      [..., dim]. Expected to be in the log-space to avoid underflow.
+    log_predictions: Probabilities of predicted distribution with shape [...,
+      dim]. Expected to be in the log-space to avoid underflow.
     targets: Probabilities of target distribution with shape [..., dim].
       Expected to be strictly positive.
 
   Returns:
     Kullback-Leibler divergence of predicted distribution from target
     distribution with shape [...].
   """
   chex.assert_type([log_predictions, targets], float)
-  loss = targets * (jnp.log(targets) - log_predictions)
+  loss = targets * (
+      jnp.where(targets == 0, 0, jnp.log(targets)) - log_predictions
+  )
   return jnp.sum(loss, axis=-1)
 
 
 def kl_divergence_with_log_targets(log_predictions: chex.Array,
                                    log_targets: chex.Array) -> chex.Array:
   """Computes the Kullback-Leibler divergence (relative entropy) loss.
```

### Comparing `optax-0.1.4/optax/_src/loss_test.py` & `optax-0.1.5/optax/_src/loss_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,42 @@
 import jax
 import jax.numpy as jnp
 import numpy as np
 
 from optax._src import loss
 
 
+class SquaredErrorTest(parameterized.TestCase):
+
+  def setUp(self):
+    super().setUp()
+    self.ys = jnp.array([-2., -1., 0.5, 1.])
+    self.ts = jnp.array([-1.5, 0., -1, 1.])
+    # compute expected outputs in numpy.
+    self.exp = (self.ts - self.ys) ** 2
+
+  @chex.all_variants
+  def test_scalar(self):
+    np.testing.assert_allclose(
+        self.variant(loss.squared_error)(
+            self.ys[0], self.ts[0]), self.exp[0])
+
+  @chex.all_variants
+  def test_batched(self):
+    np.testing.assert_allclose(
+        self.variant(loss.squared_error)(
+            self.ys, self.ts), self.exp)
+
+  @chex.all_variants
+  def test_shape_mismatch(self):
+    with self.assertRaises(AssertionError):
+      _ = self.variant(loss.squared_error)(
+          self.ys, jnp.expand_dims(self.ts, axis=-1))
+
+
 class L2LossTest(parameterized.TestCase):
 
   def setUp(self):
     super().setUp()
     self.ys = jnp.array([-2., -1., 0.5, 1.])
     self.ts = jnp.array([-1.5, 0., -1, 1.])
     # compute expected outputs in numpy.
@@ -417,25 +445,57 @@
     for n in range(batch_size):
       expected_loss = -sum(logprobs[n, t, k]
                            for t, k in enumerate(expected_alignment[n]))
       np.testing.assert_allclose(
           jnp.array(expected_loss), per_seq_loss[n], rtol=self._rtol)
 
 
+class ConvexKLDivergenceTest(parameterized.TestCase):
+
+  def setUp(self):
+    super().setUp()
+    self.log_ps = np.array([
+        [-2.9957, -3.5066, -3.9120, -1.2040, -0.6931, -2.3026],
+        [-1.6094, -1.6094, -1.6094, -2.3026, -1.8971, -1.8971],
+    ])
+    self.qs = np.array(
+        [[0.2, 0.2, 0.2, 0.1, 0.15, 0.15], [0.05, 0.03, 0.02, 0.3, 0.5, 0.0]]
+    )
+
+    # Computed convex kullback-leibler divergence of P from Q.
+    self.exp = np.array([0.88757247, 0.859308])
+
+  @chex.all_variants
+  def test_scalar(self):
+    np.testing.assert_allclose(
+        self.variant(loss.convex_kl_divergence)(self.log_ps[0], self.qs[0]),
+        self.exp[0],
+        atol=1e-4,
+    )
+
+  @chex.all_variants
+  def test_batched(self):
+    np.testing.assert_allclose(
+        self.variant(loss.convex_kl_divergence)(self.log_ps, self.qs),
+        self.exp,
+        atol=1e-4,
+    )
+
+
 class KLDivergenceTest(parameterized.TestCase):
 
   def setUp(self):
     super().setUp()
     self.log_ps = np.array(
         [[-2.9957, -3.5066, -3.9120, -1.2040, -0.6931, -2.3026],
          [-1.6094, -1.6094, -1.6094, -2.3026, -1.8971, -1.8971]])
     self.qs = np.array([[0.2, 0.2, 0.2, 0.1, 0.15, 0.15],
-                        [0.05, 0.03, 0.02, 0.3, 0.5, 0.1]])
+                        [0.05, 0.03, 0.02, 0.3, 0.5, 0.]])
     # Computed kullback-leibler divergence of P from Q.
-    self.exp = np.array([0.8875625, 0.7187435584901326])
+    self.exp = np.array([0.8875577, 0.7592807])
 
   @chex.all_variants
   def test_scalar(self):
     np.testing.assert_allclose(
         self.variant(loss.kl_divergence)(self.log_ps[0], self.qs[0]),
         self.exp[0],
         atol=1e-4)
```

### Comparing `optax-0.1.4/optax/_src/numerics.py` & `optax-0.1.5/optax/_src/numerics.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.4/optax/_src/numerics_test.py` & `optax-0.1.5/optax/_src/numerics_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
   def test_complex_vs_real_abs_sqr(self):
     # Tests that JAX generates the same HLO from `numerics.abs_sq`,
     # `jnp.square(x)`, `x * x`,  and `x**2`.
     real_sq_fns = (lambda x: x**2, lambda x: x * x, jnp.square)
 
     def _get_hlo_repr(f, x):
-      hlo_string = jax.xla_computation(f)(x).as_hlo_text()
+      hlo_string = jax.jit(f).lower(x).compiler_ir(dialect='hlo').as_hlo_text()
       return re.sub('HloModule.*?\n', '',
                     re.sub('ENTRY.*?{', 'ENTRY XXXX', hlo_string))
 
     # Real arg (same HLO).
     for real_sq_fn in real_sq_fns:
       for real_x in (3, 3.0, np.array([4, 5.2])):
         self.assertEqual(
```

### Comparing `optax-0.1.4/optax/_src/privacy.py` & `optax-0.1.5/optax/_src/privacy.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.4/optax/_src/privacy_test.py` & `optax-0.1.5/optax/_src/privacy_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         seed=0)
     state = dp_agg.init(self.params)
     update_fn = self.variant(dp_agg.update)
     mean_grads = jax.tree_util.tree_map(lambda g: g.mean(0), self.per_eg_grads)
 
     for _ in range(3):
       updates, state = update_fn(self.per_eg_grads, state)
-      chex.assert_tree_all_close(updates, mean_grads)
+      chex.assert_trees_all_close(updates, mean_grads)
 
   @chex.all_variants
   @parameterized.parameters(0.5, 10.0, 20.0, 40.0, 80.0)
   def test_clipping_norm(self, l2_norm_clip):
     dp_agg = privacy.differentially_private_aggregate(
         l2_norm_clip=l2_norm_clip,
         noise_multiplier=0.,
@@ -72,15 +72,15 @@
     # we can easily compute what the values should be:
     expected_val = jnp.mean(jnp.arange(self.batch_size) / divisors)
     expected_tree = jax.tree_util.tree_map(
         lambda p: jnp.broadcast_to(expected_val, p.shape), self.params)
 
     for _ in range(3):
       updates, state = update_fn(self.per_eg_grads, state, self.params)
-      chex.assert_tree_all_close(updates, expected_tree, rtol=2e-7)
+      chex.assert_trees_all_close(updates, expected_tree, rtol=2e-7)
 
   @chex.all_variants
   @parameterized.parameters((3.0, 2.0), (1.0, 5.0), (100.0, 4.0), (1.0, 90.0))
   def test_noise_multiplier(self, l2_norm_clip, noise_multiplier):
     """Standard dev. of noise should be l2_norm_clip * noise_multiplier."""
     dp_agg = privacy.differentially_private_aggregate(
         l2_norm_clip=l2_norm_clip,
@@ -89,17 +89,17 @@
     state = dp_agg.init(None)
     update_fn = self.variant(dp_agg.update)
     expected_std = l2_norm_clip * noise_multiplier
 
     grads = [jnp.ones((1, 100, 100))]  # batch size 1
     for _ in range(3):
       updates, state = update_fn(grads, state)
-      chex.assert_tree_all_close(expected_std,
-                                 jnp.std(updates[0]),
-                                 atol=0.1 * expected_std)
+      chex.assert_trees_all_close(expected_std,
+                                  jnp.std(updates[0]),
+                                  atol=0.1 * expected_std)
 
   def test_aggregated_updates_as_input_fails(self):
     """Expect per-example gradients as input to this transform."""
     dp_agg = privacy.differentially_private_aggregate(l2_norm_clip=0.1,
                                                       noise_multiplier=1.1,
                                                       seed=2021)
     state = dp_agg.init(self.params)
```

### Comparing `optax-0.1.4/optax/_src/schedule.py` & `optax-0.1.5/optax/_src/schedule.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 import inspect
 from typing import Callable, Dict, Union, NamedTuple, Optional, Iterable, Sequence
 
 from absl import logging
 import chex
 import jax
 import jax.numpy as jnp
+import numpy as np
 
 from optax._src import base
 from optax._src import numerics
 
 
 def constant_schedule(
     value: Union[float, int]
@@ -203,15 +204,16 @@
 
   return schedule
 
 
 def cosine_decay_schedule(
     init_value: float,
     decay_steps: int,
-    alpha: float = 0.0
+    alpha: float = 0.0,
+    exponent: float = 1.0,
 ) -> base.Schedule:
   """Returns a function which implements cosine learning rate decay.
 
   The schedule does not restart when ``decay_steps`` has been reached. Instead,
   the learning rate remains constant afterwards. For a cosine schedule with
   restarts, :func:`optax.join_schedules` can be used to join several cosine
   decay schedules.
@@ -220,25 +222,28 @@
 
   Args:
     init_value: An initial value `init_v`.
     decay_steps: Positive integer - the number of steps for which to apply
       the decay for.
     alpha: Float. The minimum value of the multiplier used to adjust the
       learning rate.
+    exponent: Float. The default decay is 0.5 * (1 + cos(pi * t/T)), where t is
+      the current timestep and T is the `decay_steps`. The exponent modifies
+      this to be (0.5 * (1 + cos(pi * t/T))) ** exponent. Defaults to 1.0.
 
   Returns:
     schedule: A function that maps step counts to values.
   """
   if not decay_steps > 0:
     raise ValueError('The cosine_decay_schedule requires positive decay_steps!')
 
   def schedule(count):
     count = jnp.minimum(count, decay_steps)
     cosine_decay = 0.5 * (1 + jnp.cos(jnp.pi * count / decay_steps))
-    decayed = (1 - alpha) * cosine_decay + alpha
+    decayed = (1 - alpha) * cosine_decay ** exponent + alpha
     return init_value * decayed
 
   return schedule
 
 
 def _linear_interpolate(start: float, end: float, pct: float):
   return (end-start) * pct + start
@@ -278,17 +283,17 @@
     boundaries, scales = zip(*sorted(boundaries_and_scales.items()))
     if not all(scale >= 0. for scale in scales):
       raise ValueError(
           '`piecewise_interpolate_schedule` expects non-negative scale factors')
   else:
     boundaries, scales = (), ()
 
-  bounds = jnp.stack((0,) + boundaries)
-  values = jnp.cumprod(jnp.stack((init_value,) + scales))
-  interval_sizes = (bounds[1:] - bounds[:-1])
+  bounds = np.stack((0,) + boundaries)
+  values = np.cumprod(np.stack((init_value,) + scales))
+  interval_sizes = bounds[1:] - bounds[:-1]
 
   def schedule(count):
     indicator = (bounds[:-1] <= count) & (count < bounds[1:])
     pct = (count - bounds[:-1]) / interval_sizes
     interp_vals = interpolate_fn(values[:-1], values[1:], pct)
     return indicator.dot(interp_vals) + (bounds[-1] <= count) * values[-1]
 
@@ -384,51 +389,56 @@
       schedule will receive a step count indicating the number of steps since
       the previous boundary transition.
     boundaries: A list of integers (of length one less than schedules) that
       indicate when to transition between schedules.
   Returns:
     schedule: A function that maps step counts to values.
   """
-  def schedule(step: jnp.DeviceArray) -> jnp.DeviceArray:
+  def schedule(step: chex.Numeric) -> chex.Numeric:
     output = schedules[0](step)
     for boundary, schedule in zip(boundaries, schedules[1:]):
       output = jnp.where(step < boundary, output, schedule(step - boundary))
     return output
   return schedule
 
 
 def warmup_cosine_decay_schedule(
     init_value: float,
     peak_value: float,
     warmup_steps: int,
     decay_steps: int,
-    end_value: float = 0.0
+    end_value: float = 0.0,
+    exponent: float = 1.0,
 ) -> base.Schedule:
   """Linear warmup followed by cosine decay.
 
   Args:
     init_value: Initial value for the scalar to be annealed.
     peak_value: Peak value for scalar to be annealed at end of warmup.
     warmup_steps: Positive integer, the length of the linear warmup.
     decay_steps: Positive integer, the total length of the schedule. Note that
       this includes the warmup time, so the number of steps during which cosine
       annealing is applied is `decay_steps - warmup_steps`.
     end_value: End value of the scalar to be annealed.
+    exponent: Float. The default decay is 0.5 * (1 + cos(pi * t/T)), where t is
+      the current timestep and T is the `decay_steps`. The exponent modifies
+      this to be (0.5 * (1 + cos(pi * t/T))) ** exponent. Defaults to 1.0.
   Returns:
     schedule: A function that maps step counts to values.
   """
   schedules = [
       linear_schedule(
           init_value=init_value,
           end_value=peak_value,
           transition_steps=warmup_steps),
       cosine_decay_schedule(
           init_value=peak_value,
           decay_steps=decay_steps - warmup_steps,
-          alpha=end_value/peak_value)]
+          alpha=end_value/peak_value,
+          exponent=exponent)]
   return join_schedules(schedules, [warmup_steps])
 
 
 def warmup_exponential_decay_schedule(
     init_value: float,
     peak_value: float,
     warmup_steps: int,
@@ -572,15 +582,15 @@
 
     sched_hps, numeric_hps, other_hps = {}, {}, {}
     for name, value in bound_arguments.arguments.items():
       if name in static_args or isinstance(value, bool):
         other_hps[name] = value
       elif callable(value):
         sched_hps[name] = value
-      elif isinstance(value, (int, float, chex.Array)):
+      elif isinstance(value, (int, float, jax.Array, np.ndarray)):
         numeric_hps[name] = value
       else:
         other_hps[name] = value
 
     def schedule_fn(count, dtype):
       return {k: _convert_floats(f(count), dtype) for k, f in sched_hps.items()}
```

### Comparing `optax-0.1.4/optax/_src/schedule_test.py` & `optax-0.1.5/optax/_src/schedule_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import chex
 import jax
 import jax.numpy as jnp
 import numpy as np
 
 from optax._src import clipping
 from optax._src import schedule
+from optax._src import state_utils
 from optax._src import transform
 from optax._src import wrappers
 
 
 class ConstantTest(chex.TestCase):
 
   @chex.all_variants
@@ -364,14 +365,28 @@
             np.pi * np.array(
                 [0.0, 0.2, 0.4, 0.6, 0.8, 1., 1., 1., 1., 1., 1., 1.])))
     expected_multipliers = 0.9 * expected_multipliers + 0.1
     np.testing.assert_allclose(
         initial_value * expected_multipliers,
         np.array(generated_vals), atol=1e-3)
 
+  @chex.all_variants
+  def test_with_exponent(self):
+    """Check cosine schedule decay with exponent on."""
+    schedule_fn = self.variant(
+        schedule.cosine_decay_schedule(init_value=0.1,
+                                       decay_steps=100,
+                                       alpha=0.0,
+                                       exponent=2))
+    output = schedule_fn(np.array([0, 10, 50, 75, 100]))
+    np.testing.assert_allclose(
+        output,
+        np.array([0.1, 0.09516553580760956, 0.025, 0.0021446612663567066, 0.0]),
+        rtol=1e-6, atol=1e-8)
+
 
 class WarmupCosineDecayTest(chex.TestCase):
 
   @chex.all_variants
   @parameterized.named_parameters(
       ('with end value', 10, 0.5, 1e-4),
       ('without end value', 5, 3, 0.),)
@@ -385,14 +400,34 @@
         end_value=end_value,
     ))
 
     np.testing.assert_allclose(init_value, schedule_fn(0))
     np.testing.assert_allclose(peak_value, schedule_fn(100))
     np.testing.assert_allclose(end_value, schedule_fn(1000), rtol=1e-3)
 
+  @chex.all_variants
+  def test_with_exponent(self):
+    """Check that we get correct results when running with exponent on."""
+    schedule_fn = self.variant(schedule.warmup_cosine_decay_schedule(
+        init_value=0.2,
+        peak_value=1.21,
+        end_value=-3.0,
+        warmup_steps=50,
+        decay_steps=100,
+        exponent=2))
+    output = schedule_fn(np.array([0, 10, 50, 75, 100]))
+    np.testing.assert_allclose(
+        output, np.array([0.20000004768371582,
+                          0.4020000100135803,
+                          1.2100000381469727,
+                          -1.947500228881836,
+                          -3.000000238418579]),
+        rtol=1e-6, atol=1e-8
+    )
+
 
 class SGDRTest(chex.TestCase):
 
   @chex.all_variants
   @parameterized.named_parameters(
       ('with step decay', 1.6, 0.8, 0.4),
       ('without step_decay', 1.6, 1.6, 1.6),)
@@ -502,14 +537,18 @@
   def test_updates(self):
     optim = schedule.inject_hyperparams(transform.scale)(  # stateless
         step_size=schedule.piecewise_constant_schedule(
             3.0, {1: 5, 7: 2, 12: 1.5}))
 
     params = [jnp.zeros([], dtype=jnp.float32)]
     state = self.variant(optim.init)(params)
+
+    # A no-op change, to verify that tree map works.
+    state = state_utils.tree_map_params(optim, lambda v: v, state)
+
     update_fn = self.variant(optim.update)
     expected_step_size = [3.0]*2 + [15.0]*6 + [30.0]*5 + [45.0]*3
 
     grads = [jnp.ones([], dtype=jnp.float32)]
     for i in range(15):
       updates, state = update_fn(grads, state, params=params)
       np.testing.assert_almost_equal(updates[0], expected_step_size[i+1])
@@ -547,15 +586,15 @@
     for _ in range(5):
       updates, state = update_fn(grads, state, params)
       np.testing.assert_almost_equal(state.hyperparams['b1'], 0.0)
       np.testing.assert_almost_equal(state.hyperparams['b2'], 0.0)
       np.testing.assert_almost_equal(state.hyperparams['eps'], 1e-8)
       np.testing.assert_almost_equal(state.hyperparams['eps_root'], 0.0)
       assert 'eps' in state.hyperparams
-      chex.assert_tree_all_close(updates, grads)
+      chex.assert_trees_all_close(updates, grads)
 
   @chex.all_variants
   def test_overriding_hyperparam(self):
     optim = schedule.inject_hyperparams(clipping.clip_by_global_norm)(0.1)
     params = jnp.zeros((3, 5, 7))
     state = self.variant(optim.init)(params)
     update_fn = self.variant(optim.update)
@@ -579,15 +618,15 @@
     grads = params
     state = self.variant(optim.init)(params)
     updates, state = self.variant(optim.update)(grads, state)
     expected_updates = jax.tree_util.tree_map(
         lambda x: -0.1 * x if x.ndim > 1 else x, grads)
 
     assert set(state.hyperparams.keys()) == {'learning_rate'}, state.hyperparams
-    chex.assert_tree_all_close(updates, expected_updates)
+    chex.assert_trees_all_close(updates, expected_updates)
 
   @chex.all_variants
   @parameterized.named_parameters(('one_arg', 'b1'), ('two_arg', ['b1', 'b2']))
   def test_numeric_static_args(self, static_args):
     optim = schedule.inject_hyperparams(
         transform.scale_by_adam, static_args=static_args)(b1=0.9, b2=0.95)
```

### Comparing `optax-0.1.4/optax/_src/second_order.py` & `optax-0.1.5/optax/_src/second_order.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,19 +39,19 @@
 
 def ravel(p: Any) -> Array:
   return ravel_pytree(p)[0]
 
 
 def hvp(
     loss: LossFun,
-    v: jnp.DeviceArray,
+    v: jax.Array,
     params: Any,
-    inputs: jnp.DeviceArray,
-    targets: jnp.DeviceArray,
-) -> jnp.DeviceArray:
+    inputs: jax.Array,
+    targets: jax.Array,
+) -> jax.Array:
   """Performs an efficient vector-Hessian (of `loss`) product.
 
   Args:
     loss: the loss function.
     v: a vector of size `ravel(params)`.
     params: model parameters.
     inputs: inputs at which `loss` is evaluated.
@@ -65,17 +65,17 @@
   loss_fn = lambda p: loss(p, inputs, targets)
   return jax.jvp(jax.grad(loss_fn), [params], [unravel_fn(v)])[1]
 
 
 def hessian_diag(
     loss: LossFun,
     params: Any,
-    inputs: jnp.DeviceArray,
-    targets: jnp.DeviceArray,
-) -> jnp.DeviceArray:
+    inputs: jax.Array,
+    targets: jax.Array,
+) -> jax.Array:
   """Computes the diagonal hessian of `loss` at (`inputs`, `targets`).
 
   Args:
     loss: the loss function.
     params: model parameters.
     inputs: inputs at which `loss` is evaluated.
     targets: targets at which `loss` is evaluated.
@@ -90,15 +90,15 @@
 
 
 def fisher_diag(
     negative_log_likelihood: LossFun,
     params: Any,
     inputs: jnp.ndarray,
     targets: jnp.ndarray,
-) -> jnp.DeviceArray:
+) -> jax.Array:
   """Computes the diagonal of the (observed) Fisher information matrix.
 
   Args:
     negative_log_likelihood: the negative log likelihood function.
     params: model parameters.
     inputs: inputs at which `negative_log_likelihood` is evaluated.
     targets: targets at which `negative_log_likelihood` is evaluated.
```

### Comparing `optax-0.1.4/optax/_src/second_order_test.py` & `optax-0.1.5/optax/_src/second_order_test.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.4/optax/_src/stochastic_gradient_estimators.py` & `optax-0.1.5/optax/_src/stochastic_gradient_estimators.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.4/optax/_src/stochastic_gradient_estimators_test.py` & `optax-0.1.5/optax/_src/stochastic_gradient_estimators_test.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.4/optax/_src/test_utils.py` & `optax-0.1.5/optax/_src/test_utils.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.4/optax/_src/transform.py` & `optax-0.1.5/optax/_src/transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,29 +305,29 @@
 
 
 def scale_by_adam(
     b1: float = 0.9,
     b2: float = 0.999,
     eps: float = 1e-8,
     eps_root: float = 0.0,
-    mu_dtype: Optional[Any] = None,
+    mu_dtype: Optional[chex.ArrayDType] = None,
 ) -> base.GradientTransformation:
   """Rescale updates according to the Adam algorithm.
 
   References:
     [Kingma et al, 2014](https://arxiv.org/abs/1412.6980)
 
   Args:
     b1: Decay rate for the exponentially weighted average of grads.
     b2: Decay rate for the exponentially weighted average of squared grads.
     eps: Term added to the denominator to improve numerical stability.
     eps_root: Term added to the denominator inside the square-root to improve
       numerical stability when backpropagating gradients through the rescaling.
     mu_dtype: Optional `dtype` to be used for the first order accumulator; if
-      `None` then the `dtype is inferred from `params` and `updates`.
+      `None` then the `dtype` is inferred from `params` and `updates`.
 
   Returns:
     A `GradientTransformation` object.
   """
 
   mu_dtype = utils.canonicalize_dtype(mu_dtype)
 
@@ -361,29 +361,29 @@
 
 
 def scale_by_amsgrad(
     b1: float = 0.9,
     b2: float = 0.999,
     eps: float = 1e-8,
     eps_root: float = 0.0,
-    mu_dtype: Optional[Any] = None,
+    mu_dtype: Optional[chex.ArrayDType] = None,
 ) -> base.GradientTransformation:
   """Rescale updates according to the AMSGrad algorithm.
 
   References:
     [Reddi et al, 2018](https://openreview.net/forum?id=ryQu7f-RZ)
 
   Args:
     b1: Decay rate for the exponentially weighted average of grads.
     b2: Decay rate for the exponentially weighted average of squared grads.
     eps: Term added to the denominator to improve numerical stability.
     eps_root: Term added to the denominator inside the square-root to improve
       numerical stability when backpropagating gradients through the rescaling.
     mu_dtype: Optional `dtype` to be used for the first order accumulator; if
-      `None` then the `dtype is inferred from `params` and `updates`.
+      `None` then the `dtype` is inferred from `params` and `updates`.
 
   Returns:
     A `GradientTransformation` object.
   """
 
   mu_dtype = utils.canonicalize_dtype(mu_dtype)
 
@@ -445,14 +445,59 @@
     mu_hat = bias_correction(mu, b1, count_inc)
     updates = jax.tree_util.tree_map(lambda m, v: m / v, mu_hat, nu)
     return updates, ScaleByAdamState(count=count_inc, mu=mu, nu=nu)
 
   return base.GradientTransformation(init_fn, update_fn)
 
 
+class ScaleByLionState(NamedTuple):
+  """State for the Lion algorithm."""
+  count: chex.Array  # shape=(), dtype=jnp.int32.
+  mu: base.Updates
+
+
+def scale_by_lion(
+    b1: float = 0.9,
+    b2: float = 0.99,
+    mu_dtype: Optional[chex.ArrayDType] = None,
+) -> base.GradientTransformation:
+  """Rescale updates according to the Lion algorithm.
+
+  References:
+    [Chen et al, 2023](https://arxiv.org/abs/2302.06675)
+
+  Args:
+    b1: Rate for combining the momentum and the current grad.
+    b2: Decay rate for the exponentially weighted average of grads.
+    mu_dtype: Optional `dtype` to be used for the momentum; if
+      `None` then the `dtype is inferred from `params` and `updates`.
+
+  Returns:
+    A `GradientTransformation` object.
+  """
+
+  mu_dtype = utils.canonicalize_dtype(mu_dtype)
+
+  def init_fn(params):
+    mu = jax.tree_util.tree_map(  # moment
+        lambda t: jnp.zeros_like(t, dtype=mu_dtype), params)
+    return ScaleByLionState(count=jnp.zeros([], jnp.int32), mu=mu)
+
+  def update_fn(updates, state, params=None):
+    del params
+    updates_new = jax.tree_util.tree_map(
+        lambda g, m: jnp.sign((1. - b1) * g + b1 * m), updates, state.mu)
+    mu = update_moment(updates, state.mu, b2, 1)
+    mu = utils.cast_tree(mu, mu_dtype)
+    count_inc = numerics.safe_int32_increment(state.count)
+    return updates_new, ScaleByLionState(count=count_inc, mu=mu)
+
+  return base.GradientTransformation(init_fn, update_fn)
+
+
 ScaleState = base.EmptyState
 
 
 def scale(
     step_size: float
 ) -> base.GradientTransformation:
   """Scale updates by some fixed scalar `step_size`.
@@ -694,15 +739,15 @@
   return base.GradientTransformation(init_fn, update_fn)
 
 
 AddDecayedWeightsState = base.EmptyState
 
 
 def add_decayed_weights(
-    weight_decay: float = 0.0,
+    weight_decay: Union[float, jax.Array] = 0.0,
     mask: Optional[Union[Any, Callable[[base.Params], Any]]] = None
 ) -> base.GradientTransformation:
   """Add parameter scaled by `weight_decay`.
 
   Args:
     weight_decay: A scalar weight decay rate.
     mask: A tree with same structure as (or a prefix of) the params PyTree,
@@ -762,29 +807,24 @@
         lambda g: jnp.array(step_size, dtype=g.dtype) * g, updates)
     return updates, ScaleByScheduleState(
         count=numerics.safe_int32_increment(state.count))
 
   return base.GradientTransformation(init_fn, update_fn)
 
 
-class ScaleByFromageState(NamedTuple):
-  """Maintains count for step-size scheduling."""
-  count: chex.Array  # shape=(), dtype=jnp.int32
-
-
 class ScaleByTrustRatioState(NamedTuple):
   """The scale and decay trust ratio transformation is stateless."""
 
 
 def scale_by_trust_ratio(
     min_norm: float = 0.0,
     trust_coefficient: float = 1.,
     eps: float = 0.,
 ) -> base.GradientTransformation:
-  """Scale updates by trust ratio`.
+  """Scale updates by `trust ratio`.
 
   References:
     [You et. al 2020](https://arxiv.org/abs/1904.00962)
 
   Args:
     min_norm: Minimum norm for params and gradient norms; by default is zero.
     trust_coefficient: A multiplier for the trust ratio.
@@ -953,15 +993,15 @@
 
 
 def scale_by_sm3(
     b1: float = 0.9,
     b2: float = 1.0,
     eps: float = 1e-8
 ) -> base.GradientTransformation:
-  """Scale updates by sm3`.
+  """Scale updates by `sm3`.
 
   References:
     [Anil et. al 2019](https://arxiv.org/abs/1901.11150)
 
   Args:
     b1: Decay rate for the exponentially weighted average of grads.
     b2: Decay rate for the exponentially weighted average of squared grads.
@@ -1030,30 +1070,30 @@
 
 def scale_by_novograd(
     b1: float = 0.9,
     b2: float = 0.25,
     eps: float = 1e-8,
     eps_root: float = 0.0,
     weight_decay: float = 0.0,
-    mu_dtype: Optional[Any] = None,
+    mu_dtype: Optional[chex.ArrayDType] = None,
 ) -> base.GradientTransformation:
   """Computes NovoGrad updates.
 
   References:
     [Ginsburg et al, 2019](https://arxiv.org/abs/1905.11286)
 
   Args:
     b1: A decay rate for the exponentially weighted average of grads.
     b2: A decay rate for the exponentially weighted average of squared grads.
     eps: A term added to the denominator to improve numerical stability.
     eps_root: A term added to the denominator inside the square-root to improve
       numerical stability when backpropagating gradients through the rescaling.
     weight_decay: A scalar weight decay rate.
     mu_dtype: An optional `dtype` to be used for the first order accumulator; if
-      `None` then the `dtype is inferred from `params` and `updates`.
+      `None` then the `dtype` is inferred from `params` and `updates`.
 
   Returns:
     The corresponding `GradientTransformation`.
   """
 
   mu_dtype = utils.canonicalize_dtype(mu_dtype)
 
@@ -1137,7 +1177,8 @@
 # To be removed once checkpoints have updated.
 _safe_int32_increment = numerics.safe_int32_increment
 safe_int32_increment = numerics.safe_int32_increment
 AdditiveWeightDecayState = AddDecayedWeightsState
 additive_weight_decay = add_decayed_weights
 ClipState = clipping.ClipState
 ClipByGlobalNormState = clipping.ClipByGlobalNormState
+
```

### Comparing `optax-0.1.4/optax/_src/transform_test.py` & `optax-0.1.5/optax/_src/transform_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     self.init_params = (jnp.array([1., 2.]), jnp.array([3., 4.]))
     self.per_step_updates = (jnp.array([500., 5.]), jnp.array([300., 3.]))
 
   @chex.all_variants
   @parameterized.named_parameters([
       ('adam', transform.scale_by_adam),
       ('adamax', transform.scale_by_adamax),
+      ('lion', transform.scale_by_lion),
       ('rmsprop', transform.scale_by_rms),
       ('stddev', transform.scale_by_stddev),
       ('trust_ratio', transform.scale_by_trust_ratio),
       ('param_block_norm', transform.scale_by_param_block_norm),
       ('param_block_rms', transform.scale_by_param_block_rms),
   ])
   def test_scalers(self, scaler_constr):
@@ -91,15 +92,15 @@
             a=0.1*jnp.ones((2,), dtype=jnp.float32),
             b=jnp.zeros((2,), dtype=jnp.float32),))
     # Apply transform
     state = tx.init(weights)
     transform_fn = self.variant(tx.update)
     new_updates, _ = transform_fn(updates, state, weights)
     # Assert output as expected.
-    chex.assert_tree_all_close(new_updates, expected_tx_updates)
+    chex.assert_trees_all_close(new_updates, expected_tx_updates)
 
   @chex.all_variants
   def test_ema(self):
     values = jnp.array([5.0, 7.0])
     decay = 0.9
     d = decay
 
@@ -202,49 +203,49 @@
       updates_sgd_apply_every, state_sgd_apply_every = transform_fn(
           self.per_step_updates, state_sgd_apply_every)
       optax_sgd_apply_every_params = update.apply_updates(
           optax_sgd_apply_every_params, updates_sgd_apply_every)
 
       # Every k steps, check equivalence.
       if i % k == k-1:
-        chex.assert_tree_all_close(
+        chex.assert_trees_all_close(
             optax_sgd_apply_every_params, optax_sgd_params,
             atol=1e-6, rtol=1e-5)
       # Otherwise, check update is zero.
       else:
-        chex.assert_tree_all_close(
+        chex.assert_trees_all_close(
             updates_sgd_apply_every, zero_update, atol=0.0, rtol=0.0)
 
   def test_scale(self):
     updates = self.per_step_updates
     for i in range(1, STEPS + 1):
       factor = 0.1 ** i
       rescaler = transform.scale(factor)
       # Apply rescaling.
-      scaled_updates, _ = rescaler.update(updates, None)
+      scaled_updates, _ = rescaler.update(updates, {})
       # Manually scale updates.
       def rescale(t):
         return t * factor  # pylint:disable=cell-var-from-loop
       manual_updates = jax.tree_util.tree_map(rescale, updates)
       # Check the rescaled updates match.
-      chex.assert_tree_all_close(scaled_updates, manual_updates)
+      chex.assert_trees_all_close(scaled_updates, manual_updates)
 
   @parameterized.named_parameters([
       ('1d', [1.0, 2.0], [1.0, 2.0]),
       ('2d', [[1.0, 2.0], [3.0, 4.0]], [[-0.5, 0.5], [-0.5, 0.5]]),
       ('3d', [[[1., 2.], [3., 4.]],
               [[5., 6.], [7., 8.]]], [[[-1.5, -0.5], [0.5, 1.5]],
                                       [[-1.5, -0.5], [0.5, 1.5]]]),
   ])
   def test_centralize(self, inputs, outputs):
     inputs = jnp.asarray(inputs)
     outputs = jnp.asarray(outputs)
     centralizer = transform.centralize()
-    centralized_inputs, _ = centralizer.update(inputs, None)
-    chex.assert_tree_all_close(centralized_inputs, outputs)
+    centralized_inputs, _ = centralizer.update(inputs, {})
+    chex.assert_trees_all_close(centralized_inputs, outputs)
 
   @chex.all_variants
   def test_add_noise_has_correct_variance_scaling(self):
     # Prepare to compare noise with a rescaled unit-variance substitute.
     eta = 0.3
     gamma = 0.55
     seed = 314
@@ -263,36 +264,36 @@
       updates_i_unit, state_unit = noise_unit.update(updates, state_unit)
 
       scale = jnp.sqrt(eta / i**gamma)
 
       updates_i_rescaled = jax.tree_util.tree_map(
           lambda g, s=scale: g * s, updates_i_unit)
 
-      chex.assert_tree_all_close(updates_i, updates_i_rescaled, rtol=1e-4)
+      chex.assert_trees_all_close(updates_i, updates_i_rescaled, rtol=1e-4)
 
   def test_scale_by_optimistic_gradient(self):
 
     def f(params: jnp.ndarray) -> jnp.ndarray:
       return params['x'] ** 2
 
     initial_params = {
         'x': jnp.array(2.0)
     }
 
     og = transform.scale_by_optimistic_gradient()
     og_state = og.init(initial_params)
     # Provide some arbitrary previous gradient.
-    og_state.trace['x'] = 1.5
+    getattr(og_state, 'trace')['x'] = 1.5
 
     g = jax.grad(f)(initial_params)
-    og_true = 2 * g['x'] - og_state.trace['x']
+    og_true = 2 * g['x'] - getattr(og_state, 'trace')['x']
     og, og_state = og.update(g, og_state)
 
     # Compare transformation output with manually computed optimistic gradient.
-    chex.assert_tree_all_close(og_true, og['x'])
+    chex.assert_trees_all_close(og_true, og['x'])
 
   @chex.all_variants
   def test_bias_correction_bf16(self):
     bias_correction_fn = self.variant(transform.bias_correction)
     m = jnp.logspace(-10, 10, num=21, dtype=jnp.bfloat16)  # 1e-10 ... 1e10
     for decay in (0.9, 0.99, 0.999, 0.9995):
       for count in (1, 10, 100, 1000):
```

### Comparing `optax-0.1.4/optax/_src/update.py` & `optax-0.1.5/optax/_src/update.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.4/optax/_src/update_test.py` & `optax-0.1.5/optax/_src/update_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
   @chex.all_variants
   def test_apply_updates(self):
     params = ({'a': jnp.ones((3, 2))}, jnp.ones((1,)))
     grads = jax.tree_util.tree_map(lambda t: 2 * t, params)
     exp_params = jax.tree_util.tree_map(lambda t: 3 * t, params)
     new_params = self.variant(update.apply_updates)(params, grads)
 
-    chex.assert_tree_all_close(
+    chex.assert_trees_all_close(
         exp_params, new_params, atol=1e-10, rtol=1e-5)
 
   @chex.all_variants
   def test_apply_updates_mixed_precision(self):
     params = (
         {'a': jnp.ones((3, 2), dtype=jnp.bfloat16)},
         jnp.ones((1,), dtype=jnp.bfloat16))
@@ -51,33 +51,33 @@
   def test_incremental_update(self):
     params_1 = ({'a': jnp.ones((3, 2))}, jnp.ones((1,)))
     params_2 = jax.tree_util.tree_map(lambda t: 2 * t, params_1)
     exp_params = jax.tree_util.tree_map(lambda t: 1.5 * t, params_1)
     new_params = self.variant(
         update.incremental_update)(params_2, params_1, 0.5)
 
-    chex.assert_tree_all_close(
+    chex.assert_trees_all_close(
         exp_params, new_params, atol=1e-10, rtol=1e-5)
 
   @chex.all_variants
   def test_periodic_update(self):
     params_1 = ({'a': jnp.ones((3, 2))}, jnp.ones((1,)))
     params_2 = jax.tree_util.tree_map(lambda t: 2 * t, params_1)
 
     update_period = 5
     update_fn = self.variant(update.periodic_update)
 
     for j in range(3):
       for i in range(1, update_period):
         new_params = update_fn(
             params_2, params_1, j*update_period+i, update_period)
-        chex.assert_tree_all_close(
+        chex.assert_trees_all_close(
             params_1, new_params, atol=1e-10, rtol=1e-5)
 
       new_params = update_fn(
           params_2, params_1, (j+1)*update_period, update_period)
-      chex.assert_tree_all_close(
+      chex.assert_trees_all_close(
           params_2, new_params, atol=1e-10, rtol=1e-5)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `optax-0.1.4/optax/_src/utils.py` & `optax-0.1.5/optax/_src/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -55,16 +55,33 @@
     a: rank 3, tensor NxDxD.
     new_diags: NxD matrix, the new diagonals of each DxD matrix.
 
   Returns:
     NxDxD tensor, with the same contents as `a` but with the diagonal
       changed to `new_diags`.
   """
+  a_dim, new_diags_dim = len(a.shape), len(new_diags.shape)
+  if a_dim != 3:
+    raise ValueError(f'Expected `a` to be a 3D tensor, got {a_dim}D instead')
+  if new_diags_dim != 2:
+    raise ValueError(
+        f'Expected `new_diags` to be a 2D array, got {new_diags_dim}D instead'
+    )
   n, d, d1 = a.shape
-  assert d == d1
+  n_diags, d_diags = new_diags.shape
+  if d != d1:
+    raise ValueError(
+        f'Shape mismatch: expected `a.shape` to be {(n, d, d)}, '
+        f'got {(n, d, d1)} instead'
+    )
+  if d_diags != d or n_diags != n:
+    raise ValueError(
+        f'Shape mismatch: expected `new_diags.shape` to be {(n, d)}, '
+        f'got {(n_diags, d_diags)} instead'
+    )
 
   indices1 = jnp.repeat(jnp.arange(n), d)
   indices2 = jnp.tile(jnp.arange(d), n)
   indices3 = indices2
 
   # Use numpy array setting
   a = a.at[indices1, indices2, indices3].set(new_diags.flatten())
```

### Comparing `optax-0.1.4/optax/_src/wrappers.py` & `optax-0.1.5/optax/_src/wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,46 +11,47 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Transformation wrappers."""
 
 import functools
-from typing import Any, Callable, NamedTuple, Optional, Tuple, Union
+from typing import Any, Callable, NamedTuple, Optional, Protocol, Tuple, Union
 
 import chex
 import jax
 from jax import lax
 import jax.numpy as jnp
 from jax.tree_util import tree_flatten
 from jax.tree_util import tree_map
 from jax.tree_util import tree_unflatten
 import numpy as np
 from optax._src import base
 from optax._src import numerics
-import typing_extensions
 
 Array = jnp.ndarray
 
 
 def flatten(
     inner: base.GradientTransformation
-) -> base.GradientTransformation:
+) -> base.GradientTransformationExtraArgs:
   """Flattens parameters and gradients for init and update of inner transform.
 
   This can reduce the overhead of performing many calculations on lots of small
   variables, at the cost of slightly increased memory usage.
 
   Args:
     inner: Inner transformation to flatten inputs for.
 
   Returns:
-    New GradientTransformation.
+    New ``GradientTransformationExtraArgs``
   """
 
+  inner = base.with_extra_args_support(inner)
+
   def _flatten(params):
     """Flattens and concatenates all tensors in params to a single vector."""
     params, _ = tree_flatten(params)
     return jnp.concatenate([jnp.reshape(param, [-1]) for param in params])
 
   def _unflatten(updates, flat):
     """Extracts tensors from flat, using the structure and shapes of params."""
@@ -70,22 +71,24 @@
     ]
     return tree_unflatten(treedef, reshaped)
 
   def init_fn(params):
     flat = _flatten(params)
     return inner.init(flat)
 
-  def update_fn(updates, state, params=None):
+  def update_fn(updates, state, params=None, **extra_args):
     if params is not None:
       params = _flatten(params)
-    updates_flat, state = inner.update(_flatten(updates), state, params)
+    updates_flat, state = inner.update(
+        _flatten(updates), state, params, **extra_args
+    )
     updates = _unflatten(updates, updates_flat)
     return updates, state
 
-  return base.GradientTransformation(init_fn, update_fn)
+  return base.GradientTransformationExtraArgs(init_fn, update_fn)
 
 
 class ApplyIfFiniteState(NamedTuple):
   """State of the `GradientTransformation` returned by `apply_if_finite`.
 
   Fields:
     notfinite_count: Number of consecutive gradient updates containing an Inf or
@@ -118,35 +121,37 @@
   Args:
     inner: Inner transformation to be wrapped.
     max_consecutive_errors: Maximum number of consecutive gradient updates
       containing NaNs of Infs that the wrapped optimizer will ignore. After
       that many ignored updates, the optimizer will give up and accept.
 
   Returns:
-    New GradientTransformation.
+    New ``GradientTransformationExtraArgs``.
   """
 
+  inner = base.with_extra_args_support(inner)
+
   def init(params):
     return ApplyIfFiniteState(
         notfinite_count=jnp.zeros([], jnp.int32),
         last_finite=jnp.array(True, jnp.bool_),
         total_notfinite=jnp.zeros([], jnp.int32),
         inner_state=inner.init(params))
 
-  def update(updates, state, params=None):
+  def update(updates, state, params=None, **extra_args):
     inner_state = state.inner_state
     flat_updates = tree_flatten(updates)[0]
     isfinite = jnp.all(
         jnp.array([jnp.all(jnp.isfinite(p)) for p in flat_updates]))
     notfinite_count = jnp.where(
         isfinite, jnp.zeros([], jnp.int32),
         numerics.safe_int32_increment(state.notfinite_count))
 
     def do_update(_):
-      return inner.update(updates, inner_state, params)
+      return inner.update(updates, inner_state, params, **extra_args)
     def reject_update(_):
       return (tree_map(jnp.zeros_like, updates), inner_state)
 
     updates, new_inner_state = lax.cond(
         jnp.logical_or(isfinite, notfinite_count > max_consecutive_errors),
         do_update, reject_update, operand=None)
 
@@ -154,15 +159,15 @@
         notfinite_count=notfinite_count,
         last_finite=isfinite,
         total_notfinite=jnp.where(
             isfinite, state.total_notfinite,
             numerics.safe_int32_increment(state.total_notfinite)),
         inner_state=new_inner_state)
 
-  return base.GradientTransformation(init=init, update=update)
+  return base.GradientTransformationExtraArgs(init=init, update=update)
 
 
 def _zeros_tree_like(inp_tree):
   return jax.tree_util.tree_map(jnp.zeros_like, inp_tree)
 
 
 class MultiStepsState(NamedTuple):
@@ -184,15 +189,15 @@
   mini_step: Array
   gradient_step: Array
   inner_opt_state: Any
   acc_grads: Any
   skip_state: chex.ArrayTree = ()
 
 
-class ShouldSkipUpdateFunction(typing_extensions.Protocol):
+class ShouldSkipUpdateFunction(Protocol):
 
   def __call__(self, updates: base.Updates, gradient_step: Array,
                params: Optional[base.Params]) -> Tuple[Array, chex.ArrayTree]:
     """Returns true to indicate that updates should be skipped in a multi-step.
 
     Args:
       updates: The updates that the gradient transformation has proposed
@@ -315,15 +320,16 @@
         * to ignore updates with a norm square larger then 42, do
           `should_skip_update_fn=functools.partial(skip_large_updates,
                                                    max_norm_sq=42.)`.
         Note that the optimizer's state `MultiStepsState` contains a field
         `skip_state` in which debugging and monitoring information returned
         by `should_skip_update_fn` is written.
     """
-    self._opt = opt
+    self._opt = base.with_extra_args_support(opt)
+
     if isinstance(every_k_schedule, int):
       self._every_k_schedule = lambda step: every_k_schedule
     else:
       self._every_k_schedule = every_k_schedule
     self._use_grad_mean = use_grad_mean
 
     if self._use_grad_mean:
@@ -356,29 +362,30 @@
         acc_grads=updates,
         skip_state=skip_state)
     return init_state
 
   def update(self,
              updates: base.Updates,
              state: MultiStepsState,
-             params: Optional[base.Params] = None
+             params: Optional[base.Params] = None,
+             **extra_args: Any,
              ) -> Tuple[base.Updates, MultiStepsState]:
     """Accumulates gradients and proposes non-zero updates every `k_steps`."""
     k_steps = self._every_k_schedule(state.gradient_step)
     acc_grads = jax.tree_util.tree_map(
         functools.partial(self._acc_update, n_acc=state.mini_step),
         updates, state.acc_grads)
 
     should_skip_update, skip_state = self._should_skip_update_fn(
         updates, state.gradient_step, params)
 
     def final_step(args):
       del args
       final_updates, new_inner_state = self._opt.update(
-          acc_grads, state.inner_opt_state, params=params)
+          acc_grads, state.inner_opt_state, params=params, **extra_args)
       new_state = MultiStepsState(
           mini_step=jnp.zeros([], dtype=jnp.int32),
           gradient_step=numerics.safe_int32_increment(state.gradient_step),
           inner_opt_state=new_inner_state,
           acc_grads=_zeros_tree_like(acc_grads),
           skip_state=skip_state)
       return final_updates, new_state
@@ -416,16 +423,19 @@
     new_updates, new_state = jax.lax.cond(
         should_skip_update,
         (), lambda args: (zero_updates, multi_state_when_skip),
         (), lambda args: (new_updates, new_state))
 
     return new_updates, new_state
 
-  def has_updated(self, state: MultiStepsState) -> Array:
-    return jnp.logical_and(state.mini_step == 0, state.gradient_step > 0)
+  def has_updated(self, state: Union[MultiStepsState, chex.ArrayTree]) -> Array:
+    # Use `getattr` to bypass pytype checks.
+    return jnp.logical_and(
+        getattr(state, 'mini_step') == 0, getattr(state, 'gradient_step') > 0
+    )
 
   def gradient_transformation(self) -> base.GradientTransformation:
     return base.GradientTransformation(init=self.init, update=self.update)
 
 
 class MaskedState(NamedTuple):
   """Maintains inner transform state for masked transformations."""
@@ -440,15 +450,15 @@
   therefore be used to mask out parts of a tree.
   """
 
 
 def masked(
     inner: base.GradientTransformation,
     mask: Union[base.PyTree, Callable[[base.Params], base.PyTree]]
-) -> base.GradientTransformation:
+) -> base.GradientTransformationExtraArgs:
   """Mask updates so only some are transformed, the rest are passed through.
 
   For example, it is common to skip weight decay for BatchNorm scale and all
   bias parameters. In many networks, these are the only parameters with only
   one dimension. So, you may create a mask function to mask these out as
   follows::
 
@@ -468,50 +478,52 @@
     mask: a PyTree with same structure as (or a prefix of) the params PyTree, or
       a Callable that returns such a pytree given the params/updates. The leaves
       should be booleans, ``True`` for leaves/subtrees you want to apply the
       transformation to, and ``False`` for those you want to skip. The mask must
       be static for the gradient transformation to be jit-compilable.
 
   Returns:
-    New GradientTransformation wrapping ``inner``.
+    New ``GradientTransformationExtraArgs`` wrapping ``inner``.
   """
+  inner = base.with_extra_args_support(inner)
+
   def mask_pytree(pytree, mask_tree):
     return tree_map(lambda m, p: p if m else MaskedNode(), mask_tree, pytree)
 
   def init_fn(params):
     mask_tree = mask(params) if callable(mask) else mask
     masked_params = mask_pytree(params, mask_tree)
     return MaskedState(inner_state=inner.init(masked_params))
 
-  def update_fn(updates, state, params=None):
+  def update_fn(updates, state, params=None, **extra_args):
     mask_tree = mask(updates) if callable(mask) else mask
     masked_updates = mask_pytree(updates, mask_tree)
     masked_params = None if params is None else mask_pytree(params, mask_tree)
 
     new_masked_updates, new_inner_state = inner.update(
-        masked_updates, state.inner_state, masked_params)
+        masked_updates, state.inner_state, masked_params, **extra_args)
 
     new_updates = tree_map(
         lambda m, new_u, old_u: new_u if m else old_u,
         mask_tree, new_masked_updates, updates)
     return new_updates, MaskedState(inner_state=new_inner_state)
 
-  return base.GradientTransformation(init_fn, update_fn)
+  return base.GradientTransformationExtraArgs(init_fn, update_fn)
 
 
 class MaybeUpdateState(NamedTuple):
   """Maintains inner transform state and adds a step counter."""
   inner_state: Any
   step: Array
 
 
 def maybe_update(
     inner: base.GradientTransformation,
     should_update_fn: Callable[[Array], Array]
-) -> base.GradientTransformation:
+) -> base.GradientTransformationExtraArgs:
   """Calls the inner update function only at certain steps.
 
   Creates a transformation wrapper which counts the number of times the `update`
   function has been called. This counter is passed to the `should_update_fn` to
   decide when to call the inner update function.
 
   When not calling the inner update function, the `updates` and the inner state
@@ -520,28 +532,29 @@
 
   Args:
     inner: the inner transformation.
     should_update_fn: this function takes in a step counter (array of shape []
       and dtype int32), and returns a boolean array of shape [].
 
   Returns:
-    An `optax.GradientTransformation`.
+    A new ``GradientTransformationExtraArgs``.
   """
+  inner = base.with_extra_args_support(inner)
 
   def init_fn(params):
     return MaybeUpdateState(
         inner_state=inner.init(params), step=jnp.zeros([], dtype=jnp.int32))
 
-  def update_fn(updates, state, params=None):
+  def update_fn(updates, state, params=None, **extra_args):
 
     def do_update(_):
-      return inner.update(updates, state.inner_state, params)
+      return inner.update(updates, state.inner_state, params, **extra_args)
 
     def reject_update(_):
       return updates, state.inner_state
 
     updates, new_inner_state = lax.cond(
         should_update_fn(state.step), do_update, reject_update, operand=None)
     return updates, MaybeUpdateState(new_inner_state,
                                      numerics.safe_int32_increment(state.step))
 
-  return base.GradientTransformation(init_fn, update_fn)
+  return base.GradientTransformationExtraArgs(init_fn, update_fn)
```

### Comparing `optax-0.1.4/optax/_src/wrappers_test.py` & `optax-0.1.5/optax/_src/wrappers_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,18 @@
 
 import chex
 import haiku as hk
 import jax
 import jax.numpy as jnp
 import numpy as np
 from optax._src import alias
+from optax._src import base
 from optax._src import combine
 from optax._src import constrain
+from optax._src import state_utils
 from optax._src import transform
 from optax._src import update
 from optax._src import wrappers
 import tree
 
 
 def _build_sgd():
@@ -40,14 +42,28 @@
 def _build_stateful_sgd():
   # This SGD behaves like _build_sgd but also tests the optimizer state. The
   # momentum is set to zero rather than None so that the momentum terms are
   # calculated, but do not change the results.
   return alias.sgd(1., momentum=0.)
 
 
+def _build_sgd_extra_args():
+
+  def init_fn(params):
+    del params
+    return {'foo': 1}
+
+  def update_fn(grads, state, params=None, *, foo=None, **extra_args):
+    del extra_args, foo, params
+    return grads, state
+
+  t = base.GradientTransformationExtraArgs(init_fn, update_fn)
+  return combine.chain(_build_sgd(), t)
+
+
 class WrappersTest(parameterized.TestCase):
 
   def test_flatten(self):
     def init_params():
       return (jnp.array([1., 2.]), jnp.array([3., 4.]))
 
     per_step_updates = (jnp.array([500., 5.]), jnp.array([300., 3.]))
@@ -58,26 +74,28 @@
     state_sgd = sgd.init(optax_sgd_params)
     updates_sgd, state_sgd = sgd.update(per_step_updates, state_sgd)
     sgd_params_no_flatten = update.apply_updates(optax_sgd_params, updates_sgd)
 
     # And now calculate new params with flattening
     optax_sgd_params = init_params()
     sgd = wrappers.flatten(sgd)
+
     state_sgd = sgd.init(optax_sgd_params)
     updates_sgd, state_sgd = sgd.update(per_step_updates, state_sgd)
     sgd_params_flatten = update.apply_updates(optax_sgd_params, updates_sgd)
 
     # Test that both give the same result
-    chex.assert_tree_all_close(
+    chex.assert_trees_all_close(
         sgd_params_no_flatten, sgd_params_flatten, atol=1e-7, rtol=1e-7)
 
   @chex.variants(with_jit=True, without_jit=True, with_pmap=True)
   @parameterized.named_parameters(
       ('sgd', _build_sgd),
       ('stateful_sgd', _build_stateful_sgd),
+      ('sgd_extra_args', _build_sgd_extra_args),
   )
   def test_apply_if_finite(self, opt_builder):
     one = jnp.ones([])
     nan = jnp.array(jnp.nan)
     def fn(x):
       return x * hk.get_parameter('p', [], init=hk.initializers.Constant(0.))
 
@@ -89,43 +107,43 @@
     # Do one successful param update
     grads = grads_fn(params, one)
     updates, state = opt.update(grads, state, params)
     params = update.apply_updates(params, updates)
     # We know exactly what should be the value of params since we are
     # effectively using sgd in all cases.
     self.assertEqual(-1., float(jax.tree_util.tree_flatten(params)[0][0]))
-    self.assertTrue(bool(state.last_finite))
+    self.assertTrue(bool(getattr(state, 'last_finite')))
     # Check 2 rejected param updates
     for step in range(2):
       grads = grads_fn(params, nan)
       updates, state = opt.update(grads, state, params)
       params = update.apply_updates(params, updates)
       self.assertEqual(-1., float(jax.tree_util.tree_flatten(params)[0][0]))
-      self.assertFalse(bool(state.last_finite))
-      self.assertEqual(step + 1, int(state.notfinite_count))
+      self.assertFalse(bool(getattr(state, 'last_finite')))
+      self.assertEqual(step + 1, int(getattr(state, 'notfinite_count')))
     # Next successful param update
     grads = grads_fn(params, one)
     updates, state = opt.update(grads, state, params)
     params = update.apply_updates(params, updates)
     self.assertEqual(-2., float(jax.tree_util.tree_flatten(params)[0][0]))
-    self.assertTrue(bool(state.last_finite))
+    self.assertTrue(bool(getattr(state, 'last_finite')))
     # Again 2 rejected param updates
     for step in range(2):
       grads = grads_fn(params, nan)
       updates, state = opt.update(grads, state, params)
       params = update.apply_updates(params, updates)
       self.assertEqual(-2., float(jax.tree_util.tree_flatten(params)[0][0]))
-      self.assertFalse(bool(state.last_finite))
-      self.assertEqual(step + 1, int(state.notfinite_count))
+      self.assertFalse(bool(getattr(state, 'last_finite')))
+      self.assertEqual(step + 1, int(getattr(state, 'notfinite_count')))
     # Next param update with NaN is accepted since we reached maximum
     grads = grads_fn(params, nan)
     updates, state = opt.update(grads, state, params)
     params = update.apply_updates(params, updates)
     self.assertTrue(bool(jnp.isnan(jax.tree_util.tree_flatten(params)[0][0])))
-    self.assertEqual(5, int(state.total_notfinite))
+    self.assertEqual(5, int(getattr(state, 'total_notfinite')))
 
   def test_apply_if_finite_pmap(self):
     # Unlike in `test_apply_if_finite`:
     # * pmap is applied to the gradient computation and the optimisation;
     # * the NaNs are caused inside the function and do not come from the inputs.
     half = jnp.ones([1]) / 2.
     two = jnp.ones([1]) * 2.  # Causes a NaN in arctanh
@@ -185,14 +203,15 @@
     ms_opt = wrappers.MultiSteps(
         # Use a non-trivial inner optimiser:
         # * it has a state,
         # * it requires the params for the update.
         combine.chain(transform.scale_by_adam(),
                       transform.additive_weight_decay(1e-2),
                       transform.scale(-1e-4)), k_steps)
+
     opt_init, opt_update = ms_opt.gradient_transformation()
 
     # Put the training in one function, to check that the update is indeed
     # jittable.
     def train_step(data, opt_state, params):
       grad = jax.grad(loss_apply)(params, data)
       updates, opt_state = opt_update(grad, opt_state, params)
@@ -392,21 +411,27 @@
       return jax.tree_util.tree_map(
           lambda upd, m: -upd if m else upd, updates, mask)
     correct_updates = masked_negate(input_updates)
 
     init_fn, update_fn = wrappers.masked(opt_builder(), mask_arg)
     update_fn = self.variant(update_fn)
     state = self.variant(init_fn)(params)
+
+    # Known issue: masked does not work with arbitrary parameter trees, and
+    # so does not work with tree_map_params.
+    with self.assertRaises(ValueError):
+      state_utils.tree_map_params(init_fn, lambda v: v, state)
+
     updates, state = update_fn(input_updates, state, params)
-    chex.assert_tree_all_close(updates, correct_updates)
+    chex.assert_trees_all_close(updates, correct_updates)
 
     # Check repeated application, this time with no params.
     correct_updates = masked_negate(correct_updates)
     updates, state = update_fn(updates, state)
-    chex.assert_tree_all_close(updates, correct_updates)
+    chex.assert_trees_all_close(updates, correct_updates)
 
   @chex.all_variants
   @parameterized.named_parameters(
       ('sgd', _build_sgd),
       ('stateful_sgd', _build_stateful_sgd),
   )
   def test_prefix_mask(self, opt_builder):
@@ -422,21 +447,21 @@
     correct_updates = jax.tree_util.tree_map(
         _masked_sgd_on_updates, mask, input_updates)
 
     init_fn, update_fn = wrappers.masked(opt_builder(), mask)
     update_fn = self.variant(update_fn)
     state = self.variant(init_fn)(params)
     updates, state = update_fn(input_updates, state, params)
-    chex.assert_tree_all_close(updates, correct_updates)
+    chex.assert_trees_all_close(updates, correct_updates)
 
     # Check repeated application, this time with no params.
     correct_updates = jax.tree_util.tree_map(
         _masked_sgd_on_updates, mask, correct_updates)
     updates, state = update_fn(updates, state)
-    chex.assert_tree_all_close(updates, correct_updates)
+    chex.assert_trees_all_close(updates, correct_updates)
 
   @chex.all_variants
   def test_update_requires_params(self):
     weight_decay = 0.1
     mask = {'a': True,
             'b': [False, True],
             'c': {'d': True, 'e': (False, True)}}
@@ -450,24 +475,24 @@
 
     init_fn, update_fn = wrappers.masked(
         transform.additive_weight_decay(weight_decay), mask)
     update_fn = self.variant(update_fn)
 
     state = self.variant(init_fn)(params)
     updates, state = update_fn(input_updates, state, params)
-    chex.assert_tree_all_close(updates, correct_updates)
+    chex.assert_trees_all_close(updates, correct_updates)
 
     params = update.apply_updates(params, updates)
 
     # Test repeated application
     new_correct_updates = jax.tree_util.tree_map(
         lambda m, u, p: u + weight_decay * p if m else u,
         mask, correct_updates, params)
     updates, state = update_fn(correct_updates, state, params)
-    chex.assert_tree_all_close(updates, new_correct_updates)
+    chex.assert_trees_all_close(updates, new_correct_updates)
 
   @parameterized.parameters(list, tuple, dict)
   def test_empty(self, container):
     init_fn, update_fn = wrappers.masked(_build_sgd(), container())
     update_fn(container(), init_fn(container()))
 
   @parameterized.parameters(
```

### Comparing `optax-0.1.4/optax/experimental/__init__.py` & `optax-0.1.5/optax/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.4/optax/optax_test.py` & `optax-0.1.5/optax/optax_test.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.4/optax.egg-info/PKG-INFO` & `optax-0.1.5/optax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optax
-Version: 0.1.4
+Version: 0.1.5
 Summary: A gradient processing and optimisation library in JAX.
 Home-page: https://github.com/deepmind/optax
 Author: DeepMind
 Author-email: optax-dev@google.com
 License: Apache 2.0
 Keywords: reinforcement-learning python machine learning
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Optax
 
 ![CI status](https://github.com/deepmind/optax/workflows/tests/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/optax/badge/?version=latest)](http://optax.readthedocs.io)
```

### Comparing `optax-0.1.4/optax.egg-info/SOURCES.txt` & `optax-0.1.5/optax.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,16 @@
 optax/_src/numerics_test.py
 optax/_src/privacy.py
 optax/_src/privacy_test.py
 optax/_src/schedule.py
 optax/_src/schedule_test.py
 optax/_src/second_order.py
 optax/_src/second_order_test.py
+optax/_src/state_utils.py
+optax/_src/state_utils_test.py
 optax/_src/stochastic_gradient_estimators.py
 optax/_src/stochastic_gradient_estimators_test.py
 optax/_src/test_utils.py
 optax/_src/transform.py
 optax/_src/transform_test.py
 optax/_src/update.py
 optax/_src/update_test.py
```

### Comparing `optax-0.1.4/setup.py` & `optax-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     keywords='reinforcement-learning python machine learning',
     packages=find_namespace_packages(exclude=['*_test.py']),
     install_requires=_parse_requirements(
         os.path.join(_CURRENT_DIR, 'requirements', 'requirements.txt')),
     tests_require=_parse_requirements(
         os.path.join(_CURRENT_DIR, 'requirements', 'requirements-test.txt')),
     zip_safe=False,  # Required for full installation.
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
```

