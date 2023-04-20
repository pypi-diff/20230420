# Comparing `tmp/yace-0.5.4.tar.gz` & `tmp/yace-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yace-0.5.4.tar", last modified: Wed Mar 29 14:54:36 2023, max compression
+gzip compressed data, was "dist/yace-0.5.6.tar", last modified: Thu Apr 20 13:43:07 2023, max compression
```

## Comparing `yace-0.5.4.tar` & `yace-0.5.6.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:54:36.000000 yace-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-03-29 14:54:36.000000 yace-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-03-29 14:52:08.000000 yace-0.5.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-03-29 14:52:08.000000 yace-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 14:54:36.000000 yace-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-03-29 14:52:08.000000 yace-0.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:54:36.000000 yace-0.5.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:54:36.000000 yace-0.5.4/src/yace/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:54:36.000000 yace-0.5.4/src/yace/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3329 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/cli/yace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/emitters.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:54:36.000000 yace-0.5.4/src/yace/idl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/idl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/idl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/idl/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9279 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/idl/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/idl/derivedtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/idl/formater.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/idl/functiontypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     9841 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/idl/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/idl/linter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:54:36.000000 yace-0.5.4/src/yace/targets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/targets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:54:36.000000 yace-0.5.4/src/yace/targets/capi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/targets/capi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/targets/capi/clang-format-c.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/targets/capi/clang-format-h.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)    82299 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/targets/capi/doxygen.template
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/targets/capi/entity_define.h.template
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/targets/capi/entity_enum.h.template
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/targets/capi/entity_fun.h.template
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/targets/capi/entity_struct.h.template
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/targets/capi/file_bundle.h.template
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/targets/capi/file_check.c.template
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/targets/capi/file_core.h.template
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/targets/capi/file_pp.c.template
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/targets/capi/file_pp.h.template
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/targets/capi/target.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/targets/capi/typespec.h.template
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/targets/capi/typespec_anon.h.template
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/targets/collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:54:36.000000 yace-0.5.4/src/yace/targets/ctypes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/targets/ctypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/targets/ctypes/ctypes_sugar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/targets/ctypes/file_api.template
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/targets/ctypes/file_check.template
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/targets/ctypes/target.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/targets/ctypes/typespec.template
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/targets/ctypes/typespec_anon.template
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/targets/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-03-29 14:52:08.000000 yace-0.5.4/src/yace/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:54:36.000000 yace-0.5.4/src/yace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-03-29 14:54:36.000000 yace-0.5.4/src/yace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-03-29 14:54:36.000000 yace-0.5.4/src/yace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 14:54:36.000000 yace-0.5.4/src/yace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-29 14:54:36.000000 yace-0.5.4/src/yace.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 14:54:07.000000 yace-0.5.4/src/yace.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 14:54:36.000000 yace-0.5.4/src/yace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-29 14:54:36.000000 yace-0.5.4/src/yace.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:43:07.000000 yace-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-20 13:43:07.000000 yace-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-20 13:40:26.000000 yace-0.5.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-20 13:40:26.000000 yace-0.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-20 13:43:07.000000 yace-0.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 13:40:26.000000 yace-0.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:43:07.000000 yace-0.5.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:43:07.000000 yace-0.5.6/src/yace/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:43:07.000000 yace-0.5.6/src/yace/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3329 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/cli/yace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/emitters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:43:07.000000 yace-0.5.6/src/yace/idl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/idl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/idl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/idl/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9279 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/idl/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/idl/derivedtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/idl/formater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/idl/functiontypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10145 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/idl/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/idl/linter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:43:07.000000 yace-0.5.6/src/yace/targets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/targets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:43:07.000000 yace-0.5.6/src/yace/targets/capi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/targets/capi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/targets/capi/clang-format-c.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/targets/capi/clang-format-h.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)    82299 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/targets/capi/doxygen.template
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/targets/capi/entity_define.h.template
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/targets/capi/entity_enum.h.template
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/targets/capi/entity_fun.h.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/targets/capi/entity_struct.h.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/targets/capi/file_bundle.h.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/targets/capi/file_check.c.template
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/targets/capi/file_core.h.template
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/targets/capi/file_pp.c.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/targets/capi/file_pp.h.template
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/targets/capi/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/targets/capi/typespec.h.template
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/targets/capi/typespec_anon.h.template
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/targets/collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:43:07.000000 yace-0.5.6/src/yace/targets/ctypes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/targets/ctypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/targets/ctypes/ctypes_sugar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/targets/ctypes/file_api.template
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/targets/ctypes/file_check.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/targets/ctypes/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/targets/ctypes/typespec.template
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/targets/ctypes/typespec_anon.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/targets/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-20 13:40:26.000000 yace-0.5.6/src/yace/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:43:07.000000 yace-0.5.6/src/yace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-20 13:43:07.000000 yace-0.5.6/src/yace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-20 13:43:07.000000 yace-0.5.6/src/yace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 13:43:07.000000 yace-0.5.6/src/yace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-20 13:43:07.000000 yace-0.5.6/src/yace.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 13:42:38.000000 yace-0.5.6/src/yace.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-20 13:43:07.000000 yace-0.5.6/src/yace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-20 13:43:07.000000 yace-0.5.6/src/yace.egg-info/top_level.txt
```

### Comparing `yace-0.5.4/PKG-INFO` & `yace-0.5.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: yace
-Version: 0.5.4
-Summary: UNKNOWN
+Version: 0.5.6
+Summary: Yet Another Code Emitter / Your Artisinal Code Emitter / yace
 Home-page: https://github.com/safl/yace
 Author: Simon A. F. Lund
 Author-email: os@safl.dk
