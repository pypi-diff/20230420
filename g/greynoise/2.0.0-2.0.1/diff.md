# Comparing `tmp/greynoise-2.0.0.tar.gz` & `tmp/greynoise-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/greynoise-2.0.0.tar", last modified: Wed Feb 15 22:00:35 2023, max compression
+gzip compressed data, was "dist/greynoise-2.0.1.tar", last modified: Thu Apr 20 17:14:00 2023, max compression
```

## Comparing `greynoise-2.0.0.tar` & `greynoise-2.0.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-15 22:00:35.000000 greynoise-2.0.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9448 2023-02-15 22:00:13.000000 greynoise-2.0.0/CHANGELOG.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1052 2023-02-15 22:00:13.000000 greynoise-2.0.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-02-15 22:00:13.000000 greynoise-2.0.0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14061 2023-02-15 22:00:35.000000 greynoise-2.0.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3595 2023-02-15 22:00:13.000000 greynoise-2.0.0/README.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      281 2023-02-15 22:00:35.000000 greynoise-2.0.0/setup.cfg
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1921 2023-02-15 22:00:13.000000 greynoise-2.0.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-15 22:00:35.000000 greynoise-2.0.0/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-15 22:00:35.000000 greynoise-2.0.0/src/greynoise/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      266 2023-02-15 22:00:13.000000 greynoise-2.0.0/src/greynoise/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      255 2023-02-15 22:00:13.000000 greynoise-2.0.0/src/greynoise/__version__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-15 22:00:35.000000 greynoise-2.0.0/src/greynoise/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26445 2023-02-15 22:00:13.000000 greynoise-2.0.0/src/greynoise/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5623 2023-02-15 22:00:13.000000 greynoise-2.0.0/src/greynoise/api/analyzer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4933 2023-02-15 22:00:13.000000 greynoise-2.0.0/src/greynoise/api/filter.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-15 22:00:35.000000 greynoise-2.0.0/src/greynoise/cli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      620 2023-02-15 22:00:13.000000 greynoise-2.0.0/src/greynoise/cli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7575 2023-02-15 22:00:13.000000 greynoise-2.0.0/src/greynoise/cli/decorator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6994 2023-02-15 22:00:13.000000 greynoise-2.0.0/src/greynoise/cli/formatter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2366 2023-02-15 22:00:13.000000 greynoise-2.0.0/src/greynoise/cli/helper.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      797 2023-02-15 22:00:13.000000 greynoise-2.0.0/src/greynoise/cli/parameter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11508 2023-02-15 22:00:13.000000 greynoise-2.0.0/src/greynoise/cli/subcommand.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-15 22:00:35.000000 greynoise-2.0.0/src/greynoise/cli/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      973 2023-02-15 22:00:13.000000 greynoise-2.0.0/src/greynoise/cli/templates/analyze.txt.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      732 2023-02-15 22:00:13.000000 greynoise-2.0.0/src/greynoise/cli/templates/gnql_query.txt.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      267 2023-02-15 22:00:13.000000 greynoise-2.0.0/src/greynoise/cli/templates/gnql_stats.txt.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      123 2023-02-15 22:00:13.000000 greynoise-2.0.0/src/greynoise/cli/templates/interesting.txt.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      679 2023-02-15 22:00:13.000000 greynoise-2.0.0/src/greynoise/cli/templates/ip_community.txt.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      210 2023-02-15 22:00:13.000000 greynoise-2.0.0/src/greynoise/cli/templates/ip_context.txt.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3075 2023-02-15 22:00:13.000000 greynoise-2.0.0/src/greynoise/cli/templates/ip_context_result.txt.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2720 2023-02-15 22:00:13.000000 greynoise-2.0.0/src/greynoise/cli/templates/ip_multi_context.txt.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-02-15 22:00:13.000000 greynoise-2.0.0/src/greynoise/cli/templates/ip_quick_check.txt.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4412 2023-02-15 22:00:13.000000 greynoise-2.0.0/src/greynoise/cli/templates/macros.txt.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1461 2023-02-15 22:00:13.000000 greynoise-2.0.0/src/greynoise/cli/templates/riot.txt.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1751 2023-02-15 22:00:13.000000 greynoise-2.0.0/src/greynoise/cli/templates/similarity.txt.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1597 2023-02-15 22:00:13.000000 greynoise-2.0.0/src/greynoise/cli/templates/stats.txt.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1002 2023-02-15 22:00:13.000000 greynoise-2.0.0/src/greynoise/cli/templates/timeline.txt.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1098 2023-02-15 22:00:13.000000 greynoise-2.0.0/src/greynoise/cli/templates/timelinehourly.txt.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      258 2023-02-15 22:00:13.000000 greynoise-2.0.0/src/greynoise/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7428 2023-02-15 22:00:13.000000 greynoise-2.0.0/src/greynoise/util.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-15 22:00:35.000000 greynoise-2.0.0/src/greynoise.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14061 2023-02-15 22:00:35.000000 greynoise-2.0.0/src/greynoise.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1393 2023-02-15 22:00:35.000000 greynoise-2.0.0/src/greynoise.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-02-15 22:00:35.000000 greynoise-2.0.0/src/greynoise.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-02-15 22:00:35.000000 greynoise-2.0.0/src/greynoise.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-02-15 22:00:34.000000 greynoise-2.0.0/src/greynoise.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2023-02-15 22:00:35.000000 greynoise-2.0.0/src/greynoise.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-02-15 22:00:35.000000 greynoise-2.0.0/src/greynoise.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 17:14:00.000000 greynoise-2.0.1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9925 2023-04-20 17:13:39.000000 greynoise-2.0.1/CHANGELOG.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1052 2023-04-20 17:13:39.000000 greynoise-2.0.1/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-04-20 17:13:39.000000 greynoise-2.0.1/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14538 2023-04-20 17:14:00.000000 greynoise-2.0.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3595 2023-04-20 17:13:39.000000 greynoise-2.0.1/README.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      281 2023-04-20 17:14:00.000000 greynoise-2.0.1/setup.cfg
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1921 2023-04-20 17:13:39.000000 greynoise-2.0.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 17:14:00.000000 greynoise-2.0.1/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 17:14:00.000000 greynoise-2.0.1/src/greynoise/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      266 2023-04-20 17:13:39.000000 greynoise-2.0.1/src/greynoise/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      255 2023-04-20 17:13:39.000000 greynoise-2.0.1/src/greynoise/__version__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 17:14:00.000000 greynoise-2.0.1/src/greynoise/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26445 2023-04-20 17:13:39.000000 greynoise-2.0.1/src/greynoise/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5623 2023-04-20 17:13:39.000000 greynoise-2.0.1/src/greynoise/api/analyzer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4933 2023-04-20 17:13:39.000000 greynoise-2.0.1/src/greynoise/api/filter.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 17:14:00.000000 greynoise-2.0.1/src/greynoise/cli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      620 2023-04-20 17:13:39.000000 greynoise-2.0.1/src/greynoise/cli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7575 2023-04-20 17:13:39.000000 greynoise-2.0.1/src/greynoise/cli/decorator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6994 2023-04-20 17:13:39.000000 greynoise-2.0.1/src/greynoise/cli/formatter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2366 2023-04-20 17:13:39.000000 greynoise-2.0.1/src/greynoise/cli/helper.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      797 2023-04-20 17:13:39.000000 greynoise-2.0.1/src/greynoise/cli/parameter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11508 2023-04-20 17:13:39.000000 greynoise-2.0.1/src/greynoise/cli/subcommand.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 17:14:00.000000 greynoise-2.0.1/src/greynoise/cli/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      973 2023-04-20 17:13:39.000000 greynoise-2.0.1/src/greynoise/cli/templates/analyze.txt.j2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      732 2023-04-20 17:13:39.000000 greynoise-2.0.1/src/greynoise/cli/templates/gnql_query.txt.j2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      267 2023-04-20 17:13:39.000000 greynoise-2.0.1/src/greynoise/cli/templates/gnql_stats.txt.j2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      123 2023-04-20 17:13:39.000000 greynoise-2.0.1/src/greynoise/cli/templates/interesting.txt.j2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      679 2023-04-20 17:13:39.000000 greynoise-2.0.1/src/greynoise/cli/templates/ip_community.txt.j2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      210 2023-04-20 17:13:39.000000 greynoise-2.0.1/src/greynoise/cli/templates/ip_context.txt.j2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3075 2023-04-20 17:13:39.000000 greynoise-2.0.1/src/greynoise/cli/templates/ip_context_result.txt.j2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2720 2023-04-20 17:13:39.000000 greynoise-2.0.1/src/greynoise/cli/templates/ip_multi_context.txt.j2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-04-20 17:13:39.000000 greynoise-2.0.1/src/greynoise/cli/templates/ip_quick_check.txt.j2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4412 2023-04-20 17:13:39.000000 greynoise-2.0.1/src/greynoise/cli/templates/macros.txt.j2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1461 2023-04-20 17:13:39.000000 greynoise-2.0.1/src/greynoise/cli/templates/riot.txt.j2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1751 2023-04-20 17:13:39.000000 greynoise-2.0.1/src/greynoise/cli/templates/similarity.txt.j2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1597 2023-04-20 17:13:39.000000 greynoise-2.0.1/src/greynoise/cli/templates/stats.txt.j2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1002 2023-04-20 17:13:39.000000 greynoise-2.0.1/src/greynoise/cli/templates/timeline.txt.j2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1098 2023-04-20 17:13:39.000000 greynoise-2.0.1/src/greynoise/cli/templates/timelinehourly.txt.j2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      258 2023-04-20 17:13:39.000000 greynoise-2.0.1/src/greynoise/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7428 2023-04-20 17:13:39.000000 greynoise-2.0.1/src/greynoise/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 17:14:00.000000 greynoise-2.0.1/src/greynoise.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14538 2023-04-20 17:14:00.000000 greynoise-2.0.1/src/greynoise.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1393 2023-04-20 17:14:00.000000 greynoise-2.0.1/src/greynoise.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-20 17:14:00.000000 greynoise-2.0.1/src/greynoise.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-04-20 17:14:00.000000 greynoise-2.0.1/src/greynoise.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-20 17:13:59.000000 greynoise-2.0.1/src/greynoise.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2023-04-20 17:14:00.000000 greynoise-2.0.1/src/greynoise.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-04-20 17:14:00.000000 greynoise-2.0.1/src/greynoise.egg-info/top_level.txt
```

### Comparing `greynoise-2.0.0/CHANGELOG.rst` & `greynoise-2.0.1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,30 @@
 =========
 Changelog
 =========
 
