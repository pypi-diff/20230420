# Comparing `tmp/vcorelib-1.5.2.tar.gz` & `tmp/vcorelib-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcorelib-1.5.2.tar", last modified: Mon Apr 10 05:37:49 2023, max compression
+gzip compressed data, was "vcorelib-1.6.0.tar", last modified: Thu Apr 20 06:18:34 2023, max compression
```

## Comparing `vcorelib-1.5.2.tar` & `vcorelib-1.6.0.tar`

### file list

```diff
@@ -1,91 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.056496 vcorelib-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-10 05:36:30.000000 vcorelib-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-10 05:37:49.056496 vcorelib-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-10 05:36:30.000000 vcorelib-1.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-10 05:36:30.000000 vcorelib-1.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 05:37:49.056496 vcorelib-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-10 05:36:30.000000 vcorelib-1.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.036496 vcorelib-1.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-10 05:36:30.000000 vcorelib-1.5.2/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-10 05:36:30.000000 vcorelib-1.5.2/tests/test_namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.036496 vcorelib-1.5.2/vcorelib/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.040495 vcorelib-1.5.2/vcorelib/args/
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/args/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/args/newline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.040495 vcorelib-1.5.2/vcorelib/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/asyncio/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/asyncio/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/dev_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.044495 vcorelib-1.5.2/vcorelib/dict/
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/dict/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/dict/codec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/dict/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/dict/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.044495 vcorelib-1.5.2/vcorelib/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/graph/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/graph/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/graph/port.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.044495 vcorelib-1.5.2/vcorelib/io/
--rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/io/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.044495 vcorelib-1.5.2/vcorelib/io/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/io/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/io/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/io/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/io/encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/io/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.048495 vcorelib-1.5.2/vcorelib/math/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/math/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.048495 vcorelib-1.5.2/vcorelib/math/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/math/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/math/analysis/average.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.048495 vcorelib-1.5.2/vcorelib/math/analysis/rate/
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/math/analysis/rate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/math/analysis/rate/limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/math/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.048495 vcorelib-1.5.2/vcorelib/paths/
--rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/paths/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/paths/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/paths/info_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.048495 vcorelib-1.5.2/vcorelib/platform/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.052496 vcorelib-1.5.2/vcorelib/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/schemas/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/schemas/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/schemas/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.052496 vcorelib-1.5.2/vcorelib/script/
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.052496 vcorelib-1.5.2/vcorelib/target/
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/target/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/target/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/target/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/target/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.052496 vcorelib-1.5.2/vcorelib/task/
--rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.052496 vcorelib-1.5.2/vcorelib/task/dict/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/task/dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/task/dict/melder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/task/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.052496 vcorelib-1.5.2/vcorelib/task/subprocess/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/task/subprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/task/subprocess/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.056496 vcorelib-1.5.2/vcorelib/task/time/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/task/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/task/time/sleep.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.040495 vcorelib-1.5.2/vcorelib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-10 05:37:49.000000 vcorelib-1.5.2/vcorelib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-10 05:37:49.000000 vcorelib-1.5.2/vcorelib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 05:37:49.000000 vcorelib-1.5.2/vcorelib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-10 05:37:49.000000 vcorelib-1.5.2/vcorelib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 05:37:49.000000 vcorelib-1.5.2/vcorelib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.417159 vcorelib-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-20 06:16:50.000000 vcorelib-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-20 06:18:34.417159 vcorelib-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-20 06:16:50.000000 vcorelib-1.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-20 06:16:50.000000 vcorelib-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 06:18:34.417159 vcorelib-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-20 06:16:50.000000 vcorelib-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.401159 vcorelib-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-20 06:16:50.000000 vcorelib-1.6.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-20 06:16:50.000000 vcorelib-1.6.0/tests/test_namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.405159 vcorelib-1.6.0/vcorelib/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.405159 vcorelib-1.6.0/vcorelib/args/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/args/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/args/newline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.405159 vcorelib-1.6.0/vcorelib/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/asyncio/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/asyncio/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/dev_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.405159 vcorelib-1.6.0/vcorelib/dict/
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/dict/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/dict/codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/dict/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/dict/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.409159 vcorelib-1.6.0/vcorelib/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/graph/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/graph/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/graph/port.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.409159 vcorelib-1.6.0/vcorelib/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/io/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.409159 vcorelib-1.6.0/vcorelib/io/arbiter/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/io/arbiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/io/arbiter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/io/arbiter/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/io/arbiter/directory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.409159 vcorelib-1.6.0/vcorelib/io/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/io/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/io/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/io/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/io/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/io/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/io/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.409159 vcorelib-1.6.0/vcorelib/math/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/math/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.409159 vcorelib-1.6.0/vcorelib/math/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/math/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/math/analysis/average.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.409159 vcorelib-1.6.0/vcorelib/math/analysis/rate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/math/analysis/rate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/math/analysis/rate/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/math/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.413159 vcorelib-1.6.0/vcorelib/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/paths/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/paths/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/paths/info_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.413159 vcorelib-1.6.0/vcorelib/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.413159 vcorelib-1.6.0/vcorelib/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/schemas/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/schemas/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/schemas/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.413159 vcorelib-1.6.0/vcorelib/script/
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.413159 vcorelib-1.6.0/vcorelib/target/
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/target/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/target/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/target/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/target/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.413159 vcorelib-1.6.0/vcorelib/task/
+-rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.413159 vcorelib-1.6.0/vcorelib/task/dict/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/task/dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/task/dict/melder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/task/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.413159 vcorelib-1.6.0/vcorelib/task/subprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/task/subprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/task/subprocess/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.417159 vcorelib-1.6.0/vcorelib/task/time/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/task/time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/task/time/sleep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.405159 vcorelib-1.6.0/vcorelib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-20 06:18:34.000000 vcorelib-1.6.0/vcorelib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-20 06:18:34.000000 vcorelib-1.6.0/vcorelib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 06:18:34.000000 vcorelib-1.6.0/vcorelib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-20 06:18:34.000000 vcorelib-1.6.0/vcorelib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 06:18:34.000000 vcorelib-1.6.0/vcorelib.egg-info/top_level.txt
```

### Comparing `vcorelib-1.5.2/LICENSE` & `vcorelib-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/PKG-INFO` & `vcorelib-1.6.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcorelib
-Version: 1.5.2
+Version: 1.6.0
 Summary: A collection of core Python utilities.
 Home-page: https://github.com/vkottler/vcorelib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=4f5dac9c4ed3066040913d4d4437e4bf