+Maintainer: Simon A. F. Lund
+Maintainer-email: os@safl.dk
 License: GPL-2.0
 Description: .. image:: docs/source/_static/yace-mascot.png
            :alt: yace
         
         Welcome to yace
         ===============
         
@@ -52,9 +54,8 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

### Comparing `yace-0.5.4/README.rst` & `yace-0.5.6/README.rst`

 * *Files identical despite different names*

### Comparing `yace-0.5.4/src/yace/cli/yace.py` & `yace-0.5.6/src/yace/cli/yace.py`

 * *Files identical despite different names*

### Comparing `yace-0.5.4/src/yace/compiler.py` & `yace-0.5.6/src/yace/compiler.py`

 * *Files identical despite different names*

### Comparing `yace-0.5.4/src/yace/emitters.py` & `yace-0.5.6/src/yace/emitters.py`

 * *Files identical despite different names*

### Comparing `yace-0.5.4/src/yace/errors.py` & `yace-0.5.6/src/yace/errors.py`

 * *Files identical despite different names*

### Comparing `yace-0.5.4/src/yace/idl/base.py` & `yace-0.5.6/src/yace/idl/base.py`

 * *Files identical despite different names*

### Comparing `yace-0.5.4/src/yace/idl/constants.py` & `yace-0.5.6/src/yace/idl/constants.py`

 * *Files identical despite different names*

### Comparing `yace-0.5.4/src/yace/idl/datatypes.py` & `yace-0.5.6/src/yace/idl/datatypes.py`

 * *Files identical despite different names*

### Comparing `yace-0.5.4/src/yace/idl/derivedtypes.py` & `yace-0.5.6/src/yace/idl/derivedtypes.py`

 * *Files identical despite different names*

### Comparing `yace-0.5.4/src/yace/idl/formater.py` & `yace-0.5.6/src/yace/idl/formater.py`

 * *Files identical despite different names*

### Comparing `yace-0.5.4/src/yace/idl/functiontypes.py` & `yace-0.5.6/src/yace/idl/functiontypes.py`

 * *Files identical despite different names*