+Version `2.0.1`_
+================
+**Date**: April 14, 2023
+
+* API client:
+
+  * Updated timeline commands to support 90 day lookback period
+
+* CLI:
+
+  * Updated timeline commands to support 90 day lookback period
+
+* Dependencies:
+
+  * Updated ansimarkup to version 1.5.0
+  * Updated dict2xml to version 1.7.3
+  * Updated itertools to version 9.1.0
+  * Updated requests to version 2.28.2
+
 Version `2.0.0`_
 ================
 **Date**: February 15, 2023
 
 * BREAKING CHANGE:
 
   * Removed support for python 3.5
@@ -339,7 +358,8 @@
 .. _`0.9.1`: https://github.com/GreyNoise-Intelligence/pygreynoise/compare/v0.9.0...0.9.1
 .. _`1.0.0`: https://github.com/GreyNoise-Intelligence/pygreynoise/compare/v0.9.1...1.0.0
 .. _`1.1.0`: https://github.com/GreyNoise-Intelligence/pygreynoise/compare/v1.0.0...1.1.0
 .. _`1.2.0`: https://github.com/GreyNoise-Intelligence/pygreynoise/compare/v1.1.0...1.2.0
 .. _`1.2.1`: https://github.com/GreyNoise-Intelligence/pygreynoise/compare/v1.2.0...1.2.1
 .. _`1.3.0`: https://github.com/GreyNoise-Intelligence/pygreynoise/compare/v1.2.1...1.3.0
 .. _`2.0.0`: https://github.com/GreyNoise-Intelligence/pygreynoise/compare/v1.3.0...HEAD