+    hash=39eb60bc0fed5235f1b3cfbf49e78c66
     =====================================
 -->
 
-# vcorelib ([1.5.2](https://pypi.org/project/vcorelib/))
+# vcorelib ([1.6.0](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-1.5.2/README.md` & `vcorelib-1.6.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=4f5dac9c4ed3066040913d4d4437e4bf
+    hash=39eb60bc0fed5235f1b3cfbf49e78c66
     =====================================
 -->
 
-# vcorelib ([1.5.2](https://pypi.org/project/vcorelib/))
+# vcorelib ([1.6.0](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-1.5.2/pyproject.toml` & `vcorelib-1.6.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "vcorelib"
-version = "1.5.2"
+version = "1.6.0"
 description = "A collection of core Python utilities."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `vcorelib-1.5.2/setup.py` & `vcorelib-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/tests/test_logging.py` & `vcorelib-1.6.0/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/tests/test_namespace.py` & `vcorelib-1.6.0/tests/test_namespace.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/args/__init__.py` & `vcorelib-1.6.0/vcorelib/args/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/args/newline.py` & `vcorelib-1.6.0/vcorelib/args/newline.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/asyncio/__init__.py` & `vcorelib-1.6.0/vcorelib/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/asyncio/cli.py` & `vcorelib-1.6.0/vcorelib/asyncio/cli.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/asyncio/subprocess.py` & `vcorelib-1.6.0/vcorelib/asyncio/subprocess.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/dict/__init__.py` & `vcorelib-1.6.0/vcorelib/dict/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """
 Dictionary manipulation utilities.
 """
 
-from contextlib import contextmanager as _contextmanager
-
 # built-in
+from contextlib import contextmanager as _contextmanager
 from enum import Enum as _Enum
 from enum import auto as _auto
-from logging import Logger, getLogger
+from logging import getLogger
 from typing import Any as _Any
 from typing import Dict as _Dict
 from typing import Iterator as _Iterator
 from typing import List as _List
 
+# internal
+from vcorelib.logging import LoggerType
+
 _LOG = getLogger(__name__)
 GenericDict = _Dict[_Any, _Any]
 GenericStrDict = _Dict[str, _Any]
 
 
 def consume(data: GenericDict, key: _Any, default: _Any = None) -> _Any:
     """
@@ -77,15 +79,16 @@
 
 
 def merge_recursive(
     dict_a: GenericDict,
     dict_b: GenericDict,
     path: _List[str] = None,
     expect_overwrite: bool = False,
-    logger: Logger = None,
+    logger: LoggerType = None,
+    strategy: MergeStrategy = MergeStrategy.RECURSIVE,
 ) -> GenericDict:
     """
     Combine two dictionaries recursively, prefers dict_a in a conflict. For
     values of the same key that are lists, the lists are combined. Otherwise
     the resulting dictionary is cleanly merged.
     """
 
@@ -112,14 +115,15 @@
         elif isinstance(dict_a[key], dict) and isinstance(right_val, dict):
             merge(
                 dict_a[key],
                 right_val,
                 path + [str(key)],
                 expect_overwrite,
                 logger,
+                strategy=strategy,
             )
         elif isinstance(dict_a[key], list) and isinstance(right_val, list):
             dict_a[key].extend(right_val)
         elif not isinstance(right_val, type(dict_a[key])):
             logger.error("Type mismatch at '%s'", ".".join(path + [str(key)]))
             logger.error("left:  %s (%s)", type(dict_a[key]), dict_a[key])
             logger.error("right: %s (%s)", type(right_val), right_val)
@@ -134,36 +138,37 @@
 
 
 def merge(
     dict_a: GenericDict,
     dict_b: GenericDict,
     path: _List[str] = None,
     expect_overwrite: bool = False,
-    logger: Logger = None,
+    logger: LoggerType = None,
     strategy: MergeStrategy = MergeStrategy.RECURSIVE,
 ) -> GenericDict:
     """Combine two dictionaries based on a provided merge strategy."""
 
     if strategy is MergeStrategy.UPDATE:
         dict_a.update(dict_b)
         return dict_a
 
     return merge_recursive(
         dict_a,
         dict_b,
         path=path,
         expect_overwrite=expect_overwrite,
         logger=logger,
+        strategy=strategy,
     )
 
 
 def merge_dicts(
     dicts: _List[GenericDict],
     expect_overwrite: bool = False,
-    logger: Logger = None,
+    logger: LoggerType = None,
     strategy: MergeStrategy = MergeStrategy.RECURSIVE,
 ) -> GenericDict:
     """
     Merge a list of dictionary data into a single set (mutates the first
     element).
     """
```

