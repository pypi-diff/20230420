# Comparing `tmp/serket-0.0.9.tar.gz` & `tmp/serket-0.2.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serket-0.0.9.tar", last modified: Wed Oct 26 06:30:48 2022, max compression
+gzip compressed data, was "serket-0.2.0b2.tar", last modified: Thu Apr 20 00:19:56 2023, max compression
```

## Comparing `serket-0.0.9.tar` & `serket-0.2.0b2.tar`

### file list

```diff
@@ -1,81 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 06:30:48.149571 serket-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-10-26 06:30:40.000000 serket-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-10-26 06:30:40.000000 serket-0.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    28445 2022-10-26 06:30:48.149571 serket-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    27596 2022-10-26 06:30:40.000000 serket-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 06:30:48.141571 serket-0.0.9/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-10-26 06:30:40.000000 serket-0.0.9/requirements/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 06:30:48.141571 serket-0.0.9/serket/
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-10-26 06:30:40.000000 serket-0.0.9/serket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 06:30:48.145571 serket-0.0.9/serket/experimental/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 06:30:40.000000 serket-0.0.9/serket/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7104 2022-10-26 06:30:40.000000 serket-0.0.9/serket/experimental/conv_semi_local.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 06:30:48.145571 serket-0.0.9/serket/fd/
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-10-26 06:30:40.000000 serket-0.0.9/serket/fd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4298 2022-10-26 06:30:40.000000 serket-0.0.9/serket/fd/fgrad.py
--rw-r--r--   0 runner    (1001) docker     (121)    22393 2022-10-26 06:30:40.000000 serket-0.0.9/serket/fd/finite_diff.py
--rw-r--r--   0 runner    (1001) docker     (121)     3217 2022-10-26 06:30:40.000000 serket-0.0.9/serket/fd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 06:30:48.145571 serket-0.0.9/serket/nn/
--rw-r--r--   0 runner    (1001) docker     (121)     5412 2022-10-26 06:30:40.000000 serket-0.0.9/serket/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8731 2022-10-26 06:30:40.000000 serket-0.0.9/serket/nn/activation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 06:30:48.145571 serket-0.0.9/serket/nn/blocks/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-10-26 06:30:40.000000 serket-0.0.9/serket/nn/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12130 2022-10-26 06:30:40.000000 serket-0.0.9/serket/nn/blocks/unet.py
--rw-r--r--   0 runner    (1001) docker     (121)    15595 2022-10-26 06:30:40.000000 serket-0.0.9/serket/nn/blocks/vgg.py
--rw-r--r--   0 runner    (1001) docker     (121)     7782 2022-10-26 06:30:40.000000 serket-0.0.9/serket/nn/blur.py
--rw-r--r--   0 runner    (1001) docker     (121)     2513 2022-10-26 06:30:40.000000 serket-0.0.9/serket/nn/containers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2551 2022-10-26 06:30:40.000000 serket-0.0.9/serket/nn/contrast.py
--rw-r--r--   0 runner    (1001) docker     (121)    43416 2022-10-26 06:30:40.000000 serket-0.0.9/serket/nn/convolution.py
--rw-r--r--   0 runner    (1001) docker     (121)     2507 2022-10-26 06:30:40.000000 serket-0.0.9/serket/nn/crop.py
--rw-r--r--   0 runner    (1001) docker     (121)     3882 2022-10-26 06:30:40.000000 serket-0.0.9/serket/nn/cutout.py
--rw-r--r--   0 runner    (1001) docker     (121)     2786 2022-10-26 06:30:40.000000 serket-0.0.9/serket/nn/dropout.py
--rw-r--r--   0 runner    (1001) docker     (121)     2123 2022-10-26 06:30:40.000000 serket-0.0.9/serket/nn/flatten.py
--rw-r--r--   0 runner    (1001) docker     (121)     1333 2022-10-26 06:30:40.000000 serket-0.0.9/serket/nn/flip.py
--rw-r--r--   0 runner    (1001) docker     (121)     7731 2022-10-26 06:30:40.000000 serket-0.0.9/serket/nn/fully_connected.py
--rw-r--r--   0 runner    (1001) docker     (121)      619 2022-10-26 06:30:40.000000 serket-0.0.9/serket/nn/laplace.py
--rw-r--r--   0 runner    (1001) docker     (121)    10381 2022-10-26 06:30:40.000000 serket-0.0.9/serket/nn/linear.py
--rw-r--r--   0 runner    (1001) docker     (121)     5629 2022-10-26 06:30:40.000000 serket-0.0.9/serket/nn/normalization.py
--rw-r--r--   0 runner    (1001) docker     (121)     1723 2022-10-26 06:30:40.000000 serket-0.0.9/serket/nn/padding.py
--rw-r--r--   0 runner    (1001) docker     (121)    11479 2022-10-26 06:30:40.000000 serket-0.0.9/serket/nn/pooling.py
--rw-r--r--   0 runner    (1001) docker     (121)     2647 2022-10-26 06:30:40.000000 serket-0.0.9/serket/nn/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (121)     3817 2022-10-26 06:30:40.000000 serket-0.0.9/serket/nn/random_transform.py
--rw-r--r--   0 runner    (1001) docker     (121)    33664 2022-10-26 06:30:40.000000 serket-0.0.9/serket/nn/recurrent.py
--rw-r--r--   0 runner    (1001) docker     (121)     5182 2022-10-26 06:30:40.000000 serket-0.0.9/serket/nn/resize.py
--rw-r--r--   0 runner    (1001) docker     (121)    13237 2022-10-26 06:30:40.000000 serket-0.0.9/serket/nn/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-10-26 06:30:40.000000 serket-0.0.9/serket/operators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 06:30:48.145571 serket-0.0.9/serket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    28445 2022-10-26 06:30:48.000000 serket-0.0.9/serket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1614 2022-10-26 06:30:48.000000 serket-0.0.9/serket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 06:30:48.000000 serket-0.0.9/serket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 06:30:48.000000 serket-0.0.9/serket.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-10-26 06:30:48.000000 serket-0.0.9/serket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-10-26 06:30:48.000000 serket-0.0.9/serket.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-26 06:30:48.149571 serket-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2147 2022-10-26 06:30:40.000000 serket-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 06:30:48.149571 serket-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 06:30:40.000000 serket-0.0.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6981 2022-10-26 06:30:40.000000 serket-0.0.9/tests/test_activation.py
--rw-r--r--   0 runner    (1001) docker     (121)      844 2022-10-26 06:30:40.000000 serket-0.0.9/tests/test_blocks.py
--rw-r--r--   0 runner    (1001) docker     (121)     2493 2022-10-26 06:30:40.000000 serket-0.0.9/tests/test_blur.py
--rw-r--r--   0 runner    (1001) docker     (121)     2125 2022-10-26 06:30:40.000000 serket-0.0.9/tests/test_contrast.py
--rw-r--r--   0 runner    (1001) docker     (121)    37004 2022-10-26 06:30:40.000000 serket-0.0.9/tests/test_convolution.py
--rw-r--r--   0 runner    (1001) docker     (121)     1957 2022-10-26 06:30:40.000000 serket-0.0.9/tests/test_crop.py
--rw-r--r--   0 runner    (1001) docker     (121)     1503 2022-10-26 06:30:40.000000 serket-0.0.9/tests/test_cutout.py
--rw-r--r--   0 runner    (1001) docker     (121)      843 2022-10-26 06:30:40.000000 serket-0.0.9/tests/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-10-26 06:30:40.000000 serket-0.0.9/tests/test_dropout.py
--rw-r--r--   0 runner    (1001) docker     (121)     5262 2022-10-26 06:30:40.000000 serket-0.0.9/tests/test_fgrad.py
--rw-r--r--   0 runner    (1001) docker     (121)     9515 2022-10-26 06:30:40.000000 serket-0.0.9/tests/test_finite_diff.py
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-10-26 06:30:40.000000 serket-0.0.9/tests/test_flatten.py
--rw-r--r--   0 runner    (1001) docker     (121)      515 2022-10-26 06:30:40.000000 serket-0.0.9/tests/test_flip.py
--rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-10-26 06:30:40.000000 serket-0.0.9/tests/test_fully_connected.py
--rw-r--r--   0 runner    (1001) docker     (121)     3581 2022-10-26 06:30:40.000000 serket-0.0.9/tests/test_gradient.py
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-10-26 06:30:40.000000 serket-0.0.9/tests/test_laplace2d.py
--rw-r--r--   0 runner    (1001) docker     (121)     3955 2022-10-26 06:30:40.000000 serket-0.0.9/tests/test_linear.py
--rw-r--r--   0 runner    (1001) docker     (121)     7525 2022-10-26 06:30:40.000000 serket-0.0.9/tests/test_normalization.py
--rw-r--r--   0 runner    (1001) docker     (121)      652 2022-10-26 06:30:40.000000 serket-0.0.9/tests/test_padding.py
--rw-r--r--   0 runner    (1001) docker     (121)     8257 2022-10-26 06:30:40.000000 serket-0.0.9/tests/test_pooling.py
--rw-r--r--   0 runner    (1001) docker     (121)    30465 2022-10-26 06:30:40.000000 serket-0.0.9/tests/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-10-26 06:30:40.000000 serket-0.0.9/tests/test_random_transformation.py
--rw-r--r--   0 runner    (1001) docker     (121)    24487 2022-10-26 06:30:40.000000 serket-0.0.9/tests/test_recurrent.py
--rw-r--r--   0 runner    (1001) docker     (121)     1118 2022-10-26 06:30:40.000000 serket-0.0.9/tests/test_repeat.py
--rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-10-26 06:30:40.000000 serket-0.0.9/tests/test_sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:19:56.003651 serket-0.2.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-20 00:19:45.000000 serket-0.2.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    36824 2023-04-20 00:19:56.003651 serket-0.2.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35973 2023-04-20 00:19:45.000000 serket-0.2.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:19:55.995651 serket-0.2.0b2/serket/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:19:55.995651 serket-0.2.0b2/serket/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/experimental/lazy_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/experimental/test_lazy_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:19:55.999651 serket-0.2.0b2/serket/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13148 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/activation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:19:55.999651 serket-0.2.0b2/serket/nn/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12172 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/blocks/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/blocks/vgg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/blur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/contrast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47883 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/cutout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40972 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/fft_convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/fully_connected.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/laplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14712 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/random_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37417 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/recurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:19:55.995651 serket-0.2.0b2/serket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36824 2023-04-20 00:19:55.000000 serket-0.2.0b2/serket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-20 00:19:55.000000 serket-0.2.0b2/serket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 00:19:55.000000 serket-0.2.0b2/serket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 00:19:55.000000 serket-0.2.0b2/serket.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-20 00:19:55.000000 serket-0.2.0b2/serket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-20 00:19:55.000000 serket-0.2.0b2/serket.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 00:19:56.003651 serket-0.2.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-20 00:19:45.000000 serket-0.2.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:19:56.003651 serket-0.2.0b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_blur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33451 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_cutout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20805 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_fft_convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_fully_connected.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_laplace2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30469 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_random_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_repeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22949 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_sequential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_utils.py
```

### Comparing `serket-0.0.9/PKG-INFO` & `serket-0.2.0b2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serket
-Version: 0.0.9
+Version: 0.2.0b2
 Summary: JAX NN library.
 Home-page: https://github.com/ASEM000/serket
 Author: Mahmoud Asem
 Author-email: asem00@kaist.ac.kr
 License: MIT
 Keywords: python machine-learning pytorch jax
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,194 +13,120 @@
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
 
-
 <div align="center">
-<img width="350px" src="assets/serketLogo.svg"></div>
+<img width="350px" src="assets/logo.svg"></div>
 
 <h2 align="center">The ✨Magical✨ JAX Scientific ML Library.</h2>
-<h5 align = "center"> *Serket is the goddess of magic in Egyptian mythology 
+<h5 align = "center"> *Serket is the goddess of magic in Egyptian mythology
 
 [**Installation**](#Installation)
 |[**Description**](#Description)
 |[**Quick Example**](#QuickExample)
 |[**Freezing/Fine tuning**](#Freezing)
 |[**Filtering**](#Filtering)
 
-
 ![Tests](https://github.com/ASEM000/serket/actions/workflows/tests.yml/badge.svg)
 ![pyver](https://img.shields.io/badge/python-3.7%203.8%203.9%203.10-red)
 ![codestyle](https://img.shields.io/badge/codestyle-black-lightgrey)
 [![Downloads](https://pepy.tech/badge/serket)](https://pepy.tech/project/serket)
 [![codecov](https://codecov.io/gh/ASEM000/serket/branch/main/graph/badge.svg?token=C6NXOK9EVS)](https://codecov.io/gh/ASEM000/serket)
 [![DOI](https://zenodo.org/badge/526985786.svg)](https://zenodo.org/badge/latestdoi/526985786)
 ![PyPI](https://img.shields.io/pypi/v/serket)
 
 </h5>
 
-
 ## 🛠️ Installation<a id="Installation"></a>
 
 ```python
 pip install serket
 ```
+
 **Install development version**
+
 ```python
 pip install git+https://github.com/ASEM000/serket
 ```
 
+## 📖 Description and motivation<a id="Description"></a>
 
-## 📖 Description<a id="Description"></a>
 - `serket` aims to be the most intuitive and easy-to-use physics-based Neural network library in JAX.
-- `serket` is built on top of [`pytreeclass`](https://github.com/ASEM000/pytreeclass)
 - `serket` is fully transparent to `jax` transformation (e.g. `vmap`,`grad`,`jit`,...)
+- `serket` current aim to facilitate the integration of numerical methods in a NN setting (see examples for more)
 
-<div align="center">
+### Layer structure
 
-### ➖➕Finite difference package: `serket.fd`➕➖
+`serket` is built on top of [`PyTreeClass`](https://github.com/ASEM000/pytreeclass), this means that layers are represented as a [PyTree](https://jax.readthedocs.io/en/latest/pytrees.html) whose leaves are the layer parameters.
 
-| Group| Function/Layer|
-| ------------- | ------------- |
-|Finite difference layer|`Difference`: apply finite difference to input array to any derivative order and accuracy|
-|Finite difference functions| - `difference`: finite difference of array with any accuracy and derivative order  <br> -`generate_finitediff_coeffs` : generate coeffs using sample points and derivative order <br> - `fgrad`: differentiate _functions_ (similar to `jax.grad`) with custom accuracy and derivative order|
-|Vector operator layers|`Curl`, `Divergence`, `Gradient`, `Laplacian`, `Jacobian`, `Hessian`|
-|Vector operator function| `curl`, `divergence`, `gradient`, `laplacian`, `jacobian`, `hessian`|
+<div align="center">
 
 ### 🧠 Neural network package: `serket.nn` 🧠
-| Group | Layers |
-| ------------- | ------------- |
-| Linear  | `Linear`, `Bilinear`, `Multilinear`, `GeneralLinear`, `Identity`   |
-|Densely connected|`FNN` (Fully connected network), `PFNN` (Parallel fully connected network)|
-| Convolution | `Conv1D`, `Conv2D`, `Conv3D`, `Conv1DTranspose` , `Conv2DTranspose`, `Conv3DTranspose`, `DepthwiseConv1D`, `DepthwiseConv2D`, `DepthwiseConv3D`, `SeparableConv1D`, `SeparableConv2D`, `SeparableConv3D`, `Conv1DLocal`, `Conv2DLocal`, `Conv3DLocal` |
-| Containers| `Sequential`, `Lambda` |
-|Pooling|`MaxPool1D`, `MaxPool2D`, `MaxPool3D`, `AvgPool1D`, `AvgPool2D`, `AvgPool3D` `GlobalMaxPool1D`, `GlobalMaxPool2D`, `GlobalMaxPool3D`, `GlobalAvgPool1D`, `GlobalAvgPool2D`, `GlobalAvgPool3D` `LPPool1D`, `LPPool2D`,`LPPool3D` , `AdaptivePool1D`, `AdaptivePool2D`, `AdaptivePool3D`,`AdaptiveConcatPool1D`,`AdaptiveConcatPool2D`,`AdaptiveConcatPool3D` (`kernex` backend)|
-|Reshaping|`Flatten`, `Unflatten`, `FlipLeftRight2D`, `FlipUpDown2D`, `Repeat1D`, `Repeat2D`, `Repeat3D`, `Resize1D`, `Resize2D`, `Resize3D`, `Upsample1D`, `Upsample2D`, `Upsample3D`, `Pad1D`, `Pad2D`, `Pad3D` |
-|Crop|`Crop1D`, `Crop2D`, |
-|Normalization|`LayerNorm`, `InstanceNorm`, `GroupNorm`|
-|Blurring| `AvgBlur2D`, `GaussianBlur2D`|
-|Dropout|`Dropout`, `Dropout1D`, `Dropout2D`, `Dropout3D`, |
-|Random transforms|`RandomCrop1D`, `RandomCrop2D`, `RandomApply`, `RandomCutout1D`, `RandomCutout2D`, `RandomZoom2D`, `RandomContrast2D` |
-|Misc|`HistogramEqualization2D`, `AdjustContrast2D`, `Filter2D`, `PixelShuffle`|
-|Activations|`AdaptiveLeakyReLU`,`AdaptiveReLU`,`AdaptiveSigmoid`,`AdaptiveTanh`,<br>`CeLU`,`ELU`,`GELU`,`GLU`<br>,`HardSILU`,`HardShrink`,`HardSigmoid`,`HardSwish`,`HardTanh`,<br>`LeakyReLU`,`LogSigmoid`,`LogSoftmax`,`Mish`,`PReLU`,<br> `ReLU`,`ReLU6`,`SILU`,`SeLU`,`Sigmoid`,`SoftPlus`,`SoftShrink`,<br>`SoftSign`,`Swish`,`Tanh`,`TanhShrink`, `ThresholdedReLU`, `Snake`|
-|Recurrent|`SimpleRNNCell`, `LSTMCell`, `ConvLSTM1D`, `ConvLSTM2D`, `ConvLSTM3D`, `SeparableConvLSTM1DCell`, `SeparableConvLSTM2DCell`, `SeparableConvLSTM3DCell`|
-|Blocks|`VGG16Block`, `VGG19Block`, `UNetBlock`|
-
-
 
+| Group                           | Layers                                                                                                                                                                                                                                                                                                                                                 |
+| ------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
+| Linear                          | - `Linear`, `Bilinear`, `Multilinear`, `GeneralLinear`, `Identity`, `Embedding`                                                                                                                                                                                                                                                                        |
+| Densely connected               | - `FNN` (Fully connected network),                                                                                                                                                                                                                                                                                                                     |
+| Convolution                     | - `{Conv,FFTConv}{1D,2D,3D}` <br> - `{Conv,FFTConv}{1D,2D,3D}Transpose` <br> - `{Depthwise,Separable}{Conv,FFTConv}{1D,2D,3D}` <br> - `Conv{1D,2D,3D}Local`                                                                                                                                                                                            |
+| Containers                      | - `Sequential`, `Lambda`                                                                                                                                                                                                                                                                                                                               |
+| Pooling <br> (`kernex` backend) | - `{Avg,Max,LP}Pool{1D,2D,3D}` <br> - `Global{Avg,Max}Pool{1D,2D,3D}` <br> - `Adaptive{Avg,Max}Pool{1D,2D,3D}`                                                                                                                                                                                                                                         |
+| Reshaping                       | - `Flatten`, `Unflatten`, <br> - `FlipLeftRight2D`, `FlipUpDown2D` <br> - `Resize{1D,2D,3D}` <br> - `Upsample{1D,2D,3D}` <br> - `Pad{1D,2D,3D}`                                                                                                                                                                                                        |
+| Crop                            | - `Crop{1D,2D}`                                                                                                                                                                                                                                                                                                                                        |
+| Normalization                   | - `{Layer,Instance,Group}Norm`                                                                                                                                                                                                                                                                                                                         |
+| Blurring                        | - `{Avg,Gaussian}Blur2D`                                                                                                                                                                                                                                                                                                                               |
+| Dropout                         | - `Dropout`<br> - `Dropout{1D,2D,3D}`                                                                                                                                                                                                                                                                                                                  |
+| Random transforms               | - `RandomCrop{1D,2D}` <br> - `RandomApply`, <br> - `RandomCutout{1D,2D}` <br> - `RandomZoom2D`, <br> - `RandomContrast2D`                                                                                                                                                                                                                              |
+| Misc                            | - `HistogramEqualization2D`, `AdjustContrast2D`, `Filter2D`, `PixelShuffle2D`                                                                                                                                                                                                                                                                          |
+| Activations                     | - `Adaptive{LeakyReLU,ReLU,Sigmoid,Tanh}`,<br> - `CeLU`,`ELU`,`GELU`,`GLU`<br>- `Hard{SILU,Shrink,Sigmoid,Swish,Tanh}`, <br> - `Soft{Plus,Sign,Shrink}` <br> - `LeakyReLU`,`LogSigmoid`,`LogSoftmax`,`Mish`,`PReLU`,<br> - `ReLU`,`ReLU6`,`SILU`,`SeLU`,`Sigmoid` <br> - `Swish`,`Tanh`,`TanhShrink`, `ThresholdedReLU`, `Snake`, `Stan`, `SquarePlus` |
+| Recurrent cells                 | - `{SimpleRNN,LSTM,GRU}Cell` <br> - `Conv{LSTM,GRU}{1D,2D,3D}Cell`                                                                                                                                                                                                                                                                                     |
+| Blocks                          | - `VGG{16,19}Block`, `UNetBlock`                                                                                                                                                                                                                                                                                                                       |
 
 </div>
 
 ## ⏩ Examples: <a id="QuickExample">
 
 <details>
-
-<summary> Finite difference examples </summary>
+<summary> Linear layers examples</summary>
 
 ```python
-import jax
-
-jax.config.update("jax_enable_x64", True)
 import jax.numpy as jnp
-import numpy.testing as npt
 
 import serket as sk
 
-
-# lets first define a vector valued function F: R^3 -> R^3
-# F = F1, F2
-# F1 = x^2 + y^3
-# F2 = x^4 + y^3
-# F3 = 0
-# F = [x**2 + y**3, x**4 + y**3, 0]
-
-x, y, z = [jnp.linspace(0, 1, 100)] * 3
-dx, dy, dz = x[1] - x[0], y[1] - y[0], z[1] - z[0]
-X, Y, Z = jnp.meshgrid(x, y, z, indexing="ij")
-F1 = X**2 + Y**3
-F2 = X**4 + Y**3
-F3 = jnp.zeros_like(F1)
-F = jnp.stack([F1, F2, F3], axis=0)
-
-# ∂F1/∂x : differentiate F1 with respect to x (i.e axis=0)
-dF1dx = sk.fd.difference(F1, axis=0, step_size=dx, accuracy=6)
-dF1dx_exact = 2 * X
-npt.assert_allclose(dF1dx, dF1dx_exact, atol=1e-7)
-
-# ∂F2/∂y : differentiate F2 with respect to y (i.e axis=1)
-dF2dy = sk.fd.difference(F2, axis=1, step_size=dy, accuracy=6)
-dF2dy_exact = 3 * Y**2
-npt.assert_allclose(dF2dy, dF2dy_exact, atol=1e-7)
-
-# ∇.F : the divergence of F
-divF = sk.fd.divergence(F, step_size=(dx, dy, dz), keepdims=False, accuracy=6)
-divF_exact = 2 * X + 3 * Y**2
-npt.assert_allclose(divF, divF_exact, atol=1e-7)
-
-# ∇F1 : the gradient of F1
-gradF1 = sk.fd.gradient(F1, step_size=(dx, dy, dz), accuracy=6)
-gradF1_exact = jnp.stack([2 * X, 3 * Y**2, 0 * X], axis=0)
-npt.assert_allclose(gradF1, gradF1_exact, atol=1e-7)
-
-# ΔF1 : laplacian of F1
-lapF1 = sk.fd.laplacian(F1, step_size=(dx, dy, dz), accuracy=6)
-lapF1_exact = 2 + 6 * Y
-npt.assert_allclose(lapF1, lapF1_exact, atol=1e-7)
-
-# ∇xF : the curl of F
-curlF = sk.fd.curl(F, step_size=(dx, dy, dz), accuracy=6)
-curlF_exact = jnp.stack([F1 * 0, F1 * 0, 4 * X**3 - 3 * Y**2], axis=0)
-npt.assert_allclose(curlF, curlF_exact, atol=1e-7)
-
-# Jacobian of F
-JF = sk.fd.jacobian(F, accuracy=4, step_size=(dx, dy, dz))
-JF_exact = jnp.array(
-    [
-        [2 * X, 3 * Y**2, jnp.zeros_like(X)],
-        [4 * X**3, 3 * Y**2, jnp.zeros_like(X)],
-        [jnp.zeros_like(X), jnp.zeros_like(X), jnp.zeros_like(X)],
-    ]
-)
-npt.assert_allclose(JF, JF_exact, atol=1e-7)
-
-# Hessian of F1
-HF1 = sk.fd.hessian(F1, accuracy=4, step_size=(dx, dy, dz))
-HF1_exact = jnp.array(
-    [
-        [
-            2 * jnp.ones_like(X),  # ∂2F1/∂x2
-            0 * jnp.ones_like(X),  # ∂2F1/∂xy
-            0 * jnp.ones_like(X),  # ∂2F1/∂xz
-        ],
-        [
-            0 * jnp.ones_like(X),  # ∂2F1/∂yx
-            6 * Y**2,              # ∂2F1/∂y2
-            0 * jnp.ones_like(X),  # ∂2F1/∂yz
-        ],
-        [
-            0 * jnp.ones_like(X),  # ∂2F1/∂zx
-            0 * jnp.ones_like(X),  # ∂2F1/∂zy
-            0 * jnp.ones_like(X),  # ∂2F1/∂z2
-        ],
-    ]
-)
-npt.assert_allclose(JF, JF_exact, atol=1e-7)
-
+# Linear
+x = jnp.ones([1, 2, 3, 4])
+l1 = sk.nn.Linear(4, 5)  # last dim is 4, output dim is 5
+print(l1(x).shape)  # (1, 2, 3, 5)
+
+# Bilinear
+x1, x2 = jnp.ones([1, 2, 3, 4]), jnp.ones([1, 2, 3, 5])
+l2 = sk.nn.Bilinear(4, 5, 6)  # last dim of the input x1,x2 are 4,5, output dim is 6
+print(l2(x1, x2).shape)  # (1, 2, 3, 6)
+
+# Multilinear
+x1, x2, x3 = jnp.ones([1, 2, 3, 4]), jnp.ones([1, 2, 3, 5]), jnp.ones([1, 2, 3, 6])
+l3 = sk.nn.Multilinear((4, 5, 6), 7)  # last dim for x1,x2,x3 = 4,5,6, output dim is 7
+print(l3(x1, x2, x3).shape)  # (1, 2, 3, 7)
+
+# GeneralLinear
+x = jnp.ones([4, 5, 6, 7])
+# apply a linear layer to axis 1,2,3, with dim = (5, 6, 7) and output dim is 5
+l4 = sk.nn.GeneralLinear((5, 6, 7), 5, in_axes=(1, 2, 3))
+print(l4(x).shape)  # (4, 5)
 ```
 
 </details>
 
-
 <details>
 <summary>
 Train Bidirectional-LSTM
 </summary>
 
 ```python
 import jax
@@ -295,27 +221,25 @@
 plt.legend()
 ```
 
 ![image](assets/rnn.svg)
 
 </details>
 
-
 <details>
 
 <summary>Lazy initialization</summary>
 
-In cases where `in_features` needs to be inferred from input, use `None` instead of `in_features` to infer the value at runtime. 
-However, since the lazy module initialize it's state after the first call (i.e. mutate it's state)  `jax` transformation ex: `vmap, grad ...` is not allowed before initialization. Using any `jax` transformation before initialization will throw a `ValueError`.
-
+In cases where `in_features` needs to be inferred from input, use `None` instead of `in_features` to infer the value at runtime.
+However, since the lazy module initialize it's state after the first call (i.e. mutate it's state) `jax` transformation ex: `vmap, grad ...` is not allowed before initialization. Using any `jax` transformation before initialization will throw a `ValueError`.
 
 ```python
-import serket as sk 
+import serket as sk
 import jax
-import jax.numpy as jnp 
+import jax.numpy as jnp
 
 model = sk.nn.Sequential(
     [
         sk.nn.Conv2D(None, 128, 3),
         sk.nn.ReLU(),
         sk.nn.MaxPool2D(2, 2),
         sk.nn.Conv2D(128, 64, 3),
@@ -369,15 +293,14 @@
 #   bias_init_func=Partial(zeros(key,shape,dtype)),
 #   *groups=1
 # )
 ```
 
 </details>
 
-
 <details>
 
 <summary>Train MNIST</summary>
 
 We will use `tensorflow` datasets for dataloading. for more on interface of jax/tensorflow dataset see [here](https://jax.readthedocs.io/en/latest/notebooks/neural_network_with_tfds_data.html)
 
 ```python
@@ -385,15 +308,15 @@
 import tensorflow as tf
 # Ensure TF does not see GPU and grab all GPU memory.
 tf.config.set_visible_devices([], device_type="GPU")
 import tensorflow_datasets as tfds
 import tensorflow.experimental.numpy as tnp
 import jax
 import jax.numpy as jnp
-import jax.random as jr 
+import jax.random as jr
 import optax  # for gradient optimization
 import serket as sk
 import matplotlib.pyplot as plt
 import functools as ft
 ```
 
 ```python
@@ -420,15 +343,15 @@
 # (batches, 1, 28, 28)
 ds_test = ds_test.map(preprocess_data).prefetch(tf.data.AUTOTUNE)
 ```
 
 ### 🏗️ Model definition
 
 We will use `jax.vmap(model)` to apply `model` on batches.
-    
+
 ```python
 @sk.treeclass
 class CNN:
     def __init__(self):
         self.conv1 = sk.nn.Conv2D(1, 32, (3, 3), padding="valid")
         self.relu1 = sk.nn.ReLU()
         self.pool1 = sk.nn.MaxPool2D((2, 2), strides=(2, 2))
@@ -451,15 +374,15 @@
         x = self.linear(x)
         return x
 
 model = CNN()
 ```
 
 ### 🎨 Visualize model
-    
+
 <details><summary>Model summary</summary>
     
 ```python
 print(model.summary(show_config=False, array=jnp.empty((1, 28, 28))))  
 ┌───────┬─────────┬─────────┬──────────────┬─────────────┬─────────────┐
 │Name   │Type     │Param #  │Size          │Input        │Output       │
 ├───────┼─────────┼─────────┼──────────────┼─────────────┼─────────────┤
@@ -554,35 +477,36 @@
     
 ```python
  
 # set all dropout off
 test_model = model.at[model == "eval"].set(True, is_leaf=lambda x: x is None)
 
 def show_images_with_predictions(model, images, one_hot_labels):
-    logits = jax.vmap(model)(images)
-    predictions = jnp.argmax(logits, axis=-1)
-    fig, axes = plt.subplots(5, 5, figsize=(10, 10))
-    for i, ax in enumerate(axes.flat):
-        ax.imshow(images[i].reshape(28, 28), cmap="binary")
-        ax.set(title=f"Prediction: {predictions[i]}\nLabel: {jnp.argmax(one_hot_labels[i], axis=-1)}")
-        ax.set_xticks([])
-        ax.set_yticks([])
-    plt.show()
+logits = jax.vmap(model)(images)
+predictions = jnp.argmax(logits, axis=-1)
+fig, axes = plt.subplots(5, 5, figsize=(10, 10))
+for i, ax in enumerate(axes.flat):
+ax.imshow(images[i].reshape(28, 28), cmap="binary")
+ax.set(title=f"Prediction: {predictions[i]}\nLabel: {jnp.argmax(one_hot_labels[i], axis=-1)}")
+ax.set_xticks([])
+ax.set_yticks([])
+plt.show()
 
 example = ds_test.take(25).as_numpy_iterator()
 example = list(example)
 sample_test_images = jnp.stack([x["image"] for x in example])
 sample_test_labels = jnp.stack([x["label"] for x in example])
 
 show_images_with_predictions(test_model, sample_test_images, sample_test_labels)
-```
+
+````
 ![image](assets/before_training.svg)
- 
+
 </details>
-    
+
 ### 🏃 Train the model
 
 ```python
 @ft.partial(jax.value_and_grad, has_aux=True)
 def loss_func(model, batched_images, batched_one_hot_labels):
     logits = jax.vmap(model)(batched_images)
     loss = jnp.mean(optax.softmax_cross_entropy(logits=logits, labels=batched_one_hot_labels))
@@ -615,23 +539,22 @@
         epoch_accuracy.append(accuracy)
         epoch_loss.append(loss)
 
     epoch_loss = jnp.mean(jnp.array(epoch_loss))
     epoch_accuracy = jnp.mean(jnp.array(epoch_accuracy))
 
     print(f"epoch:{i+1:00d}\tloss:{epoch_loss:.4f}\taccuracy:{epoch_accuracy:.4f}")
-    
+
 # epoch:1	loss:0.2706	accuracy:0.9268
 # epoch:2	loss:0.0725	accuracy:0.9784
 # epoch:3	loss:0.0533	accuracy:0.9836
 # epoch:4	loss:0.0442	accuracy:0.9868
 # epoch:5	loss:0.0368	accuracy:0.9889
-```
-    
-    
+````
+
 ### 🎨 Visualize After training
 
 ```python
 test_model = model.at[model == "eval"].set(True, is_leaf=lambda x: x is None)
 show_images_with_predictions(test_model, sample_test_images, sample_test_labels)
 ```
 
@@ -639,21 +562,121 @@
     
 ![image](assets/after_training.svg)
 
 </details>
 
 </details>
 
+<br>
+
+![image](https://img.shields.io/badge/-physics%20examples-blue)
+
+<details>
+
+<summary> Finite difference examples </summary>
+
+```python
+import jax
+
+jax.config.update("jax_enable_x64", True)
+import jax.numpy as jnp
+import numpy.testing as npt
+
+import serket as sk
+
+
+# lets first define a vector valued function F: R^3 -> R^3
+# F = F1, F2
+# F1 = x^2 + y^3
+# F2 = x^4 + y^3
+# F3 = 0
+# F = [x**2 + y**3, x**4 + y**3, 0]
+
+x, y, z = [jnp.linspace(0, 1, 100)] * 3
+dx, dy, dz = x[1] - x[0], y[1] - y[0], z[1] - z[0]
+X, Y, Z = jnp.meshgrid(x, y, z, indexing="ij")
+F1 = X**2 + Y**3
+F2 = X**4 + Y**3
+F3 = jnp.zeros_like(F1)
+F = jnp.stack([F1, F2, F3], axis=0)
+
+# ∂F1/∂x : differentiate F1 with respect to x (i.e axis=0)
+dF1dx = sk.fd.difference(F1, axis=0, step_size=dx, accuracy=6)
+dF1dx_exact = 2 * X
+npt.assert_allclose(dF1dx, dF1dx_exact, atol=1e-7)
+
+# ∂F2/∂y : differentiate F2 with respect to y (i.e axis=1)
+dF2dy = sk.fd.difference(F2, axis=1, step_size=dy, accuracy=6)
+dF2dy_exact = 3 * Y**2
+npt.assert_allclose(dF2dy, dF2dy_exact, atol=1e-7)
+
+# ∇.F : the divergence of F
+divF = sk.fd.divergence(F, step_size=(dx, dy, dz), keepdims=False, accuracy=6)
+divF_exact = 2 * X + 3 * Y**2
+npt.assert_allclose(divF, divF_exact, atol=1e-7)
+
+# ∇F1 : the gradient of F1
+gradF1 = sk.fd.gradient(F1, step_size=(dx, dy, dz), accuracy=6)
+gradF1_exact = jnp.stack([2 * X, 3 * Y**2, 0 * X], axis=0)
+npt.assert_allclose(gradF1, gradF1_exact, atol=1e-7)
+
+# ΔF1 : laplacian of F1
+lapF1 = sk.fd.laplacian(F1, step_size=(dx, dy, dz), accuracy=6)
+lapF1_exact = 2 + 6 * Y
+npt.assert_allclose(lapF1, lapF1_exact, atol=1e-7)
+
+# ∇xF : the curl of F
+curlF = sk.fd.curl(F, step_size=(dx, dy, dz), accuracy=6)
+curlF_exact = jnp.stack([F1 * 0, F1 * 0, 4 * X**3 - 3 * Y**2], axis=0)
+npt.assert_allclose(curlF, curlF_exact, atol=1e-7)
+
+# Jacobian of F
+JF = sk.fd.jacobian(F, accuracy=4, step_size=(dx, dy, dz))
+JF_exact = jnp.array(
+    [
+        [2 * X, 3 * Y**2, jnp.zeros_like(X)],
+        [4 * X**3, 3 * Y**2, jnp.zeros_like(X)],
+        [jnp.zeros_like(X), jnp.zeros_like(X), jnp.zeros_like(X)],
+    ]
+)
+npt.assert_allclose(JF, JF_exact, atol=1e-7)
+
+# Hessian of F1
+HF1 = sk.fd.hessian(F1, accuracy=4, step_size=(dx, dy, dz))
+HF1_exact = jnp.array(
+    [
+        [
+            2 * jnp.ones_like(X),  # ∂2F1/∂x2
+            0 * jnp.ones_like(X),  # ∂2F1/∂xy
+            0 * jnp.ones_like(X),  # ∂2F1/∂xz
+        ],
+        [
+            0 * jnp.ones_like(X),  # ∂2F1/∂yx
+            6 * Y**2,              # ∂2F1/∂y2
+            0 * jnp.ones_like(X),  # ∂2F1/∂yz
+        ],
+        [
+            0 * jnp.ones_like(X),  # ∂2F1/∂zx
+            0 * jnp.ones_like(X),  # ∂2F1/∂zy
+            0 * jnp.ones_like(X),  # ∂2F1/∂z2
+        ],
+    ]
+)
+npt.assert_allclose(JF, JF_exact, atol=1e-7)
+
+```
+
+</details>
 
 <details> 
 <summary> 
 PINN with Finite difference
 </summary>
 
-We will try to estimate NN(x)~f(x), where df(x)/dx = cos(x) and df(x)/dx will be represented with finite difference scheme
+We will try to estimate $NN(x)~f(x)$, where $df(x)/dx = cos(x)$ and $df(x)/dx$ will be represented with finite difference scheme. The following code compares between finite difference `fd` based implementation and automatic differentation `ad` based implementation.
 
 ```python
 import copy
 
 import jax
 import jax.numpy as jnp
 import matplotlib.pyplot as plt
@@ -737,23 +760,22 @@
 y_fd = NN_fd(x)
 y_ad = NN_ad(x)
 plt.plot(x, y, "--k", label="true")
 plt.plot(x, y_fd, label="fd pred")
 plt.plot(x, y_ad, label="ad pred")
 plt.legend()
 
-# Loss_fd 0.0012 
+# Loss_fd 0.0012
 # Loss_ad 0.0235
 ```
-![image](assets/fd_vs_ad.png)
 
+![image](assets/fd_vs_ad.png)
 
 </details>
 
-
 <details>
 <summary> 
 Reconstructing a vector field F using ∇.F = 0 and ∇xF=2k condition
 </summary>
 
 ```python
 import jax
@@ -783,18 +805,18 @@
 
 optim = optax.adam(1e-3)
 
 
 @jax.value_and_grad
 def loss_func(NN, F):
     F_pred = NN(F)
-    div = sk.fd.divergence(F_pred, accuracy=5, step_size=(dx, dy))  
+    div = sk.fd.divergence(F_pred, accuracy=5, step_size=(dx, dy))
     loss = jnp.mean(div**2)  # divergence free condition
     curl = sk.fd.curl(F_pred, accuracy=2, step_size=(dx, dy))
-    loss += jnp.mean((curl-jnp.ones_like(curl)*2)**2)  # curl condition 
+    loss += jnp.mean((curl-jnp.ones_like(curl)*2)**2)  # curl condition
     return loss
 
 
 @jax.jit
 def step(NN, F, optim_state):
     loss, grads = loss_func(NN, F)
     updates, optim_state = optim.update(grads, optim_state)
@@ -820,16 +842,153 @@
 plt.quiver(X, Y, F1, F2, color="k", alpha=0.5, label="true")
 plt.legend()
 
 ```
 
 ![image](assets/nn_div_free.svg)
 
+</details>
+
+<details>
+<summary>
+Vectorized differentiable stencil computation with `serket.kmap`
+</summary>
+
+Serket uses `kernex.kmap` decorator that applies a user-defined stencil kernel. `kmap` uses `jax.vmap` as it's backend to vectorized the operation, this means that the decorator is transparent to `jax` transformation.
+
+#### Example
+
+```python
+@sk.kmap(
+     # a kernel size applied to 2D input with size =3x3
+    kernel_size = (3,3),
+
+    # a strides = 1
+    strides= (1,1) ,
+
+    # padding can be among the following options
+    # 1) a single integer for each dimension -> ex: (1,) pads zeros before and after axis=0
+    # 2) a tuple of two integer for each dimension -> ex: ((1,2),) pads one zero on left and 2 zeros on right of axis=0
+    # 3) "same"/"valid"
+    # 4) "same"/"valid" tuple for each dimension -> ex: ("same",) same padding for axis=0
+    padding = "valid",
+
+    # relative means if the indexing should be row-col wise or center wise.
+    # for example in a 3x3  1..9 kernel , x[0,0] yields
+    # 1 if relative = False
+    # 5 if relative = True (i.e. the center value)
+    relative= True,
+
+)
+def avg_blur(x):
+    return (x[-1, -1] + x[-1, 0] + x[-1, 1] +
+            x[ 0, -1] + x[ 0, 0] + x[ 0, 1] +
+            x[ 1, -1] + x[ 1, 0] + x[ 1, 1]) // 9
+
+avg_blur(jnp.arange(1,26).reshape(5,5))
+# [[ 7  8  9]
+#  [12 13 14]
+#  [17 18 19]]
+```
+
+</details>
+
+<details>
+
+<summary>
+Scan a stencil kernel to solve linear convection using `serket.kscan`
+</summary>
+
+<div align ="center">
+
+$\Large {\partial u \over \partial t} + c {\partial u \over \partial x} = 0$ <br> <br>
+$\Large u_i^{n} = u_i^{n-1} - c \frac{\Delta t}{\Delta x}(u_i^{n-1}-u_{i-1}^{n-1})$
+
+<table>
+<tr>
+<td> Problem setup </td> <td> Stencil view  </td>
+</tr>
+<tr>
+<td>
+
+<img src="assets/linear_convection_init.png" width="500px">
+
+</td>
+<td>
+
+<img src="assets/linear_convection_view.png" width="500px">
+
+</td>
+</tr>
+</table>
+</div>
+
+By using `serket.kscan`, the stencil kernel can be scanned carrying along state, in a way similar to how RNN works. This enables BPTT algorithm that is useful for some problems (ex. time-dependent PDEs) .
+
+```python
+import jax
+import jax.numpy as jnp
+import serket as sk
+import matplotlib.pyplot as plt
+
+# see https://nbviewer.org/github/barbagroup/CFDPython/blob/master/lessons/01_Step_1.ipynb
+
+tmax,xmax = 0.5,2.0
+nt,nx = 151,51
+dt,dx = tmax/(nt-1) , xmax/(nx-1)
+u = jnp.ones([nt,nx])
+c = 0.5
+
+# kscan moves sequentially in row-major order and updates in-place using lax.scan.
+
+F = sk.kscan(
+        kernel_size = (3,3),
+        padding = ((1,1),(1,1)),
+        named_axis={0:'n',1:'i'},  # n for time axis , i for spatial axis (optional naming)
+        relative=True
+    )
+
+
+# boundary condtion as a function
+def bc(u):
+    return 1
+
+# initial condtion as a function
+def ic1(u):
+    return 1
+
+def ic2(u):
+    return 2
+
+def linear_convection(u):
+    return ( u['i','n-1'] - (c*dt/dx) * (u['i','n-1'] - u['i-1','n-1']) )
+
+
+F[:,0]  = F[:,-1] = bc # assign 1 for left and right boundary for all t
+
+# square wave initial condition
+F[:,:int((nx-1)/4)+1] = F[:,int((nx-1)/2):] = ic1
+F[0:1, int((nx-1)/4)+1 : int((nx-1)/2)] = ic2
+
+# assign linear convection function for
+# interior spatial location [1:-1]
+# and start from t>0  [1:]
+F[1:,1:-1] = linear_convection
+
+kx_solution = F(jnp.array(u))
+
+plt.figure(figsize=(20,7))
+for line in kx_solution[::20]:
+    plt.plot(jnp.linspace(0,xmax,nx),line)
+```
+
+![image](assets/linear_convection.svg)
 
 </details>
 
 ## 🥶 Freezing parameters /Fine tuning<a id="Freezing" >
 
 ✨[See here for more about freezing](https://github.com/ASEM000/PyTreeClass#%EF%B8%8F-model-surgery)✨
 
 ## 🔘 Filtering by masking<a id="Filtering" >
+
 ✨[See here for more about filterning ](https://github.com/ASEM000/PyTreeClass#%EF%B8%8F-filtering-with-at-)✨
```

### Comparing `serket-0.0.9/README.md` & `serket-0.2.0b2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,183 +1,109 @@
-
 <div align="center">
-<img width="350px" src="assets/serketLogo.svg"></div>
+<img width="350px" src="assets/logo.svg"></div>
 
 <h2 align="center">The ✨Magical✨ JAX Scientific ML Library.</h2>
-<h5 align = "center"> *Serket is the goddess of magic in Egyptian mythology 
+<h5 align = "center"> *Serket is the goddess of magic in Egyptian mythology
 
 [**Installation**](#Installation)
 |[**Description**](#Description)
 |[**Quick Example**](#QuickExample)
 |[**Freezing/Fine tuning**](#Freezing)
 |[**Filtering**](#Filtering)
 
-
 ![Tests](https://github.com/ASEM000/serket/actions/workflows/tests.yml/badge.svg)
 ![pyver](https://img.shields.io/badge/python-3.7%203.8%203.9%203.10-red)
 ![codestyle](https://img.shields.io/badge/codestyle-black-lightgrey)
 [![Downloads](https://pepy.tech/badge/serket)](https://pepy.tech/project/serket)
 [![codecov](https://codecov.io/gh/ASEM000/serket/branch/main/graph/badge.svg?token=C6NXOK9EVS)](https://codecov.io/gh/ASEM000/serket)
 [![DOI](https://zenodo.org/badge/526985786.svg)](https://zenodo.org/badge/latestdoi/526985786)
 ![PyPI](https://img.shields.io/pypi/v/serket)
 
 </h5>
 
-
 ## 🛠️ Installation<a id="Installation"></a>
 
 ```python
 pip install serket
 ```
+
 **Install development version**
+
 ```python
 pip install git+https://github.com/ASEM000/serket
 ```
 
+## 📖 Description and motivation<a id="Description"></a>
 
-## 📖 Description<a id="Description"></a>
 - `serket` aims to be the most intuitive and easy-to-use physics-based Neural network library in JAX.
-- `serket` is built on top of [`pytreeclass`](https://github.com/ASEM000/pytreeclass)
 - `serket` is fully transparent to `jax` transformation (e.g. `vmap`,`grad`,`jit`,...)
+- `serket` current aim to facilitate the integration of numerical methods in a NN setting (see examples for more)
 
-<div align="center">
+### Layer structure
 
-### ➖➕Finite difference package: `serket.fd`➕➖
+`serket` is built on top of [`PyTreeClass`](https://github.com/ASEM000/pytreeclass), this means that layers are represented as a [PyTree](https://jax.readthedocs.io/en/latest/pytrees.html) whose leaves are the layer parameters.
 
-| Group| Function/Layer|
-| ------------- | ------------- |
-|Finite difference layer|`Difference`: apply finite difference to input array to any derivative order and accuracy|
-|Finite difference functions| - `difference`: finite difference of array with any accuracy and derivative order  <br> -`generate_finitediff_coeffs` : generate coeffs using sample points and derivative order <br> - `fgrad`: differentiate _functions_ (similar to `jax.grad`) with custom accuracy and derivative order|
-|Vector operator layers|`Curl`, `Divergence`, `Gradient`, `Laplacian`, `Jacobian`, `Hessian`|
-|Vector operator function| `curl`, `divergence`, `gradient`, `laplacian`, `jacobian`, `hessian`|
+<div align="center">
 
 ### 🧠 Neural network package: `serket.nn` 🧠
-| Group | Layers |
-| ------------- | ------------- |
-| Linear  | `Linear`, `Bilinear`, `Multilinear`, `GeneralLinear`, `Identity`   |
-|Densely connected|`FNN` (Fully connected network), `PFNN` (Parallel fully connected network)|
-| Convolution | `Conv1D`, `Conv2D`, `Conv3D`, `Conv1DTranspose` , `Conv2DTranspose`, `Conv3DTranspose`, `DepthwiseConv1D`, `DepthwiseConv2D`, `DepthwiseConv3D`, `SeparableConv1D`, `SeparableConv2D`, `SeparableConv3D`, `Conv1DLocal`, `Conv2DLocal`, `Conv3DLocal` |
-| Containers| `Sequential`, `Lambda` |
-|Pooling|`MaxPool1D`, `MaxPool2D`, `MaxPool3D`, `AvgPool1D`, `AvgPool2D`, `AvgPool3D` `GlobalMaxPool1D`, `GlobalMaxPool2D`, `GlobalMaxPool3D`, `GlobalAvgPool1D`, `GlobalAvgPool2D`, `GlobalAvgPool3D` `LPPool1D`, `LPPool2D`,`LPPool3D` , `AdaptivePool1D`, `AdaptivePool2D`, `AdaptivePool3D`,`AdaptiveConcatPool1D`,`AdaptiveConcatPool2D`,`AdaptiveConcatPool3D` (`kernex` backend)|
-|Reshaping|`Flatten`, `Unflatten`, `FlipLeftRight2D`, `FlipUpDown2D`, `Repeat1D`, `Repeat2D`, `Repeat3D`, `Resize1D`, `Resize2D`, `Resize3D`, `Upsample1D`, `Upsample2D`, `Upsample3D`, `Pad1D`, `Pad2D`, `Pad3D` |
-|Crop|`Crop1D`, `Crop2D`, |
-|Normalization|`LayerNorm`, `InstanceNorm`, `GroupNorm`|
-|Blurring| `AvgBlur2D`, `GaussianBlur2D`|
-|Dropout|`Dropout`, `Dropout1D`, `Dropout2D`, `Dropout3D`, |
-|Random transforms|`RandomCrop1D`, `RandomCrop2D`, `RandomApply`, `RandomCutout1D`, `RandomCutout2D`, `RandomZoom2D`, `RandomContrast2D` |
-|Misc|`HistogramEqualization2D`, `AdjustContrast2D`, `Filter2D`, `PixelShuffle`|
-|Activations|`AdaptiveLeakyReLU`,`AdaptiveReLU`,`AdaptiveSigmoid`,`AdaptiveTanh`,<br>`CeLU`,`ELU`,`GELU`,`GLU`<br>,`HardSILU`,`HardShrink`,`HardSigmoid`,`HardSwish`,`HardTanh`,<br>`LeakyReLU`,`LogSigmoid`,`LogSoftmax`,`Mish`,`PReLU`,<br> `ReLU`,`ReLU6`,`SILU`,`SeLU`,`Sigmoid`,`SoftPlus`,`SoftShrink`,<br>`SoftSign`,`Swish`,`Tanh`,`TanhShrink`, `ThresholdedReLU`, `Snake`|
-|Recurrent|`SimpleRNNCell`, `LSTMCell`, `ConvLSTM1D`, `ConvLSTM2D`, `ConvLSTM3D`, `SeparableConvLSTM1DCell`, `SeparableConvLSTM2DCell`, `SeparableConvLSTM3DCell`|
-|Blocks|`VGG16Block`, `VGG19Block`, `UNetBlock`|
-
-
 
+| Group                           | Layers                                                                                                                                                                                                                                                                                                                                                 |
+| ------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
+| Linear                          | - `Linear`, `Bilinear`, `Multilinear`, `GeneralLinear`, `Identity`, `Embedding`                                                                                                                                                                                                                                                                        |
+| Densely connected               | - `FNN` (Fully connected network),                                                                                                                                                                                                                                                                                                                     |
+| Convolution                     | - `{Conv,FFTConv}{1D,2D,3D}` <br> - `{Conv,FFTConv}{1D,2D,3D}Transpose` <br> - `{Depthwise,Separable}{Conv,FFTConv}{1D,2D,3D}` <br> - `Conv{1D,2D,3D}Local`                                                                                                                                                                                            |
+| Containers                      | - `Sequential`, `Lambda`                                                                                                                                                                                                                                                                                                                               |
+| Pooling <br> (`kernex` backend) | - `{Avg,Max,LP}Pool{1D,2D,3D}` <br> - `Global{Avg,Max}Pool{1D,2D,3D}` <br> - `Adaptive{Avg,Max}Pool{1D,2D,3D}`                                                                                                                                                                                                                                         |
+| Reshaping                       | - `Flatten`, `Unflatten`, <br> - `FlipLeftRight2D`, `FlipUpDown2D` <br> - `Resize{1D,2D,3D}` <br> - `Upsample{1D,2D,3D}` <br> - `Pad{1D,2D,3D}`                                                                                                                                                                                                        |
+| Crop                            | - `Crop{1D,2D}`                                                                                                                                                                                                                                                                                                                                        |
+| Normalization                   | - `{Layer,Instance,Group}Norm`                                                                                                                                                                                                                                                                                                                         |
+| Blurring                        | - `{Avg,Gaussian}Blur2D`                                                                                                                                                                                                                                                                                                                               |
+| Dropout                         | - `Dropout`<br> - `Dropout{1D,2D,3D}`                                                                                                                                                                                                                                                                                                                  |
+| Random transforms               | - `RandomCrop{1D,2D}` <br> - `RandomApply`, <br> - `RandomCutout{1D,2D}` <br> - `RandomZoom2D`, <br> - `RandomContrast2D`                                                                                                                                                                                                                              |
+| Misc                            | - `HistogramEqualization2D`, `AdjustContrast2D`, `Filter2D`, `PixelShuffle2D`                                                                                                                                                                                                                                                                          |
+| Activations                     | - `Adaptive{LeakyReLU,ReLU,Sigmoid,Tanh}`,<br> - `CeLU`,`ELU`,`GELU`,`GLU`<br>- `Hard{SILU,Shrink,Sigmoid,Swish,Tanh}`, <br> - `Soft{Plus,Sign,Shrink}` <br> - `LeakyReLU`,`LogSigmoid`,`LogSoftmax`,`Mish`,`PReLU`,<br> - `ReLU`,`ReLU6`,`SILU`,`SeLU`,`Sigmoid` <br> - `Swish`,`Tanh`,`TanhShrink`, `ThresholdedReLU`, `Snake`, `Stan`, `SquarePlus` |
+| Recurrent cells                 | - `{SimpleRNN,LSTM,GRU}Cell` <br> - `Conv{LSTM,GRU}{1D,2D,3D}Cell`                                                                                                                                                                                                                                                                                     |
+| Blocks                          | - `VGG{16,19}Block`, `UNetBlock`                                                                                                                                                                                                                                                                                                                       |
 
 </div>
 
 ## ⏩ Examples: <a id="QuickExample">
 
 <details>
-
-<summary> Finite difference examples </summary>
+<summary> Linear layers examples</summary>
 
 ```python
-import jax
-
-jax.config.update("jax_enable_x64", True)
 import jax.numpy as jnp
-import numpy.testing as npt
 
 import serket as sk
 
-
-# lets first define a vector valued function F: R^3 -> R^3
-# F = F1, F2
-# F1 = x^2 + y^3
-# F2 = x^4 + y^3
-# F3 = 0
-# F = [x**2 + y**3, x**4 + y**3, 0]
-
-x, y, z = [jnp.linspace(0, 1, 100)] * 3
-dx, dy, dz = x[1] - x[0], y[1] - y[0], z[1] - z[0]
-X, Y, Z = jnp.meshgrid(x, y, z, indexing="ij")
-F1 = X**2 + Y**3
-F2 = X**4 + Y**3
-F3 = jnp.zeros_like(F1)
-F = jnp.stack([F1, F2, F3], axis=0)
-
-# ∂F1/∂x : differentiate F1 with respect to x (i.e axis=0)
-dF1dx = sk.fd.difference(F1, axis=0, step_size=dx, accuracy=6)
-dF1dx_exact = 2 * X
-npt.assert_allclose(dF1dx, dF1dx_exact, atol=1e-7)
-
-# ∂F2/∂y : differentiate F2 with respect to y (i.e axis=1)
-dF2dy = sk.fd.difference(F2, axis=1, step_size=dy, accuracy=6)
-dF2dy_exact = 3 * Y**2
-npt.assert_allclose(dF2dy, dF2dy_exact, atol=1e-7)
-
-# ∇.F : the divergence of F
-divF = sk.fd.divergence(F, step_size=(dx, dy, dz), keepdims=False, accuracy=6)
-divF_exact = 2 * X + 3 * Y**2
-npt.assert_allclose(divF, divF_exact, atol=1e-7)
-
-# ∇F1 : the gradient of F1
-gradF1 = sk.fd.gradient(F1, step_size=(dx, dy, dz), accuracy=6)
-gradF1_exact = jnp.stack([2 * X, 3 * Y**2, 0 * X], axis=0)
-npt.assert_allclose(gradF1, gradF1_exact, atol=1e-7)
-
-# ΔF1 : laplacian of F1
-lapF1 = sk.fd.laplacian(F1, step_size=(dx, dy, dz), accuracy=6)
-lapF1_exact = 2 + 6 * Y
-npt.assert_allclose(lapF1, lapF1_exact, atol=1e-7)
-
-# ∇xF : the curl of F
-curlF = sk.fd.curl(F, step_size=(dx, dy, dz), accuracy=6)
-curlF_exact = jnp.stack([F1 * 0, F1 * 0, 4 * X**3 - 3 * Y**2], axis=0)
-npt.assert_allclose(curlF, curlF_exact, atol=1e-7)
-
-# Jacobian of F
-JF = sk.fd.jacobian(F, accuracy=4, step_size=(dx, dy, dz))
-JF_exact = jnp.array(
-    [
-        [2 * X, 3 * Y**2, jnp.zeros_like(X)],
-        [4 * X**3, 3 * Y**2, jnp.zeros_like(X)],
-        [jnp.zeros_like(X), jnp.zeros_like(X), jnp.zeros_like(X)],
-    ]
-)
-npt.assert_allclose(JF, JF_exact, atol=1e-7)
-
-# Hessian of F1
-HF1 = sk.fd.hessian(F1, accuracy=4, step_size=(dx, dy, dz))
-HF1_exact = jnp.array(
-    [
-        [
-            2 * jnp.ones_like(X),  # ∂2F1/∂x2
-            0 * jnp.ones_like(X),  # ∂2F1/∂xy
-            0 * jnp.ones_like(X),  # ∂2F1/∂xz
-        ],
-        [
-            0 * jnp.ones_like(X),  # ∂2F1/∂yx
-            6 * Y**2,              # ∂2F1/∂y2
-            0 * jnp.ones_like(X),  # ∂2F1/∂yz
-        ],
-        [
-            0 * jnp.ones_like(X),  # ∂2F1/∂zx
-            0 * jnp.ones_like(X),  # ∂2F1/∂zy
-            0 * jnp.ones_like(X),  # ∂2F1/∂z2
-        ],
-    ]
-)
-npt.assert_allclose(JF, JF_exact, atol=1e-7)
-
+# Linear
+x = jnp.ones([1, 2, 3, 4])
+l1 = sk.nn.Linear(4, 5)  # last dim is 4, output dim is 5
+print(l1(x).shape)  # (1, 2, 3, 5)
+
+# Bilinear
+x1, x2 = jnp.ones([1, 2, 3, 4]), jnp.ones([1, 2, 3, 5])
+l2 = sk.nn.Bilinear(4, 5, 6)  # last dim of the input x1,x2 are 4,5, output dim is 6
+print(l2(x1, x2).shape)  # (1, 2, 3, 6)
+
+# Multilinear
+x1, x2, x3 = jnp.ones([1, 2, 3, 4]), jnp.ones([1, 2, 3, 5]), jnp.ones([1, 2, 3, 6])
+l3 = sk.nn.Multilinear((4, 5, 6), 7)  # last dim for x1,x2,x3 = 4,5,6, output dim is 7
+print(l3(x1, x2, x3).shape)  # (1, 2, 3, 7)
+
+# GeneralLinear
+x = jnp.ones([4, 5, 6, 7])
+# apply a linear layer to axis 1,2,3, with dim = (5, 6, 7) and output dim is 5
+l4 = sk.nn.GeneralLinear((5, 6, 7), 5, in_axes=(1, 2, 3))
+print(l4(x).shape)  # (4, 5)
 ```
 
 </details>
 
-
 <details>
 <summary>
 Train Bidirectional-LSTM
 </summary>
 
 ```python
 import jax
@@ -272,27 +198,25 @@
 plt.legend()
 ```
 
 ![image](assets/rnn.svg)
 
 </details>
 
-
 <details>
 
 <summary>Lazy initialization</summary>
 
-In cases where `in_features` needs to be inferred from input, use `None` instead of `in_features` to infer the value at runtime. 
-However, since the lazy module initialize it's state after the first call (i.e. mutate it's state)  `jax` transformation ex: `vmap, grad ...` is not allowed before initialization. Using any `jax` transformation before initialization will throw a `ValueError`.
-
+In cases where `in_features` needs to be inferred from input, use `None` instead of `in_features` to infer the value at runtime.
+However, since the lazy module initialize it's state after the first call (i.e. mutate it's state) `jax` transformation ex: `vmap, grad ...` is not allowed before initialization. Using any `jax` transformation before initialization will throw a `ValueError`.
 
 ```python
-import serket as sk 
+import serket as sk
 import jax
-import jax.numpy as jnp 
+import jax.numpy as jnp
 
 model = sk.nn.Sequential(
     [
         sk.nn.Conv2D(None, 128, 3),
         sk.nn.ReLU(),
         sk.nn.MaxPool2D(2, 2),
         sk.nn.Conv2D(128, 64, 3),
@@ -346,15 +270,14 @@
 #   bias_init_func=Partial(zeros(key,shape,dtype)),
 #   *groups=1
 # )
 ```
 
 </details>
 
-
 <details>
 
 <summary>Train MNIST</summary>
 
 We will use `tensorflow` datasets for dataloading. for more on interface of jax/tensorflow dataset see [here](https://jax.readthedocs.io/en/latest/notebooks/neural_network_with_tfds_data.html)
 
 ```python
@@ -362,15 +285,15 @@
 import tensorflow as tf
 # Ensure TF does not see GPU and grab all GPU memory.
 tf.config.set_visible_devices([], device_type="GPU")
 import tensorflow_datasets as tfds
 import tensorflow.experimental.numpy as tnp
 import jax
 import jax.numpy as jnp
-import jax.random as jr 
+import jax.random as jr
 import optax  # for gradient optimization
 import serket as sk
 import matplotlib.pyplot as plt
 import functools as ft
 ```
 
 ```python
@@ -397,15 +320,15 @@
 # (batches, 1, 28, 28)
 ds_test = ds_test.map(preprocess_data).prefetch(tf.data.AUTOTUNE)
 ```
 
 ### 🏗️ Model definition
 
 We will use `jax.vmap(model)` to apply `model` on batches.
-    
+
 ```python
 @sk.treeclass
 class CNN:
     def __init__(self):
         self.conv1 = sk.nn.Conv2D(1, 32, (3, 3), padding="valid")
         self.relu1 = sk.nn.ReLU()
         self.pool1 = sk.nn.MaxPool2D((2, 2), strides=(2, 2))
@@ -428,15 +351,15 @@
         x = self.linear(x)
         return x
 
 model = CNN()
 ```
 
 ### 🎨 Visualize model
-    
+
 <details><summary>Model summary</summary>
     
 ```python
 print(model.summary(show_config=False, array=jnp.empty((1, 28, 28))))  
 ┌───────┬─────────┬─────────┬──────────────┬─────────────┬─────────────┐
 │Name   │Type     │Param #  │Size          │Input        │Output       │
 ├───────┼─────────┼─────────┼──────────────┼─────────────┼─────────────┤
@@ -531,35 +454,36 @@
     
 ```python
  
 # set all dropout off
 test_model = model.at[model == "eval"].set(True, is_leaf=lambda x: x is None)
 
 def show_images_with_predictions(model, images, one_hot_labels):
-    logits = jax.vmap(model)(images)
-    predictions = jnp.argmax(logits, axis=-1)
-    fig, axes = plt.subplots(5, 5, figsize=(10, 10))
-    for i, ax in enumerate(axes.flat):
-        ax.imshow(images[i].reshape(28, 28), cmap="binary")
-        ax.set(title=f"Prediction: {predictions[i]}\nLabel: {jnp.argmax(one_hot_labels[i], axis=-1)}")
-        ax.set_xticks([])
-        ax.set_yticks([])
-    plt.show()
+logits = jax.vmap(model)(images)
+predictions = jnp.argmax(logits, axis=-1)
+fig, axes = plt.subplots(5, 5, figsize=(10, 10))
+for i, ax in enumerate(axes.flat):
+ax.imshow(images[i].reshape(28, 28), cmap="binary")
+ax.set(title=f"Prediction: {predictions[i]}\nLabel: {jnp.argmax(one_hot_labels[i], axis=-1)}")
+ax.set_xticks([])
+ax.set_yticks([])
+plt.show()
 
 example = ds_test.take(25).as_numpy_iterator()
 example = list(example)
 sample_test_images = jnp.stack([x["image"] for x in example])
 sample_test_labels = jnp.stack([x["label"] for x in example])
 
 show_images_with_predictions(test_model, sample_test_images, sample_test_labels)
-```
+
+````
 ![image](assets/before_training.svg)
- 
+
 </details>
-    
+
 ### 🏃 Train the model
 
 ```python
 @ft.partial(jax.value_and_grad, has_aux=True)
 def loss_func(model, batched_images, batched_one_hot_labels):
     logits = jax.vmap(model)(batched_images)
     loss = jnp.mean(optax.softmax_cross_entropy(logits=logits, labels=batched_one_hot_labels))
@@ -592,23 +516,22 @@
         epoch_accuracy.append(accuracy)
         epoch_loss.append(loss)
 
     epoch_loss = jnp.mean(jnp.array(epoch_loss))
     epoch_accuracy = jnp.mean(jnp.array(epoch_accuracy))
 
     print(f"epoch:{i+1:00d}\tloss:{epoch_loss:.4f}\taccuracy:{epoch_accuracy:.4f}")
-    
+
 # epoch:1	loss:0.2706	accuracy:0.9268
 # epoch:2	loss:0.0725	accuracy:0.9784
 # epoch:3	loss:0.0533	accuracy:0.9836
 # epoch:4	loss:0.0442	accuracy:0.9868
 # epoch:5	loss:0.0368	accuracy:0.9889
-```
-    
-    
+````
+
 ### 🎨 Visualize After training
 
 ```python
 test_model = model.at[model == "eval"].set(True, is_leaf=lambda x: x is None)
 show_images_with_predictions(test_model, sample_test_images, sample_test_labels)
 ```
 
@@ -616,21 +539,121 @@
     
 ![image](assets/after_training.svg)
 
 </details>
 
 </details>
 
+<br>
+
+![image](https://img.shields.io/badge/-physics%20examples-blue)
+
+<details>
+
+<summary> Finite difference examples </summary>
+
+```python
+import jax
+
+jax.config.update("jax_enable_x64", True)
+import jax.numpy as jnp
+import numpy.testing as npt
+
+import serket as sk
+
+
+# lets first define a vector valued function F: R^3 -> R^3
+# F = F1, F2
+# F1 = x^2 + y^3
+# F2 = x^4 + y^3
+# F3 = 0
+# F = [x**2 + y**3, x**4 + y**3, 0]
+
+x, y, z = [jnp.linspace(0, 1, 100)] * 3
+dx, dy, dz = x[1] - x[0], y[1] - y[0], z[1] - z[0]
+X, Y, Z = jnp.meshgrid(x, y, z, indexing="ij")
+F1 = X**2 + Y**3
+F2 = X**4 + Y**3
+F3 = jnp.zeros_like(F1)
+F = jnp.stack([F1, F2, F3], axis=0)
+
+# ∂F1/∂x : differentiate F1 with respect to x (i.e axis=0)
+dF1dx = sk.fd.difference(F1, axis=0, step_size=dx, accuracy=6)
+dF1dx_exact = 2 * X
+npt.assert_allclose(dF1dx, dF1dx_exact, atol=1e-7)
+
+# ∂F2/∂y : differentiate F2 with respect to y (i.e axis=1)
+dF2dy = sk.fd.difference(F2, axis=1, step_size=dy, accuracy=6)
+dF2dy_exact = 3 * Y**2
+npt.assert_allclose(dF2dy, dF2dy_exact, atol=1e-7)
+
+# ∇.F : the divergence of F
+divF = sk.fd.divergence(F, step_size=(dx, dy, dz), keepdims=False, accuracy=6)
+divF_exact = 2 * X + 3 * Y**2
+npt.assert_allclose(divF, divF_exact, atol=1e-7)
+
+# ∇F1 : the gradient of F1
+gradF1 = sk.fd.gradient(F1, step_size=(dx, dy, dz), accuracy=6)
+gradF1_exact = jnp.stack([2 * X, 3 * Y**2, 0 * X], axis=0)
+npt.assert_allclose(gradF1, gradF1_exact, atol=1e-7)
+
+# ΔF1 : laplacian of F1
+lapF1 = sk.fd.laplacian(F1, step_size=(dx, dy, dz), accuracy=6)
+lapF1_exact = 2 + 6 * Y
+npt.assert_allclose(lapF1, lapF1_exact, atol=1e-7)
+
+# ∇xF : the curl of F
+curlF = sk.fd.curl(F, step_size=(dx, dy, dz), accuracy=6)
+curlF_exact = jnp.stack([F1 * 0, F1 * 0, 4 * X**3 - 3 * Y**2], axis=0)
+npt.assert_allclose(curlF, curlF_exact, atol=1e-7)
+
+# Jacobian of F
+JF = sk.fd.jacobian(F, accuracy=4, step_size=(dx, dy, dz))
+JF_exact = jnp.array(
+    [
+        [2 * X, 3 * Y**2, jnp.zeros_like(X)],
+        [4 * X**3, 3 * Y**2, jnp.zeros_like(X)],
+        [jnp.zeros_like(X), jnp.zeros_like(X), jnp.zeros_like(X)],
+    ]
+)
+npt.assert_allclose(JF, JF_exact, atol=1e-7)
+
+# Hessian of F1
+HF1 = sk.fd.hessian(F1, accuracy=4, step_size=(dx, dy, dz))
+HF1_exact = jnp.array(
+    [
+        [
+            2 * jnp.ones_like(X),  # ∂2F1/∂x2
+            0 * jnp.ones_like(X),  # ∂2F1/∂xy
+            0 * jnp.ones_like(X),  # ∂2F1/∂xz
+        ],
+        [
+            0 * jnp.ones_like(X),  # ∂2F1/∂yx
+            6 * Y**2,              # ∂2F1/∂y2
+            0 * jnp.ones_like(X),  # ∂2F1/∂yz
+        ],
+        [
+            0 * jnp.ones_like(X),  # ∂2F1/∂zx
+            0 * jnp.ones_like(X),  # ∂2F1/∂zy
+            0 * jnp.ones_like(X),  # ∂2F1/∂z2
+        ],
+    ]
+)
+npt.assert_allclose(JF, JF_exact, atol=1e-7)
+
+```
+
+</details>
 
 <details> 
 <summary> 
 PINN with Finite difference
 </summary>
 
-We will try to estimate NN(x)~f(x), where df(x)/dx = cos(x) and df(x)/dx will be represented with finite difference scheme
+We will try to estimate $NN(x)~f(x)$, where $df(x)/dx = cos(x)$ and $df(x)/dx$ will be represented with finite difference scheme. The following code compares between finite difference `fd` based implementation and automatic differentation `ad` based implementation.
 
 ```python
 import copy
 
 import jax
 import jax.numpy as jnp
 import matplotlib.pyplot as plt
@@ -714,23 +737,22 @@
 y_fd = NN_fd(x)
 y_ad = NN_ad(x)
 plt.plot(x, y, "--k", label="true")
 plt.plot(x, y_fd, label="fd pred")
 plt.plot(x, y_ad, label="ad pred")
 plt.legend()
 
-# Loss_fd 0.0012 
+# Loss_fd 0.0012
 # Loss_ad 0.0235
 ```
-![image](assets/fd_vs_ad.png)
 
+![image](assets/fd_vs_ad.png)
 
 </details>
 
-
 <details>
 <summary> 
 Reconstructing a vector field F using ∇.F = 0 and ∇xF=2k condition
 </summary>
 
 ```python
 import jax
@@ -760,18 +782,18 @@
 
 optim = optax.adam(1e-3)
 
 
 @jax.value_and_grad
 def loss_func(NN, F):
     F_pred = NN(F)
-    div = sk.fd.divergence(F_pred, accuracy=5, step_size=(dx, dy))  
+    div = sk.fd.divergence(F_pred, accuracy=5, step_size=(dx, dy))
     loss = jnp.mean(div**2)  # divergence free condition
     curl = sk.fd.curl(F_pred, accuracy=2, step_size=(dx, dy))
-    loss += jnp.mean((curl-jnp.ones_like(curl)*2)**2)  # curl condition 
+    loss += jnp.mean((curl-jnp.ones_like(curl)*2)**2)  # curl condition
     return loss
 
 
 @jax.jit
 def step(NN, F, optim_state):
     loss, grads = loss_func(NN, F)
     updates, optim_state = optim.update(grads, optim_state)
@@ -797,16 +819,153 @@
 plt.quiver(X, Y, F1, F2, color="k", alpha=0.5, label="true")
 plt.legend()
 
 ```
 
 ![image](assets/nn_div_free.svg)
 
+</details>
+
+<details>
+<summary>
+Vectorized differentiable stencil computation with `serket.kmap`
+</summary>
+
+Serket uses `kernex.kmap` decorator that applies a user-defined stencil kernel. `kmap` uses `jax.vmap` as it's backend to vectorized the operation, this means that the decorator is transparent to `jax` transformation.
+
+#### Example
+
+```python
+@sk.kmap(
+     # a kernel size applied to 2D input with size =3x3
+    kernel_size = (3,3),
+
+    # a strides = 1
+    strides= (1,1) ,
+
+    # padding can be among the following options
+    # 1) a single integer for each dimension -> ex: (1,) pads zeros before and after axis=0
+    # 2) a tuple of two integer for each dimension -> ex: ((1,2),) pads one zero on left and 2 zeros on right of axis=0
+    # 3) "same"/"valid"
+    # 4) "same"/"valid" tuple for each dimension -> ex: ("same",) same padding for axis=0
+    padding = "valid",
+
+    # relative means if the indexing should be row-col wise or center wise.
+    # for example in a 3x3  1..9 kernel , x[0,0] yields
+    # 1 if relative = False
+    # 5 if relative = True (i.e. the center value)
+    relative= True,
+
+)
+def avg_blur(x):
+    return (x[-1, -1] + x[-1, 0] + x[-1, 1] +
+            x[ 0, -1] + x[ 0, 0] + x[ 0, 1] +
+            x[ 1, -1] + x[ 1, 0] + x[ 1, 1]) // 9
+
+avg_blur(jnp.arange(1,26).reshape(5,5))
+# [[ 7  8  9]
+#  [12 13 14]
+#  [17 18 19]]
+```
+
+</details>
+
+<details>
+
+<summary>
+Scan a stencil kernel to solve linear convection using `serket.kscan`
+</summary>
+
+<div align ="center">
+
+$\Large {\partial u \over \partial t} + c {\partial u \over \partial x} = 0$ <br> <br>
+$\Large u_i^{n} = u_i^{n-1} - c \frac{\Delta t}{\Delta x}(u_i^{n-1}-u_{i-1}^{n-1})$
+
+<table>
+<tr>
+<td> Problem setup </td> <td> Stencil view  </td>
+</tr>
+<tr>
+<td>
+
+<img src="assets/linear_convection_init.png" width="500px">
+
+</td>
+<td>
+
+<img src="assets/linear_convection_view.png" width="500px">
+
+</td>
+</tr>
+</table>
+</div>
+
+By using `serket.kscan`, the stencil kernel can be scanned carrying along state, in a way similar to how RNN works. This enables BPTT algorithm that is useful for some problems (ex. time-dependent PDEs) .
+
+```python
+import jax
+import jax.numpy as jnp
+import serket as sk
+import matplotlib.pyplot as plt
+
+# see https://nbviewer.org/github/barbagroup/CFDPython/blob/master/lessons/01_Step_1.ipynb
+
+tmax,xmax = 0.5,2.0
+nt,nx = 151,51
+dt,dx = tmax/(nt-1) , xmax/(nx-1)
+u = jnp.ones([nt,nx])
+c = 0.5
+
+# kscan moves sequentially in row-major order and updates in-place using lax.scan.
+
+F = sk.kscan(
+        kernel_size = (3,3),
+        padding = ((1,1),(1,1)),
+        named_axis={0:'n',1:'i'},  # n for time axis , i for spatial axis (optional naming)
+        relative=True
+    )
+
+
+# boundary condtion as a function
+def bc(u):
+    return 1
+
+# initial condtion as a function
+def ic1(u):
+    return 1
+
+def ic2(u):
+    return 2
+
+def linear_convection(u):
+    return ( u['i','n-1'] - (c*dt/dx) * (u['i','n-1'] - u['i-1','n-1']) )
+
+
+F[:,0]  = F[:,-1] = bc # assign 1 for left and right boundary for all t
+
+# square wave initial condition
+F[:,:int((nx-1)/4)+1] = F[:,int((nx-1)/2):] = ic1
+F[0:1, int((nx-1)/4)+1 : int((nx-1)/2)] = ic2
+
+# assign linear convection function for
+# interior spatial location [1:-1]
+# and start from t>0  [1:]
+F[1:,1:-1] = linear_convection
+
+kx_solution = F(jnp.array(u))
+
+plt.figure(figsize=(20,7))
+for line in kx_solution[::20]:
+    plt.plot(jnp.linspace(0,xmax,nx),line)
+```
+
+![image](assets/linear_convection.svg)
 
 </details>
 
 ## 🥶 Freezing parameters /Fine tuning<a id="Freezing" >
 
 ✨[See here for more about freezing](https://github.com/ASEM000/PyTreeClass#%EF%B8%8F-model-surgery)✨
 
 ## 🔘 Filtering by masking<a id="Filtering" >
+
 ✨[See here for more about filterning ](https://github.com/ASEM000/PyTreeClass#%EF%B8%8F-filtering-with-at-)✨
```

### Comparing `serket-0.0.9/serket/nn/__init__.py` & `serket-0.2.0b2/serket/nn/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,24 +23,26 @@
     ReLU6,
     SeLU,
     Sigmoid,
     Snake,
     SoftPlus,
     SoftShrink,
     SoftSign,
+    SquarePlus,
+    Stan,
     Swish,
     Tanh,
     TanhShrink,
     ThresholdedReLU,
 )
 from .blocks import UNetBlock, VGG16Block, VGG19Block
-from .blur import AvgBlur2D, Filter2D, GaussianBlur2D
+from .blur import AvgBlur2D, FFTFilter2D, Filter2D, GaussianBlur2D
 from .containers import Lambda, Sequential
 from .contrast import AdjustContrast2D, RandomContrast2D
-from .convolution import (  # Conv1DSemiLocal,; Conv2DSemiLocal,; Conv3DSemiLocal,
+from .convolution import (
     Conv1D,
     Conv1DLocal,
     Conv1DTranspose,
     Conv2D,
     Conv2DLocal,
     Conv2DTranspose,
     Conv3D,
@@ -52,28 +54,47 @@
     SeparableConv1D,
     SeparableConv2D,
     SeparableConv3D,
 )
 from .crop import Crop1D, Crop2D, Crop3D, RandomCrop1D, RandomCrop2D, RandomCrop3D
 from .cutout import RandomCutout1D, RandomCutout2D
 from .dropout import Dropout, Dropout1D, Dropout2D, Dropout3D
+from .fft_convolution import (
+    DepthwiseFFTConv1D,
+    DepthwiseFFTConv2D,
+    DepthwiseFFTConv3D,
+    FFTConv1D,
+    FFTConv1DTranspose,
+    FFTConv2D,
+    FFTConv2DTranspose,
+    FFTConv3D,
+    FFTConv3DTranspose,
+    SeparableFFTConv1D,
+    SeparableFFTConv2D,
+    SeparableFFTConv3D,
+)
 from .flatten import Flatten, Unflatten
 from .flip import FlipLeftRight2D, FlipUpDown2D
-from .fully_connected import FNN, PFNN
+from .fully_connected import FNN  # , PFNN
 from .laplace import Laplace2D
-from .linear import Bilinear, GeneralLinear, Identity, Linear, Multilinear
+from .linear import (
+    Bilinear,
+    Embedding,
+    GeneralLinear,
+    Identity,
+    Linear,
+    MergeLinear,
+    Multilinear,
+)
 from .normalization import GroupNorm, InstanceNorm, LayerNorm
 from .padding import Pad1D, Pad2D, Pad3D
 from .pooling import (
     AdaptiveAvgPool1D,
     AdaptiveAvgPool2D,
     AdaptiveAvgPool3D,
-    AdaptiveConcatPool1D,
-    AdaptiveConcatPool2D,
-    AdaptiveConcatPool3D,
     AdaptiveMaxPool1D,
     AdaptiveMaxPool2D,
     AdaptiveMaxPool3D,
     AvgPool1D,
     AvgPool2D,
     AvgPool3D,
     GlobalAvgPool1D,
@@ -85,50 +106,42 @@
     LPPool1D,
     LPPool2D,
     LPPool3D,
     MaxPool1D,
     MaxPool2D,
     MaxPool3D,
 )
-from .preprocessing import HistogramEqualization2D, PixelShuffle
+from .preprocessing import HistogramEqualization2D, PixelShuffle2D
 from .random_transform import RandomApply, RandomZoom2D
 from .recurrent import (
+    ConvGRU1DCell,
+    ConvGRU2DCell,
+    ConvGRU3DCell,
     ConvLSTM1DCell,
     ConvLSTM2DCell,
     ConvLSTM3DCell,
+    GRUCell,
     LSTMCell,
     ScanRNN,
-    SeparableConvLSTM1DCell,
-    SeparableConvLSTM2DCell,
-    SeparableConvLSTM3DCell,
     SimpleRNNCell,
 )
-from .resize import (
-    Repeat1D,
-    Repeat2D,
-    Repeat3D,
-    Resize1D,
-    Resize2D,
-    Resize3D,
-    Upsample1D,
-    Upsample2D,
-    Upsample3D,
-)
+from .resize import Resize1D, Resize2D, Resize3D, Upsample1D, Upsample2D, Upsample3D
 
 __all__ = (
     "blocks",
     # Fully connected
     "FNN",
-    "PFNN",
     # Linear
     "Linear",
     "Bilinear",
     "Identity",
     "Multilinear",
     "GeneralLinear",
+    "Embedding",
+    "MergeLinear",
     # Dropout
     "Dropout",
     "Dropout1D",
     "Dropout2D",
     "Dropout3D",
     # containers
     "Sequential",
@@ -151,17 +164,14 @@
     "LPPool3D",
     "AdaptiveAvgPool1D",
     "AdaptiveAvgPool2D",
     "AdaptiveAvgPool3D",
     "AdaptiveMaxPool1D",
     "AdaptiveMaxPool2D",
     "AdaptiveMaxPool3D",
-    "AdaptiveConcatPool1D",
-    "AdaptiveConcatPool2D",
-    "AdaptiveConcatPool3D",
     # Convolution
     "Conv1D",
     "Conv2D",
     "Conv3D",
     "Conv1DTranspose",
     "Conv2DTranspose",
     "Conv3DTranspose",
@@ -170,31 +180,39 @@
     "DepthwiseConv3D",
     "SeparableConv1D",
     "SeparableConv2D",
     "SeparableConv3D",
     "Conv1DLocal",
     "Conv2DLocal",
     "Conv3DLocal",
-    # "Conv1DSemiLocal",
-    # "Conv2DSemiLocal",
-    # "Conv3DSemiLocal",
-    # Flattening
-    "Flatten",
-    "Unflatten",
-    "Repeat1D",
-    "Repeat2D",
-    "Repeat3D",
+    # FFT Convolution
+    "FFTConv1D",
+    "FFTConv2D",
+    "FFTConv3D",
+    "Conv1DSemiLocal",
+    "Conv2DSemiLocal",
+    "Conv3DSemiLocal",
+    "DepthwiseFFTConv1D",
+    "DepthwiseFFTConv2D",
+    "DepthwiseFFTConv3D",
+    "FFTConv1DTranspose",
+    "FFTConv2DTranspose",
+    "FFTConv3DTranspose",
+    "SeparableFFTConv1D",
+    "SeparableFFTConv2D",
+    "SeparableFFTConv3D",
     # Normalization
     "LayerNorm",
     "InstanceNorm",
     "GroupNorm",
     # Blur
     "AvgBlur2D",
     "GaussianBlur2D",
     "Filter2D",
+    "FFTFilter2D",
     # Resize
     "Laplace2D",
     "FlipLeftRight2D",
     "FlipUpDown2D",
     "Resize1D",
     "Resize2D",
     "Resize3D",
@@ -218,15 +236,15 @@
     "RandomCrop3D",
     "RandomCutout1D",
     "RandomCutout2D",
     "RandomZoom2D",
     "RandomApply",
     # Preprocessing
     "HistogramEqualization2D",
-    "PixelShuffle",
+    "PixelShuffle2D",
     # Activations
     "AdaptiveLeakyReLU",
     "AdaptiveReLU",
     "AdaptiveSigmoid",
     "AdaptiveTanh",
     "CeLU",
     "ELU",
@@ -246,26 +264,34 @@
     "ReLU6",
     "SILU",
     "SeLU",
     "Sigmoid",
     "SoftPlus",
     "SoftShrink",
     "SoftSign",
+    "Stan",
+    "SquarePlus",
     "Swish",
     "Snake",
     "Tanh",
     "TanhShrink",
     "ThresholdedReLU",
     # Contrast
     "AdjustContrast2D",
     "RandomContrast2D",
     # RNN
     "LSTMCell",
+    "GRUCell",
     "SimpleRNNCell",
-    "ScanRNN",
     "ConvLSTM1DCell",
     "ConvLSTM2DCell",
     "ConvLSTM3DCell",
-    "SeparableConvLSTM1DCell",
-    "SeparableConvLSTM2DCell",
-    "SeparableConvLSTM3DCell",
+    "ConvGRU1DCell",
+    "ConvGRU2DCell",
+    "ConvGRU3DCell",
+    "ScanRNN",
+    # Polynomial
+    "Polynomial",
+    # Flatten
+    "Flatten",
+    "Unflatten",
 )
```

### Comparing `serket-0.0.9/serket/nn/blocks/unet.py` & `serket-0.2.0b2/serket/nn/blocks/unet.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,25 +7,23 @@
 import jax
 import jax.numpy as jnp
 import pytreeclass as pytc
 
 import serket as sk
 
 
-@pytc.treeclass
-class ResizeAndCat:
-    def __call__(self, x1: jnp.ndarray, x2: jnp.ndarray) -> jnp.ndarray:
+class ResizeAndCat(pytc.TreeClass):
+    def __call__(self, x1: jax.Array, x2: jax.Array) -> jax.Array:
         """resize a tensor to the same size as another tensor and concatenate x2 to x1 along the channel axis"""
         x1 = jax.image.resize(x1, shape=x2.shape, method="nearest")
         x1 = jnp.concatenate([x2, x1], axis=0)
         return x1
 
 
-@pytc.treeclass
-class DoubleConvBlock:
+class DoubleConvBlock(pytc.TreeClass):
     def __init__(self, in_features: int, out_features: int):
         self.conv1 = sk.nn.Conv2D(
             in_features=in_features,
             out_features=out_features,
             kernel_size=3,
             padding=1,
             bias_init_func=None,
@@ -34,41 +32,39 @@
             in_features=out_features,
             out_features=out_features,
             kernel_size=3,
             padding=1,
             bias_init_func=None,
         )
 
-    def __call__(self, x: jnp.ndarray, **kwargs) -> jnp.ndarray:
+    def __call__(self, x: jax.Array, **kwargs) -> jax.Array:
         x = self.conv1(x)
         x = jax.nn.relu(x)
         x = self.conv2(x)
         x = jax.nn.relu(x)
         return x
 
 
-@pytc.treeclass
-class UpscaleBlock:
+class UpscaleBlock(pytc.TreeClass):
     def __init__(self, in_features: int, out_features: int):
         self.conv = sk.nn.Conv2DTranspose(
             in_features=in_features, out_features=out_features, kernel_size=2, strides=2
         )
 
-    def __call__(self, x: jnp.ndarray, **kwargs) -> jnp.ndarray:
+    def __call__(self, x: jax.Array, **kwargs) -> jax.Array:
         # x = self.upscale(x)
         x = self.conv(x)
         return x
 
 
-@pytc.treeclass
-class UNetBlock:
-    in_features: int = pytc.nondiff_field()
-    out_features: int = pytc.nondiff_field()
-    blocks: int = pytc.nondiff_field()
-    init_features: int = pytc.nondiff_field()
+class UNetBlock(pytc.TreeClass):
+    in_features: int = pytc.field(callbacks=[pytc.freeze])
+    out_features: int = pytc.field(callbacks=[pytc.freeze])
+    blocks: int = pytc.field(callbacks=[pytc.freeze])
+    init_features: int = pytc.field(callbacks=[pytc.freeze])
 
     def __init__(
         self,
         in_features: int,
         out_features: int,
         blocks: int = 4,
         init_features: int = 64,
@@ -176,15 +172,15 @@
             setattr(self, f"u{i-1}_2", layer)
 
             layer = DoubleConvBlock(init_features * (2 ** (i)), init_features * (2 ** (i - 1)))  # fmt: skip
             setattr(self, f"u{i-1}_3", layer)
 
         self.f0_1 = sk.nn.Conv2D(init_features, out_features, kernel_size=1)
 
-    def __call__(self, x: jnp.ndarray) -> jnp.ndarray:
+    def __call__(self, x: jax.Array) -> jax.Array:
         result = dict()
         blocks = self.blocks
 
         # contractive path
         result["d0_1"] = self.d0_1(x)
         result["d0_2"] = self.d0_2(result["d0_1"])
```

### Comparing `serket-0.0.9/serket/nn/blocks/vgg.py` & `serket-0.2.0b2/serket/nn/blocks/vgg.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from __future__ import annotations
 
 import jax
-import jax.numpy as jnp
 import jax.random as jr
 import pytreeclass as pytc
 
 import serket as sk
 
 
-@pytc.treeclass
-class VGG16Block:
+class VGG16Block(pytc.TreeClass):
     def __init__(
-        self, in_features: int, *, pooling: str = "max", key: jr.PRNGKey = jr.PRNGKey(0)
+        self,
+        in_features: int,
+        *,
+        pooling: str = "max",
+        key: jr.KeyArray = jr.PRNGKey(0),
     ):
         """
         Args:
             in_features: number of input features
             pooling: pooling method to use. GlobalMaxPool2D(`max`) or GlobalAvgPool2D(`avg`).
 
         Note:
@@ -104,15 +106,15 @@
         self.conv_5_1 = sk.nn.Conv2D(512, 512, 3, padding="same", key=keys[10])
         self.conv_5_2 = sk.nn.Conv2D(512, 512, 3, padding="same", key=keys[11])
         self.conv_5_3 = sk.nn.Conv2D(512, 512, 3, padding="same", key=keys[12])
         self.maxpool_5 = sk.nn.MaxPool2D(2, strides=2)
 
         self.pooling = sk.nn.GlobalMaxPool2D() if pooling == "max" else sk.nn.GlobalAvgPool2D()  # fmt: skip
 
-    def __call__(self, x: jnp.ndarray, **kwargs) -> jnp.ndarray:
+    def __call__(self, x: jax.Array, **kwargs) -> jax.Array:
         x = self.conv_1_1(x)
         x = jax.nn.relu(x)
         x = self.conv_1_2(x)
         x = jax.nn.relu(x)
         x = self.maxpool_1(x)
 
         x = self.conv_2_1(x)
@@ -144,18 +146,21 @@
         x = self.conv_5_3(x)
         x = jax.nn.relu(x)
         x = self.maxpool_5(x)
         x = self.pooling(x)
         return x
 
 
-@pytc.treeclass
-class VGG19Block:
+class VGG19Block(pytc.TreeClass):
     def __init__(
-        self, in_feautres: int, *, pooling: str = "max", key: jr.PRNGKey = jr.PRNGKey(0)
+        self,
+        in_feautres: int,
+        *,
+        pooling: str = "max",
+        key: jr.KeyArray = jr.PRNGKey(0),
     ):
         """
         Args:
             in_features: number of input features
             pooling: pooling method to use. GlobalMaxPool2D(`max`) or GlobalAvgPool2D(`avg`).
 
         Note:
@@ -197,15 +202,15 @@
         self.conv_5_4 = sk.nn.Conv2D(512, 512, 3, padding="same", key=keys[15])
         self.maxpool_5 = sk.nn.MaxPool2D(2, strides=2)
 
         self.pooling = (
             sk.nn.GlobalMaxPool2D() if pooling == "max" else sk.nn.GlobalAvgPool2D()
         )
 
-    def __call__(self, x: jnp.ndarray, **kwargs) -> jnp.ndarray:
+    def __call__(self, x: jax.Array, **kwargs) -> jax.Array:
         x = self.conv_1_1(x)
         x = jax.nn.relu(x)
         x = self.conv_1_2(x)
         x = jax.nn.relu(x)
         x = self.maxpool_1(x)
 
         x = self.conv_2_1(x)
```

### Comparing `serket-0.0.9/serket/nn/blur.py` & `serket-0.2.0b2/serket/nn/blur.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,60 @@
 from __future__ import annotations
 
-import dataclasses
+# import kernex as kex
 import functools as ft
 
 import jax
 import jax.numpy as jnp
-
-# import kernex as kex
 import pytreeclass as pytc
+from jax.lax import stop_gradient
 
+from serket.nn.callbacks import (
+    positive_int_cb,
+    validate_in_features,
+    validate_spatial_in_shape,
+)
 from serket.nn.convolution import DepthwiseConv2D
-from serket.nn.utils import _TRACER_ERROR_MSG
+from serket.nn.fft_convolution import DepthwiseFFTConv2D
 
 
-@pytc.treeclass
-class AvgBlur2D:
-    in_features: int = pytc.nondiff_field()
-    kernel_size: int | tuple[int, int] = pytc.nondiff_field()
-
-    conv1: DepthwiseConv2D = pytc.nondiff_field(repr=False)
-    conv2: DepthwiseConv2D = pytc.nondiff_field(repr=False)
+class AvgBlur2D(pytc.TreeClass):
+    in_features: int = pytc.field(callbacks=[positive_int_cb])
+    kernel_size: int | tuple[int, int] = pytc.field(callbacks=[positive_int_cb])
+    conv1: DepthwiseConv2D = pytc.field(repr=False)
+    conv2: DepthwiseConv2D = pytc.field(repr=False)
 
     def __init__(self, in_features: int, kernel_size: int | tuple[int, int]):
         """Average blur 2D layer
         Args:
             in_features: number of input channels
             kernel_size: size of the convolving kernel
+
+        Example:
+        >>> import serket as sk
+        >>> import jax.numpy as jnp
+        >>> layer = sk.nn.AvgBlur2D(in_features=1, kernel_size=3)
+        >>> print(layer(jnp.ones((1,5,5))))
+        [[[0.44444448 0.6666667  0.6666667  0.6666667  0.44444448]
+          [0.6666667  1.         1.         1.         0.6666667 ]
+          [0.6666667  1.         1.         1.         0.6666667 ]
+          [0.6666667  1.         1.         1.         0.6666667 ]
+          [0.44444448 0.6666667  0.6666667  0.6666667  0.44444448]]]
+
         """
-        if in_features is None:
-            for field_item in dataclasses.fields(self):
-                setattr(self, field_item.name, None)
-
-            self._partial_init = ft.partial(
-                AvgBlur2D.__init__,
-                self,
-                kernel_size=kernel_size,
-            )
-            return
-
-        if hasattr(self, "_partial_init"):
-            delattr(self, "_partial_init")
-
-        if not isinstance(in_features, int) or in_features <= 0:
-            msg = f"`in_features` must be a positive integer, got {in_features}"
-            raise ValueError(msg)
-
-        if not isinstance(kernel_size, int) or kernel_size <= 0:
-            msg = f"`kernel_size` must be a positive integer, got {kernel_size}"
-            raise ValueError(msg)
+        self.in_features = in_features
+        self.kernel_size = kernel_size
 
         w = jnp.ones(kernel_size)
         w = w / jnp.sum(w)
         w = w[:, None]
         w = jnp.repeat(w[None, None], in_features, axis=0)
 
+        self.spatial_ndim = 2
+        self.in_features = in_features
         self.conv1 = DepthwiseConv2D(
             in_features=in_features,
             kernel_size=(kernel_size, 1),
             padding="same",
             bias_init_func=None,
         )
 
@@ -67,81 +64,67 @@
             padding="same",
             bias_init_func=None,
         )
 
         self.conv1 = self.conv1.at["weight"].set(w)
         self.conv2 = self.conv2.at["weight"].set(jnp.moveaxis(w, 2, 3))  # transpose
 
-    def __call__(self, x, **kwargs) -> jnp.ndarray:
-        if hasattr(self, "_partial_init"):
-            if isinstance(x, jax.core.Tracer):
-                raise ValueError(_TRACER_ERROR_MSG(self.__class__.__name__))
-            self._partial_init(in_features=x.shape[0])
-
-        assert x.ndim == 3, "`Input` must be 3D."
-        return self.conv2(self.conv1(x))
-
-
-@pytc.treeclass
-class GaussianBlur2D:
-    in_features: int = pytc.nondiff_field()
-    kernel_size: int = pytc.nondiff_field()
-    sigma: float = pytc.nondiff_field()
+    @ft.partial(validate_spatial_in_shape, attribute_name="spatial_ndim")
+    @ft.partial(validate_in_features, attribute_name="in_features")
+    def __call__(self, x, **k) -> jax.Array:
+        return stop_gradient(self.conv2(self.conv1(x)))
 
-    conv1: DepthwiseConv2D = pytc.nondiff_field(repr=False)
-    conv2: DepthwiseConv2D = pytc.nondiff_field(repr=False)
+
+class GaussianBlur2D(pytc.TreeClass):
+    in_features: int = pytc.field(callbacks=[positive_int_cb])
+    kernel_size: int = pytc.field(callbacks=[positive_int_cb])
+    sigma: float
+    conv1: DepthwiseConv2D
+    conv2: DepthwiseConv2D
 
     def __init__(
         self,
         in_features,
         kernel_size,
         *,
         sigma=1.0,
-        # implementation="jax",
     ):
         """Apply Gaussian blur to a channel-first image.
 
         Args:
             in_features: number of input features
             kernel_size: kernel size
             sigma: sigma. Defaults to 1.
+
+        Example:
+        >>> import serket as sk
+        >>> import jax.numpy as jnp
+        >>> layer = sk.nn.GaussianBlur2D(in_features=1, kernel_size=3)
+        >>> print(layer(jnp.ones((1,5,5))))
+        [[[0.5269764 0.7259314 0.7259314 0.7259314 0.5269764]
+          [0.7259314 1.        1.        1.        0.7259314]
+          [0.7259314 1.        1.        1.        0.7259314]
+          [0.7259314 1.        1.        1.        0.7259314]
+          [0.5269764 0.7259314 0.7259314 0.7259314 0.5269764]]]
+
         """
-        if in_features is None:
-            for field_item in dataclasses.fields(self):
-                setattr(self, field_item.name, None)
-
-            self._partial_init = ft.partial(
-                GaussianBlur2D.__init__,
-                self=self,
-                kernel_size=kernel_size,
-                sigma=sigma,
-            )
-            return
-
-        if hasattr(self, "_partial_init"):
-            delattr(self, "_partial_init")
-
-        if not isinstance(in_features, int) or in_features <= 0:
-            msg = f"Expected `in_features` to be a positive integer, got {in_features}"
-            raise ValueError(msg)
-        if not isinstance(kernel_size, int) or kernel_size <= 0:
-            msg = f"Expected `kernel_size` to be a positive integer, got {kernel_size}"
-            raise ValueError(msg)
+
+        self.in_features = in_features
+        self.kernel_size = kernel_size
 
         self.in_features = in_features
         self.kernel_size = kernel_size
         self.sigma = sigma
 
         x = jnp.linspace(-(kernel_size - 1) / 2.0, (kernel_size - 1) / 2.0, kernel_size)
         w = jnp.exp(-0.5 * jnp.square(x) * jax.lax.rsqrt(self.sigma))
 
         w = w / jnp.sum(w)
         w = w[:, None]
 
-        # if implementation == "jax":
         w = jnp.repeat(w[None, None], in_features, axis=0)
         self.conv1 = DepthwiseConv2D(
             in_features=in_features,
             kernel_size=(kernel_size, 1),
             padding="same",
             bias_init_func=None,
         )
@@ -149,88 +132,105 @@
         self.conv2 = DepthwiseConv2D(
             in_features=in_features,
             kernel_size=(1, kernel_size),
             padding="same",
             bias_init_func=None,
         )
 
+        self.in_features = in_features
+        self.spatial_ndim = 2
+
         self.conv1 = self.conv1.at["weight"].set(w)
         self.conv2 = self.conv2.at["weight"].set(jnp.moveaxis(w, 2, 3))
 
-        # elif implementation == "kernex":
-        #     # usually faster than jax for small kernel sizes
-        #     # but slower for large kernel sizes
-
-        #     @jax.vmap  # channel
-        #     @kex.kmap(kernel_size=(kernel_size, 1), padding="same")
-        #     def conv1(x):
-        #         return jnp.sum(x * w)
-
-        #     @jax.vmap
-        #     @kex.kmap(kernel_size=(1, kernel_size), padding="same")
-        #     def conv2(x):
-        #         return jnp.sum(x * w.T)
-
-        #     self._func = lambda x: conv2(conv1(x))
-
-        # else:
-        #     raise ValueError(f"Unknown implementation {implementation}")
-
-    def __call__(self, x, **kwargs) -> jnp.ndarray:
-        if hasattr(self, "_partial_init"):
-            if isinstance(x, jax.core.Tracer):
-                raise ValueError(_TRACER_ERROR_MSG(self.__class__.__name__))
-            self._partial_init(in_features=x.shape[0])
-
-        assert x.ndim == 3, "`Input` must be 3D."
-        return self.conv1(self.conv2(x))
-
-
-@pytc.treeclass
-class Filter2D:
-    in_features: int = pytc.nondiff_field()
-    conv: DepthwiseConv2D = pytc.nondiff_field(repr=False)
-    kernel: jnp.ndarray = pytc.nondiff_field()
+    def __call__(self, x, **k) -> jax.Array:
+        return stop_gradient(self.conv1(self.conv2(x)))
+
+
+class Filter2D(pytc.TreeClass):
+    in_features: int = pytc.field(callbacks=[positive_int_cb])
+    conv: DepthwiseConv2D
+    kernel: jax.Array
 
-    def __init__(self, in_features: int, kernel: jnp.ndarray):
+    def __init__(self, in_features: int, kernel: jax.Array):
         """Apply 2D filter for each channel
         Args:
             in_features: number of input channels
             kernel: kernel array
+
+        Example:
+        >>> import serket as sk
+        >>> import jax.numpy as jnp
+        >>> layer = sk.nn.Filter2D(in_features=1, kernel=jnp.ones((3,3)))
+        >>> print(layer(jnp.ones((1,5,5))))
+        [[[4. 6. 6. 6. 4.]
+          [6. 9. 9. 9. 6.]
+          [6. 9. 9. 9. 6.]
+          [6. 9. 9. 9. 6.]
+          [4. 6. 6. 6. 4.]]]
+
         """
-        if in_features is None:
-            for field_item in dataclasses.fields(self):
-                setattr(self, field_item.name, None)
+        if not isinstance(kernel, jax.Array) or kernel.ndim != 2:
+            raise ValueError("Expected `kernel` to be a 2D `ndarray` with shape (H, W)")
 
-            self._partial_init = ft.partial(Filter2D.__init__, self=self, kernel=kernel)
-            return
+        self.in_features = in_features
+        self.spatial_ndim = 2
+        self.kernel = jnp.stack([kernel] * in_features, axis=0)
+        self.kernel = self.kernel[:, None]
 
-        if hasattr(self, "_partial_init"):
-            delattr(self, "_partial_init")
+        self.conv = DepthwiseConv2D(
+            in_features=in_features,
+            kernel_size=kernel.shape,
+            padding="same",
+            bias_init_func=None,
+        )
+        self.conv = self.conv.at["weight"].set(self.kernel)
 
-        if not isinstance(in_features, int) or in_features <= 0:
-            msg = f"Expected `in_features` to be a positive integer, got {in_features}"
-            raise ValueError(msg)
+    @ft.partial(validate_spatial_in_shape, attribute_name="spatial_ndim")
+    @ft.partial(validate_in_features, attribute_name="in_features")
+    def __call__(self, x, **k) -> jax.Array:
+        return stop_gradient(self.conv(x))
 
-        if not isinstance(kernel, jnp.ndarray) or kernel.ndim != 2:
+
+class FFTFilter2D(pytc.TreeClass):
+    in_features: int = pytc.field(callbacks=[positive_int_cb])
+    kernel: jax.Array
+    conv: DepthwiseFFTConv2D
+
+    def __init__(self, in_features: int, kernel: jax.Array):
+        """Apply 2D filter for each channel using FFT
+        Args:
+            in_features: number of input channels
+            kernel: kernel array
+
+        Example:
+        >>> import serket as sk
+        >>> import jax.numpy as jnp
+        >>> layer = sk.nn.FFTFilter2D(in_features=1, kernel=jnp.ones((3,3)))
+        >>> print(layer(jnp.ones((1,5,5))))
+        [[[4.0000005 6.0000005 6.000001  6.0000005 4.0000005]
+          [6.0000005 9.        9.        9.        6.0000005]
+          [6.0000005 9.        9.        9.        6.0000005]
+          [6.0000005 9.        9.        9.        6.0000005]
+          [4.        6.0000005 6.0000005 6.0000005 4.       ]]]
+        """
+
+        if not isinstance(kernel, jax.Array) or kernel.ndim != 2:
             raise ValueError("Expected `kernel` to be a 2D `ndarray` with shape (H, W)")
 
         self.in_features = in_features
+        self.spatial_ndim = 2
         self.kernel = jnp.stack([kernel] * in_features, axis=0)
         self.kernel = self.kernel[:, None]
 
-        self.conv = DepthwiseConv2D(
+        self.conv = DepthwiseFFTConv2D(
             in_features=in_features,
             kernel_size=kernel.shape,
             padding="same",
             bias_init_func=None,
         )
         self.conv = self.conv.at["weight"].set(self.kernel)
 
-    def __call__(self, x, **kwargs) -> jnp.ndarray:
-        if hasattr(self, "_partial_init"):
-            if isinstance(x, jax.core.Tracer):
-                raise ValueError(_TRACER_ERROR_MSG(self.__class__.__name__))
-            self._partial_init(in_features=x.shape[0])
-
-        assert x.ndim == 3, "`Input` must be 3D."
-        return self.conv(x)
+    @ft.partial(validate_spatial_in_shape, attribute_name="spatial_ndim")
+    @ft.partial(validate_in_features, attribute_name="in_features")
+    def __call__(self, x, **k) -> jax.Array:
+        return stop_gradient(self.conv(x))
```

### Comparing `serket-0.0.9/serket/nn/convolution.py` & `serket-0.2.0b2/serket/nn/fft_convolution.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,752 +1,906 @@
-# this script defines different convolutional layers
-# https://arxiv.org/pdf/1603.07285.pdf
-# Throughout the code, we use OIHW  as the default data format for kernels. and NCHW for data.
+# references
+# https://github.com/fkodom/fft-conv-pytorch/blob/master/fft_conv_pytorch/fft_conv.py
+# https://stackoverflow.com/questions/47272699/need-tensorflow-keras-equivalent-for-scipy-signal-fftconvolve
 
 from __future__ import annotations
 
-import dataclasses
 import functools as ft
-import operator as op
-from typing import Callable
 
 import jax
 import jax.numpy as jnp
 import jax.random as jr
 import pytreeclass as pytc
-from jax.lax import ConvDimensionNumbers
 
+from serket.nn.callbacks import (
+    init_func_cb,
+    positive_int_cb,
+    validate_in_features,
+    validate_spatial_in_shape,
+)
 from serket.nn.utils import (
-    _TRACER_ERROR_MSG,
-    _calculate_convolution_output_shape,
-    _calculate_transpose_padding,
-    _check_and_return_init_func,
-    _check_and_return_input_dilation,
-    _check_and_return_input_size,
-    _check_and_return_kernel,
-    _check_and_return_kernel_dilation,
-    _check_and_return_padding,
-    _check_and_return_strides,
+    DilationType,
+    InitFuncType,
+    KernelSizeType,
+    PaddingType,
+    StridesType,
+    calculate_transpose_padding,
+    canonicalize,
+    delayed_canonicalize_padding,
 )
 
-# ------------------------------ Convolutional Layers ------------------------------ #
-
 
-@pytc.treeclass
-class ConvND:
-    weight: jnp.ndarray
-    bias: jnp.ndarray
-
-    in_features: int = pytc.nondiff_field()
-    out_features: int = pytc.nondiff_field()
-    kernel_size: int | tuple[int, ...] = pytc.nondiff_field()
-    strides: int | tuple[int, ...] = pytc.nondiff_field()
-    padding: str | int | tuple[int, ...] | tuple[tuple[int, int], ...] = pytc.nondiff_field()  # fmt: skip
-    input_dilation: int | tuple[int, ...] = pytc.nondiff_field()
-    kernel_dilation: int | tuple[int, ...] = pytc.nondiff_field()
-    weight_init_func: str | Callable[[jr.PRNGKey, tuple[int, ...]], jnp.ndarray]
-    bias_init_func: str | Callable[[jr.PRNGKey, tuple[int]], jnp.ndarray]
-    groups: int = pytc.nondiff_field()
+@jax.jit
+def _ungrouped_matmul(x, y) -> jax.Array:
+    alpha = "abcdefghijklmnopqrstuvwx"
+    lhs = "y" + alpha[: x.ndim - 1]
+    rhs = "z" + alpha[: y.ndim - 1]
+    out = "yz" + lhs[2:]
+    return jnp.einsum(f"{lhs},{rhs}->{out}", x, y)
+
+
+@ft.partial(jax.jit, static_argnums=(2,))
+def _grouped_matmul(x, y, groups) -> jax.Array:
+    b, c, *s = x.shape  # batch, channels, spatial
+    o, i, *k = y.shape  # out_channels, in_channels, kernel
+    x = x.reshape(groups, b, c // groups, *s)  # groups, batch, channels, spatial
+    y = y.reshape(groups, o // groups, *(i, *k))
+    z = jax.vmap(_ungrouped_matmul, in_axes=(0, 0), out_axes=1)(x, y)
+    return z.reshape(z.shape[0], z.shape[1] * z.shape[2], *z.shape[3:])
+
+
+def grouped_matmul(x, y, groups: int = 1):
+    return _ungrouped_matmul(x, y) if groups == 1 else _grouped_matmul(x, y, groups)
+
+
+@ft.partial(jax.jit, static_argnums=(1, 2))
+def _intersperse_along_axis(x: jax.Array, dilation: int, axis: int) -> jax.Array:
+    shape = list(x.shape)
+    shape[axis] = (dilation) * shape[axis] - (dilation - 1)
+    z = jnp.zeros(shape)
+    z = z.at[(slice(None),) * axis + (slice(None, None, (dilation)),)].set(x)
+    return z
+
+
+@ft.partial(jax.jit, static_argnums=(1, 2))
+def _general_intersperse(
+    x: jax.Array,
+    dilation: tuple[int, ...],
+    axis: tuple[int, ...],
+) -> jax.Array:
+    for di, ai in zip(dilation, axis):
+        x = _intersperse_along_axis(x, di, ai) if di > 1 else x
+    return x
+
+
+@ft.partial(jax.jit, static_argnums=(1,))
+def _general_pad(x: jax.Array, pad_width: tuple[tuple[int, int], ...]) -> jax.Array:
+    """Pad the input with `pad_width` on each side. Negative value will lead to cropping.
+    Example:
+        >>> _general_pad(jnp.ones([3,3]),((0,0),(-1,1)))
+        [[1., 1., 0.],
+        [1., 1., 0.],
+        [1., 1., 0.]]
+    """
+
+    for axis, (lhs, rhs) in enumerate(pad_width := list(pad_width)):
+        if lhs < 0 and rhs < 0:
+            x = jax.lax.dynamic_slice_in_dim(x, -lhs, x.shape[axis] + lhs + rhs, axis)
+        elif lhs < 0:
+            x = jax.lax.dynamic_slice_in_dim(x, -lhs, x.shape[axis] + lhs, axis)
+        elif rhs < 0:
+            x = jax.lax.dynamic_slice_in_dim(x, 0, x.shape[axis] + rhs, axis)
+
+    return jnp.pad(x, [(max(lhs, 0), max(rhs, 0)) for (lhs, rhs) in (pad_width)])
+
+
+@ft.partial(jax.jit, static_argnums=(2, 3, 4, 5))
+def fft_conv_general_dilated(
+    x: jax.Array,
+    w: jax.Array,
+    strides: tuple[int, ...],
+    padding: tuple[tuple[int, int], ...],
+    groups: int,
+    dilation: tuple[int, ...],
+) -> jax.Array:
+    """General dilated convolution using FFT
+    Args:
+        x: input array in shape (batch, in_features, *spatial_in_shape)
+        w: kernel array in shape of (out_features, in_features // groups, *kernel_size)
+        strides: strides in form of tuple of ints for each spatial dimension
+        padding: padding in the form of ((before_1, after_1), ..., (before_N, after_N)) for each spatial dimension
+        groups: number of groups
+        dilation: dilation in the form of tuple of ints for each spatial dimension
+    """
+
+    spatial_ndim = x.ndim - 2  # spatial dimensions
+    w = _general_intersperse(w, dilation=dilation, axis=range(2, 2 + spatial_ndim))
+    x = _general_pad(x, ((0, 0), (0, 0), *padding))
+
+    x_shape, w_shape = x.shape, w.shape
+
+    if x.shape[-1] % 2 != 0:
+        x = jnp.pad(x, tuple([(0, 0)] * (x.ndim - 1) + [(0, 1)]))
+
+    kernel_padding = ((0, x.shape[i] - w.shape[i]) for i in range(2, spatial_ndim + 2))
+    w = _general_pad(w, ((0, 0), (0, 0), *kernel_padding))
+
+    # for real-valued input
+    x_fft = jnp.fft.rfftn(x, axes=range(2, spatial_ndim + 2))
+    w_fft = jnp.conjugate(jnp.fft.rfftn(w, axes=range(2, spatial_ndim + 2)))
+    z_fft = grouped_matmul(x_fft, w_fft, groups)
+
+    z = jnp.fft.irfftn(z_fft, axes=range(2, spatial_ndim + 2))
+
+    start = (0,) * (spatial_ndim + 2)
+    end = (z.shape[0], z.shape[1])
+    end += tuple(max((x_shape[i] - w_shape[i] + 1), 0) for i in range(2, spatial_ndim + 2))  # fmt: skip
+
+    if all(s == 1 for s in strides):
+        return jax.lax.dynamic_slice(z, start, end)
+
+    return jax.lax.slice(z, start, end, (1, 1, *strides))
+
+
+class FFTConvND(pytc.TreeClass):
+    weight: jax.Array
+    bias: jax.Array
+
+    in_features: int = pytc.field(callbacks=[positive_int_cb])
+    out_features: int = pytc.field(callbacks=[positive_int_cb])
+    kernel_size: KernelSizeType
+    strides: StridesType
+    padding: PaddingType
+    kernel_dilation: DilationType
+    weight_init_func: InitFuncType = pytc.field(callbacks=[init_func_cb])
+    bias_init_func: InitFuncType = pytc.field(callbacks=[init_func_cb])
+    groups: int = pytc.field(callbacks=[positive_int_cb])
 
     def __init__(
         self,
         in_features: int,
         out_features: int,
-        kernel_size: int | tuple[int, ...],
+        kernel_size: KernelSizeType,
         *,
-        strides: int | tuple[int, ...] = 1,
-        padding: str | int | tuple[int, ...] | tuple[tuple[int, int], ...] = "SAME",
-        input_dilation: int | tuple[int, ...] = 1,
-        kernel_dilation: int | tuple[int, ...] = 1,
-        weight_init_func: str | Callable = "glorot_uniform",
-        bias_init_func: str | Callable = "zeros",
+        strides: StridesType = 1,
+        padding: PaddingType = "SAME",
+        kernel_dilation: DilationType = 1,
+        weight_init_func: InitFuncType = "glorot_uniform",
+        bias_init_func: InitFuncType = "zeros",
         groups: int = 1,
-        ndim: int = 2,
-        key: jr.PRNGKey = jr.PRNGKey(0),
+        key: jr.KeyArray = jr.PRNGKey(0),
+        spatial_ndim: int = 2,
     ):
-        """Convolutional layer.
+        """FFT Convolutional layer.
 
         Args:
             in_features: number of input features
             out_features: number of output features
             kernel_size: size of the convolutional kernel
             strides: stride of the convolution
             padding: padding of the input
-            input_dilation: dilation of the input
-            kernel_dilation: dilation of the convolutional kernel
+            kernel_dilation: dilation of the kernel
             weight_init_func: function to use for initializing the weights
             bias_init_func: function to use for initializing the bias
             groups: number of groups to use for grouped convolution
-            ndim: number of dimensions of the convolution
+            spatial_ndim: number of dimensions of the convolution
             key: key to use for initializing the weights
 
-        See: https://jax.readthedocs.io/en/latest/_autosummary/jax.lax.conv.html
+        See:
+            https://jax.readthedocs.io/en/latest/_autosummary/jax.lax.conv.html
+            The implementation is tested against https://github.com/fkodom/fft-conv-pytorch
         """
-        if in_features is None:
-            for field_item in dataclasses.fields(self):
-                # set all fields to None to mark the class as uninitialized
-                # to the user and to avoid errors
-                setattr(self, field_item.name, None)
-
-            self._partial_init = ft.partial(
-                ConvND.__init__,
-                self=self,
-                out_features=out_features,
-                kernel_size=kernel_size,
-                strides=strides,
-                padding=padding,
-                input_dilation=input_dilation,
-                kernel_dilation=kernel_dilation,
-                weight_init_func=weight_init_func,
-                bias_init_func=bias_init_func,
-                groups=groups,
-                ndim=ndim,
-                key=key,
-            )
-
-            return
-
-        if hasattr(self, "_partial_init"):
-            delattr(self, "_partial_init")
-
-        if not isinstance(in_features, int) or in_features <= 0:
-            raise ValueError(
-                f"Expected `in_features` to be a positive integer, got {in_features}"
-            )
-
-        if not isinstance(out_features, int) or out_features <= 0:
-            raise ValueError(
-                f"Expected `out_features` to be a positive integer, got {out_features}"
-            )
-
-        if not isinstance(groups, int) or groups <= 0:
-            raise ValueError(f"Expected groups to be a positive integer, got {groups}")
-
-        assert (
-            out_features % groups == 0
-        ), f"Expected out_features % groups == 0, got {out_features % groups}"
-
+        # already checked in callbacks
         self.in_features = in_features
+        self.weight_init_func = weight_init_func
+        self.bias_init_func = bias_init_func
         self.out_features = out_features
         self.groups = groups
+        self.spatial_ndim = spatial_ndim
 
-        self.kernel_size = _check_and_return_kernel(kernel_size, ndim)
-        self.strides = _check_and_return_strides(strides, ndim)
-        self.input_dilation = _check_and_return_input_dilation(input_dilation, ndim)
-        self.kernel_dilation = _check_and_return_kernel_dilation(kernel_dilation, ndim)
-        self.padding = _check_and_return_padding(padding, self.kernel_size)
-        self.weight_init_func = _check_and_return_init_func(weight_init_func, "weight_init_func")  # fmt: skip
-        self.bias_init_func = _check_and_return_init_func(bias_init_func, "bias_init_func")  # fmt: skip
+        # needs more info to be checked
+        self.kernel_size = canonicalize(kernel_size, spatial_ndim, name="kernel_size")
+        self.strides = canonicalize(strides, spatial_ndim, name="strides")
+        self.padding = padding
+        self.kernel_dilation = canonicalize(kernel_dilation, spatial_ndim, name="kernel_dilation")  # fmt: skip
+
+        if self.out_features % self.groups != 0:
+            msg = f"Expected out_features % groups == 0, got {self.out_features % self.groups}"
+            raise ValueError(msg)
 
         weight_shape = (out_features, in_features // groups, *self.kernel_size)
         self.weight = self.weight_init_func(key, weight_shape)
 
         if bias_init_func is None:
             self.bias = None
         else:
-            bias_shape = (out_features, *(1,) * ndim)
+            bias_shape = (out_features, *(1,) * spatial_ndim)
             self.bias = self.bias_init_func(key, bias_shape)
 
-        self.dimension_numbers = ConvDimensionNumbers(*((tuple(range(ndim + 2)),) * 3))
-
-    def __call__(self, x: jnp.ndarray, **kwargs) -> jnp.ndarray:
-        if hasattr(self, "_partial_init"):
-            if isinstance(x, jax.core.Tracer):
-                raise ValueError(_TRACER_ERROR_MSG(self.__class__.__name__))
-            self._partial_init(in_features=x.shape[0])
-
-        y = jax.lax.conv_general_dilated(
-            lhs=jnp.expand_dims(x, 0),
-            rhs=self.weight,
-            window_strides=self.strides,
+    @ft.partial(validate_spatial_in_shape, attribute_name="spatial_ndim")
+    @ft.partial(validate_in_features, attribute_name="in_features")
+    def __call__(self, x: jax.Array, **k) -> jax.Array:
+        padding = delayed_canonicalize_padding(
+            in_dim=x.shape[1:],
             padding=self.padding,
-            lhs_dilation=self.input_dilation,
-            rhs_dilation=self.kernel_dilation,
-            dimension_numbers=self.dimension_numbers,
-            feature_group_count=self.groups,
+            kernel_size=self.kernel_size,
+            strides=self.strides,
         )
 
+        y = fft_conv_general_dilated(
+            jnp.expand_dims(x, axis=0),
+            self.weight,
+            strides=self.strides,
+            padding=padding,
+            groups=self.groups,
+            dilation=self.kernel_dilation,
+        )
+        y = jnp.squeeze(y, axis=0)
         if self.bias is None:
-            return y[0]
-        return (y + self.bias)[0]
+            return y
+        return y + self.bias
 
 
-@pytc.treeclass
-class Conv1D(ConvND):
+class FFTConv1D(FFTConvND):
     def __init__(
         self,
         in_features: int,
         out_features: int,
-        kernel_size: int | tuple[int, ...],
+        kernel_size: KernelSizeType,
         *,
-        strides: int | tuple[int, ...] = 1,
-        padding: str | int | tuple[int, ...] | tuple[tuple[int, int], ...] = "SAME",
-        input_dilation: int | tuple[int, ...] = 1,
-        kernel_dilation: int | tuple[int, ...] = 1,
-        weight_init_func: str | Callable = "glorot_uniform",
-        bias_init_func: str | Callable = "zeros",
+        strides: StridesType = 1,
+        padding: PaddingType = "SAME",
+        kernel_dilation: DilationType = 1,
+        weight_init_func: InitFuncType = "glorot_uniform",
+        bias_init_func: InitFuncType = "zeros",
         groups: int = 1,
-        key: jr.PRNGKey = jr.PRNGKey(0),
+        key: jr.KeyArray = jr.PRNGKey(0),
     ):
+        """1D FFT Convolutional layer.
+
+        Args:
+            in_features: number of input features
+            out_features: number of output features
+            kernel_size: size of the convolutional kernel
+            strides: stride of the convolution
+            padding: padding of the input
+            kernel_dilation: dilation of the kernel
+            weight_init_func: function to use for initializing the weights
+            bias_init_func: function to use for initializing the bias
+            groups: number of groups to use for grouped convolution
+            spatial_ndim: number of dimensions of the convolution
+            key: key to use for initializing the weights
+
+        See:
+            https://jax.readthedocs.io/en/latest/_autosummary/jax.lax.conv.html
+            The implementation is tested against https://github.com/fkodom/fft-conv-pytorch
+        """
         super().__init__(
             in_features=in_features,
             out_features=out_features,
             kernel_size=kernel_size,
             strides=strides,
             padding=padding,
-            input_dilation=input_dilation,
             kernel_dilation=kernel_dilation,
             weight_init_func=weight_init_func,
             bias_init_func=bias_init_func,
             groups=groups,
-            ndim=1,
             key=key,
+            spatial_ndim=1,
         )
 
 
-@pytc.treeclass
-class Conv2D(ConvND):
+class FFTConv2D(FFTConvND):
     def __init__(
         self,
         in_features: int,
         out_features: int,
-        kernel_size: int | tuple[int, ...],
+        kernel_size: KernelSizeType,
         *,
-        strides: int | tuple[int, ...] = 1,
-        padding: str | int | tuple[int, ...] | tuple[tuple[int, int], ...] = "SAME",
-        input_dilation: int | tuple[int, ...] = 1,
-        kernel_dilation: int | tuple[int, ...] = 1,
-        weight_init_func: str | Callable = "glorot_uniform",
-        bias_init_func: str | Callable = "zeros",
+        strides: StridesType = 1,
+        padding: PaddingType = "SAME",
+        kernel_dilation: DilationType = 1,
+        weight_init_func: InitFuncType = "glorot_uniform",
+        bias_init_func: InitFuncType = "zeros",
         groups: int = 1,
-        key: jr.PRNGKey = jr.PRNGKey(0),
+        key: jr.KeyArray = jr.PRNGKey(0),
     ):
+        """2D FFT Convolutional layer.
+
+        Args:
+            in_features: number of input features
+            out_features: number of output features
+            kernel_size: size of the convolutional kernel
+            strides: stride of the convolution
+            padding: padding of the input
+            kernel_dilation: dilation of the kernel
+            weight_init_func: function to use for initializing the weights
+            bias_init_func: function to use for initializing the bias
+            groups: number of groups to use for grouped convolution
+            spatial_ndim: number of dimensions of the convolution
+            key: key to use for initializing the weights
+
+        See:
+            https://jax.readthedocs.io/en/latest/_autosummary/jax.lax.conv.html
+            The implementation is tested against https://github.com/fkodom/fft-conv-pytorch
+        """
         super().__init__(
             in_features=in_features,
             out_features=out_features,
             kernel_size=kernel_size,
             strides=strides,
             padding=padding,
-            input_dilation=input_dilation,
             kernel_dilation=kernel_dilation,
             weight_init_func=weight_init_func,
             bias_init_func=bias_init_func,
             groups=groups,
-            ndim=2,
             key=key,
+            spatial_ndim=2,
         )
 
 
-@pytc.treeclass
-class Conv3D(ConvND):
+class FFTConv3D(FFTConvND):
     def __init__(
         self,
         in_features: int,
         out_features: int,
-        kernel_size: int | tuple[int, ...],
+        kernel_size: KernelSizeType,
         *,
-        strides: int | tuple[int, ...] = 1,
-        padding: str | int | tuple[int, ...] | tuple[tuple[int, int], ...] = "SAME",
-        input_dilation: int | tuple[int, ...] = 1,
-        kernel_dilation: int | tuple[int, ...] = 1,
-        weight_init_func: str | Callable = "glorot_uniform",
-        bias_init_func: str | Callable = "zeros",
+        strides: StridesType = 1,
+        padding: PaddingType = "SAME",
+        kernel_dilation: DilationType = 1,
+        weight_init_func: InitFuncType = "glorot_uniform",
+        bias_init_func: InitFuncType = "zeros",
         groups: int = 1,
-        key: jr.PRNGKey = jr.PRNGKey(0),
+        key: jr.KeyArray = jr.PRNGKey(0),
     ):
+        """3D FFT Convolutional layer.
+
+        Args:
+            in_features: number of input features
+            out_features: number of output features
+            kernel_size: size of the convolutional kernel
+            strides: stride of the convolution
+            padding: padding of the input
+            kernel_dilation: dilation of the kernel
+            weight_init_func: function to use for initializing the weights
+            bias_init_func: function to use for initializing the bias
+            groups: number of groups to use for grouped convolution
+            spatial_ndim: number of dimensions of the convolution
+            key: key to use for initializing the weights
+
+        See:
+            https://jax.readthedocs.io/en/latest/_autosummary/jax.lax.conv.html
+            The implementation is tested against https://github.com/fkodom/fft-conv-pytorch
+        """
         super().__init__(
             in_features=in_features,
             out_features=out_features,
             kernel_size=kernel_size,
             strides=strides,
             padding=padding,
-            input_dilation=input_dilation,
             kernel_dilation=kernel_dilation,
             weight_init_func=weight_init_func,
             bias_init_func=bias_init_func,
             groups=groups,
-            ndim=3,
             key=key,
+            spatial_ndim=3,
         )
 
 
-# ------------------------------ Transposed Convolutional Layers ------------------------------ #
+# ----------------------------------------------------------------------------------------------------------------------#
+
 
+class FFTConvNDTranspose(pytc.TreeClass):
+    weight: jax.Array
+    bias: jax.Array
 
-@pytc.treeclass
-class ConvNDTranspose:
-    weight: jnp.ndarray
-    bias: jnp.ndarray
-
-    in_features: int = pytc.nondiff_field()
-    out_features: int = pytc.nondiff_field()
-    kernel_size: int | tuple[int, ...] = pytc.nondiff_field()
-    padding: str | int | tuple[int, ...] | tuple[tuple[int, int], ...] = pytc.nondiff_field()  # fmt: skip
-    output_padding: int | tuple[int, ...] = pytc.nondiff_field()
-    strides: int | tuple[int, ...] = pytc.nondiff_field()
-    kernel_dilation: int | tuple[int, ...] = pytc.nondiff_field()
-    weight_init_func: str | Callable[[jr.PRNGKey, tuple[int, ...]], jnp.ndarray]
-    bias_init_func: Callable[[jr.PRNGKey, tuple[int]], jnp.ndarray]
-    groups: int = pytc.nondiff_field()
+    in_features: int = pytc.field(callbacks=[positive_int_cb])
+    out_features: int = pytc.field(callbacks=[positive_int_cb])
+    kernel_size: KernelSizeType
+    padding: PaddingType
+    output_padding: int | tuple[int, ...]
+    strides: StridesType
+    kernel_dilation: DilationType
+    weight_init_func: InitFuncType = pytc.field(callbacks=[init_func_cb])
+    bias_init_func: InitFuncType = pytc.field(callbacks=[init_func_cb])
+    groups: int
 
     def __init__(
         self,
         in_features: int,
         out_features: int,
-        kernel_size: int | tuple[int, ...],
+        kernel_size: KernelSizeType,
         *,
-        strides: int | tuple[int, ...] = 1,
-        padding: str | int | tuple[int, ...] | tuple[tuple[int, int], ...] = "SAME",
+        strides: StridesType = 1,
+        padding: PaddingType = "SAME",
         output_padding: int = 0,
-        kernel_dilation: int | tuple[int, ...] = 1,
-        weight_init_func: str | Callable = "glorot_uniform",
-        bias_init_func: str | Callable = "zeros",
+        kernel_dilation: DilationType = 1,
+        weight_init_func: InitFuncType = "glorot_uniform",
+        bias_init_func: InitFuncType = "zeros",
         groups: int = 1,
-        ndim: int = 2,
-        key: jr.PRNGKey = jr.PRNGKey(0),
+        key: jr.KeyArray = jr.PRNGKey(0),
+        spatial_ndim: int = 2,
     ):
         """Convolutional Transpose Layer
 
         Args:
             in_features : Number of input channels
             out_features : Number of output channels
             kernel_size : Size of the convolutional kernel
             strides : Stride of the convolution
             padding : Padding of the input
             output_padding : Additional size added to one side of the output shape
-            kernel_dilation : Dilation of the convolutional kernel
+            kernel_dilation : Dilation of the kernel
             weight_init_func : Weight initialization function
             bias_init_func : Bias initialization function
             groups : Number of groups
-            ndim : Number of dimensions
+            spatial_ndim : Number of dimensions
             key : PRNG key
         """
-        if in_features is None:
-            for field_item in dataclasses.fields(self):
-                # set all fields to None to mark the class as uninitialized
-                # to the user and to avoid errors
-                setattr(self, field_item.name, None)
-            self._partial_init = ft.partial(
-                ConvNDTranspose.__init__,
-                self=self,
-                out_features=out_features,
-                kernel_size=kernel_size,
-                strides=strides,
-                padding=padding,
-                output_padding=output_padding,
-                kernel_dilation=kernel_dilation,
-                weight_init_func=weight_init_func,
-                bias_init_func=bias_init_func,
-                groups=groups,
-                ndim=ndim,
-                key=key,
-            )
-            return
-
-        if hasattr(self, "_partial_init"):
-            delattr(self, "_partial_init")
-
-        if not isinstance(in_features, int) or in_features <= 0:
-            raise ValueError(
-                f"Expected in_features to be a positive integer, got {in_features}"
-            )
-
-        if not isinstance(out_features, int) or out_features <= 0:
-            raise ValueError(
-                f"Expected out_features to be a positive integer, got {out_features}"
-            )
-
-        if not isinstance(groups, int) or groups <= 0:
-            raise ValueError(f"Expected groups to be a positive integer, got {groups}")
-
-        assert (
-            out_features % groups == 0
-        ), f"Expected out_features % groups == 0, got {out_features % groups}"
 
+        # already checked in callbacks
         self.in_features = in_features
         self.out_features = out_features
         self.groups = groups
-
-        self.kernel_size = _check_and_return_kernel(kernel_size, ndim)
-        self.strides = _check_and_return_strides(strides, ndim)
-        self.kernel_dilation = _check_and_return_kernel_dilation(kernel_dilation, ndim)
-        self.padding = _check_and_return_padding(padding, self.kernel_size)
-        self.output_padding = _check_and_return_strides(output_padding, ndim)
-        self.weight_init_func = _check_and_return_init_func(weight_init_func, "weight_init_func")  # fmt: skip
-        self.bias_init_func = _check_and_return_init_func(bias_init_func, "bias_init_func")  # fmt: skip
+        self.spatial_ndim = spatial_ndim
+        self.weight_init_func = weight_init_func
+        self.bias_init_func = bias_init_func
+
+        # needs more info to be checked
+        self.kernel_size = canonicalize(kernel_size, spatial_ndim, name="kernel_size")
+        self.strides = canonicalize(strides, spatial_ndim, name="strides")
+        self.kernel_dilation = canonicalize(kernel_dilation, spatial_ndim, name="kernel_dilation")  # fmt: skip
+        self.padding = padding
+        self.output_padding = canonicalize(output_padding, spatial_ndim, name="output_padding")  # fmt: skip
+
+        if self.in_features % self.groups != 0:
+            msg = f"Expected in_features % groups == 0, got {self.in_features % self.groups}"
+            raise ValueError(msg)
 
         weight_shape = (out_features, in_features // groups, *self.kernel_size)  # OIHW
         self.weight = self.weight_init_func(key, weight_shape)
 
         if bias_init_func is None:
             self.bias = None
         else:
-            bias_shape = (out_features, *(1,) * ndim)
+            bias_shape = (out_features, *(1,) * spatial_ndim)
             self.bias = self.bias_init_func(key, bias_shape)
 
-        self.dimension_numbers = ConvDimensionNumbers(*((tuple(range(ndim + 2)),) * 3))
-
-        self.transposed_padding = _calculate_transpose_padding(
+    @ft.partial(validate_spatial_in_shape, attribute_name="spatial_ndim")
+    @ft.partial(validate_in_features, attribute_name="in_features")
+    def __call__(self, x: jax.Array, **k) -> jax.Array:
+        padding = delayed_canonicalize_padding(
+            in_dim=x.shape[1:],
             padding=self.padding,
+            kernel_size=self.kernel_size,
+            strides=self.strides,
+        )
+
+        transposed_padding = calculate_transpose_padding(
+            padding=padding,
             extra_padding=self.output_padding,
             kernel_size=self.kernel_size,
             input_dilation=self.kernel_dilation,
         )
 
-    def __call__(self, x: jnp.ndarray, **kwargs) -> jnp.ndarray:
-        if hasattr(self, "_partial_init"):
-            if isinstance(x, jax.core.Tracer):
-                raise ValueError(_TRACER_ERROR_MSG(self.__class__.__name__))
-            self._partial_init(in_features=x.shape[0])
-
-        y = jax.lax.conv_transpose(
-            lhs=jnp.expand_dims(x, 0),
-            rhs=self.weight,
+        y = fft_conv_general_dilated(
+            jnp.expand_dims(x, axis=0),
+            self.weight,
             strides=self.strides,
-            padding=self.transposed_padding,
-            rhs_dilation=self.kernel_dilation,
-            dimension_numbers=self.dimension_numbers,
+            padding=transposed_padding,
+            groups=self.groups,
+            dilation=self.kernel_dilation,
         )
 
+        y = jnp.squeeze(y, axis=0)
+
         if self.bias is None:
-            return y[0]
-        return (y + self.bias)[0]
+            return y
+        return y + self.bias
 
 
-@pytc.treeclass
-class Conv1DTranspose(ConvNDTranspose):
+class FFTConv1DTranspose(FFTConvNDTranspose):
     def __init__(
         self,
         in_features: int,
         out_features: int,
-        kernel_size: int | tuple[int, ...],
+        kernel_size: KernelSizeType,
         *,
-        strides: int | tuple[int, ...] = 1,
-        padding: str | int | tuple[int, ...] | tuple[tuple[int, int], ...] = "SAME",
+        strides: StridesType = 1,
+        padding: PaddingType = "SAME",
         output_padding: int = 0,
-        kernel_dilation: int | tuple[int, ...] = 1,
-        weight_init_func: str | Callable = "glorot_uniform",
-        bias_init_func: str | Callable = "zeros",
+        kernel_dilation: DilationType = 1,
+        weight_init_func: InitFuncType = "glorot_uniform",
+        bias_init_func: InitFuncType = "zeros",
         groups: int = 1,
-        key: jr.PRNGKey = jr.PRNGKey(0),
+        key: jr.KeyArray = jr.PRNGKey(0),
     ):
+        """1D FFT Convolutional Transpose Layer.
+
+        Args:
+            in_features : Number of input channels
+            out_features : Number of output channels
+            kernel_size : Size of the convolutional kernel
+            strides : Stride of the convolution
+            padding : Padding of the input
+            output_padding : Additional size added to one side of the output shape
+            kernel_dilation : Dilation of the kernel
+            weight_init_func : Weight initialization function
+            bias_init_func : Bias initialization function
+            groups : Number of groups
+            spatial_ndim : Number of dimensions
+            key : PRNG key
+        """
         super().__init__(
-            in_features,
-            out_features,
-            kernel_size,
+            in_features=in_features,
+            out_features=out_features,
+            kernel_size=kernel_size,
             strides=strides,
             padding=padding,
             output_padding=output_padding,
             kernel_dilation=kernel_dilation,
             weight_init_func=weight_init_func,
             bias_init_func=bias_init_func,
             groups=groups,
-            ndim=1,
             key=key,
+            spatial_ndim=1,
         )
 
 
-@pytc.treeclass
-class Conv2DTranspose(ConvNDTranspose):
+class FFTConv2DTranspose(FFTConvNDTranspose):
     def __init__(
         self,
         in_features: int,
         out_features: int,
-        kernel_size: int | tuple[int, ...],
+        kernel_size: KernelSizeType,
         *,
-        strides: int | tuple[int, ...] = 1,
-        padding: str | int | tuple[int, ...] | tuple[tuple[int, int], ...] = "SAME",
+        strides: StridesType = 1,
+        padding: PaddingType = "SAME",
         output_padding: int = 0,
-        kernel_dilation: int | tuple[int, ...] = 1,
-        weight_init_func: str | Callable = "glorot_uniform",
-        bias_init_func: str | Callable = "zeros",
+        kernel_dilation: DilationType = 1,
+        weight_init_func: InitFuncType = "glorot_uniform",
+        bias_init_func: InitFuncType = "zeros",
         groups: int = 1,
-        key: jr.PRNGKey = jr.PRNGKey(0),
+        key: jr.KeyArray = jr.PRNGKey(0),
     ):
+        """2D FFT Convolutional Transpose Layer.
+
+        Args:
+            in_features : Number of input channels
+            out_features : Number of output channels
+            kernel_size : Size of the convolutional kernel
+            strides : Stride of the convolution
+            padding : Padding of the input
+            output_padding : Additional size added to one side of the output shape
+            kernel_dilation : Dilation of the kernel
+            weight_init_func : Weight initialization function
+            bias_init_func : Bias initialization function
+            groups : Number of groups
+            spatial_ndim : Number of dimensions
+            key : PRNG key
+        """
         super().__init__(
-            in_features,
-            out_features,
-            kernel_size,
+            in_features=in_features,
+            out_features=out_features,
+            kernel_size=kernel_size,
             strides=strides,
             padding=padding,
             output_padding=output_padding,
             kernel_dilation=kernel_dilation,
             weight_init_func=weight_init_func,
             bias_init_func=bias_init_func,
             groups=groups,
-            ndim=2,
             key=key,
+            spatial_ndim=2,
         )
 
 
-@pytc.treeclass
-class Conv3DTranspose(ConvNDTranspose):
+class FFTConv3DTranspose(FFTConvNDTranspose):
     def __init__(
         self,
         in_features: int,
         out_features: int,
-        kernel_size: int | tuple[int, ...],
+        kernel_size: KernelSizeType,
         *,
-        strides: int | tuple[int, ...] = 1,
-        padding: str | int | tuple[int, ...] | tuple[tuple[int, int], ...] = "SAME",
+        strides: StridesType = 1,
+        padding: PaddingType = "SAME",
         output_padding: int = 0,
-        kernel_dilation: int | tuple[int, ...] = 1,
-        weight_init_func: str | Callable = "glorot_uniform",
-        bias_init_func: str | Callable = "zeros",
+        kernel_dilation: DilationType = 1,
+        weight_init_func: InitFuncType = "glorot_uniform",
+        bias_init_func: InitFuncType = "zeros",
         groups: int = 1,
-        key: jr.PRNGKey = jr.PRNGKey(0),
+        key: jr.KeyArray = jr.PRNGKey(0),
     ):
+        """3D FFT Convolutional Transpose Layer.
+
+        Args:
+            in_features : Number of input channels
+            out_features : Number of output channels
+            kernel_size : Size of the convolutional kernel
+            strides : Stride of the convolution
+            padding : Padding of the input
+            output_padding : Additional size added to one side of the output shape
+            kernel_dilation : Dilation of the kernel
+            weight_init_func : Weight initialization function
+            bias_init_func : Bias initialization function
+            groups : Number of groups
+            spatial_ndim : Number of dimensions
+            key : PRNG key
+        """
         super().__init__(
-            in_features,
-            out_features,
-            kernel_size,
+            in_features=in_features,
+            out_features=out_features,
+            kernel_size=kernel_size,
             strides=strides,
             padding=padding,
             output_padding=output_padding,
             kernel_dilation=kernel_dilation,
             weight_init_func=weight_init_func,
             bias_init_func=bias_init_func,
             groups=groups,
-            ndim=3,
             key=key,
+            spatial_ndim=3,
         )
 
 
-# ------------------------------ Depthwise Convolutional Layers ------------------------------ #
+# ----------------------------------------------------------------------------------------------------------------------#
+
+
+class DepthwiseFFTConvND(pytc.TreeClass):
+    weight: jax.Array
+    bias: jax.Array
 
+    in_features: int = pytc.field(callbacks=[positive_int_cb])
+    kernel_size: KernelSizeType
+    strides: StridesType
+    padding: PaddingType
+    depth_multiplier: int = pytc.field(callbacks=[positive_int_cb])
 
-@pytc.treeclass
-class DepthwiseConvND:
-    weight: jnp.ndarray
-    bias: jnp.ndarray
-
-    in_features: int = pytc.nondiff_field()  # number of input features
-    kernel_size: int | tuple[int, ...] = pytc.nondiff_field()
-    strides: int | tuple[int, ...] = pytc.nondiff_field()  # stride of the convolution
-    padding: str | int | tuple[int, ...] | tuple[tuple[int, int], ...] = pytc.nondiff_field()  # fmt: skip
-    depth_multiplier: int = pytc.nondiff_field()
-
-    weight_init_func: str | Callable[[jr.PRNGKey, tuple[int, ...]], jnp.ndarray]
-    bias_init_func: str | Callable[[jr.PRNGKey, tuple[int]], jnp.ndarray]
-    kernel_dilation: int | tuple[int, ...] = pytc.nondiff_field()
+    weight_init_func: InitFuncType = pytc.field(callbacks=[init_func_cb])
+    bias_init_func: InitFuncType = pytc.field(callbacks=[init_func_cb])
 
     def __init__(
         self,
         in_features: int,
         kernel_size: int | tuple[int, ...],
         *,
         depth_multiplier: int = 1,
-        strides: int = 1,
-        padding: str | int | tuple[int, ...] | tuple[tuple[int, int], ...] = "SAME",
-        weight_init_func: str | Callable = "glorot_uniform",
-        bias_init_func: str | Callable = "zeros",
-        ndim: int = 2,
-        key: jr.PRNGKey = jr.PRNGKey(0),
+        strides: StridesType = 1,
+        padding: PaddingType = "SAME",
+        weight_init_func: InitFuncType = "glorot_uniform",
+        bias_init_func: InitFuncType = "zeros",
+        key: jr.KeyArray = jr.PRNGKey(0),
+        spatial_ndim: int = 2,
     ):
         """Depthwise Convolutional layer.
 
         Args:
             in_features: number of input features
             kernel_size: size of the convolution kernel
             depth_multiplier : number of output channels per input channel
             strides: stride of the convolution
             padding: padding of the input
             weight_init_func: function to initialize the weights
             bias_init_func: function to initialize the bias
-            ndim: number of spatial dimensions
+            spatial_ndim: number of spatial dimensions
             key: random key for weight initialization
 
-        Examples:
+        Examples:----
             >>> l1 = DepthwiseConvND(3, 3, depth_multiplier=2, strides=2, padding="SAME")
             >>> l1(jnp.ones((3, 32, 32))).shape
             (3, 16, 16, 6)
 
         Note:
             See :
                 https://keras.io/api/layers/convolution_layers/depthwise_convolution2d/
                 https://github.com/google/flax/blob/main/flax/linen/linear.py
         """
-        if in_features is None:
-            for field_item in dataclasses.fields(self):
-                setattr(self, field_item.name, None)
-
-            self._partial_init = ft.partial(
-                DepthwiseConvND.__init__,
-                self=self,
-                kernel_size=kernel_size,
-                depth_multiplier=depth_multiplier,
-                strides=strides,
-                padding=padding,
-                weight_init_func=weight_init_func,
-                bias_init_func=bias_init_func,
-                ndim=ndim,
-                key=key,
-            )
-            return
-
-        if hasattr(self, "_partial_init"):
-            delattr(self, "_partial_init")
-
-        if not isinstance(in_features, int) or in_features <= 0:
-            raise ValueError(
-                f"Expected in_features to be a positive integer, got {in_features}"
-            )
-
-        if not isinstance(depth_multiplier, int) or depth_multiplier <= 0:
-            raise ValueError(
-                f"Expected depth_multiplier to be a positive integer, got {depth_multiplier}"
-            )
 
+        # already checked by the callbacks
         self.in_features = in_features
         self.depth_multiplier = depth_multiplier
+        self.spatial_ndim = spatial_ndim
+        self.weight_init_func = weight_init_func
+        self.bias_init_func = bias_init_func
+
+        # needs more info to be checked
+        self.kernel_size = canonicalize(kernel_size, spatial_ndim, "kernel_size")  # fmt: skip
+        self.strides = canonicalize(strides, spatial_ndim, "strides")  # fmt: skip
+        self.input_dilation = canonicalize(1, spatial_ndim, "input_dilation")  # fmt: skip
+        self.kernel_dilation = canonicalize(1, spatial_ndim, "kernel_dilation")  # fmt: skip
 
-        self.kernel_size = _check_and_return_kernel(kernel_size, ndim)
-        self.strides = _check_and_return_strides(strides, ndim)
-        self.input_dilation = _check_and_return_input_dilation(1, ndim)
-        self.kernel_dilation = _check_and_return_kernel_dilation(1, ndim)
-        self.padding = _check_and_return_padding(padding, self.kernel_size)
-        self.weight_init_func = _check_and_return_init_func(weight_init_func, "weight_init_func")  # fmt: skip
-        self.bias_init_func = _check_and_return_init_func(bias_init_func, "bias_init_func")  # fmt: skip
+        self.padding = padding
 
         weight_shape = (depth_multiplier * in_features, 1, *self.kernel_size)  # OIHW
         self.weight = self.weight_init_func(key, weight_shape)
 
         if bias_init_func is None:
             self.bias = None
         else:
-            bias_shape = (depth_multiplier * in_features, *(1,) * ndim)
+            bias_shape = (depth_multiplier * in_features, *(1,) * spatial_ndim)
             self.bias = self.bias_init_func(key, bias_shape)
 
-        self.dimension_numbers = ConvDimensionNumbers(*((tuple(range(ndim + 2)),) * 3))
-
-    def __call__(self, x: jnp.ndarray, **kwargs) -> jnp.ndarray:
-        if hasattr(self, "_partial_init"):
-            if isinstance(x, jax.core.Tracer):
-                raise ValueError(_TRACER_ERROR_MSG(self.__class__.__name__))
-            self._partial_init(in_features=x.shape[0])
-
-        y = jax.lax.conv_general_dilated(
-            lhs=x[None],
-            rhs=self.weight,
-            window_strides=self.strides,
+    @ft.partial(validate_spatial_in_shape, attribute_name="spatial_ndim")
+    @ft.partial(validate_in_features, attribute_name="in_features")
+    def __call__(self, x: jax.Array, **k) -> jax.Array:
+        padding = delayed_canonicalize_padding(
+            in_dim=x.shape[1:],
             padding=self.padding,
-            lhs_dilation=self.input_dilation,
-            rhs_dilation=self.kernel_dilation,
-            dimension_numbers=self.dimension_numbers,
-            feature_group_count=self.in_features,
+            kernel_size=self.kernel_size,
+            strides=self.strides,
         )
 
+        y = fft_conv_general_dilated(
+            jnp.expand_dims(x, axis=0),
+            self.weight,
+            strides=self.strides,
+            padding=padding,
+            groups=x.shape[0],
+            dilation=self.kernel_dilation,
+        )
+        y = jnp.squeeze(y, axis=0)
         if self.bias is None:
-            return y[0]
-        return (y + self.bias)[0]
+            return y
+        return y + self.bias
 
 
-@pytc.treeclass
-class DepthwiseConv1D(DepthwiseConvND):
+class DepthwiseFFTConv1D(DepthwiseFFTConvND):
     def __init__(
         self,
         in_features: int,
         kernel_size: int | tuple[int, ...],
         *,
         depth_multiplier: int = 1,
-        strides: int = 1,
-        padding: str | int | tuple[int, ...] | tuple[tuple[int, int], ...] = "SAME",
-        weight_init_func: str | Callable = "glorot_uniform",
-        bias_init_func: str | Callable = "zeros",
-        key: jr.PRNGKey = jr.PRNGKey(0),
+        strides: StridesType = 1,
+        padding: PaddingType = "SAME",
+        weight_init_func: InitFuncType = "glorot_uniform",
+        bias_init_func: InitFuncType = "zeros",
+        key: jr.KeyArray = jr.PRNGKey(0),
     ):
+        """1D Depthwise FFT Convolutional layer.
+
+        Args:
+            in_features: number of input features
+            kernel_size: size of the convolution kernel
+            depth_multiplier : number of output channels per input channel
+            strides: stride of the convolution
+            padding: padding of the input
+            weight_init_func: function to initialize the weights
+            bias_init_func: function to initialize the bias
+            spatial_ndim: number of spatial dimensions
+            key: random key for weight initialization
+
+        Note:
+            See :
+                https://keras.io/api/layers/convolution_layers/depthwise_convolution2d/
+                https://github.com/google/flax/blob/main/flax/linen/linear.py
+        """
         super().__init__(
-            in_features,
-            kernel_size,
+            in_features=in_features,
+            kernel_size=kernel_size,
             depth_multiplier=depth_multiplier,
             strides=strides,
             padding=padding,
             weight_init_func=weight_init_func,
             bias_init_func=bias_init_func,
-            ndim=1,
             key=key,
+            spatial_ndim=1,
         )
 
 
-@pytc.treeclass
-class DepthwiseConv2D(DepthwiseConvND):
+class DepthwiseFFTConv2D(DepthwiseFFTConvND):
     def __init__(
         self,
         in_features: int,
         kernel_size: int | tuple[int, ...],
         *,
         depth_multiplier: int = 1,
-        strides: int = 1,
-        padding: str | int | tuple[int, ...] | tuple[tuple[int, int], ...] = "SAME",
-        weight_init_func: str | Callable = "glorot_uniform",
-        bias_init_func: str | Callable = "zeros",
-        key: jr.PRNGKey = jr.PRNGKey(0),
+        strides: StridesType = 1,
+        padding: PaddingType = "SAME",
+        weight_init_func: InitFuncType = "glorot_uniform",
+        bias_init_func: InitFuncType = "zeros",
+        key: jr.KeyArray = jr.PRNGKey(0),
     ):
+        """2D Depthwise FFT Convolutional layer.
+
+        Args:
+            in_features: number of input features
+            kernel_size: size of the convolution kernel
+            depth_multiplier : number of output channels per input channel
+            strides: stride of the convolution
+            padding: padding of the input
+            weight_init_func: function to initialize the weights
+            bias_init_func: function to initialize the bias
+            spatial_ndim: number of spatial dimensions
+            key: random key for weight initialization
+
+        Note:
+            See :
+                https://keras.io/api/layers/convolution_layers/depthwise_convolution2d/
+                https://github.com/google/flax/blob/main/flax/linen/linear.py
+        """
         super().__init__(
-            in_features,
-            kernel_size,
+            in_features=in_features,
+            kernel_size=kernel_size,
             depth_multiplier=depth_multiplier,
             strides=strides,
             padding=padding,
             weight_init_func=weight_init_func,
             bias_init_func=bias_init_func,
-            ndim=2,
             key=key,
+            spatial_ndim=2,
         )
 
 
-@pytc.treeclass
-class DepthwiseConv3D(DepthwiseConvND):
+class DepthwiseFFTConv3D(DepthwiseFFTConvND):
     def __init__(
         self,
         in_features: int,
         kernel_size: int | tuple[int, ...],
         *,
         depth_multiplier: int = 1,
-        strides: int = 1,
-        padding: str | int | tuple[int, ...] | tuple[tuple[int, int], ...] = "SAME",
-        weight_init_func: str | Callable = "glorot_uniform",
-        bias_init_func: str | Callable = "zeros",
-        key: jr.PRNGKey = jr.PRNGKey(0),
+        strides: StridesType = 1,
+        padding: PaddingType = "SAME",
+        weight_init_func: InitFuncType = "glorot_uniform",
+        bias_init_func: InitFuncType = "zeros",
+        key: jr.KeyArray = jr.PRNGKey(0),
     ):
+        """3D Depthwise FFT Convolutional layer.
+
+        Args:
+            in_features: number of input features
+            kernel_size: size of the convolution kernel
+            depth_multiplier : number of output channels per input channel
+            strides: stride of the convolution
+            padding: padding of the input
+            weight_init_func: function to initialize the weights
+            bias_init_func: function to initialize the bias
+            spatial_ndim: number of spatial dimensions
+            key: random key for weight initialization
+
+        Note:
+            See :
+                https://keras.io/api/layers/convolution_layers/depthwise_convolution2d/
+                https://github.com/google/flax/blob/main/flax/linen/linear.py
+        """
         super().__init__(
-            in_features,
-            kernel_size,
+            in_features=in_features,
+            kernel_size=kernel_size,
             depth_multiplier=depth_multiplier,
             strides=strides,
             padding=padding,
             weight_init_func=weight_init_func,
             bias_init_func=bias_init_func,
-            ndim=3,
             key=key,
+            spatial_ndim=3,
         )
 
 
-# ------------------------------ SeparableConvND Depthwise Convolutional Layers ------------------------------ #
+# ----------------------------------------------------------------------------------------------------------------------#
 
 
-@pytc.treeclass
-class SeparableConvND:
-    depthwise_conv: DepthwiseConvND
-    pointwise_conv: DepthwiseConvND
+class SeparableFFTConvND(pytc.TreeClass):
+    depthwise_conv: DepthwiseFFTConvND
+    pointwise_conv: DepthwiseFFTConvND
 
     def __init__(
         self,
         in_features: int,
         out_features: int,
-        kernel_size: int | tuple[int, ...],
+        kernel_size: KernelSizeType,
         *,
         depth_multiplier: int = 1,
-        strides: int | tuple[int, ...] = 1,
-        padding: str | int | tuple[int, ...] | tuple[tuple[int, int], ...] = "SAME",
-        depthwise_weight_init_func: str | Callable = "glorot_uniform",
-        pointwise_weight_init_func: str | Callable = "glorot_uniform",
-        pointwise_bias_init_func: str | Callable = "zeros",
-        ndim: int = 2,
-        key: jr.PRNGKey = jr.PRNGKey(0),
+        strides: StridesType = 1,
+        padding: PaddingType = "SAME",
+        depthwise_weight_init_func: InitFuncType = "glorot_uniform",
+        pointwise_weight_init_func: InitFuncType = "glorot_uniform",
+        pointwise_bias_init_func: InitFuncType = "zeros",
+        key: jr.KeyArray = jr.PRNGKey(0),
+        spatial_ndim: int = 2,
     ):
         """Separable convolutional layer.
 
         Note:
             See:
                 https://en.wikipedia.org/wiki/Separable_filter
                 https://keras.io/api/layers/convolution_layers/separable_convolution2d/
@@ -758,439 +912,197 @@
             kernel_size : Size of the convolving kernel.
             depth_multiplier : Number of depthwise convolution output channels for each input channel.
             strides : Stride of the convolution.
             padding : Padding to apply to the input.
             depthwise_weight_init_func : Function to initialize the depthwise convolution weights.
             pointwise_weight_init_func : Function to initialize the pointwise convolution weights.
             pointwise_bias_init_func : Function to initialize the pointwise convolution bias.
-            ndim : Number of spatial dimensions.
+            spatial_ndim : Number of spatial dimensions.
 
         """
-        if in_features is None:
-            for field_item in dataclasses.fields(self):
-                setattr(self, field_item.name, None)
-            self._partial_init = ft.partial(
-                SeparableConvND.__init__,
-                self=self,
-                out_features=out_features,
-                kernel_size=kernel_size,
-                depth_multiplier=depth_multiplier,
-                strides=strides,
-                padding=padding,
-                depthwise_weight_init_func=depthwise_weight_init_func,
-                pointwise_weight_init_func=pointwise_weight_init_func,
-                pointwise_bias_init_func=pointwise_bias_init_func,
-                ndim=ndim,
-                key=key,
-            )
-            return
-
-        if hasattr(self, "_partial_init"):
-            delattr(self, "_partial_init")
-
-        if not isinstance(in_features, int) or in_features <= 0:
-            raise ValueError(
-                f"Expected in_features to be a positive integer, got {in_features}"
-            )
-
-        if not isinstance(out_features, int) or out_features <= 0:
-            raise ValueError(
-                f"Expected out_features to be a positive integer, got {out_features}"
-            )
-
-        if not isinstance(depth_multiplier, int) or depth_multiplier <= 0:
-            raise ValueError(
-                f"Expected depth_multiplier to be a positive integer, got {depth_multiplier}"
-            )
-
         self.in_features = in_features
-        self.out_features = out_features
-        self.depth_multiplier = depth_multiplier
+        self.depth_multiplier = canonicalize(depth_multiplier, self.in_features, "depth_multiplier")  # fmt: skip
+        self.spatial_ndim = spatial_ndim
 
-        self.kernel_size = _check_and_return_kernel(kernel_size, ndim)
-        self.strides = _check_and_return_strides(strides, ndim)
-        self.padding = _check_and_return_padding(padding, self.kernel_size)
-        self.depthwise_weight_init_func = _check_and_return_init_func(
-            depthwise_weight_init_func, "depthwise_weight_init_func"
-        )
-        self.pointwise_weight_init_func = _check_and_return_init_func(
-            pointwise_weight_init_func, "pointwise_weight_init_func"
-        )
-        self.pointwise_bias_init_func = _check_and_return_init_func(
-            pointwise_bias_init_func, "pointwise_bias_init_func"
-        )
-
-        self.ndim = ndim
-
-        self.depthwise_conv = DepthwiseConvND(
+        self.depthwise_conv = DepthwiseFFTConvND(
             in_features=in_features,
             depth_multiplier=depth_multiplier,
-            kernel_size=self.kernel_size,
+            kernel_size=kernel_size,
             strides=strides,
             padding=padding,
             weight_init_func=depthwise_weight_init_func,
             bias_init_func=None,  # no bias for lhs
             key=key,
-            ndim=ndim,
+            spatial_ndim=spatial_ndim,
         )
 
-        self.pointwise_conv = ConvND(
+        self.pointwise_conv = FFTConvND(
             in_features=in_features * depth_multiplier,
             out_features=out_features,
             kernel_size=1,
             strides=strides,
             padding=padding,
             weight_init_func=pointwise_weight_init_func,
             bias_init_func=pointwise_bias_init_func,
             key=key,
-            ndim=ndim,
+            spatial_ndim=spatial_ndim,
         )
 
-    def __call__(self, x: jnp.ndarray, **kwargs) -> jnp.ndarray:
-        if hasattr(self, "_partial_init"):
-            if isinstance(x, jax.core.Tracer):
-                raise ValueError(_TRACER_ERROR_MSG(self.__class__.__name__))
-            self._partial_init(in_features=x.shape[0])
-
+    @ft.partial(validate_spatial_in_shape, attribute_name="spatial_ndim")
+    @ft.partial(validate_in_features, attribute_name="in_features")
+    def __call__(self, x: jax.Array, **k) -> jax.Array:
         x = self.depthwise_conv(x)
         x = self.pointwise_conv(x)
         return x
 
 
-@pytc.treeclass
-class SeparableConv1D(SeparableConvND):
-    """1D separable convolutional layer."""
-
+class SeparableFFTConv1D(SeparableFFTConvND):
     def __init__(
         self,
         in_features: int,
         out_features: int,
-        kernel_size: int | tuple[int, ...],
+        kernel_size: KernelSizeType,
         *,
         depth_multiplier: int = 1,
-        strides: int | tuple[int, ...] = 1,
-        padding: str | int | tuple[int, ...] | tuple[tuple[int, int], ...] = "SAME",
-        depthwise_weight_init_func: str | Callable = "glorot_uniform",
-        pointwise_weight_init_func: str | Callable = "glorot_uniform",
-        pointwise_bias_init_func: str | Callable = "zeros",
-        key: jr.PRNGKey = jr.PRNGKey(0),
+        strides: StridesType = 1,
+        padding: PaddingType = "SAME",
+        depthwise_weight_init_func: InitFuncType = "glorot_uniform",
+        pointwise_weight_init_func: InitFuncType = "glorot_uniform",
+        pointwise_bias_init_func: InitFuncType = "zeros",
+        key: jr.KeyArray = jr.PRNGKey(0),
     ):
-        super().__init__(
-            in_features,
-            out_features,
-            kernel_size,
-            depth_multiplier=depth_multiplier,
-            strides=strides,
-            padding=padding,
-            depthwise_weight_init_func=depthwise_weight_init_func,
-            pointwise_weight_init_func=pointwise_weight_init_func,
-            pointwise_bias_init_func=pointwise_bias_init_func,
-            ndim=1,
-            key=key,
-        )
+        """Separable 1D FFT Convolutional layer.
 
+        Note:
+            See:
+                https://en.wikipedia.org/wiki/Separable_filter
+                https://keras.io/api/layers/convolution_layers/separable_convolution2d/
+                https://github.com/deepmind/dm-haiku/blob/main/haiku/_src/depthwise_conv.py
 
-@pytc.treeclass
-class SeparableConv2D(SeparableConvND):
-    """2D separable convolutional layer."""
+        Args:
+            in_features : Number of input channels.
+            out_features : Number of output channels.
+            kernel_size : Size of the convolving kernel.
+            depth_multiplier : Number of depthwise convolution output channels for each input channel.
+            strides : Stride of the convolution.
+            padding : Padding to apply to the input.
+            depthwise_weight_init_func : Function to initialize the depthwise convolution weights.
+            pointwise_weight_init_func : Function to initialize the pointwise convolution weights.
+            pointwise_bias_init_func : Function to initialize the pointwise convolution bias.
+            spatial_ndim : Number of spatial dimensions.
 
-    def __init__(
-        self,
-        in_features: int,
-        out_features: int,
-        kernel_size: int | tuple[int, ...],
-        *,
-        depth_multiplier: int = 1,
-        strides: int | tuple[int, ...] = 1,
-        padding: str | int | tuple[int, ...] | tuple[tuple[int, int], ...] = "SAME",
-        depthwise_weight_init_func: str | Callable = "glorot_uniform",
-        pointwise_weight_init_func: str | Callable = "glorot_uniform",
-        pointwise_bias_init_func: str | Callable = "zeros",
-        key: jr.PRNGKey = jr.PRNGKey(0),
-    ):
+        """
         super().__init__(
-            in_features,
-            out_features,
-            kernel_size,
+            in_features=in_features,
+            out_features=out_features,
+            kernel_size=kernel_size,
             depth_multiplier=depth_multiplier,
             strides=strides,
             padding=padding,
             depthwise_weight_init_func=depthwise_weight_init_func,
             pointwise_weight_init_func=pointwise_weight_init_func,
             pointwise_bias_init_func=pointwise_bias_init_func,
-            ndim=2,
             key=key,
+            spatial_ndim=1,
         )
 
 
-@pytc.treeclass
-class SeparableConv3D(SeparableConvND):
-    """3D separable convolutional layer."""
-
+class SeparableFFTConv2D(SeparableFFTConvND):
     def __init__(
         self,
         in_features: int,
         out_features: int,
-        kernel_size: int | tuple[int, ...],
+        kernel_size: KernelSizeType,
         *,
         depth_multiplier: int = 1,
-        strides: int | tuple[int, ...] = 1,
-        padding: str | int | tuple[int, ...] | tuple[tuple[int, int], ...] = "SAME",
-        depthwise_weight_init_func: str | Callable = "glorot_uniform",
-        pointwise_weight_init_func: str | Callable = "glorot_uniform",
-        pointwise_bias_init_func: str | Callable = "zeros",
-        key: jr.PRNGKey = jr.PRNGKey(0),
+        strides: StridesType = 1,
+        padding: PaddingType = "SAME",
+        depthwise_weight_init_func: InitFuncType = "glorot_uniform",
+        pointwise_weight_init_func: InitFuncType = "glorot_uniform",
+        pointwise_bias_init_func: InitFuncType = "zeros",
+        key: jr.KeyArray = jr.PRNGKey(0),
     ):
+        """Separable 2D FFT Convolutional layer.
+
+        Note:
+            See:
+                https://en.wikipedia.org/wiki/Separable_filter
+                https://keras.io/api/layers/convolution_layers/separable_convolution2d/
+                https://github.com/deepmind/dm-haiku/blob/main/haiku/_src/depthwise_conv.py
+
+        Args:
+            in_features : Number of input channels.
+            out_features : Number of output channels.
+            kernel_size : Size of the convolving kernel.
+            depth_multiplier : Number of depthwise convolution output channels for each input channel.
+            strides : Stride of the convolution.
+            padding : Padding to apply to the input.
+            depthwise_weight_init_func : Function to initialize the depthwise convolution weights.
+            pointwise_weight_init_func : Function to initialize the pointwise convolution weights.
+            pointwise_bias_init_func : Function to initialize the pointwise convolution bias.
+            spatial_ndim : Number of spatial dimensions.
+
+        """
         super().__init__(
-            in_features,
-            out_features,
-            kernel_size,
+            in_features=in_features,
+            out_features=out_features,
+            kernel_size=kernel_size,
             depth_multiplier=depth_multiplier,
             strides=strides,
             padding=padding,
             depthwise_weight_init_func=depthwise_weight_init_func,
             pointwise_weight_init_func=pointwise_weight_init_func,
             pointwise_bias_init_func=pointwise_bias_init_func,
-            ndim=3,
             key=key,
+            spatial_ndim=2,
         )
 
 
-# ------------------------------ ConvNDLocal Convolutional Layers ------------------------------ #
-
-
-@pytc.treeclass
-class ConvNDLocal:
-    weight: jnp.ndarray
-    bias: jnp.ndarray
-
-    in_features: int = pytc.nondiff_field()  # number of input features
-    out_features: int = pytc.nondiff_field()  # number of output features
-    kernel_size: int | tuple[int, ...] = pytc.nondiff_field()
-    in_size: tuple[int, ...] = pytc.nondiff_field()  # size of input
-    strides: int | tuple[int, ...] = pytc.nondiff_field()  # stride of the convolution
-    padding: str | int | tuple[int, ...] | tuple[tuple[int, int], ...] = pytc.nondiff_field()  # fmt: skip
-    input_dilation: int | tuple[int, ...] = pytc.nondiff_field()
-    kernel_dilation: int | tuple[int, ...] = pytc.nondiff_field()
-    weight_init_func: str | Callable[[jr.PRNGKey, tuple[int, ...]], jnp.ndarray]
-    bias_init_func: Callable[[jr.PRNGKey, tuple[int]], jnp.ndarray]
-
+class SeparableFFTConv3D(SeparableFFTConvND):
     def __init__(
         self,
         in_features: int,
         out_features: int,
-        kernel_size: int | tuple[int, ...],
+        kernel_size: KernelSizeType,
         *,
-        in_size: tuple[int, ...],
-        strides: int | tuple[int, ...] = 1,
-        padding: str | int | tuple[int, ...] | tuple[tuple[int, int], ...] = "SAME",
-        input_dilation: int | tuple[int, ...] = 1,
-        kernel_dilation: int | tuple[int, ...] = 1,
-        weight_init_func: str | Callable = "glorot_uniform",
-        bias_init_func: str | Callable = "zeros",
-        ndim: int = 2,
-        key: jr.PRNGKey = jr.PRNGKey(0),
+        depth_multiplier: int = 1,
+        strides: StridesType = 1,
+        padding: PaddingType = "SAME",
+        depthwise_weight_init_func: InitFuncType = "glorot_uniform",
+        pointwise_weight_init_func: InitFuncType = "glorot_uniform",
+        pointwise_bias_init_func: InitFuncType = "zeros",
+        key: jr.KeyArray = jr.PRNGKey(0),
     ):
-        """Local convolutional layer.
+        """Separable 3D FFT Convolutional layer.
 
-        Args:
-            in_features: number of input features
-            out_features: number of output features
-            kernel_size: size of the convolution kernel
-            in_size: size of the input
-            strides: stride of the convolution
-            padding: padding of the convolution
-            input_dilation: dilation of the input
-            kernel_dilation: dilation of the convolution kernel
-            weight_init_func: weight initialization function
-            bias_init_func: bias initialization function
-            ndim: number of dimensions
-            key: random number generator key
         Note:
-            See : https://keras.io/api/layers/locally_connected_layers/
-        """
-        if in_features is None:
-            for field_item in dataclasses.fields(self):
-                setattr(self, field_item.name, None)
-            self._partial_init = ft.partial(
-                ConvNDLocal.__init__,
-                self=self,
-                out_features=out_features,
-                kernel_size=kernel_size,
-                strides=strides,
-                padding=padding,
-                input_dilation=input_dilation,
-                kernel_dilation=kernel_dilation,
-                weight_init_func=weight_init_func,
-                bias_init_func=bias_init_func,
-                ndim=ndim,
-                key=key,
-            )
-            return
-
-        if hasattr(self, "_partial_init"):
-            delattr(self, "_partial_init")
-
-        if not isinstance(in_features, int) or in_features <= 0:
-            raise ValueError(
-                f"Expected in_features to be a positive integer, got {in_features}"
-            )
-
-        if not isinstance(out_features, int) or out_features <= 0:
-            raise ValueError(
-                f"Expected out_features to be a positive integer, got {out_features}"
-            )
-
-        self.in_features = in_features
-        self.out_features = out_features
-
-        self.in_size = _check_and_return_input_size(in_size, ndim)
-        self.kernel_size = _check_and_return_kernel(kernel_size, ndim)
-        self.strides = _check_and_return_strides(strides, ndim)
-        self.input_dilation = _check_and_return_input_dilation(input_dilation, ndim)
-        self.kernel_dilation = _check_and_return_kernel_dilation(1, ndim)
-        self.padding = _check_and_return_padding(padding, self.kernel_size)
-        self.weight_init_func = _check_and_return_init_func(weight_init_func, "weight_init_func")  # fmt: skip
-        self.bias_init_func = _check_and_return_init_func(bias_init_func, "bias_init_func")  # fmt: skip
-        self.dimension_numbers = ConvDimensionNumbers(*((tuple(range(ndim + 2)),) * 3))
-        self.out_size = _calculate_convolution_output_shape(
-            shape=self.in_size,
-            kernel_size=self.kernel_size,
-            padding=self.padding,
-            strides=self.strides,
-        )
-
-        # OIHW
-        self.weight_shape = (
-            self.out_features,
-            self.in_features * ft.reduce(op.mul, self.kernel_size),
-            *self.out_size,
-        )
-
-        self.weight = self.weight_init_func(key, self.weight_shape)
-
-        bias_shape = (self.out_features, *self.out_size)
-
-        if bias_init_func is None:
-            self.bias = None
-        else:
-            self.bias = self.bias_init_func(key, bias_shape)
-
-    def __call__(self, x: jnp.ndarray, **kwargs) -> jnp.ndarray:
-        if hasattr(self, "_partial_init"):
-            if isinstance(x, jax.core.Tracer):
-                raise ValueError(_TRACER_ERROR_MSG(self.__class__.__name__))
-            self._partial_init(in_features=x.shape[0], in_size=x.shape[1:])
-
-        y = jax.lax.conv_general_dilated_local(
-            lhs=x[None],
-            rhs=self.weight,
-            window_strides=self.strides,
-            padding=self.padding,
-            filter_shape=self.kernel_size,
-            lhs_dilation=self.kernel_dilation,
-            rhs_dilation=self.input_dilation,  # atrous dilation
-            dimension_numbers=self.dimension_numbers,
-        )
-
-        if self.bias is None:
-            return y[0]
-        return (y + self.bias)[0]
-
-
-@pytc.treeclass
-class Conv1DLocal(ConvNDLocal):
-    def __init__(
-        self,
-        in_features: int,
-        out_features: int,
-        kernel_size: int | tuple[int, ...],
-        *,
-        in_size: tuple[int, ...],
-        strides: int | tuple[int, ...] = 1,
-        padding: str | int | tuple[int, ...] | tuple[tuple[int, int], ...] = "SAME",
-        input_dilation: int | tuple[int, ...] = 1,
-        kernel_dilation: int | tuple[int, ...] = 1,
-        weight_init_func: str | Callable = "glorot_uniform",
-        bias_init_func: str | Callable = "zeros",
-        key: jr.PRNGKey = jr.PRNGKey(0),
-    ):
-        super().__init__(
-            in_features,
-            out_features,
-            kernel_size,
-            in_size=in_size,
-            strides=strides,
-            padding=padding,
-            input_dilation=input_dilation,
-            kernel_dilation=kernel_dilation,
-            weight_init_func=weight_init_func,
-            bias_init_func=bias_init_func,
-            ndim=1,
-            key=key,
-        )
-
-
-@pytc.treeclass
-class Conv2DLocal(ConvNDLocal):
-    def __init__(
-        self,
-        in_features: int,
-        out_features: int,
-        kernel_size: int | tuple[int, ...],
-        *,
-        in_size: tuple[int, ...],
-        strides: int | tuple[int, ...] = 1,
-        padding: str | int | tuple[int, ...] | tuple[tuple[int, int], ...] = "SAME",
-        input_dilation: int | tuple[int, ...] = 1,
-        kernel_dilation: int | tuple[int, ...] = 1,
-        weight_init_func: str | Callable = "glorot_uniform",
-        bias_init_func: str | Callable = "zeros",
-        key: jr.PRNGKey = jr.PRNGKey(0),
-    ):
-        super().__init__(
-            in_features,
-            out_features,
-            kernel_size,
-            in_size=in_size,
-            strides=strides,
-            padding=padding,
-            input_dilation=input_dilation,
-            kernel_dilation=kernel_dilation,
-            weight_init_func=weight_init_func,
-            bias_init_func=bias_init_func,
-            ndim=2,
-            key=key,
-        )
+            See:
+                https://en.wikipedia.org/wiki/Separable_filter
+                https://keras.io/api/layers/convolution_layers/separable_convolution2d/
+                https://github.com/deepmind/dm-haiku/blob/main/haiku/_src/depthwise_conv.py
 
+        Args:
+            in_features : Number of input channels.
+            out_features : Number of output channels.
+            kernel_size : Size of the convolving kernel.
+            depth_multiplier : Number of depthwise convolution output channels for each input channel.
+            strides : Stride of the convolution.
+            padding : Padding to apply to the input.
+            depthwise_weight_init_func : Function to initialize the depthwise convolution weights.
+            pointwise_weight_init_func : Function to initialize the pointwise convolution weights.
+            pointwise_bias_init_func : Function to initialize the pointwise convolution bias.
+            spatial_ndim : Number of spatial dimensions.
 
-@pytc.treeclass
-class Conv3DLocal(ConvNDLocal):
-    def __init__(
-        self,
-        in_features: int,
-        out_features: int,
-        kernel_size: int | tuple[int, ...],
-        *,
-        in_size: tuple[int, ...],
-        strides: int | tuple[int, ...] = 1,
-        padding: str | int | tuple[int, ...] | tuple[tuple[int, int], ...] = "SAME",
-        input_dilation: int | tuple[int, ...] = 1,
-        kernel_dilation: int | tuple[int, ...] = 1,
-        weight_init_func: str | Callable = "glorot_uniform",
-        bias_init_func: str | Callable = "zeros",
-        key: jr.PRNGKey = jr.PRNGKey(0),
-    ):
+        """
         super().__init__(
-            in_features,
-            out_features,
-            kernel_size,
-            in_size=in_size,
+            in_features=in_features,
+            out_features=out_features,
+            kernel_size=kernel_size,
+            depth_multiplier=depth_multiplier,
             strides=strides,
             padding=padding,
-            input_dilation=input_dilation,
-            kernel_dilation=kernel_dilation,
-            weight_init_func=weight_init_func,
-            bias_init_func=bias_init_func,
-            ndim=3,
+            depthwise_weight_init_func=depthwise_weight_init_func,
+            pointwise_weight_init_func=pointwise_weight_init_func,
+            pointwise_bias_init_func=pointwise_bias_init_func,
             key=key,
+            spatial_ndim=3,
         )
```

### Comparing `serket-0.0.9/serket/nn/flatten.py` & `serket-0.2.0b2/serket/nn/flatten.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,74 +1,68 @@
 from __future__ import annotations
 
-import functools as ft
-import operator as op
-
+import jax
 import jax.numpy as jnp
 import pytreeclass as pytc
 
+from serket.nn.callbacks import isinstance_factory
 
-@pytc.treeclass
-class Flatten:
-    start_dim: int = pytc.nondiff_field(default=0)
-    end_dim: int = pytc.nondiff_field(default=-1)
 
+class Flatten(pytc.TreeClass):
     """
-    See https://pytorch.org/docs/stable/generated/torch.nn.Flatten.html?highlight=flatten#torch.nn.Flatten
-
     Args:
         start_dim: the first dim to flatten
         end_dim: the last dim to flatten (inclusive)
-
     Returns:
         a function that flattens a jnp.ndarray
-    
+
     Example:
+        >>> import serket as sk
+        >>> import jax.numpy as jnp
         >>> Flatten(0,1)(jnp.ones([1,2,3,4,5])).shape
         (2, 3, 4, 5)
-
         >>> Flatten(0,2)(jnp.ones([1,2,3,4,5])).shape
         (6, 4, 5)
-
         >>> Flatten(1,2)(jnp.ones([1,2,3,4,5])).shape
         (1, 6, 4, 5)
-
         >>> Flatten(-1,-1)(jnp.ones([1,2,3,4,5])).shape
         (1, 2, 3, 4, 5)
-
         >>> Flatten(-2,-1)(jnp.ones([1,2,3,4,5])).shape
         (1, 2, 3, 20)
-
         >>> Flatten(-3,-1)(jnp.ones([1,2,3,4,5])).shape
         (1, 2, 60)
+
+    Note:
+        https://pytorch.org/docs/stable/generated/torch.nn.Flatten.html?highlight=flatten#torch.nn.Flatten
     """
 
-    def __call__(self, x: jnp.ndarray, **kwargs) -> jnp.ndarray:
-        # normalize start_dim and end_dim for negative indices
-        start = self.start_dim + (0 if self.start_dim >= 0 else len(x.shape))
-        end = self.end_dim + (0 if self.end_dim >= 0 else len(x.shape))
-
-        shape = list(x.shape[:start])
-        shape += [ft.reduce(op.mul, x.shape[start : end + 1])]
-        shape += list(x.shape[end + 1 :])
-        return jnp.reshape(x, shape)
+    start_dim: int = pytc.field(default=0, callbacks=[isinstance_factory(int)])
+    end_dim: int = pytc.field(default=-1, callbacks=[isinstance_factory(int)])
 
+    def __call__(self, x: jax.Array) -> jax.Array:
+        # normalize start_dim
+        start_dim = self.start_dim + (0 if self.start_dim >= 0 else x.ndim)
+        # normalize end_dim
+        end_dim = self.end_dim + 1 + (0 if self.end_dim >= 0 else x.ndim)
+        return jax.lax.collapse(x, start_dim, end_dim)
 
-@pytc.treeclass
-class Unflatten:
-    dim: int = pytc.nondiff_field(default=0)
-    shape: tuple = pytc.nondiff_field(default=None)
+
+class Unflatten(pytc.TreeClass):
+    dim: int = pytc.field(default=0, callbacks=[isinstance_factory(int)])
+    shape: tuple = pytc.field(default=None, callbacks=[isinstance_factory(tuple)])
 
     """
-    See https://pytorch.org/docs/stable/generated/torch.nn.Unflatten.html?highlight=unflatten
+    
     Example:
         >>> Unflatten(0, (1,2,3,4,5))(jnp.ones([120])).shape
         (1, 2, 3, 4, 5)
-
         >>> Unflatten(2,(2,3))(jnp.ones([1,2,6])).shape
         (1, 2, 2, 3)
+
+    Note:
+        https://pytorch.org/docs/stable/generated/torch.nn.Unflatten.html?highlight=unflatten
     """
 
-    def __call__(self, x: jnp.ndaray, **kwargs) -> jnp.ndarray:
+    def __call__(self, x: jax.Array, **k) -> jax.Array:
         shape = list(x.shape)
         shape = [*shape[: self.dim], *self.shape, *shape[self.dim + 1 :]]
         return jnp.reshape(x, shape)
```

### Comparing `serket-0.0.9/serket/nn/flip.py` & `serket-0.2.0b2/serket/nn/flip.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,63 @@
+from __future__ import annotations
+
+import functools as ft
+
 import jax
 import jax.numpy as jnp
 import pytreeclass as pytc
 
+from serket.nn.callbacks import validate_spatial_in_shape
+
 
-@pytc.treeclass
-class FlipLeftRight2D:
-    """Flip channels left to right.
-
-    Note:
-        See: https://github.com/deepmind/dm_pix/blob/master/dm_pix/_src/augment.py
-
-    Examples:
-        >>> x = jnp.arange(1,10).reshape(1,3, 3)
-        >>> x
-        [[[1 2 3]
-          [4 5 6]
-          [7 8 9]]]
-
-        >>> FlipLeftRight2D()(x)
-        [[[3 2 1]
-          [6 5 4]
-          [9 8 7]]]
-    """
-
-    def __call__(self, x: jnp.ndarray, **kwargs) -> jnp.ndarray:
-        msg = f"Input must have 3 dimensions, got {x.ndim}."
-        assert x.ndim == 3, msg
+class FlipLeftRight2D(pytc.TreeClass):
+    def __init__(self):
+        """Flip channels left to right.
+
+        Note:
+            See: https://github.com/deepmind/dm_pix/blob/master/dm_pix/_src/augment.py
+
+        Examples:
+            >>> x = jnp.arange(1,10).reshape(1,3, 3)
+            >>> x
+            [[[1 2 3]
+            [4 5 6]
+            [7 8 9]]]
+
+            >>> FlipLeftRight2D()(x)
+            [[[3 2 1]
+            [6 5 4]
+            [9 8 7]]]
+        """
+        self.spatial_ndim = 2
+
+    @ft.partial(validate_spatial_in_shape, attribute_name="spatial_ndim")
+    def __call__(self, x: jax.Array, **k) -> jax.Array:
         flip = lambda x: jnp.flip(x, axis=1)
         return jax.vmap(flip)(x)
 
 
-@pytc.treeclass
-class FlipUpDown2D:
-    """Flip channels up to down.
-
-    Note:
-        See: https://github.com/deepmind/dm_pix/blob/master/dm_pix/_src/augment.py
-
-    Examples:
-        >>> x = jnp.arange(1,10).reshape(1,3, 3)
-        >>> x
-        [[[1 2 3]
-          [4 5 6]
-          [7 8 9]]]
-
-        >>> FlipUpDown2D()(x)
-        [[[7 8 9]
-          [4 5 6]
-          [1 2 3]]]
-    """
-
-    def __call__(self, x: jnp.ndarray, **kwargs) -> jnp.ndarray:
-        msg = f"Input must have 3 dimensions, got {x.ndim}."
-        assert x.ndim == 3, msg
+class FlipUpDown2D(pytc.TreeClass):
+    def __init__(self):
+        """Flip channels up to down.
+
+        Note:
+            See: https://github.com/deepmind/dm_pix/blob/master/dm_pix/_src/augment.py
+
+        Examples:
+            >>> x = jnp.arange(1,10).reshape(1,3, 3)
+            >>> x
+            [[[1 2 3]
+            [4 5 6]
+            [7 8 9]]]
+
+            >>> FlipUpDown2D()(x)
+            [[[7 8 9]
+            [4 5 6]
+            [1 2 3]]]
+        """
+        self.spatial_ndim = 2
+
+    @ft.partial(validate_spatial_in_shape, attribute_name="spatial_ndim")
+    def __call__(self, x: jax.Array, **k) -> jax.Array:
         flip = lambda x: jnp.flip(x, axis=0)
         return jax.vmap(flip)(x)
```

### Comparing `serket-0.0.9/serket/nn/laplace.py` & `serket-0.2.0b2/serket/nn/laplace.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from __future__ import annotations
 
+import functools as ft
+
 import jax
-import jax.numpy as jnp
 import kernex as kex
 import pytreeclass as pytc
 
+from serket.nn.callbacks import validate_spatial_in_shape
+
 
-@pytc.treeclass
-class Laplace2D:
+class Laplace2D(pytc.TreeClass):
     def __init__(self):
         # apply laplace operator on channel axis
         @jax.vmap
         @kex.kmap(kernel_size=(3, 3), strides=(1, 1), padding="SAME")
         def op(x):
             return -4 * x[1, 1] + x[0, 1] + x[2, 1] + x[1, 0] + x[1, 2]
 
         self._func = op
+        self.spatial_ndim = 2
 
-    def __call__(self, x: jnp.ndarray, **kwargs) -> jnp.ndarray:
-        msg = f"Input must have 3 dimensions, got {x.ndim}."
-        assert x.ndim == 3, msg
+    @ft.partial(validate_spatial_in_shape, attribute_name="spatial_ndim")
+    def __call__(self, x: jax.Array, **k) -> jax.Array:
         return self._func(x)
```

### Comparing `serket-0.0.9/serket/nn/linear.py` & `serket-0.2.0b2/serket/nn/linear.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,183 +1,181 @@
 from __future__ import annotations
 
-import dataclasses
 import functools as ft
-from typing import Callable, Sequence
 
 import jax
 import jax.numpy as jnp
 import jax.random as jr
 import pytreeclass as pytc
 
-from serket.nn.utils import (
-    _TRACER_ERROR_MSG,
-    _check_and_return_init_func,
-    _general_linear_einsum_string,
-    _multilinear_einsum_string,
-)
+from serket.nn.callbacks import init_func_cb, isinstance_factory, positive_int_cb
+from serket.nn.utils import InitFuncType
 
 
-@pytc.treeclass
-class Multilinear:
-    weight: jnp.ndarray
-    bias: jnp.ndarray
+@ft.lru_cache(maxsize=None)
+def _multilinear_einsum_string(degree: int) -> str:
+    # Generate einsum string for a linear layer of degree n
+    # Example:
+    #     >>> _multilinear_einsum_string(1)
+    #     '...a,ab->....b'
+    #     >>> _multilinear_einsum_string(2)
+    #     '...a,...b,abc->....c'
+
+    alpha = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ"
+
+    if not (1 <= degree <= len(alpha) - 1):
+        msg = f"degree must be between 1 and {len(alpha)-1}, got {degree}"
+        raise ValueError(msg)
+
+    xs_string = [f"...{i}" for i in alpha[:degree]]
+    output_string = ",".join(xs_string)
+    output_string += f",{alpha[:degree+1]}->...{alpha[degree]}"
+    return output_string
+
+
+@ft.lru_cache(maxsize=None)
+def _general_linear_einsum_string(*axes: tuple[int, ...]) -> str:
+    # Return the einsum string for a general linear layer.
+    # Example:
+    #     # apply linear layer to last axis
+    #     >>> _general_linear_einsum_string(-1)
+    #     '...0,01->...1'
+
+    #     # apply linear layer to last two axes
+    #     >>> _general_linear_einsum_string(-1,-2)
+    #     '...01,012->...2'
+
+    #     # apply linear layer to second last axis
+    #     >>> _general_linear_einsum_string(-2)
+    #     '...01,02->...12'
+
+    #     # apply linear layer to last and third last axis
+    #     >>> _general_linear_einsum_string(-1,-3)
+    #     '...012,023->...13'
+
+    if not all([i < 0 for i in axes]):
+        raise ValueError("axes should be negative")
+
+    axes = sorted(axes)
+    total_axis = abs(min(axes))  # get the total number of axes
+    alpha = "".join(map(str, range(total_axis + 1)))
+    input_string = "..." + alpha[:total_axis]
+    weight_string = "".join([input_string[axis] for axis in axes]) + alpha[total_axis]
+    result_string = "".join([ai for ai in input_string if ai not in weight_string])
+    result_string += alpha[total_axis]
+    return f"{input_string},{weight_string}->{result_string}"
+
+
+class Multilinear(pytc.TreeClass):
+    weight: jax.Array
+    bias: jax.Array
 
-    in_features: tuple[int, ...] | None = pytc.nondiff_field()
-    out_features: int = pytc.nondiff_field()
+    in_features: tuple[int, ...] | None = pytc.field(callbacks=[isinstance_factory((int, tuple))])  # fmt: skip
+    out_features: int
 
     def __init__(
         self,
         in_features: int | tuple[int, ...] | None,
         out_features: int,
         *,
-        weight_init_func: str | Callable = "he_normal",
-        bias_init_func: str | Callable = "ones",
-        key: jr.PRNGKey = jr.PRNGKey(0),
+        weight_init_func: InitFuncType = "he_normal",
+        bias_init_func: InitFuncType = "ones",
+        key: jr.KeyArray = jr.PRNGKey(0),
     ):
         """Linear layer with arbitrary number of inputs applied to last axis of each input
 
         Args:
             in_features: number of input features for each input
             out_features: number of output features
             weight_init_func: function to initialize the weights
             bias_init_func: function to initialize the bias
             key: key for the random number generator
 
         Example:
-            # Bilinear layer
+            >>> # Bilinear layer
             >>> layer = Multilinear((5,6), 7)
             >>> layer(jnp.ones((1,5)), jnp.ones((1,6))).shape
             (1, 7)
 
-            # Trilinear layer
+            >>> # Trilinear layer
             >>> layer = Multilinear((5,6,7), 8)
             >>> layer(jnp.ones((1,5)), jnp.ones((1,6)), jnp.ones((1,7))).shape
             (1, 8)
-
-            * Use with lazy initialization
-            >>> x = jnp.linspace(0, 1, 100)[:, None]
-            >>> lhs = Multilinear(None, 10)
-            >>> assert lhs(x, x, x).shape == (100, 10)
-            # here a trilinear layer is created with in_features=(1, 1, 1)
-            # with weight shape (1, 1, 1, 10) and bias shape (10,)
         """
-        if (
-            any([i is None for i in in_features])
-            if isinstance(in_features, Sequence)
-            else (in_features is None)
-        ):
-            for field_item in dataclasses.fields(self):
-                setattr(self, field_item.name, None)
-
-            self._partial_init = ft.partial(
-                Multilinear.__init__,
-                self,
-                out_features=out_features,
-                weight_init_func=weight_init_func,
-                bias_init_func=bias_init_func,
-                key=key,
-            )
-            return
-
-        if hasattr(self, "_partial_init"):
-            delattr(self, "_partial_init")
-
         if not isinstance(in_features, (tuple, int)):
             msg = f"Expected tuple or int for in_features, got {type(in_features)}"
             raise ValueError(msg)
 
         self.in_features = in_features
         self.out_features = out_features
 
-        self.weight_init_func = _check_and_return_init_func(
-            weight_init_func, "weight_init_func"
-        )
-        self.bias_init_func = _check_and_return_init_func(
-            bias_init_func, "bias_init_func"
-        )
+        self.weight_init_func = init_func_cb(weight_init_func)
+        self.bias_init_func = init_func_cb(bias_init_func)
 
         weight_shape = (*self.in_features, out_features)
         self.weight = self.weight_init_func(key, weight_shape)
 
         if self.bias_init_func is None:
             self.bias = None
         else:
             self.bias = self.bias_init_func(key, (out_features,))
 
-    def __call__(self, *x, **kwargs) -> jnp.ndarray:
-        if hasattr(self, "_partial_init"):
-            if any(isinstance(xi, jax.core.Tracer) for xi in x):
-                raise ValueError(_TRACER_ERROR_MSG(self.__class__.__name__))
-            self._partial_init(in_features=tuple(xi.shape[-1] for xi in x))
-
+    def __call__(self, *x, **k) -> jax.Array:
         einsum_string = _multilinear_einsum_string(len(self.in_features))
         x = jnp.einsum(einsum_string, *x, self.weight)
 
         if self.bias is None:
             return x
         return x + self.bias
 
 
-@pytc.treeclass
 class Linear(Multilinear):
     """Linear layer with 1 input applied to last axis of input
 
     Args:
         in_features: number of input features
         out_features: number of output features
         weight_init_func: function to initialize the weights
         bias_init_func: function to initialize the bias
         key: key for the random number generator
 
     Example:
         >>> layer = Linear(5, 6)
         >>> layer(jnp.ones((1,5))).shape
         (1, 6)
-
-        * Use with lazy initialization
-        >>> x = jnp.linspace(0, 1, 100)[:, None]
-        >>> lhs = Linear(None, 10)
-        >>> assert lhs(x).shape == (100, 10)
-        # here a linear layer is created with in_features=1
-        # with weight shape (1, 10) and bias shape (10,)
     """
 
     def __init__(
         self,
-        in_features: int | None,
+        in_features: int,
         out_features: int,
         *,
-        weight_init_func: str | Callable = "he_normal",
-        bias_init_func: str | Callable = "ones",
-        key: jr.PRNGKey = jr.PRNGKey(0),
+        weight_init_func: InitFuncType = "he_normal",
+        bias_init_func: InitFuncType = "ones",
+        key: jr.KeyArray = jr.PRNGKey(0),
     ):
         super().__init__(
             (in_features,),
             out_features,
             weight_init_func=weight_init_func,
             bias_init_func=bias_init_func,
             key=key,
         )
 
-    def __call__(self, x: jnp.ndarray, **kwargs) -> jnp.ndarray:
-        return super().__call__(x, **kwargs)
 
-
-@pytc.treeclass
 class Bilinear(Multilinear):
     def __init__(
         self,
-        in1_features: int | None,
-        in2_features: int | None,
+        in1_features: int,
+        in2_features: int,
         out_features: int,
         *,
-        weight_init_func: str | Callable = "he_normal",
-        bias_init_func: str | Callable = "ones",
-        key: jr.PRNGKey = jr.PRNGKey(0),
+        weight_init_func: InitFuncType = "he_normal",
+        bias_init_func: InitFuncType = "ones",
+        key: jr.KeyArray = jr.PRNGKey(0),
     ):
         """Bilinear layer
 
         Args:
             in1_features: number of input features for the first input
             in2_features: number of input features for the second input
             out_features: number of output features
@@ -195,32 +193,31 @@
             out_features,
             weight_init_func=weight_init_func,
             bias_init_func=bias_init_func,
             key=key,
         )
 
 
-@pytc.treeclass
-class GeneralLinear:
-    weight: jnp.ndarray
-    bias: jnp.ndarray
-
-    in_features: tuple[int, ...] | None = pytc.nondiff_field()
-    out_features: tuple[int, ...] | None = pytc.nondiff_field()
-    in_axes: tuple[int, ...] | None = pytc.nondiff_field()
+class GeneralLinear(pytc.TreeClass):
+    weight: jax.Array
+    bias: jax.Array
+
+    in_features: tuple[int, ...] = pytc.field(callbacks=[isinstance_factory(tuple)])
+    out_features: tuple[int, ...]
+    in_axes: tuple[int, ...] = pytc.field(callbacks=[isinstance_factory(tuple)])
 
     def __init__(
         self,
-        in_features: tuple[int, ...] | None,
+        in_features: tuple[int, ...],
         out_features: int,
         *,
         in_axes: tuple[int, ...],
-        weight_init_func: str | Callable = "he_normal",
-        bias_init_func: str | Callable = "ones",
-        key: jr.PRNGKey = jr.PRNGKey(0),
+        weight_init_func: InitFuncType = "he_normal",
+        bias_init_func: InitFuncType = "ones",
+        key: jr.KeyArray = jr.PRNGKey(0),
     ):
         """Apply a Linear Layer to input at in_axes
 
         Args:
             in_features: number of input features corresponding to in_axes
             out_features: number of output features
             in_axes: axes to apply the linear layer to
@@ -233,83 +230,126 @@
             >>> layer = GeneralLinear(in_features=(1, 2), in_axes=(0, 1), out_features=5)
             >>> assert layer(x).shape == (3, 4, 5)
 
         Note:
             This layer is similar to to flax linen's DenseGeneral, the difference is that
             this layer uses einsum to apply the linear layer to the specified axes.
         """
-        if in_axes is None:
-            raise ValueError("in_axes must be specified for GeneralLinear")
-
-        if (
-            any([i is None for i in in_features])
-            if isinstance(in_features, Sequence)
-            else (in_features is None)
-        ):
-            for field_item in dataclasses.fields(self):
-                setattr(self, field_item.name, None)
-            self.in_axes = in_axes
-            self._partial_init = ft.partial(
-                GeneralLinear.__init__,
-                self,
-                in_axes=in_axes,
-                out_features=out_features,
-                weight_init_func=weight_init_func,
-                bias_init_func=bias_init_func,
-                key=key,
-            )
-            return
-
-        if hasattr(self, "_partial_init"):
-            delattr(self, "_partial_init")
-
-        if not isinstance(in_features, tuple):
-            raise ValueError(
-                f"Expected in_features to be tuple, got {type(in_features)}"
-            )
-
-        if not isinstance(in_axes, tuple):
-            raise ValueError(f"Expected in_axes to be tuple, got {type(in_axes)}")
-
-        if len(in_axes) != len(in_features):
-            raise ValueError(
-                f"Expected in_axes and in_features to have the same length, got {len(in_axes)} and {len(in_features)}"
-            )
 
         self.in_features = in_features
         self.out_features = out_features
         self.in_axes = in_axes
-        self.weight_init_func = _check_and_return_init_func(
-            weight_init_func, "weight_init_func"
-        )
-        self.bias_init_func = _check_and_return_init_func(
-            bias_init_func, "bias_init_func"
-        )
 
+        if len(in_axes) != len(in_features):
+            msg = "Expected in_axes and in_features to have the same length,"
+            msg += f"got {len(in_axes)} and {len(in_features)}"
+            raise ValueError(msg)
+
+        self.weight_init_func = init_func_cb(weight_init_func)
+        self.bias_init_func = init_func_cb(bias_init_func)
         self.weight = self.weight_init_func(key, (*self.in_features, self.out_features))
 
         if self.bias_init_func is None:
             self.bias = None
         else:
             self.bias = self.bias_init_func(key, (self.out_features,))
 
-    def __call__(self, x: jnp.ndarray, **kwargs) -> jnp.ndarray:
-        if hasattr(self, "_partial_init"):
-            if isinstance(x, jax.core.Tracer):
-                raise ValueError(_TRACER_ERROR_MSG(self.__class__.__name__))
-
-            in_features = tuple(x.shape[i] for i in self.in_axes)
-            self._partial_init(in_features=in_features)
-
+    def __call__(self, x: jax.Array, **k) -> jax.Array:
         # ensure negative axes
         axes = map(lambda i: i if i < 0 else i - x.ndim, self.in_axes)
         einsum_string = _general_linear_einsum_string(*axes)
         x = jnp.einsum(einsum_string, x, self.weight)
         return x
 
 
-@pytc.treeclass
-class Identity:
+class Identity(pytc.TreeClass):
     """Identity layer"""
 
-    def __call__(self, x: jnp.ndarray, **kwargs) -> jnp.ndarray:
+    def __call__(self, x: jax.Array, **k) -> jax.Array:
         return x
+
+
+class Embedding(pytc.TreeClass):
+    in_features: int = pytc.field(callbacks=[positive_int_cb])
+    out_features: int = pytc.field(callbacks=[positive_int_cb])
+    weight: jax.Array
+
+    def __init__(
+        self,
+        in_features: int,
+        out_features: int,
+        key: jr.KeyArray = jr.PRNGKey(0),
+    ):
+        """Defines an embedding layer.
+
+        Args:
+            in_features: vocabulary size.
+            out_features: embedding size.
+            key: random key to initialize the weights.
+
+        Example:
+            >>> import serket as sk
+            >>> # 10 words in the vocabulary, each word is represented by a 3 dimensional vector
+            >>> table = sk.nn.Embedding(10,3)
+            >>> # take the last word in the vocab
+            >>> table(jnp.array([9]))
+            Array([[0.43810904, 0.35078037, 0.13254273]], dtype=float32)
+        """
+        self.in_features = in_features
+        self.out_features = out_features
+        self.weight = jr.uniform(key, (self.in_features, self.out_features))
+
+    def __call__(self, x: jax.Array, **k) -> jax.Array:
+        """Embeds the input.
+
+        Args:
+            x: integer index array of subdtype integer.
+
+        Returns:
+            Embedding of the input.
+
+        """
+        if not jnp.issubdtype(x.dtype, jnp.integer):
+            raise TypeError("Input must be an integer array.")
+
+        return jnp.take(self.weight, x, axis=0)
+
+
+class MergeLinear(pytc.TreeClass):
+    weight: jax.Array
+    bias: jax.Array
+
+    def __init__(self, *layers: tuple[Linear, ...]):
+        """Merge multiple linear layers with the same `out_features`.
+
+        Args:
+            layers: linear layers to merge
+
+        Example:
+            >>> import serket as sk
+            >>> import numpy.testing as npt
+            >>> layer1 = sk.nn.Linear(5, 6)  # 5 input features, 6 output features
+            >>> layer2 = sk.nn.Linear(7, 6)  # 7 input features, 6 output features
+            >>> merged_layer = sk.nn.MergeLinear(layer1, layer2)  # 12 input features, 6 output features
+            >>> x1 = jnp.ones([1, 5])  # 1 sample, 5 features
+            >>> x2 = jnp.ones([1, 7])  # 1 sample, 7 features
+            >>> y = merged_layer(x1, x2)  # one matrix multiplication
+            >>> z = layer1(x1) + layer2(x2)  # two matrix multiplications
+            >>> npt.assert_allclose(y, z, atol=1e-6)
+
+        Note:
+            Use this layer to reduce the matrix multiplication operations in the forward pass.
+        """
+        out_dim0 = layers[0].out_features
+
+        for layer in layers[1:]:
+            if layer.out_features != out_dim0:
+                msg = "All layers must have the same output dimension."
+                msg += f" Got {out_dim0} and {layer.out_features}"
+                raise ValueError(msg)
+
+        self.weight = jnp.concatenate([L.weight for L in layers], axis=0)
+        self.bias = sum([L.bias for L in layers if L.bias_init_func])
+
+    def __call__(self, *xs: tuple[jax.Array, ...], **k) -> jax.Array:
+        xs = jnp.concatenate(xs, axis=-1)
+        return xs @ self.weight + self.bias
```

### Comparing `serket-0.0.9/serket/nn/normalization.py` & `serket-0.2.0b2/serket/nn/normalization.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,93 @@
 from __future__ import annotations
 
-import dataclasses
-import functools as ft
-
 import jax
 import jax.numpy as jnp
 import pytreeclass as pytc
 
-from serket.nn.utils import _TRACER_ERROR_MSG
+from serket.nn.callbacks import non_negative_scalar_cbs, positive_int_cb
 
 
-@pytc.treeclass
-class LayerNorm:
-    γ: jnp.ndarray = None
-    β: jnp.ndarray = None
+def layer_norm(
+    x: jax.Array,
+    *,
+    γ: jax.Array,
+    β: jax.Array,
+    ε: float,
+    normalized_shape: int | tuple[int],
+) -> jax.Array:
+    """Layer Normalization
+    See: https://nn.labml.ai/normalization/layer_norm/index.html
+    transform the input by scaling and shifting to have zero mean and unit variance.
+
+    Args:
+        x: input array
+        γ: scale
+        β: shift
+        ε: a value added to the denominator for numerical stability.
+        normalized_shape: the shape of the input to be normalized.
+    """
+    dims = tuple(range(len(x.shape) - len(normalized_shape), len(x.shape)))
+
+    μ = jnp.mean(x, axis=dims, keepdims=True)
+    σ_2 = jnp.var(x, axis=dims, keepdims=True)
+    x̂ = (x - μ) * jax.lax.rsqrt((σ_2 + ε))
+
+    if γ is not None and β is not None:
+        return x̂ * γ + β
+    return x̂
+
+
+def group_norm(
+    x: jax.Array,
+    *,
+    γ: jax.Array,
+    β: jax.Array,
+    ε: float,
+    in_features: int,
+    groups: int,
+) -> jax.Array:
+    """Group Normalization
+    See: https://nn.labml.ai/normalization/group_norm/index.html
+    transform the input by scaling and shifting to have zero mean and unit variance.
+
+    Args:
+        x: input array
+        γ: scale
+        β: shift
+        ε: a value added to the denominator for numerical stability.
+        in_features: number of input features
+        groups: number of groups to separate the channels into
+    """
+    if len(x.shape) <= 1:
+        raise ValueError("Input must have at least 2 dimensions")
+
+    # split channels into groups
+    xx = x.reshape(groups, in_features // groups, *x.shape[1:])
+    dims = tuple(range(1, x.ndim + 1))
+
+    μ = jnp.mean(xx, axis=dims, keepdims=True)
+    σ_2 = jnp.var(xx, axis=dims, keepdims=True)
+    x̂ = (xx - μ) * jax.lax.rsqrt((σ_2 + ε))
+    x̂ = x̂.reshape(*x.shape)
+
+    if γ is not None and β is not None:
+        γ = jnp.expand_dims(γ, axis=(dims[:-1]))
+        β = jnp.expand_dims(β, axis=(dims[:-1]))
+        x̂ = x̂ * γ + β
+    return x̂
+
+
+class LayerNorm(pytc.TreeClass):
+    γ: jax.Array = None
+    β: jax.Array = None
+    ε: float = pytc.field(callbacks=[*non_negative_scalar_cbs])
 
-    ε: float = pytc.nondiff_field()
-    affine: bool = pytc.nondiff_field()
-    normalized_shape: int | tuple[int] = pytc.nondiff_field()
+    affine: bool
+    normalized_shape: int | tuple[int]
 
     def __init__(
         self,
         normalized_shape: int | tuple[int, ...],
         *,
         eps: float = 1e-5,
         affine: bool = True,
@@ -39,41 +105,36 @@
             normalized_shape
             if isinstance(normalized_shape, tuple)
             else (normalized_shape,)
         )
         self.ε = eps
         self.affine = affine
 
-        if self.affine:
-            # make γ and β trainable
-            self.γ = jnp.ones(normalized_shape)
-            self.β = jnp.zeros(normalized_shape)
-
-    def __call__(self, x: jnp.ndarray, **kwargs) -> jnp.ndarray:
-
-        dims = tuple(range(len(x.shape) - len(self.normalized_shape), len(x.shape)))
-
-        μ = jnp.mean(x, axis=dims, keepdims=True)
-        σ_2 = jnp.var(x, axis=dims, keepdims=True)
-        x̂ = (x - μ) * jax.lax.rsqrt((σ_2 + self.ε))
-
-        x̂ = (x̂ * self.γ + self.β) if self.affine else x̂
-
-        return x̂
-
+        # make γ and β trainable
+        self.γ = jnp.ones(normalized_shape) if self.affine else None
+        self.β = jnp.zeros(normalized_shape) if self.affine else None
+
+    def __call__(self, x: jax.Array, **kwargs) -> jax.Array:
+        return layer_norm(
+            x,
+            γ=self.γ,
+            β=self.β,
+            ε=self.ε,
+            normalized_shape=self.normalized_shape,
+        )
 
-@pytc.treeclass
-class GroupNorm:
-    γ: jnp.ndarray = None
-    β: jnp.ndarray = None
 
-    in_features: int = pytc.nondiff_field()
-    groups: int = pytc.nondiff_field()
-    ε: float = pytc.nondiff_field()
-    affine: bool = pytc.nondiff_field()
+class GroupNorm(pytc.TreeClass):
+    γ: jax.Array = None
+    β: jax.Array = None
+    ε: float = pytc.field(callbacks=[*non_negative_scalar_cbs])
+
+    in_features: int = pytc.field(callbacks=[positive_int_cb])
+    groups: int = pytc.field(callbacks=[positive_int_cb])
+    affine: bool
 
     def __init__(
         self,
         in_features,
         *,
         groups: int,
         eps: float = 1e-5,
@@ -85,88 +146,56 @@
 
         Args:
             in_features : the shape of the input to be normalized.
             groups : number of groups to separate the channels into.
             eps : a value added to the denominator for numerical stability.
             affine : a boolean value that when set to True, this module has learnable affine parameters.
         """
-        if in_features is None:
-            for field_item in dataclasses.fields(self):
-                setattr(self, field_item.name, None)
-            self._partial_init = ft.partial(
-                GroupNorm.__init__,
-                self=self,
-                groups=groups,
-                eps=eps,
-                affine=affine,
-            )
-            return
-
-        if hasattr(self, "_partial_init"):
-            delattr(self, "_partial_init")
-
-        if in_features <= 0 or not isinstance(in_features, int):
-            raise ValueError("in_features must be a positive integer")
-
-        if groups <= 0 or not isinstance(groups, int):
-            raise ValueError("groups must be a positive integer")
-
-        if in_features % groups != 0:
-            raise ValueError(
-                f"in_features must be divisible by groups. Got {in_features} and {groups}"
-            )
-
-        self.ε = eps
-        self.affine = affine
+        # checked by callbacks
         self.in_features = in_features
         self.groups = groups
+        self.ε = eps
+        self.affine = affine
 
-        if self.affine:
-            # make γ and β trainable
-            self.γ = jnp.ones(self.in_features)
-            self.β = jnp.zeros(self.in_features)
-
-    def __call__(self, x: jnp.ndarray, **kwargs) -> jnp.ndarray:
-        if hasattr(self, "_partial_init"):
-            if isinstance(x, jax.core.Tracer):
-                raise ValueError(_TRACER_ERROR_MSG(self.__class__.__name__))
-            self._partial_init(in_features=x.shape[0])
-
-        assert len(x.shape) > 1, "Input must have at least 2 dimensions"
-        # split channels into groups
-        xx = x.reshape(self.groups, self.in_features // self.groups, *x.shape[1:])
-        dims = tuple(range(1, x.ndim + 1))
-
-        μ = jnp.mean(xx, axis=dims, keepdims=True)
-        σ_2 = jnp.var(xx, axis=dims, keepdims=True)
-        x̂ = (xx - μ) * jax.lax.rsqrt((σ_2 + self.ε))
-        x̂ = x̂.reshape(*x.shape)
-
-        if self.affine:
-            γ = jnp.expand_dims(self.γ, axis=(dims[:-1]))
-            β = jnp.expand_dims(self.β, axis=(dims[:-1]))
-            x̂ = x̂ * γ + β
-        return x̂
+        # needs more info for checking
+        if in_features % groups != 0:
+            msg = f"in_features must be divisible by groups. Got {in_features} and {groups}"
+            raise ValueError(msg)
+
+        # make γ and β trainable
+        self.γ = jnp.ones(self.in_features) if self.affine else None
+        self.β = jnp.zeros(self.in_features) if self.affine else None
+
+    def __call__(self, x: jax.Array, **k) -> jax.Array:
+        return group_norm(
+            x=x,
+            γ=self.γ,
+            β=self.β,
+            ε=self.ε,
+            in_features=self.in_features,
+            groups=self.groups,
+        )
 
 
-@pytc.treeclass
 class InstanceNorm(GroupNorm):
     def __init__(
         self,
         in_features: int,
         *,
-        groups: int = 1,
         eps: float = 1e-5,
         affine: bool = True,
     ):
         """Instance Normalization
         See: https://nn.labml.ai/normalization/instance_norm/index.html
         transform the input by scaling and shifting to have zero mean and unit variance.
 
         Args:
             in_features : the shape of the input to be normalized.
             eps : a value added to the denominator for numerical stability.
             affine : a boolean value that when set to True, this module has learnable affine parameters.
         """
         super().__init__(
-            in_features=in_features, groups=in_features, eps=eps, affine=affine
+            in_features=in_features,
+            groups=in_features,
+            eps=eps,
+            affine=affine,
         )
```

### Comparing `serket-0.0.9/serket/nn/preprocessing.py` & `serket-0.2.0b2/serket/nn/preprocessing.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,51 +2,50 @@
 
 import functools as ft
 
 import jax
 import jax.numpy as jnp
 import pytreeclass as pytc
 
+from serket.nn.callbacks import positive_int_cb, validate_spatial_in_shape
+
 
 @ft.partial(jax.jit, static_argnums=(1,))
-def _histeq(x, bins_count: int = 256):
+def histeq(x, bins_count: int = 256):
     hist, bins = jnp.histogram(x.flatten(), bins_count, density=True)
     cdf = hist.cumsum()
     cdf = (bins_count - 1) * cdf / cdf[-1]
     return jnp.interp(x.flatten(), bins[:-1], cdf).reshape(x.shape)
 
 
-@pytc.treeclass
-class HistogramEqualization2D:
-    bins: int = pytc.nondiff_field()
+class HistogramEqualization2D(pytc.TreeClass):
+    bins: int = pytc.field(callbacks=[positive_int_cb])
 
     def __init__(self, bins: int = 256):
         """Apply histogram equalization to 2D spatial array channel wise
         Args:
             bins: number of bins. Defaults to 256.
 
         Note:
-            See:
             https://en.wikipedia.org/wiki/Histogram_equalization
             http://www.janeriksolem.net/histogram-equalization-with-python-and.html
             https://scikit-image.org/docs/stable/api/skimage.exposure.html#skimage.exposure.equalize_hist
             https://stackoverflow.com/questions/28518684/histogram-equalization-of-grayscale-images-with-numpy
         """
+        self.spatial_ndim = 2
         self.bins = bins
 
-    def __call__(self, x: jnp.ndarray, **kwargs) -> jnp.ndarray:
-        msg = f"Input must have 3 dimensions, got {x.ndim}."
-        assert x.ndim == 3, msg
-        return _histeq(x, self.bins)
+    @ft.partial(validate_spatial_in_shape, attribute_name="spatial_ndim")
+    def __call__(self, x: jax.Array, **k) -> jax.Array:
+        return histeq(x, self.bins)
 
 
-@pytc.treeclass
-class PixelShuffle:
+class PixelShuffle2D(pytc.TreeClass):
     def __init__(self, upscale_factor: int | tuple[int, int] = 1):
-
+        self.spatial_ndim = 2
         if isinstance(upscale_factor, int):
             if upscale_factor < 1:
                 raise ValueError("upscale_factor must be >= 1")
 
             self.upscale_factor = (upscale_factor, upscale_factor)
 
         elif isinstance(upscale_factor, tuple):
@@ -55,23 +54,23 @@
             if upscale_factor[0] < 1 or upscale_factor[1] < 1:
                 raise ValueError("upscale_factor must be >= 1")
             self.upscale_factor = upscale_factor
 
         else:
             raise ValueError("upscale_factor must be an integer or tuple of length 2")
 
-    def __call__(self, x: jnp.ndarray, **kwargs):
-        msg = f"Input must have 3 dimensions, got {x.ndim}."
-        assert x.ndim == 3, msg
+    @ft.partial(validate_spatial_in_shape, attribute_name="spatial_ndim")
+    def __call__(self, x: jax.Array, **k):
         channels = x.shape[0]
 
         sr, sw = self.upscale_factor
         oc = channels // (sr * sw)
 
-        msg = f"Input channels must be divisible by {sr*sw}, got {channels}."
-        assert channels % (sr * sw) == 0, msg
+        if not (channels % (sr * sw)) == 0:
+            msg = f"Input channels must be divisible by {sr*sw}, got {channels}."
+            raise ValueError(msg)
 
         ih, iw = x.shape[1], x.shape[2]
         x = jnp.reshape(x, (sr, sw, oc, ih, iw))
         x = jnp.transpose(x, (2, 3, 0, 4, 1))
         x = jnp.reshape(x, (oc, ih * sr, iw * sw))
         return x
```

### Comparing `serket-0.0.9/serket/nn/random_transform.py` & `serket-0.2.0b2/serket/nn/random_transform.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,106 +1,92 @@
 from __future__ import annotations
 
-import jax.numpy as jnp
+from typing import Any
+
+import jax
 import jax.random as jr
 import pytreeclass as pytc
+from jax.lax import stop_gradient
 
+from serket.nn.callbacks import range_cb_factory
 from serket.nn.crop import RandomCrop2D
 from serket.nn.padding import Pad2D
 from serket.nn.resize import Resize2D
 
 
-@pytc.treeclass
-class RandomApply:
-    layer: int
-    p: float = pytc.nondiff_field()
-    eval: bool | None
-
-    def __init__(self, layer, p: float = 0.5, ndim: int = 1, eval: bool | None = None):
-        """
-        Randomly applies a layer with probability p.
-
-        Args:
-            p: probability of applying the layer
-
-        Example:
-            >>> layer = RandomApply(sk.nn.MaxPool2D(kernel_size=2, strides=2), p=0.0)
-            >>> layer(jnp.ones((1, 10, 10))).shape
-            (1, 10, 10)
-
-            >>> layer = RandomApply(sk.nn.MaxPool2D(kernel_size=2, strides=2), p=1.0)
-            >>> layer(jnp.ones((1, 10, 10))).shape
-            (1, 5, 5)
-
-        Note:
-            See: https://pytorch.org/vision/main/_modules/torchvision/transforms/transforms.html#RandomApply
-            Use sk.nn.Sequential to apply multiple layers.
-        """
-
-        if p < 0 or p > 1:
-            raise ValueError(f"p must be between 0 and 1, got {p}")
-
-        if isinstance(eval, bool) or eval is None:
-            self.eval = eval
-        else:
-            raise ValueError(f"eval must be a boolean or None, got {eval}")
-
-        self.p = p
+class RandomApply(pytc.TreeClass):
+    """
+    Randomly applies a layer with probability p.
+
+    Args:
+        layer: layer to apply.
+        p: probability of applying the layer
+
+    Example:
+        >>> layer = RandomApply(sk.nn.MaxPool2D(kernel_size=2, strides=2), p=0.0)
+        >>> layer(jnp.ones((1, 10, 10))).shape
+        (1, 10, 10)
+
+        >>> layer = RandomApply(sk.nn.MaxPool2D(kernel_size=2, strides=2), p=1.0)
+        >>> layer(jnp.ones((1, 10, 10))).shape
+        (1, 5, 5)
+
+    Note:
+        https://pytorch.org/vision/main/_modules/torchvision/transforms/transforms.html#RandomApply
+        Use sk.nn.Sequential to apply multiple layers.
+    """
 
-        if not pytc.is_treeclass(layer):
-            raise ValueError("Layer must be a `treeclass`.")
-        self.layer = layer
+    layer: Any
+    p: float = pytc.field(default=0.5, callbacks=[range_cb_factory(0, 1)])
 
-    def __call__(self, x: jnp.ndarray, key: jr.PRNGKey = jr.PRNGKey(0)):
-
-        if self.eval is True or not jr.bernoulli(key, (self.p)):
+    def __call__(self, x: jax.Array, key: jr.KeyArray = jr.PRNGKey(0)):
+        if not jr.bernoulli(key, stop_gradient(self.p)):
             return x
 
         return self.layer(x)
 
 
-@pytc.treeclass
-class RandomZoom2D:
+class RandomZoom2D(pytc.TreeClass):
     def __init__(
         self,
         height_factor: tuple[float, float] = (0.0, 1.0),
         width_factor: tuple[float, float] = (0.0, 1.0),
     ):
         """
         Args:
             height_factor: (min, max)
             width_factor: (min, max)
 
         Note:
-            See: https://www.tensorflow.org/api_docs/python/tf/keras/layers/RandomZoom
+            https://www.tensorflow.org/api_docs/python/tf/keras/layers/RandomZoom
             Positive values are zoom in, negative values are zoom out.
         """
-        assert (
-            isinstance(height_factor, tuple) and len(height_factor) == 2
-        ), "height_factor must be a tuple of length 2"
-
-        assert (
-            isinstance(width_factor, tuple) and len(width_factor) == 2
-        ), "width_factor must be a tuple of length 2"
+        if not (isinstance(height_factor, tuple) and len(height_factor) == 2):
+            raise ValueError("height_factor must be a tuple of length 2")
+
+        if not (isinstance(width_factor, tuple) and len(width_factor) == 2):
+            raise ValueError("width_factor must be a tuple of length 2")
 
         self.height_factor = height_factor
         self.width_factor = width_factor
 
-    def __call__(self, x: jnp.ndarray, key: jr.PRNGKey = jr.PRNGKey(0)) -> jnp.ndarray:
-
+    def __call__(self, x: jax.Array, key: jr.KeyArray = jr.PRNGKey(0)) -> jax.Array:
         keys = jr.split(key, 4)
 
         height_factor = jr.uniform(
             keys[0],
             shape=(),
             minval=self.height_factor[0],
             maxval=self.height_factor[1],
         )
         width_factor = jr.uniform(
-            keys[1], shape=(), minval=self.width_factor[0], maxval=self.width_factor[1]
+            keys[1],
+            shape=(),
+            minval=self.width_factor[0],
+            maxval=self.width_factor[1],
         )
 
         R, C = x.shape[1:3]  # R = rows, C = cols
         RR, CC = int(R * (1 + height_factor))  # RR = resized rows,
         CC = int(C * (1 + width_factor))  # CC = resized cols
 
         if height_factor > 0:
```

### Comparing `serket-0.0.9/serket/nn/recurrent.py` & `serket-0.2.0b2/serket/nn/recurrent.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,779 +1,861 @@
 from __future__ import annotations
 
-import dataclasses
 import functools as ft
-from typing import Callable
+from typing import Any, Callable
 
 import jax
 import jax.numpy as jnp
 import jax.random as jr
 import pytreeclass as pytc
 
-from serket.nn import Linear
-from serket.nn.convolution import ConvND, SeparableConvND
-from serket.nn.utils import _TRACER_ERROR_MSG, _act_func_map
+import serket as sk
+from serket.nn.callbacks import (
+    positive_int_cb,
+    validate_in_features,
+    validate_spatial_in_shape,
+)
+from serket.nn.utils import (
+    _ACT_FUNC_MAP,
+    ActivationType,
+    DilationType,
+    InitFuncType,
+    KernelSizeType,
+    PaddingType,
+    StridesType,
+)
 
-# --------------------------------------------------- RNN ------------------------------------------------------------ #
+"""Defines RNN related classes."""
 
 
-@pytc.treeclass
-class RNNState:
-    hidden_state: jnp.ndarray
+# =============================================== Non Spatial RNN ==================================================== #
 
 
-@pytc.treeclass
-class RNNCell:
-    pass
+class RNNState(pytc.TreeClass):
+    hidden_state: jax.Array
 
 
-@pytc.treeclass
-class SpatialRNNCell:
-    pass
+class RNNCell(pytc.TreeClass):
+    ...
+
+
+class NonSpatialRNNCell(RNNCell):
+    ...
 
 
-@pytc.treeclass
 class SimpleRNNState(RNNState):
-    pass
+    ...
 
 
-@pytc.treeclass
-class SimpleRNNCell(RNNCell):
-    in_to_hidden: Linear
-    hidden_to_hidden: Linear
+class SimpleRNNCell(NonSpatialRNNCell):
+    in_features: int = pytc.field(callbacks=[positive_int_cb])
+    hidden_features: int = pytc.field(callbacks=[positive_int_cb])
 
     def __init__(
         self,
         in_features: int,
         hidden_features: int,
         *,
-        weight_init_func: str | Callable = "glorot_uniform",
-        bias_init_func: str | Callable | None = "zeros",
-        recurrent_weight_init_func: str | Callable = "orthogonal",
-        act_func: str | None = "tanh",
-        key: jr.PRNGKey = jr.PRNGKey(0),
+        weight_init_func: InitFuncType = "glorot_uniform",
+        bias_init_func: InitFuncType = "zeros",
+        recurrent_weight_init_func: InitFuncType = "orthogonal",
+        act_func: ActivationType = jax.nn.tanh,
+        key: jr.KeyArray = jr.PRNGKey(0),
     ):
         """Vanilla RNN cell that defines the update rule for the hidden state
-        See:
-            https://www.tensorflow.org/api_docs/python/tf/keras/layers/SimpleRNNCell
 
         Args:
             in_features: the number of input features
             hidden_features: the number of hidden features
             weight_init_func: the function to use to initialize the weights
             bias_init_func: the function to use to initialize the bias
             recurrent_weight_init_func: the function to use to initialize the recurrent weights
             act_func: the activation function to use for the hidden state update
             key: the key to use to initialize the weights
-        """
-        if in_features is None:
-            for field_item in dataclasses.fields(self):
-                # set all fields to None to mark the class as uninitialized
-                # to the user and to avoid errors
-                setattr(self, field_item.name, None)
-
-            self._partial_init = ft.partial(
-                SimpleRNNCell.__init__,
-                self=self,
-                hidden_features=hidden_features,
-                weight_init_func=weight_init_func,
-                bias_init_func=bias_init_func,
-                recurrent_weight_init_func=recurrent_weight_init_func,
-                act_func=act_func,
-                key=key,
-            )
-            return
 
-        if hasattr(self, "_partial_init"):
-            delattr(self, "_partial_init")
+        Example:
+            >>> cell = SimpleRNNCell(10, 20) # 10-dimensional input, 20-dimensional hidden state
+            >>> rnn_state = cell.init_state()  # 20-dimensional hidden state
+            >>> x = jnp.ones((10,)) # 10 features
+            >>> result = cell(x, rnn_state)
+            >>> result.hidden_state.shape  # 20 features
 
+        Note:
+            https://www.tensorflow.org/api_docs/python/tf/keras/layers/SimpleRNNCell.
+        """
         k1, k2 = jr.split(key, 2)
 
-        if not isinstance(in_features, int) or in_features < 1:
-            raise ValueError(
-                f"Expected in_features to be a positive integer, got {in_features}"
-            )
-
-        if not isinstance(hidden_features, int) or hidden_features < 1:
-            raise ValueError(
-                f"Expected hidden_features to be a positive integer, got {hidden_features}"
-            )
-
-        self.act_func = _act_func_map[act_func]
-
         self.in_features = in_features
         self.hidden_features = hidden_features
+        self.act_func = _ACT_FUNC_MAP.get(act_func, act_func)
 
-        self.in_to_hidden = Linear(
+        in_to_hidden = sk.nn.Linear(
             in_features,
             hidden_features,
             weight_init_func=weight_init_func,
             bias_init_func=bias_init_func,
             key=k1,
         )
 
-        self.hidden_to_hidden = Linear(
+        hidden_to_hidden = sk.nn.Linear(
             hidden_features,
             hidden_features,
             weight_init_func=recurrent_weight_init_func,
             bias_init_func=None,
             key=k2,
         )
 
-    def __call__(
-        self, x: jnp.ndarray, state: SimpleRNNState, **kwargs
-    ) -> SimpleRNNState:
-        if hasattr(self, "_partial_init"):
-            if isinstance(x, jax.core.Tracer):
-                raise ValueError(_TRACER_ERROR_MSG(self.__class__.__name__))
-            self._partial_init(in_features=x.shape[0])
+        self.in_and_hidden_to_hidden = sk.nn.MergeLinear(in_to_hidden, hidden_to_hidden)
+        self.spatial_ndim = 0
 
-        msg = f"Expected state to be an instance of SimpleRNNState, got {type(state)}"
-        assert isinstance(state, SimpleRNNState), msg
-        h = state.hidden_state
-        h = self.act_func(self.in_to_hidden(x) + self.hidden_to_hidden(h))
+    @ft.partial(validate_spatial_in_shape, attribute_name="spatial_ndim")
+    @ft.partial(validate_in_features, attribute_name="in_features")
+    def __call__(self, x: jax.Array, state: SimpleRNNState, **k) -> SimpleRNNState:
+        if not isinstance(state, SimpleRNNState):
+            msg = "Expected state to be an instance of `SimpleRNNState`"
+            msg += f", got {type(state).__name__}"
+            raise TypeError(msg)
+
+        h = self.act_func(self.in_and_hidden_to_hidden(x, state.hidden_state))
         return SimpleRNNState(h)
 
     def init_state(self) -> SimpleRNNState:
         shape = (self.hidden_features,)
         return SimpleRNNState(jnp.zeros(shape))
 
 
-@pytc.treeclass
 class LSTMState(RNNState):
-    cell_state: jnp.ndarray
+    cell_state: jax.Array
 
 
-@pytc.treeclass
-class LSTMCell(RNNCell):
-    in_to_hidden: Linear
-    hidden_to_hidden: Linear
+class LSTMCell(NonSpatialRNNCell):
+    in_features: int = pytc.field(callbacks=[positive_int_cb])
+    hidden_features: int = pytc.field(callbacks=[positive_int_cb])
 
     def __init__(
         self,
         in_features: int,
         hidden_features: int,
         *,
         weight_init_func: str | Callable = "glorot_uniform",
         bias_init_func: str | Callable | None = "zeros",
         recurrent_weight_init_func: str | Callable = "orthogonal",
-        act_func: str | None = "tanh",
-        recurrent_act_func: str | None = "sigmoid",
-        key: jr.PRNGKey = jr.PRNGKey(0),
+        act_func: str | Callable[[Any], Any] | None = "tanh",
+        recurrent_act_func: ActivationType | None = "sigmoid",
+        key: jr.KeyArray = jr.PRNGKey(0),
     ):
         """LSTM cell that defines the update rule for the hidden state and cell state
         Args:
             in_features: the number of input features
             hidden_features: the number of hidden features
             weight_init_func: the function to use to initialize the weights
             bias_init_func: the function to use to initialize the bias
             recurrent_weight_init_func: the function to use to initialize the recurrent weights
             act_func: the activation function to use for the hidden state update
             recurrent_act_func: the activation function to use for the cell state update
             key: the key to use to initialize the weights
 
-        See:
+        Note:
             https://www.tensorflow.org/api_docs/python/tf/keras/layers/LSTMCell
             https://github.com/deepmind/dm-haiku/blob/main/haiku/_src/recurrent.py
         """
-        if in_features is None:
-            for field_item in dataclasses.fields(self):
-                # set all fields to None to mark the class as uninitialized
-                # to the user and to avoid errors
-                setattr(self, field_item.name, None)
-
-            self._partial_init = ft.partial(
-                LSTMCell.__init__,
-                self=self,
-                hidden_features=hidden_features,
-                weight_init_func=weight_init_func,
-                bias_init_func=bias_init_func,
-                recurrent_weight_init_func=recurrent_weight_init_func,
-                act_func=act_func,
-                key=key,
-            )
-            return
-
-        if hasattr(self, "_partial_init"):
-            delattr(self, "_partial_init")
-
         k1, k2 = jr.split(key, 2)
 
-        if not isinstance(in_features, int) or in_features < 1:
-            raise ValueError(
-                f"Expected in_features to be a positive integer, got {in_features}"
-            )
-
-        if not isinstance(hidden_features, int) or hidden_features < 1:
-            raise ValueError(
-                f"Expected hidden_features to be a positive integer, got {hidden_features}"
-            )
-
-        self.act_func = _act_func_map[act_func]
-        self.recurrent_act_func = _act_func_map[recurrent_act_func]
-
         self.in_features = in_features
         self.hidden_features = hidden_features
+        self.act_func = _ACT_FUNC_MAP.get(act_func, act_func)
+        self.recurrent_act_func = _ACT_FUNC_MAP.get(
+            recurrent_act_func, recurrent_act_func
+        )
 
-        self.in_to_hidden = Linear(
+        in_to_hidden = sk.nn.Linear(
             in_features,
             hidden_features * 4,
             weight_init_func=weight_init_func,
             bias_init_func=bias_init_func,
             key=k1,
         )
 
-        self.hidden_to_hidden = Linear(
+        hidden_to_hidden = sk.nn.Linear(
             hidden_features,
             hidden_features * 4,
             weight_init_func=recurrent_weight_init_func,
             bias_init_func=None,
             key=k2,
         )
 
-    def __call__(self, x: jnp.ndarray, state: LSTMState, **kwargs) -> LSTMState:
-        if hasattr(self, "_partial_init"):
-            if isinstance(x, jax.core.Tracer):
-                raise ValueError(_TRACER_ERROR_MSG(self.__class__.__name__))
-            self._partial_init(in_features=x.shape[0])
+        self.in_and_hidden_to_hidden = sk.nn.MergeLinear(in_to_hidden, hidden_to_hidden)
+        self.spatial_ndim = 0
 
-        msg = f"Expected state to be an instance of LSTMState, got {type(state)}"
-        assert isinstance(state, LSTMState), msg
-        h, c = state.hidden_state, state.cell_state
+    @ft.partial(validate_spatial_in_shape, attribute_name="spatial_ndim")
+    @ft.partial(validate_in_features, attribute_name="in_features")
+    def __call__(self, x: jax.Array, state: LSTMState, **k) -> LSTMState:
+        if not isinstance(state, LSTMState):
+            msg = "Expected state to be an instance of `LSTMState`"
+            msg += f", got {type(state).__name__}"
+            raise TypeError(msg)
 
-        h = self.in_to_hidden(x) + self.hidden_to_hidden(h)
+        h, c = state.hidden_state, state.cell_state
+        h = self.in_and_hidden_to_hidden(x, h)
         i, f, g, o = jnp.split(h, 4, axis=-1)
         i = self.recurrent_act_func(i)
         f = self.recurrent_act_func(f)
         g = self.act_func(g)
         o = self.recurrent_act_func(o)
         c = f * c + i * g
         h = o * self.act_func(c)
         return LSTMState(h, c)
 
     def init_state(self) -> LSTMState:
         shape = (self.hidden_features,)
         return LSTMState(jnp.zeros(shape), jnp.zeros(shape))
 
 
-# ------------------------------------------------- Spatial RNN ------------------------------------------------------ #
-@pytc.treeclass
+class GRUState(RNNState):
+    ...
+
+
+class GRUCell(NonSpatialRNNCell):
+    in_features: int = pytc.field(callbacks=[positive_int_cb])
+    hidden_features: int = pytc.field(callbacks=[positive_int_cb])
+
+    def __init__(
+        self,
+        in_features: int,
+        hidden_features: int,
+        *,
+        weight_init_func: InitFuncType = "glorot_uniform",
+        bias_init_func: InitFuncType = "zeros",
+        recurrent_weight_init_func: InitFuncType = "orthogonal",
+        act_func: ActivationType | None = "tanh",
+        recurrent_act_func: ActivationType | None = "sigmoid",
+        key: jr.KeyArray = jr.PRNGKey(0),
+    ):
+        """GRU cell that defines the update rule for the hidden state and cell state
+        Args:
+            in_features: the number of input features
+            hidden_features: the number of hidden features
+            weight_init_func: the function to use to initialize the weights
+            bias_init_func: the function to use to initialize the bias
+            recurrent_weight_init_func: the function to use to initialize the recurrent weights
+            act_func: the activation function to use for the hidden state update
+            recurrent_act_func: the activation function to use for the cell state update
+            key: the key to use to initialize the weights
+
+        See:
+            https://keras.io/api/layers/recurrent_layers/gru/
+        """
+        k1, k2 = jr.split(key, 2)
+
+        self.in_features = in_features
+        self.hidden_features = hidden_features
+        self.act_func = _ACT_FUNC_MAP.get(act_func, act_func)
+        self.recurrent_act_func = _ACT_FUNC_MAP[recurrent_act_func]
+
+        self.in_to_hidden = sk.nn.Linear(
+            in_features,
+            hidden_features * 3,
+            weight_init_func=weight_init_func,
+            bias_init_func=bias_init_func,
+            key=k1,
+        )
+
+        self.hidden_to_hidden = sk.nn.Linear(
+            hidden_features,
+            hidden_features * 3,
+            weight_init_func=recurrent_weight_init_func,
+            bias_init_func=None,
+            key=k2,
+        )
+
+        self.spatial_ndim = 0
+
+    @ft.partial(validate_spatial_in_shape, attribute_name="spatial_ndim")
+    @ft.partial(validate_in_features, attribute_name="in_features")
+    def __call__(self, x: jax.Array, state: GRUState, **k) -> GRUState:
+        if not isinstance(state, GRUState):
+            msg = "Expected state to be an instance of `GRUState`"
+            msg += f", got {type(state).__name__}"
+            raise TypeError(msg)
+
+        h = state.hidden_state
+        xe, xu, xo = jnp.split(self.in_to_hidden(x), 3, axis=-1)
+        he, hu, ho = jnp.split(self.hidden_to_hidden(h), 3, axis=-1)
+        e = self.recurrent_act_func(xe + he)
+        u = self.recurrent_act_func(xu + hu)
+        o = self.act_func(xo + (e * ho))
+        h = (1 - u) * o + u * h
+        return GRUState(hidden_state=h)
+
+    def init_state(self) -> GRUState:
+        shape = (self.hidden_features,)
+        return GRUState(jnp.zeros(shape, dtype=jnp.float32))
+
+
+# =============================================== Spatial RNN ======================================================= #
+
+
+class SpatialRNNCell(RNNCell):
+    ...
+
+
+# ------------------------------------------------- ConvLSTM RNN ----------------------------------------------------- #
+
+
 class ConvLSTMNDState(RNNState):
-    cell_state: jnp.ndarray
+    cell_state: jax.Array
 
 
-@pytc.treeclass
 class ConvLSTMNDCell(SpatialRNNCell):
-    in_to_hidden: ConvND
-    hidden_to_hidden: ConvND
+    in_features: int = pytc.field(callbacks=[positive_int_cb])
+    hidden_features: int = pytc.field(callbacks=[positive_int_cb])
 
     def __init__(
         self,
         in_features: int,
-        out_features: int,
-        kernel_size: int | tuple[int, ...],
+        hidden_features: int,
+        kernel_size: KernelSizeType,
         *,
-        strides: int | tuple[int, ...] = 1,
-        padding: str | tuple[int, ...] | tuple[tuple[int, int], ...] = "SAME",
-        input_dilation: int | tuple[int, ...] = 1,
-        kernel_dilation: int | tuple[int, ...] = 1,
-        weight_init_func: str | Callable = "glorot_uniform",
-        bias_init_func: str | Callable | None = "zeros",
-        recurrent_weight_init_func: str | Callable = "orthogonal",
-        act_func: str | None = "tanh",
-        recurrent_act_func: str | None = "hard_sigmoid",
-        key: jr.PRNGKey = jr.PRNGKey(0),
-        ndim: int = 2,
+        strides: StridesType = 1,
+        padding: PaddingType = "SAME",
+        input_dilation: DilationType = 1,
+        kernel_dilation: DilationType = 1,
+        weight_init_func: InitFuncType = "glorot_uniform",
+        bias_init_func: InitFuncType = "zeros",
+        recurrent_weight_init_func: InitFuncType = "orthogonal",
+        act_func: ActivationType | None = "tanh",
+        recurrent_act_func: ActivationType | None = "hard_sigmoid",
+        key: jr.KeyArray = jr.PRNGKey(0),
+        conv_layer: Any = None,
+        spatial_ndim: int = 1,
     ):
         """Convolution LSTM cell that defines the update rule for the hidden state and cell state
         Args:
             in_features: Number of input features
-            out_features: Number of output features
+            hidden_features: Number of output features
             kernel_size: Size of the convolutional kernel
             strides: Stride of the convolution
             padding: Padding of the convolution
             input_dilation: Dilation of the input
             kernel_dilation: Dilation of the convolutional kernel
             weight_init_func: Weight initialization function
             bias_init_func: Bias initialization function
             recurrent_weight_init_func: Recurrent weight initialization function
             act_func: Activation function
             recurrent_act_func: Recurrent activation function
             key: PRNG key
-            ndim: Number of spatial dimensions
+            spatial_ndim: Number of spatial dimensions
 
         See: https://www.tensorflow.org/api_docs/python/tf/keras/layers/ConvLSTM1D
         """
-        if in_features is None:
-            for field_item in dataclasses.fields(self):
-                # set all fields to None to mark the class as uninitialized
-                # to the user and to avoid errors
-                setattr(self, field_item.name, None)
-
-            self._partial_init = ft.partial(
-                ConvLSTMNDCell.__init__,
-                self=self,
-                out_features=out_features,
-                kernel_size=kernel_size,
-                strides=strides,
-                padding=padding,
-                input_dilation=input_dilation,
-                kernel_dilation=kernel_dilation,
-                weight_init_func=weight_init_func,
-                bias_init_func=bias_init_func,
-                recurrent_weight_init_func=recurrent_weight_init_func,
-                act_func=act_func,
-                recurrent_act_func=recurrent_act_func,
-                ndim=ndim,
-                key=key,
-            )
-            return
-
-        if hasattr(self, "_partial_init"):
-            delattr(self, "_partial_init")
-
         k1, k2 = jr.split(key, 2)
 
-        if not isinstance(in_features, int) or in_features < 1:
-            raise ValueError(
-                f"Expected in_features to be a positive integer, got {in_features}"
-            )
-
-        if not isinstance(out_features, int) or out_features < 1:
-            raise ValueError(
-                f"Expected out_features to be a positive integer, got {out_features}"
-            )
-
-        self.act_func = _act_func_map[act_func]
-        self.recurrent_act_func = _act_func_map[recurrent_act_func]
         self.in_features = in_features
-        self.out_features = out_features
-        self.hidden_features = out_features
-        self.ndim = ndim
+        self.hidden_features = hidden_features
+        self.spatial_ndim = spatial_ndim
+        self.act_func = _ACT_FUNC_MAP.get(act_func, act_func)
+        self.recurrent_act_func = _ACT_FUNC_MAP.get(recurrent_act_func, recurrent_act_func)  # fmt: skip
 
-        self.in_to_hidden = ConvND(
+        self.in_to_hidden = conv_layer(
             in_features,
-            out_features * 4,
+            hidden_features * 4,
             kernel_size,
             strides=strides,
             padding=padding,
             input_dilation=input_dilation,
             kernel_dilation=kernel_dilation,
             weight_init_func=weight_init_func,
             bias_init_func=bias_init_func,
             key=k1,
-            ndim=ndim,
         )
 
-        self.hidden_to_hidden = ConvND(
-            out_features,
-            out_features * 4,
+        self.hidden_to_hidden = conv_layer(
+            hidden_features,
+            hidden_features * 4,
             kernel_size,
             strides=strides,
             padding=padding,
             input_dilation=input_dilation,
             kernel_dilation=kernel_dilation,
             weight_init_func=recurrent_weight_init_func,
             bias_init_func=None,
             key=k2,
-            ndim=ndim,
         )
 
-    def __call__(
-        self, x: jnp.ndarray, state: ConvLSTMNDState, **kwargs
-    ) -> ConvLSTMNDState:
-        if hasattr(self, "_partial_init"):
-            if isinstance(x, jax.core.Tracer):
-                raise ValueError(_TRACER_ERROR_MSG(self.__class__.__name__))
-            self._partial_init(in_features=x.shape[0])
+    @ft.partial(validate_spatial_in_shape, attribute_name="spatial_ndim")
+    @ft.partial(validate_in_features, attribute_name="in_features")
+    def __call__(self, x: jax.Array, state: ConvLSTMNDState, **k) -> ConvLSTMNDState:
+        if not isinstance(state, ConvLSTMNDState):
+            msg = f"Expected state to be an instance of ConvLSTMNDState, got {type(state)}"
+            raise TypeError(msg)
 
-        msg = f"Expected state to be an instance of ConvLSTMNDState, got {type(state)}"
-        assert isinstance(state, ConvLSTMNDState), msg
         h, c = state.hidden_state, state.cell_state
-
         h = self.in_to_hidden(x) + self.hidden_to_hidden(h)
         i, f, g, o = jnp.split(h, 4, axis=0)
         i = self.recurrent_act_func(i)
         f = self.recurrent_act_func(f)
         g = self.act_func(g)
         o = self.recurrent_act_func(o)
         c = f * c + i * g
         h = o * self.act_func(c)
         return ConvLSTMNDState(h, c)
 
     def init_state(self, spatial_dim: tuple[int, ...]) -> ConvLSTMNDState:
-        msg = f"Expected spatial_dim to be a tuple of length {self.ndim}, got {spatial_dim}"
-        assert len(spatial_dim) == self.ndim, msg
+        msg = f"Expected spatial_dim to be a tuple of length {self.spatial_ndim}, got {spatial_dim}"
+        assert len(spatial_dim) == self.spatial_ndim, msg
         shape = (self.hidden_features, *spatial_dim)
         return ConvLSTMNDState(jnp.zeros(shape), jnp.zeros(shape))
 
 
-@pytc.treeclass
 class ConvLSTM1DCell(ConvLSTMNDCell):
     def __init__(
         self,
-        in_features: int | None,
-        out_features: int,
-        kernel_size: int,
-        strides: int = 1,
-        padding: str = "same",
-        input_dilation: int = 1,
-        kernel_dilation: int = 1,
-        weight_init_func: str | Callable = "glorot_uniform",
-        bias_init_func: str | Callable | None = "zeros",
-        recurrent_weight_init_func: str | Callable = "orthogonal",
-        act_func: str | None = "tanh",
-        recurrent_act_func: str | None = "sigmoid",
-        key: jr.PRNGKey = jr.PRNGKey(0),
+        in_features: int,
+        hidden_features: int,
+        kernel_size: KernelSizeType,
+        *,
+        strides: StridesType = 1,
+        padding: PaddingType = "SAME",
+        input_dilation: DilationType = 1,
+        kernel_dilation: DilationType = 1,
+        weight_init_func: InitFuncType = "glorot_uniform",
+        bias_init_func: InitFuncType = "zeros",
+        recurrent_weight_init_func: InitFuncType = "orthogonal",
+        act_func: ActivationType | None = "tanh",
+        recurrent_act_func: ActivationType | None = "hard_sigmoid",
+        key: jr.KeyArray = jr.PRNGKey(0),
     ):
+        """1D Convolution LSTM cell that defines the update rule for the hidden state and cell state
+        Args:
+            in_features: Number of input features
+            hidden_features: Number of output features
+            kernel_size: Size of the convolutional kernel
+            strides: Stride of the convolution
+            padding: Padding of the convolution
+            input_dilation: Dilation of the input
+            kernel_dilation: Dilation of the convolutional kernel
+            weight_init_func: Weight initialization function
+            bias_init_func: Bias initialization function
+            recurrent_weight_init_func: Recurrent weight initialization function
+            act_func: Activation function
+            recurrent_act_func: Recurrent activation function
+            key: PRNG key
+            spatial_ndim: Number of spatial dimensions.
+
+        Note:
+            https://www.tensorflow.org/api_docs/python/tf/keras/layers/ConvLSTM1D
+        """
         super().__init__(
             in_features=in_features,
-            out_features=out_features,
+            hidden_features=hidden_features,
             kernel_size=kernel_size,
             strides=strides,
             padding=padding,
             input_dilation=input_dilation,
             kernel_dilation=kernel_dilation,
             weight_init_func=weight_init_func,
             bias_init_func=bias_init_func,
             recurrent_weight_init_func=recurrent_weight_init_func,
             act_func=act_func,
             recurrent_act_func=recurrent_act_func,
             key=key,
-            ndim=1,
+            conv_layer=sk.nn.Conv1D,
+            spatial_ndim=1,
         )
 
 
-@pytc.treeclass
 class ConvLSTM2DCell(ConvLSTMNDCell):
     def __init__(
         self,
-        in_features: int | None,
-        out_features: int,
-        kernel_size: int | tuple[int, int],
-        strides: int | tuple[int, int] = 1,
-        padding: str = "same",
-        input_dilation: int | tuple[int, int] = 1,
-        kernel_dilation: int | tuple[int, int] = 1,
-        weight_init_func: str | Callable = "glorot_uniform",
-        bias_init_func: str | Callable | None = "zeros",
-        recurrent_weight_init_func: str | Callable = "orthogonal",
-        act_func: str | None = "tanh",
-        recurrent_act_func: str | None = "sigmoid",
-        key: jr.PRNGKey = jr.PRNGKey(0),
+        in_features: int,
+        hidden_features: int,
+        kernel_size: KernelSizeType,
+        *,
+        strides: StridesType = 1,
+        padding: PaddingType = "SAME",
+        input_dilation: DilationType = 1,
+        kernel_dilation: DilationType = 1,
+        weight_init_func: InitFuncType = "glorot_uniform",
+        bias_init_func: InitFuncType = "zeros",
+        recurrent_weight_init_func: InitFuncType = "orthogonal",
+        act_func: ActivationType | None = "tanh",
+        recurrent_act_func: ActivationType | None = "hard_sigmoid",
+        key: jr.KeyArray = jr.PRNGKey(0),
     ):
+        """2D Convolution LSTM cell that defines the update rule for the hidden state and cell state
+        Args:
+            in_features: Number of input features
+            hidden_features: Number of output features
+            kernel_size: Size of the convolutional kernel
+            strides: Stride of the convolution
+            padding: Padding of the convolution
+            input_dilation: Dilation of the input
+            kernel_dilation: Dilation of the convolutional kernel
+            weight_init_func: Weight initialization function
+            bias_init_func: Bias initialization function
+            recurrent_weight_init_func: Recurrent weight initialization function
+            act_func: Activation function
+            recurrent_act_func: Recurrent activation function
+            key: PRNG key
+            spatial_ndim: Number of spatial dimensions.
+
+        Note:
+            https://www.tensorflow.org/api_docs/python/tf/keras/layers/ConvLSTM1D
+        """
         super().__init__(
             in_features=in_features,
-            out_features=out_features,
+            hidden_features=hidden_features,
             kernel_size=kernel_size,
             strides=strides,
             padding=padding,
             input_dilation=input_dilation,
             kernel_dilation=kernel_dilation,
             weight_init_func=weight_init_func,
             bias_init_func=bias_init_func,
             recurrent_weight_init_func=recurrent_weight_init_func,
             act_func=act_func,
             recurrent_act_func=recurrent_act_func,
             key=key,
-            ndim=2,
+            conv_layer=sk.nn.Conv2D,
+            spatial_ndim=2,
         )
 
 
-@pytc.treeclass
 class ConvLSTM3DCell(ConvLSTMNDCell):
     def __init__(
         self,
-        in_features: int | None,
-        out_features: int,
-        kernel_size: int | tuple[int, int, int],
-        strides: int | tuple[int, int, int] = 1,
-        padding: str = "same",
-        input_dilation: int | tuple[int, int, int] = 1,
-        kernel_dilation: int | tuple[int, int, int] = 1,
-        weight_init_func: str | Callable = "glorot_uniform",
-        bias_init_func: str | Callable | None = "zeros",
-        recurrent_weight_init_func: str | Callable = "orthogonal",
-        act_func: str | None = "tanh",
-        recurrent_act_func: str | None = "sigmoid",
-        key: jr.PRNGKey = jr.PRNGKey(0),
+        in_features: int,
+        hidden_features: int,
+        kernel_size: KernelSizeType,
+        *,
+        strides: StridesType = 1,
+        padding: PaddingType = "SAME",
+        input_dilation: DilationType = 1,
+        kernel_dilation: DilationType = 1,
+        weight_init_func: InitFuncType = "glorot_uniform",
+        bias_init_func: InitFuncType = "zeros",
+        recurrent_weight_init_func: InitFuncType = "orthogonal",
+        act_func: ActivationType | None = "tanh",
+        recurrent_act_func: ActivationType | None = "hard_sigmoid",
+        key: jr.KeyArray = jr.PRNGKey(0),
     ):
+        """3D Convolution LSTM cell that defines the update rule for the hidden state and cell state
+        Args:
+            in_features: Number of input features
+            hidden_features: Number of output features
+            kernel_size: Size of the convolutional kernel
+            strides: Stride of the convolution
+            padding: Padding of the convolution
+            input_dilation: Dilation of the input
+            kernel_dilation: Dilation of the convolutional kernel
+            weight_init_func: Weight initialization function
+            bias_init_func: Bias initialization function
+            recurrent_weight_init_func: Recurrent weight initialization function
+            act_func: Activation function
+            recurrent_act_func: Recurrent activation function
+            key: PRNG key
+            spatial_ndim: Number of spatial dimensions.
+
+        Note:
+            https://www.tensorflow.org/api_docs/python/tf/keras/layers/ConvLSTM1D
+        """
         super().__init__(
             in_features=in_features,
-            out_features=out_features,
+            hidden_features=hidden_features,
             kernel_size=kernel_size,
             strides=strides,
             padding=padding,
             input_dilation=input_dilation,
             kernel_dilation=kernel_dilation,
             weight_init_func=weight_init_func,
             bias_init_func=bias_init_func,
             recurrent_weight_init_func=recurrent_weight_init_func,
             act_func=act_func,
             recurrent_act_func=recurrent_act_func,
             key=key,
-            ndim=3,
+            conv_layer=sk.nn.Conv3D,
+            spatial_ndim=3,
         )
 
 
-@pytc.treeclass
-class SeparableConvLSTMNDState(RNNState):
-    cell_state: jnp.ndarray
+# ------------------------------------------------- ConvGRU RNN ------------------------------------------------------ #
+
+
+class ConvGRUNDState(RNNState):
+    ...
 
 
-@pytc.treeclass
-class SeparableConvLSTMNDCell(SpatialRNNCell):
-    in_to_hidden: SeparableConvND
-    hidden_to_hidden: SeparableConvND
+class ConvGRUNDCell(SpatialRNNCell):
+    in_features: int = pytc.field(callbacks=[positive_int_cb])
+    hidden_features: int = pytc.field(callbacks=[positive_int_cb])
 
     def __init__(
         self,
         in_features: int,
-        out_features: int,
+        hidden_features: int,
         kernel_size: int | tuple[int, ...],
         *,
-        strides: int | tuple[int, ...] = 1,
-        padding: str | tuple[int, ...] | tuple[tuple[int, int], ...] = "SAME",
-        weight_init_func: str | Callable = "glorot_uniform",
-        bias_init_func: str | Callable | None = "zeros",
-        recurrent_weight_init_func: str | Callable = "orthogonal",
-        act_func: str | None = "tanh",
-        recurrent_act_func: str | None = "hard_sigmoid",
-        key: jr.PRNGKey = jr.PRNGKey(0),
-        ndim: int = 2,
+        strides: StridesType = 1,
+        padding: PaddingType = "SAME",
+        input_dilation: DilationType = 1,
+        kernel_dilation: DilationType = 1,
+        weight_init_func: InitFuncType = "glorot_uniform",
+        bias_init_func: InitFuncType = "zeros",
+        recurrent_weight_init_func: InitFuncType = "orthogonal",
+        act_func: ActivationType | None = "tanh",
+        recurrent_act_func: ActivationType | None = "sigmoid",
+        key: jr.KeyArray = jr.PRNGKey(0),
+        conv_layer: Any = None,
+        spatial_ndim: int = 1,
     ):
-        """Separable Convolution LSTM cell that defines the update rule for the hidden state and cell state
+        """Convolution GRU cell that defines the update rule for the hidden state and cell state
         Args:
             in_features: Number of input features
-            out_features: Number of output features
+            hidden_features: Number of output features
             kernel_size: Size of the convolutional kernel
             strides: Stride of the convolution
             padding: Padding of the convolution
+            input_dilation: Dilation of the input
+            kernel_dilation: Dilation of the convolutional kernel
             weight_init_func: Weight initialization function
             bias_init_func: Bias initialization function
             recurrent_weight_init_func: Recurrent weight initialization function
             act_func: Activation function
             recurrent_act_func: Recurrent activation function
             key: PRNG key
-            ndim: Number of spatial dimensions
+            spatial_ndim: Number of spatial dimensions.
 
-        See: https://www.tensorflow.org/api_docs/python/tf/keras/layers/ConvLSTM1D
         """
-        if in_features is None:
-            for field_item in dataclasses.fields(self):
-                # set all fields to None to mark the class as uninitialized
-                # to the user and to avoid errors
-                setattr(self, field_item.name, None)
-
-            self._partial_init = ft.partial(
-                SeparableConvLSTMNDCell.__init__,
-                self=self,
-                out_features=out_features,
-                kernel_size=kernel_size,
-                strides=strides,
-                padding=padding,
-                weight_init_func=weight_init_func,
-                bias_init_func=bias_init_func,
-                recurrent_weight_init_func=recurrent_weight_init_func,
-                act_func=act_func,
-                recurrent_act_func=recurrent_act_func,
-                key=key,
-                ndim=ndim,
-            )
-            return
-
-        if hasattr(self, "_partial_init"):
-            delattr(self, "_partial_init")
-
         k1, k2 = jr.split(key, 2)
 
-        if not isinstance(in_features, int) or in_features < 1:
-            raise ValueError(
-                f"Expected in_features to be a positive integer, got {in_features}"
-            )
-
-        if not isinstance(out_features, int) or out_features < 1:
-            raise ValueError(
-                f"Expected out_features to be a positive integer, got {out_features}"
-            )
-
-        self.act_func = _act_func_map[act_func]
-        self.recurrent_act_func = _act_func_map[recurrent_act_func]
         self.in_features = in_features
-        self.out_features = out_features
-        self.hidden_features = out_features
-        self.ndim = ndim
+        self.hidden_features = hidden_features
+        self.spatial_ndim = spatial_ndim
+        self.act_func = _ACT_FUNC_MAP.get(act_func, act_func)
+        self.recurrent_act_func = _ACT_FUNC_MAP.get(recurrent_act_func, recurrent_act_func)  # fmt: skip
 
-        self.in_to_hidden = SeparableConvND(
+        self.in_to_hidden = conv_layer(
             in_features,
-            out_features * 4,
+            hidden_features * 3,
             kernel_size,
             strides=strides,
             padding=padding,
-            depth_multiplier=1,
-            depthwise_weight_init_func=weight_init_func,
-            pointwise_weight_init_func=weight_init_func,
-            pointwise_bias_init_func=bias_init_func,
+            input_dilation=input_dilation,
+            kernel_dilation=kernel_dilation,
+            weight_init_func=weight_init_func,
+            bias_init_func=bias_init_func,
             key=k1,
-            ndim=ndim,
         )
 
-        self.hidden_to_hidden = SeparableConvND(
-            out_features,
-            out_features * 4,
+        self.hidden_to_hidden = conv_layer(
+            hidden_features,
+            hidden_features * 3,
             kernel_size,
             strides=strides,
             padding=padding,
-            depth_multiplier=1,
-            depthwise_weight_init_func=recurrent_weight_init_func,
-            pointwise_weight_init_func=recurrent_weight_init_func,
-            pointwise_bias_init_func=None,  # no bias
+            input_dilation=input_dilation,
+            kernel_dilation=kernel_dilation,
+            weight_init_func=recurrent_weight_init_func,
+            bias_init_func=None,
             key=k2,
-            ndim=ndim,
         )
 
-    def __call__(
-        self, x: jnp.ndarray, state: SeparableConvLSTMNDState, **kwargs
-    ) -> SeparableConvLSTMNDState:
-        if hasattr(self, "_partial_init"):
-            if isinstance(x, jax.core.Tracer):
-                raise ValueError(_TRACER_ERROR_MSG(self.__class__.__name__))
-            self._partial_init(in_features=x.shape[0])
-
-        msg = f"Expected input to have shape (batch_size, in_features, *spatial_dims), got {x.shape}"
-        assert isinstance(state, SeparableConvLSTMNDState), msg
-        h, c = state.hidden_state, state.cell_state
+    @ft.partial(validate_spatial_in_shape, attribute_name="spatial_ndim")
+    def __call__(self, x: jax.Array, state: ConvGRUNDState, **k) -> ConvGRUNDState:
+        if not isinstance(state, ConvGRUNDState):
+            msg = f"Expected state to be an instance of GRUState, got {type(state)}"
+            raise TypeError(msg)
 
-        h = self.in_to_hidden(x) + self.hidden_to_hidden(h)
-        i, f, g, o = jnp.split(h, 4, axis=0)
-        i = self.recurrent_act_func(i)
-        f = self.recurrent_act_func(f)
-        g = self.act_func(g)
-        o = self.recurrent_act_func(o)
-        c = f * c + i * g
-        h = o * self.act_func(c)
-        return SeparableConvLSTMNDState(hidden_state=h, cell_state=c)
-
-    def init_state(self, spatial_dim: tuple[int, ...]) -> SeparableConvLSTMNDState:
-        msg = f"Expected spatial_dim to be a tuple of length {self.ndim}, got {spatial_dim}"
-        assert len(spatial_dim) == self.ndim, msg
+        h = state.hidden_state
+        xe, xu, xo = jnp.split(self.in_to_hidden(x), 3, axis=0)
+        he, hu, ho = jnp.split(self.hidden_to_hidden(h), 3, axis=0)
+        e = self.recurrent_act_func(xe + he)
+        u = self.recurrent_act_func(xu + hu)
+        o = self.act_func(xo + (e * ho))
+        h = (1 - u) * o + u * h
+        return ConvGRUNDState(hidden_state=h)
+
+    def init_state(self, spatial_dim: tuple[int, ...]) -> ConvGRUNDState:
+        msg = f"Expected spatial_dim to be a tuple of length {self.spatial_ndim}, got {spatial_dim}"
+        assert len(spatial_dim) == self.spatial_ndim, msg
         shape = (self.hidden_features, *spatial_dim)
-        return SeparableConvLSTMNDState(jnp.zeros(shape), jnp.zeros(shape))
+        return ConvGRUNDState(hidden_state=jnp.zeros(shape))
 
 
-@pytc.treeclass
-class SeparableConvLSTM1DCell(SeparableConvLSTMNDCell):
+class ConvGRU1DCell(ConvGRUNDCell):
     def __init__(
         self,
         in_features: int,
-        out_features: int,
-        kernel_size: int,
+        hidden_features: int,
+        kernel_size: int | tuple[int, ...],
         *,
-        strides: int = 1,
-        padding: str = "SAME",
-        weight_init_func: str | Callable = "glorot_uniform",
-        bias_init_func: str | Callable | None = "zeros",
-        recurrent_weight_init_func: str | Callable = "orthogonal",
-        act_func: str | None = "tanh",
-        recurrent_act_func: str | None = "hard_sigmoid",
-        key: jr.PRNGKey = jr.PRNGKey(0),
+        strides: StridesType = 1,
+        padding: PaddingType = "SAME",
+        input_dilation: DilationType = 1,
+        kernel_dilation: DilationType = 1,
+        weight_init_func: InitFuncType = "glorot_uniform",
+        bias_init_func: InitFuncType = "zeros",
+        recurrent_weight_init_func: InitFuncType = "orthogonal",
+        act_func: ActivationType | None = "tanh",
+        recurrent_act_func: ActivationType | None = "sigmoid",
+        key: jr.KeyArray = jr.PRNGKey(0),
     ):
+        """1D Convolution GRU cell that defines the update rule for the hidden state and cell state
+        Args:
+            in_features: Number of input features
+            hidden_features: Number of output features
+            kernel_size: Size of the convolutional kernel
+            strides: Stride of the convolution
+            padding: Padding of the convolution
+            input_dilation: Dilation of the input
+            kernel_dilation: Dilation of the convolutional kernel
+            weight_init_func: Weight initialization function
+            bias_init_func: Bias initialization function
+            recurrent_weight_init_func: Recurrent weight initialization function
+            act_func: Activation function
+            recurrent_act_func: Recurrent activation function
+            key: PRNG key
+            spatial_ndim: Number of spatial dimensions.
+
+        """
         super().__init__(
             in_features=in_features,
-            out_features=out_features,
+            hidden_features=hidden_features,
             kernel_size=kernel_size,
             strides=strides,
             padding=padding,
+            input_dilation=input_dilation,
+            kernel_dilation=kernel_dilation,
             weight_init_func=weight_init_func,
             bias_init_func=bias_init_func,
             recurrent_weight_init_func=recurrent_weight_init_func,
             act_func=act_func,
             recurrent_act_func=recurrent_act_func,
             key=key,
-            ndim=1,
+            conv_layer=sk.nn.Conv1D,
+            spatial_ndim=1,
         )
 
 
-@pytc.treeclass
-class SeparableConvLSTM2DCell(SeparableConvLSTMNDCell):
+class ConvGRU2DCell(ConvGRUNDCell):
     def __init__(
         self,
         in_features: int,
-        out_features: int,
-        kernel_size: int | tuple[int, int],
+        hidden_features: int,
+        kernel_size: int | tuple[int, ...],
         *,
-        strides: int | tuple[int, int] = 1,
-        padding: str
-        | tuple[int, int]
-        | tuple[tuple[int, int], tuple[int, int]] = "SAME",
-        weight_init_func: str | Callable = "glorot_uniform",
-        bias_init_func: str | Callable | None = "zeros",
-        recurrent_weight_init_func: str | Callable = "orthogonal",
-        act_func: str | None = "tanh",
-        recurrent_act_func: str | None = "hard_sigmoid",
-        key: jr.PRNGKey = jr.PRNGKey(0),
+        strides: StridesType = 1,
+        padding: PaddingType = "SAME",
+        input_dilation: DilationType = 1,
+        kernel_dilation: DilationType = 1,
+        weight_init_func: InitFuncType = "glorot_uniform",
+        bias_init_func: InitFuncType = "zeros",
+        recurrent_weight_init_func: InitFuncType = "orthogonal",
+        act_func: ActivationType | None = "tanh",
+        recurrent_act_func: ActivationType | None = "sigmoid",
+        key: jr.KeyArray = jr.PRNGKey(0),
     ):
+        """2D Convolution GRU cell that defines the update rule for the hidden state and cell state
+        Args:
+            in_features: Number of input features
+            hidden_features: Number of output features
+            kernel_size: Size of the convolutional kernel
+            strides: Stride of the convolution
+            padding: Padding of the convolution
+            input_dilation: Dilation of the input
+            kernel_dilation: Dilation of the convolutional kernel
+            weight_init_func: Weight initialization function
+            bias_init_func: Bias initialization function
+            recurrent_weight_init_func: Recurrent weight initialization function
+            act_func: Activation function
+            recurrent_act_func: Recurrent activation function
+            key: PRNG key
+            spatial_ndim: Number of spatial dimensions.
+
+        """
         super().__init__(
             in_features=in_features,
-            out_features=out_features,
+            hidden_features=hidden_features,
             kernel_size=kernel_size,
             strides=strides,
             padding=padding,
+            input_dilation=input_dilation,
+            kernel_dilation=kernel_dilation,
             weight_init_func=weight_init_func,
             bias_init_func=bias_init_func,
             recurrent_weight_init_func=recurrent_weight_init_func,
             act_func=act_func,
             recurrent_act_func=recurrent_act_func,
             key=key,
-            ndim=2,
+            conv_layer=sk.nn.Conv2D,
+            spatial_ndim=2,
         )
 
 
-@pytc.treeclass
-class SeparableConvLSTM3DCell(SeparableConvLSTMNDCell):
+class ConvGRU3DCell(ConvGRUNDCell):
     def __init__(
         self,
         in_features: int,
-        out_features: int,
-        kernel_size: int | tuple[int, int, int],
+        hidden_features: int,
+        kernel_size: int | tuple[int, ...],
         *,
-        strides: int | tuple[int, int, int] = 1,
-        padding: str
-        | tuple[int, int, int]
-        | tuple[tuple[int, int, int], tuple[int, int, int]] = "SAME",
-        weight_init_func: str | Callable = "glorot_uniform",
-        bias_init_func: str | Callable | None = "zeros",
-        recurrent_weight_init_func: str | Callable = "orthogonal",
-        act_func: str | None = "tanh",
-        recurrent_act_func: str | None = "hard_sigmoid",
-        key: jr.PRNGKey = jr.PRNGKey(0),
+        strides: StridesType = 1,
+        padding: PaddingType = "SAME",
+        input_dilation: DilationType = 1,
+        kernel_dilation: DilationType = 1,
+        weight_init_func: InitFuncType = "glorot_uniform",
+        bias_init_func: InitFuncType = "zeros",
+        recurrent_weight_init_func: InitFuncType = "orthogonal",
+        act_func: ActivationType | None = "tanh",
+        recurrent_act_func: ActivationType | None = "sigmoid",
+        key: jr.KeyArray = jr.PRNGKey(0),
     ):
+        """3D Convolution GRU cell that defines the update rule for the hidden state and cell state
+        Args:
+            in_features: Number of input features
+            hidden_features: Number of output features
+            kernel_size: Size of the convolutional kernel
+            strides: Stride of the convolution
+            padding: Padding of the convolution
+            input_dilation: Dilation of the input
+            kernel_dilation: Dilation of the convolutional kernel
+            weight_init_func: Weight initialization function
+            bias_init_func: Bias initialization function
+            recurrent_weight_init_func: Recurrent weight initialization function
+            act_func: Activation function
+            recurrent_act_func: Recurrent activation function
+            key: PRNG key
+            spatial_ndim: Number of spatial dimensions.
+
+        """
         super().__init__(
             in_features=in_features,
-            out_features=out_features,
+            hidden_features=hidden_features,
             kernel_size=kernel_size,
             strides=strides,
             padding=padding,
+            input_dilation=input_dilation,
+            kernel_dilation=kernel_dilation,
             weight_init_func=weight_init_func,
             bias_init_func=bias_init_func,
             recurrent_weight_init_func=recurrent_weight_init_func,
             act_func=act_func,
             recurrent_act_func=recurrent_act_func,
             key=key,
-            ndim=3,
+            conv_layer=sk.nn.Conv3D,
+            spatial_ndim=3,
         )
 
 
-# ------------------------------------------------- Scan layer ------------------------------------------------------ #
+# =============================================== Scanning API ======================================================= #
 
 
-@pytc.treeclass
-class ScanRNN:
-    cell: RNNCell | SpatialRNNCell
-    backward_cell: RNNCell | SpatialRNNCell | None
+class ScanRNN(pytc.TreeClass):
+    cell: RNNCell
+    backward_cell: RNNCell
 
     def __init__(
         self,
         cell: RNNCell | SpatialRNNCell,
         backward_cell: RNNCell | SpatialRNNCell | None = None,
         *,
         return_sequences: bool = False,
@@ -786,122 +868,110 @@
             return_sequences: whether to return the hidden state for each timestep
 
         Example:
             >>> cell = SimpleRNNCell(10, 20) # 10-dimensional input, 20-dimensional hidden state
             >>> rnn = ScanRNN(cell)
             >>> x = jnp.ones((5, 10)) # 5 timesteps, 10 features
             >>> result = rnn(x)  # 20 features
-
-            # bidirectional convolution lstm
-            >>> cell = ConvLSTM1DCell(10, 20, kernel_size=3) # 10-features input, 20-features hidden state
-            >>> reverse_cell = ConvLSTM1DCell(10, 20, kernel_size=3) # 10-features input, 20-features hidden state
-            >>> rnn = ScanRNN(cell, reverse_cell, return_sequences=True)
-            >>> x = jnp.ones((5, 10,12)) # 5 timesteps, 10 features, width 12
-            >>> result = rnn(x)  # 5 timestep, 20*2 features, width 12
-        """
-        if not isinstance(cell, (RNNCell, SpatialRNNCell)):
-            msg = f"Expected cell to be an instance of RNNCell or SpatialRNNCell, got {type(cell)}"
-            raise ValueError(msg)
-
-        if not isinstance(backward_cell, (RNNCell, SpatialRNNCell, type(None))):
-            msg = "Expected backward_cell to be an instance of RNNCell, SpatialRNNCell or None"
-            msg += f", got {type(backward_cell)}"
-            raise ValueError(msg)
+        """
+        if not isinstance(cell, RNNCell):
+            msg = f"Expected `cell` to be an instance of RNNCell got {type(cell)}"
+            raise TypeError(msg)
+
+        if not isinstance(backward_cell, (RNNCell, type(None))):
+            msg = "Expected `backward_cell` to be an instance of RNNCell, "
+            msg += f"got {type(backward_cell).__name__}"
+            raise TypeError(msg)
 
         self.cell = cell
         self.backward_cell = backward_cell
         self.return_sequences = return_sequences
 
     def __call__(
         self,
-        x: jnp.ndarray,
-        state: RNNState = None,
-        backward_state: RNNState = None,
-        **kwargs,
-    ) -> jnp.ndarray:
-        if hasattr(self.cell, "_partial_init"):
-            if isinstance(x, jax.core.Tracer):
-                raise ValueError(_TRACER_ERROR_MSG(self.__class__.__name__))
-            self.cell._partial_init(in_features=x.shape[1])
-
-        if hasattr(self.backward_cell, "_partial_init"):
-            if isinstance(x, jax.core.Tracer):
-                raise ValueError(_TRACER_ERROR_MSG(self.__class__.__name__))
-            self.backward_cell._partial_init(in_features=x.shape[1])
-
-        if not isinstance(state, (type(None), RNNState)):
-            msg = f"Expected state to be an instance of RNNState, got {type(state)}"
-            raise ValueError(msg)
-
-        # backward cell
-        if not isinstance(backward_state, (type(None), RNNState)):
-            msg = f"Expected backward_state to be an instance of RNNState, got {type(backward_state)}"
-            raise ValueError(msg)
-
-        if isinstance(self.cell, SpatialRNNCell):
-            # (time steps, in_features, *spatial_dims)
-            msg = f"Expected x to have {self.cell.ndim + 2}"  # account for time and in_features
-            msg += f"dimensions corresponds to (timesteps, in_features, *spatial_dims), got {x.ndim}"
-            assert x.ndim == (self.cell.ndim + 2), msg
-            msg = f"Expected x to have shape (timesteps, {self.cell.in_features}, *spatial_dims)"
-            msg += f", got {x.shape}"
-            assert self.cell.in_features == x.shape[1], msg
-            state = state or self.cell.init_state(spatial_dim=x.shape[2:])
+        x: jax.Array,
+        state: RNNCell | None = None,
+        backward_state: RNNState | None = None,
+        **k,
+    ) -> jax.Array:
+        # check state
+        if not isinstance(state, (RNNState, type(None))):
+            msg = "Expected state to be an instance of RNNState, "
+            msg += f"got {type(state).__name__}"
+            raise TypeError(msg)
+
+        if isinstance(self.cell, NonSpatialRNNCell):
+            # non-spatial RNN : (time steps, in_features)
+            if x.ndim != 2:
+                msg = "Expected x to have 2 dimensions corresponds "
+                msg += f"to (timesteps, in_features), got {x.ndim}"
+                raise ValueError(msg)
+
+            if self.cell.in_features != x.shape[1]:
+                # check input shape
+                msg = f"Expected x to have shape (timesteps, {self.cell.in_features})"
+                msg += f", got {x.shape}"
+                raise ValueError(msg)
+
+            state = state or self.cell.init_state()
 
             if self.backward_cell is not None:
-                msg = f"Expected backward cell to be an instance of SpatialRNNCell, got {type(self.backward_cell)}"
-                assert isinstance(self.backward_cell, SpatialRNNCell), msg
-                backward_state = backward_state or self.backward_cell.init_state(
-                    spatial_dim=x.shape[2:]
-                )
+                backward_state = backward_state or self.backward_cell.init_state()
 
         else:
-            # (time steps, in_features)
-            msg = f"Expected x to have 2 dimensions corresponds to (timesteps, in_features), got {x.ndim}"
-            assert x.ndim == 2, msg
-            msg = f"Expected x to have shape (timesteps, {self.cell.in_features})"
-            msg += f", got {x.shape}"
-            assert self.cell.in_features == x.shape[1], msg
-            state = state or self.cell.init_state()
+            # spatial RNN : (time steps, in_features, *spatial_dims)
+
+            if x.ndim != self.cell.spatial_ndim + 2:
+                msg = f"Expected x to have {self.cell.spatial_ndim + 2}"  # account for time and in_features
+                msg += f" dimensions corresponds to (timesteps, in_features, *spatial_dims), got {x.ndim}"
+                raise ValueError(msg)
+
+            if self.cell.in_features != x.shape[1]:
+                # check input shape
+                msg = f"Expected x to have shape (timesteps, {self.cell.in_features}, *spatial_dims)"
+                msg += f", got {x.shape}"
+                raise ValueError(msg)
+
+            state = state or self.cell.init_state(spatial_dim=x.shape[2:])
 
             if self.backward_cell is not None:
-                msg = f"Expected backward cell to be an instance of RNNCell, got {type(self.backward_cell)}"
-                assert isinstance(self.backward_cell, RNNCell), msg
-                backward_state = backward_state or self.backward_cell.init_state()
+                backward_state = backward_state or self.backward_cell.init_state(x.shape[2:])  # fmt: skip
+
+        # scan over the time axis
 
         if self.return_sequences:
             # accumulate the hidden state for each timestep
+            # in essence, this means return a state along with the carry
+            # in `jax.lax.scan`
             def general_scan_func(cell, carry, x):
                 state = cell(x, state=carry)
                 return state, state
 
             scan_func = ft.partial(general_scan_func, self.cell)
             result = jax.lax.scan(scan_func, state, x)[1].hidden_state
 
-            # backward cell
-            if self.backward_cell is not None:
+            if self.backward_cell:
                 scan_func = ft.partial(general_scan_func, self.backward_cell)
                 x = jnp.flip(x, axis=0)  # reverse the time axis
                 back_result = jax.lax.scan(scan_func, backward_state, x)[1].hidden_state
                 # reverse once again over the accumulated time axis
                 back_result = jnp.flip(back_result, axis=-1)
                 result = jnp.concatenate([result, back_result], axis=1)
 
-            return result
-
         else:
-            # only return the hidden state for the last timestep
+            # no return sequences case, return carry only
+            # (i.e. only return the hidden state for the last timestep)
             def general_scan_func(cell, carry, x):
                 state = cell(x, state=carry)
                 return state, None
 
             scan_func = ft.partial(general_scan_func, self.cell)
             result = jax.lax.scan(scan_func, state, x)[0].hidden_state
 
             # backward cell
             if self.backward_cell is not None:
                 scan_func = ft.partial(general_scan_func, self.backward_cell)
                 x = jnp.flip(x, axis=0)
                 back_result = jax.lax.scan(scan_func, backward_state, x)[0].hidden_state
                 result = jnp.concatenate([result, back_result], axis=0)
 
-            return result
+        return result
```

### Comparing `serket-0.0.9/serket.egg-info/PKG-INFO` & `serket-0.2.0b2/serket.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serket
-Version: 0.0.9
+Version: 0.2.0b2
 Summary: JAX NN library.
 Home-page: https://github.com/ASEM000/serket
 Author: Mahmoud Asem
 Author-email: asem00@kaist.ac.kr
 License: MIT
 Keywords: python machine-learning pytorch jax
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,194 +13,120 @@
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
 
-
 <div align="center">
-<img width="350px" src="assets/serketLogo.svg"></div>
+<img width="350px" src="assets/logo.svg"></div>
 
 <h2 align="center">The ✨Magical✨ JAX Scientific ML Library.</h2>
-<h5 align = "center"> *Serket is the goddess of magic in Egyptian mythology 
+<h5 align = "center"> *Serket is the goddess of magic in Egyptian mythology
 
 [**Installation**](#Installation)
 |[**Description**](#Description)
 |[**Quick Example**](#QuickExample)
 |[**Freezing/Fine tuning**](#Freezing)
 |[**Filtering**](#Filtering)
 
-
 ![Tests](https://github.com/ASEM000/serket/actions/workflows/tests.yml/badge.svg)
 ![pyver](https://img.shields.io/badge/python-3.7%203.8%203.9%203.10-red)
 ![codestyle](https://img.shields.io/badge/codestyle-black-lightgrey)
 [![Downloads](https://pepy.tech/badge/serket)](https://pepy.tech/project/serket)
 [![codecov](https://codecov.io/gh/ASEM000/serket/branch/main/graph/badge.svg?token=C6NXOK9EVS)](https://codecov.io/gh/ASEM000/serket)
 [![DOI](https://zenodo.org/badge/526985786.svg)](https://zenodo.org/badge/latestdoi/526985786)
 ![PyPI](https://img.shields.io/pypi/v/serket)
 
 </h5>
 
-
 ## 🛠️ Installation<a id="Installation"></a>
 
 ```python
 pip install serket
 ```
+
 **Install development version**
+
 ```python
 pip install git+https://github.com/ASEM000/serket
 ```
 
+## 📖 Description and motivation<a id="Description"></a>
 
-## 📖 Description<a id="Description"></a>
 - `serket` aims to be the most intuitive and easy-to-use physics-based Neural network library in JAX.
-- `serket` is built on top of [`pytreeclass`](https://github.com/ASEM000/pytreeclass)
 - `serket` is fully transparent to `jax` transformation (e.g. `vmap`,`grad`,`jit`,...)
+- `serket` current aim to facilitate the integration of numerical methods in a NN setting (see examples for more)
 
-<div align="center">
+### Layer structure
 
-### ➖➕Finite difference package: `serket.fd`➕➖
+`serket` is built on top of [`PyTreeClass`](https://github.com/ASEM000/pytreeclass), this means that layers are represented as a [PyTree](https://jax.readthedocs.io/en/latest/pytrees.html) whose leaves are the layer parameters.
 
-| Group| Function/Layer|
-| ------------- | ------------- |
-|Finite difference layer|`Difference`: apply finite difference to input array to any derivative order and accuracy|
-|Finite difference functions| - `difference`: finite difference of array with any accuracy and derivative order  <br> -`generate_finitediff_coeffs` : generate coeffs using sample points and derivative order <br> - `fgrad`: differentiate _functions_ (similar to `jax.grad`) with custom accuracy and derivative order|
-|Vector operator layers|`Curl`, `Divergence`, `Gradient`, `Laplacian`, `Jacobian`, `Hessian`|
-|Vector operator function| `curl`, `divergence`, `gradient`, `laplacian`, `jacobian`, `hessian`|
+<div align="center">
 
 ### 🧠 Neural network package: `serket.nn` 🧠
-| Group | Layers |
-| ------------- | ------------- |
-| Linear  | `Linear`, `Bilinear`, `Multilinear`, `GeneralLinear`, `Identity`   |
-|Densely connected|`FNN` (Fully connected network), `PFNN` (Parallel fully connected network)|
-| Convolution | `Conv1D`, `Conv2D`, `Conv3D`, `Conv1DTranspose` , `Conv2DTranspose`, `Conv3DTranspose`, `DepthwiseConv1D`, `DepthwiseConv2D`, `DepthwiseConv3D`, `SeparableConv1D`, `SeparableConv2D`, `SeparableConv3D`, `Conv1DLocal`, `Conv2DLocal`, `Conv3DLocal` |
-| Containers| `Sequential`, `Lambda` |
-|Pooling|`MaxPool1D`, `MaxPool2D`, `MaxPool3D`, `AvgPool1D`, `AvgPool2D`, `AvgPool3D` `GlobalMaxPool1D`, `GlobalMaxPool2D`, `GlobalMaxPool3D`, `GlobalAvgPool1D`, `GlobalAvgPool2D`, `GlobalAvgPool3D` `LPPool1D`, `LPPool2D`,`LPPool3D` , `AdaptivePool1D`, `AdaptivePool2D`, `AdaptivePool3D`,`AdaptiveConcatPool1D`,`AdaptiveConcatPool2D`,`AdaptiveConcatPool3D` (`kernex` backend)|
-|Reshaping|`Flatten`, `Unflatten`, `FlipLeftRight2D`, `FlipUpDown2D`, `Repeat1D`, `Repeat2D`, `Repeat3D`, `Resize1D`, `Resize2D`, `Resize3D`, `Upsample1D`, `Upsample2D`, `Upsample3D`, `Pad1D`, `Pad2D`, `Pad3D` |
-|Crop|`Crop1D`, `Crop2D`, |
-|Normalization|`LayerNorm`, `InstanceNorm`, `GroupNorm`|
-|Blurring| `AvgBlur2D`, `GaussianBlur2D`|
-|Dropout|`Dropout`, `Dropout1D`, `Dropout2D`, `Dropout3D`, |
-|Random transforms|`RandomCrop1D`, `RandomCrop2D`, `RandomApply`, `RandomCutout1D`, `RandomCutout2D`, `RandomZoom2D`, `RandomContrast2D` |
-|Misc|`HistogramEqualization2D`, `AdjustContrast2D`, `Filter2D`, `PixelShuffle`|
-|Activations|`AdaptiveLeakyReLU`,`AdaptiveReLU`,`AdaptiveSigmoid`,`AdaptiveTanh`,<br>`CeLU`,`ELU`,`GELU`,`GLU`<br>,`HardSILU`,`HardShrink`,`HardSigmoid`,`HardSwish`,`HardTanh`,<br>`LeakyReLU`,`LogSigmoid`,`LogSoftmax`,`Mish`,`PReLU`,<br> `ReLU`,`ReLU6`,`SILU`,`SeLU`,`Sigmoid`,`SoftPlus`,`SoftShrink`,<br>`SoftSign`,`Swish`,`Tanh`,`TanhShrink`, `ThresholdedReLU`, `Snake`|
-|Recurrent|`SimpleRNNCell`, `LSTMCell`, `ConvLSTM1D`, `ConvLSTM2D`, `ConvLSTM3D`, `SeparableConvLSTM1DCell`, `SeparableConvLSTM2DCell`, `SeparableConvLSTM3DCell`|
-|Blocks|`VGG16Block`, `VGG19Block`, `UNetBlock`|
-
-
 
+| Group                           | Layers                                                                                                                                                                                                                                                                                                                                                 |
+| ------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
+| Linear                          | - `Linear`, `Bilinear`, `Multilinear`, `GeneralLinear`, `Identity`, `Embedding`                                                                                                                                                                                                                                                                        |
+| Densely connected               | - `FNN` (Fully connected network),                                                                                                                                                                                                                                                                                                                     |
+| Convolution                     | - `{Conv,FFTConv}{1D,2D,3D}` <br> - `{Conv,FFTConv}{1D,2D,3D}Transpose` <br> - `{Depthwise,Separable}{Conv,FFTConv}{1D,2D,3D}` <br> - `Conv{1D,2D,3D}Local`                                                                                                                                                                                            |
+| Containers                      | - `Sequential`, `Lambda`                                                                                                                                                                                                                                                                                                                               |
+| Pooling <br> (`kernex` backend) | - `{Avg,Max,LP}Pool{1D,2D,3D}` <br> - `Global{Avg,Max}Pool{1D,2D,3D}` <br> - `Adaptive{Avg,Max}Pool{1D,2D,3D}`                                                                                                                                                                                                                                         |
+| Reshaping                       | - `Flatten`, `Unflatten`, <br> - `FlipLeftRight2D`, `FlipUpDown2D` <br> - `Resize{1D,2D,3D}` <br> - `Upsample{1D,2D,3D}` <br> - `Pad{1D,2D,3D}`                                                                                                                                                                                                        |
+| Crop                            | - `Crop{1D,2D}`                                                                                                                                                                                                                                                                                                                                        |
+| Normalization                   | - `{Layer,Instance,Group}Norm`                                                                                                                                                                                                                                                                                                                         |
+| Blurring                        | - `{Avg,Gaussian}Blur2D`                                                                                                                                                                                                                                                                                                                               |
+| Dropout                         | - `Dropout`<br> - `Dropout{1D,2D,3D}`                                                                                                                                                                                                                                                                                                                  |
+| Random transforms               | - `RandomCrop{1D,2D}` <br> - `RandomApply`, <br> - `RandomCutout{1D,2D}` <br> - `RandomZoom2D`, <br> - `RandomContrast2D`                                                                                                                                                                                                                              |
+| Misc                            | - `HistogramEqualization2D`, `AdjustContrast2D`, `Filter2D`, `PixelShuffle2D`                                                                                                                                                                                                                                                                          |
+| Activations                     | - `Adaptive{LeakyReLU,ReLU,Sigmoid,Tanh}`,<br> - `CeLU`,`ELU`,`GELU`,`GLU`<br>- `Hard{SILU,Shrink,Sigmoid,Swish,Tanh}`, <br> - `Soft{Plus,Sign,Shrink}` <br> - `LeakyReLU`,`LogSigmoid`,`LogSoftmax`,`Mish`,`PReLU`,<br> - `ReLU`,`ReLU6`,`SILU`,`SeLU`,`Sigmoid` <br> - `Swish`,`Tanh`,`TanhShrink`, `ThresholdedReLU`, `Snake`, `Stan`, `SquarePlus` |
+| Recurrent cells                 | - `{SimpleRNN,LSTM,GRU}Cell` <br> - `Conv{LSTM,GRU}{1D,2D,3D}Cell`                                                                                                                                                                                                                                                                                     |
+| Blocks                          | - `VGG{16,19}Block`, `UNetBlock`                                                                                                                                                                                                                                                                                                                       |
 
 </div>
 
 ## ⏩ Examples: <a id="QuickExample">
 
 <details>
-
-<summary> Finite difference examples </summary>
+<summary> Linear layers examples</summary>
 
 ```python
-import jax
-
-jax.config.update("jax_enable_x64", True)
 import jax.numpy as jnp
-import numpy.testing as npt
 
 import serket as sk
 
-
-# lets first define a vector valued function F: R^3 -> R^3
-# F = F1, F2
-# F1 = x^2 + y^3
-# F2 = x^4 + y^3
-# F3 = 0
-# F = [x**2 + y**3, x**4 + y**3, 0]
-
-x, y, z = [jnp.linspace(0, 1, 100)] * 3
-dx, dy, dz = x[1] - x[0], y[1] - y[0], z[1] - z[0]
-X, Y, Z = jnp.meshgrid(x, y, z, indexing="ij")
-F1 = X**2 + Y**3
-F2 = X**4 + Y**3
-F3 = jnp.zeros_like(F1)
-F = jnp.stack([F1, F2, F3], axis=0)
-
-# ∂F1/∂x : differentiate F1 with respect to x (i.e axis=0)
-dF1dx = sk.fd.difference(F1, axis=0, step_size=dx, accuracy=6)
-dF1dx_exact = 2 * X
-npt.assert_allclose(dF1dx, dF1dx_exact, atol=1e-7)
-
-# ∂F2/∂y : differentiate F2 with respect to y (i.e axis=1)
-dF2dy = sk.fd.difference(F2, axis=1, step_size=dy, accuracy=6)
-dF2dy_exact = 3 * Y**2
-npt.assert_allclose(dF2dy, dF2dy_exact, atol=1e-7)
-
-# ∇.F : the divergence of F
-divF = sk.fd.divergence(F, step_size=(dx, dy, dz), keepdims=False, accuracy=6)
-divF_exact = 2 * X + 3 * Y**2
-npt.assert_allclose(divF, divF_exact, atol=1e-7)
-
-# ∇F1 : the gradient of F1
-gradF1 = sk.fd.gradient(F1, step_size=(dx, dy, dz), accuracy=6)
-gradF1_exact = jnp.stack([2 * X, 3 * Y**2, 0 * X], axis=0)
-npt.assert_allclose(gradF1, gradF1_exact, atol=1e-7)
-
-# ΔF1 : laplacian of F1
-lapF1 = sk.fd.laplacian(F1, step_size=(dx, dy, dz), accuracy=6)
-lapF1_exact = 2 + 6 * Y
-npt.assert_allclose(lapF1, lapF1_exact, atol=1e-7)
-
-# ∇xF : the curl of F
-curlF = sk.fd.curl(F, step_size=(dx, dy, dz), accuracy=6)
-curlF_exact = jnp.stack([F1 * 0, F1 * 0, 4 * X**3 - 3 * Y**2], axis=0)
-npt.assert_allclose(curlF, curlF_exact, atol=1e-7)
-
-# Jacobian of F
-JF = sk.fd.jacobian(F, accuracy=4, step_size=(dx, dy, dz))
-JF_exact = jnp.array(
-    [
-        [2 * X, 3 * Y**2, jnp.zeros_like(X)],
-        [4 * X**3, 3 * Y**2, jnp.zeros_like(X)],
-        [jnp.zeros_like(X), jnp.zeros_like(X), jnp.zeros_like(X)],
-    ]
-)
-npt.assert_allclose(JF, JF_exact, atol=1e-7)
-
-# Hessian of F1
-HF1 = sk.fd.hessian(F1, accuracy=4, step_size=(dx, dy, dz))
-HF1_exact = jnp.array(
-    [
-        [
-            2 * jnp.ones_like(X),  # ∂2F1/∂x2
-            0 * jnp.ones_like(X),  # ∂2F1/∂xy
-            0 * jnp.ones_like(X),  # ∂2F1/∂xz
-        ],
-        [
-            0 * jnp.ones_like(X),  # ∂2F1/∂yx
-            6 * Y**2,              # ∂2F1/∂y2
-            0 * jnp.ones_like(X),  # ∂2F1/∂yz
-        ],
-        [
-            0 * jnp.ones_like(X),  # ∂2F1/∂zx
-            0 * jnp.ones_like(X),  # ∂2F1/∂zy
-            0 * jnp.ones_like(X),  # ∂2F1/∂z2
-        ],
-    ]
-)
-npt.assert_allclose(JF, JF_exact, atol=1e-7)
-
+# Linear
+x = jnp.ones([1, 2, 3, 4])
+l1 = sk.nn.Linear(4, 5)  # last dim is 4, output dim is 5
+print(l1(x).shape)  # (1, 2, 3, 5)
+
+# Bilinear
+x1, x2 = jnp.ones([1, 2, 3, 4]), jnp.ones([1, 2, 3, 5])
+l2 = sk.nn.Bilinear(4, 5, 6)  # last dim of the input x1,x2 are 4,5, output dim is 6
+print(l2(x1, x2).shape)  # (1, 2, 3, 6)
+
+# Multilinear
+x1, x2, x3 = jnp.ones([1, 2, 3, 4]), jnp.ones([1, 2, 3, 5]), jnp.ones([1, 2, 3, 6])
+l3 = sk.nn.Multilinear((4, 5, 6), 7)  # last dim for x1,x2,x3 = 4,5,6, output dim is 7
+print(l3(x1, x2, x3).shape)  # (1, 2, 3, 7)
+
+# GeneralLinear
+x = jnp.ones([4, 5, 6, 7])
+# apply a linear layer to axis 1,2,3, with dim = (5, 6, 7) and output dim is 5
+l4 = sk.nn.GeneralLinear((5, 6, 7), 5, in_axes=(1, 2, 3))
+print(l4(x).shape)  # (4, 5)
 ```
 
 </details>
 
-
 <details>
 <summary>
 Train Bidirectional-LSTM
 </summary>
 
 ```python
 import jax
@@ -295,27 +221,25 @@
 plt.legend()
 ```
 
 ![image](assets/rnn.svg)
 
 </details>
 
-
 <details>
 
 <summary>Lazy initialization</summary>
 
-In cases where `in_features` needs to be inferred from input, use `None` instead of `in_features` to infer the value at runtime. 
-However, since the lazy module initialize it's state after the first call (i.e. mutate it's state)  `jax` transformation ex: `vmap, grad ...` is not allowed before initialization. Using any `jax` transformation before initialization will throw a `ValueError`.
-
+In cases where `in_features` needs to be inferred from input, use `None` instead of `in_features` to infer the value at runtime.
+However, since the lazy module initialize it's state after the first call (i.e. mutate it's state) `jax` transformation ex: `vmap, grad ...` is not allowed before initialization. Using any `jax` transformation before initialization will throw a `ValueError`.
 
 ```python
-import serket as sk 
+import serket as sk
 import jax
-import jax.numpy as jnp 
+import jax.numpy as jnp
 
 model = sk.nn.Sequential(
     [
         sk.nn.Conv2D(None, 128, 3),
         sk.nn.ReLU(),
         sk.nn.MaxPool2D(2, 2),
         sk.nn.Conv2D(128, 64, 3),
@@ -369,15 +293,14 @@
 #   bias_init_func=Partial(zeros(key,shape,dtype)),
 #   *groups=1
 # )
 ```
 
 </details>
 
-
 <details>
 
 <summary>Train MNIST</summary>
 
 We will use `tensorflow` datasets for dataloading. for more on interface of jax/tensorflow dataset see [here](https://jax.readthedocs.io/en/latest/notebooks/neural_network_with_tfds_data.html)
 
 ```python
@@ -385,15 +308,15 @@
 import tensorflow as tf
 # Ensure TF does not see GPU and grab all GPU memory.
 tf.config.set_visible_devices([], device_type="GPU")
 import tensorflow_datasets as tfds
 import tensorflow.experimental.numpy as tnp
 import jax
 import jax.numpy as jnp
-import jax.random as jr 
+import jax.random as jr
 import optax  # for gradient optimization
 import serket as sk
 import matplotlib.pyplot as plt
 import functools as ft
 ```
 
 ```python
@@ -420,15 +343,15 @@
 # (batches, 1, 28, 28)
 ds_test = ds_test.map(preprocess_data).prefetch(tf.data.AUTOTUNE)
 ```
 
 ### 🏗️ Model definition
 
 We will use `jax.vmap(model)` to apply `model` on batches.
-    
+
 ```python
 @sk.treeclass
 class CNN:
     def __init__(self):
         self.conv1 = sk.nn.Conv2D(1, 32, (3, 3), padding="valid")
         self.relu1 = sk.nn.ReLU()
         self.pool1 = sk.nn.MaxPool2D((2, 2), strides=(2, 2))
@@ -451,15 +374,15 @@
         x = self.linear(x)
         return x
 
 model = CNN()
 ```
 
 ### 🎨 Visualize model
-    
+
 <details><summary>Model summary</summary>
     
 ```python
 print(model.summary(show_config=False, array=jnp.empty((1, 28, 28))))  
 ┌───────┬─────────┬─────────┬──────────────┬─────────────┬─────────────┐
 │Name   │Type     │Param #  │Size          │Input        │Output       │
 ├───────┼─────────┼─────────┼──────────────┼─────────────┼─────────────┤
@@ -554,35 +477,36 @@
     
 ```python
  
 # set all dropout off
 test_model = model.at[model == "eval"].set(True, is_leaf=lambda x: x is None)
 
 def show_images_with_predictions(model, images, one_hot_labels):
-    logits = jax.vmap(model)(images)
-    predictions = jnp.argmax(logits, axis=-1)
-    fig, axes = plt.subplots(5, 5, figsize=(10, 10))
-    for i, ax in enumerate(axes.flat):
-        ax.imshow(images[i].reshape(28, 28), cmap="binary")
-        ax.set(title=f"Prediction: {predictions[i]}\nLabel: {jnp.argmax(one_hot_labels[i], axis=-1)}")
-        ax.set_xticks([])
-        ax.set_yticks([])
-    plt.show()
+logits = jax.vmap(model)(images)
+predictions = jnp.argmax(logits, axis=-1)
+fig, axes = plt.subplots(5, 5, figsize=(10, 10))
+for i, ax in enumerate(axes.flat):
+ax.imshow(images[i].reshape(28, 28), cmap="binary")
+ax.set(title=f"Prediction: {predictions[i]}\nLabel: {jnp.argmax(one_hot_labels[i], axis=-1)}")
+ax.set_xticks([])
+ax.set_yticks([])
+plt.show()
 
 example = ds_test.take(25).as_numpy_iterator()
 example = list(example)
 sample_test_images = jnp.stack([x["image"] for x in example])
 sample_test_labels = jnp.stack([x["label"] for x in example])
 
 show_images_with_predictions(test_model, sample_test_images, sample_test_labels)
-```
+
+````
 ![image](assets/before_training.svg)
- 
+
 </details>
-    
+
 ### 🏃 Train the model
 
 ```python
 @ft.partial(jax.value_and_grad, has_aux=True)
 def loss_func(model, batched_images, batched_one_hot_labels):
     logits = jax.vmap(model)(batched_images)
     loss = jnp.mean(optax.softmax_cross_entropy(logits=logits, labels=batched_one_hot_labels))
@@ -615,23 +539,22 @@
         epoch_accuracy.append(accuracy)
         epoch_loss.append(loss)
 
     epoch_loss = jnp.mean(jnp.array(epoch_loss))
     epoch_accuracy = jnp.mean(jnp.array(epoch_accuracy))
 
     print(f"epoch:{i+1:00d}\tloss:{epoch_loss:.4f}\taccuracy:{epoch_accuracy:.4f}")
-    
+
 # epoch:1	loss:0.2706	accuracy:0.9268
 # epoch:2	loss:0.0725	accuracy:0.9784
 # epoch:3	loss:0.0533	accuracy:0.9836
 # epoch:4	loss:0.0442	accuracy:0.9868
 # epoch:5	loss:0.0368	accuracy:0.9889
-```
-    
-    
+````
+
 ### 🎨 Visualize After training
 
 ```python
 test_model = model.at[model == "eval"].set(True, is_leaf=lambda x: x is None)
 show_images_with_predictions(test_model, sample_test_images, sample_test_labels)
 ```
 
@@ -639,21 +562,121 @@
     
 ![image](assets/after_training.svg)
 
 </details>
 
 </details>
 
+<br>
+
+![image](https://img.shields.io/badge/-physics%20examples-blue)
+
+<details>
+
+<summary> Finite difference examples </summary>
+
+```python
+import jax
+
+jax.config.update("jax_enable_x64", True)
+import jax.numpy as jnp
+import numpy.testing as npt
+
+import serket as sk
+
+
+# lets first define a vector valued function F: R^3 -> R^3
+# F = F1, F2
+# F1 = x^2 + y^3
+# F2 = x^4 + y^3
+# F3 = 0
+# F = [x**2 + y**3, x**4 + y**3, 0]
+
+x, y, z = [jnp.linspace(0, 1, 100)] * 3
+dx, dy, dz = x[1] - x[0], y[1] - y[0], z[1] - z[0]
+X, Y, Z = jnp.meshgrid(x, y, z, indexing="ij")
+F1 = X**2 + Y**3
+F2 = X**4 + Y**3
+F3 = jnp.zeros_like(F1)
+F = jnp.stack([F1, F2, F3], axis=0)
+
+# ∂F1/∂x : differentiate F1 with respect to x (i.e axis=0)
+dF1dx = sk.fd.difference(F1, axis=0, step_size=dx, accuracy=6)
+dF1dx_exact = 2 * X
+npt.assert_allclose(dF1dx, dF1dx_exact, atol=1e-7)
+
+# ∂F2/∂y : differentiate F2 with respect to y (i.e axis=1)
+dF2dy = sk.fd.difference(F2, axis=1, step_size=dy, accuracy=6)
+dF2dy_exact = 3 * Y**2
+npt.assert_allclose(dF2dy, dF2dy_exact, atol=1e-7)
+
+# ∇.F : the divergence of F
+divF = sk.fd.divergence(F, step_size=(dx, dy, dz), keepdims=False, accuracy=6)
+divF_exact = 2 * X + 3 * Y**2
+npt.assert_allclose(divF, divF_exact, atol=1e-7)
+
+# ∇F1 : the gradient of F1
+gradF1 = sk.fd.gradient(F1, step_size=(dx, dy, dz), accuracy=6)
+gradF1_exact = jnp.stack([2 * X, 3 * Y**2, 0 * X], axis=0)
+npt.assert_allclose(gradF1, gradF1_exact, atol=1e-7)
+
+# ΔF1 : laplacian of F1
+lapF1 = sk.fd.laplacian(F1, step_size=(dx, dy, dz), accuracy=6)
+lapF1_exact = 2 + 6 * Y
+npt.assert_allclose(lapF1, lapF1_exact, atol=1e-7)
+
+# ∇xF : the curl of F
+curlF = sk.fd.curl(F, step_size=(dx, dy, dz), accuracy=6)
+curlF_exact = jnp.stack([F1 * 0, F1 * 0, 4 * X**3 - 3 * Y**2], axis=0)
+npt.assert_allclose(curlF, curlF_exact, atol=1e-7)
+
+# Jacobian of F
+JF = sk.fd.jacobian(F, accuracy=4, step_size=(dx, dy, dz))
+JF_exact = jnp.array(
+    [
+        [2 * X, 3 * Y**2, jnp.zeros_like(X)],
+        [4 * X**3, 3 * Y**2, jnp.zeros_like(X)],
+        [jnp.zeros_like(X), jnp.zeros_like(X), jnp.zeros_like(X)],
+    ]
+)
+npt.assert_allclose(JF, JF_exact, atol=1e-7)
+
+# Hessian of F1
+HF1 = sk.fd.hessian(F1, accuracy=4, step_size=(dx, dy, dz))
+HF1_exact = jnp.array(
+    [
+        [
+            2 * jnp.ones_like(X),  # ∂2F1/∂x2
+            0 * jnp.ones_like(X),  # ∂2F1/∂xy
+            0 * jnp.ones_like(X),  # ∂2F1/∂xz
+        ],
+        [
+            0 * jnp.ones_like(X),  # ∂2F1/∂yx
+            6 * Y**2,              # ∂2F1/∂y2
+            0 * jnp.ones_like(X),  # ∂2F1/∂yz
+        ],
+        [
+            0 * jnp.ones_like(X),  # ∂2F1/∂zx
+            0 * jnp.ones_like(X),  # ∂2F1/∂zy
+            0 * jnp.ones_like(X),  # ∂2F1/∂z2
+        ],
+    ]
+)
+npt.assert_allclose(JF, JF_exact, atol=1e-7)
+
+```
+
+</details>
 
 <details> 
 <summary> 
 PINN with Finite difference
 </summary>
 
-We will try to estimate NN(x)~f(x), where df(x)/dx = cos(x) and df(x)/dx will be represented with finite difference scheme
+We will try to estimate $NN(x)~f(x)$, where $df(x)/dx = cos(x)$ and $df(x)/dx$ will be represented with finite difference scheme. The following code compares between finite difference `fd` based implementation and automatic differentation `ad` based implementation.
 
 ```python
 import copy
 
 import jax
 import jax.numpy as jnp
 import matplotlib.pyplot as plt
@@ -737,23 +760,22 @@
 y_fd = NN_fd(x)
 y_ad = NN_ad(x)
 plt.plot(x, y, "--k", label="true")
 plt.plot(x, y_fd, label="fd pred")
 plt.plot(x, y_ad, label="ad pred")
 plt.legend()
 
-# Loss_fd 0.0012 
+# Loss_fd 0.0012
 # Loss_ad 0.0235
 ```
-![image](assets/fd_vs_ad.png)
 
+![image](assets/fd_vs_ad.png)
 
 </details>
 
-
 <details>
 <summary> 
 Reconstructing a vector field F using ∇.F = 0 and ∇xF=2k condition
 </summary>
 
 ```python
 import jax
@@ -783,18 +805,18 @@
 
 optim = optax.adam(1e-3)
 
 
 @jax.value_and_grad
 def loss_func(NN, F):
     F_pred = NN(F)
-    div = sk.fd.divergence(F_pred, accuracy=5, step_size=(dx, dy))  
+    div = sk.fd.divergence(F_pred, accuracy=5, step_size=(dx, dy))
     loss = jnp.mean(div**2)  # divergence free condition
     curl = sk.fd.curl(F_pred, accuracy=2, step_size=(dx, dy))
-    loss += jnp.mean((curl-jnp.ones_like(curl)*2)**2)  # curl condition 
+    loss += jnp.mean((curl-jnp.ones_like(curl)*2)**2)  # curl condition
     return loss
 
 
 @jax.jit
 def step(NN, F, optim_state):
     loss, grads = loss_func(NN, F)
     updates, optim_state = optim.update(grads, optim_state)
@@ -820,16 +842,153 @@
 plt.quiver(X, Y, F1, F2, color="k", alpha=0.5, label="true")
 plt.legend()
 
 ```
 
 ![image](assets/nn_div_free.svg)
 
+</details>
+
+<details>
+<summary>
+Vectorized differentiable stencil computation with `serket.kmap`
+</summary>
+
+Serket uses `kernex.kmap` decorator that applies a user-defined stencil kernel. `kmap` uses `jax.vmap` as it's backend to vectorized the operation, this means that the decorator is transparent to `jax` transformation.
+
+#### Example
+
+```python
+@sk.kmap(
+     # a kernel size applied to 2D input with size =3x3
+    kernel_size = (3,3),
+
+    # a strides = 1
+    strides= (1,1) ,
+
+    # padding can be among the following options
+    # 1) a single integer for each dimension -> ex: (1,) pads zeros before and after axis=0
+    # 2) a tuple of two integer for each dimension -> ex: ((1,2),) pads one zero on left and 2 zeros on right of axis=0
+    # 3) "same"/"valid"
+    # 4) "same"/"valid" tuple for each dimension -> ex: ("same",) same padding for axis=0
+    padding = "valid",
+
+    # relative means if the indexing should be row-col wise or center wise.
+    # for example in a 3x3  1..9 kernel , x[0,0] yields
+    # 1 if relative = False
+    # 5 if relative = True (i.e. the center value)
+    relative= True,
+
+)
+def avg_blur(x):
+    return (x[-1, -1] + x[-1, 0] + x[-1, 1] +
+            x[ 0, -1] + x[ 0, 0] + x[ 0, 1] +
+            x[ 1, -1] + x[ 1, 0] + x[ 1, 1]) // 9
+
+avg_blur(jnp.arange(1,26).reshape(5,5))
+# [[ 7  8  9]
+#  [12 13 14]
+#  [17 18 19]]
+```
+
+</details>
+
+<details>
+
+<summary>
+Scan a stencil kernel to solve linear convection using `serket.kscan`
+</summary>
+
+<div align ="center">
+
+$\Large {\partial u \over \partial t} + c {\partial u \over \partial x} = 0$ <br> <br>
+$\Large u_i^{n} = u_i^{n-1} - c \frac{\Delta t}{\Delta x}(u_i^{n-1}-u_{i-1}^{n-1})$
+
+<table>
+<tr>
+<td> Problem setup </td> <td> Stencil view  </td>
+</tr>
+<tr>
+<td>
+
+<img src="assets/linear_convection_init.png" width="500px">
+
+</td>
+<td>
+
+<img src="assets/linear_convection_view.png" width="500px">
+
+</td>
+</tr>
+</table>
+</div>
+
+By using `serket.kscan`, the stencil kernel can be scanned carrying along state, in a way similar to how RNN works. This enables BPTT algorithm that is useful for some problems (ex. time-dependent PDEs) .
+
+```python
+import jax
+import jax.numpy as jnp
+import serket as sk
+import matplotlib.pyplot as plt
+
+# see https://nbviewer.org/github/barbagroup/CFDPython/blob/master/lessons/01_Step_1.ipynb
+
+tmax,xmax = 0.5,2.0
+nt,nx = 151,51
+dt,dx = tmax/(nt-1) , xmax/(nx-1)
+u = jnp.ones([nt,nx])
+c = 0.5
+
+# kscan moves sequentially in row-major order and updates in-place using lax.scan.
+
+F = sk.kscan(
+        kernel_size = (3,3),
+        padding = ((1,1),(1,1)),
+        named_axis={0:'n',1:'i'},  # n for time axis , i for spatial axis (optional naming)
+        relative=True
+    )
+
+
+# boundary condtion as a function
+def bc(u):
+    return 1
+
+# initial condtion as a function
+def ic1(u):
+    return 1
+
+def ic2(u):
+    return 2
+
+def linear_convection(u):
+    return ( u['i','n-1'] - (c*dt/dx) * (u['i','n-1'] - u['i-1','n-1']) )
+
+
+F[:,0]  = F[:,-1] = bc # assign 1 for left and right boundary for all t
+
+# square wave initial condition
+F[:,:int((nx-1)/4)+1] = F[:,int((nx-1)/2):] = ic1
+F[0:1, int((nx-1)/4)+1 : int((nx-1)/2)] = ic2
+
+# assign linear convection function for
+# interior spatial location [1:-1]
+# and start from t>0  [1:]
+F[1:,1:-1] = linear_convection
+
+kx_solution = F(jnp.array(u))
+
+plt.figure(figsize=(20,7))
+for line in kx_solution[::20]:
+    plt.plot(jnp.linspace(0,xmax,nx),line)
+```
+
+![image](assets/linear_convection.svg)
 
 </details>
 
 ## 🥶 Freezing parameters /Fine tuning<a id="Freezing" >
 
 ✨[See here for more about freezing](https://github.com/ASEM000/PyTreeClass#%EF%B8%8F-model-surgery)✨
 
 ## 🔘 Filtering by masking<a id="Filtering" >
+
 ✨[See here for more about filterning ](https://github.com/ASEM000/PyTreeClass#%EF%B8%8F-filtering-with-at-)✨
```

### Comparing `serket-0.0.9/serket.egg-info/SOURCES.txt` & `serket-0.2.0b2/serket.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 LICENSE
-MANIFEST.in
 README.md
 setup.py
-requirements/requirements.txt
 serket/__init__.py
 serket/operators.py
 serket.egg-info/PKG-INFO
 serket.egg-info/SOURCES.txt
 serket.egg-info/dependency_links.txt
 serket.egg-info/not-zip-safe
 serket.egg-info/requires.txt
 serket.egg-info/top_level.txt
 serket/experimental/__init__.py
-serket/experimental/conv_semi_local.py
-serket/fd/__init__.py
-serket/fd/fgrad.py
-serket/fd/finite_diff.py
-serket/fd/utils.py
+serket/experimental/lazy_class.py
+serket/experimental/test_lazy_class.py
 serket/nn/__init__.py
 serket/nn/activation.py
 serket/nn/blur.py
+serket/nn/callbacks.py
 serket/nn/containers.py
 serket/nn/contrast.py
 serket/nn/convolution.py
 serket/nn/crop.py
 serket/nn/cutout.py
 serket/nn/dropout.py
+serket/nn/fft_convolution.py
 serket/nn/flatten.py
 serket/nn/flip.py
 serket/nn/fully_connected.py
 serket/nn/laplace.py
 serket/nn/linear.py
 serket/nn/normalization.py
 serket/nn/padding.py
@@ -43,28 +40,27 @@
 serket/nn/blocks/unet.py
 serket/nn/blocks/vgg.py
 tests/__init__.py
 tests/test_activation.py
 tests/test_blocks.py
 tests/test_blur.py
 tests/test_contrast.py
+tests/test_conv.py
 tests/test_convolution.py
 tests/test_crop.py
 tests/test_cutout.py
-tests/test_diff.py
 tests/test_dropout.py
-tests/test_fgrad.py
-tests/test_finite_diff.py
+tests/test_fft_convolution.py
 tests/test_flatten.py
 tests/test_flip.py
 tests/test_fully_connected.py
-tests/test_gradient.py
 tests/test_laplace2d.py
 tests/test_linear.py
 tests/test_normalization.py
 tests/test_padding.py
 tests/test_pooling.py
 tests/test_preprocessing.py
 tests/test_random_transformation.py
-tests/test_recurrent.py
 tests/test_repeat.py
-tests/test_sequential.py
+tests/test_rnn.py
+tests/test_sequential.py
+tests/test_utils.py
```

### Comparing `serket-0.0.9/setup.py` & `serket-0.2.0b2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,14 @@
                 version = line[line.find("=") + 1 :].strip(" '\"\n")
                 if version:
                     return version
         raise ValueError("`__version__` not defined in `serket/__init__.py`")
 
 
 def _parse_requirements(path):
-
     with open(os.path.join(_CURRENT_DIR, path)) as f:
         return [
             line.rstrip() for line in f if not (line.isspace() or line.startswith("#"))
         ]
 
 
 setup(
@@ -33,21 +32,17 @@
     author="Mahmoud Asem",
     description=("JAX NN library."),
     long_description=open(os.path.join(_CURRENT_DIR, "README.md")).read(),
     long_description_content_type="text/markdown",
     author_email="asem00@kaist.ac.kr",
     keywords="python machine-learning pytorch jax",
     packages=find_namespace_packages(exclude=['examples", "tests","experimental']),
-    install_requires=_parse_requirements(
-        os.path.join(_CURRENT_DIR, "requirements", "requirements.txt")
-    ),
-    # tests_require=_parse_requirements(
-    #     os.path.join(_CURRENT_DIR, 'requirements', 'requirements-test.txt')),
-    zip_safe=False,  # Required for full installation.
-    python_requires=">=3.7",
+    install_requires=["jax>=0.4.0", "pytreeclass>=0.3.0", "kernex"],
+    zip_safe=False,
+    python_requires=">=3.8",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
```

### Comparing `serket-0.0.9/tests/test_activation.py` & `serket-0.2.0b2/tests/test_activation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import jax
 import jax.numpy as jnp
 import numpy.testing as npt
 
 from serket.nn import (
     ELU,
     GELU,
```

### Comparing `serket-0.0.9/tests/test_blocks.py` & `serket-0.2.0b2/tests/test_blocks.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-import jax.numpy as jnp
-from pytreeclass.tree_viz.utils import _reduce_count_and_size
+from __future__ import annotations
 
-from serket.nn.blocks import UNetBlock, VGG16Block, VGG19Block
+# from serket.nn.blocks import UNetBlock, VGG16Block, VGG19Block
 
+# def test_vgg16_block():
+#     block = VGG16Block(3)
+#     count, _ = _reduce_count_and_size(block)
+#     assert count.real == 14_714_688
+#     model = VGG16Block(3)
+#     assert model(jnp.ones([3, 224, 224])).shape == (512, 1, 1)
 
-def test_vgg16_block():
-    block = VGG16Block(3)
-    count, _ = _reduce_count_and_size(block)
-    assert count.real == 14_714_688
-    model = VGG16Block(3)
-    assert model(jnp.ones([3, 224, 224])).shape == (512, 1, 1)
 
+# def test_vgg19_block():
+#     block = VGG19Block(3)
+#     count, _ = _reduce_count_and_size(block)
+#     assert count.real == 20_024_384
 
-def test_vgg19_block():
-    block = VGG19Block(3)
-    count, _ = _reduce_count_and_size(block)
-    assert count.real == 20_024_384
+#     model = VGG19Block(3)
+#     assert model(jnp.ones([3, 224, 224])).shape == (512, 1, 1)
 
-    model = VGG19Block(3)
-    assert model(jnp.ones([3, 224, 224])).shape == (512, 1, 1)
 
+# def test_unet_block():
+#     block = UNetBlock(3, 1, init_features=32)
+#     count, _ = _reduce_count_and_size(block)
+#     assert count.real == 7_757_153
 
-def test_unet_block():
-    block = UNetBlock(3, 1, init_features=32)
-    count, _ = _reduce_count_and_size(block)
-    assert count.real == 7_757_153
+#     model = UNetBlock(3, 1, 2)
 
-    model = UNetBlock(3, 1, 2)
-
-    assert model(jnp.ones((3, 320, 320))).shape == (1, 320, 320)
+#     assert model(jnp.ones((3, 320, 320))).shape == (1, 320, 320)
```

### Comparing `serket-0.0.9/tests/test_contrast.py` & `serket-0.2.0b2/tests/test_contrast.py`

 * *Files identical despite different names*

### Comparing `serket-0.0.9/tests/test_convolution.py` & `serket-0.2.0b2/tests/test_convolution.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-import jax
 import jax.numpy as jnp
-import jax.random as jr
-import jax.tree_util as jtu
 import numpy.testing as npt
 import pytest
 
 from serket.nn.convolution import (  # Conv3DLocal,; Conv1DSemiLocal,; Conv2DSemiLocal,; Conv3DSemiLocal,
     Conv1D,
     Conv1DLocal,
     Conv1DTranspose,
@@ -14,96 +11,24 @@
     Conv2DTranspose,
     Conv3D,
     Conv3DTranspose,
     DepthwiseConv1D,
     DepthwiseConv2D,
     SeparableConv1D,
     SeparableConv2D,
-    _check_and_return_init_func,
-    _check_and_return_input_dilation,
-    _check_and_return_kernel,
-    _check_and_return_padding,
-    _check_and_return_strides,
 )
 
 
-def test_check_and_return_init_func():
-    _check_partial = lambda f: _check_and_return_init_func(f, "test")
-    k = jr.PRNGKey(0)
-
-    assert _check_partial("he_normal")(k, (2, 2)).shape == (2, 2)
-    assert _check_partial("he_uniform")(k, (2, 2)).shape == (2, 2)
-    assert _check_partial("glorot_normal")(k, (2, 2)).shape == (2, 2)
-    assert _check_partial("glorot_uniform")(k, (2, 2)).shape == (2, 2)
-    assert _check_partial("lecun_normal")(k, (2, 2)).shape == (2, 2)
-    assert _check_partial("lecun_uniform")(k, (2, 2)).shape == (2, 2)
-    assert _check_partial("normal")(k, (2, 2)).shape == (2, 2)
-    assert _check_partial("uniform")(k, (2, 2)).shape == (2, 2)
-    assert _check_partial("ones")(k, (2, 2)).shape == (2, 2)
-    assert _check_partial("zeros")(k, (2, 2)).shape == (2, 2)
-    assert _check_partial("xavier_normal")(k, (2, 2)).shape == (2, 2)
-    assert _check_partial("xavier_uniform")(k, (2, 2)).shape == (2, 2)
-
-    assert isinstance(_check_partial(jax.nn.initializers.he_normal()), jtu.Partial)
-    assert isinstance(_check_partial(None), type(None))
-
-    with pytest.raises(ValueError):
-        _check_partial("invalid")
-
-    with pytest.raises(ValueError):
-        _check_partial(1)
-
-
-def test_check_and_return():
-
-    assert _check_and_return_kernel(3, 2) == (3, 3)
-    assert _check_and_return_kernel((3, 3), 2) == (3, 3)
-    assert _check_and_return_kernel((3, 3, 3), 3) == (3, 3, 3)
-
-    with pytest.raises(AssertionError):
-        _check_and_return_kernel((3, 3), 3)
-
-    with pytest.raises(AssertionError):
-        _check_and_return_kernel((3, 3, 3), 2)
-
-    with pytest.raises(AssertionError):
-        _check_and_return_kernel((3, 3, 3), 1)
-
-    assert _check_and_return_input_dilation(3, 2) == (3, 3)
-    assert _check_and_return_input_dilation((3, 3), 2) == (3, 3)
-    assert _check_and_return_input_dilation((3, 3, 3), 3) == (3, 3, 3)
-
-    assert _check_and_return_strides(3, 2) == (3, 3)
-    assert _check_and_return_strides((3, 3), 2) == (3, 3)
-    assert _check_and_return_strides((3, 3, 3), 3) == (3, 3, 3)
-
-
-def test_check_and_return_padding():
-    assert _check_and_return_padding(1, (3, 3)) == ((1, 1), (1, 1))
-    assert _check_and_return_padding(0, (3, 3)) == ((0, 0), (0, 0))
-    assert _check_and_return_padding(2, (3, 3)) == ((2, 2), (2, 2))
-
-    assert _check_and_return_padding((1, 1), (3, 3)) == ((1, 1), (1, 1))
-    assert _check_and_return_padding(((1, 1), (1, 1)), (3, 3)) == ((1, 1), (1, 1))
-    assert _check_and_return_padding(("same", "same"), (3, 3)) == ((1, 1), (1, 1))
-    assert _check_and_return_padding(("valid", "valid"), (3, 3)) == ((0, 0), (0, 0))
-    with pytest.raises(ValueError):
-        _check_and_return_padding(("invalid", "valid"), (3, 3))
-
-    with pytest.raises(ValueError):
-        _check_and_return_padding(("valid", "invalid"), (3, 3))
-
-    with pytest.raises(ValueError):
-        _check_and_return_padding(("invalid", {}), (3, 3))
-
-
 def test_conv1D():
-
     layer = Conv1D(
-        in_features=1, out_features=1, kernel_size=2, padding="SAME", strides=1
+        in_features=1,
+        out_features=1,
+        kernel_size=2,
+        padding="SAME",
+        strides=1,
     )
 
     layer = layer.at["weight"].set(jnp.ones([1, 1, 2], dtype=jnp.float32))  # OIW
     x = jnp.arange(1, 11).reshape([1, 10]).astype(jnp.float32)
     npt.assert_allclose(layer(x), jnp.array([[3, 5, 7, 9, 11, 13, 15, 17, 19, 10]]))
 
     layer = Conv1D(
@@ -186,15 +111,14 @@
         1, 2, 3, padding=2, strides=1, kernel_dilation=2, bias_init_func=None
     )
     layer = layer.at["weight"].set(w)
     npt.assert_allclose(layer(x), y)
 
 
 def test_conv2D():
-
     layer = Conv2D(in_features=1, out_features=1, kernel_size=2)
     layer = layer.at["weight"].set(jnp.ones([1, 1, 2, 2], dtype=jnp.float32))  # OIHW
     x = jnp.arange(1, 17).reshape([1, 4, 4]).astype(jnp.float32)
 
     npt.assert_allclose(
         layer(x)[0],
         jnp.array(
@@ -265,15 +189,14 @@
         jnp.array(
             [[14, 18, 22, 12], [30, 34, 38, 20], [46, 50, 54, 28], [27, 29, 31, 16]]
         ),
     )
 
 
 def test_conv3D():
-
     layer = Conv3D(1, 3, 3)
     layer = layer.at["weight"].set(jnp.ones([3, 1, 3, 3, 3]))
     layer = layer.at["bias"].set(jnp.zeros([3, 1, 1, 1]))
     npt.assert_allclose(
         layer(jnp.ones([1, 1, 3, 3])),
         jnp.tile(jnp.array([[4, 6, 4], [6, 9, 6], [4, 6, 4]]), [3, 1, 1, 1]),
     )
@@ -360,15 +283,15 @@
                 ],
             ]
         ]
     )
 
     b = jnp.array([[[0.0]]])
 
-    layer = Conv2DTranspose(4, 1, 3, padding=2, strides=1, kernel_dilation=2)
+    layer = Conv2DTranspose(3, 1, 3, padding=2, strides=1, kernel_dilation=2)
 
     layer = layer.at["weight"].set(w)
     layer = layer.at["bias"].set(b)
 
     y = jnp.array(
         [
             [
@@ -379,15 +302,15 @@
             ]
         ]
     )
 
     npt.assert_allclose(layer(x), y, atol=1e-5)
 
     layer = Conv2DTranspose(
-        4, 1, 3, padding=2, strides=1, kernel_dilation=2, bias_init_func=None
+        3, 1, 3, padding=2, strides=1, kernel_dilation=2, bias_init_func=None
     )
 
     layer = layer.at["weight"].set(w)
 
     y = jnp.array(
         [
             [
@@ -399,15 +322,14 @@
         ]
     )
 
     npt.assert_allclose(layer(x), y, atol=1e-5)
 
 
 def test_conv3dtranspose():
-
     x = jnp.array(
         [
             [
                 [
                     [0.9922036, 0.8135023, 0.4357065],
                     [0.5499866, 0.16954863, 0.7430643],
                     [0.43268728, 0.39654946, 0.4743309],
@@ -656,15 +578,14 @@
     layer = DepthwiseConv1D(in_features=5, kernel_size=3, depth_multiplier=2)
     layer = layer.at["weight"].set(w)
 
     npt.assert_allclose(y, layer(x), atol=1e-5)
 
 
 def test_depthwise_conv2d():
-
     w = jnp.array(
         [
             [
                 [
                     [-0.2693168, -0.01502147, 0.15012494],
                     [-0.00952473, 0.2306507, -0.18514359],
                     [0.42974612, 0.01279813, -0.3835524],
@@ -721,15 +642,14 @@
     layer = DepthwiseConv2D(2, 3)
     layer = layer.at["weight"].set(w)
 
     npt.assert_allclose(y, layer(x), atol=1e-5)
 
 
 def test_seperable_conv1d():
-
     x = jnp.array(
         [
             [0.60440326, 0.44108868, 0.89211035, 0.86819136, 0.99565816],
             [0.9063431, 0.64626694, 0.97458243, 0.163221, 0.24878585],
         ]
     )
 
@@ -746,16 +666,16 @@
 
     y = jnp.array([[0.5005436, 0.44051802, 0.5662357, 0.13085097, -0.22720146]])
 
     layer = SeparableConv1D(
         in_features=2, out_features=1, kernel_size=3, depth_multiplier=2
     )
 
-    layer = layer.at["depthwise_conv.weight"].set(w1)
-    layer = layer.at["pointwise_conv.weight"].set(w2)
+    layer = layer.at["depthwise_conv"].at["weight"].set(w1)
+    layer = layer.at["pointwise_conv"].at["weight"].set(w2)
 
     npt.assert_allclose(y, layer(x), atol=1e-5)
 
 
 def test_seperable_conv2d():
     x = jnp.array(
         [
@@ -823,16 +743,16 @@
         ]
     )
 
     layer_jax = SeparableConv2D(
         in_features=2, out_features=1, kernel_size=3, depth_multiplier=2
     )
 
-    layer_jax = layer_jax.at["depthwise_conv.weight"].set(w1)
-    layer_jax = layer_jax.at["pointwise_conv.weight"].set(w2)
+    layer_jax = layer_jax.at["depthwise_conv"].at["weight"].set(w1)
+    layer_jax = layer_jax.at["pointwise_conv"].at["weight"].set(w2)
 
     npt.assert_allclose(y, layer_jax(x), atol=1e-5)
 
 
 def test_conv1d_local():
     x = jnp.ones((2, 28))
 
@@ -964,15 +884,14 @@
 
     layer = layer.at["weight"].set(w)
 
     npt.assert_allclose(y, layer(x), atol=1e-5)
 
 
 def test_conv2d_local():
-
     w = jnp.array(
         [
             [
                 [[-0.21994266, -0.2716022]],
                 [[0.2665612, -0.15465173]],
                 [[0.08909398, -0.36371586]],
                 [[0.1832841, -0.07327542]],
@@ -1027,15 +946,14 @@
         DepthwiseConv1D(0, 1)
 
     with pytest.raises(ValueError):
         DepthwiseConv2D(0, 1)
 
 
 def test_out_feature_error():
-
     with pytest.raises(ValueError):
         Conv1D(1, 0, 2)
 
     with pytest.raises(ValueError):
         Conv2D(1, 0, 2)
 
     with pytest.raises(ValueError):
@@ -1054,15 +972,14 @@
         Conv2DTranspose(1, 0, 3)
 
     with pytest.raises(ValueError):
         Conv3DTranspose(1, 0, 3)
 
 
 def test_groups_error():
-
     with pytest.raises(ValueError):
         Conv1D(1, 1, 2, groups=0)
 
     with pytest.raises(ValueError):
         Conv2D(1, 1, 2, groups=0)
 
     with pytest.raises(ValueError):
@@ -1074,104 +991,79 @@
     with pytest.raises(ValueError):
         Conv2DTranspose(1, 1, 3, groups=0)
 
     with pytest.raises(ValueError):
         Conv3DTranspose(1, 1, 3, groups=0)
 
 
-def test_lazy_conv():
-    layer = Conv1D(None, 1, 3)
-    assert layer.weight is None
-    assert layer(jnp.ones([10, 3])).shape == (1, 3)
-
-    layer = Conv2D(None, 1, 3)
-    assert layer.weight is None
-    assert layer(jnp.ones([10, 3, 3])).shape == (1, 3, 3)
-
-    layer = Conv3D(None, 1, 3)
-    assert layer.weight is None
-    assert layer(jnp.ones([10, 3, 3, 3])).shape == (1, 3, 3, 3)
-
-    layer = Conv1DTranspose(None, 1, 3)
-    assert layer.weight is None
-    assert layer(jnp.ones([10, 3])).shape == (1, 3)
-
-    layer = Conv2DTranspose(None, 1, 3)
-    assert layer.weight is None
-    assert layer(jnp.ones([10, 3, 3])).shape == (1, 3, 3)
-
-    layer = Conv3DTranspose(None, 1, 3)
-    assert layer.weight is None
-    assert layer(jnp.ones([10, 3, 3, 3])).shape == (1, 3, 3, 3)
+# def test_lazy_conv():
+#     layer = Conv1D(None, 1, 3)
+#     assert layer(jnp.ones([10, 3])).shape == (1, 3)
 
-    layer = DepthwiseConv1D(None, 3)
-    assert layer.weight is None
-    assert layer(jnp.ones([10, 3])).shape == (10, 3)
+#     layer = Conv2D(None, 1, 3)
+#     assert layer(jnp.ones([10, 3, 3])).shape == (1, 3, 3)
 
-    layer = DepthwiseConv2D(None, 3)
-    assert layer.weight is None
-    assert layer(jnp.ones([10, 3, 3])).shape == (10, 3, 3)
+#     layer = Conv3D(None, 1, 3)
+#     assert layer(jnp.ones([10, 3, 3, 3])).shape == (1, 3, 3, 3)
 
-    layer = Conv1DLocal(None, 1, 3, in_size=(3,))
-    assert layer.weight is None
-    assert layer(jnp.ones([10, 3])).shape == (1, 3)
+#     layer = Conv1DTranspose(None, 1, 3)
+#     assert layer(jnp.ones([10, 3])).shape == (1, 3)
 
-    layer = Conv2DLocal(None, 1, 3, in_size=(3, 3))
-    assert layer.weight is None
-    assert layer(jnp.ones([10, 3, 3])).shape == (1, 3, 3)
+#     layer = Conv2DTranspose(None, 1, 3)
+#     assert layer(jnp.ones([10, 3, 3])).shape == (1, 3, 3)
 
-    layer = SeparableConv1D(None, 1, 3)
-    assert layer(jnp.ones([10, 3])).shape == (1, 3)
+#     layer = Conv3DTranspose(None, 1, 3)
+#     assert layer(jnp.ones([10, 3, 3, 3])).shape == (1, 3, 3, 3)
 
-    layer = SeparableConv2D(None, 1, 3)
-    assert layer(jnp.ones([10, 3, 3])).shape == (1, 3, 3)
+#     layer = DepthwiseConv1D(None, 3)
+#     assert layer(jnp.ones([10, 3])).shape == (10, 3)
 
-    with pytest.raises(ValueError):
-        jax.jit(Conv1D(None, 1, 3))(jnp.ones([10, 3]))
+#     layer = DepthwiseConv2D(None, 3)
+#     assert layer(jnp.ones([10, 3, 3])).shape == (10, 3, 3)
 
-    with pytest.raises(ValueError):
-        jax.jit(Conv2D(None, 1, 3))(jnp.ones([10, 3, 3]))
+#     layer = Conv1DLocal(None, 1, 3, in_size=(3,))
+#     assert layer(jnp.ones([10, 3])).shape == (1, 3)
 
-    with pytest.raises(ValueError):
-        jax.jit(Conv3D(None, 1, 3))(jnp.ones([10, 3, 3, 3]))
+#     layer = Conv2DLocal(None, 1, 3, in_size=(3, 3))
+#     assert layer(jnp.ones([10, 3, 3])).shape == (1, 3, 3)
 
-    with pytest.raises(ValueError):
-        jax.jit(Conv1DTranspose(None, 1, 3))(jnp.ones([10, 3]))
+#     layer = SeparableConv1D(None, 1, 3)
+#     assert layer(jnp.ones([10, 3])).shape == (1, 3)
 
-    with pytest.raises(ValueError):
-        jax.jit(Conv2DTranspose(None, 1, 3))(jnp.ones([10, 3, 3]))
+#     layer = SeparableConv2D(None, 1, 3)
+#     assert layer(jnp.ones([10, 3, 3])).shape == (1, 3, 3)
 
-    with pytest.raises(ValueError):
-        jax.jit(Conv3DTranspose(None, 1, 3))(jnp.ones([10, 3, 3, 3]))
+#     with pytest.raises(ConcretizationTypeError):
+#         jax.jit(Conv1D(None, 1, 3))(jnp.ones([10, 3]))
 
-    with pytest.raises(ValueError):
-        jax.jit(DepthwiseConv1D(None, 3))(jnp.ones([10, 3]))
+#     with pytest.raises(ConcretizationTypeError):
+#         jax.jit(Conv2D(None, 1, 3))(jnp.ones([10, 3, 3]))
 
-    with pytest.raises(ValueError):
-        jax.jit(DepthwiseConv2D(None, 3))(jnp.ones([10, 3, 3]))
-
-    with pytest.raises(ValueError):
-        jax.jit(Conv1DLocal(None, 1, 3, in_size=(3,)))(jnp.ones([10, 3]))
+#     with pytest.raises(ConcretizationTypeError):
+#         jax.jit(Conv3D(None, 1, 3))(jnp.ones([10, 3, 3, 3]))
 
-    with pytest.raises(ValueError):
-        jax.jit(Conv2DLocal(None, 1, 3, in_size=(3, 3)))(jnp.ones([10, 3, 3]))
+#     with pytest.raises(ConcretizationTypeError):
+#         jax.jit(Conv1DTranspose(None, 1, 3))(jnp.ones([10, 3]))
 
-    with pytest.raises(ValueError):
-        jax.jit(SeparableConv1D(None, 1, 3))(jnp.ones([10, 3]))
+#     with pytest.raises(ConcretizationTypeError):
+#         jax.jit(Conv2DTranspose(None, 1, 3))(jnp.ones([10, 3, 3]))
 
-    with pytest.raises(ValueError):
-        jax.jit(SeparableConv2D(None, 1, 3))(jnp.ones([10, 3, 3]))
+#     with pytest.raises(ConcretizationTypeError):
+#         jax.jit(Conv3DTranspose(None, 1, 3))(jnp.ones([10, 3, 3, 3]))
 
+#     with pytest.raises(ConcretizationTypeError):
+#         jax.jit(DepthwiseConv1D(None, 3))(jnp.ones([10, 3]))
 
-# def test_conv1d_semilocal():
-#     layer = Conv1DSemiLocal(1, 3, 3)
-#     assert layer(jnp.ones([1, 3])).shape == (3, 3)
+#     with pytest.raises(ConcretizationTypeError):
+#         jax.jit(DepthwiseConv2D(None, 3))(jnp.ones([10, 3, 3]))
 
+#     with pytest.raises(ConcretizationTypeError):
+#         jax.jit(Conv1DLocal(None, 1, 3, in_size=(3,)))(jnp.ones([10, 3]))
 
-# def test_conv2d_semilocal():
-#     layer = Conv2DSemiLocal(1, 3, 3)
-#     assert layer(jnp.ones([1, 3, 3])).shape == (3, 3, 3)
+#     with pytest.raises(ConcretizationTypeError):
+#         jax.jit(Conv2DLocal(None, 1, 3, in_size=(3, 3)))(jnp.ones([10, 3, 3]))
 
+#     with pytest.raises(ConcretizationTypeError):
+#         jax.jit(SeparableConv1D(None, 1, 3))(jnp.ones([10, 3]))
 
-# def test_conv3d_semilocal():
-#     layer = Conv3DSemiLocal(1, 3, 3)
-#     assert layer(jnp.ones([1, 3, 3, 3])).shape == (3, 3, 3, 3)
+#     with pytest.raises(ConcretizationTypeError):
+#         jax.jit(SeparableConv2D(None, 1, 3))(jnp.ones([10, 3, 3]))
```

### Comparing `serket-0.0.9/tests/test_crop.py` & `serket-0.2.0b2/tests/test_crop.py`

 * *Files identical despite different names*

### Comparing `serket-0.0.9/tests/test_cutout.py` & `serket-0.2.0b2/tests/test_cutout.py`

 * *Files identical despite different names*

### Comparing `serket-0.0.9/tests/test_flatten.py` & `serket-0.2.0b2/tests/test_flatten.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import jax.numpy as jnp
 
 from serket.nn.flatten import Flatten, Unflatten
 
 
 def test_flatten():
-
     assert Flatten(0, 1)(jnp.ones([1, 2, 3, 4, 5])).shape == (2, 3, 4, 5)
     assert Flatten(0, 2)(jnp.ones([1, 2, 3, 4, 5])).shape == (6, 4, 5)
     assert Flatten(1, 2)(jnp.ones([1, 2, 3, 4, 5])).shape == (1, 6, 4, 5)
     assert Flatten(-1, -1)(jnp.ones([1, 2, 3, 4, 5])).shape == (1, 2, 3, 4, 5)
     assert Flatten(-2, -1)(jnp.ones([1, 2, 3, 4, 5])).shape == (1, 2, 3, 20)
     assert Flatten(-3, -1)(jnp.ones([1, 2, 3, 4, 5])).shape == (1, 2, 60)
 
 
 def test_unflatten():
-
     assert Unflatten(0, (1, 2, 3))(jnp.ones([6])).shape == (1, 2, 3)
     assert Unflatten(0, (1, 2, 3))(jnp.ones([6, 4])).shape == (1, 2, 3, 4)
```

### Comparing `serket-0.0.9/tests/test_flip.py` & `serket-0.2.0b2/tests/test_flip.py`

 * *Files identical despite different names*

### Comparing `serket-0.0.9/tests/test_fully_connected.py` & `serket-0.2.0b2/tests/test_fully_connected.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,50 @@
-import jax.numpy as jnp
-import pytest
+# import jax.numpy as jnp
+# import pytest
 
-from serket.nn import PFNN, Linear
+# from serket.nn import PFNN, Linear
 
 
-def test_PFNN():
+# def test_PFNN():
 
-    with pytest.raises(ValueError):
-        PFNN([1, 2, [3, 2], 3, 2])
+#     with pytest.raises(ValueError):
+#         PFNN([1, 2, [3, 2], 3, 2])
 
-    with pytest.raises(ValueError):
-        PFNN([1, 2, [3, 2], 3, 2])
+#     with pytest.raises(ValueError):
+#         PFNN([1, 2, [3, 2], 3, 2])
 
-    with pytest.raises(AssertionError):
-        PFNN([1, 2, [3, 2], 3, 1])
+#     with pytest.raises(AssertionError):
+#         PFNN([1, 2, [3, 2], 3, 1])
 
-    with pytest.raises(TypeError):
-        PFNN([1, 2, [3, "a"], 3, 2])
+#     with pytest.raises(TypeError):
+#         PFNN([1, 2, [3, "a"], 3, 2])
 
-    assert PFNN([1, 2]).layers == [[Linear(1, 1)]] * 2
-    assert PFNN([1, [2, 3], 2]).layers == [
-        [Linear(1, 2), Linear(2, 1)],
-        [Linear(1, 3), Linear(3, 1)],
-    ]
-    assert PFNN([1, 2, 3]).layers == [[Linear(1, 2), Linear(2, 1)]] * 3
+#     assert PFNN([1, 2]).layers == [[Linear(1, 1)]] * 2
+#     assert PFNN([1, [2, 3], 2]).layers == [
+#         [Linear(1, 2), Linear(2, 1)],
+#         [Linear(1, 3), Linear(3, 1)],
+#     ]
+#     assert PFNN([1, 2, 3]).layers == [[Linear(1, 2), Linear(2, 1)]] * 3
 
-    assert PFNN([1, [2, 2, 2], 3]).layers == [[Linear(1, 2), Linear(2, 1)]] * 3
-    assert PFNN([1, [2, 3, 4], 3]).layers == [
-        [Linear(1, 2), Linear(2, 1)],
-        [Linear(1, 3), Linear(3, 1)],
-        [Linear(1, 4), Linear(4, 1)],
-    ]
+#     assert PFNN([1, [2, 2, 2], 3]).layers == [[Linear(1, 2), Linear(2, 1)]] * 3
+#     assert PFNN([1, [2, 3, 4], 3]).layers == [
+#         [Linear(1, 2), Linear(2, 1)],
+#         [Linear(1, 3), Linear(3, 1)],
+#         [Linear(1, 4), Linear(4, 1)],
+#     ]
 
-    assert PFNN([1, [2, 3, 4],[1,1,1], 3]).layers == [
-        [Linear(1, 2), Linear(2, 1),Linear(1, 1)],
-        [Linear(1, 3), Linear(3, 1),Linear(1, 1)],
-        [Linear(1, 4), Linear(4, 1),Linear(1, 1)],
-    ]
+#     assert PFNN([1, [2, 3, 4],[1,1,1], 3]).layers == [
+#         [Linear(1, 2), Linear(2, 1),Linear(1, 1)],
+#         [Linear(1, 3), Linear(3, 1),Linear(1, 1)],
+#         [Linear(1, 4), Linear(4, 1),Linear(1, 1)],
+#     ]
 
-    with pytest.raises(TypeError):
-        PFNN([1, [2, "a", 2], 3])
+#     with pytest.raises(TypeError):
+#         PFNN([1, [2, "a", 2], 3])
 
-    assert PFNN([1, [2, 3], 2])(jnp.ones([1, 1])).shape == (1, 2)
+#     assert PFNN([1, [2, 3], 2])(jnp.ones([1, 1])).shape == (1, 2)
 
-    with pytest.raises(AssertionError):
-        PFNN([1,[2,3],[3,4,5],2])
-
-    with pytest.raises(TypeError):
-        PFNN([1,"a",[3,4,5],2])
-    
+#     with pytest.raises(AssertionError):
+#         PFNN([1,[2,3],[3,4,5],2])
 
+#     with pytest.raises(TypeError):
+#         PFNN([1,"a",[3,4,5],2])
```

### Comparing `serket-0.0.9/tests/test_laplace2d.py` & `serket-0.2.0b2/tests/test_laplace2d.py`

 * *Files identical despite different names*

### Comparing `serket-0.0.9/tests/test_linear.py` & `serket-0.2.0b2/tests/test_linear.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,57 @@
 import jax
 import jax.numpy as jnp
+import jax.tree_util as jtu
 import numpy.testing as npt
 import pytest
 import pytreeclass as pytc
 
-from serket.nn import FNN, Bilinear, GeneralLinear, Identity, Linear, Multilinear
+from serket.nn import (
+    FNN,
+    Bilinear,
+    Embedding,
+    GeneralLinear,
+    Identity,
+    Linear,
+    MergeLinear,
+    Multilinear,
+)
+
+
+def test_embed():
+    table = Embedding(10, 3)
+    x = jnp.array([9])
+    npt.assert_allclose(table(x), jnp.array([[0.43810904, 0.35078037, 0.13254273]]))
+
+    with pytest.raises(TypeError):
+        table(jnp.array([9.0]))
 
 
 def test_linear():
     x = jnp.linspace(0, 1, 100)[:, None]
     y = x**3 + jax.random.uniform(jax.random.PRNGKey(0), (100, 1)) * 0.01
 
     @jax.value_and_grad
-    def loss_func(model, x, y):
-        return jnp.mean((model(x) - y) ** 2)
+    def loss_func(NN, x, y):
+        NN = NN.at[...].apply(pytc.unfreeze, is_leaf=pytc.is_frozen)
+        return jnp.mean((NN(x) - y) ** 2)
 
     @jax.jit
-    def update(model, x, y):
-        value, grad = loss_func(model, x, y)
-        return value, model - 1e-3 * grad
+    def update(NN, x, y):
+        value, grad = loss_func(NN, x, y)
+        return value, jtu.tree_map(lambda x, g: x - 1e-3 * g, NN, grad)
+
+    NN = FNN([1, 128, 128, 1])
 
-    model = FNN([1, 128, 128, 1])
+    # NN = jtu.tree_map(lambda x: pytc.freeze(x) if pytc.is_nondiff(x) else x, NN)
+    NN = NN.at[pytc.bcmap(pytc.is_nondiff)(NN)].apply(pytc.freeze)
 
-    model = pytc.filter_nondiff(model)
-    print(model.tree_diagram())
+    # print(pytc.tree_diagram(NN))
     for _ in range(20_000):
-        value, model = update(model, x, y)
+        value, NN = update(NN, x, y)
 
     npt.assert_allclose(jnp.array(4.933563e-05), value, atol=1e-3)
 
     layer = Linear(1, 1, bias_init_func=None)
     w = jnp.array([[-0.31568417]])
     layer = layer.at["weight"].set(w)
     y = jnp.array([[-0.31568417]])
@@ -66,42 +88,20 @@
 
 def test_identity():
     x = jnp.array([[1, 2, 3], [4, 5, 6]])
     layer = Identity()
     npt.assert_allclose(x, layer(x))
 
 
-def test_lazy():
-
-    layer = Linear(None, 1)
-    assert layer.weight is None
-    assert layer(jnp.ones([10, 2])).shape == (10, 1)
-
-    layer = Bilinear(None, None, 1)
-    assert layer.weight is None
-    assert layer(jnp.ones([10, 2]), jnp.ones([10, 3])).shape == (10, 1)
-
-    with pytest.raises(ValueError):
-        layer = jax.jit(Linear(None, 1))
-        layer(jnp.ones([10, 2]))
-
-    with pytest.raises(ValueError):
-        layer = jax.jit(Bilinear(None, None, 1))
-        layer(jnp.ones([10, 2]), jnp.ones([10, 3]))
-
-
 def test_multi_linear():
     x = jnp.linspace(0, 1, 100)[:, None]
     lhs = Linear(1, 10)
     rhs = Multilinear((1,), 10)
     npt.assert_allclose(lhs(x), rhs(x), atol=1e-4)
 
-    lhs = Multilinear(None, 10)
-    assert lhs(x, x, x).shape == (100, 10)
-
     with pytest.raises(ValueError):
         Multilinear([1, 2], 10)
 
 
 def test_general_linear():
     x = jnp.ones([1, 2, 3, 4])
     layer = GeneralLinear(in_features=(1, 2), in_axes=(0, 1), out_features=5)
@@ -115,21 +115,32 @@
     layer = GeneralLinear(in_features=(1, 2), in_axes=(0, -3), out_features=5)
     assert layer(x).shape == (3, 4, 5)
 
     x = jnp.ones([1, 2, 3, 4])
     layer = GeneralLinear(in_features=(2, 3), in_axes=(1, -2), out_features=5)
     assert layer(x).shape == (1, 4, 5)
 
-    with pytest.raises(ValueError):
+    with pytest.raises(TypeError):
         GeneralLinear(in_features=2, in_axes=(1, -2), out_features=5)
 
-    with pytest.raises(ValueError):
+    with pytest.raises(TypeError):
         GeneralLinear(in_features=(2, 3), in_axes=2, out_features=5)
 
     with pytest.raises(ValueError):
         GeneralLinear(in_features=(1,), in_axes=(0, -3), out_features=5)
 
 
-def test_lazy_general_linear():
-    x = jnp.ones([1, 2, 3, 4])
-    layer = GeneralLinear(None, in_axes=(0, 1), out_features=5)
-    assert layer(x).shape == (3, 4, 5)
+def test_merge_linear():
+    layer1 = Linear(5, 6)  # 5 input features, 6 output features
+    layer2 = Linear(7, 6)  # 7 input features, 6 output features
+    merged_layer = MergeLinear(layer1, layer2)  # 12 input features, 6 output features
+    x1 = jnp.ones([1, 5])  # 1 sample, 5 features
+    x2 = jnp.ones([1, 7])  # 1 sample, 7 features
+    y = merged_layer(x1, x2)
+    z = layer1(x1) + layer2(x2)
+    npt.assert_allclose(y, z, atol=1e-6)
+
+    with pytest.raises(ValueError):
+        # output features of layer1 and layer2 mismatch
+        l1 = Linear(5, 6)
+        l2 = Linear(7, 8)
+        MergeLinear(l1, l2)
```

### Comparing `serket-0.0.9/tests/test_normalization.py` & `serket-0.2.0b2/tests/test_normalization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-import jax
 import jax.numpy as jnp
 import numpy.testing as npt
 import pytest
 
 from serket.nn import GroupNorm, InstanceNorm, LayerNorm
 
 
 def test_LayerNorm():
-
     layer = LayerNorm((5, 2), affine=False)
 
     x = jnp.array(
         [
             [10, 12],
             [20, 22],
             [30, 32],
@@ -30,15 +28,14 @@
         ]
     )
 
     npt.assert_allclose(layer(x), y, atol=1e-5)
 
 
 def test_InstanceNorm():
-
     x = jnp.array(
         [
             [
                 [-1.1472481, -1.9474537, -2.0057163, 0.6425913, 0.36222667],
                 [-1.2547379, 0.9062948, 0.17921783, 1.3880836, -0.27561226],
                 [-1.257894, -0.8935803, 1.2161034, 0.19008707, 1.4399774],
                 [1.3984185, -1.0334028, -0.24350524, -1.1016859, -2.2860343],
@@ -87,15 +84,14 @@
 
     layer = InstanceNorm(in_features=3, affine=False)
 
     npt.assert_allclose(layer(x), y, atol=1e-5)
 
 
 def test_group_norm():
-
     x = jnp.array(
         [
             [
                 [-0.63612133, 0.19765279, 2.1146476],
                 [0.031331, -1.311904, -0.0374171],
                 [-0.54120636, -0.6456455, 0.9654913],
                 [0.2920794, -0.22726963, -0.24639332],
@@ -196,15 +192,14 @@
     with pytest.raises(ValueError):
         layer = GroupNorm(in_features=0, groups=1)
 
     with pytest.raises(ValueError):
         layer = GroupNorm(in_features=-1, groups=0)
 
 
-def test_lazy_normalization():
-    layer = GroupNorm(None, groups=1)
-    assert layer.groups is None
-    assert layer(jnp.ones([1, 2, 3, 4])).shape == (1, 2, 3, 4)
-
-    with pytest.raises(ValueError):
-        layer = jax.jit(GroupNorm(None, groups=1))
-        layer(jnp.ones([1, 2, 3, 4]))
+# def test_lazy_normalization():
+#     layer = GroupNorm(None, groups=1)
+#     assert layer(jnp.ones([1, 2, 3, 4])).shape == (1, 2, 3, 4)
+
+#     with pytest.raises(ConcretizationTypeError):
+#         layer = jax.jit(GroupNorm(None, groups=1))
+#         layer(jnp.ones([1, 2, 3, 4]))
```

### Comparing `serket-0.0.9/tests/test_padding.py` & `serket-0.2.0b2/tests/test_padding.py`

 * *Files identical despite different names*

### Comparing `serket-0.0.9/tests/test_pooling.py` & `serket-0.2.0b2/tests/test_pooling.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,14 @@
 import jax.numpy as jnp
 import numpy.testing as npt
 
 from serket.nn.pooling import (
     AdaptiveAvgPool1D,
     AdaptiveAvgPool2D,
     AdaptiveAvgPool3D,
-    AdaptiveConcatPool1D,
-    AdaptiveConcatPool2D,
-    AdaptiveConcatPool3D,
     AdaptiveMaxPool1D,
     AdaptiveMaxPool2D,
     AdaptiveMaxPool3D,
     AvgPool1D,
     AvgPool2D,
     AvgPool3D,
     GlobalAvgPool1D,
@@ -29,15 +26,14 @@
     MaxPool1D,
     MaxPool2D,
     MaxPool3D,
 )
 
 
 def test_MaxPool1D():
-
     layer = MaxPool1D(kernel_size=2, padding="SAME", strides=1)
     x = jnp.arange(1, 11).reshape(1, 10).astype(jnp.float32)
     npt.assert_allclose(layer(x), jnp.array([[2, 3, 4, 5, 6, 7, 8, 9, 10, 10]]))
 
     layer = MaxPool1D(kernel_size=2, padding="SAME", strides=2)
     npt.assert_allclose(layer(x), jnp.array([[2, 4, 6, 8, 10]]))
 
@@ -45,15 +41,14 @@
     npt.assert_allclose(layer(x), jnp.array([[2, 3, 4, 5, 6, 7, 8, 9, 10]]))
 
     layer = MaxPool1D(kernel_size=2, padding="VALID", strides=2)
     npt.assert_allclose(layer(x), jnp.array([[2, 4, 6, 8, 10]]))
 
 
 def test_MaxPool2D():
-
     layer = MaxPool2D(kernel_size=2, padding="SAME", strides=1)
     x = jnp.arange(1, 10).reshape(1, 3, 3).astype(jnp.float32)
     npt.assert_allclose(layer(x), jnp.array([[[5, 6, 6], [8, 9, 9], [8, 9, 9]]]))
 
 
 def test_MaxPool3D():
     layer = MaxPool3D(kernel_size=(1, 2, 2), padding="SAME", strides=1)
@@ -199,57 +194,43 @@
 
     npt.assert_allclose(layer(x), y, atol=1e-4)
 
 
 def test_adaptive_pool1d():
     layer_avg = AdaptiveAvgPool1D(2)
     layer_max = AdaptiveMaxPool1D(2)
-    layer_concat = AdaptiveConcatPool1D(2)
-    for input_shape in [2, 3, 4, 5, 6, 7, 8, 9, 10, 13, 14]:
+    for input_shape in [2, 3, 4, 5, 10, 13, 14]:
         x = jnp.ones([1, input_shape])
         assert layer_avg(x).shape == (1, 2)
         assert layer_max(x).shape == (1, 2)
-        assert layer_concat(x).shape == (2, 2)
 
 
 def test_adaptive_pool2d():
     layer_avg = AdaptiveAvgPool2D((2, 3))
     layer_max = AdaptiveMaxPool2D((2, 3))
-    layer_concat = AdaptiveConcatPool2D((2, 3))
-    for input_size in product([2, 3, 4, 5, 6, 7, 8, 9], [3, 4, 5, 6, 7, 8, 9]):
+    for input_size in product([2, 3, 4, 5], [3, 4]):
         x = jnp.ones([1, *input_size])
         assert layer_avg(x).shape == (1, 2, 3)
         assert layer_max(x).shape == (1, 2, 3)
-        assert layer_concat(x).shape == (2, 2, 3)
 
     layer_avg = AdaptiveAvgPool2D((4, 7))
     layer_max = AdaptiveMaxPool2D((4, 7))
-    layer_concat = AdaptiveConcatPool2D((4, 7))
-    for input_size in product([4, 5, 6, 7, 8, 9], [7, 8, 9, 16, 18]):
+    for input_size in product([4, 5], [7, 8, 9, 16, 18]):
         x = jnp.ones([1, *input_size])
         assert layer_avg(x).shape == (1, 4, 7)
         assert layer_max(x).shape == (1, 4, 7)
-        assert layer_concat(x).shape == (2, 4, 7)
 
 
 def test_adaptive_pool3d():
     layer_avg = AdaptiveAvgPool3D((2, 3, 4))
     layer_max = AdaptiveMaxPool3D((2, 3, 4))
-    layer_concat = AdaptiveConcatPool3D((2, 3, 4))
-    for input_size in product(
-        [2, 3, 4, 5, 6, 7, 8, 9], [3, 4, 5, 6, 7, 8, 9], [4, 5, 6, 7, 8, 9]
-    ):
+    for input_size in product([2, 3, 4, 5], [3, 4, 5], [4, 5]):
         x = jnp.ones([1, *input_size])
         assert layer_avg(x).shape == (1, 2, 3, 4)
         assert layer_max(x).shape == (1, 2, 3, 4)
-        assert layer_concat(x).shape == (2, 2, 3, 4)
 
     layer_avg = AdaptiveAvgPool3D((4, 7, 8))
     layer_max = AdaptiveMaxPool3D((4, 7, 8))
-    layer_concat = AdaptiveConcatPool3D((4, 7, 8))
-    for input_size in product(
-        [4, 5, 6, 7, 8, 9], [7, 8, 9, 16, 18], [8, 9, 10, 11, 12]
-    ):
+    for input_size in product([4, 5], [7, 8, 9, 16, 18], [8, 9]):
         x = jnp.ones([1, *input_size])
         assert layer_avg(x).shape == (1, 4, 7, 8)
         assert layer_max(x).shape == (1, 4, 7, 8)
-        assert layer_concat(x).shape == (2, 4, 7, 8)
```

### Comparing `serket-0.0.9/tests/test_preprocessing.py` & `serket-0.2.0b2/tests/test_preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import jax.numpy as jnp
 import numpy.testing as npt
 import pytest
 
-from serket.nn import HistogramEqualization2D, PixelShuffle
+from serket.nn import HistogramEqualization2D, PixelShuffle2D
 
 
 def test_pixel_shuffle():
     x = jnp.array(
         [
             [[0.08482574, 1.9097648], [0.29561743, 1.120948]],
             [[0.33432344, -0.82606775], [0.6481277, 1.0434873]],
             [[-0.7824839, -0.4539462], [0.6297971, 0.81524646]],
             [[-0.32787678, -1.1234448], [-1.6607416, 0.27290547]],
         ]
     )
 
-    ps = PixelShuffle(2)
+    ps = PixelShuffle2D(2)
     y = jnp.array([0.08482574, 0.33432344, 1.9097648, -0.82606775])
 
     npt.assert_allclose(ps(x)[0, 0], y, atol=1e-5)
 
-    with pytest.raises(AssertionError):
-        PixelShuffle(3)(jnp.ones([6, 4, 4]))
+    with pytest.raises(ValueError):
+        PixelShuffle2D(3)(jnp.ones([6, 4, 4]))
 
     with pytest.raises(ValueError):
-        PixelShuffle(-3)(jnp.ones([9, 6, 4]))
+        PixelShuffle2D(-3)(jnp.ones([9, 6, 4]))
 
 
 def test_histogram():
     # tested against skimage.exposure.equalize_hist
 
     x = jnp.array(
         [
```

### Comparing `serket-0.0.9/tests/test_recurrent.py` & `serket-0.2.0b2/tests/test_rnn.py`

 * *Files 16% similar despite different names*

```diff
@@ -50,31 +50,26 @@
 # reverse_cell = reverse_cell.at["hidden_to_hidden.bias"].set(b_hidden_to_hidden_reverse)
 
 
 import jax.numpy as jnp
 import numpy.testing as npt
 import pytest
 
-from serket.nn.recurrent import (
+from serket.nn.recurrent import (  # ConvGRU1DCell,; ConvGRU2DCell,; ConvGRU3DCell,; ConvLSTM2DCell,; ConvLSTM3DCell,
     ConvLSTM1DCell,
-    ConvLSTM2DCell,
-    ConvLSTM3DCell,
+    GRUCell,
     LSTMCell,
     ScanRNN,
-    SeparableConvLSTM1DCell,
-    SeparableConvLSTM2DCell,
-    SeparableConvLSTM3DCell,
     SimpleRNNCell,
 )
 
 # import pytest
 
 
 def test_vanilla_rnn():
-
     in_features = 2
     hidden_features = 3
     # batch_size = 1
     time_steps = 10
 
     # test against keras
     # copy weights from keras to serket and compare outputs
@@ -99,24 +94,22 @@
 
     cell = SimpleRNNCell(
         in_features=in_features,
         hidden_features=hidden_features,
         recurrent_weight_init_func="glorot_uniform",
     )
 
-    cell = cell.at["in_to_hidden.weight"].set(w_in_to_hidden)
-    cell = cell.at["hidden_to_hidden.weight"].set(w_hidden_to_hidden)
-
+    w_combined = jnp.concatenate([w_in_to_hidden, w_hidden_to_hidden], axis=0)
+    cell = cell.at["in_and_hidden_to_hidden"].at["weight"].set(w_combined)
     sk_layer = ScanRNN(cell)
     y = jnp.array([0.9637042, -0.8282256, 0.7314449])
     npt.assert_allclose(sk_layer(x), y)
 
 
 def test_lstm():
-
     # tensorflow
     in_features = 2
     hidden_features = 3
     # batch_size = 1
     time_steps = 10
 
     # inputs = np.ones([batch_size,time_steps, in_features]).astype(np.float32)
@@ -215,17 +208,17 @@
     )
 
     cell = LSTMCell(
         in_features=in_features,
         hidden_features=hidden_features,
         recurrent_weight_init_func="glorot_uniform",
     )
-    cell = cell.at["in_to_hidden.weight"].set(w_in_to_hidden)
-    cell = cell.at["hidden_to_hidden.weight"].set(w_hidden_to_hidden)
-    cell = cell.at["hidden_to_hidden.bias"].set(b_hidden_to_hidden)
+    w_combined = jnp.concatenate([w_in_to_hidden, w_hidden_to_hidden], axis=0)
+    cell = cell.at["in_and_hidden_to_hidden"].at["weight"].set(w_combined)
+    cell = cell.at["in_and_hidden_to_hidden"].at["bias"].set(b_hidden_to_hidden)
 
     sk_layer = ScanRNN(cell, return_sequences=False)
     y = jnp.array([0.18658024, -0.6338659, 0.3445018])
     npt.assert_allclose(y, sk_layer(x), atol=1e-5)
 
     w_in_to_hidden = jnp.array(
         [
@@ -312,17 +305,19 @@
     )
 
     cell = LSTMCell(
         in_features=in_features,
         hidden_features=hidden_features,
         recurrent_weight_init_func="glorot_uniform",
     )
-    cell = cell.at["in_to_hidden.weight"].set(w_in_to_hidden)
-    cell = cell.at["hidden_to_hidden.weight"].set(w_hidden_to_hidden)
-    cell = cell.at["hidden_to_hidden.bias"].set(b_hidden_to_hidden)
+
+    w_combined = jnp.concatenate([w_in_to_hidden, w_hidden_to_hidden], axis=0)
+
+    cell = cell.at["in_and_hidden_to_hidden"].at["weight"].set(w_combined)
+    cell = cell.at["in_and_hidden_to_hidden"].at["bias"].set(b_hidden_to_hidden)
 
     sk_layer = ScanRNN(cell, return_sequences=True)
 
     y = jnp.array(
         [
             [-0.07431775, 0.05081949, 0.07480226],
             [-0.12263095, 0.07622699, 0.1146026],
@@ -336,23 +331,86 @@
             [-0.20601842, 0.09728104, 0.16009602],
         ]
     )
 
     npt.assert_allclose(y, sk_layer(x), atol=1e-5)
 
     cell = LSTMCell(
-        in_features=None,
+        in_features=in_features,
         hidden_features=hidden_features,
         recurrent_weight_init_func="glorot_uniform",
     )
 
     sk_layer = ScanRNN(cell, return_sequences=True)
     assert sk_layer(x).shape == (10, 3)
 
 
+def test_gru():
+    w1 = jnp.array(
+        [
+            [
+                -0.04667467,
+                0.25340378,
+                0.26873875,
+                0.15961742,
+                0.56519365,
+                0.46263158,
+                -0.0030899,
+                0.31380886,
+                0.44481528,
+            ]
+        ]
+    )
+
+    w2 = jnp.array(
+        [
+            [
+                0.23404205,
+                0.10193896,
+                0.27892762,
+                -0.488236,
+                -0.4173184,
+                -0.0588184,
+                0.41350085,
+                0.36151117,
+                -0.45407838,
+            ],
+            [
+                -0.560196,
+                -0.22648495,
+                -0.12656957,
+                0.31881046,
+                0.47110367,
+                0.30805635,
+                0.41259462,
+                0.40002275,
+                -0.0368616,
+            ],
+            [
+                0.5745573,
+                0.4343021,
+                0.42046744,
+                -0.09401041,
+                0.5539224,
+                -0.13675115,
+                -0.5197817,
+                -0.21241805,
+                -0.16732433,
+            ],
+        ]
+    )
+
+    cell = GRUCell(1, 3, bias_init_func=None)
+    cell = cell.at["in_to_hidden"].at["weight"].set(w1)
+    cell = cell.at["hidden_to_hidden"].at["weight"].set(w2)
+    y = jnp.array([[-0.00142191, 0.11011646, 0.1613554]])
+    ypred = ScanRNN(cell, return_sequences=True)(jnp.ones([1, 1]))
+    npt.assert_allclose(y, ypred, atol=1e-4)
+
+
 def test_conv_lstm1d():
     w_in_to_hidden = jnp.array(
         [
             [
                 [0.3159187, -0.37110862, 0.23497376],
                 [0.06916022, 0.16520068, -0.1498835],
             ],
@@ -482,38 +540,38 @@
             [0.0],
             [0.0],
             [0.0],
         ]
     )
 
     in_features = 2
-    out_features = 3
+    hidden_features = 3
     time_steps = 1
     spatial_dim = (3,)
 
     # inputs = np.ones([batch_size,time_steps, in_features,*spatial_dim]).astype(np.float32)
     # inp = tf.keras.Input(shape=(time_steps, in_features,*spatial_dim))
-    # rnn = (tf.keras.layers.ConvLSTM1D(out_features,recurrent_activation="sigmoid", kernel_size=3, padding='same',
+    # rnn = (tf.keras.layers.ConvLSTM1D(hidden_features,recurrent_activation="sigmoid", kernel_size=3, padding='same',
     # return_sequences=False,data_format='channels_first'))(inp)
     # rnn = tf.keras.Model(inputs=inp, outputs=rnn)
 
     cell = ConvLSTM1DCell(
         in_features=in_features,
-        out_features=out_features,
+        hidden_features=hidden_features,
         recurrent_act_func="sigmoid",
         kernel_size=3,
         padding="same",
         weight_init_func="glorot_uniform",
         recurrent_weight_init_func="glorot_uniform",
         bias_init_func="zeros",
     )
 
-    cell = cell.at["in_to_hidden.weight"].set(w_in_to_hidden)
-    cell = cell.at["hidden_to_hidden.weight"].set(w_hidden_to_hidden)
-    cell = cell.at["hidden_to_hidden.bias"].set(b_hidden_to_hidden)
+    cell = cell.at["in_to_hidden"].at["weight"].set(w_in_to_hidden)
+    cell = cell.at["hidden_to_hidden"].at["weight"].set(w_hidden_to_hidden)
+    cell = cell.at["hidden_to_hidden"].at["bias"].set(b_hidden_to_hidden)
 
     x = jnp.ones([time_steps, in_features, *spatial_dim])
 
     res_sk = ScanRNN(cell, return_sequences=False)(x)
 
     y = jnp.array(
         [
@@ -522,16 +580,16 @@
             [0.01413723, 0.00672858, -0.03464129],
         ]
     )
 
     assert jnp.allclose(res_sk, y, atol=1e-5)
 
     cell = ConvLSTM1DCell(
-        in_features=None,
-        out_features=out_features,
+        in_features=in_features,
+        hidden_features=hidden_features,
         recurrent_act_func="sigmoid",
         kernel_size=3,
         padding="same",
         weight_init_func="glorot_uniform",
         recurrent_weight_init_func="glorot_uniform",
         bias_init_func="zeros",
     )
@@ -670,103 +728,43 @@
                 3.26157391e-01,
             ],
         ]
     )
 
     b_hidden_to_hidden_reverse = jnp.array([0.0, 0.0, 1.0, 1.0, 0.0, 0.0, 0.0, 0.0])
 
-    cell = cell.at["in_to_hidden.weight"].set(w_in_to_hidden)
-    cell = cell.at["hidden_to_hidden.weight"].set(w_hidden_to_hidden)
-    cell = cell.at["hidden_to_hidden.bias"].set(b_hidden_to_hidden)
-
-    reverse_cell = reverse_cell.at["in_to_hidden.weight"].set(w_in_to_hidden_reverse)
-    reverse_cell = reverse_cell.at["hidden_to_hidden.weight"].set(
-        w_hidden_to_hidden_reverse
-    )
-    reverse_cell = reverse_cell.at["hidden_to_hidden.bias"].set(
-        b_hidden_to_hidden_reverse
+    combined_w = jnp.concatenate([w_in_to_hidden, w_hidden_to_hidden], axis=0)
+    cell = cell.at["in_and_hidden_to_hidden"].at["weight"].set(combined_w)
+    cell = cell.at["in_and_hidden_to_hidden"].at["bias"].set(b_hidden_to_hidden)
+
+    combined_w_reverse = jnp.concatenate(
+        [w_in_to_hidden_reverse, w_hidden_to_hidden_reverse], axis=0
+    )
+    reverse_cell = (
+        reverse_cell.at["in_and_hidden_to_hidden"].at["weight"].set(combined_w_reverse)
+    )
+    reverse_cell = (
+        reverse_cell.at["in_and_hidden_to_hidden"]
+        .at["bias"]
+        .set(b_hidden_to_hidden_reverse)
     )
 
     res = ScanRNN(cell, backward_cell=reverse_cell, return_sequences=False)(x)
 
     y = jnp.array([0.35901642, 0.00826644, -0.3015435, -0.13661332])
 
     npt.assert_allclose(res, y, atol=1e-5)
 
 
-def test_lazy_rnn():
-
-    x = jnp.ones([10, 1])  # time_steps, in_features
-    left = SimpleRNNCell(None, 15)  # in_features, hidden_features
-    assert ScanRNN(left)(x).shape == (15,)
-    assert ScanRNN(left, return_sequences=True)(x).shape == (10, 15)
-
-    right = SimpleRNNCell(None, 15)  # in_features, hidden_features
-    assert ScanRNN(left, right)(x).shape == (30,)
-    assert ScanRNN(left, right, return_sequences=True)(x).shape == (10, 30)
-
-    x = jnp.ones([10, 3, 5])  # time_steps, in_features, spatial_features
-    left = ConvLSTM1DCell(None, 10, 3)  # in_features, hidden_features
-    assert ScanRNN(left)(x).shape == (10, 5)  # hidden_features, spatial_features
-    right = ConvLSTM1DCell(None, 10, 3)  # in_features, hidden_features
-    assert ScanRNN(left, right)(x).shape == (20, 5)
-    assert ScanRNN(left, right, return_sequences=True)(x).shape == (10, 20, 5)
-
-
 def test_rnn_error():
-    with pytest.raises(ValueError):
+    with pytest.raises(TypeError):
         ScanRNN(None)
 
-    with pytest.raises(ValueError):
+    with pytest.raises(TypeError):
         ScanRNN(SimpleRNNCell(3, 3), 1)
 
     layer = ScanRNN(SimpleRNNCell(3, 3), SimpleRNNCell(3, 3))
-    with pytest.raises(ValueError):
+    with pytest.raises(TypeError):
         layer(jnp.ones([10, 3]), 1.0)
 
-    with pytest.raises(AssertionError):
+    with pytest.raises(ValueError):
         layer(jnp.ones([10, 3, 3]))
-
-
-def test_conv_lstm2d():
-    x = jnp.ones([10, 3, 5, 5])  # time_steps, in_features, spatial_features
-    left = ConvLSTM2DCell(None, 10, 3)  # in_features, hidden_features
-    assert ScanRNN(left)(x).shape == (10, 5, 5)  # hidden_features, spatial_features
-    right = ConvLSTM2DCell(None, 10, 3)  # in_features, hidden_features
-    assert ScanRNN(left, right)(x).shape == (20, 5, 5)
-    assert ScanRNN(left, right, return_sequences=True)(x).shape == (10, 20, 5, 5)
-
-
-def test_conv_lstm3d():
-    x = jnp.ones([10, 3, 5, 5, 5])  # time_steps, in_features, spatial_features
-    left = ConvLSTM3DCell(None, 10, 3)  # in_features, hidden_features
-    assert ScanRNN(left)(x).shape == (10, 5, 5, 5)  # hidden_features, spatial_features
-    right = ConvLSTM3DCell(None, 10, 3)  # in_features, hidden_features
-    assert ScanRNN(left, right)(x).shape == (20, 5, 5, 5)
-    assert ScanRNN(left, right, return_sequences=True)(x).shape == (10, 20, 5, 5, 5)
-
-
-def test_separable_conv_lstm1d():
-    x = jnp.ones([10, 3, 5])  # time_steps, in_features, spatial_features
-    left = SeparableConvLSTM1DCell(None, 10, 3)  # in_features, hidden_features
-    assert ScanRNN(left)(x).shape == (10, 5)  # hidden_features, spatial_features
-    right = SeparableConvLSTM1DCell(None, 10, 3)  # in_features, hidden_features
-    assert ScanRNN(left, right)(x).shape == (20, 5)
-    assert ScanRNN(left, right, return_sequences=True)(x).shape == (10, 20, 5)
-
-
-def test_separable_conv_lstm2d():
-    x = jnp.ones([10, 3, 5, 5])  # time_steps, in_features, spatial_features
-    left = SeparableConvLSTM2DCell(None, 10, 3)  # in_features, hidden_features
-    assert ScanRNN(left)(x).shape == (10, 5, 5)  # hidden_features, spatial_features
-    right = SeparableConvLSTM2DCell(None, 10, 3)  # in_features, hidden_features
-    assert ScanRNN(left, right)(x).shape == (20, 5, 5)
-    assert ScanRNN(left, right, return_sequences=True)(x).shape == (10, 20, 5, 5)
-
-
-def test_separable_conv_lstm3d():
-    x = jnp.ones([10, 3, 5, 5, 5])  # time_steps, in_features, spatial_features
-    left = SeparableConvLSTM3DCell(None, 10, 3)  # in_features, hidden_features
-    assert ScanRNN(left)(x).shape == (10, 5, 5, 5)  # hidden_features, spatial_features
-    right = SeparableConvLSTM3DCell(None, 10, 3)  # in_features, hidden_features
-    assert ScanRNN(left, right)(x).shape == (20, 5, 5, 5)
-    assert ScanRNN(left, right, return_sequences=True)(x).shape == (10, 20, 5, 5, 5)
```

### Comparing `serket-0.0.9/tests/test_sequential.py` & `serket-0.2.0b2/tests/test_sequential.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 from serket.nn import Lambda, Sequential
 
 
 def test_sequential():
-
-    model = Sequential([Lambda(lambda x: x)])
+    model = Sequential((Lambda(lambda x: x),))
     assert model(1.0) == 1.0
 
-    model = Sequential([Lambda(lambda x: x + 1), Lambda(lambda x: x + 1)])
+    model = Sequential((Lambda(lambda x: x + 1), Lambda(lambda x: x + 1)))
     assert model(1.0) == 3.0
 
-    model = Sequential([lambda x, key: x])
+    model = Sequential((lambda x, key: x,))
     assert model(1.0) == 1.0
 
 
 def test_sequential_getitem():
-    model = Sequential([Lambda(lambda x: x + 1), Lambda(lambda x: x + 1)])
+    model = Sequential((Lambda(lambda x: x + 1), Lambda(lambda x: x + 1)))
     assert model[0](1.0) == 2.0
     assert model[1](1.0) == 2.0
     assert model[0:1](1.0) == 2.0
     assert model[1:2](1.0) == 2.0
     assert model[0:2](1.0) == 3.0
 
 
 def test_sequential_len():
-    model = Sequential([Lambda(lambda x: x + 1), Lambda(lambda x: x + 1)])
+    model = Sequential((Lambda(lambda x: x + 1), Lambda(lambda x: x + 1)))
     assert len(model) == 2
 
 
 def test_sequential_iter():
-    model = Sequential([Lambda(lambda x: x + 1), Lambda(lambda x: x + 1)])
+    model = Sequential((Lambda(lambda x: x + 1), Lambda(lambda x: x + 1)))
     assert list(model) == [model[0], model[1]]
 
 
 def test_sequential_reversed():
-    model = Sequential([Lambda(lambda x: x + 1), Lambda(lambda x: x + 1)])
+    model = Sequential((Lambda(lambda x: x + 1), Lambda(lambda x: x + 1)))
     assert list(reversed(model)) == [model[1], model[0]]
```