+.. _`2.0.1`: https://github.com/GreyNoise-Intelligence/pygreynoise/compare/v2.0.0...2.0.1
```

### Comparing `greynoise-2.0.0/LICENSE` & `greynoise-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `greynoise-2.0.0/PKG-INFO` & `greynoise-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: greynoise
-Version: 2.0.0
+Version: 2.0.1
 Summary: Abstraction to interact with GreyNoise API.
 Home-page: https://greynoise.io/
 Download-URL: https://github.com/GreyNoise-Intelligence/pygreynoise
 Author: GreyNoise Intelligence
 Author-email: hello@greynoise.io
 License: MIT
 Keywords: internet,scanning,threat intelligence,security
@@ -120,14 +120,33 @@
 
 
 
 =========
 Changelog
 =========
 
+Version `2.0.1`_
+================
+**Date**: April 14, 2023
+
+* API client:
+
+  * Updated timeline commands to support 90 day lookback period
+
+* CLI:
+
+  * Updated timeline commands to support 90 day lookback period
+
+* Dependencies:
+
+  * Updated ansimarkup to version 1.5.0
+  * Updated dict2xml to version 1.7.3
+  * Updated itertools to version 9.1.0
+  * Updated requests to version 2.28.2
+
 Version `2.0.0`_
 ================
 **Date**: February 15, 2023
 
 * BREAKING CHANGE:
 
   * Removed support for python 3.5
@@ -461,7 +480,8 @@
 .. _`0.9.1`: https://github.com/GreyNoise-Intelligence/pygreynoise/compare/v0.9.0...0.9.1
 .. _`1.0.0`: https://github.com/GreyNoise-Intelligence/pygreynoise/compare/v0.9.1...1.0.0
 .. _`1.1.0`: https://github.com/GreyNoise-Intelligence/pygreynoise/compare/v1.0.0...1.1.0
 .. _`1.2.0`: https://github.com/GreyNoise-Intelligence/pygreynoise/compare/v1.1.0...1.2.0
 .. _`1.2.1`: https://github.com/GreyNoise-Intelligence/pygreynoise/compare/v1.2.0...1.2.1
 .. _`1.3.0`: https://github.com/GreyNoise-Intelligence/pygreynoise/compare/v1.2.1...1.3.0
 .. _`2.0.0`: https://github.com/GreyNoise-Intelligence/pygreynoise/compare/v1.3.0...HEAD
+.. _`2.0.1`: https://github.com/GreyNoise-Intelligence/pygreynoise/compare/v2.0.0...2.0.1
```