### Comparing `vcorelib-1.5.2/vcorelib/dict/cache.py` & `vcorelib-1.6.0/vcorelib/dict/cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/dict/codec.py` & `vcorelib-1.6.0/vcorelib/dict/codec.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/dict/config.py` & `vcorelib-1.6.0/vcorelib/dict/config.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/dict/env.py` & `vcorelib-1.6.0/vcorelib/dict/env.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/graph/__init__.py` & `vcorelib-1.6.0/vcorelib/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/graph/abc.py` & `vcorelib-1.6.0/vcorelib/graph/abc.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/graph/edge.py` & `vcorelib-1.6.0/vcorelib/graph/edge.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/graph/node.py` & `vcorelib-1.6.0/vcorelib/graph/node.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/graph/port.py` & `vcorelib-1.6.0/vcorelib/graph/port.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/io/abc.py` & `vcorelib-1.6.0/vcorelib/io/abc.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/io/archive/__init__.py` & `vcorelib-1.6.0/vcorelib/io/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/io/cache.py` & `vcorelib-1.6.0/vcorelib/io/cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/io/decode.py` & `vcorelib-1.6.0/vcorelib/io/decode.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,37 +2,38 @@
 A module implementing various data-file decoders.
 """
 
 # built-in
 from configparser import ConfigParser, Error, ExtendedInterpolation
 from json import load
 from json.decoder import JSONDecodeError
-from logging import Logger, getLogger
+from logging import getLogger
 from typing import cast as _cast
 
 # third-party
 from ruamel.yaml.parser import ParserError
 from ruamel.yaml.scanner import ScannerError
 from tomli import TOMLDecodeError, loads
 
 # internal
 from vcorelib.dict import consume
 from vcorelib.io.types import DataStream as _DataStream
 from vcorelib.io.types import JsonObject as _JsonObject
 from vcorelib.io.types import LoadResult
 from vcorelib.io.types import YAML_INTERFACE as _YAML_INTERFACE
+from vcorelib.logging import LoggerType
 from vcorelib.math.time import TIMER as _TIMER
 
 _LOG = getLogger(__name__)
 _INI_INTERPOLATION = ExtendedInterpolation()
 
 
 def decode_ini(
     data_file: _DataStream,
-    logger: Logger = _LOG,
+    logger: LoggerType = _LOG,
     **kwargs,
 ) -> LoadResult:
     """Load INI data from a text stream."""
 
     data = {}
     loaded = True
 
@@ -50,15 +51,15 @@
             logger.error("config-load error: %s", exc)
 
     return LoadResult(_cast(_JsonObject, data), loaded, _TIMER.result(token))
 
 
 def decode_json(
     data_file: _DataStream,
-    logger: Logger = _LOG,
+    logger: LoggerType = _LOG,
     **kwargs,
 ) -> LoadResult:
     """Load JSON data from a text stream."""
 
     data = {}
     loaded = True
 
@@ -72,15 +73,15 @@
             logger.error("json-load error: %s", exc)
 
     return LoadResult(data, loaded, _TIMER.result(token))
 
 
 def decode_yaml(
     data_file: _DataStream,
-    logger: Logger = _LOG,
+    logger: LoggerType = _LOG,
     **kwargs,
 ) -> LoadResult:
     """Load YAML data from a text stream."""
 
     data = {}
     loaded = True
 
@@ -94,15 +95,15 @@
             logger.error("yaml-load error: %s", exc)
 
     return LoadResult(data, loaded, _TIMER.result(token))
 
 
 def decode_toml(
     data_file: _DataStream,
-    logger: Logger = _LOG,
+    logger: LoggerType = _LOG,
     **kwargs,
 ) -> LoadResult:
     """Load TOML data from a text stream."""
 
     data = {}
     loaded = True
```

### Comparing `vcorelib-1.5.2/vcorelib/io/encode.py` & `vcorelib-1.6.0/vcorelib/io/encode.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 """
 A module implementing various data-file encoders.
 """
 
 # built-in
 from configparser import ConfigParser
 from json import dump
-from logging import Logger, getLogger
+from logging import getLogger
 from typing import cast as _cast
 
 # third-party
 from tomli_w import dumps
 
 # internal
 from vcorelib import DEFAULT_INDENT as _DEFAULT_INDENT
 from vcorelib.dict import GenericStrDict as _GenericStrDict
 from vcorelib.dict import consume
 from vcorelib.io.types import DataStream as _DataStream
 from vcorelib.io.types import JsonObject as _JsonObject
 from vcorelib.io.types import YAML_INTERFACE as _YAML_INTERFACE
+from vcorelib.logging import LoggerType
 from vcorelib.math.time import TIMER as _TIMER
 
 _LOG = getLogger(__name__)
 
 
 def encode_json(
-    configs: _JsonObject, ostream: _DataStream, _: Logger = _LOG, **kwargs
+    configs: _JsonObject, ostream: _DataStream, _: LoggerType = _LOG, **kwargs
 ) -> int:
     """Write config data as JSON to the output stream."""
 
     with _TIMER.measure_ns() as token:
         # Normalize arguments with some defaults.
         dump(
             configs,
@@ -37,38 +38,38 @@
             sort_keys=consume(kwargs, "sort_keys", True),
             **kwargs,
         )
     return _TIMER.result(token)
 
 
 def encode_yaml(
-    configs: _JsonObject, ostream: _DataStream, _: Logger = _LOG, **kwargs
+    configs: _JsonObject, ostream: _DataStream, _: LoggerType = _LOG, **kwargs
 ) -> int:
     """Write config data as YAML to the output stream."""
 
     with _TIMER.measure_ns() as token:
         _YAML_INTERFACE.dump(configs, ostream, **kwargs)
     return _TIMER.result(token)
 
 
 def encode_ini(
-    configs: _JsonObject, ostream: _DataStream, _: Logger = _LOG, **kwargs
+    configs: _JsonObject, ostream: _DataStream, _: LoggerType = _LOG, **kwargs
 ) -> int:
     """Write config data as INI to the output stream."""
 
     with _TIMER.measure_ns() as token:
         cparser = ConfigParser(
             interpolation=consume(kwargs, "interpolation"), **kwargs
         )
         cparser.read_dict(_cast(_GenericStrDict, configs))
         cparser.write(ostream)
     return _TIMER.result(token)
 
 
 def encode_toml(
-    configs: _JsonObject, ostream: _DataStream, _: Logger = _LOG, **kwargs
+    configs: _JsonObject, ostream: _DataStream, _: LoggerType = _LOG, **kwargs
 ) -> int:
     """Write config data as TOML to the output stream."""
 
     with _TIMER.measure_ns() as token:
         ostream.write(dumps(configs, **kwargs))
     return _TIMER.result(token)
```

### Comparing `vcorelib-1.5.2/vcorelib/io/types.py` & `vcorelib-1.6.0/vcorelib/io/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Common type definitions for data encoding and decoding interfaces.
 """
 
 # built-in
 from enum import Enum
 from io import StringIO