### Comparing `yace-0.5.4/src/yace/idl/generator.py` & `yace-0.5.6/src/yace/idl/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 
 In this specific instance, to parse C Headers, and emit equivalent
 **Yace**-files.
 
 * :class:`.CParser`, parse a C header and emit a **Yace**-file
 """
 import logging as log
+import os
 import re
 from pathlib import Path
 
 import typing
+import clang
 from clang.cindex import Config, CursorKind, Index
 import yace.idl.datatypes
 from yace.idl.formater import ydata_to_file
 
 
 REGEX_INTEGER_FIXEDWIDTH = "(?P<unsigned>u?)int(?P<width>8|16|32|64|128)_t"
 
@@ -185,17 +187,24 @@
     """
     Primitive wrapper around libclang Python bindings
     """
 
     def __init__(self):
         """Figure out a way to setup the index..."""
 
-        Config().set_library_path("/Library/Developer/CommandLineTools/usr/lib/")
-        index = Index.create()
-        self.index = index
+        searchpath = print(os.environ.get("YACE_SEARCHPATH_LIBCLANG"))
+        if not searchpath:
+            for path in Path(clang.__file__).resolve().parent.rglob("*libclang.*"):
+                if path.suffix in [".dylib", ".so"]:
+                    searchpath = str(path.parent)
+                    break
+        if searchpath:
+            Config().set_library_path(searchpath)
+
+        self.index = Index.create()
 
     def parse_file(self, path: Path):
         """Parse the given file into a :class:`clang.cindex.TranslationUnit`."""
 
         return self.index.parse(path)
 
     def parse_enum(self, cursor, data):
```

### Comparing `yace-0.5.4/src/yace/idl/linter.py` & `yace-0.5.6/src/yace/idl/linter.py`

 * *Files identical despite different names*

### Comparing `yace-0.5.4/src/yace/model.py` & `yace-0.5.6/src/yace/model.py`

 * *Files identical despite different names*

### Comparing `yace-0.5.4/src/yace/targets/capi/doxygen.template` & `yace-0.5.6/src/yace/targets/capi/doxygen.template`

 * *Files identical despite different names*

### Comparing `yace-0.5.4/src/yace/targets/capi/entity_struct.h.template` & `yace-0.5.6/src/yace/targets/capi/entity_struct.h.template`

 * *Files identical despite different names*

### Comparing `yace-0.5.4/src/yace/targets/capi/file_bundle.h.template` & `yace-0.5.6/src/yace/targets/capi/file_bundle.h.template`

 * *Files identical despite different names*

### Comparing `yace-0.5.4/src/yace/targets/capi/file_check.c.template` & `yace-0.5.6/src/yace/targets/capi/file_check.c.template`

 * *Files identical despite different names*

### Comparing `yace-0.5.4/src/yace/targets/capi/file_core.h.template` & `yace-0.5.6/src/yace/targets/capi/file_core.h.template`

 * *Files identical despite different names*

### Comparing `yace-0.5.4/src/yace/targets/capi/file_pp.c.template` & `yace-0.5.6/src/yace/targets/capi/file_pp.c.template`

 * *Files identical despite different names*

### Comparing `yace-0.5.4/src/yace/targets/capi/file_pp.h.template` & `yace-0.5.6/src/yace/targets/capi/file_pp.h.template`

 * *Files identical despite different names*

### Comparing `yace-0.5.4/src/yace/targets/capi/target.py` & `yace-0.5.6/src/yace/targets/capi/target.py`

 * *Files identical despite different names*

### Comparing `yace-0.5.4/src/yace/targets/capi/typespec.h.template` & `yace-0.5.6/src/yace/targets/capi/typespec.h.template`

 * *Files identical despite different names*

### Comparing `yace-0.5.4/src/yace/targets/collector.py` & `yace-0.5.6/src/yace/targets/collector.py`

 * *Files identical despite different names*

### Comparing `yace-0.5.4/src/yace/targets/ctypes/ctypes_sugar.py` & `yace-0.5.6/src/yace/targets/ctypes/ctypes_sugar.py`

 * *Files identical despite different names*

### Comparing `yace-0.5.4/src/yace/targets/ctypes/file_api.template` & `yace-0.5.6/src/yace/targets/ctypes/file_api.template`

 * *Files identical despite different names*

### Comparing `yace-0.5.4/src/yace/targets/ctypes/target.py` & `yace-0.5.6/src/yace/targets/ctypes/target.py`

 * *Files identical despite different names*

### Comparing `yace-0.5.4/src/yace/targets/ctypes/typespec.template` & `yace-0.5.6/src/yace/targets/ctypes/typespec.template`

 * *Files identical despite different names*

### Comparing `yace-0.5.4/src/yace/targets/ctypes/typespec_anon.template` & `yace-0.5.6/src/yace/targets/ctypes/typespec_anon.template`

 * *Files identical despite different names*

### Comparing `yace-0.5.4/src/yace/targets/target.py` & `yace-0.5.6/src/yace/targets/target.py`

 * *Files identical despite different names*

### Comparing `yace-0.5.4/src/yace/tools.py` & `yace-0.5.6/src/yace/tools.py`

 * *Files identical despite different names*

### Comparing `yace-0.5.4/src/yace/transformations.py` & `yace-0.5.6/src/yace/transformations.py`

 * *Files identical despite different names*

### Comparing `yace-0.5.4/src/yace.egg-info/PKG-INFO` & `yace-0.5.6/src/yace.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: yace
-Version: 0.5.4
-Summary: UNKNOWN
+Version: 0.5.6
+Summary: Yet Another Code Emitter / Your Artisinal Code Emitter / yace
 Home-page: https://github.com/safl/yace
 Author: Simon A. F. Lund
 Author-email: os@safl.dk
+Maintainer: Simon A. F. Lund
+Maintainer-email: os@safl.dk
 License: GPL-2.0
 Description: .. image:: docs/source/_static/yace-mascot.png
            :alt: yace
         
         Welcome to yace
         ===============
         
@@ -52,9 +54,8 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

### Comparing `yace-0.5.4/src/yace.egg-info/SOURCES.txt` & `yace-0.5.6/src/yace.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 README.rst
 pyproject.toml
+setup.cfg
 setup.py
 src/yace/__init__.py
 src/yace/__main__.py
 src/yace/compiler.py
 src/yace/emitters.py
 src/yace/errors.py
 src/yace/model.py
```