### Comparing `greynoise-2.0.0/README.rst` & `greynoise-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `greynoise-2.0.0/setup.py` & `greynoise-2.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "more-itertools",
     "requests",
     "six",
 ]
 
 setup(
     name="greynoise",
-    version="2.0.0",
+    version="2.0.1",
     description="Abstraction to interact with GreyNoise API.",
     url="https://greynoise.io/",
     author="GreyNoise Intelligence",
     author_email="hello@greynoise.io",
     license="MIT",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
```

### Comparing `greynoise-2.0.0/src/greynoise/api/__init__.py` & `greynoise-2.0.1/src/greynoise/api/__init__.py`

 * *Files identical despite different names*

### Comparing `greynoise-2.0.0/src/greynoise/api/analyzer.py` & `greynoise-2.0.1/src/greynoise/api/analyzer.py`

 * *Files identical despite different names*

### Comparing `greynoise-2.0.0/src/greynoise/api/filter.py` & `greynoise-2.0.1/src/greynoise/api/filter.py`

 * *Files identical despite different names*

### Comparing `greynoise-2.0.0/src/greynoise/cli/__init__.py` & `greynoise-2.0.1/src/greynoise/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `greynoise-2.0.0/src/greynoise/cli/decorator.py` & `greynoise-2.0.1/src/greynoise/cli/decorator.py`

 * *Files identical despite different names*

### Comparing `greynoise-2.0.0/src/greynoise/cli/formatter.py` & `greynoise-2.0.1/src/greynoise/cli/formatter.py`

 * *Files identical despite different names*

### Comparing `greynoise-2.0.0/src/greynoise/cli/helper.py` & `greynoise-2.0.1/src/greynoise/cli/helper.py`

 * *Files identical despite different names*

### Comparing `greynoise-2.0.0/src/greynoise/cli/parameter.py` & `greynoise-2.0.1/src/greynoise/cli/parameter.py`

 * *Files identical despite different names*

### Comparing `greynoise-2.0.0/src/greynoise/cli/subcommand.py` & `greynoise-2.0.1/src/greynoise/cli/subcommand.py`

 * *Files identical despite different names*

### Comparing `greynoise-2.0.0/src/greynoise/cli/templates/analyze.txt.j2` & `greynoise-2.0.1/src/greynoise/cli/templates/analyze.txt.j2`

 * *Files identical despite different names*

### Comparing `greynoise-2.0.0/src/greynoise/cli/templates/gnql_query.txt.j2` & `greynoise-2.0.1/src/greynoise/cli/templates/gnql_query.txt.j2`

 * *Files identical despite different names*

### Comparing `greynoise-2.0.0/src/greynoise/cli/templates/ip_community.txt.j2` & `greynoise-2.0.1/src/greynoise/cli/templates/ip_community.txt.j2`

 * *Files identical despite different names*

### Comparing `greynoise-2.0.0/src/greynoise/cli/templates/ip_context_result.txt.j2` & `greynoise-2.0.1/src/greynoise/cli/templates/ip_context_result.txt.j2`

 * *Files identical despite different names*

### Comparing `greynoise-2.0.0/src/greynoise/cli/templates/ip_multi_context.txt.j2` & `greynoise-2.0.1/src/greynoise/cli/templates/ip_multi_context.txt.j2`

 * *Files identical despite different names*

### Comparing `greynoise-2.0.0/src/greynoise/cli/templates/ip_quick_check.txt.j2` & `greynoise-2.0.1/src/greynoise/cli/templates/ip_quick_check.txt.j2`

 * *Files identical despite different names*

### Comparing `greynoise-2.0.0/src/greynoise/cli/templates/macros.txt.j2` & `greynoise-2.0.1/src/greynoise/cli/templates/macros.txt.j2`

 * *Files identical despite different names*

### Comparing `greynoise-2.0.0/src/greynoise/cli/templates/riot.txt.j2` & `greynoise-2.0.1/src/greynoise/cli/templates/riot.txt.j2`

 * *Files identical despite different names*

### Comparing `greynoise-2.0.0/src/greynoise/cli/templates/similarity.txt.j2` & `greynoise-2.0.1/src/greynoise/cli/templates/similarity.txt.j2`

 * *Files identical despite different names*

### Comparing `greynoise-2.0.0/src/greynoise/cli/templates/stats.txt.j2` & `greynoise-2.0.1/src/greynoise/cli/templates/stats.txt.j2`

 * *Files identical despite different names*

### Comparing `greynoise-2.0.0/src/greynoise/cli/templates/timeline.txt.j2` & `greynoise-2.0.1/src/greynoise/cli/templates/timeline.txt.j2`

 * *Files identical despite different names*

### Comparing `greynoise-2.0.0/src/greynoise/cli/templates/timelinehourly.txt.j2` & `greynoise-2.0.1/src/greynoise/cli/templates/timelinehourly.txt.j2`

 * *Files identical despite different names*

### Comparing `greynoise-2.0.0/src/greynoise/util.py` & `greynoise-2.0.1/src/greynoise/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,21 +186,21 @@
 
     :param days: field value to validate.
     :type days: str
 
     """
     if isinstance(days, str):
         raise ValueError(
-            "Days must be a valid integer between 1 and 30.  Current input is a "
+            "Days must be a valid integer between 1 and 90.  Current input is a "
             "string."
         )
-    if isinstance(days, int) and 1 <= int(days) <= 30:
+    if isinstance(days, int) and 1 <= int(days) <= 90:
         return True
     else:
-        raise ValueError("Days must be a valid integer between 1 and 30.")
+        raise ValueError("Days must be a valid integer between 1 and 90.")
 
 
 def validate_timeline_granularity(granularity):
     """Check if the Timeline granularity value is valid.
 
     :param granularity: field value to validate.
     :type granularity: str
```

### Comparing `greynoise-2.0.0/src/greynoise.egg-info/PKG-INFO` & `greynoise-2.0.1/src/greynoise.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: greynoise
-Version: 2.0.0
+Version: 2.0.1
 Summary: Abstraction to interact with GreyNoise API.
 Home-page: https://greynoise.io/
 Download-URL: https://github.com/GreyNoise-Intelligence/pygreynoise
 Author: GreyNoise Intelligence
 Author-email: hello@greynoise.io
 License: MIT
 Keywords: internet,scanning,threat intelligence,security
@@ -120,14 +120,33 @@
 
 
 
 =========
 Changelog
 =========
 
+Version `2.0.1`_
+================
+**Date**: April 14, 2023
+
+* API client:
+
+  * Updated timeline commands to support 90 day lookback period
+
+* CLI:
+
+  * Updated timeline commands to support 90 day lookback period
+
+* Dependencies:
+
+  * Updated ansimarkup to version 1.5.0
+  * Updated dict2xml to version 1.7.3
+  * Updated itertools to version 9.1.0
+  * Updated requests to version 2.28.2
+
 Version `2.0.0`_
 ================
 **Date**: February 15, 2023
 
 * BREAKING CHANGE:
 
   * Removed support for python 3.5
@@ -461,7 +480,8 @@
 .. _`0.9.1`: https://github.com/GreyNoise-Intelligence/pygreynoise/compare/v0.9.0...0.9.1
 .. _`1.0.0`: https://github.com/GreyNoise-Intelligence/pygreynoise/compare/v0.9.1...1.0.0
 .. _`1.1.0`: https://github.com/GreyNoise-Intelligence/pygreynoise/compare/v1.0.0...1.1.0
 .. _`1.2.0`: https://github.com/GreyNoise-Intelligence/pygreynoise/compare/v1.1.0...1.2.0
 .. _`1.2.1`: https://github.com/GreyNoise-Intelligence/pygreynoise/compare/v1.2.0...1.2.1
 .. _`1.3.0`: https://github.com/GreyNoise-Intelligence/pygreynoise/compare/v1.2.1...1.3.0
 .. _`2.0.0`: https://github.com/GreyNoise-Intelligence/pygreynoise/compare/v1.3.0...HEAD
+.. _`2.0.1`: https://github.com/GreyNoise-Intelligence/pygreynoise/compare/v2.0.0...2.0.1
```

### Comparing `greynoise-2.0.0/src/greynoise.egg-info/SOURCES.txt` & `greynoise-2.0.1/src/greynoise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