-from logging import Logger
 from pathlib import Path
 from typing import Callable as _Callable
 from typing import Dict as _Dict
 from typing import Iterator as _Iterator
 from typing import List as _List
 from typing import NamedTuple
 from typing import Optional as _Optional
@@ -18,14 +17,15 @@
 from typing import Union as _Union
 
 # third-party
 from ruamel.yaml import YAML
 
 # internal
 from vcorelib.dict import merge
+from vcorelib.logging import LoggerType
 from vcorelib.paths import Pathlike as _Pathlike
 from vcorelib.paths import get_file_ext
 
 DEFAULT_ARCHIVE_EXT = "tar.gz"
 DEFAULT_DATA_EXT = "json"
 
 # A simple type system for JSON.
@@ -164,31 +164,31 @@
         assert isinstance(other, (LoadResult, tuple))
         return bool(self.data == other[0] and self.success == other[1])
 
     def require_success(self, path: _Union[Path, str]) -> None:
         """Raise a canonical exception if this result is a failure."""
         assert self.success, f"Couldn't load '{path}'!"
 
-    def merge(self, other: "LoadResult") -> "LoadResult":
+    def merge(self, other: "LoadResult", **kwargs) -> "LoadResult":
         """Merge two load results."""
 
         # Add the time fields up if they're both positive.
         time_ns = self.time_ns
         if time_ns > 0 and other.time_ns > 0:
             time_ns += other.time_ns
 
         return LoadResult(
-            merge(self.data, other.data),
+            merge(self.data, other.data, **kwargs),
             self.success and other.success,
             time_ns,
         )
 
 
 EncodeResult = _Tuple[bool, int]
 DataStream = _Union[TextIO, StringIO]
 StreamProcessor = _Callable[[DataStream], DataStream]
