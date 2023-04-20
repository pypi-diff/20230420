# Comparing `tmp/cy-root-1.0.1.tar.gz` & `tmp/cy-root-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cy-root-1.0.1.tar", last modified: Sun Apr 16 05:30:25 2023, max compression
+gzip compressed data, was "cy-root-1.0.2.tar", last modified: Thu Apr 20 19:56:43 2023, max compression
```

## Comparing `cy-root-1.0.1.tar` & `cy-root-1.0.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:30:25.012637 cy-root-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-16 05:29:44.000000 cy-root-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-16 05:29:44.000000 cy-root-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-04-16 05:30:25.012637 cy-root-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15077 2023-04-16 05:29:44.000000 cy-root-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:30:24.988637 cy-root-1.0.1/cy_root.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-04-16 05:30:24.000000 cy-root-1.0.1/cy_root.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-16 05:30:24.000000 cy-root-1.0.1/cy_root.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 05:30:24.000000 cy-root-1.0.1/cy_root.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 05:30:24.000000 cy-root-1.0.1/cy_root.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-16 05:30:24.000000 cy-root-1.0.1/cy_root.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-16 05:30:24.000000 cy-root-1.0.1/cy_root.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:30:25.008637 cy-root-1.0.1/cyroot/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1144817 2023-04-16 05:30:16.000000 cy-root-1.0.1/cyroot/_check_args.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/_check_args.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    12474 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/_check_args.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/_return_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)  1449732 2023-04-16 05:30:10.000000 cy-root-1.0.1/cyroot/fptr.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/fptr.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/fptr.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:30:25.012637 cy-root-1.0.1/cyroot/ops/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/ops/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   301922 2023-04-16 05:30:16.000000 cy-root-1.0.1/cyroot/ops/matrix_ops.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/ops/matrix_ops.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/ops/matrix_ops.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   126171 2023-04-16 05:30:10.000000 cy-root-1.0.1/cyroot/ops/scalar_ops.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/ops/scalar_ops.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/ops/scalar_ops.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   995644 2023-04-16 05:30:11.000000 cy-root-1.0.1/cyroot/ops/vector_ops.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/ops/vector_ops.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/ops/vector_ops.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  2034789 2023-04-16 05:30:12.000000 cy-root-1.0.1/cyroot/scalar_bracketing.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    68287 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/scalar_bracketing.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  1228034 2023-04-16 05:30:17.000000 cy-root-1.0.1/cyroot/scalar_derivative_approximation.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/scalar_derivative_approximation.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/scalar_derivative_approximation.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  2821531 2023-04-16 05:30:14.000000 cy-root-1.0.1/cyroot/scalar_newton.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    44827 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/scalar_newton.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  1522297 2023-04-16 05:30:19.000000 cy-root-1.0.1/cyroot/scalar_quasi_newton.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    30004 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/scalar_quasi_newton.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/scalar_root.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:30:25.012637 cy-root-1.0.1/cyroot/typing/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/typing/_array_like.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:30:25.012637 cy-root-1.0.1/cyroot/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/utils/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/utils/_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/utils/function_tagging.py
--rw-r--r--   0 runner    (1001) docker     (123)   888661 2023-04-16 05:30:19.000000 cy-root-1.0.1/cyroot/utils/itertools.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/utils/itertools.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/utils/itertools.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/utils/namedtuple.py
--rw-r--r--   0 runner    (1001) docker     (123)  1499637 2023-04-16 05:30:21.000000 cy-root-1.0.1/cyroot/vector_bracketing.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15178 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/vector_bracketing.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  1389285 2023-04-16 05:30:15.000000 cy-root-1.0.1/cyroot/vector_derivative_approximation.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/vector_derivative_approximation.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    11326 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/vector_derivative_approximation.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  1554514 2023-04-16 05:30:22.000000 cy-root-1.0.1/cyroot/vector_newton.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    28441 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/vector_newton.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  1902923 2023-04-16 05:30:23.000000 cy-root-1.0.1/cyroot/vector_quasi_newton.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    37153 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/vector_quasi_newton.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-16 05:29:44.000000 cy-root-1.0.1/cyroot/vector_root.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-16 05:29:44.000000 cy-root-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-16 05:29:44.000000 cy-root-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-16 05:30:25.012637 cy-root-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-16 05:29:44.000000 cy-root-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:56:43.003521 cy-root-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-20 19:55:52.000000 cy-root-1.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-20 19:55:52.000000 cy-root-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-04-20 19:56:43.003521 cy-root-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15077 2023-04-20 19:55:52.000000 cy-root-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:56:42.971521 cy-root-1.0.2/cy_root.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-04-20 19:56:42.000000 cy-root-1.0.2/cy_root.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-20 19:56:42.000000 cy-root-1.0.2/cy_root.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:56:42.000000 cy-root-1.0.2/cy_root.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:56:42.000000 cy-root-1.0.2/cy_root.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-20 19:56:42.000000 cy-root-1.0.2/cy_root.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 19:56:42.000000 cy-root-1.0.2/cy_root.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:56:42.995521 cy-root-1.0.2/cyroot/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1145539 2023-04-20 19:56:29.000000 cy-root-1.0.2/cyroot/_check_args.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/_check_args.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    12542 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/_check_args.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/_return_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1449732 2023-04-20 19:56:31.000000 cy-root-1.0.2/cyroot/fptr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/fptr.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/fptr.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:56:42.999521 cy-root-1.0.2/cyroot/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/ops/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   301922 2023-04-20 19:56:31.000000 cy-root-1.0.2/cyroot/ops/matrix_ops.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/ops/matrix_ops.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/ops/matrix_ops.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   139381 2023-04-20 19:56:21.000000 cy-root-1.0.2/cyroot/ops/scalar_ops.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/ops/scalar_ops.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/ops/scalar_ops.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   995715 2023-04-20 19:56:22.000000 cy-root-1.0.2/cyroot/ops/vector_ops.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/ops/vector_ops.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/ops/vector_ops.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  2036364 2023-04-20 19:56:24.000000 cy-root-1.0.2/cyroot/scalar_bracketing.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    68297 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/scalar_bracketing.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1228105 2023-04-20 19:56:33.000000 cy-root-1.0.2/cyroot/scalar_derivative_approximation.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/scalar_derivative_approximation.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/scalar_derivative_approximation.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  2821602 2023-04-20 19:56:26.000000 cy-root-1.0.2/cyroot/scalar_newton.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    44827 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/scalar_newton.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1522539 2023-04-20 19:56:34.000000 cy-root-1.0.2/cyroot/scalar_quasi_newton.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30025 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/scalar_quasi_newton.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/scalar_root.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:56:42.999521 cy-root-1.0.2/cyroot/typing/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/typing/_array_like.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:56:43.003521 cy-root-1.0.2/cyroot/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/utils/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/utils/_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/utils/function_tagging.py
+-rw-r--r--   0 runner    (1001) docker     (123)   888732 2023-04-20 19:56:36.000000 cy-root-1.0.2/cyroot/utils/itertools.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/utils/itertools.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/utils/itertools.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/utils/namedtuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1499708 2023-04-20 19:56:37.000000 cy-root-1.0.2/cyroot/vector_bracketing.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15178 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/vector_bracketing.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1389356 2023-04-20 19:56:28.000000 cy-root-1.0.2/cyroot/vector_derivative_approximation.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/vector_derivative_approximation.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    11326 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/vector_derivative_approximation.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1554585 2023-04-20 19:56:39.000000 cy-root-1.0.2/cyroot/vector_newton.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28441 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/vector_newton.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1904574 2023-04-20 19:56:41.000000 cy-root-1.0.2/cyroot/vector_quasi_newton.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    37172 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/vector_quasi_newton.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-20 19:55:52.000000 cy-root-1.0.2/cyroot/vector_root.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-20 19:55:52.000000 cy-root-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-20 19:55:52.000000 cy-root-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-20 19:56:43.003521 cy-root-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-20 19:55:52.000000 cy-root-1.0.2/setup.py
```

### Comparing `cy-root-1.0.1/LICENSE.txt` & `cy-root-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cy-root-1.0.1/PKG-INFO` & `cy-root-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cy-root
-Version: 1.0.1
+Version: 1.0.2
 Summary: Cython implementations of multiple root-finding methods.
 Home-page: https://github.com/inspiros/cy-root
 Author: Hoang-Nhat Tran (inspiros)
 Author-email: hnhat.tran@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/inspiros/cy-root
 Keywords: root-finding
```

### Comparing `cy-root-1.0.1/README.md` & `cy-root-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cy-root-1.0.1/cy_root.egg-info/PKG-INFO` & `cy-root-1.0.2/cy_root.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cy-root
-Version: 1.0.1
+Version: 1.0.2
 Summary: Cython implementations of multiple root-finding methods.
 Home-page: https://github.com/inspiros/cy-root
 Author: Hoang-Nhat Tran (inspiros)
 Author-email: hnhat.tran@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/inspiros/cy-root
 Keywords: root-finding
```

### Comparing `cy-root-1.0.1/cy_root.egg-info/SOURCES.txt` & `cy-root-1.0.2/cy_root.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cy-root-1.0.1/cyroot/_check_args.cpp` & `cy-root-1.0.2/cyroot/_check_args.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
             "cyroot",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include",
             "cyroot/ops",
             "cyroot/utils"
         ],
         "language": "c++",
         "name": "cyroot._check_args",
         "sources": [
             "cyroot/_check_args.pyx"
@@ -1166,195 +1166,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1389,42 +1389,42 @@
 struct __pyx_obj_6cyroot_11_check_args___pyx_scope_struct_2__check_initial_vals_uniqueness;
 struct __pyx_obj_6cyroot_11_check_args___pyx_scope_struct_3_genexpr;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1432,28 +1432,28 @@
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_cisclose;
 
 /* "scalar_ops.pxd":18
  *     double complex
  * 
  * cdef bint isclose(double a, double b, double rtol=*, double atol=*) nogil             # <<<<<<<<<<<<<<
  * cdef bint cisclose(double complex a, double complex b, double rtol=*, double atol=*) nogil
- * 
+ * cdef real min(real a, real b) nogil
  */
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_isclose {
   int __pyx_n;
   double rtol;
   double atol;
 };
 
 /* "scalar_ops.pxd":19
  * 
  * cdef bint isclose(double a, double b, double rtol=*, double atol=*) nogil
  * cdef bint cisclose(double complex a, double complex b, double rtol=*, double atol=*) nogil             # <<<<<<<<<<<<<<
- * 
- * cdef extern from '<math.h>' nogil:
+ * cdef real min(real a, real b) nogil
+ * cdef real max(real a, real b) nogil
  */
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_cisclose {
   int __pyx_n;
   double rtol;
   double atol;
 };
 struct __pyx_opt_args_6cyroot_3ops_10vector_ops_allclose;
@@ -1595,56 +1595,56 @@
   double f0;
   double f1;
 };
 
 /* "cyroot/_check_args.pyx":55
  * 
  * # noinspection DuplicatedCode
- * def _check_initial_guesses_uniqueness(xs: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):             # <<<<<<<<<<<<<<
- *     if not len(xs):
+ * def _check_initial_guesses_uniqueness(x0s: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):             # <<<<<<<<<<<<<<
+ *     if not len(x0s):
  *         raise ValueError('Empty.')
  */
 struct __pyx_obj_6cyroot_11_check_args___pyx_scope_struct___check_initial_guesses_uniqueness {
   PyObject_HEAD
-  PyObject *__pyx_v_xs;
+  PyObject *__pyx_v_x0s;
 };
 
 
 /* "cyroot/_check_args.pyx":62
- *                      np.stack(xs), axis=0).shape[0] < len(xs):
+ *                      np.stack(x0s), axis=0).shape[0] < len(x0s):
  *             raise ValueError(f'Initial guesses must be unique. Got:\n' +
- *                              '\n'.join(repr(_) for _ in xs))             # <<<<<<<<<<<<<<
- *     elif len(set(xs)) < len(xs):
- *         raise ValueError(f'Initial guesses must be unique. Got {xs}.')
+ *                              '\n'.join(repr(_) for _ in x0s))             # <<<<<<<<<<<<<<
+ *     elif len(set(x0s)) < len(x0s):
+ *         raise ValueError(f'Initial guesses must be unique. Got {x0s}.')
  */
 struct __pyx_obj_6cyroot_11_check_args___pyx_scope_struct_1_genexpr {
   PyObject_HEAD
   struct __pyx_obj_6cyroot_11_check_args___pyx_scope_struct___check_initial_guesses_uniqueness *__pyx_outer_scope;
   PyObject *__pyx_v__;
 };
 
 
 /* "cyroot/_check_args.pyx":67
  * 
  * # noinspection DuplicatedCode
- * def _check_initial_vals_uniqueness(f_xs: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):             # <<<<<<<<<<<<<<
- *     if not len(f_xs):
+ * def _check_initial_vals_uniqueness(f_x0s: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):             # <<<<<<<<<<<<<<
+ *     if not len(f_x0s):
  *         raise ValueError('Empty.')
  */
 struct __pyx_obj_6cyroot_11_check_args___pyx_scope_struct_2__check_initial_vals_uniqueness {
   PyObject_HEAD
-  PyObject *__pyx_v_f_xs;
+  PyObject *__pyx_v_f_x0s;
 };
 
 
 /* "cyroot/_check_args.pyx":74
- *                      np.stack(f_xs), axis=0).shape[0] < len(f_xs):
+ *                      np.stack(f_x0s), axis=0).shape[0] < len(f_x0s):
  *             raise ValueError('Initial guesses\' values must be unique. '
- *                              'Got:\n' + '\n'.join(repr(_) for _ in f_xs))             # <<<<<<<<<<<<<<
- *     elif len(set(f_xs)) < len(f_xs):
+ *                              'Got:\n' + '\n'.join(repr(_) for _ in f_x0s))             # <<<<<<<<<<<<<<
+ *     elif len(set(f_x0s)) < len(f_x0s):
  *         raise ValueError('Initial guesses\' values must be unique. '
  */
 struct __pyx_obj_6cyroot_11_check_args___pyx_scope_struct_3_genexpr {
   PyObject_HEAD
   struct __pyx_obj_6cyroot_11_check_args___pyx_scope_struct_2__check_initial_vals_uniqueness *__pyx_outer_scope;
   PyObject *__pyx_v__;
 };
@@ -2785,28 +2785,27 @@
 static PyObject *__pyx_builtin_IndexError;
 static const char __pyx_k_[] = ".";
 static const char __pyx_k_O[] = "O";
 static const char __pyx_k_c[] = "c";
 static const char __pyx_k__4[] = "\n";
 static const char __pyx_k_id[] = "id";
 static const char __pyx_k_np[] = "np";
-static const char __pyx_k_xs[] = "xs";
 static const char __pyx_k_abs[] = "abs";
 static const char __pyx_k_all[] = "__all__";
 static const char __pyx_k_max[] = "max";
 static const char __pyx_k_min[] = "min";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_obj[] = "obj";
 static const char __pyx_k_tol[] = "tol";
+static const char __pyx_k_x0s[] = "x0s";
 static const char __pyx_k_args[] = "args";
 static const char __pyx_k_axis[] = "axis";
 static const char __pyx_k_base[] = "base";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_etol[] = "etol";
-static const char __pyx_k_f_xs[] = "f_xs";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_math[] = "math";
 static const char __pyx_k_mode[] = "mode";
 static const char __pyx_k_name[] = "name";
 static const char __pyx_k_ndim[] = "ndim";
 static const char __pyx_k_pack[] = "pack";
 static const char __pyx_k_ptol[] = "ptol";
@@ -2818,14 +2817,15 @@
 static const char __pyx_k_ASCII[] = "ASCII";
 static const char __pyx_k_Empty[] = "Empty.";
 static const char __pyx_k_Union[] = "Union";
 static const char __pyx_k_class[] = "__class__";
 static const char __pyx_k_close[] = "close";
 static const char __pyx_k_error[] = "error";
 static const char __pyx_k_ertol[] = "ertol";
+static const char __pyx_k_f_x0s[] = "f_x0s";
 static const char __pyx_k_flags[] = "flags";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_prtol[] = "prtol";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_shape[] = "shape";
 static const char __pyx_k_stack[] = "stack";
 static const char __pyx_k_start[] = "start";
@@ -2981,15 +2981,15 @@
 static PyObject *__pyx_n_s_encode;
 static PyObject *__pyx_n_s_enumerate;
 static PyObject *__pyx_n_s_error;
 static PyObject *__pyx_n_s_ertol;
 static PyObject *__pyx_n_u_ertol;
 static PyObject *__pyx_n_s_etol;
 static PyObject *__pyx_n_u_etol;
-static PyObject *__pyx_n_s_f_xs;
+static PyObject *__pyx_n_s_f_x0s;
 static PyObject *__pyx_n_s_flags;
 static PyObject *__pyx_n_s_format;
 static PyObject *__pyx_n_s_fortran;
 static PyObject *__pyx_n_u_fortran;
 static PyObject *__pyx_n_s_genexpr;
 static PyObject *__pyx_n_s_getstate;
 static PyObject *__pyx_kp_s_got_differing_extents_in_dimensi;
@@ -3054,21 +3054,21 @@
 static PyObject *__pyx_n_u_tol;
 static PyObject *__pyx_n_s_typing;
 static PyObject *__pyx_kp_s_unable_to_allocate_array_data;
 static PyObject *__pyx_kp_s_unable_to_allocate_shape_and_str;
 static PyObject *__pyx_n_s_unique;
 static PyObject *__pyx_n_s_unpack;
 static PyObject *__pyx_n_s_update;
-static PyObject *__pyx_n_s_xs;
+static PyObject *__pyx_n_s_x0s;
 static PyObject *__pyx_pf_6cyroot_11_check_args__check_stop_cond_arg(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_tol, PyObject *__pyx_v_arg_name); /* proto */
 static PyObject *__pyx_pf_6cyroot_11_check_args_2_check_stop_cond_args(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_etol, double __pyx_v_ertol, double __pyx_v_ptol, double __pyx_v_prtol, PyObject *__pyx_v_max_iter); /* proto */
 static PyObject *__pyx_pf_6cyroot_11_check_args_33_check_initial_guesses_uniqueness_genexpr(PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_6cyroot_11_check_args_4_check_initial_guesses_uniqueness(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_xs); /* proto */
+static PyObject *__pyx_pf_6cyroot_11_check_args_4_check_initial_guesses_uniqueness(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_x0s); /* proto */
 static PyObject *__pyx_pf_6cyroot_11_check_args_30_check_initial_vals_uniqueness_genexpr(PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_6cyroot_11_check_args_6_check_initial_vals_uniqueness(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_f_xs); /* proto */
+static PyObject *__pyx_pf_6cyroot_11_check_args_6_check_initial_vals_uniqueness(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_f_x0s); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_8__getattr__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_attr); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_10__getitem__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_item); /* proto */
@@ -4014,40 +4014,40 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cyroot/_check_args.pyx":55
  * 
  * # noinspection DuplicatedCode
- * def _check_initial_guesses_uniqueness(xs: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):             # <<<<<<<<<<<<<<
- *     if not len(xs):
+ * def _check_initial_guesses_uniqueness(x0s: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):             # <<<<<<<<<<<<<<
+ *     if not len(x0s):
  *         raise ValueError('Empty.')
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6cyroot_11_check_args_5_check_initial_guesses_uniqueness(PyObject *__pyx_self, PyObject *__pyx_v_xs); /*proto*/
+static PyObject *__pyx_pw_6cyroot_11_check_args_5_check_initial_guesses_uniqueness(PyObject *__pyx_self, PyObject *__pyx_v_x0s); /*proto*/
 static PyMethodDef __pyx_mdef_6cyroot_11_check_args_5_check_initial_guesses_uniqueness = {"_check_initial_guesses_uniqueness", (PyCFunction)__pyx_pw_6cyroot_11_check_args_5_check_initial_guesses_uniqueness, METH_O, 0};
-static PyObject *__pyx_pw_6cyroot_11_check_args_5_check_initial_guesses_uniqueness(PyObject *__pyx_self, PyObject *__pyx_v_xs) {
+static PyObject *__pyx_pw_6cyroot_11_check_args_5_check_initial_guesses_uniqueness(PyObject *__pyx_self, PyObject *__pyx_v_x0s) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_check_initial_guesses_uniqueness (wrapper)", 0);
-  __pyx_r = __pyx_pf_6cyroot_11_check_args_4_check_initial_guesses_uniqueness(__pyx_self, ((PyObject *)__pyx_v_xs));
+  __pyx_r = __pyx_pf_6cyroot_11_check_args_4_check_initial_guesses_uniqueness(__pyx_self, ((PyObject *)__pyx_v_x0s));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_6cyroot_11_check_args_33_check_initial_guesses_uniqueness_2generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
 /* "cyroot/_check_args.pyx":62
- *                      np.stack(xs), axis=0).shape[0] < len(xs):
+ *                      np.stack(x0s), axis=0).shape[0] < len(x0s):
  *             raise ValueError(f'Initial guesses must be unique. Got:\n' +
- *                              '\n'.join(repr(_) for _ in xs))             # <<<<<<<<<<<<<<
- *     elif len(set(xs)) < len(xs):
- *         raise ValueError(f'Initial guesses must be unique. Got {xs}.')
+ *                              '\n'.join(repr(_) for _ in x0s))             # <<<<<<<<<<<<<<
+ *     elif len(set(x0s)) < len(x0s):
+ *         raise ValueError(f'Initial guesses must be unique. Got {x0s}.')
  */
 
 static PyObject *__pyx_pf_6cyroot_11_check_args_33_check_initial_guesses_uniqueness_genexpr(PyObject *__pyx_self) {
   struct __pyx_obj_6cyroot_11_check_args___pyx_scope_struct_1_genexpr *__pyx_cur_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
@@ -4101,20 +4101,20 @@
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
   if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 62, __pyx_L1_error)
   __pyx_r = PyList_New(0); if (unlikely(!__pyx_r)) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_r);
-  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_xs)) { __Pyx_RaiseClosureNameError("xs"); __PYX_ERR(0, 62, __pyx_L1_error) }
-  if (likely(PyList_CheckExact(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_xs)) || PyTuple_CheckExact(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_xs)) {
-    __pyx_t_1 = __pyx_cur_scope->__pyx_outer_scope->__pyx_v_xs; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
+  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_x0s)) { __Pyx_RaiseClosureNameError("x0s"); __PYX_ERR(0, 62, __pyx_L1_error) }
+  if (likely(PyList_CheckExact(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_x0s)) || PyTuple_CheckExact(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_x0s)) {
+    __pyx_t_1 = __pyx_cur_scope->__pyx_outer_scope->__pyx_v_x0s; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
     __pyx_t_3 = NULL;
   } else {
-    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_xs); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_x0s); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 62, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_3)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
@@ -4174,20 +4174,20 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cyroot/_check_args.pyx":55
  * 
  * # noinspection DuplicatedCode
- * def _check_initial_guesses_uniqueness(xs: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):             # <<<<<<<<<<<<<<
- *     if not len(xs):
+ * def _check_initial_guesses_uniqueness(x0s: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):             # <<<<<<<<<<<<<<
+ *     if not len(x0s):
  *         raise ValueError('Empty.')
  */
 
-static PyObject *__pyx_pf_6cyroot_11_check_args_4_check_initial_guesses_uniqueness(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_xs) {
+static PyObject *__pyx_pf_6cyroot_11_check_args_4_check_initial_guesses_uniqueness(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_x0s) {
   struct __pyx_obj_6cyroot_11_check_args___pyx_scope_struct___check_initial_guesses_uniqueness *__pyx_cur_scope;
   PyObject *__pyx_gb_6cyroot_11_check_args_33_check_initial_guesses_uniqueness_2generator = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t __pyx_t_2;
   int __pyx_t_3;
@@ -4206,95 +4206,95 @@
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_6cyroot_11_check_args___pyx_scope_struct___check_initial_guesses_uniqueness *)Py_None);
     __Pyx_INCREF(Py_None);
     __PYX_ERR(0, 55, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
-  __pyx_cur_scope->__pyx_v_xs = __pyx_v_xs;
-  __Pyx_INCREF(__pyx_cur_scope->__pyx_v_xs);
-  __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_xs);
+  __pyx_cur_scope->__pyx_v_x0s = __pyx_v_x0s;
+  __Pyx_INCREF(__pyx_cur_scope->__pyx_v_x0s);
+  __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_x0s);
 
   /* "cyroot/_check_args.pyx":56
  * # noinspection DuplicatedCode
- * def _check_initial_guesses_uniqueness(xs: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):
- *     if not len(xs):             # <<<<<<<<<<<<<<
+ * def _check_initial_guesses_uniqueness(x0s: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):
+ *     if not len(x0s):             # <<<<<<<<<<<<<<
  *         raise ValueError('Empty.')
- *     elif isinstance(xs[0], np.ndarray):
+ *     elif isinstance(x0s[0], np.ndarray):
  */
-  __pyx_t_1 = __pyx_cur_scope->__pyx_v_xs;
+  __pyx_t_1 = __pyx_cur_scope->__pyx_v_x0s;
   __Pyx_INCREF(__pyx_t_1);
   __pyx_t_2 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = ((!(__pyx_t_2 != 0)) != 0);
   if (unlikely(__pyx_t_3)) {
 
     /* "cyroot/_check_args.pyx":57
- * def _check_initial_guesses_uniqueness(xs: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):
- *     if not len(xs):
+ * def _check_initial_guesses_uniqueness(x0s: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):
+ *     if not len(x0s):
  *         raise ValueError('Empty.')             # <<<<<<<<<<<<<<
- *     elif isinstance(xs[0], np.ndarray):
- *         if np.unique(xs if isinstance(xs, np.ndarray) else
+ *     elif isinstance(x0s[0], np.ndarray):
+ *         if np.unique(x0s if isinstance(x0s, np.ndarray) else
  */
     __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __PYX_ERR(0, 57, __pyx_L1_error)
 
     /* "cyroot/_check_args.pyx":56
  * # noinspection DuplicatedCode
- * def _check_initial_guesses_uniqueness(xs: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):
- *     if not len(xs):             # <<<<<<<<<<<<<<
+ * def _check_initial_guesses_uniqueness(x0s: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):
+ *     if not len(x0s):             # <<<<<<<<<<<<<<
  *         raise ValueError('Empty.')
- *     elif isinstance(xs[0], np.ndarray):
+ *     elif isinstance(x0s[0], np.ndarray):
  */
   }
 
   /* "cyroot/_check_args.pyx":58
- *     if not len(xs):
+ *     if not len(x0s):
  *         raise ValueError('Empty.')
- *     elif isinstance(xs[0], np.ndarray):             # <<<<<<<<<<<<<<
- *         if np.unique(xs if isinstance(xs, np.ndarray) else
- *                      np.stack(xs), axis=0).shape[0] < len(xs):
+ *     elif isinstance(x0s[0], np.ndarray):             # <<<<<<<<<<<<<<
+ *         if np.unique(x0s if isinstance(x0s, np.ndarray) else
+ *                      np.stack(x0s), axis=0).shape[0] < len(x0s):
  */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_cur_scope->__pyx_v_xs, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_cur_scope->__pyx_v_x0s, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = __Pyx_TypeCheck(__pyx_t_1, __pyx_ptype_5numpy_ndarray); 
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_4 = (__pyx_t_3 != 0);
   if (__pyx_t_4) {
 
     /* "cyroot/_check_args.pyx":59
  *         raise ValueError('Empty.')
- *     elif isinstance(xs[0], np.ndarray):
- *         if np.unique(xs if isinstance(xs, np.ndarray) else             # <<<<<<<<<<<<<<
- *                      np.stack(xs), axis=0).shape[0] < len(xs):
+ *     elif isinstance(x0s[0], np.ndarray):
+ *         if np.unique(x0s if isinstance(x0s, np.ndarray) else             # <<<<<<<<<<<<<<
+ *                      np.stack(x0s), axis=0).shape[0] < len(x0s):
  *             raise ValueError(f'Initial guesses must be unique. Got:\n' +
  */
     __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 59, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_unique); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 59, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_6 = __pyx_cur_scope->__pyx_v_xs;
+    __pyx_t_6 = __pyx_cur_scope->__pyx_v_x0s;
     __Pyx_INCREF(__pyx_t_6);
     __pyx_t_4 = __Pyx_TypeCheck(__pyx_t_6, __pyx_ptype_5numpy_ndarray); 
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if ((__pyx_t_4 != 0)) {
-      __Pyx_INCREF(__pyx_cur_scope->__pyx_v_xs);
-      __pyx_t_1 = __pyx_cur_scope->__pyx_v_xs;
+      __Pyx_INCREF(__pyx_cur_scope->__pyx_v_x0s);
+      __pyx_t_1 = __pyx_cur_scope->__pyx_v_x0s;
     } else {
 
       /* "cyroot/_check_args.pyx":60
- *     elif isinstance(xs[0], np.ndarray):
- *         if np.unique(xs if isinstance(xs, np.ndarray) else
- *                      np.stack(xs), axis=0).shape[0] < len(xs):             # <<<<<<<<<<<<<<
+ *     elif isinstance(x0s[0], np.ndarray):
+ *         if np.unique(x0s if isinstance(x0s, np.ndarray) else
+ *                      np.stack(x0s), axis=0).shape[0] < len(x0s):             # <<<<<<<<<<<<<<
  *             raise ValueError(f'Initial guesses must be unique. Got:\n' +
- *                              '\n'.join(repr(_) for _ in xs))
+ *                              '\n'.join(repr(_) for _ in x0s))
  */
       __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 60, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_stack); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 60, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __pyx_t_7 = NULL;
@@ -4303,180 +4303,180 @@
         if (likely(__pyx_t_7)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
           __Pyx_INCREF(__pyx_t_7);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_8, function);
         }
       }
-      __pyx_t_6 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_7, __pyx_cur_scope->__pyx_v_xs) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_cur_scope->__pyx_v_xs);
+      __pyx_t_6 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_7, __pyx_cur_scope->__pyx_v_x0s) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_cur_scope->__pyx_v_x0s);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 60, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __pyx_t_1 = __pyx_t_6;
       __pyx_t_6 = 0;
     }
 
     /* "cyroot/_check_args.pyx":59
  *         raise ValueError('Empty.')
- *     elif isinstance(xs[0], np.ndarray):
- *         if np.unique(xs if isinstance(xs, np.ndarray) else             # <<<<<<<<<<<<<<
- *                      np.stack(xs), axis=0).shape[0] < len(xs):
+ *     elif isinstance(x0s[0], np.ndarray):
+ *         if np.unique(x0s if isinstance(x0s, np.ndarray) else             # <<<<<<<<<<<<<<
+ *                      np.stack(x0s), axis=0).shape[0] < len(x0s):
  *             raise ValueError(f'Initial guesses must be unique. Got:\n' +
  */
     __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 59, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_1);
     __pyx_t_1 = 0;
 
     /* "cyroot/_check_args.pyx":60
- *     elif isinstance(xs[0], np.ndarray):
- *         if np.unique(xs if isinstance(xs, np.ndarray) else
- *                      np.stack(xs), axis=0).shape[0] < len(xs):             # <<<<<<<<<<<<<<
+ *     elif isinstance(x0s[0], np.ndarray):
+ *         if np.unique(x0s if isinstance(x0s, np.ndarray) else
+ *                      np.stack(x0s), axis=0).shape[0] < len(x0s):             # <<<<<<<<<<<<<<
  *             raise ValueError(f'Initial guesses must be unique. Got:\n' +
- *                              '\n'.join(repr(_) for _ in xs))
+ *                              '\n'.join(repr(_) for _ in x0s))
  */
     __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_axis, __pyx_int_0) < 0) __PYX_ERR(0, 60, __pyx_L1_error)
 
     /* "cyroot/_check_args.pyx":59
  *         raise ValueError('Empty.')
- *     elif isinstance(xs[0], np.ndarray):
- *         if np.unique(xs if isinstance(xs, np.ndarray) else             # <<<<<<<<<<<<<<
- *                      np.stack(xs), axis=0).shape[0] < len(xs):
+ *     elif isinstance(x0s[0], np.ndarray):
+ *         if np.unique(x0s if isinstance(x0s, np.ndarray) else             # <<<<<<<<<<<<<<
+ *                      np.stack(x0s), axis=0).shape[0] < len(x0s):
  *             raise ValueError(f'Initial guesses must be unique. Got:\n' +
  */
     __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_6, __pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 59, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "cyroot/_check_args.pyx":60
- *     elif isinstance(xs[0], np.ndarray):
- *         if np.unique(xs if isinstance(xs, np.ndarray) else
- *                      np.stack(xs), axis=0).shape[0] < len(xs):             # <<<<<<<<<<<<<<
+ *     elif isinstance(x0s[0], np.ndarray):
+ *         if np.unique(x0s if isinstance(x0s, np.ndarray) else
+ *                      np.stack(x0s), axis=0).shape[0] < len(x0s):             # <<<<<<<<<<<<<<
  *             raise ValueError(f'Initial guesses must be unique. Got:\n' +
- *                              '\n'.join(repr(_) for _ in xs))
+ *                              '\n'.join(repr(_) for _ in x0s))
  */
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_shape); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __pyx_t_8 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 60, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __pyx_cur_scope->__pyx_v_xs;
+    __pyx_t_1 = __pyx_cur_scope->__pyx_v_x0s;
     __Pyx_INCREF(__pyx_t_1);
     __pyx_t_2 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 60, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_6 = PyObject_RichCompare(__pyx_t_8, __pyx_t_1, Py_LT); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 60, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 60, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
     /* "cyroot/_check_args.pyx":59
  *         raise ValueError('Empty.')
- *     elif isinstance(xs[0], np.ndarray):
- *         if np.unique(xs if isinstance(xs, np.ndarray) else             # <<<<<<<<<<<<<<
- *                      np.stack(xs), axis=0).shape[0] < len(xs):
+ *     elif isinstance(x0s[0], np.ndarray):
+ *         if np.unique(x0s if isinstance(x0s, np.ndarray) else             # <<<<<<<<<<<<<<
+ *                      np.stack(x0s), axis=0).shape[0] < len(x0s):
  *             raise ValueError(f'Initial guesses must be unique. Got:\n' +
  */
     if (unlikely(__pyx_t_4)) {
 
       /* "cyroot/_check_args.pyx":62
- *                      np.stack(xs), axis=0).shape[0] < len(xs):
+ *                      np.stack(x0s), axis=0).shape[0] < len(x0s):
  *             raise ValueError(f'Initial guesses must be unique. Got:\n' +
- *                              '\n'.join(repr(_) for _ in xs))             # <<<<<<<<<<<<<<
- *     elif len(set(xs)) < len(xs):
- *         raise ValueError(f'Initial guesses must be unique. Got {xs}.')
+ *                              '\n'.join(repr(_) for _ in x0s))             # <<<<<<<<<<<<<<
+ *     elif len(set(x0s)) < len(x0s):
+ *         raise ValueError(f'Initial guesses must be unique. Got {x0s}.')
  */
       __pyx_t_6 = __pyx_pf_6cyroot_11_check_args_33_check_initial_guesses_uniqueness_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 62, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_1 = __Pyx_Generator_Next(__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_6 = PyUnicode_Join(__pyx_kp_u__4, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 62, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
       /* "cyroot/_check_args.pyx":61
- *         if np.unique(xs if isinstance(xs, np.ndarray) else
- *                      np.stack(xs), axis=0).shape[0] < len(xs):
+ *         if np.unique(x0s if isinstance(x0s, np.ndarray) else
+ *                      np.stack(x0s), axis=0).shape[0] < len(x0s):
  *             raise ValueError(f'Initial guesses must be unique. Got:\n' +             # <<<<<<<<<<<<<<
- *                              '\n'.join(repr(_) for _ in xs))
- *     elif len(set(xs)) < len(xs):
+ *                              '\n'.join(repr(_) for _ in x0s))
+ *     elif len(set(x0s)) < len(x0s):
  */
       __pyx_t_1 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Initial_guesses_must_be_unique_G, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 61, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 61, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __PYX_ERR(0, 61, __pyx_L1_error)
 
       /* "cyroot/_check_args.pyx":59
  *         raise ValueError('Empty.')
- *     elif isinstance(xs[0], np.ndarray):
- *         if np.unique(xs if isinstance(xs, np.ndarray) else             # <<<<<<<<<<<<<<
- *                      np.stack(xs), axis=0).shape[0] < len(xs):
+ *     elif isinstance(x0s[0], np.ndarray):
+ *         if np.unique(x0s if isinstance(x0s, np.ndarray) else             # <<<<<<<<<<<<<<
+ *                      np.stack(x0s), axis=0).shape[0] < len(x0s):
  *             raise ValueError(f'Initial guesses must be unique. Got:\n' +
  */
     }
 
     /* "cyroot/_check_args.pyx":58
- *     if not len(xs):
+ *     if not len(x0s):
  *         raise ValueError('Empty.')
- *     elif isinstance(xs[0], np.ndarray):             # <<<<<<<<<<<<<<
- *         if np.unique(xs if isinstance(xs, np.ndarray) else
- *                      np.stack(xs), axis=0).shape[0] < len(xs):
+ *     elif isinstance(x0s[0], np.ndarray):             # <<<<<<<<<<<<<<
+ *         if np.unique(x0s if isinstance(x0s, np.ndarray) else
+ *                      np.stack(x0s), axis=0).shape[0] < len(x0s):
  */
     goto __pyx_L3;
   }
 
   /* "cyroot/_check_args.pyx":63
  *             raise ValueError(f'Initial guesses must be unique. Got:\n' +
- *                              '\n'.join(repr(_) for _ in xs))
- *     elif len(set(xs)) < len(xs):             # <<<<<<<<<<<<<<
- *         raise ValueError(f'Initial guesses must be unique. Got {xs}.')
+ *                              '\n'.join(repr(_) for _ in x0s))
+ *     elif len(set(x0s)) < len(x0s):             # <<<<<<<<<<<<<<
+ *         raise ValueError(f'Initial guesses must be unique. Got {x0s}.')
  * 
  */
-  __pyx_t_6 = PySet_New(__pyx_cur_scope->__pyx_v_xs); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_6 = PySet_New(__pyx_cur_scope->__pyx_v_x0s); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_2 = PySet_GET_SIZE(__pyx_t_6); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __pyx_cur_scope->__pyx_v_xs;
+  __pyx_t_6 = __pyx_cur_scope->__pyx_v_x0s;
   __Pyx_INCREF(__pyx_t_6);
   __pyx_t_9 = PyObject_Length(__pyx_t_6); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_4 = ((__pyx_t_2 < __pyx_t_9) != 0);
   if (unlikely(__pyx_t_4)) {
 
     /* "cyroot/_check_args.pyx":64
- *                              '\n'.join(repr(_) for _ in xs))
- *     elif len(set(xs)) < len(xs):
- *         raise ValueError(f'Initial guesses must be unique. Got {xs}.')             # <<<<<<<<<<<<<<
+ *                              '\n'.join(repr(_) for _ in x0s))
+ *     elif len(set(x0s)) < len(x0s):
+ *         raise ValueError(f'Initial guesses must be unique. Got {x0s}.')             # <<<<<<<<<<<<<<
  * 
  * # noinspection DuplicatedCode
  */
     __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 64, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_9 = 0;
     __pyx_t_10 = 127;
     __Pyx_INCREF(__pyx_kp_u_Initial_guesses_must_be_unique_G_2);
     __pyx_t_9 += 36;
     __Pyx_GIVEREF(__pyx_kp_u_Initial_guesses_must_be_unique_G_2);
     PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_kp_u_Initial_guesses_must_be_unique_G_2);
-    __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_cur_scope->__pyx_v_xs, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_cur_scope->__pyx_v_x0s, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_10 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_1) > __pyx_t_10) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_1) : __pyx_t_10;
     __pyx_t_9 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_1);
     __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_kp_u_);
@@ -4491,27 +4491,27 @@
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __PYX_ERR(0, 64, __pyx_L1_error)
 
     /* "cyroot/_check_args.pyx":63
  *             raise ValueError(f'Initial guesses must be unique. Got:\n' +
- *                              '\n'.join(repr(_) for _ in xs))
- *     elif len(set(xs)) < len(xs):             # <<<<<<<<<<<<<<
- *         raise ValueError(f'Initial guesses must be unique. Got {xs}.')
+ *                              '\n'.join(repr(_) for _ in x0s))
+ *     elif len(set(x0s)) < len(x0s):             # <<<<<<<<<<<<<<
+ *         raise ValueError(f'Initial guesses must be unique. Got {x0s}.')
  * 
  */
   }
   __pyx_L3:;
 
   /* "cyroot/_check_args.pyx":55
  * 
  * # noinspection DuplicatedCode
- * def _check_initial_guesses_uniqueness(xs: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):             # <<<<<<<<<<<<<<
- *     if not len(xs):
+ * def _check_initial_guesses_uniqueness(x0s: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):             # <<<<<<<<<<<<<<
+ *     if not len(x0s):
  *         raise ValueError('Empty.')
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
@@ -4529,39 +4529,39 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cyroot/_check_args.pyx":67
  * 
  * # noinspection DuplicatedCode
- * def _check_initial_vals_uniqueness(f_xs: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):             # <<<<<<<<<<<<<<
- *     if not len(f_xs):
+ * def _check_initial_vals_uniqueness(f_x0s: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):             # <<<<<<<<<<<<<<
+ *     if not len(f_x0s):
  *         raise ValueError('Empty.')
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6cyroot_11_check_args_7_check_initial_vals_uniqueness(PyObject *__pyx_self, PyObject *__pyx_v_f_xs); /*proto*/
+static PyObject *__pyx_pw_6cyroot_11_check_args_7_check_initial_vals_uniqueness(PyObject *__pyx_self, PyObject *__pyx_v_f_x0s); /*proto*/
 static PyMethodDef __pyx_mdef_6cyroot_11_check_args_7_check_initial_vals_uniqueness = {"_check_initial_vals_uniqueness", (PyCFunction)__pyx_pw_6cyroot_11_check_args_7_check_initial_vals_uniqueness, METH_O, 0};
-static PyObject *__pyx_pw_6cyroot_11_check_args_7_check_initial_vals_uniqueness(PyObject *__pyx_self, PyObject *__pyx_v_f_xs) {
+static PyObject *__pyx_pw_6cyroot_11_check_args_7_check_initial_vals_uniqueness(PyObject *__pyx_self, PyObject *__pyx_v_f_x0s) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_check_initial_vals_uniqueness (wrapper)", 0);
-  __pyx_r = __pyx_pf_6cyroot_11_check_args_6_check_initial_vals_uniqueness(__pyx_self, ((PyObject *)__pyx_v_f_xs));
+  __pyx_r = __pyx_pf_6cyroot_11_check_args_6_check_initial_vals_uniqueness(__pyx_self, ((PyObject *)__pyx_v_f_x0s));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_6cyroot_11_check_args_30_check_initial_vals_uniqueness_2generator1(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
 /* "cyroot/_check_args.pyx":74
- *                      np.stack(f_xs), axis=0).shape[0] < len(f_xs):
+ *                      np.stack(f_x0s), axis=0).shape[0] < len(f_x0s):
  *             raise ValueError('Initial guesses\' values must be unique. '
- *                              'Got:\n' + '\n'.join(repr(_) for _ in f_xs))             # <<<<<<<<<<<<<<
- *     elif len(set(f_xs)) < len(f_xs):
+ *                              'Got:\n' + '\n'.join(repr(_) for _ in f_x0s))             # <<<<<<<<<<<<<<
+ *     elif len(set(f_x0s)) < len(f_x0s):
  *         raise ValueError('Initial guesses\' values must be unique. '
  */
 
 static PyObject *__pyx_pf_6cyroot_11_check_args_30_check_initial_vals_uniqueness_genexpr(PyObject *__pyx_self) {
   struct __pyx_obj_6cyroot_11_check_args___pyx_scope_struct_3_genexpr *__pyx_cur_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
@@ -4616,20 +4616,20 @@
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
   if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 74, __pyx_L1_error)
   __pyx_r = PyList_New(0); if (unlikely(!__pyx_r)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_r);
-  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_f_xs)) { __Pyx_RaiseClosureNameError("f_xs"); __PYX_ERR(0, 74, __pyx_L1_error) }
-  if (likely(PyList_CheckExact(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_f_xs)) || PyTuple_CheckExact(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_f_xs)) {
-    __pyx_t_1 = __pyx_cur_scope->__pyx_outer_scope->__pyx_v_f_xs; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
+  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_f_x0s)) { __Pyx_RaiseClosureNameError("f_x0s"); __PYX_ERR(0, 74, __pyx_L1_error) }
+  if (likely(PyList_CheckExact(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_f_x0s)) || PyTuple_CheckExact(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_f_x0s)) {
+    __pyx_t_1 = __pyx_cur_scope->__pyx_outer_scope->__pyx_v_f_x0s; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
     __pyx_t_3 = NULL;
   } else {
-    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_f_xs); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_f_x0s); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 74, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_3)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
@@ -4689,20 +4689,20 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cyroot/_check_args.pyx":67
  * 
  * # noinspection DuplicatedCode
- * def _check_initial_vals_uniqueness(f_xs: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):             # <<<<<<<<<<<<<<
- *     if not len(f_xs):
+ * def _check_initial_vals_uniqueness(f_x0s: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):             # <<<<<<<<<<<<<<
+ *     if not len(f_x0s):
  *         raise ValueError('Empty.')
  */
 
-static PyObject *__pyx_pf_6cyroot_11_check_args_6_check_initial_vals_uniqueness(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_f_xs) {
+static PyObject *__pyx_pf_6cyroot_11_check_args_6_check_initial_vals_uniqueness(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_f_x0s) {
   struct __pyx_obj_6cyroot_11_check_args___pyx_scope_struct_2__check_initial_vals_uniqueness *__pyx_cur_scope;
   PyObject *__pyx_gb_6cyroot_11_check_args_30_check_initial_vals_uniqueness_2generator1 = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t __pyx_t_2;
   int __pyx_t_3;
@@ -4721,95 +4721,95 @@
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_6cyroot_11_check_args___pyx_scope_struct_2__check_initial_vals_uniqueness *)Py_None);
     __Pyx_INCREF(Py_None);
     __PYX_ERR(0, 67, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
-  __pyx_cur_scope->__pyx_v_f_xs = __pyx_v_f_xs;
-  __Pyx_INCREF(__pyx_cur_scope->__pyx_v_f_xs);
-  __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_f_xs);
+  __pyx_cur_scope->__pyx_v_f_x0s = __pyx_v_f_x0s;
+  __Pyx_INCREF(__pyx_cur_scope->__pyx_v_f_x0s);
+  __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_f_x0s);
 
   /* "cyroot/_check_args.pyx":68
  * # noinspection DuplicatedCode
- * def _check_initial_vals_uniqueness(f_xs: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):
- *     if not len(f_xs):             # <<<<<<<<<<<<<<
+ * def _check_initial_vals_uniqueness(f_x0s: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):
+ *     if not len(f_x0s):             # <<<<<<<<<<<<<<
  *         raise ValueError('Empty.')
- *     elif isinstance(f_xs[0], np.ndarray):
+ *     elif isinstance(f_x0s[0], np.ndarray):
  */
-  __pyx_t_1 = __pyx_cur_scope->__pyx_v_f_xs;
+  __pyx_t_1 = __pyx_cur_scope->__pyx_v_f_x0s;
   __Pyx_INCREF(__pyx_t_1);
   __pyx_t_2 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = ((!(__pyx_t_2 != 0)) != 0);
   if (unlikely(__pyx_t_3)) {
 
     /* "cyroot/_check_args.pyx":69
- * def _check_initial_vals_uniqueness(f_xs: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):
- *     if not len(f_xs):
+ * def _check_initial_vals_uniqueness(f_x0s: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):
+ *     if not len(f_x0s):
  *         raise ValueError('Empty.')             # <<<<<<<<<<<<<<
- *     elif isinstance(f_xs[0], np.ndarray):
- *         if np.unique(f_xs if isinstance(f_xs, np.ndarray) else
+ *     elif isinstance(f_x0s[0], np.ndarray):
+ *         if np.unique(f_x0s if isinstance(f_x0s, np.ndarray) else
  */
     __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __PYX_ERR(0, 69, __pyx_L1_error)
 
     /* "cyroot/_check_args.pyx":68
  * # noinspection DuplicatedCode
- * def _check_initial_vals_uniqueness(f_xs: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):
- *     if not len(f_xs):             # <<<<<<<<<<<<<<
+ * def _check_initial_vals_uniqueness(f_x0s: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):
+ *     if not len(f_x0s):             # <<<<<<<<<<<<<<
  *         raise ValueError('Empty.')
- *     elif isinstance(f_xs[0], np.ndarray):
+ *     elif isinstance(f_x0s[0], np.ndarray):
  */
   }
 
   /* "cyroot/_check_args.pyx":70
- *     if not len(f_xs):
+ *     if not len(f_x0s):
  *         raise ValueError('Empty.')
- *     elif isinstance(f_xs[0], np.ndarray):             # <<<<<<<<<<<<<<
- *         if np.unique(f_xs if isinstance(f_xs, np.ndarray) else
- *                      np.stack(f_xs), axis=0).shape[0] < len(f_xs):
+ *     elif isinstance(f_x0s[0], np.ndarray):             # <<<<<<<<<<<<<<
+ *         if np.unique(f_x0s if isinstance(f_x0s, np.ndarray) else
+ *                      np.stack(f_x0s), axis=0).shape[0] < len(f_x0s):
  */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_cur_scope->__pyx_v_f_xs, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_cur_scope->__pyx_v_f_x0s, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = __Pyx_TypeCheck(__pyx_t_1, __pyx_ptype_5numpy_ndarray); 
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_4 = (__pyx_t_3 != 0);
   if (__pyx_t_4) {
 
     /* "cyroot/_check_args.pyx":71
  *         raise ValueError('Empty.')
- *     elif isinstance(f_xs[0], np.ndarray):
- *         if np.unique(f_xs if isinstance(f_xs, np.ndarray) else             # <<<<<<<<<<<<<<
- *                      np.stack(f_xs), axis=0).shape[0] < len(f_xs):
+ *     elif isinstance(f_x0s[0], np.ndarray):
+ *         if np.unique(f_x0s if isinstance(f_x0s, np.ndarray) else             # <<<<<<<<<<<<<<
+ *                      np.stack(f_x0s), axis=0).shape[0] < len(f_x0s):
  *             raise ValueError('Initial guesses\' values must be unique. '
  */
     __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 71, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_unique); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 71, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_6 = __pyx_cur_scope->__pyx_v_f_xs;
+    __pyx_t_6 = __pyx_cur_scope->__pyx_v_f_x0s;
     __Pyx_INCREF(__pyx_t_6);
     __pyx_t_4 = __Pyx_TypeCheck(__pyx_t_6, __pyx_ptype_5numpy_ndarray); 
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if ((__pyx_t_4 != 0)) {
-      __Pyx_INCREF(__pyx_cur_scope->__pyx_v_f_xs);
-      __pyx_t_1 = __pyx_cur_scope->__pyx_v_f_xs;
+      __Pyx_INCREF(__pyx_cur_scope->__pyx_v_f_x0s);
+      __pyx_t_1 = __pyx_cur_scope->__pyx_v_f_x0s;
     } else {
 
       /* "cyroot/_check_args.pyx":72
- *     elif isinstance(f_xs[0], np.ndarray):
- *         if np.unique(f_xs if isinstance(f_xs, np.ndarray) else
- *                      np.stack(f_xs), axis=0).shape[0] < len(f_xs):             # <<<<<<<<<<<<<<
+ *     elif isinstance(f_x0s[0], np.ndarray):
+ *         if np.unique(f_x0s if isinstance(f_x0s, np.ndarray) else
+ *                      np.stack(f_x0s), axis=0).shape[0] < len(f_x0s):             # <<<<<<<<<<<<<<
  *             raise ValueError('Initial guesses\' values must be unique. '
- *                              'Got:\n' + '\n'.join(repr(_) for _ in f_xs))
+ *                              'Got:\n' + '\n'.join(repr(_) for _ in f_x0s))
  */
       __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 72, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_stack); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 72, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __pyx_t_7 = NULL;
@@ -4818,99 +4818,99 @@
         if (likely(__pyx_t_7)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
           __Pyx_INCREF(__pyx_t_7);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_8, function);
         }
       }
-      __pyx_t_6 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_7, __pyx_cur_scope->__pyx_v_f_xs) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_cur_scope->__pyx_v_f_xs);
+      __pyx_t_6 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_7, __pyx_cur_scope->__pyx_v_f_x0s) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_cur_scope->__pyx_v_f_x0s);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 72, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __pyx_t_1 = __pyx_t_6;
       __pyx_t_6 = 0;
     }
 
     /* "cyroot/_check_args.pyx":71
  *         raise ValueError('Empty.')
- *     elif isinstance(f_xs[0], np.ndarray):
- *         if np.unique(f_xs if isinstance(f_xs, np.ndarray) else             # <<<<<<<<<<<<<<
- *                      np.stack(f_xs), axis=0).shape[0] < len(f_xs):
+ *     elif isinstance(f_x0s[0], np.ndarray):
+ *         if np.unique(f_x0s if isinstance(f_x0s, np.ndarray) else             # <<<<<<<<<<<<<<
+ *                      np.stack(f_x0s), axis=0).shape[0] < len(f_x0s):
  *             raise ValueError('Initial guesses\' values must be unique. '
  */
     __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 71, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_1);
     __pyx_t_1 = 0;
 
     /* "cyroot/_check_args.pyx":72
- *     elif isinstance(f_xs[0], np.ndarray):
- *         if np.unique(f_xs if isinstance(f_xs, np.ndarray) else
- *                      np.stack(f_xs), axis=0).shape[0] < len(f_xs):             # <<<<<<<<<<<<<<
+ *     elif isinstance(f_x0s[0], np.ndarray):
+ *         if np.unique(f_x0s if isinstance(f_x0s, np.ndarray) else
+ *                      np.stack(f_x0s), axis=0).shape[0] < len(f_x0s):             # <<<<<<<<<<<<<<
  *             raise ValueError('Initial guesses\' values must be unique. '
- *                              'Got:\n' + '\n'.join(repr(_) for _ in f_xs))
+ *                              'Got:\n' + '\n'.join(repr(_) for _ in f_x0s))
  */
     __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_axis, __pyx_int_0) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
 
     /* "cyroot/_check_args.pyx":71
  *         raise ValueError('Empty.')
- *     elif isinstance(f_xs[0], np.ndarray):
- *         if np.unique(f_xs if isinstance(f_xs, np.ndarray) else             # <<<<<<<<<<<<<<
- *                      np.stack(f_xs), axis=0).shape[0] < len(f_xs):
+ *     elif isinstance(f_x0s[0], np.ndarray):
+ *         if np.unique(f_x0s if isinstance(f_x0s, np.ndarray) else             # <<<<<<<<<<<<<<
+ *                      np.stack(f_x0s), axis=0).shape[0] < len(f_x0s):
  *             raise ValueError('Initial guesses\' values must be unique. '
  */
     __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_6, __pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 71, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "cyroot/_check_args.pyx":72
- *     elif isinstance(f_xs[0], np.ndarray):
- *         if np.unique(f_xs if isinstance(f_xs, np.ndarray) else
- *                      np.stack(f_xs), axis=0).shape[0] < len(f_xs):             # <<<<<<<<<<<<<<
+ *     elif isinstance(f_x0s[0], np.ndarray):
+ *         if np.unique(f_x0s if isinstance(f_x0s, np.ndarray) else
+ *                      np.stack(f_x0s), axis=0).shape[0] < len(f_x0s):             # <<<<<<<<<<<<<<
  *             raise ValueError('Initial guesses\' values must be unique. '
- *                              'Got:\n' + '\n'.join(repr(_) for _ in f_xs))
+ *                              'Got:\n' + '\n'.join(repr(_) for _ in f_x0s))
  */
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_shape); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __pyx_t_8 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 72, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __pyx_cur_scope->__pyx_v_f_xs;
+    __pyx_t_1 = __pyx_cur_scope->__pyx_v_f_x0s;
     __Pyx_INCREF(__pyx_t_1);
     __pyx_t_2 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 72, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_6 = PyObject_RichCompare(__pyx_t_8, __pyx_t_1, Py_LT); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 72, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 72, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
     /* "cyroot/_check_args.pyx":71
  *         raise ValueError('Empty.')
- *     elif isinstance(f_xs[0], np.ndarray):
- *         if np.unique(f_xs if isinstance(f_xs, np.ndarray) else             # <<<<<<<<<<<<<<
- *                      np.stack(f_xs), axis=0).shape[0] < len(f_xs):
+ *     elif isinstance(f_x0s[0], np.ndarray):
+ *         if np.unique(f_x0s if isinstance(f_x0s, np.ndarray) else             # <<<<<<<<<<<<<<
+ *                      np.stack(f_x0s), axis=0).shape[0] < len(f_x0s):
  *             raise ValueError('Initial guesses\' values must be unique. '
  */
     if (unlikely(__pyx_t_4)) {
 
       /* "cyroot/_check_args.pyx":74
- *                      np.stack(f_xs), axis=0).shape[0] < len(f_xs):
+ *                      np.stack(f_x0s), axis=0).shape[0] < len(f_x0s):
  *             raise ValueError('Initial guesses\' values must be unique. '
- *                              'Got:\n' + '\n'.join(repr(_) for _ in f_xs))             # <<<<<<<<<<<<<<
- *     elif len(set(f_xs)) < len(f_xs):
+ *                              'Got:\n' + '\n'.join(repr(_) for _ in f_x0s))             # <<<<<<<<<<<<<<
+ *     elif len(set(f_x0s)) < len(f_x0s):
  *         raise ValueError('Initial guesses\' values must be unique. '
  */
       __pyx_t_6 = __pyx_pf_6cyroot_11_check_args_30_check_initial_vals_uniqueness_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 74, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_1 = __Pyx_Generator_Next(__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
@@ -4918,131 +4918,131 @@
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_1 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Initial_guesses_values_must_be_u, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
       /* "cyroot/_check_args.pyx":73
- *         if np.unique(f_xs if isinstance(f_xs, np.ndarray) else
- *                      np.stack(f_xs), axis=0).shape[0] < len(f_xs):
+ *         if np.unique(f_x0s if isinstance(f_x0s, np.ndarray) else
+ *                      np.stack(f_x0s), axis=0).shape[0] < len(f_x0s):
  *             raise ValueError('Initial guesses\' values must be unique. '             # <<<<<<<<<<<<<<
- *                              'Got:\n' + '\n'.join(repr(_) for _ in f_xs))
- *     elif len(set(f_xs)) < len(f_xs):
+ *                              'Got:\n' + '\n'.join(repr(_) for _ in f_x0s))
+ *     elif len(set(f_x0s)) < len(f_x0s):
  */
       __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 73, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __PYX_ERR(0, 73, __pyx_L1_error)
 
       /* "cyroot/_check_args.pyx":71
  *         raise ValueError('Empty.')
- *     elif isinstance(f_xs[0], np.ndarray):
- *         if np.unique(f_xs if isinstance(f_xs, np.ndarray) else             # <<<<<<<<<<<<<<
- *                      np.stack(f_xs), axis=0).shape[0] < len(f_xs):
+ *     elif isinstance(f_x0s[0], np.ndarray):
+ *         if np.unique(f_x0s if isinstance(f_x0s, np.ndarray) else             # <<<<<<<<<<<<<<
+ *                      np.stack(f_x0s), axis=0).shape[0] < len(f_x0s):
  *             raise ValueError('Initial guesses\' values must be unique. '
  */
     }
 
     /* "cyroot/_check_args.pyx":70
- *     if not len(f_xs):
+ *     if not len(f_x0s):
  *         raise ValueError('Empty.')
- *     elif isinstance(f_xs[0], np.ndarray):             # <<<<<<<<<<<<<<
- *         if np.unique(f_xs if isinstance(f_xs, np.ndarray) else
- *                      np.stack(f_xs), axis=0).shape[0] < len(f_xs):
+ *     elif isinstance(f_x0s[0], np.ndarray):             # <<<<<<<<<<<<<<
+ *         if np.unique(f_x0s if isinstance(f_x0s, np.ndarray) else
+ *                      np.stack(f_x0s), axis=0).shape[0] < len(f_x0s):
  */
     goto __pyx_L3;
   }
 
   /* "cyroot/_check_args.pyx":75
  *             raise ValueError('Initial guesses\' values must be unique. '
- *                              'Got:\n' + '\n'.join(repr(_) for _ in f_xs))
- *     elif len(set(f_xs)) < len(f_xs):             # <<<<<<<<<<<<<<
+ *                              'Got:\n' + '\n'.join(repr(_) for _ in f_x0s))
+ *     elif len(set(f_x0s)) < len(f_x0s):             # <<<<<<<<<<<<<<
  *         raise ValueError('Initial guesses\' values must be unique. '
- *                          f'Got {f_xs}.')
+ *                          f'Got {f_x0s}.')
  */
-  __pyx_t_6 = PySet_New(__pyx_cur_scope->__pyx_v_f_xs); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_6 = PySet_New(__pyx_cur_scope->__pyx_v_f_x0s); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_2 = PySet_GET_SIZE(__pyx_t_6); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __pyx_cur_scope->__pyx_v_f_xs;
+  __pyx_t_6 = __pyx_cur_scope->__pyx_v_f_x0s;
   __Pyx_INCREF(__pyx_t_6);
   __pyx_t_9 = PyObject_Length(__pyx_t_6); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_4 = ((__pyx_t_2 < __pyx_t_9) != 0);
   if (unlikely(__pyx_t_4)) {
 
     /* "cyroot/_check_args.pyx":76
- *                              'Got:\n' + '\n'.join(repr(_) for _ in f_xs))
- *     elif len(set(f_xs)) < len(f_xs):
+ *                              'Got:\n' + '\n'.join(repr(_) for _ in f_x0s))
+ *     elif len(set(f_x0s)) < len(f_x0s):
  *         raise ValueError('Initial guesses\' values must be unique. '             # <<<<<<<<<<<<<<
- *                          f'Got {f_xs}.')
+ *                          f'Got {f_x0s}.')
  * 
  */
     __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 76, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_9 = 0;
     __pyx_t_10 = 127;
     __Pyx_INCREF(__pyx_kp_u_Initial_guesses_values_must_be_u_2);
     __pyx_t_9 += 44;
     __Pyx_GIVEREF(__pyx_kp_u_Initial_guesses_values_must_be_u_2);
     PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_kp_u_Initial_guesses_values_must_be_u_2);
 
     /* "cyroot/_check_args.pyx":77
- *     elif len(set(f_xs)) < len(f_xs):
+ *     elif len(set(f_x0s)) < len(f_x0s):
  *         raise ValueError('Initial guesses\' values must be unique. '
- *                          f'Got {f_xs}.')             # <<<<<<<<<<<<<<
+ *                          f'Got {f_x0s}.')             # <<<<<<<<<<<<<<
  * 
  * ################################################################################
  */
-    __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_cur_scope->__pyx_v_f_xs, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 77, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_cur_scope->__pyx_v_f_x0s, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 77, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_10 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_1) > __pyx_t_10) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_1) : __pyx_t_10;
     __pyx_t_9 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_1);
     __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_kp_u_);
     __pyx_t_9 += 1;
     __Pyx_GIVEREF(__pyx_kp_u_);
     PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_kp_u_);
 
     /* "cyroot/_check_args.pyx":76
- *                              'Got:\n' + '\n'.join(repr(_) for _ in f_xs))
- *     elif len(set(f_xs)) < len(f_xs):
+ *                              'Got:\n' + '\n'.join(repr(_) for _ in f_x0s))
+ *     elif len(set(f_x0s)) < len(f_x0s):
  *         raise ValueError('Initial guesses\' values must be unique. '             # <<<<<<<<<<<<<<
- *                          f'Got {f_xs}.')
+ *                          f'Got {f_x0s}.')
  * 
  */
     __pyx_t_1 = __Pyx_PyUnicode_Join(__pyx_t_6, 3, __pyx_t_9, __pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 76, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __PYX_ERR(0, 76, __pyx_L1_error)
 
     /* "cyroot/_check_args.pyx":75
  *             raise ValueError('Initial guesses\' values must be unique. '
- *                              'Got:\n' + '\n'.join(repr(_) for _ in f_xs))
- *     elif len(set(f_xs)) < len(f_xs):             # <<<<<<<<<<<<<<
+ *                              'Got:\n' + '\n'.join(repr(_) for _ in f_x0s))
+ *     elif len(set(f_x0s)) < len(f_x0s):             # <<<<<<<<<<<<<<
  *         raise ValueError('Initial guesses\' values must be unique. '
- *                          f'Got {f_xs}.')
+ *                          f'Got {f_x0s}.')
  */
   }
   __pyx_L3:;
 
   /* "cyroot/_check_args.pyx":67
  * 
  * # noinspection DuplicatedCode
- * def _check_initial_vals_uniqueness(f_xs: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):             # <<<<<<<<<<<<<<
- *     if not len(f_xs):
+ * def _check_initial_vals_uniqueness(f_x0s: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):             # <<<<<<<<<<<<<<
+ *     if not len(f_x0s):
  *         raise ValueError('Empty.')
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
@@ -5770,19 +5770,19 @@
   return __pyx_r;
 }
 
 /* "cyroot/_check_args.pyx":178
  * 
  * # noinspection DuplicatedCode
  * cdef inline bint _check_stop_cond_scalar_initial_guesses(             # <<<<<<<<<<<<<<
- *         double[:] xs,
- *         double[:] f_xs,
+ *         double[:] x0s,
+ *         double[:] f_x0s,
  */
 
-static CYTHON_INLINE int __pyx_f_6cyroot_11_check_args__check_stop_cond_scalar_initial_guesses(__Pyx_memviewslice __pyx_v_xs, __Pyx_memviewslice __pyx_v_f_xs, double __pyx_v_etol, double __pyx_v_ertol, double __pyx_v_ptol, double __pyx_v_prtol, double *__pyx_v_r, double *__pyx_v_f_r, double *__pyx_v_precision, double *__pyx_v_error, int *__pyx_v_converged, int *__pyx_v_optimal) {
+static CYTHON_INLINE int __pyx_f_6cyroot_11_check_args__check_stop_cond_scalar_initial_guesses(__Pyx_memviewslice __pyx_v_x0s, __Pyx_memviewslice __pyx_v_f_x0s, double __pyx_v_etol, double __pyx_v_ertol, double __pyx_v_ptol, double __pyx_v_prtol, double *__pyx_v_r, double *__pyx_v_f_r, double *__pyx_v_precision, double *__pyx_v_error, int *__pyx_v_converged, int *__pyx_v_optimal) {
   __Pyx_memviewslice __pyx_v_errors = { 0, 0, { 0 }, { 0 }, { 0 } };
   unsigned long __pyx_v_best_i;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t __pyx_t_3;
@@ -5797,199 +5797,199 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_check_stop_cond_scalar_initial_guesses", 0);
 
   /* "cyroot/_check_args.pyx":192
  *         bint* optimal):
  *     """Check if stop condition is already met."""
- *     if xs.shape[0] == 0:             # <<<<<<<<<<<<<<
+ *     if x0s.shape[0] == 0:             # <<<<<<<<<<<<<<
  *         raise ValueError('Empty sequence.')
- *     if xs.shape[0] == 1:
+ *     if x0s.shape[0] == 1:
  */
-  __pyx_t_1 = (((__pyx_v_xs.shape[0]) == 0) != 0);
+  __pyx_t_1 = (((__pyx_v_x0s.shape[0]) == 0) != 0);
   if (unlikely(__pyx_t_1)) {
 
     /* "cyroot/_check_args.pyx":193
  *     """Check if stop condition is already met."""
- *     if xs.shape[0] == 0:
+ *     if x0s.shape[0] == 0:
  *         raise ValueError('Empty sequence.')             # <<<<<<<<<<<<<<
- *     if xs.shape[0] == 1:
- *         r[0], f_r[0] = xs[0], f_xs[0]
+ *     if x0s.shape[0] == 1:
+ *         r[0], f_r[0] = x0s[0], f_x0s[0]
  */
     __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(0, 193, __pyx_L1_error)
 
     /* "cyroot/_check_args.pyx":192
  *         bint* optimal):
  *     """Check if stop condition is already met."""
- *     if xs.shape[0] == 0:             # <<<<<<<<<<<<<<
+ *     if x0s.shape[0] == 0:             # <<<<<<<<<<<<<<
  *         raise ValueError('Empty sequence.')
- *     if xs.shape[0] == 1:
+ *     if x0s.shape[0] == 1:
  */
   }
 
   /* "cyroot/_check_args.pyx":194
- *     if xs.shape[0] == 0:
+ *     if x0s.shape[0] == 0:
  *         raise ValueError('Empty sequence.')
- *     if xs.shape[0] == 1:             # <<<<<<<<<<<<<<
- *         r[0], f_r[0] = xs[0], f_xs[0]
+ *     if x0s.shape[0] == 1:             # <<<<<<<<<<<<<<
+ *         r[0], f_r[0] = x0s[0], f_x0s[0]
  *         precision[0] = math.INFINITY
  */
-  __pyx_t_1 = (((__pyx_v_xs.shape[0]) == 1) != 0);
+  __pyx_t_1 = (((__pyx_v_x0s.shape[0]) == 1) != 0);
   if (__pyx_t_1) {
 
     /* "cyroot/_check_args.pyx":195
  *         raise ValueError('Empty sequence.')
- *     if xs.shape[0] == 1:
- *         r[0], f_r[0] = xs[0], f_xs[0]             # <<<<<<<<<<<<<<
+ *     if x0s.shape[0] == 1:
+ *         r[0], f_r[0] = x0s[0], f_x0s[0]             # <<<<<<<<<<<<<<
  *         precision[0] = math.INFINITY
- *         error[0] = math.fabs(f_xs[0])
+ *         error[0] = math.fabs(f_x0s[0])
  */
     __pyx_t_3 = 0;
-    if (__pyx_t_3 < 0) __pyx_t_3 += __pyx_v_xs.shape[0];
-    __pyx_t_4 = (*((double *) ( /* dim=0 */ (__pyx_v_xs.data + __pyx_t_3 * __pyx_v_xs.strides[0]) )));
+    if (__pyx_t_3 < 0) __pyx_t_3 += __pyx_v_x0s.shape[0];
+    __pyx_t_4 = (*((double *) ( /* dim=0 */ (__pyx_v_x0s.data + __pyx_t_3 * __pyx_v_x0s.strides[0]) )));
     __pyx_t_3 = 0;
-    if (__pyx_t_3 < 0) __pyx_t_3 += __pyx_v_f_xs.shape[0];
-    __pyx_t_5 = (*((double *) ( /* dim=0 */ (__pyx_v_f_xs.data + __pyx_t_3 * __pyx_v_f_xs.strides[0]) )));
+    if (__pyx_t_3 < 0) __pyx_t_3 += __pyx_v_f_x0s.shape[0];
+    __pyx_t_5 = (*((double *) ( /* dim=0 */ (__pyx_v_f_x0s.data + __pyx_t_3 * __pyx_v_f_x0s.strides[0]) )));
     (__pyx_v_r[0]) = __pyx_t_4;
     (__pyx_v_f_r[0]) = __pyx_t_5;
 
     /* "cyroot/_check_args.pyx":196
- *     if xs.shape[0] == 1:
- *         r[0], f_r[0] = xs[0], f_xs[0]
+ *     if x0s.shape[0] == 1:
+ *         r[0], f_r[0] = x0s[0], f_x0s[0]
  *         precision[0] = math.INFINITY             # <<<<<<<<<<<<<<
- *         error[0] = math.fabs(f_xs[0])
+ *         error[0] = math.fabs(f_x0s[0])
  *         optimal[0] = sops.isclose(0, error[0], ertol, etol)
  */
     (__pyx_v_precision[0]) = INFINITY;
 
     /* "cyroot/_check_args.pyx":197
- *         r[0], f_r[0] = xs[0], f_xs[0]
+ *         r[0], f_r[0] = x0s[0], f_x0s[0]
  *         precision[0] = math.INFINITY
- *         error[0] = math.fabs(f_xs[0])             # <<<<<<<<<<<<<<
+ *         error[0] = math.fabs(f_x0s[0])             # <<<<<<<<<<<<<<
  *         optimal[0] = sops.isclose(0, error[0], ertol, etol)
  *         converged[0] = optimal[0]
  */
     __pyx_t_3 = 0;
-    if (__pyx_t_3 < 0) __pyx_t_3 += __pyx_v_f_xs.shape[0];
-    (__pyx_v_error[0]) = fabs((*((double *) ( /* dim=0 */ (__pyx_v_f_xs.data + __pyx_t_3 * __pyx_v_f_xs.strides[0]) ))));
+    if (__pyx_t_3 < 0) __pyx_t_3 += __pyx_v_f_x0s.shape[0];
+    (__pyx_v_error[0]) = fabs((*((double *) ( /* dim=0 */ (__pyx_v_f_x0s.data + __pyx_t_3 * __pyx_v_f_x0s.strides[0]) ))));
 
     /* "cyroot/_check_args.pyx":198
  *         precision[0] = math.INFINITY
- *         error[0] = math.fabs(f_xs[0])
+ *         error[0] = math.fabs(f_x0s[0])
  *         optimal[0] = sops.isclose(0, error[0], ertol, etol)             # <<<<<<<<<<<<<<
  *         converged[0] = optimal[0]
  *         return optimal[0]
  */
     __pyx_t_6.__pyx_n = 2;
     __pyx_t_6.rtol = __pyx_v_ertol;
     __pyx_t_6.atol = __pyx_v_etol;
     __pyx_t_1 = __pyx_f_6cyroot_3ops_10scalar_ops_isclose(0.0, (__pyx_v_error[0]), &__pyx_t_6); 
     (__pyx_v_optimal[0]) = __pyx_t_1;
 
     /* "cyroot/_check_args.pyx":199
- *         error[0] = math.fabs(f_xs[0])
+ *         error[0] = math.fabs(f_x0s[0])
  *         optimal[0] = sops.isclose(0, error[0], ertol, etol)
  *         converged[0] = optimal[0]             # <<<<<<<<<<<<<<
  *         return optimal[0]
- *     cdef double[:] errors = vops.fabs(f_xs)
+ *     cdef double[:] errors = vops.fabs(f_x0s)
  */
     (__pyx_v_converged[0]) = (__pyx_v_optimal[0]);
 
     /* "cyroot/_check_args.pyx":200
  *         optimal[0] = sops.isclose(0, error[0], ertol, etol)
  *         converged[0] = optimal[0]
  *         return optimal[0]             # <<<<<<<<<<<<<<
- *     cdef double[:] errors = vops.fabs(f_xs)
+ *     cdef double[:] errors = vops.fabs(f_x0s)
  *     cdef unsigned long best_i = vops.argmin(errors)
  */
     __pyx_r = (__pyx_v_optimal[0]);
     goto __pyx_L0;
 
     /* "cyroot/_check_args.pyx":194
- *     if xs.shape[0] == 0:
+ *     if x0s.shape[0] == 0:
  *         raise ValueError('Empty sequence.')
- *     if xs.shape[0] == 1:             # <<<<<<<<<<<<<<
- *         r[0], f_r[0] = xs[0], f_xs[0]
+ *     if x0s.shape[0] == 1:             # <<<<<<<<<<<<<<
+ *         r[0], f_r[0] = x0s[0], f_x0s[0]
  *         precision[0] = math.INFINITY
  */
   }
 
   /* "cyroot/_check_args.pyx":201
  *         converged[0] = optimal[0]
  *         return optimal[0]
- *     cdef double[:] errors = vops.fabs(f_xs)             # <<<<<<<<<<<<<<
+ *     cdef double[:] errors = vops.fabs(f_x0s)             # <<<<<<<<<<<<<<
  *     cdef unsigned long best_i = vops.argmin(errors)
- *     r[0], f_r[0] = xs[best_i], f_xs[best_i]
+ *     r[0], f_r[0] = x0s[best_i], f_x0s[best_i]
  */
-  __pyx_t_7 = __pyx_f_6cyroot_3ops_10vector_ops_fabs(__pyx_v_f_xs); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 201, __pyx_L1_error)
+  __pyx_t_7 = __pyx_f_6cyroot_3ops_10vector_ops_fabs(__pyx_v_f_x0s); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 201, __pyx_L1_error)
   __pyx_v_errors = __pyx_t_7;
   __pyx_t_7.memview = NULL;
   __pyx_t_7.data = NULL;
 
   /* "cyroot/_check_args.pyx":202
  *         return optimal[0]
- *     cdef double[:] errors = vops.fabs(f_xs)
+ *     cdef double[:] errors = vops.fabs(f_x0s)
  *     cdef unsigned long best_i = vops.argmin(errors)             # <<<<<<<<<<<<<<
- *     r[0], f_r[0] = xs[best_i], f_xs[best_i]
+ *     r[0], f_r[0] = x0s[best_i], f_x0s[best_i]
  *     error[0] = errors[best_i]
  */
   __pyx_v_best_i = __pyx_f_6cyroot_3ops_10vector_ops_argmin(__pyx_v_errors);
 
   /* "cyroot/_check_args.pyx":203
- *     cdef double[:] errors = vops.fabs(f_xs)
+ *     cdef double[:] errors = vops.fabs(f_x0s)
  *     cdef unsigned long best_i = vops.argmin(errors)
- *     r[0], f_r[0] = xs[best_i], f_xs[best_i]             # <<<<<<<<<<<<<<
+ *     r[0], f_r[0] = x0s[best_i], f_x0s[best_i]             # <<<<<<<<<<<<<<
  *     error[0] = errors[best_i]
- *     precision[0] = vops.max(xs) - vops.min(xs)
+ *     precision[0] = vops.max(x0s) - vops.min(x0s)
  */
   __pyx_t_8 = __pyx_v_best_i;
-  __pyx_t_5 = (*((double *) ( /* dim=0 */ (__pyx_v_xs.data + __pyx_t_8 * __pyx_v_xs.strides[0]) )));
+  __pyx_t_5 = (*((double *) ( /* dim=0 */ (__pyx_v_x0s.data + __pyx_t_8 * __pyx_v_x0s.strides[0]) )));
   __pyx_t_8 = __pyx_v_best_i;
-  __pyx_t_4 = (*((double *) ( /* dim=0 */ (__pyx_v_f_xs.data + __pyx_t_8 * __pyx_v_f_xs.strides[0]) )));
+  __pyx_t_4 = (*((double *) ( /* dim=0 */ (__pyx_v_f_x0s.data + __pyx_t_8 * __pyx_v_f_x0s.strides[0]) )));
   (__pyx_v_r[0]) = __pyx_t_5;
   (__pyx_v_f_r[0]) = __pyx_t_4;
 
   /* "cyroot/_check_args.pyx":204
  *     cdef unsigned long best_i = vops.argmin(errors)
- *     r[0], f_r[0] = xs[best_i], f_xs[best_i]
+ *     r[0], f_r[0] = x0s[best_i], f_x0s[best_i]
  *     error[0] = errors[best_i]             # <<<<<<<<<<<<<<
- *     precision[0] = vops.max(xs) - vops.min(xs)
+ *     precision[0] = vops.max(x0s) - vops.min(x0s)
  *     optimal[0] = sops.isclose(0, error[0], ertol, etol)
  */
   __pyx_t_8 = __pyx_v_best_i;
   (__pyx_v_error[0]) = (*((double *) ( /* dim=0 */ (__pyx_v_errors.data + __pyx_t_8 * __pyx_v_errors.strides[0]) )));
 
   /* "cyroot/_check_args.pyx":205
- *     r[0], f_r[0] = xs[best_i], f_xs[best_i]
+ *     r[0], f_r[0] = x0s[best_i], f_x0s[best_i]
  *     error[0] = errors[best_i]
- *     precision[0] = vops.max(xs) - vops.min(xs)             # <<<<<<<<<<<<<<
+ *     precision[0] = vops.max(x0s) - vops.min(x0s)             # <<<<<<<<<<<<<<
  *     optimal[0] = sops.isclose(0, error[0], ertol, etol)
  *     converged[0] = sops.isclose(0, precision[0], prtol, ptol) or optimal[0]
  */
-  (__pyx_v_precision[0]) = (__pyx_f_6cyroot_3ops_10vector_ops_max(__pyx_v_xs) - __pyx_f_6cyroot_3ops_10vector_ops_min(__pyx_v_xs));
+  (__pyx_v_precision[0]) = (__pyx_f_6cyroot_3ops_10vector_ops_max(__pyx_v_x0s) - __pyx_f_6cyroot_3ops_10vector_ops_min(__pyx_v_x0s));
 
   /* "cyroot/_check_args.pyx":206
  *     error[0] = errors[best_i]
- *     precision[0] = vops.max(xs) - vops.min(xs)
+ *     precision[0] = vops.max(x0s) - vops.min(x0s)
  *     optimal[0] = sops.isclose(0, error[0], ertol, etol)             # <<<<<<<<<<<<<<
  *     converged[0] = sops.isclose(0, precision[0], prtol, ptol) or optimal[0]
  *     return optimal[0] or sops.isclose(0, precision[0], prtol, ptol)
  */
   __pyx_t_6.__pyx_n = 2;
   __pyx_t_6.rtol = __pyx_v_ertol;
   __pyx_t_6.atol = __pyx_v_etol;
   __pyx_t_1 = __pyx_f_6cyroot_3ops_10scalar_ops_isclose(0.0, (__pyx_v_error[0]), &__pyx_t_6); 
   (__pyx_v_optimal[0]) = __pyx_t_1;
 
   /* "cyroot/_check_args.pyx":207
- *     precision[0] = vops.max(xs) - vops.min(xs)
+ *     precision[0] = vops.max(x0s) - vops.min(x0s)
  *     optimal[0] = sops.isclose(0, error[0], ertol, etol)
  *     converged[0] = sops.isclose(0, precision[0], prtol, ptol) or optimal[0]             # <<<<<<<<<<<<<<
  *     return optimal[0] or sops.isclose(0, precision[0], prtol, ptol)
  * 
  */
   __pyx_t_6.__pyx_n = 2;
   __pyx_t_6.rtol = __pyx_v_prtol;
@@ -6029,16 +6029,16 @@
   __pyx_r = __pyx_t_1;
   goto __pyx_L0;
 
   /* "cyroot/_check_args.pyx":178
  * 
  * # noinspection DuplicatedCode
  * cdef inline bint _check_stop_cond_scalar_initial_guesses(             # <<<<<<<<<<<<<<
- *         double[:] xs,
- *         double[:] f_xs,
+ *         double[:] x0s,
+ *         double[:] f_x0s,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __PYX_XDEC_MEMVIEW(&__pyx_t_7, 1);
   __Pyx_WriteUnraisable("cyroot._check_args._check_stop_cond_scalar_initial_guesses", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
@@ -6049,19 +6049,19 @@
   return __pyx_r;
 }
 
 /* "cyroot/_check_args.pyx":211
  * 
  * # noinspection DuplicatedCode
  * cdef inline bint _check_stop_cond_vector_initial_guesses(             # <<<<<<<<<<<<<<
- *         double[:, :] xs,
- *         double[:, :] F_xs,
+ *         double[:, :] x0s,
+ *         double[:, :] F_x0s,
  */
 
-static CYTHON_INLINE int __pyx_f_6cyroot_11_check_args__check_stop_cond_vector_initial_guesses(__Pyx_memviewslice __pyx_v_xs, __Pyx_memviewslice __pyx_v_F_xs, double __pyx_v_etol, double __pyx_v_ertol, double __pyx_v_ptol, double __pyx_v_prtol, __Pyx_memviewslice __pyx_v_r, __Pyx_memviewslice __pyx_v_F_r, double *__pyx_v_precision, double *__pyx_v_error, int *__pyx_v_converged, int *__pyx_v_optimal) {
+static CYTHON_INLINE int __pyx_f_6cyroot_11_check_args__check_stop_cond_vector_initial_guesses(__Pyx_memviewslice __pyx_v_x0s, __Pyx_memviewslice __pyx_v_F_x0s, double __pyx_v_etol, double __pyx_v_ertol, double __pyx_v_ptol, double __pyx_v_prtol, __Pyx_memviewslice __pyx_v_r, __Pyx_memviewslice __pyx_v_F_r, double *__pyx_v_precision, double *__pyx_v_error, int *__pyx_v_converged, int *__pyx_v_optimal) {
   __Pyx_memviewslice __pyx_v_errors = { 0, 0, { 0 }, { 0 }, { 0 } };
   unsigned long __pyx_v_best_i;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   __Pyx_memviewslice __pyx_t_3 = { 0, 0, { 0 }, { 0 }, { 0 } };
@@ -6080,196 +6080,196 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_check_stop_cond_vector_initial_guesses", 0);
 
   /* "cyroot/_check_args.pyx":225
  *         bint* optimal):
  *     """Check if stop condition is already met."""
- *     if xs.shape[0] == 0:             # <<<<<<<<<<<<<<
+ *     if x0s.shape[0] == 0:             # <<<<<<<<<<<<<<
  *         raise ValueError('Empty sequence.')
- *     if xs.shape[0] == 1:
+ *     if x0s.shape[0] == 1:
  */
-  __pyx_t_1 = (((__pyx_v_xs.shape[0]) == 0) != 0);
+  __pyx_t_1 = (((__pyx_v_x0s.shape[0]) == 0) != 0);
   if (unlikely(__pyx_t_1)) {
 
     /* "cyroot/_check_args.pyx":226
  *     """Check if stop condition is already met."""
- *     if xs.shape[0] == 0:
+ *     if x0s.shape[0] == 0:
  *         raise ValueError('Empty sequence.')             # <<<<<<<<<<<<<<
- *     if xs.shape[0] == 1:
- *         r[:], F_r[:] = xs[0], F_xs[0]
+ *     if x0s.shape[0] == 1:
+ *         r[:], F_r[:] = x0s[0], F_x0s[0]
  */
     __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 226, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(0, 226, __pyx_L1_error)
 
     /* "cyroot/_check_args.pyx":225
  *         bint* optimal):
  *     """Check if stop condition is already met."""
- *     if xs.shape[0] == 0:             # <<<<<<<<<<<<<<
+ *     if x0s.shape[0] == 0:             # <<<<<<<<<<<<<<
  *         raise ValueError('Empty sequence.')
- *     if xs.shape[0] == 1:
+ *     if x0s.shape[0] == 1:
  */
   }
 
   /* "cyroot/_check_args.pyx":227
- *     if xs.shape[0] == 0:
+ *     if x0s.shape[0] == 0:
  *         raise ValueError('Empty sequence.')
- *     if xs.shape[0] == 1:             # <<<<<<<<<<<<<<
- *         r[:], F_r[:] = xs[0], F_xs[0]
+ *     if x0s.shape[0] == 1:             # <<<<<<<<<<<<<<
+ *         r[:], F_r[:] = x0s[0], F_x0s[0]
  *         precision[0] = math.INFINITY
  */
-  __pyx_t_1 = (((__pyx_v_xs.shape[0]) == 1) != 0);
+  __pyx_t_1 = (((__pyx_v_x0s.shape[0]) == 1) != 0);
   if (__pyx_t_1) {
 
     /* "cyroot/_check_args.pyx":228
  *         raise ValueError('Empty sequence.')
- *     if xs.shape[0] == 1:
- *         r[:], F_r[:] = xs[0], F_xs[0]             # <<<<<<<<<<<<<<
+ *     if x0s.shape[0] == 1:
+ *         r[:], F_r[:] = x0s[0], F_x0s[0]             # <<<<<<<<<<<<<<
  *         precision[0] = math.INFINITY
- *         error[0] = vops.max(vops.fabs(F_xs[0]))
+ *         error[0] = vops.max(vops.fabs(F_x0s[0]))
  */
-    __pyx_t_3.data = __pyx_v_xs.data;
-    __pyx_t_3.memview = __pyx_v_xs.memview;
+    __pyx_t_3.data = __pyx_v_x0s.data;
+    __pyx_t_3.memview = __pyx_v_x0s.memview;
     __PYX_INC_MEMVIEW(&__pyx_t_3, 0);
     {
     Py_ssize_t __pyx_tmp_idx = 0;
-        Py_ssize_t __pyx_tmp_shape = __pyx_v_xs.shape[0];
-    Py_ssize_t __pyx_tmp_stride = __pyx_v_xs.strides[0];
+        Py_ssize_t __pyx_tmp_shape = __pyx_v_x0s.shape[0];
+    Py_ssize_t __pyx_tmp_stride = __pyx_v_x0s.strides[0];
         if (__pyx_tmp_idx < 0)
             __pyx_tmp_idx += __pyx_tmp_shape;
         __pyx_t_3.data += __pyx_tmp_idx * __pyx_tmp_stride;
 }
 
-__pyx_t_3.shape[0] = __pyx_v_xs.shape[1];
-__pyx_t_3.strides[0] = __pyx_v_xs.strides[1];
+__pyx_t_3.shape[0] = __pyx_v_x0s.shape[1];
+__pyx_t_3.strides[0] = __pyx_v_x0s.strides[1];
     __pyx_t_3.suboffsets[0] = -1;
 
-__pyx_t_4.data = __pyx_v_F_xs.data;
-    __pyx_t_4.memview = __pyx_v_F_xs.memview;
+__pyx_t_4.data = __pyx_v_F_x0s.data;
+    __pyx_t_4.memview = __pyx_v_F_x0s.memview;
     __PYX_INC_MEMVIEW(&__pyx_t_4, 0);
     {
     Py_ssize_t __pyx_tmp_idx = 0;
-        Py_ssize_t __pyx_tmp_shape = __pyx_v_F_xs.shape[0];
-    Py_ssize_t __pyx_tmp_stride = __pyx_v_F_xs.strides[0];
+        Py_ssize_t __pyx_tmp_shape = __pyx_v_F_x0s.shape[0];
+    Py_ssize_t __pyx_tmp_stride = __pyx_v_F_x0s.strides[0];
         if (__pyx_tmp_idx < 0)
             __pyx_tmp_idx += __pyx_tmp_shape;
         __pyx_t_4.data += __pyx_tmp_idx * __pyx_tmp_stride;
 }
 
-__pyx_t_4.shape[0] = __pyx_v_F_xs.shape[1];
-__pyx_t_4.strides[0] = __pyx_v_F_xs.strides[1];
+__pyx_t_4.shape[0] = __pyx_v_F_x0s.shape[1];
+__pyx_t_4.strides[0] = __pyx_v_F_x0s.strides[1];
     __pyx_t_4.suboffsets[0] = -1;
 
 if (unlikely(__pyx_memoryview_copy_contents(__pyx_t_3, __pyx_v_r, 1, 1, 0) < 0)) __PYX_ERR(0, 228, __pyx_L1_error)
     __PYX_XDEC_MEMVIEW(&__pyx_t_3, 1);
     __pyx_t_3.memview = NULL;
     __pyx_t_3.data = NULL;
     if (unlikely(__pyx_memoryview_copy_contents(__pyx_t_4, __pyx_v_F_r, 1, 1, 0) < 0)) __PYX_ERR(0, 228, __pyx_L1_error)
     __PYX_XDEC_MEMVIEW(&__pyx_t_4, 1);
     __pyx_t_4.memview = NULL;
     __pyx_t_4.data = NULL;
 
     /* "cyroot/_check_args.pyx":229
- *     if xs.shape[0] == 1:
- *         r[:], F_r[:] = xs[0], F_xs[0]
+ *     if x0s.shape[0] == 1:
+ *         r[:], F_r[:] = x0s[0], F_x0s[0]
  *         precision[0] = math.INFINITY             # <<<<<<<<<<<<<<
- *         error[0] = vops.max(vops.fabs(F_xs[0]))
+ *         error[0] = vops.max(vops.fabs(F_x0s[0]))
  *         optimal[0] = sops.isclose(0, error[0], ertol, etol)
  */
     (__pyx_v_precision[0]) = INFINITY;
 
     /* "cyroot/_check_args.pyx":230
- *         r[:], F_r[:] = xs[0], F_xs[0]
+ *         r[:], F_r[:] = x0s[0], F_x0s[0]
  *         precision[0] = math.INFINITY
- *         error[0] = vops.max(vops.fabs(F_xs[0]))             # <<<<<<<<<<<<<<
+ *         error[0] = vops.max(vops.fabs(F_x0s[0]))             # <<<<<<<<<<<<<<
  *         optimal[0] = sops.isclose(0, error[0], ertol, etol)
  *         converged[0] = optimal[0]
  */
-    __pyx_t_4.data = __pyx_v_F_xs.data;
-    __pyx_t_4.memview = __pyx_v_F_xs.memview;
+    __pyx_t_4.data = __pyx_v_F_x0s.data;
+    __pyx_t_4.memview = __pyx_v_F_x0s.memview;
     __PYX_INC_MEMVIEW(&__pyx_t_4, 0);
     {
     Py_ssize_t __pyx_tmp_idx = 0;
-        Py_ssize_t __pyx_tmp_shape = __pyx_v_F_xs.shape[0];
-    Py_ssize_t __pyx_tmp_stride = __pyx_v_F_xs.strides[0];
+        Py_ssize_t __pyx_tmp_shape = __pyx_v_F_x0s.shape[0];
+    Py_ssize_t __pyx_tmp_stride = __pyx_v_F_x0s.strides[0];
         if (__pyx_tmp_idx < 0)
             __pyx_tmp_idx += __pyx_tmp_shape;
         __pyx_t_4.data += __pyx_tmp_idx * __pyx_tmp_stride;
 }
 
-__pyx_t_4.shape[0] = __pyx_v_F_xs.shape[1];
-__pyx_t_4.strides[0] = __pyx_v_F_xs.strides[1];
+__pyx_t_4.shape[0] = __pyx_v_F_x0s.shape[1];
+__pyx_t_4.strides[0] = __pyx_v_F_x0s.strides[1];
     __pyx_t_4.suboffsets[0] = -1;
 
 __pyx_t_3 = __pyx_f_6cyroot_3ops_10vector_ops_fabs(__pyx_t_4); if (unlikely(!__pyx_t_3.memview)) __PYX_ERR(0, 230, __pyx_L1_error)
     __PYX_XDEC_MEMVIEW(&__pyx_t_4, 1);
     __pyx_t_4.memview = NULL;
     __pyx_t_4.data = NULL;
     (__pyx_v_error[0]) = __pyx_f_6cyroot_3ops_10vector_ops_max(__pyx_t_3);
     __PYX_XDEC_MEMVIEW(&__pyx_t_3, 1);
     __pyx_t_3.memview = NULL;
     __pyx_t_3.data = NULL;
 
     /* "cyroot/_check_args.pyx":231
  *         precision[0] = math.INFINITY
- *         error[0] = vops.max(vops.fabs(F_xs[0]))
+ *         error[0] = vops.max(vops.fabs(F_x0s[0]))
  *         optimal[0] = sops.isclose(0, error[0], ertol, etol)             # <<<<<<<<<<<<<<
  *         converged[0] = optimal[0]
  *         return optimal[0]
  */
     __pyx_t_5.__pyx_n = 2;
     __pyx_t_5.rtol = __pyx_v_ertol;
     __pyx_t_5.atol = __pyx_v_etol;
     __pyx_t_1 = __pyx_f_6cyroot_3ops_10scalar_ops_isclose(0.0, (__pyx_v_error[0]), &__pyx_t_5); 
     (__pyx_v_optimal[0]) = __pyx_t_1;
 
     /* "cyroot/_check_args.pyx":232
- *         error[0] = vops.max(vops.fabs(F_xs[0]))
+ *         error[0] = vops.max(vops.fabs(F_x0s[0]))
  *         optimal[0] = sops.isclose(0, error[0], ertol, etol)
  *         converged[0] = optimal[0]             # <<<<<<<<<<<<<<
  *         return optimal[0]
- *     cdef double[:] errors = np.abs(F_xs).max(1)
+ *     cdef double[:] errors = np.abs(F_x0s).max(1)
  */
     (__pyx_v_converged[0]) = (__pyx_v_optimal[0]);
 
     /* "cyroot/_check_args.pyx":233
  *         optimal[0] = sops.isclose(0, error[0], ertol, etol)
  *         converged[0] = optimal[0]
  *         return optimal[0]             # <<<<<<<<<<<<<<
- *     cdef double[:] errors = np.abs(F_xs).max(1)
+ *     cdef double[:] errors = np.abs(F_x0s).max(1)
  *     cdef unsigned long best_i = vops.argmin(errors)
  */
     __pyx_r = (__pyx_v_optimal[0]);
     goto __pyx_L0;
 
     /* "cyroot/_check_args.pyx":227
- *     if xs.shape[0] == 0:
+ *     if x0s.shape[0] == 0:
  *         raise ValueError('Empty sequence.')
- *     if xs.shape[0] == 1:             # <<<<<<<<<<<<<<
- *         r[:], F_r[:] = xs[0], F_xs[0]
+ *     if x0s.shape[0] == 1:             # <<<<<<<<<<<<<<
+ *         r[:], F_r[:] = x0s[0], F_x0s[0]
  *         precision[0] = math.INFINITY
  */
   }
 
   /* "cyroot/_check_args.pyx":234
  *         converged[0] = optimal[0]
  *         return optimal[0]
- *     cdef double[:] errors = np.abs(F_xs).max(1)             # <<<<<<<<<<<<<<
+ *     cdef double[:] errors = np.abs(F_x0s).max(1)             # <<<<<<<<<<<<<<
  *     cdef unsigned long best_i = vops.argmin(errors)
- *     r[:], F_r[:] = xs[best_i], F_xs[best_i]
+ *     r[:], F_r[:] = x0s[best_i], F_x0s[best_i]
  */
   __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 234, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_abs); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 234, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __pyx_memoryview_fromslice(__pyx_v_F_xs, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 234, __pyx_L1_error)
+  __pyx_t_7 = __pyx_memoryview_fromslice(__pyx_v_F_x0s, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 234, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_t_9 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
     __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
     if (likely(__pyx_t_9)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
       __Pyx_INCREF(__pyx_t_9);
@@ -6305,92 +6305,92 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_errors = __pyx_t_3;
   __pyx_t_3.memview = NULL;
   __pyx_t_3.data = NULL;
 
   /* "cyroot/_check_args.pyx":235
  *         return optimal[0]
- *     cdef double[:] errors = np.abs(F_xs).max(1)
+ *     cdef double[:] errors = np.abs(F_x0s).max(1)
  *     cdef unsigned long best_i = vops.argmin(errors)             # <<<<<<<<<<<<<<
- *     r[:], F_r[:] = xs[best_i], F_xs[best_i]
+ *     r[:], F_r[:] = x0s[best_i], F_x0s[best_i]
  *     error[0] = errors[best_i]
  */
   __pyx_v_best_i = __pyx_f_6cyroot_3ops_10vector_ops_argmin(__pyx_v_errors);
 
   /* "cyroot/_check_args.pyx":236
- *     cdef double[:] errors = np.abs(F_xs).max(1)
+ *     cdef double[:] errors = np.abs(F_x0s).max(1)
  *     cdef unsigned long best_i = vops.argmin(errors)
- *     r[:], F_r[:] = xs[best_i], F_xs[best_i]             # <<<<<<<<<<<<<<
+ *     r[:], F_r[:] = x0s[best_i], F_x0s[best_i]             # <<<<<<<<<<<<<<
  *     error[0] = errors[best_i]
- *     precision[0] = vops.max(np.max(xs, 0) - np.min(xs, 0))
+ *     precision[0] = vops.max(np.max(x0s, 0) - np.min(x0s, 0))
  */
-  __pyx_t_3.data = __pyx_v_xs.data;
-  __pyx_t_3.memview = __pyx_v_xs.memview;
+  __pyx_t_3.data = __pyx_v_x0s.data;
+  __pyx_t_3.memview = __pyx_v_x0s.memview;
   __PYX_INC_MEMVIEW(&__pyx_t_3, 0);
   {
     Py_ssize_t __pyx_tmp_idx = __pyx_v_best_i;
-        Py_ssize_t __pyx_tmp_shape = __pyx_v_xs.shape[0];
-    Py_ssize_t __pyx_tmp_stride = __pyx_v_xs.strides[0];
+        Py_ssize_t __pyx_tmp_shape = __pyx_v_x0s.shape[0];
+    Py_ssize_t __pyx_tmp_stride = __pyx_v_x0s.strides[0];
         if (__pyx_tmp_idx < 0)
             __pyx_tmp_idx += __pyx_tmp_shape;
         __pyx_t_3.data += __pyx_tmp_idx * __pyx_tmp_stride;
 }
 
-__pyx_t_3.shape[0] = __pyx_v_xs.shape[1];
-__pyx_t_3.strides[0] = __pyx_v_xs.strides[1];
+__pyx_t_3.shape[0] = __pyx_v_x0s.shape[1];
+__pyx_t_3.strides[0] = __pyx_v_x0s.strides[1];
     __pyx_t_3.suboffsets[0] = -1;
 
-__pyx_t_4.data = __pyx_v_F_xs.data;
-  __pyx_t_4.memview = __pyx_v_F_xs.memview;
+__pyx_t_4.data = __pyx_v_F_x0s.data;
+  __pyx_t_4.memview = __pyx_v_F_x0s.memview;
   __PYX_INC_MEMVIEW(&__pyx_t_4, 0);
   {
     Py_ssize_t __pyx_tmp_idx = __pyx_v_best_i;
-        Py_ssize_t __pyx_tmp_shape = __pyx_v_F_xs.shape[0];
-    Py_ssize_t __pyx_tmp_stride = __pyx_v_F_xs.strides[0];
+        Py_ssize_t __pyx_tmp_shape = __pyx_v_F_x0s.shape[0];
+    Py_ssize_t __pyx_tmp_stride = __pyx_v_F_x0s.strides[0];
         if (__pyx_tmp_idx < 0)
             __pyx_tmp_idx += __pyx_tmp_shape;
         __pyx_t_4.data += __pyx_tmp_idx * __pyx_tmp_stride;
 }
 
-__pyx_t_4.shape[0] = __pyx_v_F_xs.shape[1];
-__pyx_t_4.strides[0] = __pyx_v_F_xs.strides[1];
+__pyx_t_4.shape[0] = __pyx_v_F_x0s.shape[1];
+__pyx_t_4.strides[0] = __pyx_v_F_x0s.strides[1];
     __pyx_t_4.suboffsets[0] = -1;
 
 if (unlikely(__pyx_memoryview_copy_contents(__pyx_t_3, __pyx_v_r, 1, 1, 0) < 0)) __PYX_ERR(0, 236, __pyx_L1_error)
   __PYX_XDEC_MEMVIEW(&__pyx_t_3, 1);
   __pyx_t_3.memview = NULL;
   __pyx_t_3.data = NULL;
   if (unlikely(__pyx_memoryview_copy_contents(__pyx_t_4, __pyx_v_F_r, 1, 1, 0) < 0)) __PYX_ERR(0, 236, __pyx_L1_error)
   __PYX_XDEC_MEMVIEW(&__pyx_t_4, 1);
   __pyx_t_4.memview = NULL;
   __pyx_t_4.data = NULL;
 
   /* "cyroot/_check_args.pyx":237
  *     cdef unsigned long best_i = vops.argmin(errors)
- *     r[:], F_r[:] = xs[best_i], F_xs[best_i]
+ *     r[:], F_r[:] = x0s[best_i], F_x0s[best_i]
  *     error[0] = errors[best_i]             # <<<<<<<<<<<<<<
- *     precision[0] = vops.max(np.max(xs, 0) - np.min(xs, 0))
+ *     precision[0] = vops.max(np.max(x0s, 0) - np.min(x0s, 0))
  *     optimal[0] = sops.isclose(0, error[0], ertol, etol)
  */
   __pyx_t_10 = __pyx_v_best_i;
   (__pyx_v_error[0]) = (*((double *) ( /* dim=0 */ (__pyx_v_errors.data + __pyx_t_10 * __pyx_v_errors.strides[0]) )));
 
   /* "cyroot/_check_args.pyx":238
- *     r[:], F_r[:] = xs[best_i], F_xs[best_i]
+ *     r[:], F_r[:] = x0s[best_i], F_x0s[best_i]
  *     error[0] = errors[best_i]
- *     precision[0] = vops.max(np.max(xs, 0) - np.min(xs, 0))             # <<<<<<<<<<<<<<
+ *     precision[0] = vops.max(np.max(x0s, 0) - np.min(x0s, 0))             # <<<<<<<<<<<<<<
  *     optimal[0] = sops.isclose(0, error[0], ertol, etol)
  *     converged[0] = sops.isclose(0, precision[0], prtol, ptol) or optimal[0]
  */
   __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_max); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __pyx_memoryview_fromslice(__pyx_v_xs, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 238, __pyx_L1_error)
+  __pyx_t_8 = __pyx_memoryview_fromslice(__pyx_v_x0s, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __pyx_t_7 = NULL;
   __pyx_t_11 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -6436,15 +6436,15 @@
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_min); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  __pyx_t_9 = __pyx_memoryview_fromslice(__pyx_v_xs, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 238, __pyx_L1_error)
+  __pyx_t_9 = __pyx_memoryview_fromslice(__pyx_v_x0s, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __pyx_t_7 = NULL;
   __pyx_t_11 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_8);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
@@ -6498,27 +6498,27 @@
   (__pyx_v_precision[0]) = __pyx_f_6cyroot_3ops_10vector_ops_max(__pyx_t_4);
   __PYX_XDEC_MEMVIEW(&__pyx_t_4, 1);
   __pyx_t_4.memview = NULL;
   __pyx_t_4.data = NULL;
 
   /* "cyroot/_check_args.pyx":239
  *     error[0] = errors[best_i]
- *     precision[0] = vops.max(np.max(xs, 0) - np.min(xs, 0))
+ *     precision[0] = vops.max(np.max(x0s, 0) - np.min(x0s, 0))
  *     optimal[0] = sops.isclose(0, error[0], ertol, etol)             # <<<<<<<<<<<<<<
  *     converged[0] = sops.isclose(0, precision[0], prtol, ptol) or optimal[0]
  *     return optimal[0] or sops.isclose(0, precision[0], prtol, ptol)
  */
   __pyx_t_5.__pyx_n = 2;
   __pyx_t_5.rtol = __pyx_v_ertol;
   __pyx_t_5.atol = __pyx_v_etol;
   __pyx_t_1 = __pyx_f_6cyroot_3ops_10scalar_ops_isclose(0.0, (__pyx_v_error[0]), &__pyx_t_5); 
   (__pyx_v_optimal[0]) = __pyx_t_1;
 
   /* "cyroot/_check_args.pyx":240
- *     precision[0] = vops.max(np.max(xs, 0) - np.min(xs, 0))
+ *     precision[0] = vops.max(np.max(x0s, 0) - np.min(x0s, 0))
  *     optimal[0] = sops.isclose(0, error[0], ertol, etol)
  *     converged[0] = sops.isclose(0, precision[0], prtol, ptol) or optimal[0]             # <<<<<<<<<<<<<<
  *     return optimal[0] or sops.isclose(0, precision[0], prtol, ptol)
  * 
  */
   __pyx_t_5.__pyx_n = 2;
   __pyx_t_5.rtol = __pyx_v_prtol;
@@ -6558,16 +6558,16 @@
   __pyx_r = __pyx_t_1;
   goto __pyx_L0;
 
   /* "cyroot/_check_args.pyx":211
  * 
  * # noinspection DuplicatedCode
  * cdef inline bint _check_stop_cond_vector_initial_guesses(             # <<<<<<<<<<<<<<
- *         double[:, :] xs,
- *         double[:, :] F_xs,
+ *         double[:, :] x0s,
+ *         double[:, :] F_x0s,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __PYX_XDEC_MEMVIEW(&__pyx_t_3, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_t_4, 1);
@@ -6754,19 +6754,19 @@
   return __pyx_r;
 }
 
 /* "cyroot/_check_args.pyx":285
  * 
  * # noinspection DuplicatedCode
  * cdef inline bint _check_stop_cond_complex_scalar_initial_guesses(             # <<<<<<<<<<<<<<
- *         double complex[:] xs,
- *         double complex[:] f_xs,
+ *         double complex[:] x0s,
+ *         double complex[:] f_x0s,
  */
 
-static CYTHON_INLINE int __pyx_f_6cyroot_11_check_args__check_stop_cond_complex_scalar_initial_guesses(__Pyx_memviewslice __pyx_v_xs, __Pyx_memviewslice __pyx_v_f_xs, double __pyx_v_etol, double __pyx_v_ertol, double __pyx_v_ptol, double __pyx_v_prtol, __pyx_t_double_complex *__pyx_v_r, __pyx_t_double_complex *__pyx_v_f_r, double *__pyx_v_precision, double *__pyx_v_error, int *__pyx_v_converged, int *__pyx_v_optimal) {
+static CYTHON_INLINE int __pyx_f_6cyroot_11_check_args__check_stop_cond_complex_scalar_initial_guesses(__Pyx_memviewslice __pyx_v_x0s, __Pyx_memviewslice __pyx_v_f_x0s, double __pyx_v_etol, double __pyx_v_ertol, double __pyx_v_ptol, double __pyx_v_prtol, __pyx_t_double_complex *__pyx_v_r, __pyx_t_double_complex *__pyx_v_f_r, double *__pyx_v_precision, double *__pyx_v_error, int *__pyx_v_converged, int *__pyx_v_optimal) {
   __Pyx_memviewslice __pyx_v_errors = { 0, 0, { 0 }, { 0 }, { 0 } };
   unsigned long __pyx_v_best_i;
   __Pyx_memviewslice __pyx_v_xs_abs = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
@@ -6782,198 +6782,198 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_check_stop_cond_complex_scalar_initial_guesses", 0);
 
   /* "cyroot/_check_args.pyx":299
  *         bint* optimal):
  *     """Check if stop condition is already met."""
- *     if xs.shape[0] == 0:             # <<<<<<<<<<<<<<
+ *     if x0s.shape[0] == 0:             # <<<<<<<<<<<<<<
  *         raise ValueError('Empty sequence.')
- *     if xs.shape[0] == 1:
+ *     if x0s.shape[0] == 1:
  */
-  __pyx_t_1 = (((__pyx_v_xs.shape[0]) == 0) != 0);
+  __pyx_t_1 = (((__pyx_v_x0s.shape[0]) == 0) != 0);
   if (unlikely(__pyx_t_1)) {
 
     /* "cyroot/_check_args.pyx":300
  *     """Check if stop condition is already met."""
- *     if xs.shape[0] == 0:
+ *     if x0s.shape[0] == 0:
  *         raise ValueError('Empty sequence.')             # <<<<<<<<<<<<<<
- *     if xs.shape[0] == 1:
- *         r[0], f_r[0] = xs[0], f_xs[0]
+ *     if x0s.shape[0] == 1:
+ *         r[0], f_r[0] = x0s[0], f_x0s[0]
  */
     __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 300, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(0, 300, __pyx_L1_error)
 
     /* "cyroot/_check_args.pyx":299
  *         bint* optimal):
  *     """Check if stop condition is already met."""
- *     if xs.shape[0] == 0:             # <<<<<<<<<<<<<<
+ *     if x0s.shape[0] == 0:             # <<<<<<<<<<<<<<
  *         raise ValueError('Empty sequence.')
- *     if xs.shape[0] == 1:
+ *     if x0s.shape[0] == 1:
  */
   }
 
   /* "cyroot/_check_args.pyx":301
- *     if xs.shape[0] == 0:
+ *     if x0s.shape[0] == 0:
  *         raise ValueError('Empty sequence.')
- *     if xs.shape[0] == 1:             # <<<<<<<<<<<<<<
- *         r[0], f_r[0] = xs[0], f_xs[0]
+ *     if x0s.shape[0] == 1:             # <<<<<<<<<<<<<<
+ *         r[0], f_r[0] = x0s[0], f_x0s[0]
  *         precision[0] = math.INFINITY
  */
-  __pyx_t_1 = (((__pyx_v_xs.shape[0]) == 1) != 0);
+  __pyx_t_1 = (((__pyx_v_x0s.shape[0]) == 1) != 0);
   if (__pyx_t_1) {
 
     /* "cyroot/_check_args.pyx":302
  *         raise ValueError('Empty sequence.')
- *     if xs.shape[0] == 1:
- *         r[0], f_r[0] = xs[0], f_xs[0]             # <<<<<<<<<<<<<<
+ *     if x0s.shape[0] == 1:
+ *         r[0], f_r[0] = x0s[0], f_x0s[0]             # <<<<<<<<<<<<<<
  *         precision[0] = math.INFINITY
- *         error[0] = sops.cabs(f_xs[0])
+ *         error[0] = sops.cabs(f_x0s[0])
  */
     __pyx_t_3 = 0;
-    if (__pyx_t_3 < 0) __pyx_t_3 += __pyx_v_xs.shape[0];
-    __pyx_t_4 = (*((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_xs.data + __pyx_t_3 * __pyx_v_xs.strides[0]) )));
+    if (__pyx_t_3 < 0) __pyx_t_3 += __pyx_v_x0s.shape[0];
+    __pyx_t_4 = (*((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_x0s.data + __pyx_t_3 * __pyx_v_x0s.strides[0]) )));
     __pyx_t_3 = 0;
-    if (__pyx_t_3 < 0) __pyx_t_3 += __pyx_v_f_xs.shape[0];
-    __pyx_t_5 = (*((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_f_xs.data + __pyx_t_3 * __pyx_v_f_xs.strides[0]) )));
+    if (__pyx_t_3 < 0) __pyx_t_3 += __pyx_v_f_x0s.shape[0];
+    __pyx_t_5 = (*((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_f_x0s.data + __pyx_t_3 * __pyx_v_f_x0s.strides[0]) )));
     (__pyx_v_r[0]) = __pyx_t_4;
     (__pyx_v_f_r[0]) = __pyx_t_5;
 
     /* "cyroot/_check_args.pyx":303
- *     if xs.shape[0] == 1:
- *         r[0], f_r[0] = xs[0], f_xs[0]
+ *     if x0s.shape[0] == 1:
+ *         r[0], f_r[0] = x0s[0], f_x0s[0]
  *         precision[0] = math.INFINITY             # <<<<<<<<<<<<<<
- *         error[0] = sops.cabs(f_xs[0])
+ *         error[0] = sops.cabs(f_x0s[0])
  *         optimal[0] = sops.isclose(0, error[0], ertol, etol)
  */
     (__pyx_v_precision[0]) = INFINITY;
 
     /* "cyroot/_check_args.pyx":304
- *         r[0], f_r[0] = xs[0], f_xs[0]
+ *         r[0], f_r[0] = x0s[0], f_x0s[0]
  *         precision[0] = math.INFINITY
- *         error[0] = sops.cabs(f_xs[0])             # <<<<<<<<<<<<<<
+ *         error[0] = sops.cabs(f_x0s[0])             # <<<<<<<<<<<<<<
  *         optimal[0] = sops.isclose(0, error[0], ertol, etol)
  *         converged[0] = optimal[0]
  */
     __pyx_t_3 = 0;
-    if (__pyx_t_3 < 0) __pyx_t_3 += __pyx_v_f_xs.shape[0];
-    (__pyx_v_error[0]) = abs((*((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_f_xs.data + __pyx_t_3 * __pyx_v_f_xs.strides[0]) ))));
+    if (__pyx_t_3 < 0) __pyx_t_3 += __pyx_v_f_x0s.shape[0];
+    (__pyx_v_error[0]) = abs((*((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_f_x0s.data + __pyx_t_3 * __pyx_v_f_x0s.strides[0]) ))));
 
     /* "cyroot/_check_args.pyx":305
  *         precision[0] = math.INFINITY
- *         error[0] = sops.cabs(f_xs[0])
+ *         error[0] = sops.cabs(f_x0s[0])
  *         optimal[0] = sops.isclose(0, error[0], ertol, etol)             # <<<<<<<<<<<<<<
  *         converged[0] = optimal[0]
  *         return optimal[0]
  */
     __pyx_t_6.__pyx_n = 2;
     __pyx_t_6.rtol = __pyx_v_ertol;
     __pyx_t_6.atol = __pyx_v_etol;
     __pyx_t_1 = __pyx_f_6cyroot_3ops_10scalar_ops_isclose(0.0, (__pyx_v_error[0]), &__pyx_t_6); 
     (__pyx_v_optimal[0]) = __pyx_t_1;
 
     /* "cyroot/_check_args.pyx":306
- *         error[0] = sops.cabs(f_xs[0])
+ *         error[0] = sops.cabs(f_x0s[0])
  *         optimal[0] = sops.isclose(0, error[0], ertol, etol)
  *         converged[0] = optimal[0]             # <<<<<<<<<<<<<<
  *         return optimal[0]
- *     cdef double[:] errors = vops.cabs(f_xs)
+ *     cdef double[:] errors = vops.cabs(f_x0s)
  */
     (__pyx_v_converged[0]) = (__pyx_v_optimal[0]);
 
     /* "cyroot/_check_args.pyx":307
  *         optimal[0] = sops.isclose(0, error[0], ertol, etol)
  *         converged[0] = optimal[0]
  *         return optimal[0]             # <<<<<<<<<<<<<<
- *     cdef double[:] errors = vops.cabs(f_xs)
+ *     cdef double[:] errors = vops.cabs(f_x0s)
  *     cdef unsigned long best_i = vops.argmin(errors)
  */
     __pyx_r = (__pyx_v_optimal[0]);
     goto __pyx_L0;
 
     /* "cyroot/_check_args.pyx":301
- *     if xs.shape[0] == 0:
+ *     if x0s.shape[0] == 0:
  *         raise ValueError('Empty sequence.')
- *     if xs.shape[0] == 1:             # <<<<<<<<<<<<<<
- *         r[0], f_r[0] = xs[0], f_xs[0]
+ *     if x0s.shape[0] == 1:             # <<<<<<<<<<<<<<
+ *         r[0], f_r[0] = x0s[0], f_x0s[0]
  *         precision[0] = math.INFINITY
  */
   }
 
   /* "cyroot/_check_args.pyx":308
  *         converged[0] = optimal[0]
  *         return optimal[0]
- *     cdef double[:] errors = vops.cabs(f_xs)             # <<<<<<<<<<<<<<
+ *     cdef double[:] errors = vops.cabs(f_x0s)             # <<<<<<<<<<<<<<
  *     cdef unsigned long best_i = vops.argmin(errors)
- *     r[0], f_r[0] = xs[best_i], f_xs[best_i]
+ *     r[0], f_r[0] = x0s[best_i], f_x0s[best_i]
  */
-  __pyx_t_7 = __pyx_f_6cyroot_3ops_10vector_ops_cabs(__pyx_v_f_xs); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 308, __pyx_L1_error)
+  __pyx_t_7 = __pyx_f_6cyroot_3ops_10vector_ops_cabs(__pyx_v_f_x0s); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 308, __pyx_L1_error)
   __pyx_v_errors = __pyx_t_7;
   __pyx_t_7.memview = NULL;
   __pyx_t_7.data = NULL;
 
   /* "cyroot/_check_args.pyx":309
  *         return optimal[0]
- *     cdef double[:] errors = vops.cabs(f_xs)
+ *     cdef double[:] errors = vops.cabs(f_x0s)
  *     cdef unsigned long best_i = vops.argmin(errors)             # <<<<<<<<<<<<<<
- *     r[0], f_r[0] = xs[best_i], f_xs[best_i]
+ *     r[0], f_r[0] = x0s[best_i], f_x0s[best_i]
  *     error[0] = errors[best_i]
  */
   __pyx_v_best_i = __pyx_f_6cyroot_3ops_10vector_ops_argmin(__pyx_v_errors);
 
   /* "cyroot/_check_args.pyx":310
- *     cdef double[:] errors = vops.cabs(f_xs)
+ *     cdef double[:] errors = vops.cabs(f_x0s)
  *     cdef unsigned long best_i = vops.argmin(errors)
- *     r[0], f_r[0] = xs[best_i], f_xs[best_i]             # <<<<<<<<<<<<<<
+ *     r[0], f_r[0] = x0s[best_i], f_x0s[best_i]             # <<<<<<<<<<<<<<
  *     error[0] = errors[best_i]
- *     cdef double[:] xs_abs = vops.cabs(xs)
+ *     cdef double[:] xs_abs = vops.cabs(x0s)
  */
   __pyx_t_8 = __pyx_v_best_i;
-  __pyx_t_5 = (*((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_xs.data + __pyx_t_8 * __pyx_v_xs.strides[0]) )));
+  __pyx_t_5 = (*((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_x0s.data + __pyx_t_8 * __pyx_v_x0s.strides[0]) )));
   __pyx_t_8 = __pyx_v_best_i;
-  __pyx_t_4 = (*((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_f_xs.data + __pyx_t_8 * __pyx_v_f_xs.strides[0]) )));
+  __pyx_t_4 = (*((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_f_x0s.data + __pyx_t_8 * __pyx_v_f_x0s.strides[0]) )));
   (__pyx_v_r[0]) = __pyx_t_5;
   (__pyx_v_f_r[0]) = __pyx_t_4;
 
   /* "cyroot/_check_args.pyx":311
  *     cdef unsigned long best_i = vops.argmin(errors)
- *     r[0], f_r[0] = xs[best_i], f_xs[best_i]
+ *     r[0], f_r[0] = x0s[best_i], f_x0s[best_i]
  *     error[0] = errors[best_i]             # <<<<<<<<<<<<<<
- *     cdef double[:] xs_abs = vops.cabs(xs)
+ *     cdef double[:] xs_abs = vops.cabs(x0s)
  *     precision[0] = vops.max(xs_abs) - vops.min(xs_abs)
  */
   __pyx_t_8 = __pyx_v_best_i;
   (__pyx_v_error[0]) = (*((double *) ( /* dim=0 */ (__pyx_v_errors.data + __pyx_t_8 * __pyx_v_errors.strides[0]) )));
 
   /* "cyroot/_check_args.pyx":312
- *     r[0], f_r[0] = xs[best_i], f_xs[best_i]
+ *     r[0], f_r[0] = x0s[best_i], f_x0s[best_i]
  *     error[0] = errors[best_i]
- *     cdef double[:] xs_abs = vops.cabs(xs)             # <<<<<<<<<<<<<<
+ *     cdef double[:] xs_abs = vops.cabs(x0s)             # <<<<<<<<<<<<<<
  *     precision[0] = vops.max(xs_abs) - vops.min(xs_abs)
  *     optimal[0] = sops.isclose(0, error[0], ertol, etol)
  */
-  __pyx_t_7 = __pyx_f_6cyroot_3ops_10vector_ops_cabs(__pyx_v_xs); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 312, __pyx_L1_error)
+  __pyx_t_7 = __pyx_f_6cyroot_3ops_10vector_ops_cabs(__pyx_v_x0s); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 312, __pyx_L1_error)
   __pyx_v_xs_abs = __pyx_t_7;
   __pyx_t_7.memview = NULL;
   __pyx_t_7.data = NULL;
 
   /* "cyroot/_check_args.pyx":313
  *     error[0] = errors[best_i]
- *     cdef double[:] xs_abs = vops.cabs(xs)
+ *     cdef double[:] xs_abs = vops.cabs(x0s)
  *     precision[0] = vops.max(xs_abs) - vops.min(xs_abs)             # <<<<<<<<<<<<<<
  *     optimal[0] = sops.isclose(0, error[0], ertol, etol)
  *     converged[0] = sops.isclose(0, precision[0], prtol, ptol) or optimal[0]
  */
   (__pyx_v_precision[0]) = (__pyx_f_6cyroot_3ops_10vector_ops_max(__pyx_v_xs_abs) - __pyx_f_6cyroot_3ops_10vector_ops_min(__pyx_v_xs_abs));
 
   /* "cyroot/_check_args.pyx":314
- *     cdef double[:] xs_abs = vops.cabs(xs)
+ *     cdef double[:] xs_abs = vops.cabs(x0s)
  *     precision[0] = vops.max(xs_abs) - vops.min(xs_abs)
  *     optimal[0] = sops.isclose(0, error[0], ertol, etol)             # <<<<<<<<<<<<<<
  *     converged[0] = sops.isclose(0, precision[0], prtol, ptol) or optimal[0]
  *     return optimal[0] or sops.isclose(0, precision[0], prtol, ptol)
  */
   __pyx_t_6.__pyx_n = 2;
   __pyx_t_6.rtol = __pyx_v_ertol;
@@ -7026,16 +7026,16 @@
   __pyx_r = __pyx_t_1;
   goto __pyx_L0;
 
   /* "cyroot/_check_args.pyx":285
  * 
  * # noinspection DuplicatedCode
  * cdef inline bint _check_stop_cond_complex_scalar_initial_guesses(             # <<<<<<<<<<<<<<
- *         double complex[:] xs,
- *         double complex[:] f_xs,
+ *         double complex[:] x0s,
+ *         double complex[:] f_x0s,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __PYX_XDEC_MEMVIEW(&__pyx_t_7, 1);
   __Pyx_WriteUnraisable("cyroot._check_args._check_stop_cond_complex_scalar_initial_guesses", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
@@ -7047,19 +7047,19 @@
   return __pyx_r;
 }
 
 /* "cyroot/_check_args.pyx":319
  * 
  * # noinspection DuplicatedCode
  * cdef inline bint _check_stop_cond_complex_vector_initial_guesses(             # <<<<<<<<<<<<<<
- *         double complex[:, :] xs,
- *         double complex[:, :] F_xs,
+ *         double complex[:, :] x0s,
+ *         double complex[:, :] F_x0s,
  */
 
-static CYTHON_INLINE int __pyx_f_6cyroot_11_check_args__check_stop_cond_complex_vector_initial_guesses(__Pyx_memviewslice __pyx_v_xs, __Pyx_memviewslice __pyx_v_F_xs, double __pyx_v_etol, double __pyx_v_ertol, double __pyx_v_ptol, double __pyx_v_prtol, __Pyx_memviewslice __pyx_v_r, __Pyx_memviewslice __pyx_v_F_r, double *__pyx_v_precision, double *__pyx_v_error, int *__pyx_v_converged, int *__pyx_v_optimal) {
+static CYTHON_INLINE int __pyx_f_6cyroot_11_check_args__check_stop_cond_complex_vector_initial_guesses(__Pyx_memviewslice __pyx_v_x0s, __Pyx_memviewslice __pyx_v_F_x0s, double __pyx_v_etol, double __pyx_v_ertol, double __pyx_v_ptol, double __pyx_v_prtol, __Pyx_memviewslice __pyx_v_r, __Pyx_memviewslice __pyx_v_F_r, double *__pyx_v_precision, double *__pyx_v_error, int *__pyx_v_converged, int *__pyx_v_optimal) {
   __Pyx_memviewslice __pyx_v_errors = { 0, 0, { 0 }, { 0 }, { 0 } };
   unsigned long __pyx_v_best_i;
   __Pyx_memviewslice __pyx_v_xs_abs = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
@@ -7081,196 +7081,196 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_check_stop_cond_complex_vector_initial_guesses", 0);
 
   /* "cyroot/_check_args.pyx":333
  *         bint* optimal):
  *     """Check if stop condition is already met."""
- *     if xs.shape[0] == 0:             # <<<<<<<<<<<<<<
+ *     if x0s.shape[0] == 0:             # <<<<<<<<<<<<<<
  *         raise ValueError('Empty sequence.')
- *     if xs.shape[0] == 1:
+ *     if x0s.shape[0] == 1:
  */
-  __pyx_t_1 = (((__pyx_v_xs.shape[0]) == 0) != 0);
+  __pyx_t_1 = (((__pyx_v_x0s.shape[0]) == 0) != 0);
   if (unlikely(__pyx_t_1)) {
 
     /* "cyroot/_check_args.pyx":334
  *     """Check if stop condition is already met."""
- *     if xs.shape[0] == 0:
+ *     if x0s.shape[0] == 0:
  *         raise ValueError('Empty sequence.')             # <<<<<<<<<<<<<<
- *     if xs.shape[0] == 1:
- *         r[:], F_r[:] = xs[0], F_xs[0]
+ *     if x0s.shape[0] == 1:
+ *         r[:], F_r[:] = x0s[0], F_x0s[0]
  */
     __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 334, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(0, 334, __pyx_L1_error)
 
     /* "cyroot/_check_args.pyx":333
  *         bint* optimal):
  *     """Check if stop condition is already met."""
- *     if xs.shape[0] == 0:             # <<<<<<<<<<<<<<
+ *     if x0s.shape[0] == 0:             # <<<<<<<<<<<<<<
  *         raise ValueError('Empty sequence.')
- *     if xs.shape[0] == 1:
+ *     if x0s.shape[0] == 1:
  */
   }
 
   /* "cyroot/_check_args.pyx":335
- *     if xs.shape[0] == 0:
+ *     if x0s.shape[0] == 0:
  *         raise ValueError('Empty sequence.')
- *     if xs.shape[0] == 1:             # <<<<<<<<<<<<<<
- *         r[:], F_r[:] = xs[0], F_xs[0]
+ *     if x0s.shape[0] == 1:             # <<<<<<<<<<<<<<
+ *         r[:], F_r[:] = x0s[0], F_x0s[0]
  *         precision[0] = math.INFINITY
  */
-  __pyx_t_1 = (((__pyx_v_xs.shape[0]) == 1) != 0);
+  __pyx_t_1 = (((__pyx_v_x0s.shape[0]) == 1) != 0);
   if (__pyx_t_1) {
 
     /* "cyroot/_check_args.pyx":336
  *         raise ValueError('Empty sequence.')
- *     if xs.shape[0] == 1:
- *         r[:], F_r[:] = xs[0], F_xs[0]             # <<<<<<<<<<<<<<
+ *     if x0s.shape[0] == 1:
+ *         r[:], F_r[:] = x0s[0], F_x0s[0]             # <<<<<<<<<<<<<<
  *         precision[0] = math.INFINITY
- *         error[0] = vops.max(vops.cabs(F_xs[0]))
+ *         error[0] = vops.max(vops.cabs(F_x0s[0]))
  */
-    __pyx_t_3.data = __pyx_v_xs.data;
-    __pyx_t_3.memview = __pyx_v_xs.memview;
+    __pyx_t_3.data = __pyx_v_x0s.data;
+    __pyx_t_3.memview = __pyx_v_x0s.memview;
     __PYX_INC_MEMVIEW(&__pyx_t_3, 0);
     {
     Py_ssize_t __pyx_tmp_idx = 0;
-        Py_ssize_t __pyx_tmp_shape = __pyx_v_xs.shape[0];
-    Py_ssize_t __pyx_tmp_stride = __pyx_v_xs.strides[0];
+        Py_ssize_t __pyx_tmp_shape = __pyx_v_x0s.shape[0];
+    Py_ssize_t __pyx_tmp_stride = __pyx_v_x0s.strides[0];
         if (__pyx_tmp_idx < 0)
             __pyx_tmp_idx += __pyx_tmp_shape;
         __pyx_t_3.data += __pyx_tmp_idx * __pyx_tmp_stride;
 }
 
-__pyx_t_3.shape[0] = __pyx_v_xs.shape[1];
-__pyx_t_3.strides[0] = __pyx_v_xs.strides[1];
+__pyx_t_3.shape[0] = __pyx_v_x0s.shape[1];
+__pyx_t_3.strides[0] = __pyx_v_x0s.strides[1];
     __pyx_t_3.suboffsets[0] = -1;
 
-__pyx_t_4.data = __pyx_v_F_xs.data;
-    __pyx_t_4.memview = __pyx_v_F_xs.memview;
+__pyx_t_4.data = __pyx_v_F_x0s.data;
+    __pyx_t_4.memview = __pyx_v_F_x0s.memview;
     __PYX_INC_MEMVIEW(&__pyx_t_4, 0);
     {
     Py_ssize_t __pyx_tmp_idx = 0;
-        Py_ssize_t __pyx_tmp_shape = __pyx_v_F_xs.shape[0];
-    Py_ssize_t __pyx_tmp_stride = __pyx_v_F_xs.strides[0];
+        Py_ssize_t __pyx_tmp_shape = __pyx_v_F_x0s.shape[0];
+    Py_ssize_t __pyx_tmp_stride = __pyx_v_F_x0s.strides[0];
         if (__pyx_tmp_idx < 0)
             __pyx_tmp_idx += __pyx_tmp_shape;
         __pyx_t_4.data += __pyx_tmp_idx * __pyx_tmp_stride;
 }
 
-__pyx_t_4.shape[0] = __pyx_v_F_xs.shape[1];
-__pyx_t_4.strides[0] = __pyx_v_F_xs.strides[1];
+__pyx_t_4.shape[0] = __pyx_v_F_x0s.shape[1];
+__pyx_t_4.strides[0] = __pyx_v_F_x0s.strides[1];
     __pyx_t_4.suboffsets[0] = -1;
 
 if (unlikely(__pyx_memoryview_copy_contents(__pyx_t_3, __pyx_v_r, 1, 1, 0) < 0)) __PYX_ERR(0, 336, __pyx_L1_error)
     __PYX_XDEC_MEMVIEW(&__pyx_t_3, 1);
     __pyx_t_3.memview = NULL;
     __pyx_t_3.data = NULL;
     if (unlikely(__pyx_memoryview_copy_contents(__pyx_t_4, __pyx_v_F_r, 1, 1, 0) < 0)) __PYX_ERR(0, 336, __pyx_L1_error)
     __PYX_XDEC_MEMVIEW(&__pyx_t_4, 1);
     __pyx_t_4.memview = NULL;
     __pyx_t_4.data = NULL;
 
     /* "cyroot/_check_args.pyx":337
- *     if xs.shape[0] == 1:
- *         r[:], F_r[:] = xs[0], F_xs[0]
+ *     if x0s.shape[0] == 1:
+ *         r[:], F_r[:] = x0s[0], F_x0s[0]
  *         precision[0] = math.INFINITY             # <<<<<<<<<<<<<<
- *         error[0] = vops.max(vops.cabs(F_xs[0]))
+ *         error[0] = vops.max(vops.cabs(F_x0s[0]))
  *         optimal[0] = sops.isclose(0, error[0], ertol, etol)
  */
     (__pyx_v_precision[0]) = INFINITY;
 
     /* "cyroot/_check_args.pyx":338
- *         r[:], F_r[:] = xs[0], F_xs[0]
+ *         r[:], F_r[:] = x0s[0], F_x0s[0]
  *         precision[0] = math.INFINITY
- *         error[0] = vops.max(vops.cabs(F_xs[0]))             # <<<<<<<<<<<<<<
+ *         error[0] = vops.max(vops.cabs(F_x0s[0]))             # <<<<<<<<<<<<<<
  *         optimal[0] = sops.isclose(0, error[0], ertol, etol)
  *         converged[0] = optimal[0]
  */
-    __pyx_t_4.data = __pyx_v_F_xs.data;
-    __pyx_t_4.memview = __pyx_v_F_xs.memview;
+    __pyx_t_4.data = __pyx_v_F_x0s.data;
+    __pyx_t_4.memview = __pyx_v_F_x0s.memview;
     __PYX_INC_MEMVIEW(&__pyx_t_4, 0);
     {
     Py_ssize_t __pyx_tmp_idx = 0;
-        Py_ssize_t __pyx_tmp_shape = __pyx_v_F_xs.shape[0];
-    Py_ssize_t __pyx_tmp_stride = __pyx_v_F_xs.strides[0];
+        Py_ssize_t __pyx_tmp_shape = __pyx_v_F_x0s.shape[0];
+    Py_ssize_t __pyx_tmp_stride = __pyx_v_F_x0s.strides[0];
         if (__pyx_tmp_idx < 0)
             __pyx_tmp_idx += __pyx_tmp_shape;
         __pyx_t_4.data += __pyx_tmp_idx * __pyx_tmp_stride;
 }
 
-__pyx_t_4.shape[0] = __pyx_v_F_xs.shape[1];
-__pyx_t_4.strides[0] = __pyx_v_F_xs.strides[1];
+__pyx_t_4.shape[0] = __pyx_v_F_x0s.shape[1];
+__pyx_t_4.strides[0] = __pyx_v_F_x0s.strides[1];
     __pyx_t_4.suboffsets[0] = -1;
 
 __pyx_t_5 = __pyx_f_6cyroot_3ops_10vector_ops_cabs(__pyx_t_4); if (unlikely(!__pyx_t_5.memview)) __PYX_ERR(0, 338, __pyx_L1_error)
     __PYX_XDEC_MEMVIEW(&__pyx_t_4, 1);
     __pyx_t_4.memview = NULL;
     __pyx_t_4.data = NULL;
     (__pyx_v_error[0]) = __pyx_f_6cyroot_3ops_10vector_ops_max(__pyx_t_5);
     __PYX_XDEC_MEMVIEW(&__pyx_t_5, 1);
     __pyx_t_5.memview = NULL;
     __pyx_t_5.data = NULL;
 
     /* "cyroot/_check_args.pyx":339
  *         precision[0] = math.INFINITY
- *         error[0] = vops.max(vops.cabs(F_xs[0]))
+ *         error[0] = vops.max(vops.cabs(F_x0s[0]))
  *         optimal[0] = sops.isclose(0, error[0], ertol, etol)             # <<<<<<<<<<<<<<
  *         converged[0] = optimal[0]
  *         return optimal[0]
  */
     __pyx_t_6.__pyx_n = 2;
     __pyx_t_6.rtol = __pyx_v_ertol;
     __pyx_t_6.atol = __pyx_v_etol;
     __pyx_t_1 = __pyx_f_6cyroot_3ops_10scalar_ops_isclose(0.0, (__pyx_v_error[0]), &__pyx_t_6); 
     (__pyx_v_optimal[0]) = __pyx_t_1;
 
     /* "cyroot/_check_args.pyx":340
- *         error[0] = vops.max(vops.cabs(F_xs[0]))
+ *         error[0] = vops.max(vops.cabs(F_x0s[0]))
  *         optimal[0] = sops.isclose(0, error[0], ertol, etol)
  *         converged[0] = optimal[0]             # <<<<<<<<<<<<<<
  *         return optimal[0]
- *     cdef double[:] errors = np.abs(F_xs).max(1)
+ *     cdef double[:] errors = np.abs(F_x0s).max(1)
  */
     (__pyx_v_converged[0]) = (__pyx_v_optimal[0]);
 
     /* "cyroot/_check_args.pyx":341
  *         optimal[0] = sops.isclose(0, error[0], ertol, etol)
  *         converged[0] = optimal[0]
  *         return optimal[0]             # <<<<<<<<<<<<<<
- *     cdef double[:] errors = np.abs(F_xs).max(1)
+ *     cdef double[:] errors = np.abs(F_x0s).max(1)
  *     cdef unsigned long best_i = vops.argmin(errors)
  */
     __pyx_r = (__pyx_v_optimal[0]);
     goto __pyx_L0;
 
     /* "cyroot/_check_args.pyx":335
- *     if xs.shape[0] == 0:
+ *     if x0s.shape[0] == 0:
  *         raise ValueError('Empty sequence.')
- *     if xs.shape[0] == 1:             # <<<<<<<<<<<<<<
- *         r[:], F_r[:] = xs[0], F_xs[0]
+ *     if x0s.shape[0] == 1:             # <<<<<<<<<<<<<<
+ *         r[:], F_r[:] = x0s[0], F_x0s[0]
  *         precision[0] = math.INFINITY
  */
   }
 
   /* "cyroot/_check_args.pyx":342
  *         converged[0] = optimal[0]
  *         return optimal[0]
- *     cdef double[:] errors = np.abs(F_xs).max(1)             # <<<<<<<<<<<<<<
+ *     cdef double[:] errors = np.abs(F_x0s).max(1)             # <<<<<<<<<<<<<<
  *     cdef unsigned long best_i = vops.argmin(errors)
- *     r[:], F_r[:] = xs[best_i], F_xs[best_i]
+ *     r[:], F_r[:] = x0s[best_i], F_x0s[best_i]
  */
   __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 342, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_abs); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 342, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __pyx_memoryview_fromslice(__pyx_v_F_xs, 2, (PyObject *(*)(char *)) __pyx_memview_get___pyx_t_double_complex, (int (*)(char *, PyObject *)) __pyx_memview_set___pyx_t_double_complex, 0);; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 342, __pyx_L1_error)
+  __pyx_t_8 = __pyx_memoryview_fromslice(__pyx_v_F_x0s, 2, (PyObject *(*)(char *)) __pyx_memview_get___pyx_t_double_complex, (int (*)(char *, PyObject *)) __pyx_memview_set___pyx_t_double_complex, 0);; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 342, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __pyx_t_10 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
     __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
     if (likely(__pyx_t_10)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
       __Pyx_INCREF(__pyx_t_10);
@@ -7306,92 +7306,92 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_errors = __pyx_t_5;
   __pyx_t_5.memview = NULL;
   __pyx_t_5.data = NULL;
 
   /* "cyroot/_check_args.pyx":343
  *         return optimal[0]
- *     cdef double[:] errors = np.abs(F_xs).max(1)
+ *     cdef double[:] errors = np.abs(F_x0s).max(1)
  *     cdef unsigned long best_i = vops.argmin(errors)             # <<<<<<<<<<<<<<
- *     r[:], F_r[:] = xs[best_i], F_xs[best_i]
+ *     r[:], F_r[:] = x0s[best_i], F_x0s[best_i]
  *     error[0] = errors[best_i]
  */
   __pyx_v_best_i = __pyx_f_6cyroot_3ops_10vector_ops_argmin(__pyx_v_errors);
 
   /* "cyroot/_check_args.pyx":344
- *     cdef double[:] errors = np.abs(F_xs).max(1)
+ *     cdef double[:] errors = np.abs(F_x0s).max(1)
  *     cdef unsigned long best_i = vops.argmin(errors)
- *     r[:], F_r[:] = xs[best_i], F_xs[best_i]             # <<<<<<<<<<<<<<
+ *     r[:], F_r[:] = x0s[best_i], F_x0s[best_i]             # <<<<<<<<<<<<<<
  *     error[0] = errors[best_i]
- *     cdef double[:, :] xs_abs = np.abs(xs)
+ *     cdef double[:, :] xs_abs = np.abs(x0s)
  */
-  __pyx_t_4.data = __pyx_v_xs.data;
-  __pyx_t_4.memview = __pyx_v_xs.memview;
+  __pyx_t_4.data = __pyx_v_x0s.data;
+  __pyx_t_4.memview = __pyx_v_x0s.memview;
   __PYX_INC_MEMVIEW(&__pyx_t_4, 0);
   {
     Py_ssize_t __pyx_tmp_idx = __pyx_v_best_i;
-        Py_ssize_t __pyx_tmp_shape = __pyx_v_xs.shape[0];
-    Py_ssize_t __pyx_tmp_stride = __pyx_v_xs.strides[0];
+        Py_ssize_t __pyx_tmp_shape = __pyx_v_x0s.shape[0];
+    Py_ssize_t __pyx_tmp_stride = __pyx_v_x0s.strides[0];
         if (__pyx_tmp_idx < 0)
             __pyx_tmp_idx += __pyx_tmp_shape;
         __pyx_t_4.data += __pyx_tmp_idx * __pyx_tmp_stride;
 }
 
-__pyx_t_4.shape[0] = __pyx_v_xs.shape[1];
-__pyx_t_4.strides[0] = __pyx_v_xs.strides[1];
+__pyx_t_4.shape[0] = __pyx_v_x0s.shape[1];
+__pyx_t_4.strides[0] = __pyx_v_x0s.strides[1];
     __pyx_t_4.suboffsets[0] = -1;
 
-__pyx_t_3.data = __pyx_v_F_xs.data;
-  __pyx_t_3.memview = __pyx_v_F_xs.memview;
+__pyx_t_3.data = __pyx_v_F_x0s.data;
+  __pyx_t_3.memview = __pyx_v_F_x0s.memview;
   __PYX_INC_MEMVIEW(&__pyx_t_3, 0);
   {
     Py_ssize_t __pyx_tmp_idx = __pyx_v_best_i;
-        Py_ssize_t __pyx_tmp_shape = __pyx_v_F_xs.shape[0];
-    Py_ssize_t __pyx_tmp_stride = __pyx_v_F_xs.strides[0];
+        Py_ssize_t __pyx_tmp_shape = __pyx_v_F_x0s.shape[0];
+    Py_ssize_t __pyx_tmp_stride = __pyx_v_F_x0s.strides[0];
         if (__pyx_tmp_idx < 0)
             __pyx_tmp_idx += __pyx_tmp_shape;
         __pyx_t_3.data += __pyx_tmp_idx * __pyx_tmp_stride;
 }
 
-__pyx_t_3.shape[0] = __pyx_v_F_xs.shape[1];
-__pyx_t_3.strides[0] = __pyx_v_F_xs.strides[1];
+__pyx_t_3.shape[0] = __pyx_v_F_x0s.shape[1];
+__pyx_t_3.strides[0] = __pyx_v_F_x0s.strides[1];
     __pyx_t_3.suboffsets[0] = -1;
 
 if (unlikely(__pyx_memoryview_copy_contents(__pyx_t_4, __pyx_v_r, 1, 1, 0) < 0)) __PYX_ERR(0, 344, __pyx_L1_error)
   __PYX_XDEC_MEMVIEW(&__pyx_t_4, 1);
   __pyx_t_4.memview = NULL;
   __pyx_t_4.data = NULL;
   if (unlikely(__pyx_memoryview_copy_contents(__pyx_t_3, __pyx_v_F_r, 1, 1, 0) < 0)) __PYX_ERR(0, 344, __pyx_L1_error)
   __PYX_XDEC_MEMVIEW(&__pyx_t_3, 1);
   __pyx_t_3.memview = NULL;
   __pyx_t_3.data = NULL;
 
   /* "cyroot/_check_args.pyx":345
  *     cdef unsigned long best_i = vops.argmin(errors)
- *     r[:], F_r[:] = xs[best_i], F_xs[best_i]
+ *     r[:], F_r[:] = x0s[best_i], F_x0s[best_i]
  *     error[0] = errors[best_i]             # <<<<<<<<<<<<<<
- *     cdef double[:, :] xs_abs = np.abs(xs)
+ *     cdef double[:, :] xs_abs = np.abs(x0s)
  *     precision[0] = vops.max(np.max(xs_abs, 0) - np.min(xs_abs, 0))
  */
   __pyx_t_11 = __pyx_v_best_i;
   (__pyx_v_error[0]) = (*((double *) ( /* dim=0 */ (__pyx_v_errors.data + __pyx_t_11 * __pyx_v_errors.strides[0]) )));
 
   /* "cyroot/_check_args.pyx":346
- *     r[:], F_r[:] = xs[best_i], F_xs[best_i]
+ *     r[:], F_r[:] = x0s[best_i], F_x0s[best_i]
  *     error[0] = errors[best_i]
- *     cdef double[:, :] xs_abs = np.abs(xs)             # <<<<<<<<<<<<<<
+ *     cdef double[:, :] xs_abs = np.abs(x0s)             # <<<<<<<<<<<<<<
  *     precision[0] = vops.max(np.max(xs_abs, 0) - np.min(xs_abs, 0))
  *     optimal[0] = sops.isclose(0, error[0], ertol, etol)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 346, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_abs); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 346, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  __pyx_t_9 = __pyx_memoryview_fromslice(__pyx_v_xs, 2, (PyObject *(*)(char *)) __pyx_memview_get___pyx_t_double_complex, (int (*)(char *, PyObject *)) __pyx_memview_set___pyx_t_double_complex, 0);; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 346, __pyx_L1_error)
+  __pyx_t_9 = __pyx_memoryview_fromslice(__pyx_v_x0s, 2, (PyObject *(*)(char *)) __pyx_memview_get___pyx_t_double_complex, (int (*)(char *, PyObject *)) __pyx_memview_set___pyx_t_double_complex, 0);; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 346, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __pyx_t_8 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
     __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
     if (likely(__pyx_t_8)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
       __Pyx_INCREF(__pyx_t_8);
@@ -7409,15 +7409,15 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_xs_abs = __pyx_t_12;
   __pyx_t_12.memview = NULL;
   __pyx_t_12.data = NULL;
 
   /* "cyroot/_check_args.pyx":347
  *     error[0] = errors[best_i]
- *     cdef double[:, :] xs_abs = np.abs(xs)
+ *     cdef double[:, :] xs_abs = np.abs(x0s)
  *     precision[0] = vops.max(np.max(xs_abs, 0) - np.min(xs_abs, 0))             # <<<<<<<<<<<<<<
  *     optimal[0] = sops.isclose(0, error[0], ertol, etol)
  *     converged[0] = sops.isclose(0, precision[0], prtol, ptol) or optimal[0]
  */
   __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 347, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_max); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 347, __pyx_L1_error)
@@ -7534,15 +7534,15 @@
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   (__pyx_v_precision[0]) = __pyx_f_6cyroot_3ops_10vector_ops_max(__pyx_t_5);
   __PYX_XDEC_MEMVIEW(&__pyx_t_5, 1);
   __pyx_t_5.memview = NULL;
   __pyx_t_5.data = NULL;
 
   /* "cyroot/_check_args.pyx":348
- *     cdef double[:, :] xs_abs = np.abs(xs)
+ *     cdef double[:, :] xs_abs = np.abs(x0s)
  *     precision[0] = vops.max(np.max(xs_abs, 0) - np.min(xs_abs, 0))
  *     optimal[0] = sops.isclose(0, error[0], ertol, etol)             # <<<<<<<<<<<<<<
  *     converged[0] = sops.isclose(0, precision[0], prtol, ptol) or optimal[0]
  *     return optimal[0] or sops.isclose(0, precision[0], prtol, ptol)
  */
   __pyx_t_6.__pyx_n = 2;
   __pyx_t_6.rtol = __pyx_v_ertol;
@@ -7592,16 +7592,16 @@
   __pyx_r = __pyx_t_1;
   goto __pyx_L0;
 
   /* "cyroot/_check_args.pyx":319
  * 
  * # noinspection DuplicatedCode
  * cdef inline bint _check_stop_cond_complex_vector_initial_guesses(             # <<<<<<<<<<<<<<
- *         double complex[:, :] xs,
- *         double complex[:, :] F_xs,
+ *         double complex[:, :] x0s,
+ *         double complex[:, :] F_x0s,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __PYX_XDEC_MEMVIEW(&__pyx_t_3, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_t_4, 1);
@@ -7617,15 +7617,15 @@
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_errors, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_xs_abs, 1);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -7634,29 +7634,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -7667,15 +7667,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -7684,29 +7684,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -7717,15 +7717,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -7734,29 +7734,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -7767,15 +7767,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -7784,29 +7784,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -7817,15 +7817,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -7834,29 +7834,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -7867,212 +7867,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -8088,15 +8088,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -8104,53 +8104,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
@@ -8158,30 +8158,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -8196,15 +8196,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8220,15 +8220,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -8236,53 +8236,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
@@ -8290,30 +8290,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8328,15 +8328,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8352,15 +8352,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -8368,53 +8368,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
@@ -8422,30 +8422,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8460,176 +8460,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -21695,36 +21695,36 @@
   }
   return o;
 }
 
 static void __pyx_tp_dealloc_6cyroot_11_check_args___pyx_scope_struct___check_initial_guesses_uniqueness(PyObject *o) {
   struct __pyx_obj_6cyroot_11_check_args___pyx_scope_struct___check_initial_guesses_uniqueness *p = (struct __pyx_obj_6cyroot_11_check_args___pyx_scope_struct___check_initial_guesses_uniqueness *)o;
   PyObject_GC_UnTrack(o);
-  Py_CLEAR(p->__pyx_v_xs);
+  Py_CLEAR(p->__pyx_v_x0s);
   if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_6cyroot_11_check_args___pyx_scope_struct___check_initial_guesses_uniqueness < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_6cyroot_11_check_args___pyx_scope_struct___check_initial_guesses_uniqueness)))) {
     __pyx_freelist_6cyroot_11_check_args___pyx_scope_struct___check_initial_guesses_uniqueness[__pyx_freecount_6cyroot_11_check_args___pyx_scope_struct___check_initial_guesses_uniqueness++] = ((struct __pyx_obj_6cyroot_11_check_args___pyx_scope_struct___check_initial_guesses_uniqueness *)o);
   } else {
     (*Py_TYPE(o)->tp_free)(o);
   }
 }
 
 static int __pyx_tp_traverse_6cyroot_11_check_args___pyx_scope_struct___check_initial_guesses_uniqueness(PyObject *o, visitproc v, void *a) {
   int e;
   struct __pyx_obj_6cyroot_11_check_args___pyx_scope_struct___check_initial_guesses_uniqueness *p = (struct __pyx_obj_6cyroot_11_check_args___pyx_scope_struct___check_initial_guesses_uniqueness *)o;
-  if (p->__pyx_v_xs) {
-    e = (*v)(p->__pyx_v_xs, a); if (e) return e;
+  if (p->__pyx_v_x0s) {
+    e = (*v)(p->__pyx_v_x0s, a); if (e) return e;
   }
   return 0;
 }
 
 static int __pyx_tp_clear_6cyroot_11_check_args___pyx_scope_struct___check_initial_guesses_uniqueness(PyObject *o) {
   PyObject* tmp;
   struct __pyx_obj_6cyroot_11_check_args___pyx_scope_struct___check_initial_guesses_uniqueness *p = (struct __pyx_obj_6cyroot_11_check_args___pyx_scope_struct___check_initial_guesses_uniqueness *)o;
-  tmp = ((PyObject*)p->__pyx_v_xs);
-  p->__pyx_v_xs = Py_None; Py_INCREF(Py_None);
+  tmp = ((PyObject*)p->__pyx_v_x0s);
+  p->__pyx_v_x0s = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   return 0;
 }
 
 static PyTypeObject __pyx_type_6cyroot_11_check_args___pyx_scope_struct___check_initial_guesses_uniqueness = {
   PyVarObject_HEAD_INIT(0, 0)
   "cyroot._check_args.__pyx_scope_struct___check_initial_guesses_uniqueness", /*tp_name*/
@@ -21926,36 +21926,36 @@
   }
   return o;
 }
 
 static void __pyx_tp_dealloc_6cyroot_11_check_args___pyx_scope_struct_2__check_initial_vals_uniqueness(PyObject *o) {
   struct __pyx_obj_6cyroot_11_check_args___pyx_scope_struct_2__check_initial_vals_uniqueness *p = (struct __pyx_obj_6cyroot_11_check_args___pyx_scope_struct_2__check_initial_vals_uniqueness *)o;
   PyObject_GC_UnTrack(o);
-  Py_CLEAR(p->__pyx_v_f_xs);
+  Py_CLEAR(p->__pyx_v_f_x0s);
   if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_6cyroot_11_check_args___pyx_scope_struct_2__check_initial_vals_uniqueness < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_6cyroot_11_check_args___pyx_scope_struct_2__check_initial_vals_uniqueness)))) {
     __pyx_freelist_6cyroot_11_check_args___pyx_scope_struct_2__check_initial_vals_uniqueness[__pyx_freecount_6cyroot_11_check_args___pyx_scope_struct_2__check_initial_vals_uniqueness++] = ((struct __pyx_obj_6cyroot_11_check_args___pyx_scope_struct_2__check_initial_vals_uniqueness *)o);
   } else {
     (*Py_TYPE(o)->tp_free)(o);
   }
 }
 
 static int __pyx_tp_traverse_6cyroot_11_check_args___pyx_scope_struct_2__check_initial_vals_uniqueness(PyObject *o, visitproc v, void *a) {
   int e;
   struct __pyx_obj_6cyroot_11_check_args___pyx_scope_struct_2__check_initial_vals_uniqueness *p = (struct __pyx_obj_6cyroot_11_check_args___pyx_scope_struct_2__check_initial_vals_uniqueness *)o;
-  if (p->__pyx_v_f_xs) {
-    e = (*v)(p->__pyx_v_f_xs, a); if (e) return e;
+  if (p->__pyx_v_f_x0s) {
+    e = (*v)(p->__pyx_v_f_x0s, a); if (e) return e;
   }
   return 0;
 }
 
 static int __pyx_tp_clear_6cyroot_11_check_args___pyx_scope_struct_2__check_initial_vals_uniqueness(PyObject *o) {
   PyObject* tmp;
   struct __pyx_obj_6cyroot_11_check_args___pyx_scope_struct_2__check_initial_vals_uniqueness *p = (struct __pyx_obj_6cyroot_11_check_args___pyx_scope_struct_2__check_initial_vals_uniqueness *)o;
-  tmp = ((PyObject*)p->__pyx_v_f_xs);
-  p->__pyx_v_f_xs = Py_None; Py_INCREF(Py_None);
+  tmp = ((PyObject*)p->__pyx_v_f_x0s);
+  p->__pyx_v_f_x0s = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   return 0;
 }
 
 static PyTypeObject __pyx_type_6cyroot_11_check_args___pyx_scope_struct_2__check_initial_vals_uniqueness = {
   PyVarObject_HEAD_INIT(0, 0)
   "cyroot._check_args.__pyx_scope_struct_2__check_initial_vals_uniqueness", /*tp_name*/
@@ -22979,15 +22979,15 @@
   {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
   {&__pyx_n_s_enumerate, __pyx_k_enumerate, sizeof(__pyx_k_enumerate), 0, 0, 1, 1},
   {&__pyx_n_s_error, __pyx_k_error, sizeof(__pyx_k_error), 0, 0, 1, 1},
   {&__pyx_n_s_ertol, __pyx_k_ertol, sizeof(__pyx_k_ertol), 0, 0, 1, 1},
   {&__pyx_n_u_ertol, __pyx_k_ertol, sizeof(__pyx_k_ertol), 0, 1, 0, 1},
   {&__pyx_n_s_etol, __pyx_k_etol, sizeof(__pyx_k_etol), 0, 0, 1, 1},
   {&__pyx_n_u_etol, __pyx_k_etol, sizeof(__pyx_k_etol), 0, 1, 0, 1},
-  {&__pyx_n_s_f_xs, __pyx_k_f_xs, sizeof(__pyx_k_f_xs), 0, 0, 1, 1},
+  {&__pyx_n_s_f_x0s, __pyx_k_f_x0s, sizeof(__pyx_k_f_x0s), 0, 0, 1, 1},
   {&__pyx_n_s_flags, __pyx_k_flags, sizeof(__pyx_k_flags), 0, 0, 1, 1},
   {&__pyx_n_s_format, __pyx_k_format, sizeof(__pyx_k_format), 0, 0, 1, 1},
   {&__pyx_n_s_fortran, __pyx_k_fortran, sizeof(__pyx_k_fortran), 0, 0, 1, 1},
   {&__pyx_n_u_fortran, __pyx_k_fortran, sizeof(__pyx_k_fortran), 0, 1, 0, 1},
   {&__pyx_n_s_genexpr, __pyx_k_genexpr, sizeof(__pyx_k_genexpr), 0, 0, 1, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
   {&__pyx_kp_s_got_differing_extents_in_dimensi, __pyx_k_got_differing_extents_in_dimensi, sizeof(__pyx_k_got_differing_extents_in_dimensi), 0, 0, 1, 0},
@@ -23052,15 +23052,15 @@
   {&__pyx_n_u_tol, __pyx_k_tol, sizeof(__pyx_k_tol), 0, 1, 0, 1},
   {&__pyx_n_s_typing, __pyx_k_typing, sizeof(__pyx_k_typing), 0, 0, 1, 1},
   {&__pyx_kp_s_unable_to_allocate_array_data, __pyx_k_unable_to_allocate_array_data, sizeof(__pyx_k_unable_to_allocate_array_data), 0, 0, 1, 0},
   {&__pyx_kp_s_unable_to_allocate_shape_and_str, __pyx_k_unable_to_allocate_shape_and_str, sizeof(__pyx_k_unable_to_allocate_shape_and_str), 0, 0, 1, 0},
   {&__pyx_n_s_unique, __pyx_k_unique, sizeof(__pyx_k_unique), 0, 0, 1, 1},
   {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
-  {&__pyx_n_s_xs, __pyx_k_xs, sizeof(__pyx_k_xs), 0, 0, 1, 1},
+  {&__pyx_n_s_x0s, __pyx_k_x0s, sizeof(__pyx_k_x0s), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 29, __pyx_L1_error)
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 944, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(2, 149, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(2, 152, __pyx_L1_error)
@@ -23086,19 +23086,19 @@
  *     return etol, ertol, ptol, prtol, max_iter
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_Disabling_both_tolerances_and_ma); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "cyroot/_check_args.pyx":57
- * def _check_initial_guesses_uniqueness(xs: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):
- *     if not len(xs):
+ * def _check_initial_guesses_uniqueness(x0s: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):
+ *     if not len(x0s):
  *         raise ValueError('Empty.')             # <<<<<<<<<<<<<<
- *     elif isinstance(xs[0], np.ndarray):
- *         if np.unique(xs if isinstance(xs, np.ndarray) else
+ *     elif isinstance(x0s[0], np.ndarray):
+ *         if np.unique(x0s if isinstance(x0s, np.ndarray) else
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_Empty); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
   /* "cyroot/_check_args.pyx":123
  *     """Check if stop condition is already met."""
@@ -23107,26 +23107,26 @@
  *     precision[0] = vops.max(np.max(bs, 0) - np.min(bs, 0))
  *     cdef double[:] errors = np.abs(F_bs).max(1)
  */
   __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_Empty_sequence); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 123, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 950, __pyx_L1_error)
@@ -23351,31 +23351,31 @@
   __Pyx_GOTREF(__pyx_tuple__29);
   __Pyx_GIVEREF(__pyx_tuple__29);
   __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(5, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cyroot__check_args_pyx, __pyx_n_s_check_stop_cond_args, 33, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 33, __pyx_L1_error)
 
   /* "cyroot/_check_args.pyx":55
  * 
  * # noinspection DuplicatedCode
- * def _check_initial_guesses_uniqueness(xs: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):             # <<<<<<<<<<<<<<
- *     if not len(xs):
+ * def _check_initial_guesses_uniqueness(x0s: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):             # <<<<<<<<<<<<<<
+ *     if not len(x0s):
  *         raise ValueError('Empty.')
  */
-  __pyx_tuple__31 = PyTuple_Pack(3, __pyx_n_s_xs, __pyx_n_s_genexpr, __pyx_n_s_genexpr); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __pyx_tuple__31 = PyTuple_Pack(3, __pyx_n_s_x0s, __pyx_n_s_genexpr, __pyx_n_s_genexpr); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 55, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__31);
   __Pyx_GIVEREF(__pyx_tuple__31);
   __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cyroot__check_args_pyx, __pyx_n_s_check_initial_guesses_uniquenes_2, 55, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 55, __pyx_L1_error)
 
   /* "cyroot/_check_args.pyx":67
  * 
  * # noinspection DuplicatedCode
- * def _check_initial_vals_uniqueness(f_xs: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):             # <<<<<<<<<<<<<<
- *     if not len(f_xs):
+ * def _check_initial_vals_uniqueness(f_x0s: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):             # <<<<<<<<<<<<<<
+ *     if not len(f_x0s):
  *         raise ValueError('Empty.')
  */
-  __pyx_tuple__33 = PyTuple_Pack(3, __pyx_n_s_f_xs, __pyx_n_s_genexpr, __pyx_n_s_genexpr); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_tuple__33 = PyTuple_Pack(3, __pyx_n_s_f_x0s, __pyx_n_s_genexpr, __pyx_n_s_genexpr); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__33);
   __Pyx_GIVEREF(__pyx_tuple__33);
   __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cyroot__check_args_pyx, __pyx_n_s_check_initial_vals_uniqueness, 67, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 67, __pyx_L1_error)
 
   /* "View.MemoryView":287
  *         return self.name
  * 
@@ -24019,28 +24019,28 @@
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_check_stop_cond_args, __pyx_t_2) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "cyroot/_check_args.pyx":55
  * 
  * # noinspection DuplicatedCode
- * def _check_initial_guesses_uniqueness(xs: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):             # <<<<<<<<<<<<<<
- *     if not len(xs):
+ * def _check_initial_guesses_uniqueness(x0s: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):             # <<<<<<<<<<<<<<
+ *     if not len(x0s):
  *         raise ValueError('Empty.')
  */
   __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_6cyroot_11_check_args_5_check_initial_guesses_uniqueness, NULL, __pyx_n_s_cyroot__check_args); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 55, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_check_initial_guesses_uniquenes_2, __pyx_t_2) < 0) __PYX_ERR(0, 55, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "cyroot/_check_args.pyx":67
  * 
  * # noinspection DuplicatedCode
- * def _check_initial_vals_uniqueness(f_xs: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):             # <<<<<<<<<<<<<<
- *     if not len(f_xs):
+ * def _check_initial_vals_uniqueness(f_x0s: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):             # <<<<<<<<<<<<<<
+ *     if not len(f_x0s):
  *         raise ValueError('Empty.')
  */
   __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_6cyroot_11_check_args_7_check_initial_vals_uniqueness, NULL, __pyx_n_s_cyroot__check_args); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_check_initial_vals_uniqueness, __pyx_t_2) < 0) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
```

### Comparing `cy-root-1.0.1/cyroot/_check_args.pxd` & `cy-root-1.0.2/cyroot/_check_args.pxd`

 * *Files 4% similar despite different names*

```diff
@@ -62,30 +62,30 @@
         double prtol,
         double* precision,
         double* error,
         bint* converged,
         bint* optimal)
 
 cdef bint _check_stop_cond_scalar_initial_guesses(
-        double[:] xs,
-        double[:] f_xs,
+        double[:] x0s,
+        double[:] f_x0s,
         double etol,
         double ertol,
         double ptol,
         double prtol,
         double* r,
         double* f_r,
         double* precision,
         double* error,
         bint* converged,
         bint* optimal)
 
 cdef bint _check_stop_cond_vector_initial_guesses(
-        double[:, :] xs,
-        double[:, :] F_xs,
+        double[:, :] x0s,
+        double[:, :] F_x0s,
         double etol,
         double ertol,
         double ptol,
         double prtol,
         double[:] r,
         double[:] F_r,
         double* precision,
@@ -119,30 +119,30 @@
         double prtol,
         double* precision,
         double* error,
         bint* converged,
         bint* optimal)
 
 cdef bint _check_stop_cond_complex_scalar_initial_guesses(
-        double complex[:] xs,
-        double complex[:] f_xs,
+        double complex[:] x0s,
+        double complex[:] f_x0s,
         double etol,
         double ertol,
         double ptol,
         double prtol,
         double complex* r,
         double complex* f_r,
         double* precision,
         double* error,
         bint* converged,
         bint* optimal)
 
 cdef bint _check_stop_cond_complex_vector_initial_guesses(
-        double complex[:, :] xs,
-        double complex[:, :] F_xs,
+        double complex[:, :] x0s,
+        double complex[:, :] F_x0s,
         double etol,
         double ertol,
         double ptol,
         double prtol,
         double complex[:] r,
         double complex[:] F_r,
         double* precision,
```

### Comparing `cy-root-1.0.1/cyroot/_check_args.pyx` & `cy-root-1.0.2/cyroot/_check_args.pyx`

 * *Files 5% similar despite different names*

```diff
@@ -48,37 +48,37 @@
 
     if etol == ertol == ptol == prtol == max_iter == 0:
         raise ValueError(f'Disabling both tolerances and max_iter will '
                          f'likely cause the algorithm to run indefinitely.')
     return etol, ertol, ptol, prtol, max_iter
 
 # noinspection DuplicatedCode
-def _check_initial_guesses_uniqueness(xs: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):
-    if not len(xs):
+def _check_initial_guesses_uniqueness(x0s: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):
+    if not len(x0s):
         raise ValueError('Empty.')
-    elif isinstance(xs[0], np.ndarray):
-        if np.unique(xs if isinstance(xs, np.ndarray) else
-                     np.stack(xs), axis=0).shape[0] < len(xs):
+    elif isinstance(x0s[0], np.ndarray):
+        if np.unique(x0s if isinstance(x0s, np.ndarray) else
+                     np.stack(x0s), axis=0).shape[0] < len(x0s):
             raise ValueError(f'Initial guesses must be unique. Got:\n' +
-                             '\n'.join(repr(_) for _ in xs))
-    elif len(set(xs)) < len(xs):
-        raise ValueError(f'Initial guesses must be unique. Got {xs}.')
+                             '\n'.join(repr(_) for _ in x0s))
+    elif len(set(x0s)) < len(x0s):
+        raise ValueError(f'Initial guesses must be unique. Got {x0s}.')
 
 # noinspection DuplicatedCode
-def _check_initial_vals_uniqueness(f_xs: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):
-    if not len(f_xs):
+def _check_initial_vals_uniqueness(f_x0s: Union[Sequence[Union[float, complex, np.ndarray]], np.ndarray]):
+    if not len(f_x0s):
         raise ValueError('Empty.')
-    elif isinstance(f_xs[0], np.ndarray):
-        if np.unique(f_xs if isinstance(f_xs, np.ndarray) else
-                     np.stack(f_xs), axis=0).shape[0] < len(f_xs):
+    elif isinstance(f_x0s[0], np.ndarray):
+        if np.unique(f_x0s if isinstance(f_x0s, np.ndarray) else
+                     np.stack(f_x0s), axis=0).shape[0] < len(f_x0s):
             raise ValueError('Initial guesses\' values must be unique. '
-                             'Got:\n' + '\n'.join(repr(_) for _ in f_xs))
-    elif len(set(f_xs)) < len(f_xs):
+                             'Got:\n' + '\n'.join(repr(_) for _ in f_x0s))
+    elif len(set(f_x0s)) < len(f_x0s):
         raise ValueError('Initial guesses\' values must be unique. '
-                         f'Got {f_xs}.')
+                         f'Got {f_x0s}.')
 
 ################################################################################
 # Bracketing methods
 ################################################################################
 # noinspection DuplicatedCode
 cdef inline bint _check_stop_cond_scalar_bracket(
         double a,
@@ -172,74 +172,74 @@
     error[0] = vops.max(vops.fabs(F_x0))
     optimal[0] = sops.isclose(0, error[0], ertol, etol)
     converged[0] = optimal[0]
     return optimal[0]
 
 # noinspection DuplicatedCode
 cdef inline bint _check_stop_cond_scalar_initial_guesses(
-        double[:] xs,
-        double[:] f_xs,
+        double[:] x0s,
+        double[:] f_x0s,
         double etol,
         double ertol,
         double ptol,
         double prtol,
         double* r,
         double* f_r,
         double* precision,
         double* error,
         bint* converged,
         bint* optimal):
     """Check if stop condition is already met."""
-    if xs.shape[0] == 0:
+    if x0s.shape[0] == 0:
         raise ValueError('Empty sequence.')
-    if xs.shape[0] == 1:
-        r[0], f_r[0] = xs[0], f_xs[0]
+    if x0s.shape[0] == 1:
+        r[0], f_r[0] = x0s[0], f_x0s[0]
         precision[0] = math.INFINITY
-        error[0] = math.fabs(f_xs[0])
+        error[0] = math.fabs(f_x0s[0])
         optimal[0] = sops.isclose(0, error[0], ertol, etol)
         converged[0] = optimal[0]
         return optimal[0]
-    cdef double[:] errors = vops.fabs(f_xs)
+    cdef double[:] errors = vops.fabs(f_x0s)
     cdef unsigned long best_i = vops.argmin(errors)
-    r[0], f_r[0] = xs[best_i], f_xs[best_i]
+    r[0], f_r[0] = x0s[best_i], f_x0s[best_i]
     error[0] = errors[best_i]
-    precision[0] = vops.max(xs) - vops.min(xs)
+    precision[0] = vops.max(x0s) - vops.min(x0s)
     optimal[0] = sops.isclose(0, error[0], ertol, etol)
     converged[0] = sops.isclose(0, precision[0], prtol, ptol) or optimal[0]
     return optimal[0] or sops.isclose(0, precision[0], prtol, ptol)
 
 # noinspection DuplicatedCode
 cdef inline bint _check_stop_cond_vector_initial_guesses(
-        double[:, :] xs,
-        double[:, :] F_xs,
+        double[:, :] x0s,
+        double[:, :] F_x0s,
         double etol,
         double ertol,
         double ptol,
         double prtol,
         double[:] r,
         double[:] F_r,
         double* precision,
         double* error,
         bint* converged,
         bint* optimal):
     """Check if stop condition is already met."""
-    if xs.shape[0] == 0:
+    if x0s.shape[0] == 0:
         raise ValueError('Empty sequence.')
-    if xs.shape[0] == 1:
-        r[:], F_r[:] = xs[0], F_xs[0]
+    if x0s.shape[0] == 1:
+        r[:], F_r[:] = x0s[0], F_x0s[0]
         precision[0] = math.INFINITY
-        error[0] = vops.max(vops.fabs(F_xs[0]))
+        error[0] = vops.max(vops.fabs(F_x0s[0]))
         optimal[0] = sops.isclose(0, error[0], ertol, etol)
         converged[0] = optimal[0]
         return optimal[0]
-    cdef double[:] errors = np.abs(F_xs).max(1)
+    cdef double[:] errors = np.abs(F_x0s).max(1)
     cdef unsigned long best_i = vops.argmin(errors)
-    r[:], F_r[:] = xs[best_i], F_xs[best_i]
+    r[:], F_r[:] = x0s[best_i], F_x0s[best_i]
     error[0] = errors[best_i]
-    precision[0] = vops.max(np.max(xs, 0) - np.min(xs, 0))
+    precision[0] = vops.max(np.max(x0s, 0) - np.min(x0s, 0))
     optimal[0] = sops.isclose(0, error[0], ertol, etol)
     converged[0] = sops.isclose(0, precision[0], prtol, ptol) or optimal[0]
     return optimal[0] or sops.isclose(0, precision[0], prtol, ptol)
 
 # --------------------------------
 # Double Complex
 # --------------------------------
@@ -279,72 +279,72 @@
     error[0] = vops.max(vops.cabs(F_x0))
     optimal[0] = sops.isclose(0, error[0], ertol, etol)
     converged[0] = optimal[0]
     return optimal[0]
 
 # noinspection DuplicatedCode
 cdef inline bint _check_stop_cond_complex_scalar_initial_guesses(
-        double complex[:] xs,
-        double complex[:] f_xs,
+        double complex[:] x0s,
+        double complex[:] f_x0s,
         double etol,
         double ertol,
         double ptol,
         double prtol,
         double complex* r,
         double complex* f_r,
         double* precision,
         double* error,
         bint* converged,
         bint* optimal):
     """Check if stop condition is already met."""
-    if xs.shape[0] == 0:
+    if x0s.shape[0] == 0:
         raise ValueError('Empty sequence.')
-    if xs.shape[0] == 1:
-        r[0], f_r[0] = xs[0], f_xs[0]
+    if x0s.shape[0] == 1:
+        r[0], f_r[0] = x0s[0], f_x0s[0]
         precision[0] = math.INFINITY
-        error[0] = sops.cabs(f_xs[0])
+        error[0] = sops.cabs(f_x0s[0])
         optimal[0] = sops.isclose(0, error[0], ertol, etol)
         converged[0] = optimal[0]
         return optimal[0]
-    cdef double[:] errors = vops.cabs(f_xs)
+    cdef double[:] errors = vops.cabs(f_x0s)
     cdef unsigned long best_i = vops.argmin(errors)
-    r[0], f_r[0] = xs[best_i], f_xs[best_i]
+    r[0], f_r[0] = x0s[best_i], f_x0s[best_i]
     error[0] = errors[best_i]
-    cdef double[:] xs_abs = vops.cabs(xs)
+    cdef double[:] xs_abs = vops.cabs(x0s)
     precision[0] = vops.max(xs_abs) - vops.min(xs_abs)
     optimal[0] = sops.isclose(0, error[0], ertol, etol)
     converged[0] = sops.isclose(0, precision[0], prtol, ptol) or optimal[0]
     return optimal[0] or sops.isclose(0, precision[0], prtol, ptol)
 
 # noinspection DuplicatedCode
 cdef inline bint _check_stop_cond_complex_vector_initial_guesses(
-        double complex[:, :] xs,
-        double complex[:, :] F_xs,
+        double complex[:, :] x0s,
+        double complex[:, :] F_x0s,
         double etol,
         double ertol,
         double ptol,
         double prtol,
         double complex[:] r,
         double complex[:] F_r,
         double* precision,
         double* error,
         bint* converged,
         bint* optimal):
     """Check if stop condition is already met."""
-    if xs.shape[0] == 0:
+    if x0s.shape[0] == 0:
         raise ValueError('Empty sequence.')
-    if xs.shape[0] == 1:
-        r[:], F_r[:] = xs[0], F_xs[0]
+    if x0s.shape[0] == 1:
+        r[:], F_r[:] = x0s[0], F_x0s[0]
         precision[0] = math.INFINITY
-        error[0] = vops.max(vops.cabs(F_xs[0]))
+        error[0] = vops.max(vops.cabs(F_x0s[0]))
         optimal[0] = sops.isclose(0, error[0], ertol, etol)
         converged[0] = optimal[0]
         return optimal[0]
-    cdef double[:] errors = np.abs(F_xs).max(1)
+    cdef double[:] errors = np.abs(F_x0s).max(1)
     cdef unsigned long best_i = vops.argmin(errors)
-    r[:], F_r[:] = xs[best_i], F_xs[best_i]
+    r[:], F_r[:] = x0s[best_i], F_x0s[best_i]
     error[0] = errors[best_i]
-    cdef double[:, :] xs_abs = np.abs(xs)
+    cdef double[:, :] xs_abs = np.abs(x0s)
     precision[0] = vops.max(np.max(xs_abs, 0) - np.min(xs_abs, 0))
     optimal[0] = sops.isclose(0, error[0], ertol, etol)
     converged[0] = sops.isclose(0, precision[0], prtol, ptol) or optimal[0]
     return optimal[0] or sops.isclose(0, precision[0], prtol, ptol)
```

### Comparing `cy-root-1.0.1/cyroot/_defaults.py` & `cy-root-1.0.2/cyroot/_defaults.py`

 * *Files identical despite different names*

### Comparing `cy-root-1.0.1/cyroot/_return_types.py` & `cy-root-1.0.2/cyroot/_return_types.py`

 * *Files identical despite different names*

### Comparing `cy-root-1.0.1/cyroot/fptr.cpp` & `cy-root-1.0.2/cyroot/fptr.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
             "cyroot",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include",
             "cyroot/ops",
             "cyroot/utils"
         ],
         "language": "c++",
         "name": "cyroot.fptr",
         "sources": [
             "cyroot/fptr.pyx"
@@ -1132,195 +1132,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1373,42 +1373,42 @@
 struct __pyx_obj_6cyroot_4fptr_CyNdArrayFPtr;
 struct __pyx_obj_6cyroot_4fptr_PyNdArrayFPtr;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -12740,15 +12740,15 @@
   __Pyx_AddTraceback("cyroot.fptr.PyNdArrayFPtr.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -12757,29 +12757,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -12790,15 +12790,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -12807,29 +12807,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -12840,15 +12840,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -12857,29 +12857,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -12890,15 +12890,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -12907,29 +12907,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -12940,15 +12940,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -12957,29 +12957,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -12990,212 +12990,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -13211,15 +13211,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -13227,53 +13227,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 942, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__46, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 944, __pyx_L5_except_error)
@@ -13281,30 +13281,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -13319,15 +13319,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -13343,15 +13343,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -13359,53 +13359,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 948, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__47, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 950, __pyx_L5_except_error)
@@ -13413,30 +13413,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -13451,15 +13451,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -13475,15 +13475,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -13491,53 +13491,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 954, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__47, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 956, __pyx_L5_except_error)
@@ -13545,30 +13545,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -13583,176 +13583,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -30465,26 +30465,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__45 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__45);
   __Pyx_GIVEREF(__pyx_tuple__45);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__46 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__46)) __PYX_ERR(3, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__46);
   __Pyx_GIVEREF(__pyx_tuple__46);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__47 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__47)) __PYX_ERR(3, 950, __pyx_L1_error)
```

### Comparing `cy-root-1.0.1/cyroot/fptr.pxd` & `cy-root-1.0.2/cyroot/fptr.pxd`

 * *Files identical despite different names*

### Comparing `cy-root-1.0.1/cyroot/fptr.pyx` & `cy-root-1.0.2/cyroot/fptr.pyx`

 * *Files identical despite different names*

### Comparing `cy-root-1.0.1/cyroot/ops/matrix_ops.cpp` & `cy-root-1.0.2/cyroot/ops/matrix_ops.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
             "cyroot",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include",
             "cyroot/ops",
             "cyroot/utils"
         ],
         "language": "c++",
         "name": "cyroot.ops.matrix_ops",
         "sources": [
             "cyroot/ops/matrix_ops.pyx"
@@ -1059,195 +1059,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1274,42 +1274,42 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -3058,15 +3058,15 @@
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_A_inv);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3075,29 +3075,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3108,15 +3108,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3125,29 +3125,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3158,15 +3158,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3175,29 +3175,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3208,15 +3208,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3225,29 +3225,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3258,15 +3258,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3275,29 +3275,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3308,212 +3308,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3529,15 +3529,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -3545,53 +3545,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
@@ -3599,30 +3599,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3637,15 +3637,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3661,15 +3661,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3677,53 +3677,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
@@ -3731,30 +3731,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3769,15 +3769,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3793,15 +3793,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3809,53 +3809,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
@@ -3863,30 +3863,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3901,176 +3901,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -4163,26 +4163,26 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 950, __pyx_L1_error)
@@ -4571,15 +4571,15 @@
  * # cython: initializedcheck = False
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
```

### Comparing `cy-root-1.0.1/cyroot/ops/matrix_ops.pyx` & `cy-root-1.0.2/cyroot/ops/matrix_ops.pyx`

 * *Files identical despite different names*

### Comparing `cy-root-1.0.1/cyroot/ops/scalar_ops.cpp` & `cy-root-1.0.2/cyroot/ops/scalar_ops.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "include_dirs": [
             "cyroot",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include",
             "cyroot/ops",
             "cyroot/utils"
         ],
         "language": "c++",
         "name": "cyroot.ops.scalar_ops",
         "sources": [
             "cyroot/ops/scalar_ops.pyx"
@@ -1061,28 +1061,28 @@
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_cisclose;
 
 /* "cyroot/ops/scalar_ops.pxd":18
  *     double complex
  * 
  * cdef bint isclose(double a, double b, double rtol=*, double atol=*) nogil             # <<<<<<<<<<<<<<
  * cdef bint cisclose(double complex a, double complex b, double rtol=*, double atol=*) nogil
- * 
+ * cdef real min(real a, real b) nogil
  */
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_isclose {
   int __pyx_n;
   double rtol;
   double atol;
 };
 
 /* "cyroot/ops/scalar_ops.pxd":19
  * 
  * cdef bint isclose(double a, double b, double rtol=*, double atol=*) nogil
  * cdef bint cisclose(double complex a, double complex b, double rtol=*, double atol=*) nogil             # <<<<<<<<<<<<<<
- * 
- * cdef extern from '<math.h>' nogil:
+ * cdef real min(real a, real b) nogil
+ * cdef real max(real a, real b) nogil
  */
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_cisclose {
   int __pyx_n;
   double rtol;
   double atol;
 };
 
@@ -1344,14 +1344,26 @@
 
 /* Module declarations from 'libc' */
 
 /* Module declarations from 'libc.math' */
 
 /* Module declarations from 'cyroot.ops.scalar_ops' */
 static CYTHON_INLINE int __pyx_f_6cyroot_3ops_10scalar_ops_isclose(double, double, struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_isclose *__pyx_optional_args); /*proto*/
+static CYTHON_INLINE int __pyx_fuse_0__pyx_f_6cyroot_3ops_10scalar_ops_min(int, int); /*proto*/
+static CYTHON_INLINE unsigned int __pyx_fuse_1__pyx_f_6cyroot_3ops_10scalar_ops_min(unsigned int, unsigned int); /*proto*/
+static CYTHON_INLINE long __pyx_fuse_2__pyx_f_6cyroot_3ops_10scalar_ops_min(long, long); /*proto*/
+static CYTHON_INLINE unsigned long __pyx_fuse_3__pyx_f_6cyroot_3ops_10scalar_ops_min(unsigned long, unsigned long); /*proto*/
+static CYTHON_INLINE float __pyx_fuse_4__pyx_f_6cyroot_3ops_10scalar_ops_min(float, float); /*proto*/
+static CYTHON_INLINE double __pyx_fuse_5__pyx_f_6cyroot_3ops_10scalar_ops_min(double, double); /*proto*/
+static CYTHON_INLINE int __pyx_fuse_0__pyx_f_6cyroot_3ops_10scalar_ops_max(int, int); /*proto*/
+static CYTHON_INLINE unsigned int __pyx_fuse_1__pyx_f_6cyroot_3ops_10scalar_ops_max(unsigned int, unsigned int); /*proto*/
+static CYTHON_INLINE long __pyx_fuse_2__pyx_f_6cyroot_3ops_10scalar_ops_max(long, long); /*proto*/
+static CYTHON_INLINE unsigned long __pyx_fuse_3__pyx_f_6cyroot_3ops_10scalar_ops_max(unsigned long, unsigned long); /*proto*/
+static CYTHON_INLINE float __pyx_fuse_4__pyx_f_6cyroot_3ops_10scalar_ops_max(float, float); /*proto*/
+static CYTHON_INLINE double __pyx_fuse_5__pyx_f_6cyroot_3ops_10scalar_ops_max(double, double); /*proto*/
 #define __Pyx_MODULE_NAME "cyroot.ops.scalar_ops"
 extern int __pyx_module_is_main_cyroot__ops__scalar_ops;
 int __pyx_module_is_main_cyroot__ops__scalar_ops = 0;
 
 /* Implementation of 'cyroot.ops.scalar_ops' */
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
@@ -1456,14 +1468,15 @@
 }
 
 /* "cyroot/ops/scalar_ops.pyx":14
  *     return math.fabs(a - b) <= atol + rtol * math.fabs(b)
  * 
  * cdef inline bint cisclose(double complex a, double complex b, double rtol=1e-5, double atol=1e-8) nogil:             # <<<<<<<<<<<<<<
  *     return isclose(a.real, b.real, rtol, atol) and isclose(a.imag, b.imag, rtol, atol)
+ * 
  */
 
 static CYTHON_INLINE int __pyx_f_6cyroot_3ops_10scalar_ops_cisclose(__pyx_t_double_complex __pyx_v_a, __pyx_t_double_complex __pyx_v_b, struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_cisclose *__pyx_optional_args) {
   double __pyx_v_rtol = ((double)1e-5);
   double __pyx_v_atol = ((double)1e-8);
   int __pyx_r;
   int __pyx_t_1;
@@ -1479,14 +1492,16 @@
     }
   }
 
   /* "cyroot/ops/scalar_ops.pyx":15
  * 
  * cdef inline bint cisclose(double complex a, double complex b, double rtol=1e-5, double atol=1e-8) nogil:
  *     return isclose(a.real, b.real, rtol, atol) and isclose(a.imag, b.imag, rtol, atol)             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline real min(real a, real b) nogil:
  */
   __pyx_t_3.__pyx_n = 2;
   __pyx_t_3.rtol = __pyx_v_rtol;
   __pyx_t_3.atol = __pyx_v_atol;
   __pyx_t_2 = __pyx_f_6cyroot_3ops_10scalar_ops_isclose(__Pyx_CREAL(__pyx_v_a), __Pyx_CREAL(__pyx_v_b), &__pyx_t_3); 
   __pyx_t_4 = (__pyx_t_2 != 0);
   if (__pyx_t_4) {
@@ -1505,14 +1520,396 @@
   goto __pyx_L0;
 
   /* "cyroot/ops/scalar_ops.pyx":14
  *     return math.fabs(a - b) <= atol + rtol * math.fabs(b)
  * 
  * cdef inline bint cisclose(double complex a, double complex b, double rtol=1e-5, double atol=1e-8) nogil:             # <<<<<<<<<<<<<<
  *     return isclose(a.real, b.real, rtol, atol) and isclose(a.imag, b.imag, rtol, atol)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "cyroot/ops/scalar_ops.pyx":17
+ *     return isclose(a.real, b.real, rtol, atol) and isclose(a.imag, b.imag, rtol, atol)
+ * 
+ * cdef inline real min(real a, real b) nogil:             # <<<<<<<<<<<<<<
+ *     return b if a > b else a
+ * 
+ */
+
+static CYTHON_INLINE int __pyx_fuse_0__pyx_f_6cyroot_3ops_10scalar_ops_min(int __pyx_v_a, int __pyx_v_b) {
+  int __pyx_r;
+  int __pyx_t_1;
+
+  /* "cyroot/ops/scalar_ops.pyx":18
+ * 
+ * cdef inline real min(real a, real b) nogil:
+ *     return b if a > b else a             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline real max(real a, real b) nogil:
+ */
+  if (((__pyx_v_a > __pyx_v_b) != 0)) {
+    __pyx_t_1 = __pyx_v_b;
+  } else {
+    __pyx_t_1 = __pyx_v_a;
+  }
+  __pyx_r = __pyx_t_1;
+  goto __pyx_L0;
+
+  /* "cyroot/ops/scalar_ops.pyx":17
+ *     return isclose(a.real, b.real, rtol, atol) and isclose(a.imag, b.imag, rtol, atol)
+ * 
+ * cdef inline real min(real a, real b) nogil:             # <<<<<<<<<<<<<<
+ *     return b if a > b else a
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+static CYTHON_INLINE unsigned int __pyx_fuse_1__pyx_f_6cyroot_3ops_10scalar_ops_min(unsigned int __pyx_v_a, unsigned int __pyx_v_b) {
+  unsigned int __pyx_r;
+  unsigned int __pyx_t_1;
+
+  /* "cyroot/ops/scalar_ops.pyx":18
+ * 
+ * cdef inline real min(real a, real b) nogil:
+ *     return b if a > b else a             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline real max(real a, real b) nogil:
+ */
+  if (((__pyx_v_a > __pyx_v_b) != 0)) {
+    __pyx_t_1 = __pyx_v_b;
+  } else {
+    __pyx_t_1 = __pyx_v_a;
+  }
+  __pyx_r = __pyx_t_1;
+  goto __pyx_L0;
+
+  /* "cyroot/ops/scalar_ops.pyx":17
+ *     return isclose(a.real, b.real, rtol, atol) and isclose(a.imag, b.imag, rtol, atol)
+ * 
+ * cdef inline real min(real a, real b) nogil:             # <<<<<<<<<<<<<<
+ *     return b if a > b else a
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+static CYTHON_INLINE long __pyx_fuse_2__pyx_f_6cyroot_3ops_10scalar_ops_min(long __pyx_v_a, long __pyx_v_b) {
+  long __pyx_r;
+  long __pyx_t_1;
+
+  /* "cyroot/ops/scalar_ops.pyx":18
+ * 
+ * cdef inline real min(real a, real b) nogil:
+ *     return b if a > b else a             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline real max(real a, real b) nogil:
+ */
+  if (((__pyx_v_a > __pyx_v_b) != 0)) {
+    __pyx_t_1 = __pyx_v_b;
+  } else {
+    __pyx_t_1 = __pyx_v_a;
+  }
+  __pyx_r = __pyx_t_1;
+  goto __pyx_L0;
+
+  /* "cyroot/ops/scalar_ops.pyx":17
+ *     return isclose(a.real, b.real, rtol, atol) and isclose(a.imag, b.imag, rtol, atol)
+ * 
+ * cdef inline real min(real a, real b) nogil:             # <<<<<<<<<<<<<<
+ *     return b if a > b else a
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+static CYTHON_INLINE unsigned long __pyx_fuse_3__pyx_f_6cyroot_3ops_10scalar_ops_min(unsigned long __pyx_v_a, unsigned long __pyx_v_b) {
+  unsigned long __pyx_r;
+  unsigned long __pyx_t_1;
+
+  /* "cyroot/ops/scalar_ops.pyx":18
+ * 
+ * cdef inline real min(real a, real b) nogil:
+ *     return b if a > b else a             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline real max(real a, real b) nogil:
+ */
+  if (((__pyx_v_a > __pyx_v_b) != 0)) {
+    __pyx_t_1 = __pyx_v_b;
+  } else {
+    __pyx_t_1 = __pyx_v_a;
+  }
+  __pyx_r = __pyx_t_1;
+  goto __pyx_L0;
+
+  /* "cyroot/ops/scalar_ops.pyx":17
+ *     return isclose(a.real, b.real, rtol, atol) and isclose(a.imag, b.imag, rtol, atol)
+ * 
+ * cdef inline real min(real a, real b) nogil:             # <<<<<<<<<<<<<<
+ *     return b if a > b else a
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+static CYTHON_INLINE float __pyx_fuse_4__pyx_f_6cyroot_3ops_10scalar_ops_min(float __pyx_v_a, float __pyx_v_b) {
+  float __pyx_r;
+  float __pyx_t_1;
+
+  /* "cyroot/ops/scalar_ops.pyx":18
+ * 
+ * cdef inline real min(real a, real b) nogil:
+ *     return b if a > b else a             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline real max(real a, real b) nogil:
+ */
+  if (((__pyx_v_a > __pyx_v_b) != 0)) {
+    __pyx_t_1 = __pyx_v_b;
+  } else {
+    __pyx_t_1 = __pyx_v_a;
+  }
+  __pyx_r = __pyx_t_1;
+  goto __pyx_L0;
+
+  /* "cyroot/ops/scalar_ops.pyx":17
+ *     return isclose(a.real, b.real, rtol, atol) and isclose(a.imag, b.imag, rtol, atol)
+ * 
+ * cdef inline real min(real a, real b) nogil:             # <<<<<<<<<<<<<<
+ *     return b if a > b else a
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+static CYTHON_INLINE double __pyx_fuse_5__pyx_f_6cyroot_3ops_10scalar_ops_min(double __pyx_v_a, double __pyx_v_b) {
+  double __pyx_r;
+  double __pyx_t_1;
+
+  /* "cyroot/ops/scalar_ops.pyx":18
+ * 
+ * cdef inline real min(real a, real b) nogil:
+ *     return b if a > b else a             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline real max(real a, real b) nogil:
+ */
+  if (((__pyx_v_a > __pyx_v_b) != 0)) {
+    __pyx_t_1 = __pyx_v_b;
+  } else {
+    __pyx_t_1 = __pyx_v_a;
+  }
+  __pyx_r = __pyx_t_1;
+  goto __pyx_L0;
+
+  /* "cyroot/ops/scalar_ops.pyx":17
+ *     return isclose(a.real, b.real, rtol, atol) and isclose(a.imag, b.imag, rtol, atol)
+ * 
+ * cdef inline real min(real a, real b) nogil:             # <<<<<<<<<<<<<<
+ *     return b if a > b else a
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "cyroot/ops/scalar_ops.pyx":20
+ *     return b if a > b else a
+ * 
+ * cdef inline real max(real a, real b) nogil:             # <<<<<<<<<<<<<<
+ *     return b if a < b else a
+ */
+
+static CYTHON_INLINE int __pyx_fuse_0__pyx_f_6cyroot_3ops_10scalar_ops_max(int __pyx_v_a, int __pyx_v_b) {
+  int __pyx_r;
+  int __pyx_t_1;
+
+  /* "cyroot/ops/scalar_ops.pyx":21
+ * 
+ * cdef inline real max(real a, real b) nogil:
+ *     return b if a < b else a             # <<<<<<<<<<<<<<
+ */
+  if (((__pyx_v_a < __pyx_v_b) != 0)) {
+    __pyx_t_1 = __pyx_v_b;
+  } else {
+    __pyx_t_1 = __pyx_v_a;
+  }
+  __pyx_r = __pyx_t_1;
+  goto __pyx_L0;
+
+  /* "cyroot/ops/scalar_ops.pyx":20
+ *     return b if a > b else a
+ * 
+ * cdef inline real max(real a, real b) nogil:             # <<<<<<<<<<<<<<
+ *     return b if a < b else a
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+static CYTHON_INLINE unsigned int __pyx_fuse_1__pyx_f_6cyroot_3ops_10scalar_ops_max(unsigned int __pyx_v_a, unsigned int __pyx_v_b) {
+  unsigned int __pyx_r;
+  unsigned int __pyx_t_1;
+
+  /* "cyroot/ops/scalar_ops.pyx":21
+ * 
+ * cdef inline real max(real a, real b) nogil:
+ *     return b if a < b else a             # <<<<<<<<<<<<<<
+ */
+  if (((__pyx_v_a < __pyx_v_b) != 0)) {
+    __pyx_t_1 = __pyx_v_b;
+  } else {
+    __pyx_t_1 = __pyx_v_a;
+  }
+  __pyx_r = __pyx_t_1;
+  goto __pyx_L0;
+
+  /* "cyroot/ops/scalar_ops.pyx":20
+ *     return b if a > b else a
+ * 
+ * cdef inline real max(real a, real b) nogil:             # <<<<<<<<<<<<<<
+ *     return b if a < b else a
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+static CYTHON_INLINE long __pyx_fuse_2__pyx_f_6cyroot_3ops_10scalar_ops_max(long __pyx_v_a, long __pyx_v_b) {
+  long __pyx_r;
+  long __pyx_t_1;
+
+  /* "cyroot/ops/scalar_ops.pyx":21
+ * 
+ * cdef inline real max(real a, real b) nogil:
+ *     return b if a < b else a             # <<<<<<<<<<<<<<
+ */
+  if (((__pyx_v_a < __pyx_v_b) != 0)) {
+    __pyx_t_1 = __pyx_v_b;
+  } else {
+    __pyx_t_1 = __pyx_v_a;
+  }
+  __pyx_r = __pyx_t_1;
+  goto __pyx_L0;
+
+  /* "cyroot/ops/scalar_ops.pyx":20
+ *     return b if a > b else a
+ * 
+ * cdef inline real max(real a, real b) nogil:             # <<<<<<<<<<<<<<
+ *     return b if a < b else a
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+static CYTHON_INLINE unsigned long __pyx_fuse_3__pyx_f_6cyroot_3ops_10scalar_ops_max(unsigned long __pyx_v_a, unsigned long __pyx_v_b) {
+  unsigned long __pyx_r;
+  unsigned long __pyx_t_1;
+
+  /* "cyroot/ops/scalar_ops.pyx":21
+ * 
+ * cdef inline real max(real a, real b) nogil:
+ *     return b if a < b else a             # <<<<<<<<<<<<<<
+ */
+  if (((__pyx_v_a < __pyx_v_b) != 0)) {
+    __pyx_t_1 = __pyx_v_b;
+  } else {
+    __pyx_t_1 = __pyx_v_a;
+  }
+  __pyx_r = __pyx_t_1;
+  goto __pyx_L0;
+
+  /* "cyroot/ops/scalar_ops.pyx":20
+ *     return b if a > b else a
+ * 
+ * cdef inline real max(real a, real b) nogil:             # <<<<<<<<<<<<<<
+ *     return b if a < b else a
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+static CYTHON_INLINE float __pyx_fuse_4__pyx_f_6cyroot_3ops_10scalar_ops_max(float __pyx_v_a, float __pyx_v_b) {
+  float __pyx_r;
+  float __pyx_t_1;
+
+  /* "cyroot/ops/scalar_ops.pyx":21
+ * 
+ * cdef inline real max(real a, real b) nogil:
+ *     return b if a < b else a             # <<<<<<<<<<<<<<
+ */
+  if (((__pyx_v_a < __pyx_v_b) != 0)) {
+    __pyx_t_1 = __pyx_v_b;
+  } else {
+    __pyx_t_1 = __pyx_v_a;
+  }
+  __pyx_r = __pyx_t_1;
+  goto __pyx_L0;
+
+  /* "cyroot/ops/scalar_ops.pyx":20
+ *     return b if a > b else a
+ * 
+ * cdef inline real max(real a, real b) nogil:             # <<<<<<<<<<<<<<
+ *     return b if a < b else a
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+static CYTHON_INLINE double __pyx_fuse_5__pyx_f_6cyroot_3ops_10scalar_ops_max(double __pyx_v_a, double __pyx_v_b) {
+  double __pyx_r;
+  double __pyx_t_1;
+
+  /* "cyroot/ops/scalar_ops.pyx":21
+ * 
+ * cdef inline real max(real a, real b) nogil:
+ *     return b if a < b else a             # <<<<<<<<<<<<<<
+ */
+  if (((__pyx_v_a < __pyx_v_b) != 0)) {
+    __pyx_t_1 = __pyx_v_b;
+  } else {
+    __pyx_t_1 = __pyx_v_a;
+  }
+  __pyx_r = __pyx_t_1;
+  goto __pyx_L0;
+
+  /* "cyroot/ops/scalar_ops.pyx":20
+ *     return b if a > b else a
+ * 
+ * cdef inline real max(real a, real b) nogil:             # <<<<<<<<<<<<<<
+ *     return b if a < b else a
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
@@ -1615,14 +2012,26 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_export_code", 0);
   /*--- Function export code ---*/
   if (__Pyx_ExportFunction("isclose", (void (*)(void))__pyx_f_6cyroot_3ops_10scalar_ops_isclose, "int (double, double, struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_isclose *__pyx_optional_args)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("cisclose", (void (*)(void))__pyx_f_6cyroot_3ops_10scalar_ops_cisclose, "int (__pyx_t_double_complex, __pyx_t_double_complex, struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_cisclose *__pyx_optional_args)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("__pyx_fuse_0min", (void (*)(void))__pyx_fuse_0__pyx_f_6cyroot_3ops_10scalar_ops_min, "int (int, int)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("__pyx_fuse_1min", (void (*)(void))__pyx_fuse_1__pyx_f_6cyroot_3ops_10scalar_ops_min, "unsigned int (unsigned int, unsigned int)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("__pyx_fuse_2min", (void (*)(void))__pyx_fuse_2__pyx_f_6cyroot_3ops_10scalar_ops_min, "long (long, long)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("__pyx_fuse_3min", (void (*)(void))__pyx_fuse_3__pyx_f_6cyroot_3ops_10scalar_ops_min, "unsigned long (unsigned long, unsigned long)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("__pyx_fuse_4min", (void (*)(void))__pyx_fuse_4__pyx_f_6cyroot_3ops_10scalar_ops_min, "float (float, float)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("__pyx_fuse_5min", (void (*)(void))__pyx_fuse_5__pyx_f_6cyroot_3ops_10scalar_ops_min, "double (double, double)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("__pyx_fuse_0max", (void (*)(void))__pyx_fuse_0__pyx_f_6cyroot_3ops_10scalar_ops_max, "int (int, int)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("__pyx_fuse_1max", (void (*)(void))__pyx_fuse_1__pyx_f_6cyroot_3ops_10scalar_ops_max, "unsigned int (unsigned int, unsigned int)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("__pyx_fuse_2max", (void (*)(void))__pyx_fuse_2__pyx_f_6cyroot_3ops_10scalar_ops_max, "long (long, long)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("__pyx_fuse_3max", (void (*)(void))__pyx_fuse_3__pyx_f_6cyroot_3ops_10scalar_ops_max, "unsigned long (unsigned long, unsigned long)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("__pyx_fuse_4max", (void (*)(void))__pyx_fuse_4__pyx_f_6cyroot_3ops_10scalar_ops_max, "float (float, float)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("__pyx_fuse_5max", (void (*)(void))__pyx_fuse_5__pyx_f_6cyroot_3ops_10scalar_ops_max, "double (double, double)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
```

### Comparing `cy-root-1.0.1/cyroot/ops/scalar_ops.pxd` & `cy-root-1.0.2/cyroot/ops/scalar_ops.pxd`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     unsigned long
     float
     double
     double complex
 
 cdef bint isclose(double a, double b, double rtol=*, double atol=*) nogil
 cdef bint cisclose(double complex a, double complex b, double rtol=*, double atol=*) nogil
+cdef real min(real a, real b) nogil
+cdef real max(real a, real b) nogil
 
 cdef extern from '<math.h>' nogil:
     double fabs(double)
     double sqrt(double)
 
 cdef extern from '<complex>' nogil:
     double cabs 'abs'(double complex)
```

### Comparing `cy-root-1.0.1/cyroot/ops/scalar_ops.pyx` & `cy-root-1.0.2/cyroot/ops/scalar_ops.pyx`

 * *Files 24% similar despite different names*

```diff
@@ -9,7 +9,13 @@
 cdef inline bint isclose(double a, double b, double rtol=1e-5, double atol=1e-8) nogil:
     if math.isinf(b) or math.isinf(a):
         return math.isinf(a) and math.isinf(b)
     return math.fabs(a - b) <= atol + rtol * math.fabs(b)
 
 cdef inline bint cisclose(double complex a, double complex b, double rtol=1e-5, double atol=1e-8) nogil:
     return isclose(a.real, b.real, rtol, atol) and isclose(a.imag, b.imag, rtol, atol)
+
+cdef inline real min(real a, real b) nogil:
+    return b if a > b else a
+
+cdef inline real max(real a, real b) nogil:
+    return b if a < b else a
```

### Comparing `cy-root-1.0.1/cyroot/ops/vector_ops.cpp` & `cy-root-1.0.2/cyroot/ops/vector_ops.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "include_dirs": [
             "cyroot",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include",
             "cyroot/ops",
             "cyroot/utils"
         ],
         "language": "c++",
         "name": "cyroot.ops.vector_ops",
         "sources": [
             "cyroot/ops/vector_ops.pyx"
@@ -1181,28 +1181,28 @@
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_cisclose;
 
 /* "scalar_ops.pxd":18
  *     double complex
  * 
  * cdef bint isclose(double a, double b, double rtol=*, double atol=*) nogil             # <<<<<<<<<<<<<<
  * cdef bint cisclose(double complex a, double complex b, double rtol=*, double atol=*) nogil
- * 
+ * cdef real min(real a, real b) nogil
  */
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_isclose {
   int __pyx_n;
   double rtol;
   double atol;
 };
 
 /* "scalar_ops.pxd":19
  * 
  * cdef bint isclose(double a, double b, double rtol=*, double atol=*) nogil
  * cdef bint cisclose(double complex a, double complex b, double rtol=*, double atol=*) nogil             # <<<<<<<<<<<<<<
- * 
- * cdef extern from '<math.h>' nogil:
+ * cdef real min(real a, real b) nogil
+ * cdef real max(real a, real b) nogil
  */
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_cisclose {
   int __pyx_n;
   double rtol;
   double atol;
 };
 struct __pyx_opt_args_6cyroot_3ops_10vector_ops_allclose;
```

### Comparing `cy-root-1.0.1/cyroot/ops/vector_ops.pxd` & `cy-root-1.0.2/cyroot/ops/vector_ops.pxd`

 * *Files identical despite different names*

### Comparing `cy-root-1.0.1/cyroot/ops/vector_ops.pyx` & `cy-root-1.0.2/cyroot/ops/vector_ops.pyx`

 * *Files identical despite different names*

### Comparing `cy-root-1.0.1/cyroot/scalar_bracketing.cpp` & `cy-root-1.0.2/cyroot/scalar_bracketing.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
             "cyroot",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include",
             "cyroot/ops",
             "cyroot/utils"
         ],
         "language": "c++",
         "name": "cyroot.scalar_bracketing",
         "sources": [
             "cyroot/scalar_bracketing.pyx"
@@ -1185,195 +1185,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1426,42 +1426,42 @@
 struct __pyx_obj_6cyroot_4fptr_CyNdArrayFPtr;
 struct __pyx_obj_6cyroot_4fptr_PyNdArrayFPtr;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1562,28 +1562,28 @@
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_cisclose;
 
 /* "scalar_ops.pxd":18
  *     double complex
  * 
  * cdef bint isclose(double a, double b, double rtol=*, double atol=*) nogil             # <<<<<<<<<<<<<<
  * cdef bint cisclose(double complex a, double complex b, double rtol=*, double atol=*) nogil
- * 
+ * cdef real min(real a, real b) nogil
  */
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_isclose {
   int __pyx_n;
   double rtol;
   double atol;
 };
 
 /* "scalar_ops.pxd":19
  * 
  * cdef bint isclose(double a, double b, double rtol=*, double atol=*) nogil
  * cdef bint cisclose(double complex a, double complex b, double rtol=*, double atol=*) nogil             # <<<<<<<<<<<<<<
- * 
- * cdef extern from '<math.h>' nogil:
+ * cdef real min(real a, real b) nogil
+ * cdef real max(real a, real b) nogil
  */
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_cisclose {
   int __pyx_n;
   double rtol;
   double atol;
 };
 struct __pyx_ctuple_ee55be__double__and_double__and_double__and_double__and_double__and_double__etc;
@@ -3783,14 +3783,20 @@
 static PyTypeObject *__pyx_ptype_6cyroot_4fptr_CyNdArrayFPtr = 0;
 static PyTypeObject *__pyx_ptype_6cyroot_4fptr_PyNdArrayFPtr = 0;
 
 /* Module declarations from 'cyroot.ops' */
 
 /* Module declarations from 'cyroot.ops.scalar_ops' */
 static int (*__pyx_f_6cyroot_3ops_10scalar_ops_isclose)(double, double, struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_isclose *__pyx_optional_args); /*proto*/
+static int (*__pyx_fuse_0__pyx_f_6cyroot_3ops_10scalar_ops_min)(int, int); /*proto*/
+static unsigned int (*__pyx_fuse_1__pyx_f_6cyroot_3ops_10scalar_ops_min)(unsigned int, unsigned int); /*proto*/
+static long (*__pyx_fuse_2__pyx_f_6cyroot_3ops_10scalar_ops_min)(long, long); /*proto*/
+static unsigned long (*__pyx_fuse_3__pyx_f_6cyroot_3ops_10scalar_ops_min)(unsigned long, unsigned long); /*proto*/
+static float (*__pyx_fuse_4__pyx_f_6cyroot_3ops_10scalar_ops_min)(float, float); /*proto*/
+static double (*__pyx_fuse_5__pyx_f_6cyroot_3ops_10scalar_ops_min)(double, double); /*proto*/
 
 /* Module declarations from 'cyroot.scalar_bracketing' */
 static PyTypeObject *__pyx_array_type = 0;
 static PyTypeObject *__pyx_MemviewEnum_type = 0;
 static PyTypeObject *__pyx_memoryview_type = 0;
 static PyTypeObject *__pyx_memoryviewslice_type = 0;
 static double __pyx_v_6cyroot_17scalar_bracketing_PHI;
@@ -16451,22 +16457,22 @@
   __Pyx_memviewslice __pyx_r = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_RefNannyDeclarations
   size_t __pyx_t_1;
   int __pyx_t_2;
   __Pyx_memviewslice __pyx_t_3 = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_t_4;
   unsigned int __pyx_t_5;
-  unsigned int __pyx_t_6;
-  unsigned int __pyx_t_7;
-  unsigned int __pyx_t_8;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
-  PyObject *__pyx_t_10 = NULL;
-  PyObject *__pyx_t_11 = NULL;
-  PyObject *__pyx_t_12 = NULL;
-  __Pyx_memviewslice __pyx_t_13 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  __Pyx_memviewslice __pyx_t_10 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  unsigned int __pyx_t_11;
+  unsigned int __pyx_t_12;
+  unsigned int __pyx_t_13;
   unsigned int __pyx_t_14;
   unsigned int __pyx_t_15;
   Py_ssize_t __pyx_t_16;
   Py_ssize_t __pyx_t_17;
   Py_ssize_t __pyx_t_18;
   size_t __pyx_t_19;
   size_t __pyx_t_20;
@@ -16497,24 +16503,24 @@
   __pyx_v_M = ((unsigned int)__pyx_t_1);
 
   /* "cyroot/scalar_bracketing.pyx":1186
  *     If forward is False, return f[c], f[b, c], f[a, b, c]."""
  *     cdef unsigned int i, j, M = <unsigned int> len(xs)
  *     if not forward:             # <<<<<<<<<<<<<<
  *         xs = xs[::-1]
- *     N = M if N == 0 else min(N, M)
+ *     N = M if N == 0 else sops.min(N, M)
  */
   __pyx_t_2 = ((!(__pyx_v_forward != 0)) != 0);
   if (__pyx_t_2) {
 
     /* "cyroot/scalar_bracketing.pyx":1187
  *     cdef unsigned int i, j, M = <unsigned int> len(xs)
  *     if not forward:
  *         xs = xs[::-1]             # <<<<<<<<<<<<<<
- *     N = M if N == 0 else min(N, M)
+ *     N = M if N == 0 else sops.min(N, M)
  *     cdef double[:, :] DD = view.array(shape=(M, N), itemsize=sizeof(double), format='d')
  */
     __pyx_t_3.data = __pyx_v_xs.data;
     __pyx_t_3.memview = __pyx_v_xs.memview;
     __PYX_INC_MEMVIEW(&__pyx_t_3, 0);
     __pyx_t_4 = -1;
     if (unlikely(__pyx_memoryview_slice_memviewslice(
@@ -16540,78 +16546,71 @@
     __pyx_t_3.data = NULL;
 
     /* "cyroot/scalar_bracketing.pyx":1186
  *     If forward is False, return f[c], f[b, c], f[a, b, c]."""
  *     cdef unsigned int i, j, M = <unsigned int> len(xs)
  *     if not forward:             # <<<<<<<<<<<<<<
  *         xs = xs[::-1]
- *     N = M if N == 0 else min(N, M)
+ *     N = M if N == 0 else sops.min(N, M)
  */
   }
 
   /* "cyroot/scalar_bracketing.pyx":1188
  *     if not forward:
  *         xs = xs[::-1]
- *     N = M if N == 0 else min(N, M)             # <<<<<<<<<<<<<<
+ *     N = M if N == 0 else sops.min(N, M)             # <<<<<<<<<<<<<<
  *     cdef double[:, :] DD = view.array(shape=(M, N), itemsize=sizeof(double), format='d')
  *     DD[:, 0] = fs
  */
   if (((__pyx_v_N == 0) != 0)) {
     __pyx_t_5 = __pyx_v_M;
   } else {
-    __pyx_t_6 = __pyx_v_M;
-    __pyx_t_7 = __pyx_v_N;
-    if (((__pyx_t_6 < __pyx_t_7) != 0)) {
-      __pyx_t_8 = __pyx_t_6;
-    } else {
-      __pyx_t_8 = __pyx_t_7;
-    }
-    __pyx_t_5 = __pyx_t_8;
+    __pyx_t_5 = __pyx_fuse_1__pyx_f_6cyroot_3ops_10scalar_ops_min(__pyx_v_N, __pyx_v_M);
   }
   __pyx_v_N = __pyx_t_5;
 
   /* "cyroot/scalar_bracketing.pyx":1189
  *         xs = xs[::-1]
- *     N = M if N == 0 else min(N, M)
+ *     N = M if N == 0 else sops.min(N, M)
  *     cdef double[:, :] DD = view.array(shape=(M, N), itemsize=sizeof(double), format='d')             # <<<<<<<<<<<<<<
  *     DD[:, 0] = fs
  *     for j in range(1, N):
  */
-  __pyx_t_9 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1189, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1189, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_7 = __Pyx_PyInt_From_unsigned_int(__pyx_v_M); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1189, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_8 = __Pyx_PyInt_From_unsigned_int(__pyx_v_N); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1189, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_9 = PyTuple_New(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_10 = __Pyx_PyInt_From_unsigned_int(__pyx_v_M); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1189, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_10);
-  __pyx_t_11 = __Pyx_PyInt_From_unsigned_int(__pyx_v_N); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 1189, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_11);
-  __pyx_t_12 = PyTuple_New(2); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 1189, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_12);
-  __Pyx_GIVEREF(__pyx_t_10);
-  PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_10);
-  __Pyx_GIVEREF(__pyx_t_11);
-  PyTuple_SET_ITEM(__pyx_t_12, 1, __pyx_t_11);
-  __pyx_t_10 = 0;
-  __pyx_t_11 = 0;
-  if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_shape, __pyx_t_12) < 0) __PYX_ERR(0, 1189, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  __pyx_t_12 = __Pyx_PyInt_FromSize_t((sizeof(double))); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 1189, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_12);
-  if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_itemsize, __pyx_t_12) < 0) __PYX_ERR(0, 1189, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_format, __pyx_n_u_d) < 0) __PYX_ERR(0, 1189, __pyx_L1_error)
-  __pyx_t_12 = __Pyx_PyObject_Call(((PyObject *)__pyx_array_type), __pyx_empty_tuple, __pyx_t_9); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 1189, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_12);
+  __Pyx_GIVEREF(__pyx_t_7);
+  PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_7);
+  __Pyx_GIVEREF(__pyx_t_8);
+  PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_t_8);
+  __pyx_t_7 = 0;
+  __pyx_t_8 = 0;
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_shape, __pyx_t_9) < 0) __PYX_ERR(0, 1189, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  __pyx_t_13 = __Pyx_PyObject_to_MemoryviewSlice_dsds_double(__pyx_t_12, PyBUF_WRITABLE); if (unlikely(!__pyx_t_13.memview)) __PYX_ERR(0, 1189, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  __pyx_v_DD = __pyx_t_13;
-  __pyx_t_13.memview = NULL;
-  __pyx_t_13.data = NULL;
+  __pyx_t_9 = __Pyx_PyInt_FromSize_t((sizeof(double))); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1189, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_itemsize, __pyx_t_9) < 0) __PYX_ERR(0, 1189, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_format, __pyx_n_u_d) < 0) __PYX_ERR(0, 1189, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_Call(((PyObject *)__pyx_array_type), __pyx_empty_tuple, __pyx_t_6); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1189, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_dsds_double(__pyx_t_9, PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 1189, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+  __pyx_v_DD = __pyx_t_10;
+  __pyx_t_10.memview = NULL;
+  __pyx_t_10.data = NULL;
 
   /* "cyroot/scalar_bracketing.pyx":1190
- *     N = M if N == 0 else min(N, M)
+ *     N = M if N == 0 else sops.min(N, M)
  *     cdef double[:, :] DD = view.array(shape=(M, N), itemsize=sizeof(double), format='d')
  *     DD[:, 0] = fs             # <<<<<<<<<<<<<<
  *     for j in range(1, N):
  *         DD[:j, j] = 0
  */
   __pyx_t_3.data = __pyx_v_DD.data;
   __pyx_t_3.memview = __pyx_v_DD.memview;
@@ -16638,17 +16637,17 @@
  *     cdef double[:, :] DD = view.array(shape=(M, N), itemsize=sizeof(double), format='d')
  *     DD[:, 0] = fs
  *     for j in range(1, N):             # <<<<<<<<<<<<<<
  *         DD[:j, j] = 0
  *         for i in range(j, M):
  */
   __pyx_t_5 = __pyx_v_N;
-  __pyx_t_8 = __pyx_t_5;
-  for (__pyx_t_6 = 1; __pyx_t_6 < __pyx_t_8; __pyx_t_6+=1) {
-    __pyx_v_j = __pyx_t_6;
+  __pyx_t_11 = __pyx_t_5;
+  for (__pyx_t_12 = 1; __pyx_t_12 < __pyx_t_11; __pyx_t_12+=1) {
+    __pyx_v_j = __pyx_t_12;
 
     /* "cyroot/scalar_bracketing.pyx":1192
  *     DD[:, 0] = fs
  *     for j in range(1, N):
  *         DD[:j, j] = 0             # <<<<<<<<<<<<<<
  *         for i in range(j, M):
  *             DD[i, j] = (DD[i, j - 1] - DD[i - 1, j - 1]) / (xs[i] - xs[i - j])
@@ -16704,16 +16703,16 @@
     /* "cyroot/scalar_bracketing.pyx":1193
  *     for j in range(1, N):
  *         DD[:j, j] = 0
  *         for i in range(j, M):             # <<<<<<<<<<<<<<
  *             DD[i, j] = (DD[i, j - 1] - DD[i - 1, j - 1]) / (xs[i] - xs[i - j])
  *     return DD
  */
-    __pyx_t_7 = __pyx_v_M;
-    __pyx_t_14 = __pyx_t_7;
+    __pyx_t_13 = __pyx_v_M;
+    __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = __pyx_v_j; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_i = __pyx_t_15;
 
       /* "cyroot/scalar_bracketing.pyx":1194
  *         DD[:j, j] = 0
  *         for i in range(j, M):
  *             DD[i, j] = (DD[i, j - 1] - DD[i - 1, j - 1]) / (xs[i] - xs[i - j])             # <<<<<<<<<<<<<<
@@ -16753,19 +16752,19 @@
  *         double[:] xs,
  *         double[:] fs,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __PYX_XDEC_MEMVIEW(&__pyx_t_3, 1);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_9);
-  __Pyx_XDECREF(__pyx_t_10);
-  __Pyx_XDECREF(__pyx_t_11);
-  __Pyx_XDECREF(__pyx_t_12);
-  __PYX_XDEC_MEMVIEW(&__pyx_t_13, 1);
+  __PYX_XDEC_MEMVIEW(&__pyx_t_10, 1);
   __pyx_r.data = NULL;
   __pyx_r.memview = NULL;
   __Pyx_AddTraceback("cyroot.scalar_bracketing._divided_differences", __pyx_clineno, __pyx_lineno, __pyx_filename);
   goto __pyx_L2;
   __pyx_L0:;
   if (unlikely(!__pyx_r.memview)) {
     PyErr_SetString(PyExc_TypeError, "Memoryview return value is not initialized");
@@ -16800,27 +16799,26 @@
   unsigned int __pyx_v_M;
   __Pyx_memviewslice __pyx_v_DD = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_dd = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_r = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_RefNannyDeclarations
   size_t __pyx_t_1;
   unsigned int __pyx_t_2;
-  unsigned int __pyx_t_3;
-  unsigned int __pyx_t_4;
-  unsigned int __pyx_t_5;
-  __Pyx_memviewslice __pyx_t_6 = { 0, 0, { 0 }, { 0 }, { 0 } };
-  struct __pyx_opt_args_6cyroot_17scalar_bracketing__divided_differences __pyx_t_7;
-  PyObject *__pyx_t_8 = NULL;
-  PyObject *__pyx_t_9 = NULL;
-  PyObject *__pyx_t_10 = NULL;
-  __Pyx_memviewslice __pyx_t_11 = { 0, 0, { 0 }, { 0 }, { 0 } };
-  int __pyx_t_12;
+  __Pyx_memviewslice __pyx_t_3 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  struct __pyx_opt_args_6cyroot_17scalar_bracketing__divided_differences __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  __Pyx_memviewslice __pyx_t_8 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  int __pyx_t_9;
+  unsigned int __pyx_t_10;
+  unsigned int __pyx_t_11;
+  size_t __pyx_t_12;
   size_t __pyx_t_13;
-  size_t __pyx_t_14;
-  Py_ssize_t __pyx_t_15;
+  Py_ssize_t __pyx_t_14;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_diag_divided_differences", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_N = __pyx_optional_args->N;
@@ -16830,120 +16828,113 @@
     }
   }
 
   /* "cyroot/scalar_bracketing.pyx":1207
  *       f[a], f[a, b] and f[a, b, c].
  *     """
  *     cdef unsigned int j, M = <unsigned int> len(xs)             # <<<<<<<<<<<<<<
- *     N = M if N == 0 else min(N, M)
+ *     N = M if N == 0 else sops.min(N, M)
  *     cdef double[:, :] DD = _divided_differences(xs, fs, N)
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_xs); 
   __pyx_v_M = ((unsigned int)__pyx_t_1);
 
   /* "cyroot/scalar_bracketing.pyx":1208
  *     """
  *     cdef unsigned int j, M = <unsigned int> len(xs)
- *     N = M if N == 0 else min(N, M)             # <<<<<<<<<<<<<<
+ *     N = M if N == 0 else sops.min(N, M)             # <<<<<<<<<<<<<<
  *     cdef double[:, :] DD = _divided_differences(xs, fs, N)
  *     cdef double[:] dd = view.array(shape=(N,), itemsize=sizeof(double), format='d')
  */
   if (((__pyx_v_N == 0) != 0)) {
     __pyx_t_2 = __pyx_v_M;
   } else {
-    __pyx_t_3 = __pyx_v_M;
-    __pyx_t_4 = __pyx_v_N;
-    if (((__pyx_t_3 < __pyx_t_4) != 0)) {
-      __pyx_t_5 = __pyx_t_3;
-    } else {
-      __pyx_t_5 = __pyx_t_4;
-    }
-    __pyx_t_2 = __pyx_t_5;
+    __pyx_t_2 = __pyx_fuse_1__pyx_f_6cyroot_3ops_10scalar_ops_min(__pyx_v_N, __pyx_v_M);
   }
   __pyx_v_N = __pyx_t_2;
 
   /* "cyroot/scalar_bracketing.pyx":1209
  *     cdef unsigned int j, M = <unsigned int> len(xs)
- *     N = M if N == 0 else min(N, M)
+ *     N = M if N == 0 else sops.min(N, M)
  *     cdef double[:, :] DD = _divided_differences(xs, fs, N)             # <<<<<<<<<<<<<<
  *     cdef double[:] dd = view.array(shape=(N,), itemsize=sizeof(double), format='d')
  *     if forward:
  */
-  __pyx_t_7.__pyx_n = 1;
-  __pyx_t_7.N = __pyx_v_N;
-  __pyx_t_6 = __pyx_f_6cyroot_17scalar_bracketing__divided_differences(__pyx_v_xs, __pyx_v_fs, &__pyx_t_7); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 1209, __pyx_L1_error)
-  __pyx_v_DD = __pyx_t_6;
-  __pyx_t_6.memview = NULL;
-  __pyx_t_6.data = NULL;
+  __pyx_t_4.__pyx_n = 1;
+  __pyx_t_4.N = __pyx_v_N;
+  __pyx_t_3 = __pyx_f_6cyroot_17scalar_bracketing__divided_differences(__pyx_v_xs, __pyx_v_fs, &__pyx_t_4); if (unlikely(!__pyx_t_3.memview)) __PYX_ERR(0, 1209, __pyx_L1_error)
+  __pyx_v_DD = __pyx_t_3;
+  __pyx_t_3.memview = NULL;
+  __pyx_t_3.data = NULL;
 
   /* "cyroot/scalar_bracketing.pyx":1210
- *     N = M if N == 0 else min(N, M)
+ *     N = M if N == 0 else sops.min(N, M)
  *     cdef double[:, :] DD = _divided_differences(xs, fs, N)
  *     cdef double[:] dd = view.array(shape=(N,), itemsize=sizeof(double), format='d')             # <<<<<<<<<<<<<<
  *     if forward:
  *         for j in range(N):
  */
-  __pyx_t_8 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1210, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_9 = __Pyx_PyInt_From_unsigned_int(__pyx_v_N); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1210, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_10 = PyTuple_New(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1210, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_10);
-  __Pyx_GIVEREF(__pyx_t_9);
-  PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_9);
-  __pyx_t_9 = 0;
-  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_shape, __pyx_t_10) < 0) __PYX_ERR(0, 1210, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __pyx_t_10 = __Pyx_PyInt_FromSize_t((sizeof(double))); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1210, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_10);
-  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_itemsize, __pyx_t_10) < 0) __PYX_ERR(0, 1210, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_format, __pyx_n_u_d) < 0) __PYX_ERR(0, 1210, __pyx_L1_error)
-  __pyx_t_10 = __Pyx_PyObject_Call(((PyObject *)__pyx_array_type), __pyx_empty_tuple, __pyx_t_8); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1210, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_10);
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_11 = __Pyx_PyObject_to_MemoryviewSlice_ds_double(__pyx_t_10, PyBUF_WRITABLE); if (unlikely(!__pyx_t_11.memview)) __PYX_ERR(0, 1210, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __pyx_v_dd = __pyx_t_11;
-  __pyx_t_11.memview = NULL;
-  __pyx_t_11.data = NULL;
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1210, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_6 = __Pyx_PyInt_From_unsigned_int(__pyx_v_N); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1210, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1210, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_GIVEREF(__pyx_t_6);
+  PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_6);
+  __pyx_t_6 = 0;
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_shape, __pyx_t_7) < 0) __PYX_ERR(0, 1210, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_7 = __Pyx_PyInt_FromSize_t((sizeof(double))); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1210, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_itemsize, __pyx_t_7) < 0) __PYX_ERR(0, 1210, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_format, __pyx_n_u_d) < 0) __PYX_ERR(0, 1210, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)__pyx_array_type), __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1210, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_ds_double(__pyx_t_7, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 1210, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_v_dd = __pyx_t_8;
+  __pyx_t_8.memview = NULL;
+  __pyx_t_8.data = NULL;
 
   /* "cyroot/scalar_bracketing.pyx":1211
  *     cdef double[:, :] DD = _divided_differences(xs, fs, N)
  *     cdef double[:] dd = view.array(shape=(N,), itemsize=sizeof(double), format='d')
  *     if forward:             # <<<<<<<<<<<<<<
  *         for j in range(N):
  *             dd[j] = DD[j, j]
  */
-  __pyx_t_12 = (__pyx_v_forward != 0);
-  if (__pyx_t_12) {
+  __pyx_t_9 = (__pyx_v_forward != 0);
+  if (__pyx_t_9) {
 
     /* "cyroot/scalar_bracketing.pyx":1212
  *     cdef double[:] dd = view.array(shape=(N,), itemsize=sizeof(double), format='d')
  *     if forward:
  *         for j in range(N):             # <<<<<<<<<<<<<<
  *             dd[j] = DD[j, j]
  *     else:
  */
     __pyx_t_2 = __pyx_v_N;
-    __pyx_t_5 = __pyx_t_2;
-    for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_5; __pyx_t_3+=1) {
-      __pyx_v_j = __pyx_t_3;
+    __pyx_t_10 = __pyx_t_2;
+    for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_10; __pyx_t_11+=1) {
+      __pyx_v_j = __pyx_t_11;
 
       /* "cyroot/scalar_bracketing.pyx":1213
  *     if forward:
  *         for j in range(N):
  *             dd[j] = DD[j, j]             # <<<<<<<<<<<<<<
  *     else:
  *         for j in range(N):
  */
       __pyx_t_1 = __pyx_v_j;
+      __pyx_t_12 = __pyx_v_j;
       __pyx_t_13 = __pyx_v_j;
-      __pyx_t_14 = __pyx_v_j;
-      *((double *) ( /* dim=0 */ (__pyx_v_dd.data + __pyx_t_14 * __pyx_v_dd.strides[0]) )) = (*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_DD.data + __pyx_t_1 * __pyx_v_DD.strides[0]) ) + __pyx_t_13 * __pyx_v_DD.strides[1]) )));
+      *((double *) ( /* dim=0 */ (__pyx_v_dd.data + __pyx_t_13 * __pyx_v_dd.strides[0]) )) = (*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_DD.data + __pyx_t_1 * __pyx_v_DD.strides[0]) ) + __pyx_t_12 * __pyx_v_DD.strides[1]) )));
     }
 
     /* "cyroot/scalar_bracketing.pyx":1211
  *     cdef double[:, :] DD = _divided_differences(xs, fs, N)
  *     cdef double[:] dd = view.array(shape=(N,), itemsize=sizeof(double), format='d')
  *     if forward:             # <<<<<<<<<<<<<<
  *         for j in range(N):
@@ -16957,30 +16948,30 @@
  *     else:
  *         for j in range(N):             # <<<<<<<<<<<<<<
  *             dd[j] = DD[-1, j]
  *     return dd
  */
   /*else*/ {
     __pyx_t_2 = __pyx_v_N;
-    __pyx_t_5 = __pyx_t_2;
-    for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_5; __pyx_t_3+=1) {
-      __pyx_v_j = __pyx_t_3;
+    __pyx_t_10 = __pyx_t_2;
+    for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_10; __pyx_t_11+=1) {
+      __pyx_v_j = __pyx_t_11;
 
       /* "cyroot/scalar_bracketing.pyx":1216
  *     else:
  *         for j in range(N):
  *             dd[j] = DD[-1, j]             # <<<<<<<<<<<<<<
  *     return dd
  * 
  */
-      __pyx_t_15 = -1L;
-      __pyx_t_13 = __pyx_v_j;
-      if (__pyx_t_15 < 0) __pyx_t_15 += __pyx_v_DD.shape[0];
+      __pyx_t_14 = -1L;
+      __pyx_t_12 = __pyx_v_j;
+      if (__pyx_t_14 < 0) __pyx_t_14 += __pyx_v_DD.shape[0];
       __pyx_t_1 = __pyx_v_j;
-      *((double *) ( /* dim=0 */ (__pyx_v_dd.data + __pyx_t_1 * __pyx_v_dd.strides[0]) )) = (*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_DD.data + __pyx_t_15 * __pyx_v_DD.strides[0]) ) + __pyx_t_13 * __pyx_v_DD.strides[1]) )));
+      *((double *) ( /* dim=0 */ (__pyx_v_dd.data + __pyx_t_1 * __pyx_v_dd.strides[0]) )) = (*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_DD.data + __pyx_t_14 * __pyx_v_DD.strides[0]) ) + __pyx_t_12 * __pyx_v_DD.strides[1]) )));
     }
   }
   __pyx_L3:;
 
   /* "cyroot/scalar_bracketing.pyx":1217
  *         for j in range(N):
  *             dd[j] = DD[-1, j]
@@ -16998,19 +16989,19 @@
  * cdef double[:] _diag_divided_differences(             # <<<<<<<<<<<<<<
  *         double[:] xs,
  *         double[:] fs,
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __PYX_XDEC_MEMVIEW(&__pyx_t_6, 1);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_XDECREF(__pyx_t_9);
-  __Pyx_XDECREF(__pyx_t_10);
-  __PYX_XDEC_MEMVIEW(&__pyx_t_11, 1);
+  __PYX_XDEC_MEMVIEW(&__pyx_t_3, 1);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __PYX_XDEC_MEMVIEW(&__pyx_t_8, 1);
   __pyx_r.data = NULL;
   __pyx_r.memview = NULL;
   __Pyx_AddTraceback("cyroot.scalar_bracketing._diag_divided_differences", __pyx_clineno, __pyx_lineno, __pyx_filename);
   goto __pyx_L2;
   __pyx_L0:;
   if (unlikely(!__pyx_r.memview)) {
     PyErr_SetString(PyExc_TypeError, "Memoryview return value is not initialized");
@@ -22315,15 +22306,15 @@
   __Pyx_XDECREF(__pyx_v_prtol);
   __Pyx_XDECREF(__pyx_v_max_iter);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -22332,29 +22323,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -22365,15 +22356,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -22382,29 +22373,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -22415,15 +22406,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -22432,29 +22423,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -22465,15 +22456,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -22482,29 +22473,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -22515,15 +22506,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -22532,29 +22523,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -22565,212 +22556,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -22786,15 +22777,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -22802,53 +22793,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__60, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
@@ -22856,30 +22847,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -22894,15 +22885,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -22918,15 +22909,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -22934,53 +22925,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__61, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
@@ -22988,30 +22979,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -23026,15 +23017,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -23050,15 +23041,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -23066,53 +23057,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__61, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
@@ -23120,30 +23111,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -23158,176 +23149,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -38021,26 +38012,26 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__60 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__60)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__60);
   __Pyx_GIVEREF(__pyx_tuple__60);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__61 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__61)) __PYX_ERR(1, 950, __pyx_L1_error)
@@ -38781,14 +38772,20 @@
   __Pyx_GOTREF(__pyx_t_1);
   if (__Pyx_ImportFunction(__pyx_t_1, "_check_stop_cond_scalar_bracket", (void (**)(void))&__pyx_f_6cyroot_11_check_args__check_stop_cond_scalar_bracket, "int (double, double, double, double, double, double, double, double, double *, double *, double *, double *, int *, int *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ImportFunction(__pyx_t_1, "_check_stop_cond_scalar_initial_guess", (void (**)(void))&__pyx_f_6cyroot_11_check_args__check_stop_cond_scalar_initial_guess, "int (double, double, double, double, double, double, double *, double *, int *, int *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("cyroot.ops.scalar_ops"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (__Pyx_ImportFunction(__pyx_t_1, "isclose", (void (**)(void))&__pyx_f_6cyroot_3ops_10scalar_ops_isclose, "int (double, double, struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_isclose *__pyx_optional_args)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_0min", (void (**)(void))&__pyx_fuse_0__pyx_f_6cyroot_3ops_10scalar_ops_min, "int (int, int)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_1min", (void (**)(void))&__pyx_fuse_1__pyx_f_6cyroot_3ops_10scalar_ops_min, "unsigned int (unsigned int, unsigned int)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_2min", (void (**)(void))&__pyx_fuse_2__pyx_f_6cyroot_3ops_10scalar_ops_min, "long (long, long)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_3min", (void (**)(void))&__pyx_fuse_3__pyx_f_6cyroot_3ops_10scalar_ops_min, "unsigned long (unsigned long, unsigned long)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_4min", (void (**)(void))&__pyx_fuse_4__pyx_f_6cyroot_3ops_10scalar_ops_min, "float (float, float)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction(__pyx_t_1, "__pyx_fuse_5min", (void (**)(void))&__pyx_fuse_5__pyx_f_6cyroot_3ops_10scalar_ops_min, "double (double, double)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
```

### Comparing `cy-root-1.0.1/cyroot/scalar_bracketing.pyx` & `cy-root-1.0.2/cyroot/scalar_bracketing.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -1181,15 +1181,15 @@
     """Return a matrix of divided differences for the xs, fs pairs
 
     DD[i, j] = f[x_{i-j}, ..., x_i] for 0 <= j <= i
     If forward is False, return f[c], f[b, c], f[a, b, c]."""
     cdef unsigned int i, j, M = <unsigned int> len(xs)
     if not forward:
         xs = xs[::-1]
-    N = M if N == 0 else min(N, M)
+    N = M if N == 0 else sops.min(N, M)
     cdef double[:, :] DD = view.array(shape=(M, N), itemsize=sizeof(double), format='d')
     DD[:, 0] = fs
     for j in range(1, N):
         DD[:j, j] = 0
         for i in range(j, M):
             DD[i, j] = (DD[i, j - 1] - DD[i - 1, j - 1]) / (xs[i] - xs[i - j])
     return DD
@@ -1201,15 +1201,15 @@
         unsigned int N=0,
         bint forward=True):
     """
     Just return the main diagonal(or last row):
       f[a], f[a, b] and f[a, b, c].
     """
     cdef unsigned int j, M = <unsigned int> len(xs)
-    N = M if N == 0 else min(N, M)
+    N = M if N == 0 else sops.min(N, M)
     cdef double[:, :] DD = _divided_differences(xs, fs, N)
     cdef double[:] dd = view.array(shape=(N,), itemsize=sizeof(double), format='d')
     if forward:
         for j in range(N):
             dd[j] = DD[j, j]
     else:
         for j in range(N):
```

### Comparing `cy-root-1.0.1/cyroot/scalar_derivative_approximation.cpp` & `cy-root-1.0.2/cyroot/scalar_derivative_approximation.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
             "cyroot",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include",
             "cyroot/ops",
             "cyroot/utils"
         ],
         "language": "c++",
         "name": "cyroot.scalar_derivative_approximation",
         "sources": [
             "cyroot/scalar_derivative_approximation.pyx"
@@ -1168,195 +1168,195 @@
   Py_ssize_t shape[8];
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1413,42 +1413,42 @@
 struct __pyx_obj_6cyroot_31scalar_derivative_approximation___pyx_scope_struct___check_finite_difference_args;
 struct __pyx_obj_6cyroot_31scalar_derivative_approximation___pyx_scope_struct_1_genexpr;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1531,28 +1531,28 @@
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_cisclose;
 
 /* "scalar_ops.pxd":18
  *     double complex
  * 
  * cdef bint isclose(double a, double b, double rtol=*, double atol=*) nogil             # <<<<<<<<<<<<<<
  * cdef bint cisclose(double complex a, double complex b, double rtol=*, double atol=*) nogil
- * 
+ * cdef real min(real a, real b) nogil
  */
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_isclose {
   int __pyx_n;
   double rtol;
   double atol;
 };
 
 /* "scalar_ops.pxd":19
  * 
  * cdef bint isclose(double a, double b, double rtol=*, double atol=*) nogil
  * cdef bint cisclose(double complex a, double complex b, double rtol=*, double atol=*) nogil             # <<<<<<<<<<<<<<
- * 
- * cdef extern from '<math.h>' nogil:
+ * cdef real min(real a, real b) nogil
+ * cdef real max(real a, real b) nogil
  */
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_cisclose {
   int __pyx_n;
   double rtol;
   double atol;
 };
 struct __pyx_opt_args_6cyroot_31scalar_derivative_approximation_finite_difference_kernel;
@@ -8096,15 +8096,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -8113,29 +8113,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -8146,15 +8146,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -8163,29 +8163,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -8196,15 +8196,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -8213,29 +8213,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -8246,15 +8246,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -8263,29 +8263,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -8296,15 +8296,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -8313,29 +8313,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -8346,212 +8346,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -8567,15 +8567,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -8583,53 +8583,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 942, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 944, __pyx_L5_except_error)
@@ -8637,30 +8637,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -8675,15 +8675,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8699,15 +8699,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -8715,53 +8715,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 948, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 950, __pyx_L5_except_error)
@@ -8769,30 +8769,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8807,15 +8807,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8831,15 +8831,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -8847,53 +8847,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 954, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 956, __pyx_L5_except_error)
@@ -8901,30 +8901,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8939,176 +8939,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -23618,26 +23618,26 @@
   __pyx_tuple__4 = PyTuple_Pack(3, __pyx_int_205748470, __pyx_int_27230149, __pyx_int_266326257); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
   __pyx_tuple__5 = PyTuple_Pack(3, __pyx_int_227476734, __pyx_int_233537600, __pyx_int_246520410); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(3, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(3, 950, __pyx_L1_error)
```

### Comparing `cy-root-1.0.1/cyroot/scalar_derivative_approximation.pxd` & `cy-root-1.0.2/cyroot/scalar_derivative_approximation.pxd`

 * *Files identical despite different names*

### Comparing `cy-root-1.0.1/cyroot/scalar_derivative_approximation.pyx` & `cy-root-1.0.2/cyroot/scalar_derivative_approximation.pyx`

 * *Files identical despite different names*

### Comparing `cy-root-1.0.1/cyroot/scalar_newton.cpp` & `cy-root-1.0.2/cyroot/scalar_newton.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
             "cyroot",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include",
             "cyroot/ops",
             "cyroot/utils"
         ],
         "language": "c++",
         "name": "cyroot.scalar_newton",
         "sources": [
             "cyroot/scalar_newton.pyx"
@@ -1172,195 +1172,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1436,42 +1436,42 @@
 struct __pyx_obj_6cyroot_13scalar_newton___pyx_scope_struct__householder;
 struct __pyx_obj_6cyroot_13scalar_newton___pyx_scope_struct_1_genexpr;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1572,28 +1572,28 @@
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_cisclose;
 
 /* "scalar_ops.pxd":18
  *     double complex
  * 
  * cdef bint isclose(double a, double b, double rtol=*, double atol=*) nogil             # <<<<<<<<<<<<<<
  * cdef bint cisclose(double complex a, double complex b, double rtol=*, double atol=*) nogil
- * 
+ * cdef real min(real a, real b) nogil
  */
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_isclose {
   int __pyx_n;
   double rtol;
   double atol;
 };
 
 /* "scalar_ops.pxd":19
  * 
  * cdef bint isclose(double a, double b, double rtol=*, double atol=*) nogil
  * cdef bint cisclose(double complex a, double complex b, double rtol=*, double atol=*) nogil             # <<<<<<<<<<<<<<
- * 
- * cdef extern from '<math.h>' nogil:
+ * cdef real min(real a, real b) nogil
+ * cdef real max(real a, real b) nogil
  */
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_cisclose {
   int __pyx_n;
   double rtol;
   double atol;
 };
 struct __pyx_ctuple_9a9163__double__and_double__and_double__and_unsigned__space_long__and_double__and_double__and_int__and_int__etc;
@@ -34575,15 +34575,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -34592,29 +34592,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -34625,15 +34625,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -34642,29 +34642,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -34675,15 +34675,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -34692,29 +34692,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -34725,15 +34725,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -34742,29 +34742,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -34775,15 +34775,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -34792,29 +34792,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -34825,212 +34825,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -35046,15 +35046,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -35062,53 +35062,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 942, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__39, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 944, __pyx_L5_except_error)
@@ -35116,30 +35116,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -35154,15 +35154,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -35178,15 +35178,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -35194,53 +35194,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 948, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__40, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 950, __pyx_L5_except_error)
@@ -35248,30 +35248,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -35286,15 +35286,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -35310,15 +35310,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -35326,53 +35326,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 954, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__40, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 956, __pyx_L5_except_error)
@@ -35380,30 +35380,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -35418,176 +35418,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -52268,26 +52268,26 @@
   __pyx_tuple__37 = PyTuple_Pack(3, __pyx_int_115507066, __pyx_int_31713873, __pyx_int_76435203); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__37);
   __Pyx_GIVEREF(__pyx_tuple__37);
   __pyx_tuple__38 = PyTuple_Pack(3, __pyx_int_187108125, __pyx_int_229155923, __pyx_int_143107811); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__38);
   __Pyx_GIVEREF(__pyx_tuple__38);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__39 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(2, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__39);
   __Pyx_GIVEREF(__pyx_tuple__39);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__40 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(2, 950, __pyx_L1_error)
```

### Comparing `cy-root-1.0.1/cyroot/scalar_newton.pyx` & `cy-root-1.0.2/cyroot/scalar_newton.pyx`

 * *Files identical despite different names*

### Comparing `cy-root-1.0.1/cyroot/scalar_quasi_newton.cpp` & `cy-root-1.0.2/cyroot/scalar_quasi_newton.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
             "cyroot",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include",
             "cyroot/ops",
             "cyroot/utils"
         ],
         "language": "c++",
         "name": "cyroot.scalar_quasi_newton",
         "sources": [
             "cyroot/scalar_quasi_newton.pyx"
@@ -1167,195 +1167,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1409,42 +1409,42 @@
 struct __pyx_obj_6cyroot_4fptr_PyNdArrayFPtr;
 struct __pyx_obj_6cyroot_19scalar_quasi_newton_NewtonPolynomial;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1545,28 +1545,28 @@
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_cisclose;
 
 /* "scalar_ops.pxd":18
  *     double complex
  * 
  * cdef bint isclose(double a, double b, double rtol=*, double atol=*) nogil             # <<<<<<<<<<<<<<
  * cdef bint cisclose(double complex a, double complex b, double rtol=*, double atol=*) nogil
- * 
+ * cdef real min(real a, real b) nogil
  */
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_isclose {
   int __pyx_n;
   double rtol;
   double atol;
 };
 
 /* "scalar_ops.pxd":19
  * 
  * cdef bint isclose(double a, double b, double rtol=*, double atol=*) nogil
  * cdef bint cisclose(double complex a, double complex b, double rtol=*, double atol=*) nogil             # <<<<<<<<<<<<<<
- * 
- * cdef extern from '<math.h>' nogil:
+ * cdef real min(real a, real b) nogil
+ * cdef real max(real a, real b) nogil
  */
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_cisclose {
   int __pyx_n;
   double rtol;
   double atol;
 };
 struct __pyx_opt_args_6cyroot_3ops_10vector_ops_allclose;
@@ -3739,37 +3739,36 @@
   static const char __pyx_k_s[] = "(%s)";
   static const char __pyx_k_x[] = "x";
   static const char __pyx_k_id[] = "id";
   static const char __pyx_k_np[] = "np";
   static const char __pyx_k_x0[] = "x0";
   static const char __pyx_k_x1[] = "x1";
   static const char __pyx_k_x2[] = "x2";
-  static const char __pyx_k_xs[] = "xs";
   static const char __pyx_k__14[] = ".";
   static const char __pyx_k__56[] = "^";
   static const char __pyx_k__57[] = "";
   static const char __pyx_k__58[] = ":";
 static const char __pyx_k__59[] = "}";
 static const char __pyx_k__60[] = ",";
 static const char __pyx_k_all[] = "__all__";
 static const char __pyx_k_and[] = " and ";
 static const char __pyx_k_int[] = "int";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_obj[] = "obj";
 static const char __pyx_k_res[] = "res";
 static const char __pyx_k_tag[] = "tag";
+static const char __pyx_k_x0s[] = "x0s";
 static const char __pyx_k_ETOL[] = "ETOL";
 static const char __pyx_k_PTOL[] = "PTOL";
 static const char __pyx_k_base[] = "base";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_etol[] = "etol";
 static const char __pyx_k_f_x0[] = "f_x0";
 static const char __pyx_k_f_x1[] = "f_x1";
 static const char __pyx_k_f_x2[] = "f_x2";
-static const char __pyx_k_f_xs[] = "f_xs";
 static const char __pyx_k_join[] = "join";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_mode[] = "mode";
 static const char __pyx_k_name[] = "name";
 static const char __pyx_k_ndim[] = "ndim";
 static const char __pyx_k_pack[] = "pack";
 static const char __pyx_k_ptol[] = "ptol";
@@ -3782,14 +3781,15 @@
 static const char __pyx_k_ERTOL[] = "ERTOL";
 static const char __pyx_k_PRTOL[] = "PRTOL";
 static const char __pyx_k_array[] = "array";
 static const char __pyx_k_class[] = "__class__";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_error[] = "error";
 static const char __pyx_k_ertol[] = "ertol";
+static const char __pyx_k_f_x0s[] = "f_x0s";
 static const char __pyx_k_flags[] = "flags";
 static const char __pyx_k_float[] = "float";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_prtol[] = "prtol";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_shape[] = "shape";
 static const char __pyx_k_start[] = "start";
@@ -3964,17 +3964,17 @@
 static PyObject *__pyx_n_s_enumerate;
 static PyObject *__pyx_n_s_error;
 static PyObject *__pyx_n_s_ertol;
 static PyObject *__pyx_n_s_etol;
 static PyObject *__pyx_n_s_f;
 static PyObject *__pyx_n_s_f_wrapper;
 static PyObject *__pyx_n_s_f_x0;
+static PyObject *__pyx_n_s_f_x0s;
 static PyObject *__pyx_n_s_f_x1;
 static PyObject *__pyx_n_s_f_x2;
-static PyObject *__pyx_n_s_f_xs;
 static PyObject *__pyx_n_s_flags;
 static PyObject *__pyx_n_u_float;
 static PyObject *__pyx_n_s_float64;
 static PyObject *__pyx_n_s_format;
 static PyObject *__pyx_n_s_fortran;
 static PyObject *__pyx_n_u_fortran;
 static PyObject *__pyx_n_s_from_results;
@@ -4052,26 +4052,26 @@
 static PyObject *__pyx_kp_s_unable_to_allocate_array_data;
 static PyObject *__pyx_kp_s_unable_to_allocate_shape_and_str;
 static PyObject *__pyx_n_s_unpack;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_n_s_utils_function_tagging;
 static PyObject *__pyx_n_s_x;
 static PyObject *__pyx_n_s_x0;
+static PyObject *__pyx_n_s_x0s;
 static PyObject *__pyx_n_s_x1;
 static PyObject *__pyx_n_s_x2;
-static PyObject *__pyx_n_s_xs;
 static PyObject *__pyx_kp_u_xs_and_f_xs_must_have_same_size;
 static PyObject *__pyx_pf_6cyroot_19scalar_quasi_newton_12__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_6cyroot_19scalar_quasi_newton_secant(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_f, double __pyx_v_x0, double __pyx_v_x1, PyObject *__pyx_v_f_x0, PyObject *__pyx_v_f_x1, PyObject *__pyx_v_etol, PyObject *__pyx_v_ertol, PyObject *__pyx_v_ptol, PyObject *__pyx_v_prtol, PyObject *__pyx_v_max_iter); /* proto */
 static int __pyx_pf_6cyroot_19scalar_quasi_newton_16NewtonPolynomial___cinit__(struct __pyx_obj_6cyroot_19scalar_quasi_newton_NewtonPolynomial *__pyx_v_self, unsigned int __pyx_v_n); /* proto */
 static PyObject *__pyx_pf_6cyroot_19scalar_quasi_newton_16NewtonPolynomial_2__call__(struct __pyx_obj_6cyroot_19scalar_quasi_newton_NewtonPolynomial *__pyx_v_self, double __pyx_v_x); /* proto */
 static PyObject *__pyx_pf_6cyroot_19scalar_quasi_newton_16NewtonPolynomial_4__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_6cyroot_19scalar_quasi_newton_NewtonPolynomial *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6cyroot_19scalar_quasi_newton_16NewtonPolynomial_6__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_6cyroot_19scalar_quasi_newton_NewtonPolynomial *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_6cyroot_19scalar_quasi_newton_14__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_6cyroot_19scalar_quasi_newton_2sidi(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_f, PyObject *__pyx_v_xs, PyObject *__pyx_v_f_xs, PyObject *__pyx_v_etol, PyObject *__pyx_v_ertol, PyObject *__pyx_v_ptol, PyObject *__pyx_v_prtol, PyObject *__pyx_v_max_iter); /* proto */
+static PyObject *__pyx_pf_6cyroot_19scalar_quasi_newton_2sidi(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_f, PyObject *__pyx_v_x0s, PyObject *__pyx_v_f_x0s, PyObject *__pyx_v_etol, PyObject *__pyx_v_ertol, PyObject *__pyx_v_ptol, PyObject *__pyx_v_prtol, PyObject *__pyx_v_max_iter); /* proto */
 static PyObject *__pyx_pf_6cyroot_19scalar_quasi_newton_16__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_6cyroot_19scalar_quasi_newton_4steffensen(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_f, double __pyx_v_x0, PyObject *__pyx_v_f_x0, PyObject *__pyx_v_aitken, PyObject *__pyx_v_etol, PyObject *__pyx_v_ertol, PyObject *__pyx_v_ptol, PyObject *__pyx_v_prtol, PyObject *__pyx_v_max_iter); /* proto */
 static PyObject *__pyx_pf_6cyroot_19scalar_quasi_newton_18__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_6cyroot_19scalar_quasi_newton_6inverse_quadratic_interp(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_f, double __pyx_v_x0, double __pyx_v_x1, double __pyx_v_x2, PyObject *__pyx_v_f_x0, PyObject *__pyx_v_f_x1, PyObject *__pyx_v_f_x2, PyObject *__pyx_v_etol, PyObject *__pyx_v_ertol, PyObject *__pyx_v_ptol, PyObject *__pyx_v_prtol, PyObject *__pyx_v_max_iter); /* proto */
 static PyObject *__pyx_pf_6cyroot_19scalar_quasi_newton_20__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_6cyroot_19scalar_quasi_newton_8hyperbolic_interp(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_f, double __pyx_v_x0, double __pyx_v_x1, double __pyx_v_x2, PyObject *__pyx_v_f_x0, PyObject *__pyx_v_f_x1, PyObject *__pyx_v_f_x2, PyObject *__pyx_v_etol, PyObject *__pyx_v_ertol, PyObject *__pyx_v_ptol, PyObject *__pyx_v_prtol, PyObject *__pyx_v_max_iter); /* proto */
 static PyObject *__pyx_pf_6cyroot_19scalar_quasi_newton_22__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
@@ -6950,16 +6950,16 @@
   return __pyx_r;
 }
 
 /* "cyroot/scalar_quasi_newton.pyx":265
  * @dynamic_default_args()
  * @cython.binding(True)
  * def sidi(f: Callable[[float], float],             # <<<<<<<<<<<<<<
- *          xs: VectorLike,
- *          f_xs: Optional[VectorLike] = None,
+ *          x0s: VectorLike,
+ *          f_x0s: Optional[VectorLike] = None,
  */
 
 static PyObject *__pyx_pf_6cyroot_19scalar_quasi_newton_14__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
@@ -6967,16 +6967,16 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__defaults__", 0);
   __Pyx_XDECREF(__pyx_r);
 
   /* "cyroot/scalar_quasi_newton.pyx":267
  * def sidi(f: Callable[[float], float],
- *          xs: VectorLike,
- *          f_xs: Optional[VectorLike] = None,             # <<<<<<<<<<<<<<
+ *          x0s: VectorLike,
+ *          f_x0s: Optional[VectorLike] = None,             # <<<<<<<<<<<<<<
  *          etol: float = named_default(ETOL=ETOL),
  *          ertol: float = named_default(ERTOL=ERTOL),
  */
   __pyx_t_1 = PyTuple_New(6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(((PyObject *)Py_None));
   __Pyx_GIVEREF(((PyObject *)Py_None));
@@ -6997,16 +6997,16 @@
   __Pyx_GIVEREF(__Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_self)->__pyx_arg_max_iter);
   PyTuple_SET_ITEM(__pyx_t_1, 5, __Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_self)->__pyx_arg_max_iter);
 
   /* "cyroot/scalar_quasi_newton.pyx":265
  * @dynamic_default_args()
  * @cython.binding(True)
  * def sidi(f: Callable[[float], float],             # <<<<<<<<<<<<<<
- *          xs: VectorLike,
- *          f_xs: Optional[VectorLike] = None,
+ *          x0s: VectorLike,
+ *          f_x0s: Optional[VectorLike] = None,
  */
   __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
@@ -7026,33 +7026,33 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6cyroot_19scalar_quasi_newton_3sidi(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6cyroot_19scalar_quasi_newton_2sidi[] = "\n    Sidi's Generalized Secant method for scalar root-finding.\n\n    Args:\n        f (function): Function for which the root is sought.\n        xs (tuple of float): Tuple of initial points.\n        f_xs (tuple of float, optional): Tuple of values evaluated at initial points.\n        etol (float, optional): Error tolerance, indicating the\n         desired precision of the root. Defaults to {etol}.\n        ertol (float, optional): Relative error tolerance.\n         Defaults to {ertol}.\n        ptol (float, optional): Precision tolerance, indicating\n         the minimum change of root approximations or width of\n         brackets (in bracketing methods) after each iteration.\n         Defaults to {ptol}.\n        prtol (float, optional): Relative precision tolerance.\n         Defaults to {prtol}.\n        max_iter (int, optional): Maximum number of iterations.\n         If set to 0, the procedure will run indefinitely until\n         stopping condition is met. Defaults to {max_iter}.\n\n    Returns:\n        solution: The solution represented as a ``RootResults`` object.\n    ";
+static char __pyx_doc_6cyroot_19scalar_quasi_newton_2sidi[] = "\n    Sidi's Generalized Secant method for scalar root-finding.\n\n    Args:\n        f (function): Function for which the root is sought.\n        x0s (tuple of float): Tuple of initial points.\n        f_x0s (tuple of float, optional): Tuple of values evaluated at initial points.\n        etol (float, optional): Error tolerance, indicating the\n         desired precision of the root. Defaults to {etol}.\n        ertol (float, optional): Relative error tolerance.\n         Defaults to {ertol}.\n        ptol (float, optional): Precision tolerance, indicating\n         the minimum change of root approximations or width of\n         brackets (in bracketing methods) after each iteration.\n         Defaults to {ptol}.\n        prtol (float, optional): Relative precision tolerance.\n         Defaults to {prtol}.\n        max_iter (int, optional): Maximum number of iterations.\n         If set to 0, the procedure will run indefinitely until\n         stopping condition is met. Defaults to {max_iter}.\n\n    Returns:\n        solution: The solution represented as a ``RootResults`` object.\n    ";
 static PyMethodDef __pyx_mdef_6cyroot_19scalar_quasi_newton_3sidi = {"sidi", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6cyroot_19scalar_quasi_newton_3sidi, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6cyroot_19scalar_quasi_newton_2sidi};
 static PyObject *__pyx_pw_6cyroot_19scalar_quasi_newton_3sidi(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_f = 0;
-  PyObject *__pyx_v_xs = 0;
-  PyObject *__pyx_v_f_xs = 0;
+  PyObject *__pyx_v_x0s = 0;
+  PyObject *__pyx_v_f_x0s = 0;
   PyObject *__pyx_v_etol = 0;
   PyObject *__pyx_v_ertol = 0;
   PyObject *__pyx_v_ptol = 0;
   PyObject *__pyx_v_prtol = 0;
   PyObject *__pyx_v_max_iter = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("sidi (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_f,&__pyx_n_s_xs,&__pyx_n_s_f_xs,&__pyx_n_s_etol,&__pyx_n_s_ertol,&__pyx_n_s_ptol,&__pyx_n_s_prtol,&__pyx_n_s_max_iter,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_f,&__pyx_n_s_x0s,&__pyx_n_s_f_x0s,&__pyx_n_s_etol,&__pyx_n_s_ertol,&__pyx_n_s_ptol,&__pyx_n_s_prtol,&__pyx_n_s_max_iter,0};
     PyObject* values[8] = {0,0,0,0,0,0,0,0};
     __pyx_defaults1 *__pyx_dynamic_args = __Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_self);
     values[2] = ((PyObject *)((PyObject *)Py_None));
     values[3] = __pyx_dynamic_args->__pyx_arg_etol;
     values[4] = __pyx_dynamic_args->__pyx_arg_ertol;
     values[5] = __pyx_dynamic_args->__pyx_arg_ptol;
     values[6] = __pyx_dynamic_args->__pyx_arg_prtol;
@@ -7083,22 +7083,22 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_f)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_xs)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_x0s)) != 0)) kw_args--;
         else {
           __Pyx_RaiseArgtupleInvalid("sidi", 0, 2, 8, 1); __PYX_ERR(0, 265, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_f_xs);
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_f_x0s);
           if (value) { values[2] = value; kw_args--; }
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_etol);
           if (value) { values[3] = value; kw_args--; }
@@ -7148,38 +7148,38 @@
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_f = values[0];
-    __pyx_v_xs = values[1];
-    __pyx_v_f_xs = values[2];
+    __pyx_v_x0s = values[1];
+    __pyx_v_f_x0s = values[2];
     __pyx_v_etol = values[3];
     __pyx_v_ertol = values[4];
     __pyx_v_ptol = values[5];
     __pyx_v_prtol = values[6];
     __pyx_v_max_iter = values[7];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("sidi", 0, 2, 8, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 265, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cyroot.scalar_quasi_newton.sidi", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6cyroot_19scalar_quasi_newton_2sidi(__pyx_self, __pyx_v_f, __pyx_v_xs, __pyx_v_f_xs, __pyx_v_etol, __pyx_v_ertol, __pyx_v_ptol, __pyx_v_prtol, __pyx_v_max_iter);
+  __pyx_r = __pyx_pf_6cyroot_19scalar_quasi_newton_2sidi(__pyx_self, __pyx_v_f, __pyx_v_x0s, __pyx_v_f_x0s, __pyx_v_etol, __pyx_v_ertol, __pyx_v_ptol, __pyx_v_prtol, __pyx_v_max_iter);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6cyroot_19scalar_quasi_newton_2sidi(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_f, PyObject *__pyx_v_xs, PyObject *__pyx_v_f_xs, PyObject *__pyx_v_etol, PyObject *__pyx_v_ertol, PyObject *__pyx_v_ptol, PyObject *__pyx_v_prtol, PyObject *__pyx_v_max_iter) {
+static PyObject *__pyx_pf_6cyroot_19scalar_quasi_newton_2sidi(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_f, PyObject *__pyx_v_x0s, PyObject *__pyx_v_f_x0s, PyObject *__pyx_v_etol, PyObject *__pyx_v_ertol, PyObject *__pyx_v_ptol, PyObject *__pyx_v_prtol, PyObject *__pyx_v_max_iter) {
   struct __pyx_obj_6cyroot_4fptr_DoubleScalarFPtr *__pyx_v_f_wrapper = NULL;
   PyObject *__pyx_v_res = NULL;
   PyObject *__pyx_7genexpr__pyx_v_x = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
@@ -7204,28 +7204,28 @@
   unsigned long __pyx_t_21;
   __pyx_ctuple_de07d9__double__and_double__and_unsigned__space_long__and_double__and_double__and_int__and_int__etc __pyx_t_22;
   struct __pyx_opt_args_6cyroot_19scalar_quasi_newton_sidi_kernel __pyx_t_23;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("sidi", 0);
-  __Pyx_INCREF(__pyx_v_xs);
-  __Pyx_INCREF(__pyx_v_f_xs);
+  __Pyx_INCREF(__pyx_v_x0s);
+  __Pyx_INCREF(__pyx_v_f_x0s);
   __Pyx_INCREF(__pyx_v_etol);
   __Pyx_INCREF(__pyx_v_ertol);
   __Pyx_INCREF(__pyx_v_ptol);
   __Pyx_INCREF(__pyx_v_prtol);
   __Pyx_INCREF(__pyx_v_max_iter);
 
   /* "cyroot/scalar_quasi_newton.pyx":298
  *     """
  *     # check params
  *     etol, ertol, ptol, prtol, max_iter = _check_stop_cond_args(etol, ertol, ptol, prtol, max_iter)             # <<<<<<<<<<<<<<
  * 
- *     xs = np.asarray(xs, dtype=np.float64)
+ *     x0s = np.asarray(x0s, dtype=np.float64)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_check_stop_cond_args); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 298, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
@@ -7351,87 +7351,87 @@
   __pyx_t_6 = 0;
   __Pyx_DECREF_SET(__pyx_v_max_iter, __pyx_t_7);
   __pyx_t_7 = 0;
 
   /* "cyroot/scalar_quasi_newton.pyx":300
  *     etol, ertol, ptol, prtol, max_iter = _check_stop_cond_args(etol, ertol, ptol, prtol, max_iter)
  * 
- *     xs = np.asarray(xs, dtype=np.float64)             # <<<<<<<<<<<<<<
- *     if xs.shape[0] < 2:
+ *     x0s = np.asarray(x0s, dtype=np.float64)             # <<<<<<<<<<<<<<
+ *     if x0s.shape[0] < 2:
  *         raise ValueError('Requires at least 2 initial guesses. '
  */
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 300, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_asarray); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 300, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 300, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_INCREF(__pyx_v_xs);
-  __Pyx_GIVEREF(__pyx_v_xs);
-  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_xs);
+  __Pyx_INCREF(__pyx_v_x0s);
+  __Pyx_GIVEREF(__pyx_v_x0s);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_x0s);
   __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 300, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 300, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 300, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 300, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_1, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 300, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_DECREF_SET(__pyx_v_xs, __pyx_t_5);
+  __Pyx_DECREF_SET(__pyx_v_x0s, __pyx_t_5);
   __pyx_t_5 = 0;
 
   /* "cyroot/scalar_quasi_newton.pyx":301
  * 
- *     xs = np.asarray(xs, dtype=np.float64)
- *     if xs.shape[0] < 2:             # <<<<<<<<<<<<<<
+ *     x0s = np.asarray(x0s, dtype=np.float64)
+ *     if x0s.shape[0] < 2:             # <<<<<<<<<<<<<<
  *         raise ValueError('Requires at least 2 initial guesses. '
- *                          f'Got {xs.shape[0]}.')
+ *                          f'Got {x0s.shape[0]}.')
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_xs, __pyx_n_s_shape); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 301, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_x0s, __pyx_n_s_shape); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 301, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_6 = __Pyx_GetItemInt(__pyx_t_5, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 301, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = PyObject_RichCompare(__pyx_t_6, __pyx_int_2, Py_LT); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 301, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 301, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (unlikely(__pyx_t_10)) {
 
     /* "cyroot/scalar_quasi_newton.pyx":302
- *     xs = np.asarray(xs, dtype=np.float64)
- *     if xs.shape[0] < 2:
+ *     x0s = np.asarray(x0s, dtype=np.float64)
+ *     if x0s.shape[0] < 2:
  *         raise ValueError('Requires at least 2 initial guesses. '             # <<<<<<<<<<<<<<
- *                          f'Got {xs.shape[0]}.')
- *     _check_initial_guesses_uniqueness(xs)
+ *                          f'Got {x0s.shape[0]}.')
+ *     _check_initial_guesses_uniqueness(x0s)
  */
     __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 302, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_11 = 0;
     __pyx_t_12 = 127;
     __Pyx_INCREF(__pyx_kp_u_Requires_at_least_2_initial_gues);
     __pyx_t_11 += 41;
     __Pyx_GIVEREF(__pyx_kp_u_Requires_at_least_2_initial_gues);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_kp_u_Requires_at_least_2_initial_gues);
 
     /* "cyroot/scalar_quasi_newton.pyx":303
- *     if xs.shape[0] < 2:
+ *     if x0s.shape[0] < 2:
  *         raise ValueError('Requires at least 2 initial guesses. '
- *                          f'Got {xs.shape[0]}.')             # <<<<<<<<<<<<<<
- *     _check_initial_guesses_uniqueness(xs)
+ *                          f'Got {x0s.shape[0]}.')             # <<<<<<<<<<<<<<
+ *     _check_initial_guesses_uniqueness(x0s)
  * 
  */
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_xs, __pyx_n_s_shape); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 303, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_x0s, __pyx_n_s_shape); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 303, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_1 = __Pyx_GetItemInt(__pyx_t_6, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 303, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_t_1, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 303, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -7442,43 +7442,43 @@
     __pyx_t_6 = 0;
     __Pyx_INCREF(__pyx_kp_u__14);
     __pyx_t_11 += 1;
     __Pyx_GIVEREF(__pyx_kp_u__14);
     PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_kp_u__14);
 
     /* "cyroot/scalar_quasi_newton.pyx":302
- *     xs = np.asarray(xs, dtype=np.float64)
- *     if xs.shape[0] < 2:
+ *     x0s = np.asarray(x0s, dtype=np.float64)
+ *     if x0s.shape[0] < 2:
  *         raise ValueError('Requires at least 2 initial guesses. '             # <<<<<<<<<<<<<<
- *                          f'Got {xs.shape[0]}.')
- *     _check_initial_guesses_uniqueness(xs)
+ *                          f'Got {x0s.shape[0]}.')
+ *     _check_initial_guesses_uniqueness(x0s)
  */
     __pyx_t_6 = __Pyx_PyUnicode_Join(__pyx_t_5, 3, __pyx_t_11, __pyx_t_12); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 302, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 302, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_Raise(__pyx_t_5, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __PYX_ERR(0, 302, __pyx_L1_error)
 
     /* "cyroot/scalar_quasi_newton.pyx":301
  * 
- *     xs = np.asarray(xs, dtype=np.float64)
- *     if xs.shape[0] < 2:             # <<<<<<<<<<<<<<
+ *     x0s = np.asarray(x0s, dtype=np.float64)
+ *     if x0s.shape[0] < 2:             # <<<<<<<<<<<<<<
  *         raise ValueError('Requires at least 2 initial guesses. '
- *                          f'Got {xs.shape[0]}.')
+ *                          f'Got {x0s.shape[0]}.')
  */
   }
 
   /* "cyroot/scalar_quasi_newton.pyx":304
  *         raise ValueError('Requires at least 2 initial guesses. '
- *                          f'Got {xs.shape[0]}.')
- *     _check_initial_guesses_uniqueness(xs)             # <<<<<<<<<<<<<<
+ *                          f'Got {x0s.shape[0]}.')
+ *     _check_initial_guesses_uniqueness(x0s)             # <<<<<<<<<<<<<<
  * 
  *     f_wrapper = PyDoubleScalarFPtr.from_f(f)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_check_initial_guesses_uniquenes); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 304, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
@@ -7486,64 +7486,64 @@
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
-  __pyx_t_5 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_1, __pyx_v_xs) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_xs);
+  __pyx_t_5 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_1, __pyx_v_x0s) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_x0s);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 304, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "cyroot/scalar_quasi_newton.pyx":306
- *     _check_initial_guesses_uniqueness(xs)
+ *     _check_initial_guesses_uniqueness(x0s)
  * 
  *     f_wrapper = PyDoubleScalarFPtr.from_f(f)             # <<<<<<<<<<<<<<
- *     if f_xs is None:
- *         f_xs = np.array([f_wrapper.eval(x) for x in xs], dtype=np.float64)
+ *     if f_x0s is None:
+ *         f_x0s = np.array([f_wrapper.eval(x) for x in x0s], dtype=np.float64)
  */
   __pyx_t_5 = ((PyObject *)__pyx_vtabptr_6cyroot_4fptr_PyDoubleScalarFPtr->from_f(__pyx_v_f)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 306, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_v_f_wrapper = ((struct __pyx_obj_6cyroot_4fptr_DoubleScalarFPtr *)__pyx_t_5);
   __pyx_t_5 = 0;
 
   /* "cyroot/scalar_quasi_newton.pyx":307
  * 
  *     f_wrapper = PyDoubleScalarFPtr.from_f(f)
- *     if f_xs is None:             # <<<<<<<<<<<<<<
- *         f_xs = np.array([f_wrapper.eval(x) for x in xs], dtype=np.float64)
+ *     if f_x0s is None:             # <<<<<<<<<<<<<<
+ *         f_x0s = np.array([f_wrapper.eval(x) for x in x0s], dtype=np.float64)
  *     else:
  */
-  __pyx_t_10 = (__pyx_v_f_xs == Py_None);
+  __pyx_t_10 = (__pyx_v_f_x0s == Py_None);
   __pyx_t_13 = (__pyx_t_10 != 0);
   if (__pyx_t_13) {
 
     /* "cyroot/scalar_quasi_newton.pyx":308
  *     f_wrapper = PyDoubleScalarFPtr.from_f(f)
- *     if f_xs is None:
- *         f_xs = np.array([f_wrapper.eval(x) for x in xs], dtype=np.float64)             # <<<<<<<<<<<<<<
+ *     if f_x0s is None:
+ *         f_x0s = np.array([f_wrapper.eval(x) for x in x0s], dtype=np.float64)             # <<<<<<<<<<<<<<
  *     else:
- *         f_xs = np.asarray(f_xs, dtype=np.float64)
+ *         f_x0s = np.asarray(f_x0s, dtype=np.float64)
  */
     __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 308, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_array); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 308, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     { /* enter inner scope */
       __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 308, __pyx_L9_error)
       __Pyx_GOTREF(__pyx_t_5);
-      if (likely(PyList_CheckExact(__pyx_v_xs)) || PyTuple_CheckExact(__pyx_v_xs)) {
-        __pyx_t_1 = __pyx_v_xs; __Pyx_INCREF(__pyx_t_1); __pyx_t_11 = 0;
+      if (likely(PyList_CheckExact(__pyx_v_x0s)) || PyTuple_CheckExact(__pyx_v_x0s)) {
+        __pyx_t_1 = __pyx_v_x0s; __Pyx_INCREF(__pyx_t_1); __pyx_t_11 = 0;
         __pyx_t_14 = NULL;
       } else {
-        __pyx_t_11 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_xs); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 308, __pyx_L9_error)
+        __pyx_t_11 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_x0s); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 308, __pyx_L9_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_t_14 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 308, __pyx_L9_error)
       }
       for (;;) {
         if (likely(!__pyx_t_14)) {
           if (likely(PyList_CheckExact(__pyx_t_1))) {
             if (__pyx_t_11 >= PyList_GET_SIZE(__pyx_t_1)) break;
@@ -7606,110 +7606,110 @@
     if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 308, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_1, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 308, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_DECREF_SET(__pyx_v_f_xs, __pyx_t_3);
+    __Pyx_DECREF_SET(__pyx_v_f_x0s, __pyx_t_3);
     __pyx_t_3 = 0;
 
     /* "cyroot/scalar_quasi_newton.pyx":307
  * 
  *     f_wrapper = PyDoubleScalarFPtr.from_f(f)
- *     if f_xs is None:             # <<<<<<<<<<<<<<
- *         f_xs = np.array([f_wrapper.eval(x) for x in xs], dtype=np.float64)
+ *     if f_x0s is None:             # <<<<<<<<<<<<<<
+ *         f_x0s = np.array([f_wrapper.eval(x) for x in x0s], dtype=np.float64)
  *     else:
  */
     goto __pyx_L6;
   }
 
   /* "cyroot/scalar_quasi_newton.pyx":310
- *         f_xs = np.array([f_wrapper.eval(x) for x in xs], dtype=np.float64)
+ *         f_x0s = np.array([f_wrapper.eval(x) for x in x0s], dtype=np.float64)
  *     else:
- *         f_xs = np.asarray(f_xs, dtype=np.float64)             # <<<<<<<<<<<<<<
- *         if xs.shape[0] != f_xs.shape[0]:
+ *         f_x0s = np.asarray(f_x0s, dtype=np.float64)             # <<<<<<<<<<<<<<
+ *         if x0s.shape[0] != f_x0s.shape[0]:
  *             raise ValueError('xs and f_xs must have same size. '
  */
   /*else*/ {
     __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 310, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_asarray); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 310, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 310, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_INCREF(__pyx_v_f_xs);
-    __Pyx_GIVEREF(__pyx_v_f_xs);
-    PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_f_xs);
+    __Pyx_INCREF(__pyx_v_f_x0s);
+    __Pyx_GIVEREF(__pyx_v_f_x0s);
+    PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_f_x0s);
     __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 310, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 310, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_float64); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 310, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 310, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 310, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF_SET(__pyx_v_f_xs, __pyx_t_7);
+    __Pyx_DECREF_SET(__pyx_v_f_x0s, __pyx_t_7);
     __pyx_t_7 = 0;
 
     /* "cyroot/scalar_quasi_newton.pyx":311
  *     else:
- *         f_xs = np.asarray(f_xs, dtype=np.float64)
- *         if xs.shape[0] != f_xs.shape[0]:             # <<<<<<<<<<<<<<
+ *         f_x0s = np.asarray(f_x0s, dtype=np.float64)
+ *         if x0s.shape[0] != f_x0s.shape[0]:             # <<<<<<<<<<<<<<
  *             raise ValueError('xs and f_xs must have same size. '
- *                              f'Got {xs.shape[0]} and {f_xs.shape[0]}.')
+ *                              f'Got {x0s.shape[0]} and {f_x0s.shape[0]}.')
  */
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_xs, __pyx_n_s_shape); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 311, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_x0s, __pyx_n_s_shape); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 311, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_1 = __Pyx_GetItemInt(__pyx_t_7, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 311, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_f_xs, __pyx_n_s_shape); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 311, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_f_x0s, __pyx_n_s_shape); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 311, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_7, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 311, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_t_7 = PyObject_RichCompare(__pyx_t_1, __pyx_t_3, Py_NE); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 311, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_13 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_13 < 0)) __PYX_ERR(0, 311, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     if (unlikely(__pyx_t_13)) {
 
       /* "cyroot/scalar_quasi_newton.pyx":312
- *         f_xs = np.asarray(f_xs, dtype=np.float64)
- *         if xs.shape[0] != f_xs.shape[0]:
+ *         f_x0s = np.asarray(f_x0s, dtype=np.float64)
+ *         if x0s.shape[0] != f_x0s.shape[0]:
  *             raise ValueError('xs and f_xs must have same size. '             # <<<<<<<<<<<<<<
- *                              f'Got {xs.shape[0]} and {f_xs.shape[0]}.')
- *     _check_initial_guesses_uniqueness(f_xs)
+ *                              f'Got {x0s.shape[0]} and {f_x0s.shape[0]}.')
+ *     _check_initial_guesses_uniqueness(f_x0s)
  */
       __pyx_t_7 = PyTuple_New(5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 312, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_11 = 0;
       __pyx_t_12 = 127;
       __Pyx_INCREF(__pyx_kp_u_xs_and_f_xs_must_have_same_size);
       __pyx_t_11 += 37;
       __Pyx_GIVEREF(__pyx_kp_u_xs_and_f_xs_must_have_same_size);
       PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_kp_u_xs_and_f_xs_must_have_same_size);
 
       /* "cyroot/scalar_quasi_newton.pyx":313
- *         if xs.shape[0] != f_xs.shape[0]:
+ *         if x0s.shape[0] != f_x0s.shape[0]:
  *             raise ValueError('xs and f_xs must have same size. '
- *                              f'Got {xs.shape[0]} and {f_xs.shape[0]}.')             # <<<<<<<<<<<<<<
- *     _check_initial_guesses_uniqueness(f_xs)
+ *                              f'Got {x0s.shape[0]} and {f_x0s.shape[0]}.')             # <<<<<<<<<<<<<<
+ *     _check_initial_guesses_uniqueness(f_x0s)
  * 
  */
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_xs, __pyx_n_s_shape); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 313, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_x0s, __pyx_n_s_shape); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 313, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_1 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 313, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_3 = __Pyx_PyObject_FormatSimple(__pyx_t_1, __pyx_empty_unicode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 313, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -7718,15 +7718,15 @@
       __Pyx_GIVEREF(__pyx_t_3);
       PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_3);
       __pyx_t_3 = 0;
       __Pyx_INCREF(__pyx_kp_u_and);
       __pyx_t_11 += 5;
       __Pyx_GIVEREF(__pyx_kp_u_and);
       PyTuple_SET_ITEM(__pyx_t_7, 2, __pyx_kp_u_and);
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_f_xs, __pyx_n_s_shape); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 313, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_f_x0s, __pyx_n_s_shape); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 313, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_1 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 313, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_3 = __Pyx_PyObject_FormatSimple(__pyx_t_1, __pyx_empty_unicode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 313, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -7737,76 +7737,76 @@
       __pyx_t_3 = 0;
       __Pyx_INCREF(__pyx_kp_u__14);
       __pyx_t_11 += 1;
       __Pyx_GIVEREF(__pyx_kp_u__14);
       PyTuple_SET_ITEM(__pyx_t_7, 4, __pyx_kp_u__14);
 
       /* "cyroot/scalar_quasi_newton.pyx":312
- *         f_xs = np.asarray(f_xs, dtype=np.float64)
- *         if xs.shape[0] != f_xs.shape[0]:
+ *         f_x0s = np.asarray(f_x0s, dtype=np.float64)
+ *         if x0s.shape[0] != f_x0s.shape[0]:
  *             raise ValueError('xs and f_xs must have same size. '             # <<<<<<<<<<<<<<
- *                              f'Got {xs.shape[0]} and {f_xs.shape[0]}.')
- *     _check_initial_guesses_uniqueness(f_xs)
+ *                              f'Got {x0s.shape[0]} and {f_x0s.shape[0]}.')
+ *     _check_initial_guesses_uniqueness(f_x0s)
  */
       __pyx_t_3 = __Pyx_PyUnicode_Join(__pyx_t_7, 5, __pyx_t_11, __pyx_t_12); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 312, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __pyx_t_7 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 312, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_Raise(__pyx_t_7, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __PYX_ERR(0, 312, __pyx_L1_error)
 
       /* "cyroot/scalar_quasi_newton.pyx":311
  *     else:
- *         f_xs = np.asarray(f_xs, dtype=np.float64)
- *         if xs.shape[0] != f_xs.shape[0]:             # <<<<<<<<<<<<<<
+ *         f_x0s = np.asarray(f_x0s, dtype=np.float64)
+ *         if x0s.shape[0] != f_x0s.shape[0]:             # <<<<<<<<<<<<<<
  *             raise ValueError('xs and f_xs must have same size. '
- *                              f'Got {xs.shape[0]} and {f_xs.shape[0]}.')
+ *                              f'Got {x0s.shape[0]} and {f_x0s.shape[0]}.')
  */
     }
   }
   __pyx_L6:;
 
   /* "cyroot/scalar_quasi_newton.pyx":314
  *             raise ValueError('xs and f_xs must have same size. '
- *                              f'Got {xs.shape[0]} and {f_xs.shape[0]}.')
- *     _check_initial_guesses_uniqueness(f_xs)             # <<<<<<<<<<<<<<
+ *                              f'Got {x0s.shape[0]} and {f_x0s.shape[0]}.')
+ *     _check_initial_guesses_uniqueness(f_x0s)             # <<<<<<<<<<<<<<
  * 
- *     res = sidi_kernel(f_wrapper, xs, f_xs, etol, ertol, ptol, prtol, max_iter)
+ *     res = sidi_kernel(f_wrapper, x0s, f_x0s, etol, ertol, ptol, prtol, max_iter)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_check_initial_guesses_uniquenes); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 314, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
-  __pyx_t_7 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_1, __pyx_v_f_xs) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_f_xs);
+  __pyx_t_7 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_1, __pyx_v_f_x0s) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_f_x0s);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 314, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "cyroot/scalar_quasi_newton.pyx":316
- *     _check_initial_guesses_uniqueness(f_xs)
+ *     _check_initial_guesses_uniqueness(f_x0s)
  * 
- *     res = sidi_kernel(f_wrapper, xs, f_xs, etol, ertol, ptol, prtol, max_iter)             # <<<<<<<<<<<<<<
+ *     res = sidi_kernel(f_wrapper, x0s, f_x0s, etol, ertol, ptol, prtol, max_iter)             # <<<<<<<<<<<<<<
  *     return QuasiNewtonMethodReturnType.from_results(res, f_wrapper.n_f_calls)
  * 
  */
-  __pyx_t_17 = __Pyx_PyObject_to_MemoryviewSlice_ds_double(__pyx_v_xs, PyBUF_WRITABLE); if (unlikely(!__pyx_t_17.memview)) __PYX_ERR(0, 316, __pyx_L1_error)
-  __pyx_t_18 = __Pyx_PyObject_to_MemoryviewSlice_ds_double(__pyx_v_f_xs, PyBUF_WRITABLE); if (unlikely(!__pyx_t_18.memview)) __PYX_ERR(0, 316, __pyx_L1_error)
+  __pyx_t_17 = __Pyx_PyObject_to_MemoryviewSlice_ds_double(__pyx_v_x0s, PyBUF_WRITABLE); if (unlikely(!__pyx_t_17.memview)) __PYX_ERR(0, 316, __pyx_L1_error)
+  __pyx_t_18 = __Pyx_PyObject_to_MemoryviewSlice_ds_double(__pyx_v_f_x0s, PyBUF_WRITABLE); if (unlikely(!__pyx_t_18.memview)) __PYX_ERR(0, 316, __pyx_L1_error)
   __pyx_t_16 = __pyx_PyFloat_AsDouble(__pyx_v_etol); if (unlikely((__pyx_t_16 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 316, __pyx_L1_error)
   __pyx_t_15 = __pyx_PyFloat_AsDouble(__pyx_v_ertol); if (unlikely((__pyx_t_15 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 316, __pyx_L1_error)
   __pyx_t_19 = __pyx_PyFloat_AsDouble(__pyx_v_ptol); if (unlikely((__pyx_t_19 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 316, __pyx_L1_error)
   __pyx_t_20 = __pyx_PyFloat_AsDouble(__pyx_v_prtol); if (unlikely((__pyx_t_20 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 316, __pyx_L1_error)
   __pyx_t_21 = __Pyx_PyInt_As_unsigned_long(__pyx_v_max_iter); if (unlikely((__pyx_t_21 == (unsigned long)-1) && PyErr_Occurred())) __PYX_ERR(0, 316, __pyx_L1_error)
   __pyx_t_23.__pyx_n = 5;
   __pyx_t_23.etol = __pyx_t_16;
@@ -7824,15 +7824,15 @@
   __pyx_t_7 = __pyx_convert__to_py___pyx_ctuple_de07d9__double__and_double__and_unsigned__space_long__and_double__and_double__and_int__and_int__etc(__pyx_t_22); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 316, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_v_res = __pyx_t_7;
   __pyx_t_7 = 0;
 
   /* "cyroot/scalar_quasi_newton.pyx":317
  * 
- *     res = sidi_kernel(f_wrapper, xs, f_xs, etol, ertol, ptol, prtol, max_iter)
+ *     res = sidi_kernel(f_wrapper, x0s, f_x0s, etol, ertol, ptol, prtol, max_iter)
  *     return QuasiNewtonMethodReturnType.from_results(res, f_wrapper.n_f_calls)             # <<<<<<<<<<<<<<
  * 
  * ################################################################################
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_QuasiNewtonMethodReturnType); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 317, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
@@ -7892,16 +7892,16 @@
   __pyx_t_7 = 0;
   goto __pyx_L0;
 
   /* "cyroot/scalar_quasi_newton.pyx":265
  * @dynamic_default_args()
  * @cython.binding(True)
  * def sidi(f: Callable[[float], float],             # <<<<<<<<<<<<<<
- *          xs: VectorLike,
- *          f_xs: Optional[VectorLike] = None,
+ *          x0s: VectorLike,
+ *          f_x0s: Optional[VectorLike] = None,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
@@ -7913,16 +7913,16 @@
   __PYX_XDEC_MEMVIEW(&__pyx_t_18, 1);
   __Pyx_AddTraceback("cyroot.scalar_quasi_newton.sidi", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_f_wrapper);
   __Pyx_XDECREF(__pyx_v_res);
   __Pyx_XDECREF(__pyx_7genexpr__pyx_v_x);
-  __Pyx_XDECREF(__pyx_v_xs);
-  __Pyx_XDECREF(__pyx_v_f_xs);
+  __Pyx_XDECREF(__pyx_v_x0s);
+  __Pyx_XDECREF(__pyx_v_f_x0s);
   __Pyx_XDECREF(__pyx_v_etol);
   __Pyx_XDECREF(__pyx_v_ertol);
   __Pyx_XDECREF(__pyx_v_ptol);
   __Pyx_XDECREF(__pyx_v_prtol);
   __Pyx_XDECREF(__pyx_v_max_iter);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -13082,15 +13082,15 @@
   __Pyx_XDECREF(__pyx_v_prtol);
   __Pyx_XDECREF(__pyx_v_max_iter);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -13099,29 +13099,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -13132,15 +13132,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -13149,29 +13149,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -13182,15 +13182,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -13199,29 +13199,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -13232,15 +13232,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -13249,29 +13249,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -13282,15 +13282,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -13299,29 +13299,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -13332,212 +13332,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -13553,15 +13553,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -13569,53 +13569,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 942, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__35, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 944, __pyx_L5_except_error)
@@ -13623,30 +13623,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -13661,15 +13661,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -13685,15 +13685,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -13701,53 +13701,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 948, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__36, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 950, __pyx_L5_except_error)
@@ -13755,30 +13755,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -13793,15 +13793,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -13817,15 +13817,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -13833,53 +13833,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 954, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__36, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 956, __pyx_L5_except_error)
@@ -13887,30 +13887,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -13925,176 +13925,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -28461,17 +28461,17 @@
   {&__pyx_n_s_enumerate, __pyx_k_enumerate, sizeof(__pyx_k_enumerate), 0, 0, 1, 1},
   {&__pyx_n_s_error, __pyx_k_error, sizeof(__pyx_k_error), 0, 0, 1, 1},
   {&__pyx_n_s_ertol, __pyx_k_ertol, sizeof(__pyx_k_ertol), 0, 0, 1, 1},
   {&__pyx_n_s_etol, __pyx_k_etol, sizeof(__pyx_k_etol), 0, 0, 1, 1},
   {&__pyx_n_s_f, __pyx_k_f, sizeof(__pyx_k_f), 0, 0, 1, 1},
   {&__pyx_n_s_f_wrapper, __pyx_k_f_wrapper, sizeof(__pyx_k_f_wrapper), 0, 0, 1, 1},
   {&__pyx_n_s_f_x0, __pyx_k_f_x0, sizeof(__pyx_k_f_x0), 0, 0, 1, 1},
+  {&__pyx_n_s_f_x0s, __pyx_k_f_x0s, sizeof(__pyx_k_f_x0s), 0, 0, 1, 1},
   {&__pyx_n_s_f_x1, __pyx_k_f_x1, sizeof(__pyx_k_f_x1), 0, 0, 1, 1},
   {&__pyx_n_s_f_x2, __pyx_k_f_x2, sizeof(__pyx_k_f_x2), 0, 0, 1, 1},
-  {&__pyx_n_s_f_xs, __pyx_k_f_xs, sizeof(__pyx_k_f_xs), 0, 0, 1, 1},
   {&__pyx_n_s_flags, __pyx_k_flags, sizeof(__pyx_k_flags), 0, 0, 1, 1},
   {&__pyx_n_u_float, __pyx_k_float, sizeof(__pyx_k_float), 0, 1, 0, 1},
   {&__pyx_n_s_float64, __pyx_k_float64, sizeof(__pyx_k_float64), 0, 0, 1, 1},
   {&__pyx_n_s_format, __pyx_k_format, sizeof(__pyx_k_format), 0, 0, 1, 1},
   {&__pyx_n_s_fortran, __pyx_k_fortran, sizeof(__pyx_k_fortran), 0, 0, 1, 1},
   {&__pyx_n_u_fortran, __pyx_k_fortran, sizeof(__pyx_k_fortran), 0, 1, 0, 1},
   {&__pyx_n_s_from_results, __pyx_k_from_results, sizeof(__pyx_k_from_results), 0, 0, 1, 1},
@@ -28549,17 +28549,17 @@
   {&__pyx_kp_s_unable_to_allocate_array_data, __pyx_k_unable_to_allocate_array_data, sizeof(__pyx_k_unable_to_allocate_array_data), 0, 0, 1, 0},
   {&__pyx_kp_s_unable_to_allocate_shape_and_str, __pyx_k_unable_to_allocate_shape_and_str, sizeof(__pyx_k_unable_to_allocate_shape_and_str), 0, 0, 1, 0},
   {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_utils_function_tagging, __pyx_k_utils_function_tagging, sizeof(__pyx_k_utils_function_tagging), 0, 0, 1, 1},
   {&__pyx_n_s_x, __pyx_k_x, sizeof(__pyx_k_x), 0, 0, 1, 1},
   {&__pyx_n_s_x0, __pyx_k_x0, sizeof(__pyx_k_x0), 0, 0, 1, 1},
+  {&__pyx_n_s_x0s, __pyx_k_x0s, sizeof(__pyx_k_x0s), 0, 0, 1, 1},
   {&__pyx_n_s_x1, __pyx_k_x1, sizeof(__pyx_k_x1), 0, 0, 1, 1},
   {&__pyx_n_s_x2, __pyx_k_x2, sizeof(__pyx_k_x2), 0, 0, 1, 1},
-  {&__pyx_n_s_xs, __pyx_k_xs, sizeof(__pyx_k_xs), 0, 0, 1, 1},
   {&__pyx_kp_u_xs_and_f_xs_must_have_same_size, __pyx_k_xs_and_f_xs_must_have_same_size, sizeof(__pyx_k_xs_and_f_xs_must_have_same_size), 0, 1, 0, 0},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 228, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 302, __pyx_L1_error)
@@ -28604,26 +28604,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__35 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(2, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__35);
   __Pyx_GIVEREF(__pyx_tuple__35);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__36 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(2, 950, __pyx_L1_error)
@@ -28848,18 +28848,18 @@
   __Pyx_GIVEREF(__pyx_tuple__62);
   __pyx_codeobj__63 = (PyObject*)__Pyx_PyCode_New(10, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__62, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cyroot_scalar_quasi_newton_pyx, __pyx_n_s_secant, 96, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__63)) __PYX_ERR(0, 96, __pyx_L1_error)
 
   /* "cyroot/scalar_quasi_newton.pyx":265
  * @dynamic_default_args()
  * @cython.binding(True)
  * def sidi(f: Callable[[float], float],             # <<<<<<<<<<<<<<
- *          xs: VectorLike,
- *          f_xs: Optional[VectorLike] = None,
+ *          x0s: VectorLike,
+ *          f_x0s: Optional[VectorLike] = None,
  */
-  __pyx_tuple__64 = PyTuple_Pack(11, __pyx_n_s_f, __pyx_n_s_xs, __pyx_n_s_f_xs, __pyx_n_s_etol, __pyx_n_s_ertol, __pyx_n_s_ptol, __pyx_n_s_prtol, __pyx_n_s_max_iter, __pyx_n_s_f_wrapper, __pyx_n_s_res, __pyx_n_s_x); if (unlikely(!__pyx_tuple__64)) __PYX_ERR(0, 265, __pyx_L1_error)
+  __pyx_tuple__64 = PyTuple_Pack(11, __pyx_n_s_f, __pyx_n_s_x0s, __pyx_n_s_f_x0s, __pyx_n_s_etol, __pyx_n_s_ertol, __pyx_n_s_ptol, __pyx_n_s_prtol, __pyx_n_s_max_iter, __pyx_n_s_f_wrapper, __pyx_n_s_res, __pyx_n_s_x); if (unlikely(!__pyx_tuple__64)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__64);
   __Pyx_GIVEREF(__pyx_tuple__64);
   __pyx_codeobj__65 = (PyObject*)__Pyx_PyCode_New(8, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__64, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cyroot_scalar_quasi_newton_pyx, __pyx_n_s_sidi, 265, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__65)) __PYX_ERR(0, 265, __pyx_L1_error)
 
   /* "cyroot/scalar_quasi_newton.pyx":371
  * @dynamic_default_args()
  * @cython.binding(True)
@@ -30197,16 +30197,16 @@
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "cyroot/scalar_quasi_newton.pyx":265
  * @dynamic_default_args()
  * @cython.binding(True)
  * def sidi(f: Callable[[float], float],             # <<<<<<<<<<<<<<
- *          xs: VectorLike,
- *          f_xs: Optional[VectorLike] = None,
+ *          x0s: VectorLike,
+ *          f_x0s: Optional[VectorLike] = None,
  */
   __pyx_t_7 = __Pyx_PyDict_NewPresized(9); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Callable); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_9 = PyList_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
@@ -30227,39 +30227,39 @@
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_f, __pyx_t_9) < 0) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
   /* "cyroot/scalar_quasi_newton.pyx":266
  * @cython.binding(True)
  * def sidi(f: Callable[[float], float],
- *          xs: VectorLike,             # <<<<<<<<<<<<<<
- *          f_xs: Optional[VectorLike] = None,
+ *          x0s: VectorLike,             # <<<<<<<<<<<<<<
+ *          f_x0s: Optional[VectorLike] = None,
  *          etol: float = named_default(ETOL=ETOL),
  */
   __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_VectorLike); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 266, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_xs, __pyx_t_9) < 0) __PYX_ERR(0, 265, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_x0s, __pyx_t_9) < 0) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
   /* "cyroot/scalar_quasi_newton.pyx":267
  * def sidi(f: Callable[[float], float],
- *          xs: VectorLike,
- *          f_xs: Optional[VectorLike] = None,             # <<<<<<<<<<<<<<
+ *          x0s: VectorLike,
+ *          f_x0s: Optional[VectorLike] = None,             # <<<<<<<<<<<<<<
  *          etol: float = named_default(ETOL=ETOL),
  *          ertol: float = named_default(ERTOL=ERTOL),
  */
   __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_Optional); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 267, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_VectorLike); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 267, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_t_9, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 267, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_f_xs, __pyx_t_5) < 0) __PYX_ERR(0, 265, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_f_x0s, __pyx_t_5) < 0) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_etol, __pyx_n_u_float) < 0) __PYX_ERR(0, 265, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_ertol, __pyx_n_u_float) < 0) __PYX_ERR(0, 265, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_ptol, __pyx_n_u_float) < 0) __PYX_ERR(0, 265, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_prtol, __pyx_n_u_float) < 0) __PYX_ERR(0, 265, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_max_iter, __pyx_n_u_int) < 0) __PYX_ERR(0, 265, __pyx_L1_error)
 
@@ -30275,24 +30275,24 @@
   if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_return, __pyx_t_5) < 0) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "cyroot/scalar_quasi_newton.pyx":265
  * @dynamic_default_args()
  * @cython.binding(True)
  * def sidi(f: Callable[[float], float],             # <<<<<<<<<<<<<<
- *          xs: VectorLike,
- *          f_xs: Optional[VectorLike] = None,
+ *          x0s: VectorLike,
+ *          f_x0s: Optional[VectorLike] = None,
  */
   __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_6cyroot_19scalar_quasi_newton_3sidi, 0, __pyx_n_s_sidi, NULL, __pyx_n_s_cyroot_scalar_quasi_newton_2, __pyx_d, ((PyObject *)__pyx_codeobj__65)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (!__Pyx_CyFunction_InitDefaults(__pyx_t_5, sizeof(__pyx_defaults1), 5)) __PYX_ERR(0, 265, __pyx_L1_error)
 
   /* "cyroot/scalar_quasi_newton.pyx":268
- *          xs: VectorLike,
- *          f_xs: Optional[VectorLike] = None,
+ *          x0s: VectorLike,
+ *          f_x0s: Optional[VectorLike] = None,
  *          etol: float = named_default(ETOL=ETOL),             # <<<<<<<<<<<<<<
  *          ertol: float = named_default(ERTOL=ERTOL),
  *          ptol: float = named_default(PTOL=PTOL),
  */
   __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_named_default); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 268, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_9 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 268, __pyx_L1_error)
@@ -30306,15 +30306,15 @@
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_t_5)->__pyx_arg_etol = __pyx_t_8;
   __Pyx_GIVEREF(__pyx_t_8);
   __pyx_t_8 = 0;
 
   /* "cyroot/scalar_quasi_newton.pyx":269
- *          f_xs: Optional[VectorLike] = None,
+ *          f_x0s: Optional[VectorLike] = None,
  *          etol: float = named_default(ETOL=ETOL),
  *          ertol: float = named_default(ERTOL=ERTOL),             # <<<<<<<<<<<<<<
  *          ptol: float = named_default(PTOL=PTOL),
  *          prtol: float = named_default(PRTOL=PRTOL),
  */
   __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_named_default); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 269, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
```

### Comparing `cy-root-1.0.1/cyroot/scalar_quasi_newton.pyx` & `cy-root-1.0.2/cyroot/scalar_quasi_newton.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -259,28 +259,28 @@
         return out[-1]
 
 # noinspection DuplicatedCode
 @tag('cyroot.scalar.quasi_newton')
 @dynamic_default_args()
 @cython.binding(True)
 def sidi(f: Callable[[float], float],
-         xs: VectorLike,
-         f_xs: Optional[VectorLike] = None,
+         x0s: VectorLike,
+         f_x0s: Optional[VectorLike] = None,
          etol: float = named_default(ETOL=ETOL),
          ertol: float = named_default(ERTOL=ERTOL),
          ptol: float = named_default(PTOL=PTOL),
          prtol: float = named_default(PRTOL=PRTOL),
          max_iter: int = named_default(MAX_ITER=MAX_ITER)) -> QuasiNewtonMethodReturnType:
     """
     Sidi's Generalized Secant method for scalar root-finding.
 
     Args:
         f (function): Function for which the root is sought.
-        xs (tuple of float): Tuple of initial points.
-        f_xs (tuple of float, optional): Tuple of values evaluated at initial points.
+        x0s (tuple of float): Tuple of initial points.
+        f_x0s (tuple of float, optional): Tuple of values evaluated at initial points.
         etol (float, optional): Error tolerance, indicating the
          desired precision of the root. Defaults to {etol}.
         ertol (float, optional): Relative error tolerance.
          Defaults to {ertol}.
         ptol (float, optional): Precision tolerance, indicating
          the minimum change of root approximations or width of
          brackets (in bracketing methods) after each iteration.
@@ -293,31 +293,31 @@
 
     Returns:
         solution: The solution represented as a ``RootResults`` object.
     """
     # check params
     etol, ertol, ptol, prtol, max_iter = _check_stop_cond_args(etol, ertol, ptol, prtol, max_iter)
 
-    xs = np.asarray(xs, dtype=np.float64)
-    if xs.shape[0] < 2:
+    x0s = np.asarray(x0s, dtype=np.float64)
+    if x0s.shape[0] < 2:
         raise ValueError('Requires at least 2 initial guesses. '
-                         f'Got {xs.shape[0]}.')
-    _check_initial_guesses_uniqueness(xs)
+                         f'Got {x0s.shape[0]}.')
+    _check_initial_guesses_uniqueness(x0s)
 
     f_wrapper = PyDoubleScalarFPtr.from_f(f)
-    if f_xs is None:
-        f_xs = np.array([f_wrapper.eval(x) for x in xs], dtype=np.float64)
+    if f_x0s is None:
+        f_x0s = np.array([f_wrapper.eval(x) for x in x0s], dtype=np.float64)
     else:
-        f_xs = np.asarray(f_xs, dtype=np.float64)
-        if xs.shape[0] != f_xs.shape[0]:
+        f_x0s = np.asarray(f_x0s, dtype=np.float64)
+        if x0s.shape[0] != f_x0s.shape[0]:
             raise ValueError('xs and f_xs must have same size. '
-                             f'Got {xs.shape[0]} and {f_xs.shape[0]}.')
-    _check_initial_guesses_uniqueness(f_xs)
+                             f'Got {x0s.shape[0]} and {f_x0s.shape[0]}.')
+    _check_initial_guesses_uniqueness(f_x0s)
 
-    res = sidi_kernel(f_wrapper, xs, f_xs, etol, ertol, ptol, prtol, max_iter)
+    res = sidi_kernel(f_wrapper, x0s, f_x0s, etol, ertol, ptol, prtol, max_iter)
     return QuasiNewtonMethodReturnType.from_results(res, f_wrapper.n_f_calls)
 
 ################################################################################
 # Steffensen
 ################################################################################
 # noinspection DuplicatedCode
 cdef (double, double, unsigned long, double, double, bint, bint) \
```

### Comparing `cy-root-1.0.1/cyroot/scalar_root.py` & `cy-root-1.0.2/cyroot/scalar_root.py`

 * *Files identical despite different names*

### Comparing `cy-root-1.0.1/cyroot/utils/function_tagging.py` & `cy-root-1.0.2/cyroot/utils/function_tagging.py`

 * *Files identical despite different names*

### Comparing `cy-root-1.0.1/cyroot/utils/itertools.cpp` & `cy-root-1.0.2/cyroot/utils/itertools.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
             "cyroot",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include",
             "cyroot/ops",
             "cyroot/utils"
         ],
         "language": "c++",
         "name": "cyroot.utils.itertools",
         "sources": [
             "cyroot/utils/itertools.pyx"
@@ -1166,195 +1166,195 @@
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
 #define __Pyx_FastGilFuncInit()
 
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1385,42 +1385,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1428,28 +1428,28 @@
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_cisclose;
 
 /* "scalar_ops.pxd":18
  *     double complex
  * 
  * cdef bint isclose(double a, double b, double rtol=*, double atol=*) nogil             # <<<<<<<<<<<<<<
  * cdef bint cisclose(double complex a, double complex b, double rtol=*, double atol=*) nogil
- * 
+ * cdef real min(real a, real b) nogil
  */
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_isclose {
   int __pyx_n;
   double rtol;
   double atol;
 };
 
 /* "scalar_ops.pxd":19
  * 
  * cdef bint isclose(double a, double b, double rtol=*, double atol=*) nogil
  * cdef bint cisclose(double complex a, double complex b, double rtol=*, double atol=*) nogil             # <<<<<<<<<<<<<<
- * 
- * cdef extern from '<math.h>' nogil:
+ * cdef real min(real a, real b) nogil
+ * cdef real max(real a, real b) nogil
  */
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_cisclose {
   int __pyx_n;
   double rtol;
   double atol;
 };
 struct __pyx_opt_args_6cyroot_3ops_10vector_ops_allclose;
@@ -3315,15 +3315,15 @@
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_ns, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3332,29 +3332,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3365,15 +3365,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3382,29 +3382,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3415,15 +3415,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3432,29 +3432,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3465,15 +3465,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3482,29 +3482,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3515,15 +3515,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3532,29 +3532,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3565,212 +3565,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3786,15 +3786,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -3802,53 +3802,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
@@ -3856,30 +3856,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3894,15 +3894,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3918,15 +3918,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3934,53 +3934,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
@@ -3988,30 +3988,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4026,15 +4026,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4050,15 +4050,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4066,53 +4066,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
@@ -4120,30 +4120,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4158,176 +4158,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -18279,26 +18279,26 @@
   __pyx_tuple_ = PyTuple_Pack(2, __pyx_int_0, __pyx_int_0); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_tuple_); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 950, __pyx_L1_error)
```

### Comparing `cy-root-1.0.1/cyroot/utils/itertools.pyx` & `cy-root-1.0.2/cyroot/utils/itertools.pyx`

 * *Files identical despite different names*

### Comparing `cy-root-1.0.1/cyroot/vector_bracketing.cpp` & `cy-root-1.0.2/cyroot/vector_bracketing.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
             "cyroot",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include",
             "cyroot/ops",
             "cyroot/utils"
         ],
         "language": "c++",
         "name": "cyroot.vector_bracketing",
         "sources": [
             "cyroot/vector_bracketing.pyx"
@@ -1167,195 +1167,195 @@
 
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
 
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1412,42 +1412,42 @@
 struct __pyx_obj_6cyroot_17vector_bracketing___pyx_scope_struct_2_genexpr;
 struct __pyx_obj_6cyroot_17vector_bracketing___pyx_scope_struct_3_genexpr;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1548,28 +1548,28 @@
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_cisclose;
 
 /* "scalar_ops.pxd":18
  *     double complex
  * 
  * cdef bint isclose(double a, double b, double rtol=*, double atol=*) nogil             # <<<<<<<<<<<<<<
  * cdef bint cisclose(double complex a, double complex b, double rtol=*, double atol=*) nogil
- * 
+ * cdef real min(real a, real b) nogil
  */
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_isclose {
   int __pyx_n;
   double rtol;
   double atol;
 };
 
 /* "scalar_ops.pxd":19
  * 
  * cdef bint isclose(double a, double b, double rtol=*, double atol=*) nogil
  * cdef bint cisclose(double complex a, double complex b, double rtol=*, double atol=*) nogil             # <<<<<<<<<<<<<<
- * 
- * cdef extern from '<math.h>' nogil:
+ * cdef real min(real a, real b) nogil
+ * cdef real max(real a, real b) nogil
  */
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_cisclose {
   int __pyx_n;
   double rtol;
   double atol;
 };
 struct __pyx_opt_args_6cyroot_3ops_10vector_ops_allclose;
@@ -12038,15 +12038,15 @@
   __Pyx_XDECREF(__pyx_v_prtol);
   __Pyx_XDECREF(__pyx_v_max_iter);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -12055,29 +12055,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -12088,15 +12088,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -12105,29 +12105,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -12138,15 +12138,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -12155,29 +12155,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -12188,15 +12188,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -12205,29 +12205,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -12238,15 +12238,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -12255,29 +12255,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -12288,212 +12288,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -12509,15 +12509,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -12525,53 +12525,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
@@ -12579,30 +12579,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -12617,15 +12617,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -12641,15 +12641,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -12657,53 +12657,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
@@ -12711,30 +12711,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -12749,15 +12749,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -12773,15 +12773,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -12789,53 +12789,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
@@ -12843,30 +12843,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -12881,176 +12881,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -27867,26 +27867,26 @@
  *     if x0s.shape[0] != 2 ** F_x0s.shape[1]:
  *         raise ValueError('Initial bounds do not form an admissible n-polygon. '
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_x0s_and_F_x0s_must_have_same_len); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 359, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 950, __pyx_L1_error)
```

### Comparing `cy-root-1.0.1/cyroot/vector_bracketing.pyx` & `cy-root-1.0.2/cyroot/vector_bracketing.pyx`

 * *Files identical despite different names*

### Comparing `cy-root-1.0.1/cyroot/vector_derivative_approximation.cpp` & `cy-root-1.0.2/cyroot/vector_derivative_approximation.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
             "cyroot",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include",
             "cyroot/ops",
             "cyroot/utils"
         ],
         "language": "c++",
         "name": "cyroot.vector_derivative_approximation",
         "sources": [
             "cyroot/vector_derivative_approximation.pyx"
@@ -1177,195 +1177,195 @@
 
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
 
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1424,42 +1424,42 @@
 struct __pyx_obj_6cyroot_31vector_derivative_approximation_VectorDerivativeApproximation;
 struct __pyx_obj_6cyroot_31vector_derivative_approximation_GeneralizedFiniteDifference;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1542,28 +1542,28 @@
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_cisclose;
 
 /* "scalar_ops.pxd":18
  *     double complex
  * 
  * cdef bint isclose(double a, double b, double rtol=*, double atol=*) nogil             # <<<<<<<<<<<<<<
  * cdef bint cisclose(double complex a, double complex b, double rtol=*, double atol=*) nogil
- * 
+ * cdef real min(real a, real b) nogil
  */
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_isclose {
   int __pyx_n;
   double rtol;
   double atol;
 };
 
 /* "scalar_ops.pxd":19
  * 
  * cdef bint isclose(double a, double b, double rtol=*, double atol=*) nogil
  * cdef bint cisclose(double complex a, double complex b, double rtol=*, double atol=*) nogil             # <<<<<<<<<<<<<<
- * 
- * cdef extern from '<math.h>' nogil:
+ * cdef real min(real a, real b) nogil
+ * cdef real max(real a, real b) nogil
  */
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_cisclose {
   int __pyx_n;
   double rtol;
   double atol;
 };
 struct __pyx_opt_args_6cyroot_3ops_10vector_ops_allclose;
@@ -10958,15 +10958,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -10975,29 +10975,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -11008,15 +11008,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -11025,29 +11025,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -11058,15 +11058,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -11075,29 +11075,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -11108,15 +11108,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -11125,29 +11125,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -11158,15 +11158,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -11175,29 +11175,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -11208,212 +11208,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -11429,15 +11429,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -11445,53 +11445,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 942, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 944, __pyx_L5_except_error)
@@ -11499,30 +11499,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -11537,15 +11537,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11561,15 +11561,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -11577,53 +11577,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 948, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 950, __pyx_L5_except_error)
@@ -11631,30 +11631,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11669,15 +11669,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11693,15 +11693,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -11709,53 +11709,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 954, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 956, __pyx_L5_except_error)
@@ -11763,30 +11763,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11801,176 +11801,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -27159,26 +27159,26 @@
   __pyx_tuple__4 = PyTuple_Pack(3, __pyx_int_207065528, __pyx_int_70091267, __pyx_int_234301111); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
   __pyx_tuple__5 = PyTuple_Pack(3, __pyx_int_99694685, __pyx_int_139418775, __pyx_int_39425840); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(3, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(3, 950, __pyx_L1_error)
```

### Comparing `cy-root-1.0.1/cyroot/vector_derivative_approximation.pxd` & `cy-root-1.0.2/cyroot/vector_derivative_approximation.pxd`

 * *Files identical despite different names*

### Comparing `cy-root-1.0.1/cyroot/vector_derivative_approximation.pyx` & `cy-root-1.0.2/cyroot/vector_derivative_approximation.pyx`

 * *Files identical despite different names*

### Comparing `cy-root-1.0.1/cyroot/vector_newton.cpp` & `cy-root-1.0.2/cyroot/vector_newton.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
             "cyroot",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include",
             "cyroot/ops",
             "cyroot/utils"
         ],
         "language": "c++",
         "name": "cyroot.vector_newton",
         "sources": [
             "cyroot/vector_newton.pyx"
@@ -1167,195 +1167,195 @@
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
 #define __Pyx_FastGilFuncInit()
 
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1408,42 +1408,42 @@
 struct __pyx_obj_6cyroot_4fptr_CyNdArrayFPtr;
 struct __pyx_obj_6cyroot_4fptr_PyNdArrayFPtr;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1544,28 +1544,28 @@
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_cisclose;
 
 /* "scalar_ops.pxd":18
  *     double complex
  * 
  * cdef bint isclose(double a, double b, double rtol=*, double atol=*) nogil             # <<<<<<<<<<<<<<
  * cdef bint cisclose(double complex a, double complex b, double rtol=*, double atol=*) nogil
- * 
+ * cdef real min(real a, real b) nogil
  */
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_isclose {
   int __pyx_n;
   double rtol;
   double atol;
 };
 
 /* "scalar_ops.pxd":19
  * 
  * cdef bint isclose(double a, double b, double rtol=*, double atol=*) nogil
  * cdef bint cisclose(double complex a, double complex b, double rtol=*, double atol=*) nogil             # <<<<<<<<<<<<<<
- * 
- * cdef extern from '<math.h>' nogil:
+ * cdef real min(real a, real b) nogil
+ * cdef real max(real a, real b) nogil
  */
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_cisclose {
   int __pyx_n;
   double rtol;
   double atol;
 };
 struct __pyx_opt_args_6cyroot_3ops_10vector_ops_allclose;
@@ -12631,15 +12631,15 @@
   __Pyx_XDECREF(__pyx_v_prtol);
   __Pyx_XDECREF(__pyx_v_max_iter);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -12648,29 +12648,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -12681,15 +12681,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -12698,29 +12698,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -12731,15 +12731,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -12748,29 +12748,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -12781,15 +12781,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -12798,29 +12798,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -12831,15 +12831,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -12848,29 +12848,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -12881,212 +12881,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -13102,15 +13102,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -13118,53 +13118,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
@@ -13172,30 +13172,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -13210,15 +13210,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -13234,15 +13234,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -13250,53 +13250,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
@@ -13304,30 +13304,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -13342,15 +13342,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -13366,15 +13366,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -13382,53 +13382,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
@@ -13436,30 +13436,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -13474,176 +13474,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -27857,26 +27857,26 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__22);
   __Pyx_GIVEREF(__pyx_tuple__22);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(1, 950, __pyx_L1_error)
```

### Comparing `cy-root-1.0.1/cyroot/vector_newton.pyx` & `cy-root-1.0.2/cyroot/vector_newton.pyx`

 * *Files identical despite different names*

### Comparing `cy-root-1.0.1/cyroot/vector_quasi_newton.cpp` & `cy-root-1.0.2/cyroot/vector_quasi_newton.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
             "cyroot",
-            "/tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/core/include",
+            "/tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/core/include",
             "cyroot/ops",
             "cyroot/utils"
         ],
         "language": "c++",
         "name": "cyroot.vector_quasi_newton",
         "sources": [
             "cyroot/vector_quasi_newton.pyx"
@@ -1167,195 +1167,195 @@
 
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
 
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1408,42 +1408,42 @@
 struct __pyx_obj_6cyroot_4fptr_CyNdArrayFPtr;
 struct __pyx_obj_6cyroot_4fptr_PyNdArrayFPtr;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1544,28 +1544,28 @@
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_cisclose;
 
 /* "scalar_ops.pxd":18
  *     double complex
  * 
  * cdef bint isclose(double a, double b, double rtol=*, double atol=*) nogil             # <<<<<<<<<<<<<<
  * cdef bint cisclose(double complex a, double complex b, double rtol=*, double atol=*) nogil
- * 
+ * cdef real min(real a, real b) nogil
  */
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_isclose {
   int __pyx_n;
   double rtol;
   double atol;
 };
 
 /* "scalar_ops.pxd":19
  * 
  * cdef bint isclose(double a, double b, double rtol=*, double atol=*) nogil
  * cdef bint cisclose(double complex a, double complex b, double rtol=*, double atol=*) nogil             # <<<<<<<<<<<<<<
- * 
- * cdef extern from '<math.h>' nogil:
+ * cdef real min(real a, real b) nogil
+ * cdef real max(real a, real b) nogil
  */
 struct __pyx_opt_args_6cyroot_3ops_10scalar_ops_cisclose {
   int __pyx_n;
   double rtol;
   double atol;
 };
 struct __pyx_opt_args_6cyroot_3ops_10vector_ops_allclose;
@@ -16736,17 +16736,17 @@
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *(*__pyx_t_9)(PyObject *);
   int __pyx_t_10;
-  Py_ssize_t __pyx_t_11;
-  Py_UCS4 __pyx_t_12;
-  int __pyx_t_13;
+  int __pyx_t_11;
+  Py_ssize_t __pyx_t_12;
+  Py_UCS4 __pyx_t_13;
   double __pyx_t_14;
   double __pyx_t_15;
   double __pyx_t_16;
   double __pyx_t_17;
   unsigned long __pyx_t_18;
   struct __pyx_opt_args_6cyroot_19vector_quasi_newton_broyden1_kernel __pyx_t_19;
   struct __pyx_opt_args_6cyroot_19vector_quasi_newton_broyden2_kernel __pyx_t_20;
@@ -16931,91 +16931,126 @@
   }
 
   /* "cyroot/vector_quasi_newton.pyx":794
  *     if algo == 'good':
  *         algo = 1
  *     elif algo == 'bad':             # <<<<<<<<<<<<<<
  *         algo = 2
- *     else:
+ *     elif algo not in [1, 2]:
  */
   __pyx_t_10 = (__Pyx_PyUnicode_Equals(__pyx_v_algo, __pyx_n_u_bad, Py_EQ)); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 794, __pyx_L1_error)
-  if (likely(__pyx_t_10)) {
+  if (__pyx_t_10) {
 
     /* "cyroot/vector_quasi_newton.pyx":795
  *         algo = 1
  *     elif algo == 'bad':
  *         algo = 2             # <<<<<<<<<<<<<<
- *     else:
+ *     elif algo not in [1, 2]:
  *         raise ValueError('algo must be either 1/\'good\' or 2/\'bad\'. '
  */
     __Pyx_INCREF(__pyx_int_2);
     __Pyx_DECREF_SET(__pyx_v_algo, __pyx_int_2);
 
     /* "cyroot/vector_quasi_newton.pyx":794
  *     if algo == 'good':
  *         algo = 1
  *     elif algo == 'bad':             # <<<<<<<<<<<<<<
  *         algo = 2
- *     else:
+ *     elif algo not in [1, 2]:
  */
     goto __pyx_L5;
   }
 
-  /* "cyroot/vector_quasi_newton.pyx":797
+  /* "cyroot/vector_quasi_newton.pyx":796
+ *     elif algo == 'bad':
  *         algo = 2
- *     else:
+ *     elif algo not in [1, 2]:             # <<<<<<<<<<<<<<
+ *         raise ValueError('algo must be either 1/\'good\' or 2/\'bad\'. '
+ *                          f'Got {algo}.')
+ */
+  __Pyx_INCREF(__pyx_v_algo);
+  __pyx_t_1 = __pyx_v_algo;
+  __pyx_t_7 = __Pyx_PyInt_NeObjC(__pyx_t_1, __pyx_int_1, 1, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 796, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 796, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  if (__pyx_t_11) {
+  } else {
+    __pyx_t_10 = __pyx_t_11;
+    goto __pyx_L6_bool_binop_done;
+  }
+  __pyx_t_7 = __Pyx_PyInt_NeObjC(__pyx_t_1, __pyx_int_2, 2, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 796, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 796, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_10 = __pyx_t_11;
+  __pyx_L6_bool_binop_done:;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_11 = (__pyx_t_10 != 0);
+  if (unlikely(__pyx_t_11)) {
+
+    /* "cyroot/vector_quasi_newton.pyx":797
+ *         algo = 2
+ *     elif algo not in [1, 2]:
  *         raise ValueError('algo must be either 1/\'good\' or 2/\'bad\'. '             # <<<<<<<<<<<<<<
  *                          f'Got {algo}.')
  * 
  */
-  /*else*/ {
     __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 797, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_11 = 0;
-    __pyx_t_12 = 127;
+    __pyx_t_12 = 0;
+    __pyx_t_13 = 127;
     __Pyx_INCREF(__pyx_kp_u_algo_must_be_either_1_good_or_2);
-    __pyx_t_11 += 45;
+    __pyx_t_12 += 45;
     __Pyx_GIVEREF(__pyx_kp_u_algo_must_be_either_1_good_or_2);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_algo_must_be_either_1_good_or_2);
 
     /* "cyroot/vector_quasi_newton.pyx":798
- *     else:
+ *     elif algo not in [1, 2]:
  *         raise ValueError('algo must be either 1/\'good\' or 2/\'bad\'. '
  *                          f'Got {algo}.')             # <<<<<<<<<<<<<<
  * 
  *     x0 = np.asarray(x0, dtype=np.float64)
  */
     __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_v_algo, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 798, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_12 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_12) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_12;
-    __pyx_t_11 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
+    __pyx_t_13 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_13) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_13;
+    __pyx_t_12 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_kp_u__14);
-    __pyx_t_11 += 1;
+    __pyx_t_12 += 1;
     __Pyx_GIVEREF(__pyx_kp_u__14);
     PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u__14);
 
     /* "cyroot/vector_quasi_newton.pyx":797
  *         algo = 2
- *     else:
+ *     elif algo not in [1, 2]:
  *         raise ValueError('algo must be either 1/\'good\' or 2/\'bad\'. '             # <<<<<<<<<<<<<<
  *                          f'Got {algo}.')
  * 
  */
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_11, __pyx_t_12); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 797, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_12, __pyx_t_13); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 797, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 797, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __PYX_ERR(0, 797, __pyx_L1_error)
+
+    /* "cyroot/vector_quasi_newton.pyx":796
+ *     elif algo == 'bad':
+ *         algo = 2
+ *     elif algo not in [1, 2]:             # <<<<<<<<<<<<<<
+ *         raise ValueError('algo must be either 1/\'good\' or 2/\'bad\'. '
+ *                          f'Got {algo}.')
+ */
   }
   __pyx_L5:;
 
   /* "cyroot/vector_quasi_newton.pyx":800
  *                          f'Got {algo}.')
  * 
  *     x0 = np.asarray(x0, dtype=np.float64)             # <<<<<<<<<<<<<<
@@ -17064,17 +17099,17 @@
   /* "cyroot/vector_quasi_newton.pyx":803
  * 
  *     F_wrapper = PyNdArrayFPtr.from_f(F)
  *     if F_x0 is None:             # <<<<<<<<<<<<<<
  *         F_x0 = F_wrapper.eval(x0)
  *     else:
  */
-  __pyx_t_10 = (__pyx_v_F_x0 == Py_None);
-  __pyx_t_13 = (__pyx_t_10 != 0);
-  if (__pyx_t_13) {
+  __pyx_t_11 = (__pyx_v_F_x0 == Py_None);
+  __pyx_t_10 = (__pyx_t_11 != 0);
+  if (__pyx_t_10) {
 
     /* "cyroot/vector_quasi_newton.pyx":804
  *     F_wrapper = PyNdArrayFPtr.from_f(F)
  *     if F_x0 is None:
  *         F_x0 = F_wrapper.eval(x0)             # <<<<<<<<<<<<<<
  *     else:
  *         F_x0 = np.asarray(F_x0, dtype=np.float64)
@@ -17088,15 +17123,15 @@
     /* "cyroot/vector_quasi_newton.pyx":803
  * 
  *     F_wrapper = PyNdArrayFPtr.from_f(F)
  *     if F_x0 is None:             # <<<<<<<<<<<<<<
  *         F_x0 = F_wrapper.eval(x0)
  *     else:
  */
-    goto __pyx_L6;
+    goto __pyx_L8;
   }
 
   /* "cyroot/vector_quasi_newton.pyx":806
  *         F_x0 = F_wrapper.eval(x0)
  *     else:
  *         F_x0 = np.asarray(F_x0, dtype=np.float64)             # <<<<<<<<<<<<<<
  *     if J_x0 is None:
@@ -17126,26 +17161,26 @@
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_F_x0, __pyx_t_3);
     __pyx_t_3 = 0;
   }
-  __pyx_L6:;
+  __pyx_L8:;
 
   /* "cyroot/vector_quasi_newton.pyx":807
  *     else:
  *         F_x0 = np.asarray(F_x0, dtype=np.float64)
  *     if J_x0 is None:             # <<<<<<<<<<<<<<
  *         J_x0 = generalized_finite_difference(F_wrapper, x0, F_x0, h=h, order=1)
  *     else:
  */
-  __pyx_t_13 = (__pyx_v_J_x0 == Py_None);
-  __pyx_t_10 = (__pyx_t_13 != 0);
-  if (__pyx_t_10) {
+  __pyx_t_10 = (__pyx_v_J_x0 == Py_None);
+  __pyx_t_11 = (__pyx_t_10 != 0);
+  if (__pyx_t_11) {
 
     /* "cyroot/vector_quasi_newton.pyx":808
  *         F_x0 = np.asarray(F_x0, dtype=np.float64)
  *     if J_x0 is None:
  *         J_x0 = generalized_finite_difference(F_wrapper, x0, F_x0, h=h, order=1)             # <<<<<<<<<<<<<<
  *     else:
  *         J_x0 = np.asarray(J_x0, dtype=np.float64)
@@ -17178,15 +17213,15 @@
     /* "cyroot/vector_quasi_newton.pyx":807
  *     else:
  *         F_x0 = np.asarray(F_x0, dtype=np.float64)
  *     if J_x0 is None:             # <<<<<<<<<<<<<<
  *         J_x0 = generalized_finite_difference(F_wrapper, x0, F_x0, h=h, order=1)
  *     else:
  */
-    goto __pyx_L7;
+    goto __pyx_L9;
   }
 
   /* "cyroot/vector_quasi_newton.pyx":810
  *         J_x0 = generalized_finite_difference(F_wrapper, x0, F_x0, h=h, order=1)
  *     else:
  *         J_x0 = np.asarray(J_x0, dtype=np.float64)             # <<<<<<<<<<<<<<
  * 
@@ -17216,15 +17251,15 @@
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_J_x0, __pyx_t_7);
     __pyx_t_7 = 0;
   }
-  __pyx_L7:;
+  __pyx_L9:;
 
   /* "cyroot/vector_quasi_newton.pyx":812
  *         J_x0 = np.asarray(J_x0, dtype=np.float64)
  * 
  *     if x0.shape[0] < F_x0.shape[0]:             # <<<<<<<<<<<<<<
  *         warn_value('Input dimension is smaller than output dimension. '
  *                    f'Got n={x0.shape[0]}, m={F_x0.shape[0]}.')
@@ -17238,33 +17273,33 @@
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_t_6 = __Pyx_GetItemInt(__pyx_t_7, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 812, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_7 = PyObject_RichCompare(__pyx_t_1, __pyx_t_6, Py_LT); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 812, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 812, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 812, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (__pyx_t_10) {
+  if (__pyx_t_11) {
 
     /* "cyroot/vector_quasi_newton.pyx":813
  * 
  *     if x0.shape[0] < F_x0.shape[0]:
  *         warn_value('Input dimension is smaller than output dimension. '             # <<<<<<<<<<<<<<
  *                    f'Got n={x0.shape[0]}, m={F_x0.shape[0]}.')
  * 
  */
     __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_warn_value); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 813, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_1 = PyTuple_New(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 813, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_11 = 0;
-    __pyx_t_12 = 127;
+    __pyx_t_12 = 0;
+    __pyx_t_13 = 127;
     __Pyx_INCREF(__pyx_kp_u_Input_dimension_is_smaller_than_2);
-    __pyx_t_11 += 56;
+    __pyx_t_12 += 56;
     __Pyx_GIVEREF(__pyx_kp_u_Input_dimension_is_smaller_than_2);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_Input_dimension_is_smaller_than_2);
 
     /* "cyroot/vector_quasi_newton.pyx":814
  *     if x0.shape[0] < F_x0.shape[0]:
  *         warn_value('Input dimension is smaller than output dimension. '
  *                    f'Got n={x0.shape[0]}, m={F_x0.shape[0]}.')             # <<<<<<<<<<<<<<
@@ -17275,49 +17310,49 @@
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_5, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 814, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_3, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 814, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_12 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_12) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_12;
-    __pyx_t_11 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
+    __pyx_t_13 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_13) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_13;
+    __pyx_t_12 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_5);
     __pyx_t_5 = 0;
     __Pyx_INCREF(__pyx_kp_u_m);
-    __pyx_t_11 += 4;
+    __pyx_t_12 += 4;
     __Pyx_GIVEREF(__pyx_kp_u_m);
     PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u_m);
     __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_F_x0, __pyx_n_s_shape); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 814, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_5, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 814, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_3, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 814, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_12 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_12) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_12;
-    __pyx_t_11 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
+    __pyx_t_13 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_13) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_13;
+    __pyx_t_12 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_t_5);
     __pyx_t_5 = 0;
     __Pyx_INCREF(__pyx_kp_u__14);
-    __pyx_t_11 += 1;
+    __pyx_t_12 += 1;
     __Pyx_GIVEREF(__pyx_kp_u__14);
     PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_kp_u__14);
 
     /* "cyroot/vector_quasi_newton.pyx":813
  * 
  *     if x0.shape[0] < F_x0.shape[0]:
  *         warn_value('Input dimension is smaller than output dimension. '             # <<<<<<<<<<<<<<
  *                    f'Got n={x0.shape[0]}, m={F_x0.shape[0]}.')
  * 
  */
-    __pyx_t_5 = __Pyx_PyUnicode_Join(__pyx_t_1, 5, __pyx_t_11, __pyx_t_12); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 813, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyUnicode_Join(__pyx_t_1, 5, __pyx_t_12, __pyx_t_13); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 813, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_1)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -17348,17 +17383,17 @@
  * 
  *     if algo == 1:             # <<<<<<<<<<<<<<
  *         res = broyden1_kernel(
  *             F_wrapper, x0, F_x0, J_x0, etol, ertol, ptol, prtol, max_iter)
  */
   __pyx_t_7 = __Pyx_PyInt_EqObjC(__pyx_v_algo, __pyx_int_1, 1, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 816, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 816, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 816, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (__pyx_t_10) {
+  if (__pyx_t_11) {
 
     /* "cyroot/vector_quasi_newton.pyx":818
  *     if algo == 1:
  *         res = broyden1_kernel(
  *             F_wrapper, x0, F_x0, J_x0, etol, ertol, ptol, prtol, max_iter)             # <<<<<<<<<<<<<<
  *     else:
  *         res = broyden2_kernel(
@@ -17393,15 +17428,15 @@
     /* "cyroot/vector_quasi_newton.pyx":816
  *                    f'Got n={x0.shape[0]}, m={F_x0.shape[0]}.')
  * 
  *     if algo == 1:             # <<<<<<<<<<<<<<
  *         res = broyden1_kernel(
  *             F_wrapper, x0, F_x0, J_x0, etol, ertol, ptol, prtol, max_iter)
  */
-    goto __pyx_L9;
+    goto __pyx_L11;
   }
 
   /* "cyroot/vector_quasi_newton.pyx":820
  *             F_wrapper, x0, F_x0, J_x0, etol, ertol, ptol, prtol, max_iter)
  *     else:
  *         res = broyden2_kernel(             # <<<<<<<<<<<<<<
  *             F_wrapper, x0, F_x0, J_x0, False, etol, ertol, ptol, prtol, max_iter)
@@ -17440,15 +17475,15 @@
     __pyx_t_20.prtol = __pyx_t_14;
     __pyx_t_20.max_iter = __pyx_t_18;
     __pyx_t_7 = __pyx_f_6cyroot_19vector_quasi_newton_broyden2_kernel(__pyx_v_F_wrapper, ((PyArrayObject *)__pyx_v_x0), ((PyArrayObject *)__pyx_v_F_x0), ((PyArrayObject *)__pyx_v_J_x0), &__pyx_t_20); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 820, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_v_res = __pyx_t_7;
     __pyx_t_7 = 0;
   }
-  __pyx_L9:;
+  __pyx_L11:;
 
   /* "cyroot/vector_quasi_newton.pyx":822
  *         res = broyden2_kernel(
  *             F_wrapper, x0, F_x0, J_x0, False, etol, ertol, ptol, prtol, max_iter)
  *     return QuasiNewtonMethodReturnType.from_results(res, F_wrapper.n_f_calls)             # <<<<<<<<<<<<<<
  * 
  * ################################################################################
@@ -19404,15 +19439,15 @@
   __Pyx_XDECREF(__pyx_v_prtol);
   __Pyx_XDECREF(__pyx_v_max_iter);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -19421,29 +19456,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -19454,15 +19489,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -19471,29 +19506,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -19504,15 +19539,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -19521,29 +19556,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -19554,15 +19589,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -19571,29 +19606,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -19604,15 +19639,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -19621,29 +19656,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -19654,212 +19689,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19875,15 +19910,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -19891,53 +19926,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__48, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
@@ -19945,30 +19980,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19983,15 +20018,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -20007,15 +20042,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -20023,53 +20058,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__49, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
@@ -20077,30 +20112,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -20115,15 +20150,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -20139,15 +20174,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -20155,53 +20190,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__49, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
@@ -20209,30 +20244,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -20247,176 +20282,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -34784,26 +34819,26 @@
  *             if not np.allclose(b, 0, atol=eps, rtol=0):
  *                 basis[k] = b / vops.norm(b)
  */
   __pyx_tuple__27 = PyTuple_Pack(2, __pyx_int_neg_1, __pyx_int_1); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 439, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__27);
   __Pyx_GIVEREF(__pyx_tuple__27);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__48 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__48)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__48);
   __Pyx_GIVEREF(__pyx_tuple__48);
 
-  /* "../../../../../tmp/build-env-__9z6qp0/lib/python3.10/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-xwxp9lqc/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__49 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__49)) __PYX_ERR(1, 950, __pyx_L1_error)
```

### Comparing `cy-root-1.0.1/cyroot/vector_quasi_newton.pyx` & `cy-root-1.0.2/cyroot/vector_quasi_newton.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -789,15 +789,15 @@
     # check params
     etol, ertol, ptol, prtol, max_iter = _check_stop_cond_args(etol, ertol, ptol, prtol, max_iter)
 
     if algo == 'good':
         algo = 1
     elif algo == 'bad':
         algo = 2
-    else:
+    elif algo not in [1, 2]:
         raise ValueError('algo must be either 1/\'good\' or 2/\'bad\'. '
                          f'Got {algo}.')
 
     x0 = np.asarray(x0, dtype=np.float64)
 
     F_wrapper = PyNdArrayFPtr.from_f(F)
     if F_x0 is None:
```

### Comparing `cy-root-1.0.1/cyroot/vector_root.py` & `cy-root-1.0.2/cyroot/vector_root.py`

 * *Files identical despite different names*

### Comparing `cy-root-1.0.1/setup.cfg` & `cy-root-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `cy-root-1.0.1/setup.py` & `cy-root-1.0.2/setup.py`

 * *Files identical despite different names*