-DataDecoder = _Callable[[DataStream, Logger], LoadResult]
-DataEncoder = _Callable[[JsonObject, DataStream, Logger], int]
+DataDecoder = _Callable[[DataStream, LoggerType], LoadResult]
+DataEncoder = _Callable[[JsonObject, DataStream, LoggerType], int]
 
 # Only create the interface one so it's not re-created on every read and write
 # attempt.
 YAML_INTERFACE = YAML(typ="safe")
```

### Comparing `vcorelib-1.5.2/vcorelib/logging.py` & `vcorelib-1.6.0/vcorelib/logging.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/math/__init__.py` & `vcorelib-1.6.0/vcorelib/math/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/math/analysis/average.py` & `vcorelib-1.6.0/vcorelib/math/analysis/average.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/math/analysis/rate/__init__.py` & `vcorelib-1.6.0/vcorelib/math/analysis/rate/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/math/analysis/rate/limiter.py` & `vcorelib-1.6.0/vcorelib/math/analysis/rate/limiter.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/math/time.py` & `vcorelib-1.6.0/vcorelib/math/time.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/namespace.py` & `vcorelib-1.6.0/vcorelib/namespace.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/paths/__init__.py` & `vcorelib-1.6.0/vcorelib/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/paths/context.py` & `vcorelib-1.6.0/vcorelib/paths/context.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/paths/info.py` & `vcorelib-1.6.0/vcorelib/paths/info.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/paths/info_cache.py` & `vcorelib-1.6.0/vcorelib/paths/info_cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/platform/__init__.py` & `vcorelib-1.6.0/vcorelib/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/schemas/__init__.py` & `vcorelib-1.6.0/vcorelib/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/schemas/base.py` & `vcorelib-1.6.0/vcorelib/schemas/base.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/schemas/json.py` & `vcorelib-1.6.0/vcorelib/schemas/json.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/schemas/mixins.py` & `vcorelib-1.6.0/vcorelib/schemas/mixins.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/script/__init__.py` & `vcorelib-1.6.0/vcorelib/script/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/target/__init__.py` & `vcorelib-1.6.0/vcorelib/target/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/target/evaluation.py` & `vcorelib-1.6.0/vcorelib/target/evaluation.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/target/expression.py` & `vcorelib-1.6.0/vcorelib/target/expression.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/target/resolver.py` & `vcorelib-1.6.0/vcorelib/target/resolver.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/task/__init__.py` & `vcorelib-1.6.0/vcorelib/task/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/task/dict/melder.py` & `vcorelib-1.6.0/vcorelib/task/dict/melder.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/task/manager.py` & `vcorelib-1.6.0/vcorelib/task/manager.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/task/subprocess/run.py` & `vcorelib-1.6.0/vcorelib/task/subprocess/run.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib/task/time/sleep.py` & `vcorelib-1.6.0/vcorelib/task/time/sleep.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.2/vcorelib.egg-info/PKG-INFO` & `vcorelib-1.6.0/vcorelib.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcorelib
-Version: 1.5.2
+Version: 1.6.0
 Summary: A collection of core Python utilities.
 Home-page: https://github.com/vkottler/vcorelib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=4f5dac9c4ed3066040913d4d4437e4bf
+    hash=39eb60bc0fed5235f1b3cfbf49e78c66
     =====================================
 -->
 
-# vcorelib ([1.5.2](https://pypi.org/project/vcorelib/))
+# vcorelib ([1.6.0](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-1.5.2/vcorelib.egg-info/SOURCES.txt` & `vcorelib-1.6.0/vcorelib.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -31,15 +31,20 @@
 vcorelib/graph/node.py
 vcorelib/graph/port.py
 vcorelib/io/__init__.py
 vcorelib/io/abc.py
 vcorelib/io/cache.py
 vcorelib/io/decode.py
 vcorelib/io/encode.py
+vcorelib/io/mapping.py
 vcorelib/io/types.py
+vcorelib/io/arbiter/__init__.py
+vcorelib/io/arbiter/base.py
+vcorelib/io/arbiter/context.py
+vcorelib/io/arbiter/directory.py
 vcorelib/io/archive/__init__.py
 vcorelib/math/__init__.py
 vcorelib/math/time.py
 vcorelib/math/analysis/__init__.py
 vcorelib/math/analysis/average.py
 vcorelib/math/analysis/rate/__init__.py
 vcorelib/math/analysis/rate/limiter.py
```

